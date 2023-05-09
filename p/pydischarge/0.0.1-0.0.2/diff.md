# Comparing `tmp/pydischarge-0.0.1.tar.gz` & `tmp/pydischarge-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydischarge-0.0.1.tar", last modified: Tue May  9 15:29:38 2023, max compression
+gzip compressed data, was "pydischarge-0.0.2.tar", last modified: Tue May  9 15:49:33 2023, max compression
```

## Comparing `pydischarge-0.0.1.tar` & `pydischarge-0.0.2.tar`

### file list

```diff
@@ -1,437 +1,437 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:38.146230 pydischarge-0.0.1/
--rw-rw-rw-   0        0        0       31 2023-05-02 22:41:13.000000 pydischarge-0.0.1/.gitattributes
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.050230 pydischarge-0.0.1/.github/
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.146233 pydischarge-0.0.1/.github/workflows/
--rw-rw-rw-   0        0        0     5293 2023-05-02 22:41:16.000000 pydischarge-0.0.1/.github/workflows/conda.yml
--rw-rw-rw-   0        0        0     3030 2023-05-02 22:41:16.000000 pydischarge-0.0.1/.github/workflows/dependencies.yml
--rw-rw-rw-   0        0        0     3258 2023-05-02 22:41:16.000000 pydischarge-0.0.1/.github/workflows/dist.yml
--rw-rw-rw-   0        0        0      737 2023-05-09 14:05:20.000000 pydischarge-0.0.1/.github/workflows/documentation.yml
--rw-rw-rw-   0        0        0     1481 2023-05-02 15:35:55.000000 pydischarge-0.0.1/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      798 2023-05-09 14:02:25.000000 pydischarge-0.0.1/.gitignore
--rw-rw-rw-   0        0        0      135 2023-05-02 22:40:46.000000 pydischarge-0.0.1/CODE_OF_CONDUCT.rst
--rw-rw-rw-   0        0        0     4610 2023-05-02 22:41:13.000000 pydischarge-0.0.1/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    35821 2023-05-02 15:35:55.000000 pydischarge-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      181 2023-05-02 22:41:13.000000 pydischarge-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3282 2023-05-09 15:29:38.145233 pydischarge-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1882 2023-05-03 12:40:07.000000 pydischarge-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.169230 pydischarge-0.0.1/docs/
--rw-rw-rw-   0        0        0      818 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.175231 pydischarge-0.0.1/docs/_static/
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.178230 pydischarge-0.0.1/docs/_static/css/
--rw-rw-rw-   0        0        0     1331 2023-05-02 22:40:51.000000 pydischarge-0.0.1/docs/_static/css/gwpy-sphinx.css
--rw-rw-rw-   0        0        0   174729 2023-05-09 13:06:08.000000 pydischarge-0.0.1/docs/_static/favicon.png
--rw-rw-rw-   0        0        0    15166 2023-05-02 15:35:55.000000 pydischarge-0.0.1/docs/_static/gwpy_white_24.png
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.054230 pydischarge-0.0.1/docs/_templates/
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.180231 pydischarge-0.0.1/docs/_templates/autoclass/
--rw-rw-rw-   0        0        0      915 2023-05-02 15:35:55.000000 pydischarge-0.0.1/docs/_templates/autoclass/class.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.187232 pydischarge-0.0.1/docs/_templates/autosummary/
--rw-rw-rw-   0        0        0      180 2023-05-02 15:35:55.000000 pydischarge-0.0.1/docs/_templates/autosummary/base.rst
--rw-rw-rw-   0        0        0     1210 2023-05-02 15:35:55.000000 pydischarge-0.0.1/docs/_templates/autosummary/class.rst
--rw-rw-rw-   0        0        0      744 2023-05-02 15:35:55.000000 pydischarge-0.0.1/docs/_templates/autosummary/module.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.189230 pydischarge-0.0.1/docs/astro/
--rw-rw-rw-   0        0        0      762 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/astro/index.rst
--rw-rw-rw-   0        0        0     2742 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/citing.rst.in
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.195229 pydischarge-0.0.1/docs/cli/
--rw-rw-rw-   0        0        0     5499 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/cli/examples.ini
--rw-rw-rw-   0        0        0     2959 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/cli/index.rst
--rw-rw-rw-   0        0        0    13804 2023-05-03 12:41:15.000000 pydischarge-0.0.1/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.197229 pydischarge-0.0.1/docs/detector/
--rw-rw-rw-   0        0        0     3337 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/detector/channel.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.200230 pydischarge-0.0.1/docs/dev/
--rw-rw-rw-   0        0        0     3963 2023-05-03 12:42:16.000000 pydischarge-0.0.1/docs/dev/release.rst
--rw-rw-rw-   0        0        0     1662 2023-05-02 22:40:51.000000 pydischarge-0.0.1/docs/env.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.061230 pydischarge-0.0.1/docs/examples/
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.203235 pydischarge-0.0.1/docs/examples/table/
--rw-rw-rw-   0        0        0       61 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.213233 pydischarge-0.0.1/docs/external/
--rw-rw-rw-   0        0        0     1192 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/external/framecpp.rst
--rw-rw-rw-   0        0        0     1020 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/external/framel.rst
--rw-rw-rw-   0        0        0     3240 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/external/lalsuite.rst
--rw-rw-rw-   0        0        0     1051 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/external/nds2.rst
--rw-rw-rw-   0        0        0     2604 2023-05-02 23:01:25.000000 pydischarge-0.0.1/docs/index.rst
--rw-rw-rw-   0        0        0     1370 2023-05-02 22:47:43.000000 pydischarge-0.0.1/docs/install.rst
--rw-rw-rw-   0        0        0     2755 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/overview.rst
--rw-rw-rw-   0        0        0    67943 2023-05-09 13:03:59.000000 pydischarge-0.0.1/docs/pdpy-docs-logo.png
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.234231 pydischarge-0.0.1/docs/plot/
--rw-rw-rw-   0        0        0     2688 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/plot/colorbars.rst
--rw-rw-rw-   0        0        0     3075 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/plot/colors.rst
--rw-rw-rw-   0        0        0      792 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/plot/filter.rst
--rw-rw-rw-   0        0        0     2611 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/plot/gps.rst
--rw-rw-rw-   0        0        0     3212 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/plot/index.rst
--rw-rw-rw-   0        0        0     1901 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/plot/legend.rst
--rw-rw-rw-   0        0        0     1406 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/plot/log.rst
--rw-rw-rw-   0        0        0     5073 2023-05-03 12:41:28.000000 pydischarge-0.0.1/docs/references.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.246229 pydischarge-0.0.1/docs/segments/
--rw-rw-rw-   0        0        0     1556 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/segments/dqsegdb.rst
--rw-rw-rw-   0        0        0     7057 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/segments/index.rst
--rw-rw-rw-   0        0        0     6929 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/segments/io.rst
--rw-rw-rw-   0        0        0     2156 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/segments/thresholding.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.249229 pydischarge-0.0.1/docs/signal/
--rw-rw-rw-   0        0        0     4503 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/signal/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.251230 pydischarge-0.0.1/docs/spectrogram/
--rw-rw-rw-   0        0        0     3876 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/spectrogram/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.258231 pydischarge-0.0.1/docs/spectrum/
--rw-rw-rw-   0        0        0      524 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/spectrum/filtering.rst
--rw-rw-rw-   0        0        0     3847 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/spectrum/index.rst
--rw-rw-rw-   0        0        0     5127 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/spectrum/io.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.278229 pydischarge-0.0.1/docs/table/
--rw-rw-rw-   0        0        0       58 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/table/H1-LDAS_STRAIN-968654552-10.xml.gz
--rw-rw-rw-   0        0        0     7527 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/table/filter.rst
--rw-rw-rw-   0        0        0      985 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/table/histogram.rst
--rw-rw-rw-   0        0        0     1575 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/table/index.rst
--rw-rw-rw-   0        0        0    31225 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/table/io.rst
--rw-rw-rw-   0        0        0     1809 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/table/plot.rst
--rw-rw-rw-   0        0        0     2207 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/table/rate.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.280232 pydischarge-0.0.1/docs/time/
--rw-rw-rw-   0        0        0     1127 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/time/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.295232 pydischarge-0.0.1/docs/timeseries/
--rw-rw-rw-   0        0        0    11907 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/timeseries/datafind.rst
--rw-rw-rw-   0        0        0     2833 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/timeseries/index.rst
--rw-rw-rw-   0        0        0    11004 2023-05-03 12:42:34.000000 pydischarge-0.0.1/docs/timeseries/io.rst
--rw-rw-rw-   0        0        0     2811 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/timeseries/opendata.rst
--rw-rw-rw-   0        0        0     3136 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/timeseries/plot.rst
--rw-rw-rw-   0        0        0     8699 2023-05-02 22:41:16.000000 pydischarge-0.0.1/docs/timeseries/statevector.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.298231 pydischarge-0.0.1/examples/
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.317229 pydischarge-0.0.1/examples/frequencyseries/
--rw-rw-rw-   0        0        0     2650 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/frequencyseries/coherence.py
--rw-rw-rw-   0        0        0     2119 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/frequencyseries/hoff.py
--rw-rw-rw-   0        0        0      275 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/frequencyseries/index.rst
--rw-rw-rw-   0        0        0     2656 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/frequencyseries/inject.py
--rw-rw-rw-   0        0        0     2875 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/frequencyseries/percentiles.py
--rw-rw-rw-   0        0        0     2872 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/frequencyseries/rayleigh.py
--rw-rw-rw-   0        0        0     2266 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/frequencyseries/transfer_function.py
--rw-rw-rw-   0        0        0     2694 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/frequencyseries/variance.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.328230 pydischarge-0.0.1/examples/miscellaneous/
--rw-rw-rw-   0        0        0      229 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/miscellaneous/index.rst
--rw-rw-rw-   0        0        0     3425 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/miscellaneous/open-data-spectrogram.py
--rw-rw-rw-   0        0        0     2414 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/miscellaneous/range-spectrogram.py
--rw-rw-rw-   0        0        0     2540 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/miscellaneous/range-timeseries.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.333229 pydischarge-0.0.1/examples/segments/
--rw-rw-rw-   0        0        0      169 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/segments/index.rst
--rw-rw-rw-   0        0        0     2464 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/segments/open-data.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.339229 pydischarge-0.0.1/examples/signal/
--rw-rw-rw-   0        0        0     5787 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/signal/gw150914.py
--rw-rw-rw-   0        0        0      191 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/signal/index.rst
--rw-rw-rw-   0        0        0     3230 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/signal/qscan.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.354230 pydischarge-0.0.1/examples/spectrogram/
--rw-rw-rw-   0        0        0     2454 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/spectrogram/coherence.py
--rw-rw-rw-   0        0        0      224 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/spectrogram/index.rst
--rw-rw-rw-   0        0        0     2691 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/spectrogram/plot.py
--rw-rw-rw-   0        0        0     2648 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/spectrogram/ratio.py
--rw-rw-rw-   0        0        0     2177 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/spectrogram/rayleigh.py
--rw-rw-rw-   0        0        0     2958 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/spectrogram/spectrogram2.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.372230 pydischarge-0.0.1/examples/table/
--rw-rw-rw-   0        0        0       58 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
--rw-rw-rw-   0        0        0     1646 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/table/histogram.py
--rw-rw-rw-   0        0        0      213 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/table/index.rst
--rw-rw-rw-   0        0        0     2375 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/table/rate.py
--rw-rw-rw-   0        0        0     2522 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/table/rate_binned.py
--rw-rw-rw-   0        0        0     2084 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/table/scatter.py
--rw-rw-rw-   0        0        0     2344 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/table/tiles.py
--rw-rw-rw-   0        0        0     3874 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/test_examples.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.399229 pydischarge-0.0.1/examples/timeseries/
--rw-rw-rw-   0        0        0     2637 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/timeseries/blrms.py
--rw-rw-rw-   0        0        0     4314 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/timeseries/correlate.py
--rw-rw-rw-   0        0        0     2869 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/timeseries/filter.py
--rw-rw-rw-   0        0        0      265 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/timeseries/index.rst
--rw-rw-rw-   0        0        0     2698 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/timeseries/inject.py
--rw-rw-rw-   0        0        0     2531 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/timeseries/public.py
--rw-rw-rw-   0        0        0     3883 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/timeseries/pycbc-snr.py
--rw-rw-rw-   0        0        0     2669 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/timeseries/qscan.py
--rw-rw-rw-   0        0        0     2260 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/timeseries/statevector.py
--rw-rw-rw-   0        0        0     2537 2023-05-02 22:41:16.000000 pydischarge-0.0.1/examples/timeseries/whiten.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.411229 pydischarge-0.0.1/pdpy/
--rw-rw-rw-   0        0        0     1574 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/__init__.py
--rw-rw-rw-   0        0        0      164 2023-05-09 15:29:35.000000 pydischarge-0.0.1/pdpy/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.416230 pydischarge-0.0.1/pdpy/astro/
--rw-rw-rw-   0        0        0     1967 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/astro/__init__.py
--rw-rw-rw-   0        0        0    25633 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/astro/range.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.421230 pydischarge-0.0.1/pdpy/astro/tests/
--rw-rw-rw-   0        0        0      766 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/astro/tests/__init__.py
--rw-rw-rw-   0        0        0     6248 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/astro/tests/test_range.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.447231 pydischarge-0.0.1/pdpy/cli/
--rw-rw-rw-   0        0        0     1449 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/cli/__init__.py
--rw-rw-rw-   0        0        0    36278 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/cli/cliproduct.py
--rw-rw-rw-   0        0        0     4179 2023-05-02 22:40:50.000000 pydischarge-0.0.1/pdpy/cli/coherence.py
--rw-rw-rw-   0        0        0     3454 2023-05-02 22:40:50.000000 pydischarge-0.0.1/pdpy/cli/coherencegram.py
--rw-rw-rw-   0        0        0     5288 2023-05-03 12:42:43.000000 pydischarge-0.0.1/pdpy/cli/gwpy_plot.py
--rw-rw-rw-   0        0        0     9404 2023-05-02 22:40:50.000000 pydischarge-0.0.1/pdpy/cli/qtransform.py
--rw-rw-rw-   0        0        0     7342 2023-05-02 22:40:50.000000 pydischarge-0.0.1/pdpy/cli/spectrogram.py
--rw-rw-rw-   0        0        0     5070 2023-05-02 22:40:50.000000 pydischarge-0.0.1/pdpy/cli/spectrum.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.474232 pydischarge-0.0.1/pdpy/cli/tests/
--rw-rw-rw-   0        0        0      764 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/cli/tests/__init__.py
--rw-rw-rw-   0        0        0    11169 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/cli/tests/base.py
--rw-rw-rw-   0        0        0     1392 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/cli/tests/test_coherence.py
--rw-rw-rw-   0        0        0     1625 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/cli/tests/test_coherencegram.py
--rw-rw-rw-   0        0        0     1775 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/cli/tests/test_gwpy_plot.py
--rw-rw-rw-   0        0        0     2984 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/cli/tests/test_qtransform.py
--rw-rw-rw-   0        0        0     1556 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/cli/tests/test_spectrogram.py
--rw-rw-rw-   0        0        0     1459 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/cli/tests/test_spectrum.py
--rw-rw-rw-   0        0        0     1315 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/cli/tests/test_timeseries.py
--rw-rw-rw-   0        0        0     2057 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/cli/tests/test_transferfunction.py
--rw-rw-rw-   0        0        0     4113 2023-05-02 22:40:50.000000 pydischarge-0.0.1/pdpy/cli/timeseries.py
--rw-rw-rw-   0        0        0    10080 2023-05-02 22:40:50.000000 pydischarge-0.0.1/pdpy/cli/transferfunction.py
--rw-rw-rw-   0        0        0     1695 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/conftest.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.482233 pydischarge-0.0.1/pdpy/detector/
--rw-rw-rw-   0        0        0     2330 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/detector/__init__.py
--rw-rw-rw-   0        0        0    27781 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/detector/channel.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.492232 pydischarge-0.0.1/pdpy/detector/io/
--rw-rw-rw-   0        0        0     1065 2023-05-02 22:40:50.000000 pydischarge-0.0.1/pdpy/detector/io/__init__.py
--rw-rw-rw-   0        0        0     3296 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/detector/io/cis.py
--rw-rw-rw-   0        0        0     5860 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/detector/io/clf.py
--rw-rw-rw-   0        0        0     6124 2023-05-02 22:40:50.000000 pydischarge-0.0.1/pdpy/detector/io/omega.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.500229 pydischarge-0.0.1/pdpy/detector/tests/
--rw-rw-rw-   0        0        0      769 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/detector/tests/__init__.py
--rw-rw-rw-   0        0        0    19024 2023-05-02 22:40:50.000000 pydischarge-0.0.1/pdpy/detector/tests/test_channel.py
--rw-rw-rw-   0        0        0     2629 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/detector/tests/test_units.py
--rw-rw-rw-   0        0        0     7319 2023-05-02 22:41:14.000000 pydischarge-0.0.1/pdpy/detector/units.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.510231 pydischarge-0.0.1/pdpy/frequencyseries/
--rw-rw-rw-   0        0        0     1024 2023-05-02 22:40:49.000000 pydischarge-0.0.1/pdpy/frequencyseries/__init__.py
--rw-rw-rw-   0        0        0     2009 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/frequencyseries/_fdcommon.py
--rw-rw-rw-   0        0        0    14781 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/frequencyseries/frequencyseries.py
--rw-rw-rw-   0        0        0    12308 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/frequencyseries/hist.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.519230 pydischarge-0.0.1/pdpy/frequencyseries/io/
--rw-rw-rw-   0        0        0      935 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/frequencyseries/io/__init__.py
--rw-rw-rw-   0        0        0     1099 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/frequencyseries/io/ascii.py
--rw-rw-rw-   0        0        0     1064 2023-05-02 22:40:50.000000 pydischarge-0.0.1/pdpy/frequencyseries/io/hdf5.py
--rw-rw-rw-   0        0        0     1179 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/frequencyseries/io/ligolw.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.527232 pydischarge-0.0.1/pdpy/frequencyseries/tests/
--rw-rw-rw-   0        0        0      776 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/frequencyseries/tests/__init__.py
--rw-rw-rw-   0        0        0    11357 2023-05-02 22:40:50.000000 pydischarge-0.0.1/pdpy/frequencyseries/tests/test_frequencyseries.py
--rw-rw-rw-   0        0        0     4134 2023-05-02 22:40:50.000000 pydischarge-0.0.1/pdpy/frequencyseries/tests/test_hist.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.562232 pydischarge-0.0.1/pdpy/io/
--rw-rw-rw-   0        0        0      853 2023-05-02 22:40:48.000000 pydischarge-0.0.1/pdpy/io/__init__.py
--rw-rw-rw-   0        0        0     4366 2023-05-02 22:40:48.000000 pydischarge-0.0.1/pdpy/io/_framecpp.py
--rw-rw-rw-   0        0        0    15184 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/cache.py
--rw-rw-rw-   0        0        0    19032 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/datafind.py
--rw-rw-rw-   0        0        0     8716 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/ffldatafind.py
--rw-rw-rw-   0        0        0    19671 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/gwf.py
--rw-rw-rw-   0        0        0     5426 2023-05-02 22:40:48.000000 pydischarge-0.0.1/pdpy/io/hdf5.py
--rw-rw-rw-   0        0        0     7149 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/kerberos.py
--rw-rw-rw-   0        0        0    22912 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/ligolw.py
--rw-rw-rw-   0        0        0     4242 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/mp.py
--rw-rw-rw-   0        0        0    19974 2023-05-03 14:01:13.000000 pydischarge-0.0.1/pdpy/io/nds2.py
--rw-rw-rw-   0        0        0     3623 2023-05-02 22:40:48.000000 pydischarge-0.0.1/pdpy/io/registry.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.587230 pydischarge-0.0.1/pdpy/io/tests/
--rw-rw-rw-   0        0        0      763 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/tests/__init__.py
--rw-rw-rw-   0        0        0     8871 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/tests/test_cache.py
--rw-rw-rw-   0        0        0    10959 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/tests/test_datafind.py
--rw-rw-rw-   0        0        0     6511 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/tests/test_ffldatafind.py
--rw-rw-rw-   0        0        0     4364 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/tests/test_gwf.py
--rw-rw-rw-   0        0        0     6708 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/tests/test_kerberos.py
--rw-rw-rw-   0        0        0    11024 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/tests/test_ligolw.py
--rw-rw-rw-   0        0        0     3405 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/tests/test_mp.py
--rw-rw-rw-   0        0        0    12549 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/tests/test_nds2.py
--rw-rw-rw-   0        0        0     4108 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/tests/test_utils.py
--rw-rw-rw-   0        0        0     7590 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/io/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.632232 pydischarge-0.0.1/pdpy/plot/
--rw-rw-rw-   0        0        0     1691 2023-05-02 22:40:48.000000 pydischarge-0.0.1/pdpy/plot/__init__.py
--rw-rw-rw-   0        0        0    23748 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/axes.py
--rw-rw-rw-   0        0        0     9003 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/bode.py
--rw-rw-rw-   0        0        0     7262 2023-05-02 22:40:49.000000 pydischarge-0.0.1/pdpy/plot/colorbar.py
--rw-rw-rw-   0        0        0     3468 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/colors.py
--rw-rw-rw-   0        0        0    17235 2023-05-02 22:40:49.000000 pydischarge-0.0.1/pdpy/plot/gps.py
--rw-rw-rw-   0        0        0     1688 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/legend.py
--rw-rw-rw-   0        0        0     5180 2023-05-02 22:40:49.000000 pydischarge-0.0.1/pdpy/plot/log.py
--rw-rw-rw-   0        0        0    22415 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/plot.py
--rw-rw-rw-   0        0        0     4981 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/rc.py
--rw-rw-rw-   0        0        0    17436 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/segments.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.690231 pydischarge-0.0.1/pdpy/plot/tests/
--rw-rw-rw-   0        0        0      760 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/tests/__init__.py
--rw-rw-rw-   0        0        0    11871 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/tests/test_axes.py
--rw-rw-rw-   0        0        0     3439 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/tests/test_bode.py
--rw-rw-rw-   0        0        0     1944 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/tests/test_colors.py
--rw-rw-rw-   0        0        0     5655 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/tests/test_gps.py
--rw-rw-rw-   0        0        0     2746 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/tests/test_log.py
--rw-rw-rw-   0        0        0     4527 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/tests/test_plot.py
--rw-rw-rw-   0        0        0     1294 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/tests/test_rc.py
--rw-rw-rw-   0        0        0     5601 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/tests/test_segments.py
--rw-rw-rw-   0        0        0     2399 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/tests/test_tex.py
--rw-rw-rw-   0        0        0     1332 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/tests/test_text.py
--rw-rw-rw-   0        0        0     1673 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/tests/test_utils.py
--rw-rw-rw-   0        0        0     1996 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/tests/utils.py
--rw-rw-rw-   0        0        0     4958 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/plot/tex.py
--rw-rw-rw-   0        0        0     2057 2023-05-02 22:40:49.000000 pydischarge-0.0.1/pdpy/plot/text.py
--rw-rw-rw-   0        0        0     1423 2023-05-02 22:40:49.000000 pydischarge-0.0.1/pdpy/plot/units.py
--rw-rw-rw-   0        0        0     1723 2023-05-02 22:40:48.000000 pydischarge-0.0.1/pdpy/plot/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.703231 pydischarge-0.0.1/pdpy/segments/
--rw-rw-rw-   0        0        0     1231 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/segments/__init__.py
--rw-rw-rw-   0        0        0    54276 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/segments/flag.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.721231 pydischarge-0.0.1/pdpy/segments/io/
--rw-rw-rw-   0        0        0     1034 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/segments/io/__init__.py
--rw-rw-rw-   0        0        0    11401 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/segments/io/hdf5.py
--rw-rw-rw-   0        0        0     3140 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/segments/io/json.py
--rw-rw-rw-   0        0        0     5054 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/segments/io/ligolw.py
--rw-rw-rw-   0        0        0     5165 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/segments/io/segwizard.py
--rw-rw-rw-   0        0        0     9313 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/segments/segments.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.730230 pydischarge-0.0.1/pdpy/segments/tests/
--rw-rw-rw-   0        0        0      769 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/segments/tests/__init__.py
--rw-rw-rw-   0        0        0    30537 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/segments/tests/test_flag.py
--rw-rw-rw-   0        0        0     5522 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/segments/tests/test_segments.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.762231 pydischarge-0.0.1/pdpy/signal/
--rw-rw-rw-   0        0        0      998 2023-05-02 22:53:05.000000 pydischarge-0.0.1/pdpy/signal/__init__.py
--rw-rw-rw-   0        0        0     1230 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/fft.py
--rw-rw-rw-   0        0        0    20940 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/filter_design.py
--rw-rw-rw-   0        0        0    25163 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/qtransform.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.801231 pydischarge-0.0.1/pdpy/signal/spectral/
--rw-rw-rw-   0        0        0     1882 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/spectral/__init__.py
--rw-rw-rw-   0        0        0    12395 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/spectral/_lal.py
--rw-rw-rw-   0        0        0     1904 2023-05-02 22:40:48.000000 pydischarge-0.0.1/pdpy/signal/spectral/_median_mean.py
--rw-rw-rw-   0        0        0     3696 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/spectral/_pycbc.py
--rw-rw-rw-   0        0        0     2428 2023-05-02 22:40:48.000000 pydischarge-0.0.1/pdpy/signal/spectral/_registry.py
--rw-rw-rw-   0        0        0     6706 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/spectral/_scipy.py
--rw-rw-rw-   0        0        0    14694 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/spectral/_ui.py
--rw-rw-rw-   0        0        0     1723 2023-05-02 22:40:48.000000 pydischarge-0.0.1/pdpy/signal/spectral/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.830230 pydischarge-0.0.1/pdpy/signal/tests/
--rw-rw-rw-   0        0        0      767 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/tests/__init__.py
--rw-rw-rw-   0        0        0     4504 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/tests/test_filter_design.py
--rw-rw-rw-   0        0        0     4135 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/tests/test_qtransform.py
--rw-rw-rw-   0        0        0     3642 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/tests/test_spectral_lal.py
--rw-rw-rw-   0        0        0     2265 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/tests/test_spectral_median_mean.py
--rw-rw-rw-   0        0        0     2311 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/tests/test_spectral_pycbc.py
--rw-rw-rw-   0        0        0     1495 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/tests/test_spectral_registry.py
--rw-rw-rw-   0        0        0     1926 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/tests/test_spectral_scipy.py
--rw-rw-rw-   0        0        0     3147 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/tests/test_spectral_ui.py
--rw-rw-rw-   0        0        0     1497 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/tests/test_spectral_utils.py
--rw-rw-rw-   0        0        0     2824 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/tests/test_window.py
--rw-rw-rw-   0        0        0     6130 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/signal/window.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.837230 pydischarge-0.0.1/pdpy/spectrogram/
--rw-rw-rw-   0        0        0      945 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/spectrogram/__init__.py
--rw-rw-rw-   0        0        0     5909 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/spectrogram/coherence.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.842230 pydischarge-0.0.1/pdpy/spectrogram/io/
--rw-rw-rw-   0        0        0      872 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/spectrogram/io/__init__.py
--rw-rw-rw-   0        0        0      990 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/spectrogram/io/hdf5.py
--rw-rw-rw-   0        0        0    22861 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/spectrogram/spectrogram.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.847229 pydischarge-0.0.1/pdpy/spectrogram/tests/
--rw-rw-rw-   0        0        0      772 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/spectrogram/tests/__init__.py
--rw-rw-rw-   0        0        0     6788 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/spectrogram/tests/test_spectrogram.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.859230 pydischarge-0.0.1/pdpy/table/
--rw-rw-rw-   0        0        0     1459 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/table/__init__.py
--rw-rw-rw-   0        0        0     8176 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/table/filter.py
--rw-rw-rw-   0        0        0     2726 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/table/filters.py
--rw-rw-rw-   0        0        0     8439 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/table/gravityspy.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.896229 pydischarge-0.0.1/pdpy/table/io/
--rw-rw-rw-   0        0        0     1607 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/table/io/__init__.py
--rw-rw-rw-   0        0        0     3937 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/table/io/cwb.py
--rw-rw-rw-   0        0        0     4836 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/table/io/fetch.py
--rw-rw-rw-   0        0        0     4805 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/table/io/gravityspy.py
--rw-rw-rw-   0        0        0     8616 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/table/io/gstlal.py
--rw-rw-rw-   0        0        0     5603 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/table/io/gwf.py
--rw-rw-rw-   0        0        0     5363 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/table/io/hacr.py
--rw-rw-rw-   0        0        0    13997 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/table/io/ligolw.py
--rw-rw-rw-   0        0        0     4597 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/table/io/losc.py
--rw-rw-rw-   0        0        0     2698 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/table/io/omega.py
--rw-rw-rw-   0        0        0     1372 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/table/io/omicron.py
--rw-rw-rw-   0        0        0     9197 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/table/io/pycbc.py
--rw-rw-rw-   0        0        0     3435 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/table/io/root.py
--rw-rw-rw-   0        0        0     3973 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/table/io/snax.py
--rw-rw-rw-   0        0        0     3167 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/table/io/sql.py
--rw-rw-rw-   0        0        0     3300 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/table/io/utils.py
--rw-rw-rw-   0        0        0    27118 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/table/table.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.911231 pydischarge-0.0.1/pdpy/table/tests/
--rw-rw-rw-   0        0        0      766 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/table/tests/__init__.py
--rw-rw-rw-   0        0        0     3501 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/table/tests/test_gravityspy.py
--rw-rw-rw-   0        0        0     8188 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/table/tests/test_io_gstlal.py
--rw-rw-rw-   0        0        0     2937 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/table/tests/test_io_ligolw.py
--rw-rw-rw-   0        0        0     8617 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/table/tests/test_io_pycbc.py
--rw-rw-rw-   0        0        0    31268 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/table/tests/test_table.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.924229 pydischarge-0.0.1/pdpy/testing/
--rw-rw-rw-   0        0        0      765 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/testing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.940231 pydischarge-0.0.1/pdpy/testing/data/
--rw-rw-rw-   0        0        0    58124 2023-05-02 15:35:55.000000 pydischarge-0.0.1/pdpy/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz
--rw-rw-rw-   0        0        0   377295 2023-05-02 15:35:55.000000 pydischarge-0.0.1/pdpy/testing/data/HLV-HW100916-968654552-1.gwf
--rw-rw-rw-   0        0        0   382679 2023-05-02 15:35:55.000000 pydischarge-0.0.1/pdpy/testing/data/HLV-HW100916-968654552-1.hdf
--rw-rw-rw-   0        0        0       63 2023-05-02 15:35:55.000000 pydischarge-0.0.1/pdpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.txt
--rw-rw-rw-   0        0        0      564 2023-05-02 15:35:55.000000 pydischarge-0.0.1/pdpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.xml.gz
--rw-rw-rw-   0        0        0     2879 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/testing/errors.py
--rw-rw-rw-   0        0        0     3900 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/testing/fixtures.py
--rw-rw-rw-   0        0        0     1525 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/testing/marks.py
--rw-rw-rw-   0        0        0     4257 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/testing/mocks.py
--rw-rw-rw-   0        0        0    12106 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/testing/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.948229 pydischarge-0.0.1/pdpy/time/
--rw-rw-rw-   0        0        0     1869 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/time/__init__.py
--rw-rw-rw-   0        0        0     2352 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/time/__main__.py
--rw-rw-rw-   0        0        0     9295 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/time/_tconvert.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.954230 pydischarge-0.0.1/pdpy/time/tests/
--rw-rw-rw-   0        0        0      765 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/time/tests/__init__.py
--rw-rw-rw-   0        0        0     1403 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/time/tests/test_main.py
--rw-rw-rw-   0        0        0     5923 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/time/tests/test_time.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.965231 pydischarge-0.0.1/pdpy/timeseries/
--rw-rw-rw-   0        0        0     1163 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/timeseries/__init__.py
--rw-rw-rw-   0        0        0    58616 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/timeseries/core.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.983229 pydischarge-0.0.1/pdpy/timeseries/io/
--rw-rw-rw-   0        0        0      968 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/timeseries/io/__init__.py
--rw-rw-rw-   0        0        0     1215 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/timeseries/io/ascii.py
--rw-rw-rw-   0        0        0     2676 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/timeseries/io/cache.py
--rw-rw-rw-   0        0        0     4839 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/timeseries/io/core.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:37.993230 pydischarge-0.0.1/pdpy/timeseries/io/gwf/
--rw-rw-rw-   0        0        0    13554 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/timeseries/io/gwf/__init__.py
--rw-rw-rw-   0        0        0    17713 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/timeseries/io/gwf/framecpp.py
--rw-rw-rw-   0        0        0     4943 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/timeseries/io/gwf/framel.py
--rw-rw-rw-   0        0        0     7056 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/timeseries/io/gwf/lalframe.py
--rw-rw-rw-   0        0        0     4345 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/timeseries/io/hdf5.py
--rw-rw-rw-   0        0        0     9631 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/timeseries/io/losc.py
--rw-rw-rw-   0        0        0     8016 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/timeseries/io/nds2.py
--rw-rw-rw-   0        0        0     3721 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/timeseries/io/wav.py
--rw-rw-rw-   0        0        0    36810 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/timeseries/statevector.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:38.010230 pydischarge-0.0.1/pdpy/timeseries/tests/
--rw-rw-rw-   0        0        0      771 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/timeseries/tests/__init__.py
--rw-rw-rw-   0        0        0    18737 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/timeseries/tests/test_core.py
--rw-rw-rw-   0        0        0     2348 2023-05-03 12:42:53.000000 pydischarge-0.0.1/pdpy/timeseries/tests/test_io_gwf_framecpp.py
--rw-rw-rw-   0        0        0     5155 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/timeseries/tests/test_io_gwf_lalframe.py
--rw-rw-rw-   0        0        0     1901 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/timeseries/tests/test_io_losc.py
--rw-rw-rw-   0        0        0    12743 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/timeseries/tests/test_statevector.py
--rw-rw-rw-   0        0        0    56690 2023-05-03 12:43:21.000000 pydischarge-0.0.1/pdpy/timeseries/tests/test_timeseries.py
--rw-rw-rw-   0        0        0    89994 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/timeseries/timeseries.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:38.025231 pydischarge-0.0.1/pdpy/types/
--rw-rw-rw-   0        0        0     1193 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/types/__init__.py
--rw-rw-rw-   0        0        0    15773 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/types/array.py
--rw-rw-rw-   0        0        0    12752 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/types/array2d.py
--rw-rw-rw-   0        0        0     3176 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/types/index.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:38.034229 pydischarge-0.0.1/pdpy/types/io/
--rw-rw-rw-   0        0        0      932 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/types/io/__init__.py
--rw-rw-rw-   0        0        0     2965 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/types/io/ascii.py
--rw-rw-rw-   0        0        0     8256 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/types/io/hdf5.py
--rw-rw-rw-   0        0        0     7500 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/types/io/ligolw.py
--rw-rw-rw-   0        0        0    37893 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/types/series.py
--rw-rw-rw-   0        0        0     3697 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/types/sliceutils.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:38.046229 pydischarge-0.0.1/pdpy/types/tests/
--rw-rw-rw-   0        0        0      766 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/types/tests/__init__.py
--rw-rw-rw-   0        0        0     8887 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/types/tests/test_array.py
--rw-rw-rw-   0        0        0     9340 2023-05-03 12:43:28.000000 pydischarge-0.0.1/pdpy/types/tests/test_array2d.py
--rw-rw-rw-   0        0        0     2113 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/types/tests/test_index.py
--rw-rw-rw-   0        0        0    15182 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/types/tests/test_series.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:38.066230 pydischarge-0.0.1/pdpy/utils/
--rw-rw-rw-   0        0        0      965 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/utils/__init__.py
--rw-rw-rw-   0        0        0     3841 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/utils/decorators.py
--rw-rw-rw-   0        0        0     1542 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/utils/enum.py
--rw-rw-rw-   0        0        0     1988 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/utils/env.py
--rw-rw-rw-   0        0        0     8827 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/utils/lal.py
--rw-rw-rw-   0        0        0     3410 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/utils/misc.py
--rw-rw-rw-   0        0        0     5228 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/utils/mp.py
--rw-rw-rw-   0        0        0     1413 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/utils/progress.py
--rw-rw-rw-   0        0        0     3516 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/utils/shell.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:38.075231 pydischarge-0.0.1/pdpy/utils/sphinx/
--rw-rw-rw-   0        0        0      790 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/utils/sphinx/__init__.py
--rw-rw-rw-   0        0        0     3663 2023-05-02 15:35:55.000000 pydischarge-0.0.1/pdpy/utils/sphinx/epydoc.py
--rw-rw-rw-   0        0        0     4941 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/utils/sphinx/ex2rst.py
--rw-rw-rw-   0        0        0     3530 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/utils/sphinx/zenodo.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:38.099229 pydischarge-0.0.1/pdpy/utils/tests/
--rw-rw-rw-   0        0        0      766 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/utils/tests/__init__.py
--rw-rw-rw-   0        0        0     2289 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/utils/tests/test_decorators.py
--rw-rw-rw-   0        0        0     2260 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/utils/tests/test_enum.py
--rw-rw-rw-   0        0        0     2072 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/utils/tests/test_env.py
--rw-rw-rw-   0        0        0     3605 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/utils/tests/test_lal.py
--rw-rw-rw-   0        0        0     2700 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/utils/tests/test_misc.py
--rw-rw-rw-   0        0        0     2134 2023-05-02 22:40:46.000000 pydischarge-0.0.1/pdpy/utils/tests/test_mp.py
--rw-rw-rw-   0        0        0     2444 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/utils/tests/test_shell.py
--rw-rw-rw-   0        0        0     2376 2023-05-02 22:41:13.000000 pydischarge-0.0.1/pdpy/utils/tests/test_sphinx_ex2rst.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:29:38.141231 pydischarge-0.0.1/pydischarge.egg-info/
--rw-rw-rw-   0        0        0     3282 2023-05-09 15:29:36.000000 pydischarge-0.0.1/pydischarge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10049 2023-05-09 15:29:37.000000 pydischarge-0.0.1/pydischarge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 15:29:36.000000 pydischarge-0.0.1/pydischarge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-09 15:29:36.000000 pydischarge-0.0.1/pydischarge.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      793 2023-05-09 15:29:36.000000 pydischarge-0.0.1/pydischarge.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-09 15:29:36.000000 pydischarge-0.0.1/pydischarge.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5063 2023-05-09 15:27:14.000000 pydischarge-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 15:29:38.146230 pydischarge-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:33.270437 pydischarge-0.0.2/
+-rw-rw-rw-   0        0        0       38 2023-05-09 15:33:18.000000 pydischarge-0.0.2/.gitattributes
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:31.948954 pydischarge-0.0.2/.github/
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.060944 pydischarge-0.0.2/.github/workflows/
+-rw-rw-rw-   0        0        0     5314 2023-05-09 15:34:12.000000 pydischarge-0.0.2/.github/workflows/conda.yml
+-rw-rw-rw-   0        0        0     3051 2023-05-09 15:34:12.000000 pydischarge-0.0.2/.github/workflows/dependencies.yml
+-rw-rw-rw-   0        0        0     3300 2023-05-09 15:34:12.000000 pydischarge-0.0.2/.github/workflows/dist.yml
+-rw-rw-rw-   0        0        0      737 2023-05-09 14:05:20.000000 pydischarge-0.0.2/.github/workflows/documentation.yml
+-rw-rw-rw-   0        0        0     1481 2023-05-02 15:35:55.000000 pydischarge-0.0.2/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      805 2023-05-09 15:33:18.000000 pydischarge-0.0.2/.gitignore
+-rw-rw-rw-   0        0        0      142 2023-05-09 15:34:12.000000 pydischarge-0.0.2/CODE_OF_CONDUCT.rst
+-rw-rw-rw-   0        0        0     4736 2023-05-09 15:34:12.000000 pydischarge-0.0.2/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    35821 2023-05-02 15:35:55.000000 pydischarge-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      195 2023-05-09 15:33:18.000000 pydischarge-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3513 2023-05-09 15:49:33.269437 pydischarge-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2071 2023-05-09 15:34:12.000000 pydischarge-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.082070 pydischarge-0.0.2/docs/
+-rw-rw-rw-   0        0        0      825 2023-05-09 15:33:19.000000 pydischarge-0.0.2/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.087070 pydischarge-0.0.2/docs/_static/
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.090076 pydischarge-0.0.2/docs/_static/css/
+-rw-rw-rw-   0        0        0     1366 2023-05-09 15:34:12.000000 pydischarge-0.0.2/docs/_static/css/gwpy-sphinx.css
+-rw-rw-rw-   0        0        0   174729 2023-05-09 13:06:08.000000 pydischarge-0.0.2/docs/_static/favicon.png
+-rw-rw-rw-   0        0        0    15166 2023-05-02 15:35:55.000000 pydischarge-0.0.2/docs/_static/gwpy_white_24.png
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:31.958947 pydischarge-0.0.2/docs/_templates/
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.093071 pydischarge-0.0.2/docs/_templates/autoclass/
+-rw-rw-rw-   0        0        0      915 2023-05-02 15:35:55.000000 pydischarge-0.0.2/docs/_templates/autoclass/class.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.100070 pydischarge-0.0.2/docs/_templates/autosummary/
+-rw-rw-rw-   0        0        0      180 2023-05-02 15:35:55.000000 pydischarge-0.0.2/docs/_templates/autosummary/base.rst
+-rw-rw-rw-   0        0        0     1210 2023-05-02 15:35:55.000000 pydischarge-0.0.2/docs/_templates/autosummary/class.rst
+-rw-rw-rw-   0        0        0      744 2023-05-02 15:35:55.000000 pydischarge-0.0.2/docs/_templates/autosummary/module.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.102070 pydischarge-0.0.2/docs/astro/
+-rw-rw-rw-   0        0        0      797 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/astro/index.rst
+-rw-rw-rw-   0        0        0     2812 2023-05-09 15:34:12.000000 pydischarge-0.0.2/docs/citing.rst.in
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.107075 pydischarge-0.0.2/docs/cli/
+-rw-rw-rw-   0        0        0     5555 2023-05-09 15:33:19.000000 pydischarge-0.0.2/docs/cli/examples.ini
+-rw-rw-rw-   0        0        0     3036 2023-05-09 15:34:12.000000 pydischarge-0.0.2/docs/cli/index.rst
+-rw-rw-rw-   0        0        0    14000 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.110070 pydischarge-0.0.2/docs/detector/
+-rw-rw-rw-   0        0        0     3372 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/detector/channel.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.112070 pydischarge-0.0.2/docs/dev/
+-rw-rw-rw-   0        0        0     4047 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/dev/release.rst
+-rw-rw-rw-   0        0        0     1690 2023-05-09 15:34:12.000000 pydischarge-0.0.2/docs/env.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:31.966950 pydischarge-0.0.2/docs/examples/
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.114071 pydischarge-0.0.2/docs/examples/table/
+-rw-rw-rw-   0        0        0       68 2023-05-09 15:33:19.000000 pydischarge-0.0.2/docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.123071 pydischarge-0.0.2/docs/external/
+-rw-rw-rw-   0        0        0     1206 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/external/framecpp.rst
+-rw-rw-rw-   0        0        0     1034 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/external/framel.rst
+-rw-rw-rw-   0        0        0     3310 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/external/lalsuite.rst
+-rw-rw-rw-   0        0        0     1058 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/external/nds2.rst
+-rw-rw-rw-   0        0        0     2730 2023-05-09 15:34:12.000000 pydischarge-0.0.2/docs/index.rst
+-rw-rw-rw-   0        0        0     1440 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/install.rst
+-rw-rw-rw-   0        0        0     2825 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/overview.rst
+-rw-rw-rw-   0        0        0    67943 2023-05-09 13:03:59.000000 pydischarge-0.0.2/docs/pdpy-docs-logo.png
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.141071 pydischarge-0.0.2/docs/plot/
+-rw-rw-rw-   0        0        0     2751 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/plot/colorbars.rst
+-rw-rw-rw-   0        0        0     3201 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/plot/colors.rst
+-rw-rw-rw-   0        0        0      820 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/plot/filter.rst
+-rw-rw-rw-   0        0        0     2646 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/plot/gps.rst
+-rw-rw-rw-   0        0        0     3324 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/plot/index.rst
+-rw-rw-rw-   0        0        0     1943 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/plot/legend.rst
+-rw-rw-rw-   0        0        0     1441 2023-05-09 15:34:12.000000 pydischarge-0.0.2/docs/plot/log.rst
+-rw-rw-rw-   0        0        0     5080 2023-05-09 15:33:19.000000 pydischarge-0.0.2/docs/references.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.151070 pydischarge-0.0.2/docs/segments/
+-rw-rw-rw-   0        0        0     1577 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/segments/dqsegdb.rst
+-rw-rw-rw-   0        0        0     7113 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/segments/index.rst
+-rw-rw-rw-   0        0        0     7013 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/segments/io.rst
+-rw-rw-rw-   0        0        0     2191 2023-05-09 15:34:12.000000 pydischarge-0.0.2/docs/segments/thresholding.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.153068 pydischarge-0.0.2/docs/signal/
+-rw-rw-rw-   0        0        0     4678 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/signal/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.155072 pydischarge-0.0.2/docs/spectrogram/
+-rw-rw-rw-   0        0        0     3988 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/spectrogram/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.163070 pydischarge-0.0.2/docs/spectrum/
+-rw-rw-rw-   0        0        0      559 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/spectrum/filtering.rst
+-rw-rw-rw-   0        0        0     3931 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/spectrum/index.rst
+-rw-rw-rw-   0        0        0     5204 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/spectrum/io.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.179070 pydischarge-0.0.2/docs/table/
+-rw-rw-rw-   0        0        0       65 2023-05-09 15:33:19.000000 pydischarge-0.0.2/docs/table/H1-LDAS_STRAIN-968654552-10.xml.gz
+-rw-rw-rw-   0        0        0     7597 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/table/filter.rst
+-rw-rw-rw-   0        0        0     1013 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/table/histogram.rst
+-rw-rw-rw-   0        0        0     1610 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/table/index.rst
+-rw-rw-rw-   0        0        0    31631 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/table/io.rst
+-rw-rw-rw-   0        0        0     1851 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/table/plot.rst
+-rw-rw-rw-   0        0        0     2242 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/table/rate.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.181069 pydischarge-0.0.2/docs/time/
+-rw-rw-rw-   0        0        0     1183 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/time/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.196071 pydischarge-0.0.2/docs/timeseries/
+-rw-rw-rw-   0        0        0    12005 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/timeseries/datafind.rst
+-rw-rw-rw-   0        0        0     2889 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/timeseries/index.rst
+-rw-rw-rw-   0        0        0    11214 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/timeseries/io.rst
+-rw-rw-rw-   0        0        0     2860 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/timeseries/opendata.rst
+-rw-rw-rw-   0        0        0     3206 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/timeseries/plot.rst
+-rw-rw-rw-   0        0        0     8769 2023-05-09 15:37:50.000000 pydischarge-0.0.2/docs/timeseries/statevector.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.199070 pydischarge-0.0.2/examples/
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.219071 pydischarge-0.0.2/examples/frequencyseries/
+-rw-rw-rw-   0        0        0     2699 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/frequencyseries/coherence.py
+-rw-rw-rw-   0        0        0     2203 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/frequencyseries/hoff.py
+-rw-rw-rw-   0        0        0      282 2023-05-09 15:33:19.000000 pydischarge-0.0.2/examples/frequencyseries/index.rst
+-rw-rw-rw-   0        0        0     2719 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/frequencyseries/inject.py
+-rw-rw-rw-   0        0        0     2966 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/frequencyseries/percentiles.py
+-rw-rw-rw-   0        0        0     2935 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/frequencyseries/rayleigh.py
+-rw-rw-rw-   0        0        0     2336 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/frequencyseries/transfer_function.py
+-rw-rw-rw-   0        0        0     2757 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/frequencyseries/variance.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.255071 pydischarge-0.0.2/examples/miscellaneous/
+-rw-rw-rw-   0        0        0      236 2023-05-09 15:33:19.000000 pydischarge-0.0.2/examples/miscellaneous/index.rst
+-rw-rw-rw-   0        0        0     3502 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/miscellaneous/open-data-spectrogram.py
+-rw-rw-rw-   0        0        0     2463 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/miscellaneous/range-spectrogram.py
+-rw-rw-rw-   0        0        0     2603 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/miscellaneous/range-timeseries.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.262071 pydischarge-0.0.2/examples/segments/
+-rw-rw-rw-   0        0        0      176 2023-05-09 15:33:19.000000 pydischarge-0.0.2/examples/segments/index.rst
+-rw-rw-rw-   0        0        0     2527 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/segments/open-data.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.270070 pydischarge-0.0.2/examples/signal/
+-rw-rw-rw-   0        0        0     5913 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/signal/gw150914.py
+-rw-rw-rw-   0        0        0      198 2023-05-09 15:33:19.000000 pydischarge-0.0.2/examples/signal/index.rst
+-rw-rw-rw-   0        0        0     3279 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/signal/qscan.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.289071 pydischarge-0.0.2/examples/spectrogram/
+-rw-rw-rw-   0        0        0     2517 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/spectrogram/coherence.py
+-rw-rw-rw-   0        0        0      231 2023-05-09 15:33:19.000000 pydischarge-0.0.2/examples/spectrogram/index.rst
+-rw-rw-rw-   0        0        0     2768 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/spectrogram/plot.py
+-rw-rw-rw-   0        0        0     2746 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/spectrogram/ratio.py
+-rw-rw-rw-   0        0        0     2240 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/spectrogram/rayleigh.py
+-rw-rw-rw-   0        0        0     3007 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/spectrogram/spectrogram2.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.310070 pydischarge-0.0.2/examples/table/
+-rw-rw-rw-   0        0        0       65 2023-05-09 15:33:19.000000 pydischarge-0.0.2/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
+-rw-rw-rw-   0        0        0     1695 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/table/histogram.py
+-rw-rw-rw-   0        0        0      220 2023-05-09 15:33:19.000000 pydischarge-0.0.2/examples/table/index.rst
+-rw-rw-rw-   0        0        0     2431 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/table/rate.py
+-rw-rw-rw-   0        0        0     2564 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/table/rate_binned.py
+-rw-rw-rw-   0        0        0     2133 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/table/scatter.py
+-rw-rw-rw-   0        0        0     2386 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/table/tiles.py
+-rw-rw-rw-   0        0        0     3923 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/test_examples.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.516971 pydischarge-0.0.2/examples/timeseries/
+-rw-rw-rw-   0        0        0     2693 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/timeseries/blrms.py
+-rw-rw-rw-   0        0        0     4356 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/timeseries/correlate.py
+-rw-rw-rw-   0        0        0     2946 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/timeseries/filter.py
+-rw-rw-rw-   0        0        0      272 2023-05-09 15:33:19.000000 pydischarge-0.0.2/examples/timeseries/index.rst
+-rw-rw-rw-   0        0        0     2761 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/timeseries/inject.py
+-rw-rw-rw-   0        0        0     2594 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/timeseries/public.py
+-rw-rw-rw-   0        0        0     3960 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/timeseries/pycbc-snr.py
+-rw-rw-rw-   0        0        0     2718 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/timeseries/qscan.py
+-rw-rw-rw-   0        0        0     2309 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/timeseries/statevector.py
+-rw-rw-rw-   0        0        0     2586 2023-05-09 15:34:12.000000 pydischarge-0.0.2/examples/timeseries/whiten.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.529967 pydischarge-0.0.2/pydischarge/
+-rw-rw-rw-   0        0        0     1623 2023-05-09 15:34:13.000000 pydischarge-0.0.2/pydischarge/__init__.py
+-rw-rw-rw-   0        0        0      164 2023-05-09 15:49:30.000000 pydischarge-0.0.2/pydischarge/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.575964 pydischarge-0.0.2/pydischarge/astro/
+-rw-rw-rw-   0        0        0     2051 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/astro/__init__.py
+-rw-rw-rw-   0        0        0    25906 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/astro/range.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.584963 pydischarge-0.0.2/pydischarge/astro/tests/
+-rw-rw-rw-   0        0        0      801 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/astro/tests/__init__.py
+-rw-rw-rw-   0        0        0     6325 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/astro/tests/test_range.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.611965 pydischarge-0.0.2/pydischarge/cli/
+-rw-rw-rw-   0        0        0     1505 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/__init__.py
+-rw-rw-rw-   0        0        0    36334 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/cliproduct.py
+-rw-rw-rw-   0        0        0     4207 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/coherence.py
+-rw-rw-rw-   0        0        0     3482 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/coherencegram.py
+-rw-rw-rw-   0        0        0     5365 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/gwpy_plot.py
+-rw-rw-rw-   0        0        0     9432 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/qtransform.py
+-rw-rw-rw-   0        0        0     7370 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/spectrogram.py
+-rw-rw-rw-   0        0        0     5098 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/spectrum.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.634965 pydischarge-0.0.2/pydischarge/cli/tests/
+-rw-rw-rw-   0        0        0      799 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/tests/__init__.py
+-rw-rw-rw-   0        0        0    11211 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/tests/base.py
+-rw-rw-rw-   0        0        0     1427 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/tests/test_coherence.py
+-rw-rw-rw-   0        0        0     1660 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/tests/test_coherencegram.py
+-rw-rw-rw-   0        0        0     1866 2023-05-09 15:37:50.000000 pydischarge-0.0.2/pydischarge/cli/tests/test_gwpy_plot.py
+-rw-rw-rw-   0        0        0     3026 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/tests/test_qtransform.py
+-rw-rw-rw-   0        0        0     1591 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/tests/test_spectrogram.py
+-rw-rw-rw-   0        0        0     1494 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/tests/test_spectrum.py
+-rw-rw-rw-   0        0        0     1350 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/tests/test_timeseries.py
+-rw-rw-rw-   0        0        0     2092 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/tests/test_transferfunction.py
+-rw-rw-rw-   0        0        0     4141 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/timeseries.py
+-rw-rw-rw-   0        0        0    10108 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/cli/transferfunction.py
+-rw-rw-rw-   0        0        0     1737 2023-05-09 15:34:13.000000 pydischarge-0.0.2/pydischarge/conftest.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.643964 pydischarge-0.0.2/pydischarge/detector/
+-rw-rw-rw-   0        0        0     2365 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/detector/__init__.py
+-rw-rw-rw-   0        0        0    27830 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/detector/channel.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.651965 pydischarge-0.0.2/pydischarge/detector/io/
+-rw-rw-rw-   0        0        0     1093 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/detector/io/__init__.py
+-rw-rw-rw-   0        0        0     3338 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/detector/io/cis.py
+-rw-rw-rw-   0        0        0     5902 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/detector/io/clf.py
+-rw-rw-rw-   0        0        0     6159 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/detector/io/omega.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.659964 pydischarge-0.0.2/pydischarge/detector/tests/
+-rw-rw-rw-   0        0        0      804 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/detector/tests/__init__.py
+-rw-rw-rw-   0        0        0    19052 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/detector/tests/test_channel.py
+-rw-rw-rw-   0        0        0     2664 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/detector/tests/test_units.py
+-rw-rw-rw-   0        0        0     7382 2023-05-09 15:37:50.000000 pydischarge-0.0.2/pydischarge/detector/units.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.669437 pydischarge-0.0.2/pydischarge/frequencyseries/
+-rw-rw-rw-   0        0        0     1052 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/frequencyseries/__init__.py
+-rw-rw-rw-   0        0        0     2051 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/frequencyseries/_fdcommon.py
+-rw-rw-rw-   0        0        0    14844 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/frequencyseries/frequencyseries.py
+-rw-rw-rw-   0        0        0    12357 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/frequencyseries/hist.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.679436 pydischarge-0.0.2/pydischarge/frequencyseries/io/
+-rw-rw-rw-   0        0        0      970 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/frequencyseries/io/__init__.py
+-rw-rw-rw-   0        0        0     1134 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/frequencyseries/io/ascii.py
+-rw-rw-rw-   0        0        0     1092 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/frequencyseries/io/hdf5.py
+-rw-rw-rw-   0        0        0     1214 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/frequencyseries/io/ligolw.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.686437 pydischarge-0.0.2/pydischarge/frequencyseries/tests/
+-rw-rw-rw-   0        0        0      811 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/frequencyseries/tests/__init__.py
+-rw-rw-rw-   0        0        0    11385 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/frequencyseries/tests/test_frequencyseries.py
+-rw-rw-rw-   0        0        0     4162 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/frequencyseries/tests/test_hist.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.721437 pydischarge-0.0.2/pydischarge/io/
+-rw-rw-rw-   0        0        0      881 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/__init__.py
+-rw-rw-rw-   0        0        0     4394 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/_framecpp.py
+-rw-rw-rw-   0        0        0    15275 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/cache.py
+-rw-rw-rw-   0        0        0    19137 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/datafind.py
+-rw-rw-rw-   0        0        0     8751 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/ffldatafind.py
+-rw-rw-rw-   0        0        0    19783 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/gwf.py
+-rw-rw-rw-   0        0        0     5461 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/hdf5.py
+-rw-rw-rw-   0        0        0     7184 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/kerberos.py
+-rw-rw-rw-   0        0        0    22961 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/ligolw.py
+-rw-rw-rw-   0        0        0     4277 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/mp.py
+-rw-rw-rw-   0        0        0    20037 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/nds2.py
+-rw-rw-rw-   0        0        0     3651 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/registry.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.748435 pydischarge-0.0.2/pydischarge/io/tests/
+-rw-rw-rw-   0        0        0      798 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/tests/__init__.py
+-rw-rw-rw-   0        0        0     8955 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/tests/test_cache.py
+-rw-rw-rw-   0        0        0    11022 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/tests/test_datafind.py
+-rw-rw-rw-   0        0        0     6581 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/tests/test_ffldatafind.py
+-rw-rw-rw-   0        0        0     4399 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/tests/test_gwf.py
+-rw-rw-rw-   0        0        0     6827 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/tests/test_kerberos.py
+-rw-rw-rw-   0        0        0    11073 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/tests/test_ligolw.py
+-rw-rw-rw-   0        0        0     3440 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/tests/test_mp.py
+-rw-rw-rw-   0        0        0    12794 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/tests/test_nds2.py
+-rw-rw-rw-   0        0        0     4157 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/tests/test_utils.py
+-rw-rw-rw-   0        0        0     7625 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/io/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.785436 pydischarge-0.0.2/pydischarge/plot/
+-rw-rw-rw-   0        0        0     1719 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/__init__.py
+-rw-rw-rw-   0        0        0    23909 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/axes.py
+-rw-rw-rw-   0        0        0     9059 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/bode.py
+-rw-rw-rw-   0        0        0     7290 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/colorbar.py
+-rw-rw-rw-   0        0        0     3517 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/colors.py
+-rw-rw-rw-   0        0        0    17263 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/gps.py
+-rw-rw-rw-   0        0        0     1723 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/legend.py
+-rw-rw-rw-   0        0        0     5222 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/log.py
+-rw-rw-rw-   0        0        0    22499 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/plot.py
+-rw-rw-rw-   0        0        0     5058 2023-05-09 15:37:50.000000 pydischarge-0.0.2/pydischarge/plot/rc.py
+-rw-rw-rw-   0        0        0    17597 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/segments.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.822439 pydischarge-0.0.2/pydischarge/plot/tests/
+-rw-rw-rw-   0        0        0      795 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/tests/__init__.py
+-rw-rw-rw-   0        0        0    11913 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/tests/test_axes.py
+-rw-rw-rw-   0        0        0     3474 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/tests/test_bode.py
+-rw-rw-rw-   0        0        0     1979 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/tests/test_colors.py
+-rw-rw-rw-   0        0        0     5690 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/tests/test_gps.py
+-rw-rw-rw-   0        0        0     2802 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/tests/test_log.py
+-rw-rw-rw-   0        0        0     4562 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/tests/test_plot.py
+-rw-rw-rw-   0        0        0     1329 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/tests/test_rc.py
+-rw-rw-rw-   0        0        0     5636 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/tests/test_segments.py
+-rw-rw-rw-   0        0        0     2483 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/tests/test_tex.py
+-rw-rw-rw-   0        0        0     1367 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/tests/test_text.py
+-rw-rw-rw-   0        0        0     1708 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/tests/test_utils.py
+-rw-rw-rw-   0        0        0     2031 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/tests/utils.py
+-rw-rw-rw-   0        0        0     5000 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/tex.py
+-rw-rw-rw-   0        0        0     2092 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/text.py
+-rw-rw-rw-   0        0        0     1451 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/units.py
+-rw-rw-rw-   0        0        0     1758 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/plot/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.830437 pydischarge-0.0.2/pydischarge/segments/
+-rw-rw-rw-   0        0        0     1259 2023-05-09 15:34:13.000000 pydischarge-0.0.2/pydischarge/segments/__init__.py
+-rw-rw-rw-   0        0        0    54360 2023-05-09 15:34:13.000000 pydischarge-0.0.2/pydischarge/segments/flag.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.843435 pydischarge-0.0.2/pydischarge/segments/io/
+-rw-rw-rw-   0        0        0     1069 2023-05-09 15:34:13.000000 pydischarge-0.0.2/pydischarge/segments/io/__init__.py
+-rw-rw-rw-   0        0        0    11429 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/segments/io/hdf5.py
+-rw-rw-rw-   0        0        0     3168 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/segments/io/json.py
+-rw-rw-rw-   0        0        0     5096 2023-05-09 15:34:13.000000 pydischarge-0.0.2/pydischarge/segments/io/ligolw.py
+-rw-rw-rw-   0        0        0     5207 2023-05-09 15:34:13.000000 pydischarge-0.0.2/pydischarge/segments/io/segwizard.py
+-rw-rw-rw-   0        0        0     9348 2023-05-09 15:34:13.000000 pydischarge-0.0.2/pydischarge/segments/segments.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.851438 pydischarge-0.0.2/pydischarge/segments/tests/
+-rw-rw-rw-   0        0        0      804 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/segments/tests/__init__.py
+-rw-rw-rw-   0        0        0    30628 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/segments/tests/test_flag.py
+-rw-rw-rw-   0        0        0     5564 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/segments/tests/test_segments.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.864437 pydischarge-0.0.2/pydischarge/signal/
+-rw-rw-rw-   0        0        0     1026 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/__init__.py
+-rw-rw-rw-   0        0        0     1272 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/fft.py
+-rw-rw-rw-   0        0        0    21073 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/filter_design.py
+-rw-rw-rw-   0        0        0    25296 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/qtransform.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.885437 pydischarge-0.0.2/pydischarge/signal/spectral/
+-rw-rw-rw-   0        0        0     1938 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/spectral/__init__.py
+-rw-rw-rw-   0        0        0    12500 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/spectral/_lal.py
+-rw-rw-rw-   0        0        0     1932 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/spectral/_median_mean.py
+-rw-rw-rw-   0        0        0     3752 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/spectral/_pycbc.py
+-rw-rw-rw-   0        0        0     2456 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/spectral/_registry.py
+-rw-rw-rw-   0        0        0     6797 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/spectral/_scipy.py
+-rw-rw-rw-   0        0        0    14757 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/spectral/_ui.py
+-rw-rw-rw-   0        0        0     1751 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/spectral/_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.915436 pydischarge-0.0.2/pydischarge/signal/tests/
+-rw-rw-rw-   0        0        0      802 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/tests/__init__.py
+-rw-rw-rw-   0        0        0     4539 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/tests/test_filter_design.py
+-rw-rw-rw-   0        0        0     4170 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/tests/test_qtransform.py
+-rw-rw-rw-   0        0        0     3684 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/tests/test_spectral_lal.py
+-rw-rw-rw-   0        0        0     2314 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/tests/test_spectral_median_mean.py
+-rw-rw-rw-   0        0        0     2346 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/tests/test_spectral_pycbc.py
+-rw-rw-rw-   0        0        0     1537 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/tests/test_spectral_registry.py
+-rw-rw-rw-   0        0        0     1961 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/tests/test_spectral_scipy.py
+-rw-rw-rw-   0        0        0     3203 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/tests/test_spectral_ui.py
+-rw-rw-rw-   0        0        0     1532 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/tests/test_spectral_utils.py
+-rw-rw-rw-   0        0        0     2859 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/tests/test_window.py
+-rw-rw-rw-   0        0        0     6179 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/signal/window.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.924439 pydischarge-0.0.2/pydischarge/spectrogram/
+-rw-rw-rw-   0        0        0      973 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/spectrogram/__init__.py
+-rw-rw-rw-   0        0        0     5972 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/spectrogram/coherence.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.929438 pydischarge-0.0.2/pydischarge/spectrogram/io/
+-rw-rw-rw-   0        0        0      900 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/spectrogram/io/__init__.py
+-rw-rw-rw-   0        0        0     1018 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/spectrogram/io/hdf5.py
+-rw-rw-rw-   0        0        0    22994 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/spectrogram/spectrogram.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.934436 pydischarge-0.0.2/pydischarge/spectrogram/tests/
+-rw-rw-rw-   0        0        0      807 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/spectrogram/tests/__init__.py
+-rw-rw-rw-   0        0        0     6830 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/spectrogram/tests/test_spectrogram.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.947436 pydischarge-0.0.2/pydischarge/table/
+-rw-rw-rw-   0        0        0     1494 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/__init__.py
+-rw-rw-rw-   0        0        0     8211 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/filter.py
+-rw-rw-rw-   0        0        0     2768 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/filters.py
+-rw-rw-rw-   0        0        0     8467 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/gravityspy.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.990436 pydischarge-0.0.2/pydischarge/table/io/
+-rw-rw-rw-   0        0        0     1635 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/io/__init__.py
+-rw-rw-rw-   0        0        0     3965 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/io/cwb.py
+-rw-rw-rw-   0        0        0     4864 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/io/fetch.py
+-rw-rw-rw-   0        0        0     4833 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/io/gravityspy.py
+-rw-rw-rw-   0        0        0     8693 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/io/gstlal.py
+-rw-rw-rw-   0        0        0     5645 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/io/gwf.py
+-rw-rw-rw-   0        0        0     5391 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/io/hacr.py
+-rw-rw-rw-   0        0        0    14039 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/io/ligolw.py
+-rw-rw-rw-   0        0        0     4625 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/io/losc.py
+-rw-rw-rw-   0        0        0     2726 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/io/omega.py
+-rw-rw-rw-   0        0        0     1400 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/io/omicron.py
+-rw-rw-rw-   0        0        0     9239 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/io/pycbc.py
+-rw-rw-rw-   0        0        0     3463 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/io/root.py
+-rw-rw-rw-   0        0        0     4008 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/io/snax.py
+-rw-rw-rw-   0        0        0     3195 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/io/sql.py
+-rw-rw-rw-   0        0        0     3335 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/io/utils.py
+-rw-rw-rw-   0        0        0    27321 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/table.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:33.006437 pydischarge-0.0.2/pydischarge/table/tests/
+-rw-rw-rw-   0        0        0      801 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/tests/__init__.py
+-rw-rw-rw-   0        0        0     3536 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/tests/test_gravityspy.py
+-rw-rw-rw-   0        0        0     8230 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/tests/test_io_gstlal.py
+-rw-rw-rw-   0        0        0     2986 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/tests/test_io_ligolw.py
+-rw-rw-rw-   0        0        0     8666 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/tests/test_io_pycbc.py
+-rw-rw-rw-   0        0        0    31317 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/table/tests/test_table.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:33.023437 pydischarge-0.0.2/pydischarge/testing/
+-rw-rw-rw-   0        0        0      800 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/testing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:33.040436 pydischarge-0.0.2/pydischarge/testing/data/
+-rw-rw-rw-   0        0        0    58124 2023-05-02 15:35:55.000000 pydischarge-0.0.2/pydischarge/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz
+-rw-rw-rw-   0        0        0   377295 2023-05-02 15:35:55.000000 pydischarge-0.0.2/pydischarge/testing/data/HLV-HW100916-968654552-1.gwf
+-rw-rw-rw-   0        0        0   382679 2023-05-02 15:35:55.000000 pydischarge-0.0.2/pydischarge/testing/data/HLV-HW100916-968654552-1.hdf
+-rw-rw-rw-   0        0        0       63 2023-05-02 15:35:55.000000 pydischarge-0.0.2/pydischarge/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.txt
+-rw-rw-rw-   0        0        0      564 2023-05-02 15:35:55.000000 pydischarge-0.0.2/pydischarge/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.xml.gz
+-rw-rw-rw-   0        0        0     2921 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/testing/errors.py
+-rw-rw-rw-   0        0        0     3949 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/testing/fixtures.py
+-rw-rw-rw-   0        0        0     1595 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/testing/marks.py
+-rw-rw-rw-   0        0        0     4299 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/testing/mocks.py
+-rw-rw-rw-   0        0        0    12211 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/testing/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:33.047435 pydischarge-0.0.2/pydischarge/time/
+-rw-rw-rw-   0        0        0     1897 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/time/__init__.py
+-rw-rw-rw-   0        0        0     2387 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/time/__main__.py
+-rw-rw-rw-   0        0        0     9344 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/time/_tconvert.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:33.054436 pydischarge-0.0.2/pydischarge/time/tests/
+-rw-rw-rw-   0        0        0      800 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/time/tests/__init__.py
+-rw-rw-rw-   0        0        0     1452 2023-05-09 15:37:50.000000 pydischarge-0.0.2/pydischarge/time/tests/test_main.py
+-rw-rw-rw-   0        0        0     6007 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/time/tests/test_time.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:33.066437 pydischarge-0.0.2/pydischarge/timeseries/
+-rw-rw-rw-   0        0        0     1191 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/__init__.py
+-rw-rw-rw-   0        0        0    59015 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/core.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:33.088438 pydischarge-0.0.2/pydischarge/timeseries/io/
+-rw-rw-rw-   0        0        0      996 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/io/__init__.py
+-rw-rw-rw-   0        0        0     1250 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/io/ascii.py
+-rw-rw-rw-   0        0        0     2732 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/io/cache.py
+-rw-rw-rw-   0        0        0     4888 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/io/core.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:33.101436 pydischarge-0.0.2/pydischarge/timeseries/io/gwf/
+-rw-rw-rw-   0        0        0    13652 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/io/gwf/__init__.py
+-rw-rw-rw-   0        0        0    17867 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/io/gwf/framecpp.py
+-rw-rw-rw-   0        0        0     4971 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/io/gwf/framel.py
+-rw-rw-rw-   0        0        0     7091 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/io/gwf/lalframe.py
+-rw-rw-rw-   0        0        0     4373 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/io/hdf5.py
+-rw-rw-rw-   0        0        0     9694 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/io/losc.py
+-rw-rw-rw-   0        0        0     8044 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/io/nds2.py
+-rw-rw-rw-   0        0        0     3763 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/io/wav.py
+-rw-rw-rw-   0        0        0    37118 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/statevector.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:33.147436 pydischarge-0.0.2/pydischarge/timeseries/tests/
+-rw-rw-rw-   0        0        0      806 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/tests/__init__.py
+-rw-rw-rw-   0        0        0    18807 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/tests/test_core.py
+-rw-rw-rw-   0        0        0     2397 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/tests/test_io_gwf_framecpp.py
+-rw-rw-rw-   0        0        0     5274 2023-05-09 15:37:50.000000 pydischarge-0.0.2/pydischarge/timeseries/tests/test_io_gwf_lalframe.py
+-rw-rw-rw-   0        0        0     1936 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/tests/test_io_losc.py
+-rw-rw-rw-   0        0        0    12771 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/tests/test_statevector.py
+-rw-rw-rw-   0        0        0    56795 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/tests/test_timeseries.py
+-rw-rw-rw-   0        0        0    90449 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/timeseries/timeseries.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:33.165435 pydischarge-0.0.2/pydischarge/types/
+-rw-rw-rw-   0        0        0     1221 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/types/__init__.py
+-rw-rw-rw-   0        0        0    15829 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/types/array.py
+-rw-rw-rw-   0        0        0    12822 2023-05-09 15:37:50.000000 pydischarge-0.0.2/pydischarge/types/array2d.py
+-rw-rw-rw-   0        0        0     3204 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/types/index.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:33.178436 pydischarge-0.0.2/pydischarge/types/io/
+-rw-rw-rw-   0        0        0      960 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/types/io/__init__.py
+-rw-rw-rw-   0        0        0     3000 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/types/io/ascii.py
+-rw-rw-rw-   0        0        0     8291 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/types/io/hdf5.py
+-rw-rw-rw-   0        0        0     7535 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/types/io/ligolw.py
+-rw-rw-rw-   0        0        0    37977 2023-05-09 15:37:50.000000 pydischarge-0.0.2/pydischarge/types/series.py
+-rw-rw-rw-   0        0        0     3725 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/types/sliceutils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:33.208438 pydischarge-0.0.2/pydischarge/types/tests/
+-rw-rw-rw-   0        0        0      801 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/types/tests/__init__.py
+-rw-rw-rw-   0        0        0     8943 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/types/tests/test_array.py
+-rw-rw-rw-   0        0        0     9389 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/types/tests/test_array2d.py
+-rw-rw-rw-   0        0        0     2176 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/types/tests/test_index.py
+-rw-rw-rw-   0        0        0    15217 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/types/tests/test_series.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:33.232437 pydischarge-0.0.2/pydischarge/utils/
+-rw-rw-rw-   0        0        0     1000 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/__init__.py
+-rw-rw-rw-   0        0        0     3876 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/decorators.py
+-rw-rw-rw-   0        0        0     1570 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/enum.py
+-rw-rw-rw-   0        0        0     2030 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/env.py
+-rw-rw-rw-   0        0        0     8897 2023-05-09 15:37:50.000000 pydischarge-0.0.2/pydischarge/utils/lal.py
+-rw-rw-rw-   0        0        0     3480 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/misc.py
+-rw-rw-rw-   0        0        0     5256 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/mp.py
+-rw-rw-rw-   0        0        0     1441 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/progress.py
+-rw-rw-rw-   0        0        0     3558 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/shell.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:33.243437 pydischarge-0.0.2/pydischarge/utils/sphinx/
+-rw-rw-rw-   0        0        0      825 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/sphinx/__init__.py
+-rw-rw-rw-   0        0        0     3663 2023-05-02 15:35:55.000000 pydischarge-0.0.2/pydischarge/utils/sphinx/epydoc.py
+-rw-rw-rw-   0        0        0     4983 2023-05-09 15:37:50.000000 pydischarge-0.0.2/pydischarge/utils/sphinx/ex2rst.py
+-rw-rw-rw-   0        0        0     3558 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/sphinx/zenodo.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:33.267436 pydischarge-0.0.2/pydischarge/utils/tests/
+-rw-rw-rw-   0        0        0      801 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/tests/__init__.py
+-rw-rw-rw-   0        0        0     2338 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/tests/test_decorators.py
+-rw-rw-rw-   0        0        0     2309 2023-05-09 15:37:50.000000 pydischarge-0.0.2/pydischarge/utils/tests/test_enum.py
+-rw-rw-rw-   0        0        0     2121 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/tests/test_env.py
+-rw-rw-rw-   0        0        0     3640 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/tests/test_lal.py
+-rw-rw-rw-   0        0        0     2777 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/tests/test_misc.py
+-rw-rw-rw-   0        0        0     2162 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/tests/test_mp.py
+-rw-rw-rw-   0        0        0     2479 2023-05-09 15:34:14.000000 pydischarge-0.0.2/pydischarge/utils/tests/test_shell.py
+-rw-rw-rw-   0        0        0     2446 2023-05-09 15:37:50.000000 pydischarge-0.0.2/pydischarge/utils/tests/test_sphinx_ex2rst.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:49:32.568963 pydischarge-0.0.2/pydischarge.egg-info/
+-rw-rw-rw-   0        0        0     3513 2023-05-09 15:49:31.000000 pydischarge-0.0.2/pydischarge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11764 2023-05-09 15:49:31.000000 pydischarge-0.0.2/pydischarge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 15:49:31.000000 pydischarge-0.0.2/pydischarge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-05-09 15:49:31.000000 pydischarge-0.0.2/pydischarge.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      793 2023-05-09 15:49:31.000000 pydischarge-0.0.2/pydischarge.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-09 15:49:31.000000 pydischarge-0.0.2/pydischarge.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5154 2023-05-09 15:37:50.000000 pydischarge-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 15:49:33.271436 pydischarge-0.0.2/setup.cfg
```

### Comparing `pydischarge-0.0.1/.github/workflows/conda.yml` & `pydischarge-0.0.2/.github/workflows/conda.yml`

 * *Files 2% similar despite different names*

```diff
@@ -144,22 +144,22 @@
         sudo bash -c 'cat > /etc/cvmfs/default.local' << EOF
         CVMFS_REPOSITORIES=gwosc.osgstorage.org
         CVMFS_QUOTA_LIMIT=20000
         CVMFS_HTTP_PROXY=DIRECT
         EOF
         sudo cvmfs_config probe
 
-    - name: Install PDpy
+    - name: Install pyDischarge
       run: python -m pip install .[dev] --no-build-isolation -vv
 
     - name: Package list
       run: conda list --name test
 
     - name: Run test suite
-      run: python -m pytest -ra --color yes --cov pdpy --cov-report=xml --junitxml=pytest.xml --numprocesses=auto pdpy/ examples/
+      run: python -m pytest -ra --color yes --cov pydischarge --cov-report=xml --junitxml=pytest.xml --numprocesses=auto pydischarge/ examples/
 
     - name: Coverage report
       run: python -m coverage report --show-missing
 
     - name: Publish coverage to Codecov
       uses: codecov/codecov-action@v3
       with:
```

### Comparing `pydischarge-0.0.1/.github/workflows/dependencies.yml` & `pydischarge-0.0.2/.github/workflows/dependencies.yml`

 * *Files 4% similar despite different names*

```diff
@@ -79,23 +79,23 @@
             -e 's/requires-python = "==/requires-python = ">=/' \
             pyproject.toml
 
     - name: Install system packages for experimental dependencies
       if: matrix.experimental == true
       run: sudo apt-get -y -q install libkrb5-dev
 
-    - name: Install PDpy and dependencies
+    - name: Install pyDischarge and dependencies
       run: python -m pip install .[${{ matrix.extras }}] ${{ matrix.pip-opts }}
 
     - name: Package list
       run: python -m pip list installed
 
     - name: Run test suite
       id: pytest
-      run: python -m pytest -ra --color yes --cov pdpy --pyargs pdpy --cov-report=xml --junitxml=pytest.xml
+      run: python -m pytest -ra --color yes --cov pydischarge --pyargs pydischarge --cov-report=xml --junitxml=pytest.xml
 
     - name: Coverage report
       run: python -m coverage report --show-missing
 
     - name: Publish coverage to Codecov
       uses: codecov/codecov-action@v1.2.1
       with:
```

### Comparing `pydischarge-0.0.1/.github/workflows/dist.yml` & `pydischarge-0.0.2/.github/workflows/dist.yml`

 * *Files 5% similar despite different names*

```diff
@@ -51,20 +51,20 @@
 
     - name: Create distributions
       run: python -m build . --sdist --wheel --outdir .
 
     - uses: actions/upload-artifact@v2
       with:
         name: tarball
-        path: pdpy-*.tar.*
+        path: pydischarge-*.tar.*
 
     - uses: actions/upload-artifact@v2
       with:
         name: wheel
-        path: pdpy*.whl
+        path: pydischarge*.whl
 
   # -- pip install test -----
 
   pip-install:
     name: Python ${{ matrix.python-version }} install from ${{ matrix.artifact }} (${{ matrix.os }})
 
     needs:
@@ -97,33 +97,33 @@
         name: ${{ matrix.artifact }}
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
 
-    - name: Install PDpy with test extras
+    - name: Install pyDischarge with test extras
       run: |
         # extras don't work with wildcards
-        DIST=$(ls pdpy-*.*)
+        DIST=$(ls pydischarge-*.*)
         python -m pip install ${DIST}[test]
 
     - name: Package list
       run: python -m pip list installed
 
     - name: Run test suite
       run: |
         python -m pytest \
             -ra \
             --color yes \
-            --cov pdpy \
+            --cov pydischarge \
             --cov-report=xml \
             --disable-socket \
             --junitxml=pytest.xml \
-            --pyargs pdpy \
+            --pyargs pydischarge \
         ;
 
     - name: Coverage report
       run: python -m coverage report --show-missing
 
     - name: Publish coverage to Codecov
       uses: codecov/codecov-action@v3
```

### Comparing `pydischarge-0.0.1/.github/workflows/documentation.yml` & `pydischarge-0.0.2/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.1/.github/workflows/lint.yml` & `pydischarge-0.0.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.1/.gitignore` & `pydischarge-0.0.2/.gitignore`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
 dist/
 eggs/
-/pdpy/_version.py
+/pydischarge/_version.py
 lib/
 lib64/
 parts/
 sdist/
 var/
 venv/
 *.egg-info/
```

### Comparing `pydischarge-0.0.1/CONTRIBUTING.md` & `pydischarge-0.0.2/CONTRIBUTING.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Contributing to PDpy
+# Contributing to pyDischarge
 
 ## Reporting Issues
 
 When opening an issue to report a problem, please try to provide a minimal code
 example that reproduces the issue along with details of the operating
-system and the Python, NumPy, Astropy, and PDpy versions you are using.
+system and the Python, NumPy, Astropy, and pyDischarge versions you are using.
 
 ## Contributing Code
 
 **Imposter syndrome disclaimer**: We want your help. No, really.
 
 There may be a little voice inside your head that is telling you that you're not
 ready to be an open source contributor; that your skills aren't nearly good
@@ -27,40 +27,40 @@
 process). Some of these contributions may be the most valuable to the project as
 a whole, because you're coming to the project with fresh eyes, so you can see
 the errors and assumptions that seasoned contributors have glossed over.
 
 Note: This disclaimer was originally written by
 [Adrienne Lowe](https://github.com/adriennefriend) for a
 [PyCon talk](https://www.youtube.com/watch?v=6Uj746j9Heo), and was adapted for
-PDpy based on its use in the [Astropy](https://github.com/astropy/astropy/)
+pyDischarge based on its use in the [Astropy](https://github.com/astropy/astropy/)
 contributing guide.
 
 ## Development model
 
-Contributions to PDpy are made via pull requests from GitHub users' forks of
-the main [pdpy repositories](https://github.com/pdpy/pdpy), following the
+Contributions to pyDischarge are made via pull requests from GitHub users' forks of
+the main [pydischarge repositories](https://github.com/pydischarge/pydischarge), following the
 [GitHub flow](https://guides.github.com/introduction/flow/) workflow.
 The basic idea is that all changes are proposed using a dedicated _feature_
 branch:
 
 - create the fork (if needed) by clicking _Fork_ in the upper-right corner of
-  <https://github.com/pdpy/pdpy/> - this only needs to be done once, ever
+  <https://github.com/pydischarge/pydischarge/> - this only needs to be done once, ever
 
 - clone the main repo, calling it `upstream` in the git configuration:
 
   ```bash
-  git clone https://github.com/pdpy/pdpy.git pdpy --origin upstream
-  cd pdpy
+  git clone https://github.com/pydischarge/pydischarge.git pydischarge --origin upstream
+  cd pydischarge
   ```
 
 - add your fork as the `origin` remote (replace `<username>` with your
   GitHub username):
 
   ```bash
-  git remote add origin git@github.com:<username>/pdpy.git
+  git remote add origin git@github.com:<username>/pydischarge.git
   ```
 
 - create a new branch on which to work
 
   ```bash
   git checkout -b my-new-branch
   ```
@@ -70,15 +70,15 @@
 - push changes to your remote on github.com
 
   ```bash
   git push -u origin my-new-branch
   ```
 
 - open a merge request on github.com, this will trigger a code review by one
-  of the PDpy maintainers, who may suggest modifications to your proposed
+  of the pyDischarge maintainers, who may suggest modifications to your proposed
   changes
 
 - to update your feature branch with the latest changes from the `main` branch
   of the `upstream` repository:
 
   ```bash
   git pull --rebase upstream main
@@ -96,15 +96,15 @@
 - finally, if your Pull Request is merged, you should 'delete the source branch'
   (there's a button), to keep your fork clean
 
 ## Coding guidelines
 
 ### Python compatibility
 
-**PDpy code must be compatible with Python >= 3.7.**
+**pyDischarge code must be compatible with Python >= 3.7.**
 
 ### Style
 
 This package follows [PEP 8](https://www.python.org/dev/peps/pep-0008/),
 and all code should adhere to that as far as is reasonable.
 
 The first stage in the automated testing of pull requests is a job that runs
@@ -113,17 +113,17 @@
 
 ```bash
 python3 -m flake8
 ```
 
 ### Testing
 
-PDpy has a fairly complete test suite, covering over 90% of the codebase.
+pyDischarge has a fairly complete test suite, covering over 90% of the codebase.
 All code contributions should be accompanied by (unit) tests to be executed with
 [`pytest`](https://docs.pytest.org/en/latest/), and should cover
 all new or modified lines.
 
 You can run the test suite locally from the root of the repository via:
 
 ```bash
-python3 -m pytest pdpy/
+python3 -m pytest pydischarge/
 ```
```

### Comparing `pydischarge-0.0.1/LICENSE` & `pydischarge-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.1/docs/Makefile` & `pydischarge-0.0.2/docs/Makefile`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # vim: ts=4:noet
 # Makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line.
 SPHINXOPTS    =
 SPHINXBUILD   = python -m sphinx
-SPHINXPROJ    = pdpy
+SPHINXPROJ    = pydischarge
 SOURCEDIR     = .
 BUILDDIR      = ../build/sphinx
 
 .PHONY: help html
 
 # Put it first so that "make" without argument is like "make help".
 help:
```

### Comparing `pydischarge-0.0.1/docs/_static/css/gwpy-sphinx.css` & `pydischarge-0.0.2/docs/_static/css/gwpy-sphinx.css`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 /* Copyright (C) Louisiana State University (2014-2017)
  *               Cardiff University (2017-2022)
  *
- * This file is part of PDpy.
+ * This file is part of pyDischarge.
  *
- * PDpy is free software: you can redistribute it and/or modify
+ * pyDischarge is free software: you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
- * PDpy is distributed in the hope that it will be useful,
+ * pyDischarge is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
- * along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+ * along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 /*
- * This file contains sphinx-specific extensions to the core PDpy CSS
+ * This file contains sphinx-specific extensions to the core pyDischarge CSS
  */
 
 /* change font for parameter names for callables */
 .field-list p strong {
 		font-family: "Roboto Mono", "Courier New", Courier, monospace;
 }
```

### Comparing `pydischarge-0.0.1/docs/_static/favicon.png` & `pydischarge-0.0.2/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.1/docs/_static/gwpy_white_24.png` & `pydischarge-0.0.2/docs/_static/gwpy_white_24.png`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.1/docs/_templates/autoclass/class.rst` & `pydischarge-0.0.2/docs/_templates/autoclass/class.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.1/docs/_templates/autosummary/class.rst` & `pydischarge-0.0.2/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.1/docs/_templates/autosummary/module.rst` & `pydischarge-0.0.2/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.1/docs/astro/index.rst` & `pydischarge-0.0.2/docs/astro/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-.. currentmodule:: pdpy.astro
+.. currentmodule:: pydischarge.astro
 
-.. _pdpy-astro:
+.. _pydischarge-astro:
 
 #######################
 Astrophysical modelling
 #######################
 
-Currently the only methods available from `pdpy.astro` are concerned with calculating sensitive distance.
+Currently the only methods available from `pydischarge.astro` are concerned with calculating sensitive distance.
 
-.. _pdpy-astro-range:
+.. _pydischarge-astro-range:
 
 ==================
 Sensitive distance
 ==================
 
 The sensitive distance (sometimes called 'range', or 'horizon') is a measure of how far out into the universe a gravitational-wave source can be and still be detectable by a gravitational-wave detector 
 
-`pdpy.astro` provides methods to calculate the distance to simple models of inspiral and burst signals:
+`pydischarge.astro` provides methods to calculate the distance to simple models of inspiral and burst signals:
 
 .. autosummary::
    :toctree: ../api
 
    burst_range
    burst_range_spectrum
    inspiral_range
```

### Comparing `pydischarge-0.0.1/docs/citing.rst.in` & `pydischarge-0.0.2/docs/citing.rst.in`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ###########
-Citing PDpy
+Citing pyDischarge
 ###########
 
-If you have used PDpy as part of a project that leads to a scientific
+If you have used pyDischarge as part of a project that leads to a scientific
 publication, please acknowledge this by citing the
-`PDpy paper <https://www.sciencedirect.com/science/article/pii/S2352711021000029>`_: D. M. Macleod *et al*, SoftwareX, **13**, 100657 (2021). The citation in various formats is given below:
+`pyDischarge paper <https://www.sciencedirect.com/science/article/pii/S2352711021000029>`_: D. M. Macleod *et al*, SoftwareX, **13**, 100657 (2021). The citation in various formats is given below:
 
 .. tabbed:: BibTeX
 
    .. code-block:: bibtex
 
-      @article{pdpy,
-          title = "{PDpy: A Python package for gravitational-wave astrophysics}",
+      @article{pydischarge,
+          title = "{pyDischarge: A Python package for gravitational-wave astrophysics}",
          author = {{Macleod}, D.~M. and {Areeda}, J.~S. and {Coughlin}, S.~B. and {Massinger}, T.~J. and {Urban}, A.~L.},
         journal = {SoftwareX},
          volume = 13,
           pages = 100657,
            year = 2021,
            issn = {2352-7110},
             doi = {10.1016/j.softx.2021.100657},
@@ -23,15 +23,15 @@
       }
 
 .. tabbed:: RIS
 
    .. code-block::
 
       TY  - JOUR
-      T1  - PDpy: A Python package for gravitational-wave astrophysics
+      T1  - pyDischarge: A Python package for gravitational-wave astrophysics
       AU  - Macleod, Duncan M.
       AU  - Areeda, Joseph S.
       AU  - Coughlin, Scott B.
       AU  - Massinger, Thomas J.
       AU  - Urban, Alexander L.
       JO  - SoftwareX
       VL  - 13
@@ -44,15 +44,15 @@
       ER  - 
 
 .. tabbed:: EndNode
 
    .. code-block::
 
       %0 Journal Article
-      %T PDpy: A Python package for gravitational-wave astrophysics
+      %T pyDischarge: A Python package for gravitational-wave astrophysics
       %A Macleod, Duncan M.
       %A Areeda, Joseph S.
       %A Coughlin, Scott B.
       %A Massinger, Thomas J.
       %A Urban, Alexander L.
       %J SoftwareX
       %V 13
@@ -62,28 +62,28 @@
       %@ 2352-7110
 
 .. tabbed:: RefWorks
 
    .. code-block::
 
       RT Journal
-      T1 PDpy: A Python package for gravitational-wave astrophysics
+      T1 pyDischarge: A Python package for gravitational-wave astrophysics
       A1 Macleod, Duncan M.
       A1 Areeda, Joseph S.
       A1 Coughlin, Scott B.
       A1 Massinger, Thomas J.
       A1 Urban, Alexander L.
       JF SoftwareX
       VO 13
       SP 100657
       YR 2021
       DO DOI: 10.1016/j.softx.2021.100657
       SN 2352-7110
 
-Also cite the DOI for the version of PDpy that you have used.
+Also cite the DOI for the version of pyDischarge that you have used.
 Each of the DOIs below resolves a Zenodo record for that version.
 See the *Export* section on each page for formatted citations in a number
 of common styles.
 
-The list below includes only the 10 most recent releases of PDpy.
+The list below includes only the 10 most recent releases of pyDischarge.
 For older versions, please
 `click here <https://zenodo.org//search?page=2&size=10&q=conceptrecid:"597016"&sort=-version&all_versions=True>`__.
```

### Comparing `pydischarge-0.0.1/docs/cli/examples.ini` & `pydischarge-0.0.2/docs/cli/examples.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 ;
-; ## Examples of pdpy-plot ##
+; ## Examples of pydischarge-plot ##
 ;
 ; Each example here should follow the following format:
 ;
 ; [example-name]
 ; command = <action> <arguments> <options>
 ; title = RST Page Title (optional)
 ; description = some text to display after the header (optional)
 ;
 ; The `command` option *should not include*:
-;     - the pdpy-plot executable name
+;     - the pydischarge-plot executable name
 ;     - any output file/directory options
 ;
 ; If your `command` is
 ;
 ; timeseries --chan H1:GDS-CALIB_STRAIN --start 1126259457
 ;
 ; this will get rendered in the documentation as
 ;
-; pdpy-plot timeseries \
+; pydischarge-plot timeseries \
 ;     --chan H1:GDS-CALIB_STRAIN \
 ;     --start 1126259457 \
 ;     --interactive
 ;
 ; and executed by sphinx on the build machine as
 ;
-; pdpy-plot timeseries --chan H1:GDS-CALIB_STRAIN --start 1126259457 --out <some filename>
+; pydischarge-plot timeseries --chan H1:GDS-CALIB_STRAIN --start 1126259457 --out <some filename>
 ;
 
 ; -- timeseries ---------------------------------
 
 [timeseries-simple]
 command =
 	timeseries
@@ -57,15 +57,15 @@
 	--ylabel 'Strain amplitude'
 	--geometry 1200x400
 	--suptitle 'LIGO-Hanford strain (filtered) around GW150914'
 title = Filtered timeseries
 description =
 	This example shows the strain timeseries for the LIGO-Hanford detector
 	around GW150914 filtered to emphasise the visibility of the known signal
-	(see :ref:`pdpy-example-signal-gw150914` for more detail).
+	(see :ref:`pydischarge-example-signal-gw150914` for more detail).
 
 [timeseries-long]
 command =
 	timeseries
 	--chan H1:DMT-SNSH_EFFECTIVE_RANGE_MPC.mean
 	--chan L1:DMT-SNSH_EFFECTIVE_RANGE_MPC.mean
 	--start 'August 17 2017'
@@ -149,15 +149,15 @@
 	--ifo H1
 	--start 1264316116
 	--duration 32
 	--epoch 1264316116.4
 	--ymax 4000
 title = Simple spectrogram
 description =
-	This example shows a :ref:`spectrogram <pdpy-spectrogram>` of the strain
+	This example shows a :ref:`spectrogram <pydischarge-spectrogram>` of the strain
 	data from LIGO-Hanford around the time of GW150914.
 
 [spectrogram-norm]
 command =
 	spectrogram
 	--gwosc
 	--ifo L1
@@ -165,15 +165,15 @@
 	--duration 1024
 	--norm
 	--cmap Spectral_r
 	--imin .25
 	--imax 4
 title = Normalised spectrogram
 description =
-	This example shows a normalised :ref:`spectrogram <pdpy-spectrogram>` of
+	This example shows a normalised :ref:`spectrogram <pydischarge-spectrogram>` of
 	the strain data from LIGO-Hanford around the time of GW150914.
 
 ; -- coherence-----------------------------------
 
 [coherence]
 command =
 	coherence
@@ -193,12 +193,12 @@
 command =
 	coherencegram
 	--chan H1:GDS-CALIB_STRAIN H1:PEM-CS_ACC_PSL_PERISCOPE_X_DQ
 	--start 1126260017
 	--duration 600
 title = Simple coherence spectrogram
 description =
-	This example shows the time-variation :ref:`spectrogram <pdpy-spectrogram>`
+	This example shows the time-variation :ref:`spectrogram <pydischarge-spectrogram>`
 	of the estimated coherence between the strain data for
 	LIGO-Hanford (``H1:GDS-CALIB_STRAIN``) and the motion of an optical
 	periscope used to direct the main laser beam into the Hanford
 	interferometer.
```

### Comparing `pydischarge-0.0.1/docs/cli/index.rst` & `pydischarge-0.0.2/docs/cli/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 *******************************
-Command line plotting with PDpy
+Command line plotting with pyDischarge
 *******************************
 
-The ``pdpy-plot`` command-line script provides a terminal-based user interface
+The ``pydischarge-plot`` command-line script provides a terminal-based user interface
 to querying data and generating images.
 Functionality for this tool is primarily inspired by LigoDV-web
 (LDVW, https://ldvw.ligo.caltech.edu), a web tool for viewing LIGO data,
 available to members of the joint LIGO-Virgo collaboration.
-LDVW, written in Java, uses the ``pdpy-plot`` command-line script provided by
-PDpy to generate the plots based on web-form input from the user.
+LDVW, written in Java, uses the ``pydischarge-plot`` command-line script provided by
+pyDischarge to generate the plots based on web-form input from the user.
 
-The basic usage for `pdpy-plot` is as follows:
+The basic usage for `pydischarge-plot` is as follows:
 
 .. code-block:: bash
 
-    pdpy-plot <ACTION> --chan <channel-name> --start <gps-start-time> [OPTIONS]
+    pydischarge-plot <ACTION> --chan <channel-name> --start <gps-start-time> [OPTIONS]
 
 Where ``<ACTION>`` is the type of plot to make.
 
-You can run ``pdpy-plot --help`` to list the plot types ('actions') you can use:
+You can run ``pydischarge-plot --help`` to list the plot types ('actions') you can use:
 
-.. command-output:: pdpy-plot --help
+.. command-output:: pydischarge-plot --help
 
 To see the arguments and options for a given action, you can run, for example,
-``pdpy-plot timeseries --help``:
+``pydischarge-plot timeseries --help``:
 
-.. command-output:: pdpy-plot timeseries --help
+.. command-output:: pydischarge-plot timeseries --help
 
 The options for each action vary but many are common.
 
 =====================
 Specifying input data
 =====================
 
-.. currentmodule:: pdpy.timeseries
+.. currentmodule:: pydischarge.timeseries
 
 The following table summarises the allowed number of inputs for each action
 
 +-------------------+--------------------+-----------------+
 | Action            | Number of channels | Number of times |
 +===================+====================+=================+
 | ``timeseries``    | >=1                | >=1             |
```

### Comparing `pydischarge-0.0.1/docs/conf.py` & `pydischarge-0.0.2/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017),
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 import inspect
 import os.path
 import re
 import shlex
 import shutil
 import sys
@@ -30,31 +30,31 @@
 
 import matplotlib
 
 from sphinx.util import logging
 
 from numpydoc import docscrape_sphinx
 
-import pdpy
-from pdpy.utils.sphinx import (
+import pydischarge
+from pydischarge.utils.sphinx import (
     ex2rst,
     zenodo,
 )
 
 SPHINX_DIR = Path(__file__).parent.absolute()
 STATIC_DIRNAME = "_static"
 
-# use caching in PDpy calls
+# use caching in pyDischarge calls
 os.environ.update({
     "GWPY_CACHE": "true",
 })
 
 # -- versions ---------------
 
-GWPY_VERSION = pdpy.__version__
+GWPY_VERSION = pydischarge.__version__
 
 # parse version number to get git reference
 _setuptools_scm_version_regex = re.compile(
     r"\+g(\w+)(?:\Z|\.)",
 )
 if match := _setuptools_scm_version_regex.search(GWPY_VERSION):
     GWPY_GIT_REF, = match.groups()
@@ -65,23 +65,23 @@
 
 matplotlib.use('agg')
 
 # ignore warnings that aren't useful for documentation
 if "CI" not in os.environ:
     for message, category in (
         (".*non-GUI backend.*", UserWarning),
-        (".*pdpy.plot.*", DeprecationWarning),
+        (".*pydischarge.plot.*", DeprecationWarning),
         ("", matplotlib.MatplotlibDeprecationWarning),
     ):
         warnings.filterwarnings("ignore", message=message, category=category)
 
 # -- general ----------------
 
 needs_sphinx = "4.0"
-project = 'PDpy'
+project = 'pyDischarge'
 copyright = ' and '.join((
     '2013, 2017-2021 Cardiff University',
     '2013-2017 Lousiana State University',
 ))
 version = "dev" if ".dev" in GWPY_VERSION else GWPY_VERSION
 release = GWPY_VERSION
 
@@ -101,15 +101,15 @@
     'sphinx.ext.ifconfig',
     'sphinx_automodapi.automodapi',
     'sphinx_panels',
     'sphinxcontrib.programoutput',
     'numpydoc',
     'matplotlib.sphinxext.plot_directive',
     #'sphinxcontrib.doxylink',  # noqa: E265
-    'pdpy.utils.sphinx.epydoc',
+    'pydischarge.utils.sphinx.epydoc',
 ]
 
 # content management
 default_role = "obj"
 exclude_patterns = [
     "references.rst",
     "_build",
@@ -125,17 +125,17 @@
 
 # -- HTML formatting --------
 
 extensions.append("sphinx_immaterial")
 html_theme = "sphinx_immaterial"
 html_theme_options = {
     # metadata
-    "repo_name": "PDpy",
+    "repo_name": "pyDischarge",
     "repo_type": "github",
-    "repo_url": "https://github.com/pdpy-github/pdpy",
+    "repo_url": "https://github.com/pydischarge-github/pydischarge",
     "edit_uri": "blob/main/docs",
     "globaltoc_collapse": True,
     # features
     "features": [
         "navigation.sections",
     ],
     # colouring and light/dark mode
@@ -166,15 +166,15 @@
     # version dropdown
     "version_dropdown": True,
     "version_json": "../versions.json",
 }
 html_static_path = [STATIC_DIRNAME]
 html_favicon = str(Path(STATIC_DIRNAME) / "favicon.png")
 html_logo = str(Path(STATIC_DIRNAME) / "favicon.png")
-html_css_files = ["css/pdpy-sphinx.css"]
+html_css_files = ["css/pydischarge-sphinx.css"]
 
 # -- extensions config ------
 
 # -- autodoc
 
 autoclass_content = 'class'
 autodoc_default_flags = ['show-inheritance', 'members', 'inherited-members']
@@ -277,15 +277,15 @@
             obj = getattr(obj, part)
         try:  # unwrap a decorator
             obj = obj.im_func.func_closure[0].cell_contents
         except (AttributeError, TypeError):
             pass
         # get filename
         filename = Path(inspect.getsourcefile(obj)).relative_to(
-            Path(pdpy.__file__).parent,
+            Path(pydischarge.__file__).parent,
         ).as_posix()
         # get line numbers of this object
         source, lineno = inspect.getsourcelines(obj)
         if lineno:
             return "{}#L{:d}-L{:d}".format(
                 filename,
                 lineno,
@@ -295,19 +295,19 @@
 
     try:
         fileref = find_source(info["module"], info["fullname"])
     except (
         AttributeError,  # object not found
         OSError,  # file not found
         TypeError,  # source for object not found
-        ValueError,  # file not from PDpy
+        ValueError,  # file not from pyDischarge
     ):
         return None
 
-    return "https://github.com/pdpy-github/pdpy/tree/{}/pdpy/{}".format(
+    return "https://github.com/pydischarge-github/pydischarge/tree/{}/pydischarge/{}".format(
         GWPY_GIT_REF,
         fileref,
     )
 
 
 # -- plugins ----------------
 
@@ -317,15 +317,15 @@
 .. toctree::
    :numbered:
 
    ${examples}
 """.strip())
 
 CLI_TEMPLATE = Template("""
-.. _pdpy-cli-example-${tag}:
+.. _pydischarge-cli-example-${tag}:
 
 ${titleunderline}
 ${title}
 ${titleunderline}
 
 ${description}
 
@@ -351,39 +351,39 @@
     try:
         return Path(target).read_text() != content
     except FileNotFoundError:
         return True
 
 
 def _render_cli_example(config, section, outdir, logger):
-    """Render a :mod:`pdpy.cli` example as RST to be processed by Sphinx.
+    """Render a :mod:`pydischarge.cli` example as RST to be processed by Sphinx.
     """
     # read config values (allow for multi-line definition)
     raw = config.get(
         section,
         'command',
     ).strip().replace("\n", " ") + " --interactive"
     title = config.get(
         section,
         'title',
         fallback=' '.join(map(str.title, section.split('-'))),
     )
     desc = config.get(section, 'description', fallback='')
 
     # build command-line string for display
-    cmdstr = f"pdpy-plot {raw}".replace(  # split onto multiple lines
+    cmdstr = f"pydischarge-plot {raw}".replace(  # split onto multiple lines
         ' --',
         ' \\\n       --',
     )
 
     # build code to generate the plot when sphinx runs
     args = ", ".join(map(repr, shlex.split(raw)))
     code = "\n   ".join([
-        "from pdpy.cli.pdpy_plot import main as pdpy_plot",
-        f"pdpy_plot([{args}])",
+        "from pydischarge.cli.pydischarge_plot import main as pydischarge_plot",
+        f"pydischarge_plot([{args}])",
     ])
 
     rst = CLI_TEMPLATE.substitute(
         title=title,
         titleunderline='#' * len(title),
         description=desc,
         tag=section,
@@ -396,15 +396,15 @@
     if _new_or_different(rst, rstfile):
         rstfile.write_text(rst)
         logger.info("[cli] wrote {}".format(rstfile))
     return rstfile
 
 
 def render_cli_examples(_):
-    """Render all :mod:`pdpy.cli` examples as RST to be processed by Sphinx.
+    """Render all :mod:`pydischarge.cli` examples as RST to be processed by Sphinx.
     """
     logger = logging.getLogger('cli-examples')
 
     # directories
     clidir = SPHINX_DIR / "cli"
     exini = clidir / "examples.ini"
     exdir = clidir / "examples"
```

### Comparing `pydischarge-0.0.1/docs/detector/channel.rst` & `pydischarge-0.0.2/docs/detector/channel.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-.. currentmodule:: pdpy.detector
+.. currentmodule:: pydischarge.detector
 
-.. _pdpy-channel:
+.. _pydischarge-channel:
 
 ##########################
 The :class:`Channel` class
 ##########################
 
 .. code-block:: python
 
-   >>> from pdpy.detector import Channel
+   >>> from pydischarge.detector import Channel
 
 
 ====================
 What is a 'channel'?
 ====================
 
 Each of the laser-interferometer gravitational-wave detectors record thousands of different data streams capturing a single instrumental error or control signal, or the output of an environmental sensor.
@@ -20,15 +20,15 @@
 
    L1:PSS-ISS_PDB_OUT_DQ
 
 describes the output signal (``OUT``) from photodiode-B (``PDB``) inside the Intensity Stabilisation System (``ISS``) of the Pre-Stabilised Laser (``PSL``) powering the ``L1`` instrument, hosted at the LIGO Livingston Observatory. The ``DQ`` suffix indicates that this channel was recorded in data files for offline study (many more 'test point' channels are used only in real-time, and are never recorded).
 
 A simple representation of this physical signal is provided by the :class:`Channel` object::
 
-    >>> from pdpy.detector import Channel
+    >>> from pydischarge.detector import Channel
     >>> signal = Channel('L1:PSL-ISS_PDB_OUT_DQ')
 
 This new :class:`Channel` has a number of attributes that describe its source, derived from its name::
 
     >>> print(hoft.ifo)
     'L1'
     >>> print(hoft.system)
@@ -54,15 +54,15 @@
 ==========================================================
 The LIGO Channel Information System (https://cis.ligo.org)
 ==========================================================
 
 All of the LIGO interferometer data channels are recorded in the Channel Information System (https://cis.ligo.org), a queryable database containing the details of each channel recorded to disk from the observatories.
 The :meth:`Channel.query` `classmethod` allows you to query the database as follows::
 
-    >>> from pdpy.detector import Channel
+    >>> from pydischarge.detector import Channel
     >>> chan = Channel.query('L1:IMC-F_OUT_DQ')
     >>> print(chan.sample_rate)
     16384.0 Hz
     >>> print(chan.url)
     https://cis.ligo.org/channel/282666
     >>> print(chan.model)
     l1lsc
```

### Comparing `pydischarge-0.0.1/docs/dev/release.rst` & `pydischarge-0.0.2/docs/dev/release.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-.. _pdpy-dev-release:
+.. _pydischarge-dev-release:
 
 ####################
 Publishing a release
 ####################
 
-This page describes the steps required to author a release of PDpy.
+This page describes the steps required to author a release of pyDischarge.
 
 Notes:
 
-* pdpy uses the
+* pydischarge uses the
   `stable mainline <https://www.bitsnbites.eu/a-stable-mainline-branching-model-for-git/>`_
   branching model for releases
 * all release numbers must follow `Semantic Versioning 2 <segmver.org>`_ and
   include major, minor, and patch numbers, e.g. ``X.Y.Z`` rather than
   ``1.0`` or just ``1``
 
 ============
@@ -71,48 +71,48 @@
       # push main branch
       git push --signed=if-asked origin main
       # push new tag
       git push --signed=if-asked origin vX.Y.Z
 
 #. **Draft a release on GitHub**
 
-   * Go to https://github.com/pdpy-github/pdpy/releases/new
+   * Go to https://github.com/pydischarge-github/pydischarge/releases/new
    * Use ``vX.Y.Z`` as the *Tag version*
    * Use X.Y.Z as the *Release title*
    * Copy the tag message into the text box to serve as release notes
 
 #. **Publish the release documentation**
 
    This is done from the LDAS computing centre at Caltech:
 
    .. code-block:: bash
 
-      cd /home/duncan.macleod/pdpy-nightly-build/
+      cd /home/duncan.macleod/pydischarge-nightly-build/
       bash release-build.sh X.Y.Z
 
    Once that is complete (~20 minutes), a few manual updates must be made:
 
    .. code-block:: bash
 
-      cd /home/duncan.macleod/pdpy-nightly-build/pdpy-github.github.io/docs
+      cd /home/duncan.macleod/pydischarge-nightly-build/pydischarge-github.github.io/docs
       unlink stable && ln -s X.Y.Z stable
       sed -i 's/0.9.9/X.Y.Z/g' index.html
 
    The final command should be modified to replace the previous release ID
    with the current one.
 
    Then:
 
    .. code-block:: bash
 
       git commit --gpg-sign --message="X.Y.Z: release docs"
       git push --signed=if-asked  # <- this step needs an SSH key
 
    It should take ~5 minutes for the release documentation to actually
-   appear on https://pdpy-github.github.io/docs/
+   appear on https://pydischarge-github.github.io/docs/
 
 ==============
 Linked updates
 ==============
 
 Zenodo
 ------
@@ -132,22 +132,22 @@
 To create a new release on PyPI:
 
 .. code-block:: bash
 
    rm -rf dist/
    git checkout vX.Y.Z
    python -m build
-   python -m twine upload --sign dist/pdpy-*
+   python -m twine upload --sign dist/pydischarge-*
 
 Conda
 -----
 
 Once the PyPI upload has completed, the conda-forge bot will automatically
-open a pull request to `conda-forge/pdpy-feedstock
-<https://github.com/conda-forge/pdpy-feedstock.git>`_.
+open a pull request to `conda-forge/pydischarge-feedstock
+<https://github.com/conda-forge/pydischarge-feedstock.git>`_.
 Just double-check that the dependencies and tests are up-to-date, then
 merge.
 
 Debian/RHEL
 -----------
 
 * Upload the source tarball to software.ligo.org
```

### Comparing `pydischarge-0.0.1/docs/env.rst` & `pydischarge-0.0.2/docs/env.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #####################################
-Configuring PDpy from the environment
+Configuring pyDischarge from the environment
 #####################################
 
-PDpy can be configured by setting environment variables at run time.
-Each of the variables are boolean switches, meaning they just tell PDpy to
+pyDischarge can be configured by setting environment variables at run time.
+Each of the variables are boolean switches, meaning they just tell pyDischarge to
 do something, or not to do something. The following values match as `True`:
 
 - ``'y'``
 - ``'yes'``
 - ``'1'``
 - ``'true'``
 
@@ -26,13 +26,13 @@
 +---------------------+---------+---------------------------------------------+
 | Variable            | Default | Purpose                                     |
 +=====================+=========+=============================================+
 | ``GWPY_CACHE``      | `False` | Whether to cache downloaded files from      |
 |                     |         | GWOSC to prevent repeated downloads         |
 +---------------------+---------+---------------------------------------------+
 | ``GWPY_RCPARAMS``   | `True`  | Whether to update `matplotlib.rcParams`     |
-|                     |         | with custom PDpy defaults for rendering     |
+|                     |         | with custom pyDischarge defaults for rendering     |
 |                     |         | images                                      |
 +---------------------+---------+---------------------------------------------+
 | ``GWPY_USETEX``     | `False` | Whether to use LaTeX when rendering images, |
 |                     |         | only used when ``GWPY_RCPARAMS`` is `True`  |
 +---------------------+---------+---------------------------------------------+
```

### Comparing `pydischarge-0.0.1/docs/external/framecpp.rst` & `pydischarge-0.0.2/docs/external/framecpp.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.. _pdpy-external-framecpp:
+.. _pydischarge-external-framecpp:
 
 ########
 FrameCPP
 ########
 
 .. image:: https://img.shields.io/conda/vn/conda-forge/python-ldas-tools-framecpp.svg
    :alt: python-ldas-tools-framecpp conda-forge version
@@ -13,15 +13,15 @@
 
 FrameCPP is a library for reading and writing data in GWF format defined
 in |GWFSpec|_.
 The main library is written in C++ and documented at
 
 https://computing.docs.ligo.org/ldastools/LDAS_Tools/ldas-tools-framecpp/
 
-PDpy utilises the Python bindings for FrameCPP on Unix platforms
+pyDischarge utilises the Python bindings for FrameCPP on Unix platforms
 (Linux and macOS) to provide GWF input/output capabilities.
 
 This optional dependency can be installed using `Conda <https://conda.io>`__
 (or `Mamba <https://mamba.readthedocs.io/en/stable/>`__):
 
 .. code-block:: shell
     :name: conda-install-python-ldas-tools-framecpp
```

### Comparing `pydischarge-0.0.1/docs/external/framel.rst` & `pydischarge-0.0.2/docs/external/framel.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.. _pdpy-external-framel:
+.. _pydischarge-external-framel:
 
 ######
 FrameL
 ######
 
 .. image:: https://img.shields.io/conda/vn/conda-forge/python-framel.svg
    :alt: python-ldas-tools-framecpp conda-forge version
@@ -13,15 +13,15 @@
 
 FrameL is a library for reading and writing data in GWF format defined
 in |GWFSpec|_.
 The main library is written in C and documented at
 
 https://lappweb.in2p3.fr/virgo/FrameL/
 
-PDpy can utilises the Python bindings for FrameL to provide GWF
+pyDischarge can utilises the Python bindings for FrameL to provide GWF
 input/output capabilities.
 
 This optional dependency can be installed using `Conda <https://conda.io>`__
 (or `Mamba <https://mamba.readthedocs.io/en/stable/>`__):
 
 .. code-block:: shell
     :name: conda-install-python-framel
```

### Comparing `pydischarge-0.0.1/docs/external/lalsuite.rst` & `pydischarge-0.0.2/docs/external/lalsuite.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.. _pdpy-external-lalsuite:
+.. _pydischarge-external-lalsuite:
 
 ########
 LALSuite
 ########
 
 .. image:: https://img.shields.io/conda/vn/conda-forge/lalsuite.svg
    :alt: lalsuite conda-forge version
@@ -15,37 +15,37 @@
 mainly written in C but with high-level bindings for Python.
 
 The main LALSuite documentation can be found at
 
 https://lscsoft.docs.ligo.org/lalsuite/
 
 LALSuite is made up of a number of component libraries, some of which are
-utilised by PDpy to provide various extra capabilities.
+utilised by pyDischarge to provide various extra capabilities.
 
-The full LALsuite can be installed alongside PDpy using
+The full LALsuite can be installed alongside pyDischarge using
 `Conda <https://conda.io>`__
 (or `Mamba <https://mamba.readthedocs.io/en/stable/>`__)
 or `pip`:
 
 .. md-tab-set::
-    :name: pdpy-install-lalsuite
+    :name: pydischarge-install-lalsuite
 
     .. md-tab-item:: Install LALSuite with conda/mamba
 
         .. code-block:: shell
 
             conda install -c conda-forge lalsuite
 
     .. md-tab-item:: Install LALSuite with pip
 
         .. code-block:: shell
 
             python -m pip install lalsuite
 
-.. _pdpy-external-lal:
+.. _pydischarge-external-lal:
 
 ===
 LAL
 ===
 
 .. image:: https://img.shields.io/conda/vn/conda-forge/lal.svg
    :alt: lal conda-forge version
@@ -56,29 +56,29 @@
 
 LAL is the base-level library in LALSuite that provides much of the core
 functionality.
 It's documentation is at
 
 https://lscsoft.docs.ligo.org/lalsuite/lal/
 
-PDpy provides utilities to transform to and from LAL objects
-(like the :lal:`XLALREAL8TimeSeries`) from/to their PDpy equivalent
-(e.g. :class:`pdpy.timeseries.TimeSeries`).
+pyDischarge provides utilities to transform to and from LAL objects
+(like the :lal:`XLALREAL8TimeSeries`) from/to their pyDischarge equivalent
+(e.g. :class:`pydischarge.timeseries.TimeSeries`).
 
 LAL can be installed using `Conda <https://conda.io>`__
 (or `Mamba <https://mamba.readthedocs.io/en/stable/>`__)
 on Unix systems (not Windows):
 
 .. code-block:: shell
     :name: conda-install-lal
     :caption: Install python-lal with conda
 
     conda install -c conda-forge python-lal
 
-.. _pdpy-external-lalframe:
+.. _pydischarge-external-lalframe:
 
 ========
 LALFrame
 ========
 
 .. image:: https://img.shields.io/conda/vn/conda-forge/lalframe.svg
    :alt: lalframe conda-forge version
@@ -88,15 +88,15 @@
    :target: https://anaconda.org/conda-forge/lalframe
 
 LALFrame provides a GWF I/O library compatible with LAL series types.
 It's documentation is at
 
 https://lscsoft.docs.ligo.org/lalsuite/lalframe/
 
-PDpy utilises the Python bindings for LALFrame on Unix platforms
+pyDischarge utilises the Python bindings for LALFrame on Unix platforms
 (Linux and macOS) to provide GWF input/output capabilities.
 
 This optional dependency can be installed using `Conda <https://conda.io>`__
 (or `Mamba <https://mamba.readthedocs.io/en/stable/>`__)
 on Unix systems (not Windows):
 
 .. code-block:: shell
```

### Comparing `pydischarge-0.0.1/docs/external/nds2.rst` & `pydischarge-0.0.2/docs/external/nds2.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.. _pdpy-external-nds2:
+.. _pydischarge-external-nds2:
 
 ####
 NDS2
 ####
 
 .. image:: https://img.shields.io/conda/vn/conda-forge/python-nds2-client.svg
    :alt: python-nds2-client conda-forge version
```

### Comparing `pydischarge-0.0.1/docs/index.rst` & `pydischarge-0.0.2/docs/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 #########
 |_title_|
 #########
 
-.. |_title_| image:: pdpy-docs-logo.png
+.. |_title_| image:: pydischarge-docs-logo.png
 
-.. title:: PDpy docs
+.. title:: pyDischarge docs
 
 .. ifconfig:: 'dev' in release
 
    .. warning::
 
-      You are viewing documentation for a development build of PDpy.
+      You are viewing documentation for a development build of pyDischarge.
       This version may include unstable code, or breaking changes relative
       the most recent stable release.
-      To view the documentation for the latest stable release of PDpy, please
+      To view the documentation for the latest stable release of pyDischarge, please
       `click here <../stable/>`_.
 
-PDpy is a collaboration-driven `Python <http://www.python.org>`_ package
+pyDischarge is a collaboration-driven `Python <http://www.python.org>`_ package
 providing tools for studying data from ground-based gravitational-wave
 detectors.
 
-PDpy provides a user-friendly, intuitive interface to the common time-domain
+pyDischarge provides a user-friendly, intuitive interface to the common time-domain
 and frequency-domain data produced by the `LIGO <http://www.ligo.org>`_ and
 `Virgo <http://www.ego-gw.it>`_ instruments and their analysis,
 with easy-to-follow tutorials at each step.
 
-.. image:: https://img.shields.io/conda/vn/conda-forge/pdpy
-    :target: https://anaconda.org/conda-forge/pdpy/
-    :alt: PDpy Conda-forge version badge
-.. image:: https://img.shields.io/pypi/v/pdpy
-    :target: https://pypi.org/project/pdpy/
-    :alt: PDpy PyPI version badge
+.. image:: https://img.shields.io/conda/vn/conda-forge/pydischarge
+    :target: https://anaconda.org/conda-forge/pydischarge/
+    :alt: pyDischarge Conda-forge version badge
+.. image:: https://img.shields.io/pypi/v/pydischarge
+    :target: https://pypi.org/project/pydischarge/
+    :alt: pyDischarge PyPI version badge
 .. image:: https://zenodo.org/badge/9979119.svg
     :target: https://zenodo.org/badge/latestdoi/9979119
-    :alt: PDpy DOI badge
-.. image:: https://img.shields.io/pypi/l/pdpy.svg
+    :alt: pyDischarge DOI badge
+.. image:: https://img.shields.io/pypi/l/pydischarge.svg
     :target: https://choosealicense.com/licenses/gpl-3.0/
-    :alt: PDpy license badge
+    :alt: pyDischarge license badge
 
 ***********
 First steps
 ***********
 
 .. toctree::
    :maxdepth: 1
 
-   What is PDpy? <overview>
-   How do I install PDpy? <install>
-   Citing PDpy <citing>
+   What is pyDischarge? <overview>
+   How do I install pyDischarge? <install>
+   Citing pyDischarge <citing>
 
 *****************
 Working with data
 *****************
 
 .. toctree::
    :maxdepth: 2
```

### Comparing `pydischarge-0.0.1/docs/overview.rst` & `pydischarge-0.0.2/docs/overview.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-.. _pdpy-introduction:
+.. _pydischarge-introduction:
 
 #############
-What is PDpy?
+What is pyDischarge?
 #############
 
-The PDpy package contains classes and utilities providing tools and methods for studying data from gravitational-wave detectors, for astrophysical or instrumental purposes.
+The pyDischarge package contains classes and utilities providing tools and methods for studying data from gravitational-wave detectors, for astrophysical or instrumental purposes.
 
 This package is meant for users who don't care how the code works necessarily, but want to perform some analysis on some data using a (Python) tool.
 As a result this package is meant to be as easy-to-use as possible, coupled with extensive documentation of all functions and standard examples of how to use them sensibly.
 
 The core Python infrastructure is influenced by, and extends the functionaity of, the `Astropy <http://astropy.org>`__ package, a superb set of tools for astrophysical analysis, primarily for FITS images.
 Additionally, much of the methodology has been derived from, and augmented by, the `LIGO Algorithm Library Suite (LALSuite) <https://www.lsc-group.phys.uwm.edu/daswg/projects/lalsuite.html>`_, a large collection of primarily ``C99`` routines for analysis and manipulation of data from gravitational-wave detectors.
-These packages use the `SWIG <http://www.swig.org>` program to produce Python wrappings for all ``C`` modules, allowing the PDpy package to leverage both the completeness, and the speed, of these libraries.
+These packages use the `SWIG <http://www.swig.org>` program to produce Python wrappings for all ``C`` modules, allowing the pyDischarge package to leverage both the completeness, and the speed, of these libraries.
 
 In the end, this package has begged, borrowed, and stolen a lot of code from other sources, but should end up packaging them together in a way that makes the whole set easier to use.
 
 ==============
 The basic idea
 ==============
 
-The basic idea of PDpy is to simplify all of the tedious bits of analysing data, allowing users to study and plot data quickly and effectively.
-For example, PDpy provides simple methods for input/output:
+The basic idea of pyDischarge is to simplify all of the tedious bits of analysing data, allowing users to study and plot data quickly and effectively.
+For example, pyDischarge provides simple methods for input/output:
 
 .. plot::
    :nofigs:
    :context: reset
 
-   from pdpy.timeseries import TimeSeries
+   from pydischarge.timeseries import TimeSeries
    h1 = TimeSeries.fetch_open_data('H1', 1126259457, 1126259467)
    l1 = TimeSeries.fetch_open_data('L1', 1126259457, 1126259467)
 
 and signal processing:
 
 .. plot::
    :context:
@@ -42,19 +42,19 @@
    l1b *= -1
 
 and visualisation:
 
 .. plot::
    :context:
 
-   from pdpy.plot import Plot
+   from pydischarge.plot import Plot
    plot = Plot(figsize=(12, 4))
    ax = plot.add_subplot(xscale='auto-gps')
-   ax.plot(h1b, color='pdpy:ligo-hanford', label='LIGO-Hanford')
-   ax.plot(l1b, color='pdpy:ligo-livingston', label='LIGO-Livingston')
+   ax.plot(h1b, color='pydischarge:ligo-hanford', label='LIGO-Hanford')
+   ax.plot(l1b, color='pydischarge:ligo-livingston', label='LIGO-Livingston')
    ax.set_epoch(1126259462.427)
    ax.set_xlim(1126259462.2, 1126259462.5)
    ax.set_ylim(-1e-21, 1e-21)
    ax.set_ylabel('Strain noise')
    ax.legend()
    plot.show()
```

### Comparing `pydischarge-0.0.1/docs/pdpy-docs-logo.png` & `pydischarge-0.0.2/docs/pdpy-docs-logo.png`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.1/docs/plot/colorbars.rst` & `pydischarge-0.0.2/docs/plot/colorbars.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-.. currentmodule:: pdpy.plot
+.. currentmodule:: pydischarge.plot
 
-.. _pdpy-plot-colorbars:
+.. _pydischarge-plot-colorbars:
 
 #########
 Colorbars
 #########
 
 ======================================
 Modifications to the built-in colorbar
 ======================================
 
-PDpy extends the built-in :mod:`matplotlib`
+pyDischarge extends the built-in :mod:`matplotlib`
 :meth:`~matplotlib.figure.Figure.colorbar` functionality to improve the
 defaults in a number of ways:
 
 - callable from the :class:`~matplotlib.figure.Figure`, or directly from the
   relevant :class:`~matplotlib.axes.Axes`
 - don't resize the anchor :class:`~matplotlib.axes.Axes`
 - simpler specification of log-norm colors
@@ -23,34 +23,34 @@
 See the following example for a summary of the improvements:
 
 .. plot::
    :include-source:
 
    import numpy
    data = numpy.random.rand(100, 100)
-   from pdpy.timeseries import TimeSeries
+   from pydischarge.timeseries import TimeSeries
    from matplotlib import pyplot
    fig, axes = pyplot.subplots(nrows=3, figsize=(6.4, 8))
    for ax in axes:  # plot the same data on each
       ax.imshow(data)
    fig.colorbar(axes[1].images[0], ax=axes[1])  # matplotlib default
-   axes[2].colorbar()  # pdpy colorbar
+   axes[2].colorbar()  # pydischarge colorbar
    pyplot.show()
 
 ============================
 Logarithmic colorbar scaling
 ============================
 
-With PDpy, getting logarithmic scaling on a colorbar is as simple as
+With pyDischarge, getting logarithmic scaling on a colorbar is as simple as
 specifying, ``norm='log'``:
 
 .. plot::
    :include-source:
 
-   from pdpy.timeseries import TimeSeries
+   from pydischarge.timeseries import TimeSeries
    data = TimeSeries.fetch_open_data('L1', 1187008866, 1187008898)
    specgram = data.spectrogram2(fftlength=.5, overlap=.25,
                                 window='hann') ** (1/2.)
    plot = specgram.plot(yscale='log', ylim=(30, 1400))
    plot.colorbar(norm='log', clim=(1e-24, 1e-21), label='Strain ASD')
    plot.show()
 
@@ -62,26 +62,26 @@
 Another example
 ===============
 
 .. plot::
    :include-source:
 
    # load data
-   from pdpy.timeseries import TimeSeries
+   from pydischarge.timeseries import TimeSeries
    raw = TimeSeries.fetch_open_data('L1', 1126259446, 1126259478)
 
    # calculate filtered timeseries, and Q-transform spectrogram
    data = raw.bandpass(50, 300).notch(60)
    qtrans = raw.q_transform()
 
    # plot
    from matplotlib import pyplot
    plot, axes = pyplot.subplots(nrows=2, sharex=True, figsize=(8, 6))
    tax, qax = axes
-   tax.plot(data.crop(1126259462, 1126259463), color='pdpy:ligo-livingston')
+   tax.plot(data.crop(1126259462, 1126259463), color='pydischarge:ligo-livingston')
    qax.imshow(qtrans.crop(1126259462, 1126259463))
    tax.set_xlabel('')
    tax.set_xscale('auto-gps')
    tax.set_xlim(1126259462.2, 1126259462.5)
    tax.set_ylabel('Strain amplitude')
    qax.set_yscale('log')
    qax.set_ylabel('Frequency [Hz]')
```

### Comparing `pydischarge-0.0.1/docs/plot/colors.rst` & `pydischarge-0.0.2/docs/plot/colors.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-.. _currentmodule: pdpy.plot
+.. _currentmodule: pydischarge.plot
 
-.. _pdpy-plot-colors:
+.. _pydischarge-plot-colors:
 
 ################################################
 The Gravitational-Wave Observatory colour scheme
 ################################################
 
 In order to simplify visual identification of a specific gravitational-wave observatory (GWO) on a figure where many of them are plotted (e.g. amplitude spectral densities, or filtered strain time-series), the GWO standard colour scheme should be used:
 
 .. plot::
     :include-source: False
 
     import numpy
     from matplotlib import (pyplot, rcParams)
     from matplotlib.colors import to_hex
-    from pdpy.plot import colors
+    from pydischarge.plot import colors
 
     rcParams.update({
         'text.usetex': False,
         'font.size': 15
     })
 
     th = numpy.linspace(0, 2*numpy.pi, 512)
     names = [
-         'pdpy:geo600',
-         'pdpy:kagra',
-         'pdpy:ligo-hanford',
-         'pdpy:ligo-india',
-         'pdpy:ligo-livingston',
-         'pdpy:virgo',
+         'pydischarge:geo600',
+         'pydischarge:kagra',
+         'pydischarge:ligo-hanford',
+         'pydischarge:ligo-india',
+         'pydischarge:ligo-livingston',
+         'pydischarge:virgo',
     ]
 
     fig = pyplot.figure(figsize=(5, 2))
     ax = fig.gca()
     ax.axis('off')
 
     for j, name in enumerate(sorted(names)):
@@ -50,41 +50,41 @@
                            'right': 0.78, 'top': 1})
     pyplot.show()
 
 For example:
 
 .. plot::
 
-    from pdpy.timeseries import TimeSeries
-    from pdpy.plot import Plot
+    from pydischarge.timeseries import TimeSeries
+    from pydischarge.plot import Plot
     h1 = TimeSeries.fetch_open_data('H1', 1126259457, 1126259467)
     h1b = h1.bandpass(50, 250).notch(60).notch(120)
     l1 = TimeSeries.fetch_open_data('L1', 1126259457, 1126259467)
     l1b = l1.bandpass(50, 250).notch(60).notch(120)
     plot = Plot(figsize=(12, 4.8))
     ax = plot.add_subplot(xscale='auto-gps')
-    ax.plot(h1b, color='pdpy:ligo-hanford', label='LIGO-Hanford')
-    ax.plot(l1b, color='pdpy:ligo-livingston', label='LIGO-Livingston')
+    ax.plot(h1b, color='pydischarge:ligo-hanford', label='LIGO-Hanford')
+    ax.plot(l1b, color='pydischarge:ligo-livingston', label='LIGO-Livingston')
     ax.set_epoch(1126259462.427)
     ax.set_xlim(1126259462, 1126259462.6)
     ax.set_ylim(-1e-21, 1e-21)
     ax.set_ylabel('Strain noise')
     ax.legend()
     plot.show()
 
-The above code was adapted from the example :ref:`pdpy-example-signal-gw150914`.
+The above code was adapted from the example :ref:`pydischarge-example-signal-gw150914`.
 
-The colours can also be specified using the interferometer prefix (e.g. ``'H1'``) via the `pdpy.plot.colors.GW_OBSERVATORY_COLORS` object:
+The colours can also be specified using the interferometer prefix (e.g. ``'H1'``) via the `pydischarge.plot.colors.GW_OBSERVATORY_COLORS` object:
 
 .. plot::
 
     from matplotlib import pyplot
-    from pdpy.plot.colors import GW_OBSERVATORY_COLORS
+    from pydischarge.plot.colors import GW_OBSERVATORY_COLORS
     fig = pyplot.figure()
     ax = fig.gca()
     ax.plot([1, 2, 3, 4, 5], color=GW_OBSERVATORY_COLORS['L1'])
     fig.show()
 
 .. note::
 
-   The ``'pdpy:<>'`` colours will not be available until `pdpy`
+   The ``'pydischarge:<>'`` colours will not be available until `pydischarge`
    has been imported.
```

### Comparing `pydischarge-0.0.1/docs/plot/filter.rst` & `pydischarge-0.0.2/docs/plot/filter.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-.. currentmodule:: pdpy.plot
+.. currentmodule:: pydischarge.plot
 
-.. _pdpy-plot-bode:
+.. _pydischarge-plot-bode:
 
 #######################################
 Visualising filters (:class:`BodePlot`)
 #######################################
 
 Any time-domain or Fourier-domain filters can be visualised using the Bode plot, showing the magnitude (in decibels) and phase (in degrees) response of a linear time-invariant filter. The `BodePlot` allows for simple display of these responses for any filter, for example a 40-1000 Hertz band-pass filter:
 
 .. plot::
    :include-source:
 
-   >>> from pdpy.signal.filter_design import bandpass
-   >>> from pdpy.plot import BodePlot
+   >>> from pydischarge.signal.filter_design import bandpass
+   >>> from pydischarge.plot import BodePlot
    >>> zpk = bandpass(40, 1000, 4096, analog=False)
    >>> plot = BodePlot(zpk, analog=False, sample_rate=4096, title='40-1000 Hz bandpass filter')
    >>> plot.show()
 
 |
```

### Comparing `pydischarge-0.0.1/docs/plot/gps.rst` & `pydischarge-0.0.2/docs/plot/gps.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-.. currentmodule:: pdpy.plot.gps
+.. currentmodule:: pydischarge.plot.gps
 
-.. _pdpy-plot-gps:
+.. _pydischarge-plot-gps:
 
 ########################
 Plotting GPS time scales
 ########################
 
 As we have seen, the default :mod:`matplotlib` representation of GPS scales
 is not great, given the large zero-offset typically seen with 21st century GPS
 times.
 
-To improve displays of data with GPS timestamps, PDpy provides a number of
+To improve displays of data with GPS timestamps, pyDischarge provides a number of
 custom :mod:`scales <mtplotlib.scale>`.
 Each scale uses an ``epoch`` and a ``unit`` to recentre and format the GPS
 axis in a way that clearly displays the data, without large offsets or
 multipliers.
 
 ==============
 ``'auto-gps'``
@@ -24,15 +24,15 @@
 calculates an ``epoch`` and ``unit`` each time the figure is drawn, based on
 the current view limits and data limits:
 
 .. plot::
    :include-source:
    :context: reset
 
-   >>> from pdpy.timeseries import TimeSeries
+   >>> from pydischarge.timeseries import TimeSeries
    >>> raw = TimeSeries.fetch_open_data('L1', 1126259446, 1126259478)
    >>> data = raw.bandpass(50, 300).notch(60).crop(*raw.span.contract(1))
    >>> plot = data.plot(xscale='auto-gps')
    >>> plot.show()
 
 Here the default epoch is just the epoch for the given `TimeSeries`, and the
 unit has been automatically chosen as ``'seconds'``.
@@ -77,15 +77,15 @@
 ===========
 Fixed epoch
 ===========
 
 A GPS axis can be fixed to a specific epoch via the same
 :meth:`~matplotlib.axes.Axes.set_xscale` (or
 :meth:`~matplotlib.axes.Axes.set_yscale`) method of the relevant axis, or
-via the special :meth:`~pdpy.plot.Axes.set_epoch` method:
+via the special :meth:`~pydischarge.plot.Axes.set_epoch` method:
 
 .. plot::
    :include-source:
    :context:
 
    >>> ax.set_xlim(1126259462.2, 1126259462.6)
    >>> ax.set_epoch(1126259462.42)
```

### Comparing `pydischarge-0.0.1/docs/plot/index.rst` & `pydischarge-0.0.2/docs/plot/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-.. currentmodule:: pdpy.plot
+.. currentmodule:: pydischarge.plot
 
-.. _pdpy-plot:
+.. _pydischarge-plot:
 
 ###################################
-Plotting in PDpy (:mod:`pdpy.plot`)
+Plotting in pyDischarge (:mod:`pydischarge.plot`)
 ###################################
 
 ==============
 Basic plotting
 ==============
 
-The :mod:`pdpy.plot` module provides integrated extensions to the fantastic
+The :mod:`pydischarge.plot` module provides integrated extensions to the fantastic
 data visualisation tools provided by |matplotlib|_.
 
 ---------------------------------------------
 Basic plotting with :mod:`~matplotlib.pyplot`
 ---------------------------------------------
 
-Each of the data representations provided by `pdpy` can be directly passed
+Each of the data representations provided by `pydischarge` can be directly passed
 to the standard methods available in `~matplotlib.pyplot`:
 
 .. plot::
    :include-source:
 
-   >>> from pdpy.timeseries import TimeSeries
+   >>> from pydischarge.timeseries import TimeSeries
    >>> data = TimeSeries.fetch_open_data('L1', 1126259446, 1126259478)
    >>> from matplotlib import pyplot as plt
    >>> plt.plot(data)
    >>> plt.show()
 
 ----------------------------
 ``.plot()`` instance methods
 ----------------------------
 
-Each of the data representations provided by `pdpy` also come with a
+Each of the data representations provided by `pydischarge` also come with a
 ``.plot()`` method that provides a figure with improved defaults tailored
 to those data:
 
 .. plot::
    :include-source:
 
-   >>> from pdpy.timeseries import TimeSeries
+   >>> from pydischarge.timeseries import TimeSeries
    >>> data = TimeSeries.fetch_open_data('L1', 1126259446, 1126259478)
    >>> plot = data.plot()
    >>> plot.show()
 
 The ``.plot()`` methods accept any keywords that can be used to create the
 :class:`~matplotlib.figure.Figure` and the :class:`~matplotlib.axes.Axes`,
 and to draw the element itself, e.g:
 
 .. plot::
    :include-source:
 
-   >>> from pdpy.timeseries import TimeSeries
+   >>> from pydischarge.timeseries import TimeSeries
    >>> data = TimeSeries.fetch_open_data('L1', 1126259446, 1126259478)
    >>> plot = data.plot(figsize=(8, 4.8), ylabel='Strain',
-   ...                  color='pdpy:ligo-livingston')
+   ...                  color='pydischarge:ligo-livingston')
    >>> plot.show()
 
 ----------------
 Multi-data plots
 ----------------
 
-PDpy enables trivial generation of plots with multiple datasets.
-The :class:`~pdpy.plot.Plot` constructor will accept an arbitrary
+pyDischarge enables trivial generation of plots with multiple datasets.
+The :class:`~pydischarge.plot.Plot` constructor will accept an arbitrary
 collection of data objects and will build a figure with the required geometry
 automatically.
 By default, a flat set of objects are shown on the same axes:
 
 .. plot::
    :include-source:
    :context: reset
 
-   >>> from pdpy.timeseries import TimeSeries
+   >>> from pydischarge.timeseries import TimeSeries
    >>> hdata = TimeSeries.fetch_open_data('H1', 1126259446, 1126259478)
    >>> ldata = TimeSeries.fetch_open_data('L1', 1126259446, 1126259478)
-   >>> from pdpy.plot import Plot
+   >>> from pydischarge.plot import Plot
    >>> plot = Plot(hdata, ldata, figsize=(12, 4.8))
    >>> plot.show()
 
 However, `separate=True` can be given to show each dataset on a separate
-`~pdpy.plot.Axes`:
+`~pydischarge.plot.Axes`:
 
 .. plot::
    :include-source:
    :context: close-figs
 
    >>> plot = Plot(hdata, ldata, figsize=(12, 6), separate=True, sharex=True)
    >>> plot.show()
```

### Comparing `pydischarge-0.0.1/docs/plot/legend.rst` & `pydischarge-0.0.2/docs/plot/legend.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-.. currentmodule:: pdpy.plot
+.. currentmodule:: pydischarge.plot
 
-.. _pdpy-plot-legend:
+.. _pydischarge-plot-legend:
 
 ######################
-Custom legends in PDpy
+Custom legends in pyDischarge
 ######################
 
-PDpy overrides the default :class:`~matplotlib.axes.Axes` class with one that
+pyDischarge overrides the default :class:`~matplotlib.axes.Axes` class with one that
 uses a different default legend handler for line plots.
 This means that, by default, lines in a legend will be thicker than on a
 standard matplotlib figure:
 
 .. plot::
    :include-source:
    :context: reset
 
-   >>> import pdpy  # <- import anything from pdpy
+   >>> import pydischarge  # <- import anything from pydischarge
    >>> from matplotlib import pyplot
    >>> fig = pyplot.figure()
    >>> ax = fig.gca()
    >>> ax.plot(range(10), label='My data')
    >>> ax.legend()
    >>> fig.show()
```

### Comparing `pydischarge-0.0.1/docs/plot/log.rst` & `pydischarge-0.0.2/docs/plot/log.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-.. currentmodule:: pdpy.plot
+.. currentmodule:: pydischarge.plot
 
 ##################
-Log scales in PDpy
+Log scales in pyDischarge
 ##################
 
-PDpy overrides the default :mod:`axis tick formatters <matplotlib.ticker>`
+pyDischarge overrides the default :mod:`axis tick formatters <matplotlib.ticker>`
 for logarithmic scales to one with the following logic:
 
 - ``0.1 <= x <= 1000`` and ``x`` has less than 2 decimal places, just
   represent with ``'%s'``
 - otherwise use the default formatting ``'%s^{%.2f}' % (base, logx)``
 
 This results in plots that have slightly nicer default ticks:
 
 .. plot::
    :include-source:
    :context: reset
 
-   >>> import pdpy  # <-- import anything from pdpy to active custom formatter
+   >>> import pydischarge  # <-- import anything from pydischarge to active custom formatter
    >>> import numpy
    >>> from matplotlib import pyplot
    >>> fig = pyplot.figure()
    >>> ax = fig.gca()
    >>> ax.plot(numpy.arange(.1, 5, step=.1))
    >>> ax.set_xscale('log')
    >>> ax.set_yscale('log')
```

### Comparing `pydischarge-0.0.1/docs/references.rst` & `pydischarge-0.0.2/docs/references.rst`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 .. |h5py| replace:: `h5py`
 .. _h5py: http://docs.h5py.org/en/latest/
 
 .. |ligo-segments| replace:: `ligo-segments`
 .. _ligo-segments: https://lscsoft.docs.ligo.org/ligo-segments/
 
 .. |ligotimegps| replace:: `ligotimegps`
-.. _ligotimegps: https://github.com/pdpy-github/ligotimegps/
+.. _ligotimegps: https://github.com/pydischarge-github/ligotimegps/
 
 .. |matplotlib| replace:: `matplotlib`
 .. _matplotlib: https://matplotlib.org/
 
 .. |numpy| replace:: `numpy`
 .. _numpy: http://numpy.org/
```

### Comparing `pydischarge-0.0.1/docs/segments/dqsegdb.rst` & `pydischarge-0.0.2/docs/segments/dqsegdb.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-.. currentmodule:: pdpy.segments
+.. currentmodule:: pydischarge.segments
 
-.. _pdpy-segments-dqsegdb2:
+.. _pydischarge-segments-dqsegdb2:
 
 ####################
 The Segment Database
 ####################
 
 .. warning::
 
@@ -19,15 +19,15 @@
 associated with its generation.
 The segment database is the primary access point for users to study
 data-quality flags and apply them in any analysis.
 
 The `DataQualityFlag` object includes the :meth:`~DataQualityFlag.query`
 `classmethod` with which to access segments stored in any segment database::
 
-    >>> from pdpy.segments import DataQualityFlag
+    >>> from pydischarge.segments import DataQualityFlag
     >>> segs = DataQualityFlag.query('L1:DMT-ANALYSIS_READY:1',
     ...                              'Sep 14 2015', 'Sep 15 2015')
 
 The above command will return the complete record for the
 LIGO-Livingston Observatory (``L1``) observing segments for the day of
 September 14 2015 (all times should be given in UTC or GPS).
```

### Comparing `pydischarge-0.0.1/docs/segments/index.rst` & `pydischarge-0.0.2/docs/segments/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-.. currentmodule:: pdpy.segments
+.. currentmodule:: pydischarge.segments
 
-.. _pdpy-segments:
+.. _pydischarge-segments:
 
 #####################
 Data-quality segments
 #####################
 
 In order to successfully search data for gravitational-wave signals, precise
 records of when each observatory was operating, and in which configuration,
@@ -19,15 +19,15 @@
 (seconds since the GPS epoch of midnight on January 6th 1980), and records
 such times as semi-open GPS ``[start, stop)`` segments.
 
 =====================================================
 The :class:`Segment` and :class:`SegmentList` classes
 =====================================================
 
-PDpy provides a number of classes for generating and manipulating such
+pyDischarge provides a number of classes for generating and manipulating such
 segments, enhancing the functionality provided by the (excellent)
 :mod:`ligo.segments` package.
 All credits for their usefulness go to the authors of that package.
 
 These basic objects are as follows:
 
 .. autosummary::
@@ -73,15 +73,15 @@
 
 =============================
 Combining `DataQualityFlag`\s
 =============================
 
 `DataQualityFlag`\s can be combined in a number of ways, using the standard python operators, e.g. `&` and `|`.
 
-.. _pdpy-segments-intersection:
+.. _pydischarge-segments-intersection:
 
 --------------------
 Intersection (``&``)
 --------------------
 ::
 
    >>> a & b
@@ -98,15 +98,15 @@
                     active=[[3 ... 5)
                             [10 ... 12)],
                     description=None)>
 
 This new flag represents times when both ``a`` and ``b`` were known and
 when both were active.
 
-.. _pdpy-segments-union:
+.. _pydischarge-segments-union:
 
 -------------
 Union (``|``)
 -------------
 ::
 
    >>> a | b
@@ -120,15 +120,15 @@
                  active=[[1 ... 7)
                          [10 ... 12)],
                  description=None)>
 
 This new flag represents times when either ``a`` or ``b`` were known and when
 either was active.
 
-.. _pdpy-segments-sub:
+.. _pydischarge-segments-sub:
 
 -------------------
 Subtraction (``-``)
 -------------------
 ::
 
    >>> a - b
@@ -141,24 +141,24 @@
                     known=[[0 ... 5)
                            [10 ... 12)],
                     active=[[1 ... 3)],
                     description=None)>
 
 The new flag represents times when both ``a`` and ``b`` were *known*, but only ``a`` was active.
 
-.. _pdpy-segments-add:
+.. _pydischarge-segments-add:
 
 ----------------
 Addition (``+``)
 ----------------
 ::
 
    >>> a + b
 
-This operation is the same as :ref:`pdpy-segments-union`.
+This operation is the same as :ref:`pydischarge-segments-union`.
 
 -----------------
 Inversion (``~``)
 -----------------
 ::
 
    >>> ~a
```

### Comparing `pydischarge-0.0.1/docs/segments/io.rst` & `pydischarge-0.0.2/docs/segments/io.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-.. currentmodule:: pdpy.segments
+.. currentmodule:: pydischarge.segments
 
-.. _pdpy-segments-io:
+.. _pydischarge-segments-io:
 
 ##################################
 Reading/writing segments and flags
 ##################################
 
 The `SegmentList`, `DataQualityFlag`, and `DataQualityDict` objects each include :meth:`read` and :meth:`write` methods to enable reading from and writing to a number of different file formats for segment-like objects.
-As with other classes in PDpy, the ``format`` keyword argument can be used to manually specify the input or output format, if the file extension isn't obvious enough.
+As with other classes in pyDischarge, the ``format`` keyword argument can be used to manually specify the input or output format, if the file extension isn't obvious enough.
 
 The :meth:`read` and :meth:`write` methods take different arguments and keywords based on the input/output file format, see the following sections for details on reading/writing for each of the built-in formats. Those formats are:
 
-- :ref:`pdpy-segments-io-ligolw`
-- :ref:`pdpy-segments-io-hdf5`
-- :ref:`pdpy-segments-io-json`
+- :ref:`pydischarge-segments-io-ligolw`
+- :ref:`pydischarge-segments-io-hdf5`
+- :ref:`pydischarge-segments-io-json`
 
-.. _pdpy-segments-io-ligolw:
+.. _pydischarge-segments-io-ligolw:
 
 ===============
 ``LIGO_LW`` XML
 ===============
 
 **Additional dependencies:** |python-ligo-lw|_
 
@@ -68,15 +68,15 @@
 Writing
 -------
 
 To write a `DataQualityFlag` to file in ``LIGO_LW`` format, use the :meth:`~DataQuality.write` method::
 
    >>> f.write('new-segments.xml')
 
-As with :ref:`writing tables <pdpy-table-io-ligolw>`, if the target file already exists, an :class:`~exceptions.IOError` will be raised, use ``overwrite=True`` to force a new file to be written.
+As with :ref:`writing tables <pydischarge-table-io-ligolw>`, if the target file already exists, an :class:`~exceptions.IOError` will be raised, use ``overwrite=True`` to force a new file to be written.
 
 To write a table to an existing file, use ``append=True``::
 
     >>> f.write('new-segments.xml', append=True)
 
 To replace the segment tables in an existing file, while preserving other tables, use *both* ``append=True`` and ``overwrite=True``::
 
@@ -86,36 +86,36 @@
 
     >>> f.write('new-table.xml', append=True, overwrite=True, attrs={'process_id': 0})
 
 .. note::
 
    The |python-ligo-lw| library reads and writes files using an updated
    version of the ``LIGO_LW`` format compared to :mod:`glue.ligolw` used to.
-   PDpy should support both format versions natively when _reading_, but
+   pyDischarge should support both format versions natively when _reading_, but
    only supports writing using the updated format.
 
 
 `DataQualityDict`
 -----------------
 
 The `DataQualityDict` :meth:`DataQualityDict.read` and :meth:`DataQualityDict.write` methods work in an almost identical manner, taking a list of flag names when reading::
 
     >>> fdict = DataQualityFlag.read('segments.xml', ['H1:DMT-ANALYSIS_READY:1', 'L1:DMT-ANALYSIS_READY:1'])
 
 Identical arguments should be used relative to the :meth:`DataQualityFlag.write` method when writing::
 
     >>> fdict.write('new-segments.xml')
 
-.. _pdpy-segments-io-hdf5:
+.. _pydischarge-segments-io-hdf5:
 
 ====
 HDF5
 ====
 
-PDpy uses HDF5 Groups to store a `DataQualityFlag`, with each of the :attr:`~DataQualityFlag.known` and :attr:`~DataQualityFlag.active` segment lists stored in a Dataset, and extra metadata stored in the Group's attributes.
+pyDischarge uses HDF5 Groups to store a `DataQualityFlag`, with each of the :attr:`~DataQualityFlag.known` and :attr:`~DataQualityFlag.active` segment lists stored in a Dataset, and extra metadata stored in the Group's attributes.
 
 Reading
 -------
 
 To read a `DataQualityFlag` from an ``HDF5``-format file::
 
    >>> f = DataQualityFlag.read('segments.hdf')
@@ -142,15 +142,15 @@
 
     >>> fdict = DataQualityFlag.read('segments.hdf5', ['H1:DMT-ANALYSIS_READY:1', 'L1:DMT-ANALYSIS_READY:1'])
 
 Identical arguments should be used relative to the :meth:`DataQualityFlag.write` method when writing::
 
     >>> fdict.write('new-segments.hdf5')
 
-.. _pdpy-segments-io-json:
+.. _pydischarge-segments-io-json:
 
 ====
 JSON
 ====
 
 The DQSEGDB server uses JSON as the intermediate format for returning information during queries.
```

### Comparing `pydischarge-0.0.1/docs/segments/thresholding.rst` & `pydischarge-0.0.2/docs/segments/thresholding.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #############################################
 Generating data-quality flags by thresholding
 #############################################
 
-.. currentmodule:: pdpy.segments
+.. currentmodule:: pydischarge.segments
 
 The first- and second-generation ground-based laser interferometer gravitational-wave detectors are subject to a large variety of linear noise sources, in which noise in control signals can couple directly into the gravitational-wave readout.
 If the coupling between an auxiliary signal and the gravitational-wave signal can be detected, noise in the auxiliary signal can be flagged by recording times when the time-series signal exceeded a nominal range.
 
 These times can then be recorded as GPS [start, stop) segments, and applied to any analysis of gravitational-wave data as a veto.
 
-In PDpy, a `DataQualityFlag` can be generated from any :class:`~pdpy.timeseries.TimeSeries` by applying a simple mathematical operator::
+In pyDischarge, a `DataQualityFlag` can be generated from any :class:`~pydischarge.timeseries.TimeSeries` by applying a simple mathematical operator::
 
-    >>> from pdpy.timeseries import TimeSeries
+    >>> from pydischarge.timeseries import TimeSeries
     >>> seisdata = TimeSeries.fetch('L1:HPI-BS_BLRMS_Z_3_10', 1064534416, 1064538016)
     >>> seisdata.unit = 'nm/s'
     >>> highseismic = seisdata > 400
     >>> flag = highseismic.to_dqflag(name='L1:DCH-HIGH_SEISMIC_1_3', round=True)
     >>> print(flag)
     <DataQualityFlag(valid=[[1064534416 ... 1064538016)],
                      active=[[1064535295 ... 1064535296)
@@ -25,8 +25,8 @@
                              [1064537528 ... 1064537529)],
                      ifo='L1',
                      name='DCH-HIGH_SEISMIC_1_3',
                      version=None,
                      comment='L1:HPI-BS_BLRMS_Z_3_10 > 400 nm / s')>
 
 In this worked example, times of ground-motion above 400 nm/s in the 1-3 Hz band, as recorded by a seismometer, are recorded as a `DataQualityFlag`.
-The keyword arguments given to the :meth:`~pdpy.timeseries.StateTimeSeries.to_dqflag` method give the flag a sensible name, using the standard naming convention, and make sure the segments are rounded outwards to integer start and stop times.
+The keyword arguments given to the :meth:`~pydischarge.timeseries.StateTimeSeries.to_dqflag` method give the flag a sensible name, using the standard naming convention, and make sure the segments are rounded outwards to integer start and stop times.
```

### Comparing `pydischarge-0.0.1/docs/signal/index.rst` & `pydischarge-0.0.2/docs/signal/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-.. currentmodule:: pdpy.timeseries
+.. currentmodule:: pydischarge.timeseries
 
-.. _pdpy-signal-processing:
+.. _pydischarge-signal-processing:
 
 #################
 Signal processing
 #################
 
 In a wide-array of applications, the original data recorded from a digital system must be manipulated in order to extract the greatest amount of information.
-PDpy provides a suite of functions to simplify and extend the excellent digital signal processing suite in :mod:`scipy.signal`.
+pyDischarge provides a suite of functions to simplify and extend the excellent digital signal processing suite in :mod:`scipy.signal`.
 
 ===========================
 Spectral density estimation
 ===========================
 
 `Spectral density estimation <https://en.wikipedia.org/wiki/Spectral_density>`_
 is a common way of investigating the frequency-domain content of a time-domain
 signal.
-PDpy provides wrappers of power spectral density (PSD) estimation methods
+pyDischarge provides wrappers of power spectral density (PSD) estimation methods
 from :mod:`scipy.signal` to simplify calculating a
-:class:`~pdpy.frequencyseries.FrequencySeries` from a :class:`TimeSeries`.
+:class:`~pydischarge.frequencyseries.FrequencySeries` from a :class:`TimeSeries`.
 
-The :mod:`pdpy.signal.spectral` sub-package provides the following
+The :mod:`pydischarge.signal.spectral` sub-package provides the following
 PSD estimation averaging methods:
 
 - ``'bartlett'`` - mean average of non-overlapping periodograms
 - ``'median'`` - median average of overlapping periodograms
 - ``'welch'`` - mean average of overlapping periodograms
 
 Each of these can be specified by passing the function name as the
@@ -61,15 +61,15 @@
    TimeSeries.bandpass
    TimeSeries.zpk
    TimeSeries.whiten
    TimeSeries.filter
 
 Each of the above methods eventually calls out to :meth:`TimeSeries.filter` to apply a digital linear filter, normally via cascaded second-order-sections (requires `scipy >= 0.16`).
 
-For a worked example of how to filter LIGO data to discover a gravitational-wave signal, see the example :ref:`pdpy-example-signal-gw150914`.
+For a worked example of how to filter LIGO data to discover a gravitational-wave signal, see the example :ref:`pydischarge-example-signal-gw150914`.
 
 ==========================
 Frequency-domain filtering
 ==========================
 
 Additionally, the `TimeSeries` object includes a number of instance methods to generate frequency-domain information for some data.
 Available methods include:
@@ -80,55 +80,55 @@
    TimeSeries.psd
    TimeSeries.asd
    TimeSeries.spectrogram
    TimeSeries.q_transform
    TimeSeries.rayleigh_spectrum
    TimeSeries.rayleigh_spectrogram
 
-For a worked example of how to load data and calculate the Amplitude Spectral Density `~pdpy.frequencyseries.FrequencySeries`, see the example :ref:`pdpy-example-frequencyseries-hoff`.
+For a worked example of how to load data and calculate the Amplitude Spectral Density `~pydischarge.frequencyseries.FrequencySeries`, see the example :ref:`pydischarge-example-frequencyseries-hoff`.
 
-.. _pdpy-filter-design:
+.. _pydischarge-filter-design:
 
 =============
 Filter design
 =============
 
-The :mod:`pdpy.signal` provides a number of filter design methods which, when combined with the `~pdpy.plot.BodePlot` visualisation, can be used to create a number of common filters:
+The :mod:`pydischarge.signal` provides a number of filter design methods which, when combined with the `~pydischarge.plot.BodePlot` visualisation, can be used to create a number of common filters:
 
 .. autosummary::
    :nosignatures:
 
-   ~pdpy.signal.filter_design.lowpass
-   ~pdpy.signal.filter_design.highpass
-   ~pdpy.signal.filter_design.bandpass
-   ~pdpy.signal.filter_design.notch
-   ~pdpy.signal.filter_design.concatenate_zpks
+   ~pydischarge.signal.filter_design.lowpass
+   ~pydischarge.signal.filter_design.highpass
+   ~pydischarge.signal.filter_design.bandpass
+   ~pydischarge.signal.filter_design.notch
+   ~pydischarge.signal.filter_design.concatenate_zpks
 
 Each of these will return filter coefficients that can be passed directly into `~TimeSeries.zpk` (default for analogue filters) or `~TimeSeries.filter` (default for digital filters).
 
-For a worked example of how to filter LIGO data to discover a gravitational-wave signal, see the example :ref:`pdpy-example-signal-gw150914`.
+For a worked example of how to filter LIGO data to discover a gravitational-wave signal, see the example :ref:`pydischarge-example-signal-gw150914`.
 
 **Cross-channel correlations:**
 
 .. autosummary::
    :nosignatures:
 
    TimeSeries.coherence
    TimeSeries.coherence_spectrogram
 
-For a worked example of how to compare channels like this, see the example :ref:`pdpy-example-frequencyseries-coherence`.
+For a worked example of how to compare channels like this, see the example :ref:`pydischarge-example-frequencyseries-coherence`.
 
-.. currentmodule:: pdpy.signal
+.. currentmodule:: pydischarge.signal
 
 =============
 Reference/API
 =============
 
-.. automethod:: pdpy.signal.filter_design.bandpass
+.. automethod:: pydischarge.signal.filter_design.bandpass
 
-.. automethod:: pdpy.signal.filter_design.lowpass
+.. automethod:: pydischarge.signal.filter_design.lowpass
 
-.. automethod:: pdpy.signal.filter_design.highpass
+.. automethod:: pydischarge.signal.filter_design.highpass
 
-.. automethod:: pdpy.signal.filter_design.notch
+.. automethod:: pydischarge.signal.filter_design.notch
 
-.. automethod:: pdpy.signal.filter_design.concatenate_zpks
+.. automethod:: pydischarge.signal.filter_design.concatenate_zpks
```

### Comparing `pydischarge-0.0.1/docs/spectrogram/index.rst` & `pydischarge-0.0.2/docs/spectrogram/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-.. currentmodule:: pdpy.spectrogram
+.. currentmodule:: pydischarge.spectrogram
 
-.. _pdpy-spectrogram:
+.. _pydischarge-spectrogram:
 
 #################
 The `Spectrogram`
 #################
 
-While the `~pdpy.timeseries.TimeSeries` allows us to study how the amplitude of a signal changes over time, and the `~pdpy.frequencyseries.FrequencySeries` allows us to study how that amplitude changes over frequency, the time-frequency `~pdpy.spectrogram.Spectrogram` allows us to track the evolution of the `~pdpy.frequencyseries.FrequencySeries` over time.
+While the `~pydischarge.timeseries.TimeSeries` allows us to study how the amplitude of a signal changes over time, and the `~pydischarge.frequencyseries.FrequencySeries` allows us to study how that amplitude changes over frequency, the time-frequency `~pydischarge.spectrogram.Spectrogram` allows us to track the evolution of the `~pydischarge.frequencyseries.FrequencySeries` over time.
 
 This object is a 2-dimensional array, essentially a stacked set of spectra, one per unit time.
 
-As always, a `Spectrogram` can be generated from any arbitrary data sequence, but here the required metadata are a combination of those required for the `~pdpy.timeserises.TimeSeries` and `~pdpy.frequencyseries.FrequencySeries`::
+As always, a `Spectrogram` can be generated from any arbitrary data sequence, but here the required metadata are a combination of those required for the `~pydischarge.timeserises.TimeSeries` and `~pydischarge.frequencyseries.FrequencySeries`::
 
     >>> import numpy
     >>> specgram = Spectrogram(numpy.random.random((100, 1000)), epoch=1000000000, sample_rate=1, f0=0, df=1)
     >>> print(specgram)
     Spectrogram([[ 0.58030742  0.94586261  0.79559404 ...,  0.25253688  0.61626489
                    0.22785403]
                  [ 0.95930736  0.93154594  0.13234058 ...,  0.13920997  0.94432426
@@ -44,38 +44,38 @@
    ~Spectrogram.unit
    ~Spectrogram.epoch
    ~Spectrogram.dt
    ~Spectrogram.f0
    ~Spectrogram.df
 
 ================================================================
-Calculating a `Spectrogram` from a `~pdpy.timeseries.TimeSeries`
+Calculating a `Spectrogram` from a `~pydischarge.timeseries.TimeSeries`
 ================================================================
 
-The time-frequency `Spectrogram` of a `~pdpy.timeseries.TimeSeries` can be calculated using the :meth:`~pdpy.timeseries.TimeSeries.spectrogram` method.
-We can extend previous examples of plotting a `~pdpy.timeseries.TimeSeries` with calculation of a `Spectrogram` with a 20-second stride:
+The time-frequency `Spectrogram` of a `~pydischarge.timeseries.TimeSeries` can be calculated using the :meth:`~pydischarge.timeseries.TimeSeries.spectrogram` method.
+We can extend previous examples of plotting a `~pydischarge.timeseries.TimeSeries` with calculation of a `Spectrogram` with a 20-second stride:
 
 .. plot::
    :context: reset
    :include-source:
    :nofigs:
 
-   >>> from pdpy.timeseries import TimeSeries
+   >>> from pydischarge.timeseries import TimeSeries
    >>> gwdata = TimeSeries.get('H1:LDAS-STRAIN', 'September 16 2010 06:40',
    ...                         'September 16 2010 06:50')
    >>> specgram = gwdata.spectrogram(20, fftlength=8, overlap=4) ** (1/2.)
 
 
-.. _pdpy-spectrogram-plot:
+.. _pydischarge-spectrogram-plot:
 
 ========================
 Plotting a `Spectrogram`
 ========================
 
-Like the `~pdpy.timeseries.TimeSeries` and `~pdpy.frequencyseries.FrequencySeries`, the `Spectrogram` has a convenient :meth:`~Spectrogram.plot` method, allowing us to view the data.
+Like the `~pydischarge.timeseries.TimeSeries` and `~pydischarge.frequencyseries.FrequencySeries`, the `Spectrogram` has a convenient :meth:`~Spectrogram.plot` method, allowing us to view the data.
 We can extend the previous time-series example to include a plot:
 
 .. plot::
    :context:
    :include-source:
 
    >>> plot = specgram.plot(norm='log', vmin=1e-23, vmax=1e-19)
```

### Comparing `pydischarge-0.0.1/docs/spectrum/filtering.rst` & `pydischarge-0.0.2/docs/spectrum/filtering.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-.. _pdpy-frequencyseries-filter:
+.. _pydischarge-frequencyseries-filter:
 
 ###############################
 Filtering frequency-domain data
 ###############################
 
-Frequency-domain data (a :class:`~pdpy.frequencyseries.FrequencySeries` or a :class:`~pdpy.spectrogram.Spectrogram`) can be filtered using an arbitrary filter using the :meth:`filter` methods of those objects:
+Frequency-domain data (a :class:`~pydischarge.frequencyseries.FrequencySeries` or a :class:`~pydischarge.spectrogram.Spectrogram`) can be filtered using an arbitrary filter using the :meth:`filter` methods of those objects:
 
-.. currentmodule:: pdpy.frequencyseries
+.. currentmodule:: pydischarge.frequencyseries
 
 .. autosummary::
 
    FrequencySeries.filter
 
-.. currentmodule:: pdpy.spectrogram
+.. currentmodule:: pydischarge.spectrogram
 
 .. autosummary::
 
    Spectrogram.filter
```

### Comparing `pydischarge-0.0.1/docs/spectrum/index.rst` & `pydischarge-0.0.2/docs/spectrum/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-.. currentmodule:: pdpy.frequencyseries
+.. currentmodule:: pydischarge.frequencyseries
 
-.. _pdpy-frequencyseries:
+.. _pydischarge-frequencyseries:
 
 ##################################
 The :class:`FrequencySeries` class
 ##################################
 
 While gravitational-wave detectors are time-domain instruments, their sensitivity is frequency dependent and so is often measured as a power-spectral-density over the range of interesting gravitational-wave frequencies (~10-10,000 Hz).
 Additionally, the auxiliary `channels <../detector/channel>`_ used to sense and control instrumental operations each have their own frequency-domain characteristics, contributing to the overall sensitivity spectrum.
 
 The :class:`FrequencySeries` object is used to represent any frequency series, including the power-spectral (and amplitude-spectral) density series describing instrument performance.
 
-Analogously to the :class:`~pdpy.timeseries.TimeSeries`, a new `FrequencySeries` can be generated from any data sequence along with the minimal :attr:`~FrequencySeries.f0` and :attr:`~FrequencySeries.df` metadata::
+Analogously to the :class:`~pydischarge.timeseries.TimeSeries`, a new `FrequencySeries` can be generated from any data sequence along with the minimal :attr:`~FrequencySeries.f0` and :attr:`~FrequencySeries.df` metadata::
 
-    >>> from pdpy.frequencyseries import FrequencySeries
+    >>> from pydischarge.frequencyseries import FrequencySeries
     >>> spec = FrequencySeries([1,2,3,4,5,6,7,8,9,10], f0=0, df=1)
     >>> print(spec)
     FrequencySeries([ 1  2  3  4  5  6  7  8  9 10],
                     name: None,
                     unit: None,
                     epoch: None,
                     channel: None,
@@ -32,35 +32,35 @@
    ~FrequencySeries.name
    ~FrequencySeries.unit
    ~FrequencySeries.epoch
    ~FrequencySeries.f0
    ~FrequencySeries.df
 
 ==========================================================================
-Generating a `FrequencySeries` from a :class:`~pdpy.timeseries.TimeSeries`
+Generating a `FrequencySeries` from a :class:`~pydischarge.timeseries.TimeSeries`
 ==========================================================================
 
-.. currentmodule:: pdpy.timeseries
+.. currentmodule:: pydischarge.timeseries
 
 The frequency-spectrum of a :class:`TimeSeries` can be calculated using either of the following methods:
 
 .. autosummary::
    :nosignatures:
 
    TimeSeries.psd
    TimeSeries.asd
 
-In this example we expand upon plotting a :class:`~pdpy.timeseries.TimeSeries`, by calculating the amplitude-spectral density of the gravitational-wave strain data from LHO:
+In this example we expand upon plotting a :class:`~pydischarge.timeseries.TimeSeries`, by calculating the amplitude-spectral density of the gravitational-wave strain data from LHO:
 
 .. plot::
    :context: reset
    :include-source:
    :nofigs:
 
-   >>> from pdpy.timeseries import TimeSeries
+   >>> from pydischarge.timeseries import TimeSeries
    >>> gwdata = TimeSeries.get('H1:LDAS-STRAIN', 'September 16 2010 06:40',
    ...                         'September 16 2010 06:50')
    >>> spectrum = gwdata.asd(8, 4)
 
 where the result is an average spectrum calculated using the
 `Welch method <https://en.wikipedia.org/wiki/Welch_method>`_.
 
@@ -70,23 +70,23 @@
 
 .. toctree::
    :maxdepth: 2
 
    io
 
 
-.. _pdpy-frequencyseries-plot:
+.. _pydischarge-frequencyseries-plot:
 
 ============================
 Plotting a `FrequencySeries`
 ============================
 
-.. currentmodule:: pdpy.frequencyseries
+.. currentmodule:: pydischarge.frequencyseries
 
-Similary to the :class:`~pdpy.timeseries.TimeSeries`, the `FrequencySeries` object comes with its own :meth:`~FrequencySeries.plot` method, which will quickly construct a :class:`~pdpy.plot.Plot`:
+Similary to the :class:`~pydischarge.timeseries.TimeSeries`, the `FrequencySeries` object comes with its own :meth:`~FrequencySeries.plot` method, which will quickly construct a :class:`~pydischarge.plot.Plot`:
 
 .. plot::
    :context:
    :include-source:
 
    >>> plot = spectrum.plot()
    >>> ax = plot.gca()
```

### Comparing `pydischarge-0.0.1/docs/spectrum/io.rst` & `pydischarge-0.0.2/docs/spectrum/io.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-.. currentmodule:: pdpy.frequencyseries
+.. currentmodule:: pydischarge.frequencyseries
 
-.. _pdpy-frequencyseries-io:
+.. _pydischarge-frequencyseries-io:
 
 #########################################
 Reading and writing frequency-domain data
 #########################################
 
 The `FrequencySeries` object includes :meth:`~FrequencySeries.read` and :meth:`~FrequencySeries.write` methods to enable reading from and writing to files respectively.
 For example, to read from an ASCII file containing frequency and amplitude columns::
@@ -12,25 +12,25 @@
     >>> data = FrequencySeries.read('my-data.txt')
 
 The ``format`` keyword argument can be used to manually identify the input file-format, but is not required where the file extension is sufficiently well understood.
 
 The :meth:`~FrequencySeries.read` and :meth:`~FrequencySeries.write` methods take different arguments and keywords based on the input/output file format, see the following sections for details on reading/writing for each of the built-in formats.
 Those formats are:
 
-- :ref:`pdpy-frequencyseries-io-ascii`
-- :ref:`pdpy-frequencyseries-io-hdf5`
-- :ref:`pdpy-frequencyseries-io-ligolw`
+- :ref:`pydischarge-frequencyseries-io-ascii`
+- :ref:`pydischarge-frequencyseries-io-hdf5`
+- :ref:`pydischarge-frequencyseries-io-ligolw`
 
-.. _pdpy-frequencyseries-io-ascii:
+.. _pydischarge-frequencyseries-io-ascii:
 
 =====
 ASCII
 =====
 
-PDpy supports writing `FrequencySeries` data to ASCII in a two-column ``frequency`` and ``amplitude`` format.
+pyDischarge supports writing `FrequencySeries` data to ASCII in a two-column ``frequency`` and ``amplitude`` format.
 
 Reading
 -------
 
 To read a `FrequencySeries` from ASCII::
 
    >>> t = FrequencySeries.read('data.txt')
@@ -43,21 +43,21 @@
 To write a `FrequencySeries` to ASCII::
 
    >>> t.write('data.txt')
 
 See :func:`numpy.savetxt` for keyword argument options.
 
 
-.. _pdpy-frequencyseries-io-hdf5:
+.. _pydischarge-frequencyseries-io-hdf5:
 
 ====
 HDF5
 ====
 
-PDpy allows storing data in HDF5 format files, using a custom specification for storage of metadata.
+pyDischarge allows storing data in HDF5 format files, using a custom specification for storage of metadata.
 
 Reading
 -------
 
 To read `FrequencySeries` data held in HDF5 files pass the filename (or filenames) or the source, and the path of the data inside the HDF5 file::
 
    >>> data = FrequencySeries.read('data.h5', 'psd')
@@ -76,23 +76,23 @@
     >>> data.write('output.h5', 'psd2', append=True)
 
 To replace an dataset in an existing file, while preserving other data, use *both* ``append=True`` and ``overwrite=True``::
 
     >>> data.write('output.h5', 'psd', append=True, overwrite=True)
 
 
-.. _pdpy-frequencyseries-io-ligolw:
+.. _pydischarge-frequencyseries-io-ligolw:
 
 ===============
 ``LIGO_LW`` XML
 ===============
 
 **Additional dependencies:** :mod:`python-ligo-lw`
 
-Alongside storing :ref:`tabular data <pdpy-table-io-ligolw>`, the ``LIGO_LW``
+Alongside storing :ref:`tabular data <pydischarge-table-io-ligolw>`, the ``LIGO_LW``
 XML format allows storing array data.
 These arrays are stored in ``<LIGO_LW>`` elements, which describe the metadata
 for an array (name, GPS epoch, instrument, etc.), which contain an
 ``<Array>`` element that contains the actual data values.
 
 .. note::
```

### Comparing `pydischarge-0.0.1/docs/table/filter.rst` & `pydischarge-0.0.2/docs/table/filter.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-.. currentmodule:: pdpy.table
+.. currentmodule:: pydischarge.table
 
-.. _pdpy-table-filter:
+.. _pydischarge-table-filter:
 
 ################
 Filtering tables
 ################
 
 In order to perform detailed analysis of tabular data, it is useful to
 extract portions of a table based on some criteria, this is called filtering.
 The `EventTable` object comes with a :meth:`~EventTable.filter` method
 that provides an intuitive interface to down-selecting rows in a table.
 
 To demonstrate, we can download |GWTC-2| from |GWOSC|:
 
 .. code-block:: python
 
-   >>> from pdpy.table import EventTable
+   >>> from pydischarge.table import EventTable
    >>> events = EventTable.fetch_open_data("GWTC-2")
    >>> print(events)
           name        chi_eff_upper ...     GPS      final_mass_source_upper
                                     ...                      solMass
    ------------------ ------------- ... ------------ -----------------------
    GW190408_181802-v1          0.14 ... 1238782700.3                     3.9
           GW190412-v3          0.08 ... 1239082262.2                     3.9
@@ -37,15 +37,15 @@
 The simplest `EventTable` filter is a `str` statement that provides
 a mathematical operation for a column and a threshold.
 With the above GWTC-2 events, we can use the filter
 ``"network_matched_filter_snr > 15"`` to pick out those events with
 high signal power:
 
 .. code-block:: python
-   :name: pdpy-table-filter-statement-example
+   :name: pydischarge-table-filter-statement-example
    :caption: Filtering an `EventTable` using a `str` definition
 
    >>> print(events.filter("network_matched_filter_snr > 15"))
           name        chi_eff_upper ...     GPS      final_mass_source_upper
                                     ...                      solMass
    ------------------ ------------- ... ------------ -----------------------
           GW190412-v3          0.08 ... 1239082262.2                     3.9
@@ -74,18 +74,18 @@
 If a `tuple` of names is given, the input will be a slice of the original table
 containing only the named columns.
 
 Using the same ``events`` table we can define a function to include only
 those events in the first six months of 2019:
 
 .. code-block:: python
-   :name: pdpy-table-filter-function-example
+   :name: pydischarge-table-filter-function-example
    :caption: Filtering an `EventTable` using a filter function
 
-   >>> from pdpy.time import to_gps
+   >>> from pydischarge.time import to_gps
    >>> start = to_gps("Jan 2019")
    >>> end = to_gps("Jul 2019")
    >>> def q12_2019(column, interval):
    ...     """Returns `True` if ``interval[0] <= column < interval[1]``
    ...     """
    ...     return (column >= interval[0]) & (column < interval[1])
    >>> print(events.filter(('GPS', q12_2019, (start, end))))
@@ -104,15 +104,15 @@
 The custom filter function could have been as complicated as we liked, as long
 as the two (and only two) input arguments were the column array for the
 relevant column, and the collection of other arguments to work with.
 For example could filter the table to return only those events with
 high mass ratio:
 
 .. code-block:: python
-   :name: pdpy-table-filter-function-example-2
+   :name: pydischarge-table-filter-function-example-2
    :caption: Filtering an `EventTable` using multiple columns
 
    >>> def high_mass_ratio(table, threshold):
    ...     """Returns `True` if ``mass_1_source / mass_2_source >= threshold``
    ...     """
    ...     return (table['mass_1_source'] / table['mass_2_source']) >= threshold
    >>> print(events.filter((('mass_1_source', 'mass_2_source'), high_mass_ratio, 3.0)))
@@ -127,15 +127,15 @@
 ======================
 Using multiple filters
 ======================
 
 Filters can be chained (either in `str` form, or functional form):
 
 .. code-block:: python
-   :name: pdpy-table-filter-chaining
+   :name: pydischarge-table-filter-chaining
    :caption: Chaining multiple filters with :meth:`EventTable.filter`
 
    >>> print(events.filter("network_matched_filter_snr > 15", "luminosity_distance > 1000"))
           name        chi_eff_upper ...     GPS      final_mass_source_upper
                                     ...                      solMass
    ------------------ ------------- ... ------------ -----------------------
    GW190521_074359-v1           0.1 ... 1242459857.5                     6.5
@@ -152,12 +152,12 @@
 internally by the parser anyway. E.g., use ``channel = "X1:TEST"`` and not
 ``channel = X1:TEST``.
 
 ================
 Built-in filters
 ================
 
-The PDpy package defines a small number of filter functions that implement
+The pyDischarge package defines a small number of filter functions that implement
 standard filtering operations used in gravitational-wave data analysis:
 
-.. automodsumm:: pdpy.table.filters
+.. automodsumm:: pydischarge.table.filters
    :functions-only:
```

### Comparing `pydischarge-0.0.1/docs/table/histogram.rst` & `pydischarge-0.0.2/docs/table/histogram.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-.. currentmodule:: pdpy.table
+.. currentmodule:: pydischarge.table
 
-.. _pdpy-table-histogram:
+.. _pydischarge-table-histogram:
 
 #####################
 Data table histograms
 #####################
 
 The `EventTable` object comes with a :meth:`~EventTable.hist` method, allowing
 trivial generation of histograms using any column as the counter:
@@ -13,18 +13,18 @@
    :noindex:
 
 Using the above method we can generate a histogram as follows
 
 .. plot::
    :include-source:
 
-   >>> from pdpy.table import EventTable
+   >>> from pydischarge.table import EventTable
    >>> events = EventTable.read('H1-LDAS_STRAIN-968654552-10.xml.gz', tablename='sngl_burst', columns=['snr'])
    >>> plot = events.hist('snr', weights=1/10., logbins=True, bins=50, histtype='stepfilled')
    >>> ax = plot.gca()
    >>> ax.set_xlabel('Signal-to-noise ratio (SNR)')
    >>> ax.set_ylabel('Rate [Hz]')
    >>> ax.set_title('LHO event triggers for HW100916')
    >>> ax.autoscale(axis='x', tight=True)
    >>> plot.show()
 
-This is a snippet from the example :ref:`pdpy-example-table-histogram`.
+This is a snippet from the example :ref:`pydischarge-example-table-histogram`.
```

### Comparing `pydischarge-0.0.1/docs/table/index.rst` & `pydischarge-0.0.2/docs/table/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-.. currentmodule:: pdpy.table
+.. currentmodule:: pydischarge.table
 
-.. _pdpy-table:
+.. _pydischarge-table:
 
 ###########
 Data tables
 ###########
 
 Significant events discovered in data from gravitational-wave observatories are
 stored in tabular datasets, typically describing astrophysical events, or
 noise transients (glitches).
 
 =======================
 The :class:`EventTable`
 =======================
 
-PDpy extends the (excellent) :class:`~astropy.table.Table` from
+pyDischarge extends the (excellent) :class:`~astropy.table.Table` from
 `astropy` by providing the :class:`EventTable`.
 
 This object extends the functionality of the regular
 :class:`~astropy.table.Table` with enhanced I/O to support
 gravitational-wave data, and utilities for processing and plotting tables of
 events that contain GPS timestamps.
 
 See the :any:`astropy-table` documentation for examples of how to create
 custom tables, and much more.
 The only thing to change if you want to use the `EventTable` instead of
 the basic `Table` is the import:
 
 .. code-block:: python
    :caption: Importing the `EventTable`
-   :name: pdpy-table-import
+   :name: pydischarge-table-import
 
-   >>> from pdpy.table import EventTable
+   >>> from pydischarge.table import EventTable
 
 ======================
 Reading/writing tables
 ======================
 
 .. toctree::
    :maxdepth: 2
```

### Comparing `pydischarge-0.0.1/docs/table/io.rst` & `pydischarge-0.0.2/docs/table/io.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 :tocdepth: 3
 
-.. currentmodule:: pdpy.table
+.. currentmodule:: pydischarge.table
 
-.. _pdpy-table-io:
+.. _pydischarge-table-io:
 
 #################################################################################
 Reading and writing :class:`~astropy.table.Table` and :class:`EventTable` objects
 #################################################################################
 
 .. note::
 
    This document complements the upstream Astropy documentation on
    reading/writing :class:`~astropy.table.Table` objects, please refer to
    :any:`astropy:read_write_tables`.
 
 Astropy provides an excellent :any:`unified input/output <astropy:table_io>`
-system for the `~astropy.table.Table` object, and PDpy extends upon that to
+system for the `~astropy.table.Table` object, and pyDischarge extends upon that to
 include common gravitational-wave file types, as well as providing
 event-specific input/output registrations for event data.
 In the most general case you can read a table of data as follows:
 
 .. code-block:: python
-   :name: pdpy-table-io-example
+   :name: pydischarge-table-io-example
    :caption: Reading an `EventTable` from an ASCII file
 
-   >>> from pdpy.table import EventTable
+   >>> from pydischarge.table import EventTable
    >>> table = EventTable.read('mydata.txt')
 
 :meth:`EventTable.read` will attempt to automatically identify the file
 format based on the file extension and/or the contents of the file, however,
 the ``format`` keyword argument can be used to manually identify the input
 file-format.
 
 The :meth:`~EventTable.read` and :meth:`~EventTable.write` methods take
 different arguments and keywords based on the input/output file format,
-see :ref:`pdpy-table-io-formats` for details on reading/writing for
+see :ref:`pydischarge-table-io-formats` for details on reading/writing for
 each of the built-in formats.
 
-.. _pdpy-table-gwosc:
+.. _pydischarge-table-gwosc:
 
 ************************************
 Accessing Open Data event catalogues
 ************************************
 
 |GWOSCl| publishes the Gravitational-Wave Transient Event Catalogues (GWTCs),
 allowing public access to tables of gravitational wave events and their
 parameters.
 
-PDpy's :class:`EventTable` class comes with a
+pyDischarge's :class:`EventTable` class comes with a
 :meth:`~EventTable.fetch_open_data` method that queries the GWOSC database
 to download data for the relevant catalogue.
 
-.. _pdpy-table-gwosc-query:
+.. _pydischarge-table-gwosc-query:
 
 ==============
 Simple queries
 ==============
 
 The simplest query just requires the catalogue name, and will return all parameters
 for all events in the catalogue:
 
 .. code-block:: python
-   :name: pdpy-table-io-fetch_open_data
+   :name: pydischarge-table-io-fetch_open_data
    :caption: Fetching the GWTC-2 catalogue using :meth:`EventTable.fetch_open_data` (output correct as of |today|)
 
-   >>> from pdpy.table import EventTable
+   >>> from pydischarge.table import EventTable
    >>> events = EventTable.fetch_open_data("GWTC-2")
    >>> print(events)
           name        final_mass_source_lower ... mass_2_source_upper mass_1_source_upper
                                               ...
    ------------------ ----------------------- ... ------------------- -------------------
    GW190408_181802-v1                    -2.8 ...                 3.3                 5.1
           GW190412-v3                    -3.8 ...                 1.6                 4.7
@@ -109,15 +109,15 @@
    GW190924_021846-v1                    -1.0 ...                 1.4                 7.0
    GW190929_012149-v1                   -25.3 ...                19.3                33.0
    GW190930_133541-v1                    -1.5 ...                 1.7                12.4
 
 The full list of available columns can be queried as follows:
 
 .. code-block:: python
-   :name: pdpy-table-io-fetch_open_data-info
+   :name: pydischarge-table-io-fetch_open_data-info
    :caption: Printing the columns of an `EventTable` (output correct as of |today|)
 
    >>> print(events.info)
    <EventTable masked=True length=39>
                  name                dtype    unit            description
    -------------------------------- ------- ------- --------------------------------
                                name   str18
@@ -127,26 +127,26 @@
                    chirp_mass_lower float64                         chirp_mass_lower
    ...
 
 .. admonition:: GWOSC catalogues
 
    For more details on the GWOSC catalogues, see https://gwosc.org/eventapi/html/.
 
-.. _pdpy-table-gwosc-filter:
+.. _pydischarge-table-gwosc-filter:
 
 ================
 Filtered queries
 ================
 
 The columns returned can be selected using the ``column`` keyword,
 and mathematical selection filters can be applied on-the-fly
 using the ``selection`` keyword:
 
 .. code-block:: python
-   :name: pdpy-table-io-fetch_open_data-filtered
+   :name: pydischarge-table-io-fetch_open_data-filtered
    :caption: Downloading a sub-set of a catalogue from GWOSC (output correct as of |today|)
 
    >>> t = EventTable.fetch_open_data(
    ...     "GWTC-2",
    ...     selection="mass_1_source < 4",
    ...     columns=["name", "mass_1_source", "mass_2_source", "luminosity_distance"],
    ... )
@@ -154,17 +154,17 @@
        name    mass_1_source mass_2_source luminosity_distance
                   solMass       solMass            Mpc
    ----------- ------------- ------------- -------------------
    GW190425-v2           2.0           1.4               160.0
 
 .. admonition:: More on filtering an `EventTable`
 
-   For more information on filtering, see :ref:`pdpy-table-filter`.
+   For more information on filtering, see :ref:`pydischarge-table-filter`.
 
-.. _pdpy-table-io-formats:
+.. _pydischarge-table-io-formats:
 
 ***************************
 Accessing GravitySpy events
 ***************************
 
 |GravitySpy|_ is a citizen-science project that enables the public to
 characterize and classify glitches in IGWN detector data.
@@ -177,15 +177,15 @@
 
 The :meth:`GravitySpyTable.fetch` method (inherited directly from
 `EventTable <EventTable.fetch>`) enables querying the Gravity Spy database
 directly:
 
 .. code-block:: python
 
-   >>> from pdpy.table import GravitySpyTable
+   >>> from pydischarge.table import GravitySpyTable
    >>> blips = GravitySpyTable.fetch(
    ...     "gravityspy",
    ...     "glitches",
    ...     selection="Label=Blip",
    ... )
 
 .. warning::
@@ -200,15 +200,15 @@
 
 The :meth:`GravitySpyTable.search` method enables performing a
 `Similarity Search <https://gravityspytools.ciera.northwestern.edu/search/>`__
 given the ID of a Gravity Spy event:
 
 .. code-block:: python
 
-   >>> from pdpy.table import GravitySpyTable
+   >>> from pydischarge.table import GravitySpyTable
    >>> similar = GravitySpyTable.search("8FHTgA8MEu", howmany=5)
    >>> print(similar)
    ifo  peak_frequency  links_subjects ml_label searchedID ...
    --- ---------------- -------------- -------- ---------- ...
     H1 84.4759674072266      5740011.0 Scratchy 8FHTgA8MEu ...
     L1   128.8896484375     20892636.0 Scratchy 8FHTgA8MEu ...
     L1 73.4049224853516     20892632.0 Scratchy 8FHTgA8MEu ...
@@ -218,23 +218,23 @@
 This has download 5 similarly *Scratchy* glitches from the LIGO-Hanford
 (`'H1'`) and LIGO-Livingston (`'L1'`) observatories.
 
 *********************
 Built-in file formats
 *********************
 
-PDpy extends the Astropy functionality with readers for the following file
+pyDischarge extends the Astropy functionality with readers for the following file
 formats:
 
-- :ref:`pdpy-table-io-ligolw`
-- :ref:`pdpy-table-io-ascii-cwb`
-- :ref:`pdpy-table-io-root`
-- :ref:`pdpy-table-io-pycbc_live`
-- :ref:`pdpy-table-io-gstlal`
-- :ref:`pdpy-table-io-gwf`
+- :ref:`pydischarge-table-io-ligolw`
+- :ref:`pydischarge-table-io-ascii-cwb`
+- :ref:`pydischarge-table-io-root`
+- :ref:`pydischarge-table-io-pycbc_live`
+- :ref:`pydischarge-table-io-gstlal`
+- :ref:`pydischarge-table-io-gwf`
 
 Each of the sub-sections below outlines how to read and write in these
 file formats, include the custom keyword arguments to pass to
 :meth:`EventTable.read` and :meth:`EventTable.write`.
 
 .. admonition:: Listing all available formats
 
@@ -247,15 +247,15 @@
 
 The :meth:`EventTable.read` method accepts the ``nproc``
 keyword argument, allowing multi-processed reading of lists of files.
 This argument can be used with any file-format, not just those defined below,
 but is **not** backported to for use with :meth:`Table.read`.
 
 
-.. _pdpy-table-io-ligolw:
+.. _pydischarge-table-io-ligolw:
 
 ===============
 ``LIGO_LW`` XML
 ===============
 
 **Additional dependencies:** |python-ligo-lw|_
 
@@ -272,23 +272,23 @@
 Reading
 -------
 
 When reading, the ``tablename`` keyword argument should be given to identify
 the table in the file, as follows:
 
 .. code-block:: python
-   :name: pdpy-table-io-ligolw-tablename
+   :name: pydischarge-table-io-ligolw-tablename
    :caption: Reading an `EventTable` from ``LIGO_LW`` XML.
 
    >>> t = EventTable.read('H1-LDAS_STRAIN-968654552-10.xml.gz', tablename='sngl_burst')
 
 The result should be something similar to this:
 
 .. code-block:: python
-   :name: pdpy-table-io-ligolw-output
+   :name: pydischarge-table-io-ligolw-output
    :caption: Result of reading an `EventTable` from ``LIGO_LW`` XML.
 
    >>> print(t)
    ifo peak_time peak_time_ns start_time ... confidence chisq chisq_dof bandwidth
    --- --------- ------------ ---------- ... ---------- ----- --------- ---------
     H1 968654557    783203126  968654557 ...  16.811825   0.0     512.0     256.0
     H1 968654557    781250001  968654557 ...  16.816761   0.0     512.0     256.0
@@ -332,15 +332,15 @@
    The ``tablename`` keyword can be omitted if there is only a single table
    in the file.
 
 To restrict the columns returned in the new `EventTable`, use the `columns`
 keyword argument:
 
 .. code-block:: python
-   :name: pdpy-table-io-ligolw-columns
+   :name: pydischarge-table-io-ligolw-columns
    :caption: Reading specific columns into an `EventTable` from ``LIGO_LW`` XML.
 
    >>> t = EventTable.read(
    ...     "H1-LDAS_STRAIN-968654552-10.xml.gz",
    ...     tablename="sngl_burst",
    ...     columns=["peak_time", "peak_time_ns", "snr", "peak_frequency"],
    ... )
@@ -350,15 +350,15 @@
 e.g. to calculate the Q of a sine-Gaussian pulse from the duration and
 central frequency.
 These 'columns' can be requested directly, providing the
 :class:`ligo.lw.table.Table` representation of the data has a
 :meth:`get_<name>` method for that name:
 
 .. code-block:: python
-   :name: pdpy-table-io-ligolw-get-columns
+   :name: pydischarge-table-io-ligolw-get-columns
    :caption: Reading ``get_`` columns into an `EventTable` from ``LIGO_LW`` XML.
 
    >>> t = EventTable.read(
    ...     "H1-LDAS_STRAIN-968654552-10.xml.gz",
    ...     tablename="sngl_burst",
    ...     columns=["snr", "q", "duration", "central_freq"],
    ... )
@@ -384,15 +384,15 @@
 :mod:`ligol.lw` library, and functions therein, which often end up as
 `numpy.object_` arrays in the table.
 To force all columns to have real `numpy` data types, use the
 ``use_numpy_dtypes=True`` keyword, which will cast (known) custom object
 types to a standard `numpy.dtype`, e.g:
 
 .. code-block:: python
-   :name: pdpy-table-io-ligo-lw-use_numpy_dtypes
+   :name: pydischarge-table-io-ligo-lw-use_numpy_dtypes
    :caption: Example of using ``use_numpy_dtypes=True`` when reading an `EventTable` from ``LIGO_LW`` XML.
 
    >>> t = EventTable.read(
    ...     "H1-LDAS_STRAIN-968654552-10.xml.gz",
    ...     tablename="sngl_burst",
    ...     columns=["peak"],
    ...     ligolw_columns=["peak_time", "peak_time_ns"])
@@ -436,19 +436,19 @@
 
    >>> t.write('new-table.xml', format='ligolw', tablename='sngl_burst', append=True, overwrite=True)
 
 .. note::
 
    The |python-ligo-lw| library reads and writes files using an updated
    version of the ``LIGO_LW`` format compared to :mod:`glue.ligolw` used to.
-   PDpy should support both format versions natively when _reading_, but
+   pyDischarge should support both format versions natively when _reading_, but
    only supports writing using the updated format.
 
 
-.. _pdpy-table-io-ascii-cwb:
+.. _pydischarge-table-io-ascii-cwb:
 
 ============================================
 Coherence WaveBurst ASCII (aka `EVENTS.txt`)
 ============================================
 
 |cWBl|_ is an analysis pipeline is used to detect generic gravitational-wave
 bursts, without using a signal model to restrict the analysis, and runs in
@@ -459,37 +459,37 @@
 
 Reading
 -------
 
 To read a cWB ASCII file:
 
 .. code-block:: python
-   :name: pdpy-table-io-cwb-read
+   :name: pydischarge-table-io-cwb-read
    :caption: Reading an `EventTable` from cWB-format ASCII.
 
    >>> t = EventTable.read('EVENTS.txt', format='ascii.cwb')
 
 See the :func:`astropy.io.ascii.read` documentation for full details on
 keyword arguments when reading ``ascii.cwb`` files.
 
 Writing
 -------
 
 To write a table using the cWB ASCII format:
 
 .. code-block:: python
-   :name: pdpy-table-io-cwb-write
+   :name: pydischarge-table-io-cwb-write
    :caption: Writing an `EventTable` to a cWB-format ASCII file.
 
    >>> t.write('EVENTS.txt', format='ascii.cwb')
 
 [the output file name is not required to be ``'EVENTS.txt'``, this is
 simply the convention used in the cWB analysis.]
 
-.. _pdpy-table-io-root:
+.. _pydischarge-table-io-root:
 
 ====
 ROOT
 ====
 
 **Additional dependencies:** |uproot|_
 
@@ -497,49 +497,49 @@
 -------
 
 To read a `ROOT <https://root.cern.ch/>`_ tree into a `Table`
 (or `EventTable`), specify the relevant tree via the ``treename``
 keyword argument:
 
 .. code-block:: python
-   :name: pdpy-table-io-root-read
+   :name: pydischarge-table-io-root-read
    :caption: Reading an `EventTable` from a ROOT file.
 
    >>> t = Table.read('my-data.root', treename='triggers')
 
 If ``treename=None`` is given (default), a single tree will be read if only one exists in the file, otherwise a `ValueError` will be raised.
 
 Any other keyword arguments will be passed directly to :meth:`uproot.tree.TTreeMethods.arrays`.
 
 Writing
 -------
 
 To write a `Table` as a ROOT tree:
 
 .. code-block:: python
-   :name: pdpy-table-io-root-write
+   :name: pydischarge-table-io-root-write
    :caption: Writing an `EventTable` to a ROOT file.
 
    >>> t.write('new-table.root')
 
 As with reading, the ``treename`` keyword argument can be used to specify
 the tree, the default is ``treename='tree'``.
 
 By default, an existing file with an existing tree of the given name will be
 appended to, to overwrite use the ``mode='recreate'`` keyword argument:
 
 .. code-block:: python
-   :name: pdpy-table-io-root-write-mode
+   :name: pydischarge-table-io-root-write-mode
    :caption: Writing an `EventTable` over an existing tree in a ROOT file.
 
    >>> t.write('new-table.root', treename='triggers', mode='recreate')
 
 Any other keyword arguments will be passed directly to :class:`uproot.newtree`.
 
-.. _pdpy-table-io-pycbc_live:
+.. _pydischarge-table-io-pycbc_live:
 
 =================
 PyCBC Live (HDF5)
 =================
 
 PyCBC Live is a low-latency search for gravitational waves from compact
 binary coalescences, built from the |pycbc|_ analysis package.
@@ -573,32 +573,32 @@
 
 Reading
 -------
 
 To read an `EventTable` from a ``pycbc_live`` format HDF5 file:
 
 .. code-block:: python
-   :name: pdpy-table-io-pycbc_live-read
+   :name: pydischarge-table-io-pycbc_live-read
    :caption: Reading an `EventTable` from a PyCBC-Live HDF5 file.
 
    >>> t = EventTable.read("H1-Live-1234567890-4.h5")
 
 To restrict the returned columns, use the ``columns`` keyword argument:
 
 .. code-block:: python
-   :name: pdpy-table-io-pycbc_live-read-columns
+   :name: pydischarge-table-io-pycbc_live-read-columns
    :caption: Reading specific columns into an `EventTable` from PyCBC-Live HDF5.
 
    >>> t = EventTable.read(
    ...     "H1-MY_DATA-1234567890-4.h5",
    ...     format="hdf5.pycbc_live",
    ...     columns=["end_time", "snr", "chisq"],
    ... )
 
-Similarly to the :ref:`pdpy-table-io-ligolw` format, some processed columns
+Similarly to the :ref:`pydischarge-table-io-ligolw` format, some processed columns
 can be specified that are not included in the HDF5 files, but are created
 on-the-fly.
 Supported processed columns are:
 
 - ``mchirp``
 - ``new_snr``
 
@@ -611,86 +611,86 @@
 ``extended_metadata=False``.
 
 Writing
 -------
 
 Writing tables in PyCBC Live HDF5 format is not supported at this time.
 
-.. _pdpy-table-io-gstlal:
+.. _pydischarge-table-io-gstlal:
 
 ========================
 GstLAL (``LIGO_LW`` XML)
 ========================
 
 GstLAL is a low-latency search for gravitational waves from compact
 binary coalescences, built using |GStreamer|_ elements and tools from the
-:ref:`pdpy-external-lalsuite` library.
+:ref:`pydischarge-external-lalsuite` library.
 This search writes files on the LIGO Data Grid (LIGO.ORG-authenticated users
 only) in ``LIGO_LW`` XML format, containing tables of events.
 
 Reading
 -------
 
 To read an `EventTable` from a ``gstlal`` format ``LIGO_LW`` XML file, use the
 ``format='ligolw.gstlal'`` keyword:
 
 .. code-block:: python
-   :name: pdpy-table-io-gstlal-read
+   :name: pydischarge-table-io-gstlal-read
    :caption: Reading an `EventTable` from a GstLAL ``LIGO_LW`` XML file.
 
    >>> t = EventTable.read("H1L1-GstLAL-1234567890-4.xml.gz", format="ligolw.gstlal")
 
 GstLAL ``LIGO_LW`` XML files contain information about triggers from each detector separately
 as well as from a combination of detectors. 
 Accessing these different sets of information can be done using the ``triggers`` keyword. 
 By default, information about triggers from each detector separately is read in.
 This is equivalent to using ``triggers='sngl'``. 
 To instead read information about triggers from multiple detectors, you can instead use
 the ``triggers='coinc'`` keyword:
 
 .. code-block:: python
-   :name: pdpy-table-io-gstlal-read-coinc-table
+   :name: pydischarge-table-io-gstlal-read-coinc-table
    :caption: Reading coincident triggers into an `EventTable` GstLAL ``LIGO_LW`` XML HDF5.
 
    >>> t = EventTable.read(
    ...     "H1L1-GstLAL-1234567890-4.xml.gz",
    ...     format="gstlal.gstlal",
    ...     triggers='coinc',
    ... )
 
 To restrict the returned columns, use the ``columns`` keyword argument:
 
 .. code-block:: python
-   :name: pdpy-table-io-gstlal-read-columns
+   :name: pydischarge-table-io-gstlal-read-columns
    :caption: Reading specific columns into an `EventTable` GstLAL ``LIGO_LW`` XML HDF5.
 
    >>> t = EventTable.read(
    ...     "H1L1-GstLAL-1234567890-4.xml.gz",
    ...     format="gstlal.gstlal",
    ...     columns=["end_time", "snr", "chisq"],
    ... )
 
-Similarly to the :ref:`pdpy-table-io-ligolw` format, some processed columns
+Similarly to the :ref:`pydischarge-table-io-ligolw` format, some processed columns
 can be specified that are not included in the XML files, but are created
 on-the-fly.
-In addition to processed columns support by :ref:`pdpy-table-io-ligolw`, 
+In addition to processed columns support by :ref:`pydischarge-table-io-ligolw`, 
 the additional supported processed columns are:
 
 - ``mchirp``
 - ``snr_chi``
 - ``chi_snr``
 
 These can be specified without having to specify any of the input columns.
 
 Writing
 -------
 
 Writing tables in GstLAL ``LIGO_LW`` XML format is not supported at this time.
 
-.. _pdpy-table-io-snax:
+.. _pydischarge-table-io-snax:
 
 ===========
 SNAX (HDF5)
 ===========
 
 The SNAX (Signal-based Noise Acquisition and eXtraction) analysis pipeline
 is a low-latency search for identifying glitches in h(t) and auxiliary
@@ -703,76 +703,76 @@
 Reading
 -------
 
 To read an `EventTable` from a ``snax`` format HDF5 file,
 use the ``format='hdf5.snax'`` keyword:
 
 .. code-block:: python
-   :name: pdpy-table-io-snax-read
+   :name: pydischarge-table-io-snax-read
    :caption: Reading an `EventTable` from a SNAX-format HDF5 file.
 
    >>> t = EventTable.read("H-SNAX_FEATURES-1255853400-20.h5", format="hdf5.snax")
 
 By default, all channels contained in the file are read in.
 To restrict the returned channels, use the ``channels`` keyword argument:
 
 .. code-block:: python
-   :name: pdpy-table-io-snax-read-channels
+   :name: pydischarge-table-io-snax-read-channels
    :caption: Reading specific channels into an `EventTable` from a SNAX-format HDF5 file.
 
    >>> t = EventTable.read(
    ...     "H-SNAX_FEATURES-1255853400-20.h5",
    ...     format="hdf5.snax",
    ...     channels="H1:CAL-DELTAL_EXTERNAL_DQ",
    ... )
 
 To restrict the returned columns, use the ``columns`` keyword argument:
 
 .. code-block:: python
-   :name: pdpy-table-io-snax-read
+   :name: pydischarge-table-io-snax-read
    :caption: Reading specific columns into an `EventTable` from SNAX-format HDF5.
 
    >>> t = EventTable.read(
    ...     "H-GSTLAL_IDQ_FEATURES-1255853400-20.h5",
    ...     format="hdf5.snax",
    ...     columns=["channel", "time", "snr"],
    ... )
 
 Writing
 -------
 
 Writing tables in SNAX HDF5 format is not supported at this time.
 
-.. _pdpy-table-io-gwf:
+.. _pydischarge-table-io-gwf:
 
 ===
 GWF
 ===
 
-**Additional dependencies:** :ref:`pdpy-external-framecpp`
+**Additional dependencies:** :ref:`pydischarge-external-framecpp`
 
 The Gravitational-Wave Frame file format supports tabular data via
 ``FrEvent`` structures, which allow storage of arbitrary event information.
 
 Reading
 -------
 
 To read an `EventTable` from a ``GWF``-format file, specify the filename and
 the ``name`` of the ``FrEvent`` structures to read:
 
 .. code-block:: python
-   :name: pdpy-table-io-gwf-read
+   :name: pydischarge-table-io-gwf-read
    :caption: Reading an `EventTable` from GWF.
 
    >>> t = EventTable.read('events.gwf', 'my-event-name')
 
 To restrict the returned columns, use the ``columns`` keyword argument:
 
 .. code-block:: python
-   :name: pdpy-table-io-gwf-read-columns
+   :name: pydischarge-table-io-gwf-read-columns
    :caption: Reading specific columns into an `EventTable` from GWF.
 
    >>> t = EventTable.read('events.gwf', 'my-event-name', columns=['time', 'amplitude'])
 
 All ``FrEvent`` structures contain the following columns, any other
 columns are use-specific:
```

### Comparing `pydischarge-0.0.1/docs/table/plot.rst` & `pydischarge-0.0.2/docs/table/plot.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-.. currentmodule:: pdpy.table
+.. currentmodule:: pydischarge.table
 
-.. _pdpy-table-plot:
+.. _pydischarge-table-plot:
 
 #####################
 Plotting tabular data
 #####################
 
-.. _pdpy-table-plot-scatter:
+.. _pydischarge-table-plot-scatter:
 
 =======================
 Plotting event triggers
 =======================
 
 The `EventTable` class provides a convenience instance method to
 :meth:`~EventTable.plot` events by specifying the columns to use for the
 x-axis, y-axis, and optionally colouring:
 
 .. plot::
    :context: reset
    :include-source:
 
-   >>> from pdpy.table import EventTable
+   >>> from pydischarge.table import EventTable
    >>> events = EventTable.read('H1-LDAS_STRAIN-968654552-10.xml.gz', tablename='sngl_burst', columns=['peak', 'central_freq', 'snr'])
    >>> plot = events.scatter('peak', 'central_freq', color='snr')
    >>> ax = plot.gca()
    >>> ax.set_epoch(968654552)
    >>> ax.set_yscale('log')
    >>> ax.set_ylabel('Frequency [Hz]')
    >>> ax.colorbar(clim=[1, 10], cmap='YlGnBu', norm='log', label='Signal-to-noise ratio (SNR)')
 
-.. _pdpy-table-plot-tiles:
+.. _pydischarge-table-plot-tiles:
 
 ====================
 Plotting event tiles
 ====================
 
 Many types of event triggers define a 2-dimensional tile, for example in time and frequency.
 These tiles can be plotted in a similar manner to simple triggers.
@@ -46,8 +46,8 @@
    >>> plot = events.tile('peak', 'central_freq', 'duration', 'bandwidth', color='snr')
    >>> ax = plot.gca()
    >>> ax.set_epoch(968654552)
    >>> ax.set_yscale('log')
    >>> ax.set_ylabel('Frequency [Hz]')
    >>> ax.colorbar(clim=[1, 10], cmap='YlGnBu', norm='log', label='Signal-to-noise ratio (SNR)')
 
-These code snippets are part of the example :ref:`pdpy-example-table-tiles`.
+These code snippets are part of the example :ref:`pydischarge-example-table-tiles`.
```

### Comparing `pydischarge-0.0.1/docs/table/rate.rst` & `pydischarge-0.0.2/docs/table/rate.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-.. currentmodule:: pdpy.table
+.. currentmodule:: pydischarge.table
 
-.. _pdpy-table-rate:
+.. _pydischarge-table-rate:
 
 ##############################
 Calculating event trigger rate
 ##############################
 
 =================
 Simple event rate
@@ -22,24 +22,24 @@
 For example, using the same data as before we can calculate and plot the
 event rate on a 1-second stride:
 
 .. plot::
    :context: reset
    :include-source:
 
-   >>> from pdpy.table import EventTable
+   >>> from pydischarge.table import EventTable
    >>> events = EventTable.read('H1-LDAS_STRAIN-968654552-10.xml.gz', tablename='sngl_burst', columns=['peak', 'central_freq', 'snr'])
    >>> rate = events.event_rate(1, start=968654552, end=968654562, timecolumn='peak')
    >>> plot = rate.step()
    >>> ax = plot.gca()
    >>> ax.set_ylabel('Event rate [Hz]')
    >>> ax.set_title('LIGO Hanford Observatory event rate for HW100916')
    >>> plot.show()
 
-This code is a snippet of the example :ref:`pdpy-example-table-rate`.
+This code is a snippet of the example :ref:`pydischarge-example-table-rate`.
 
 =================
 Binned event rate
 =================
 
 Following from a simple rate versus time calculation, it is often useful
 to calculate the event rate for multiple conditions on the same table.
@@ -58,8 +58,8 @@
    >>> rates = events.binned_event_rates(1, 'snr', [2, 3, 5, 8], operator='>=', start=968654552, end=968654562, timecolumn='peak')
    >>> plot = rates.step()
    >>> ax = plot.gca()
    >>> ax.set_ylabel('Event rate [Hz]')
    >>> ax.set_title('LIGO Hanford Observatory event rate for HW100916')
    >>> plot.show()
 
-This code is a snippet of the example on :ref:`pdpy-example-table-rate_binned`.
+This code is a snippet of the example on :ref:`pydischarge-example-table-rate_binned`.
```

### Comparing `pydischarge-0.0.1/docs/time/index.rst` & `pydischarge-0.0.2/docs/time/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-.. currentmodule:: pdpy.time
+.. currentmodule:: pydischarge.time
 
-.. _pdpy-time:
+.. _pydischarge-time:
 
 ####################
 Times and timestamps
 ####################
 
 ========
 GPS time
@@ -15,28 +15,28 @@
 The LIGO Scientific Collaboration stores such GPS times with nanosecond precision using the |LIGOTimeGPS| object.
 
 ================
 Time conversions
 ================
 
 `Astropy <http://astropy.org>`__ provides the excellent `Time <astropy.time>` object to allow easy conversion between this format and a number of other formats.
-For convenience, this object is available in PDpy as ``pdpy.time.Time``.
+For convenience, this object is available in pyDischarge as ``pydischarge.time.Time``.
 
 
-On top of that, PDpy provides three simple methods to simplify converting between GPS times and Python-standard `datetime` objects, namely:
+On top of that, pyDischarge provides three simple methods to simplify converting between GPS times and Python-standard `datetime` objects, namely:
 
 .. autosummary::
    :nosignatures:
 
    tconvert
    to_gps
    from_gps
 
 =========
 Reference
 =========
 
-.. autofunction:: pdpy.time.tconvert
+.. autofunction:: pydischarge.time.tconvert
 
-.. autofunction:: pdpy.time.to_gps
+.. autofunction:: pydischarge.time.to_gps
 
-.. autofunction:: pdpy.time.from_gps
+.. autofunction:: pydischarge.time.from_gps
```

### Comparing `pydischarge-0.0.1/docs/timeseries/datafind.rst` & `pydischarge-0.0.2/docs/timeseries/datafind.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-.. currentmodule:: pdpy.timeseries
+.. currentmodule:: pydischarge.timeseries
 
-.. _pdpy-timeseries-datafind:
+.. _pydischarge-timeseries-datafind:
 
 ########################
 Automatic data-discovery
 ########################
 
-.. _pdpy-timeseries-datafind-intro:
+.. _pydischarge-timeseries-datafind-intro:
 
 The :meth:`TimeSeries.fetch_open_data` method is only able to download
 GW strain data from those datasets exposed through the |GWOSC|_ API;
 this notably does not include the |GWOSC_AUX_RELEASE|_, or strain data
 for any events or observing runs not yet published.
 
 In addition, the GW strain data make up only a tiny fraction of the 'raw'
@@ -21,29 +21,29 @@
 
 The full data set for each detector is archived at the relevant observatory
 and is made freely available to all registered collaboration members.
 A discovery service called |gwdatafind|_ is provided at each location to
 simplify discovering the file(s) that contain the data of interest for any
 research.
 
-These data are also made available remotely using :ref:`pdpy-external-nds2`,
+These data are also made available remotely using :ref:`pydischarge-external-nds2`,
 which enables sending data directly over a network to any location.
 This is used for both the full proprietary data (which requires an
 authorisation credential to access) and also the |GWOSC_AUX_RELEASE|_
 (which is freely available).
 
-.. _pdpy-timeseries-get:
+.. _pydischarge-timeseries-get:
 
 **********************
 :meth:`TimeSeries.get`
 **********************
 
-**Additional dependencies:** :ref:`pdpy-external-framecpp` or :ref:`pdpy-external-nds2`
+**Additional dependencies:** :ref:`pydischarge-external-framecpp` or :ref:`pydischarge-external-nds2`
 
-PDpy provides the :meth:`TimeSeries.get` method as a one-stop interface
+pyDischarge provides the :meth:`TimeSeries.get` method as a one-stop interface
 to all automatically-discoverable data hosted locally at an IGWN
 computing centre, or available remotely.
 
 ============
 How it works
 ============
 
@@ -67,15 +67,15 @@
    data channel you want, which is often not obvious.
    The |GWOSC_AUX_RELEASE|_ includes a link to a full listing of all
    included channels.
    For the full proprietary data set, the IGWN Detector
    Characterisation working group maintains a record of the most relevant
    channels for studying a given interferometer subsystem.
 
-.. _pdpy-timeseries-get-example:
+.. _pydischarge-timeseries-get-example:
 
 =======
 Example
 =======
 
 For example, to channel that records the power incident on the
 input mode cleaner (IMC) at LIGO-Hanford, is called::
@@ -86,23 +86,23 @@
 channel by specifying the special GWOSC NDS2 server url using the
 ``host`` keyword:
 
 .. plot::
    :context: reset
 
    >>> from gwosc.datasets import event_gps
-   >>> from pdpy.timeseries import TimeSeries
+   >>> from pydischarge.timeseries import TimeSeries
    >>> gps = event_gps("GW170814")
    >>> start = int(gps) - 100
    >>> end = int(gps) + 100
    >>> data = TimeSeries.get("H1:IMC-PWR_IN_OUT_DQ", start, end, host="losc-nds.ligo.org")
    >>> plot = data.plot(ylabel="Power [W]")
    >>> plot.show()
 
-.. _pdpy-timeseries-datafind-datasets:
+.. _pydischarge-timeseries-datafind-datasets:
 
 ********************
 Proprietary datasets
 ********************
 
 All data archived at an IGWN computing centre are identified by a data
 set 'tag', which identifies which data are contained in a given ``gwf``
@@ -197,15 +197,15 @@
 
 .. admonition:: Not all datasets are available everywhere
 
    Not all datasets are available from all datafind servers.  Each LIGO Lab-operated
    computing centre has its own datafind server with a subset of the available
    datasets.
 
-.. _pdpy-timeseries-datafind-trends:
+.. _pydischarge-timeseries-datafind-trends:
 
 ***************
 LIGO trend data
 ***************
 
 The LIGO observatories produce second- and minute- trends of all channels
 automatically, and store them in the ``{H,L}1_T`` (second) and ``{H,L}1_M``
@@ -215,15 +215,15 @@
 different trends when given only the channel name.
 
 To get around this you can directly specify (e.g.) ``frametype="H1_T"``
 (for the LIGO-Hanford second trends) in your :meth:`TimeSeries.get`
 method call, or you can use a suffix in the channel name:
 
 .. table:: Channel name suffices for LIGO trends
-   :name: pdpy-timeseries-datafind-trend-types
+   :name: pydischarge-timeseries-datafind-trend-types
 
    ==========  ============  ===========
    Trend type  Dataset       Suffix
    ==========  ============  ===========
    second      ``{H,L}1_T``  ``,s-trend``
    minute      ``{H,L}1_M``  ``,m-trend``
    ==========  ============  ===========
@@ -258,15 +258,15 @@
 
    This example uses proprietary data that are only available to members
    of the LIGO Scientific Collaboration and its partners.
 
 .. plot::
    :context: reset
 
-   >>> from pdpy.timeseries import TimeSeriesDict
+   >>> from pydischarge.timeseries import TimeSeriesDict
    >>> data = TimeSeriesDict.get(
    ...     ["H1:ISI-GND_STS_ITMY_Z_BLRMS_30M_100M.rms,s-trend",
    ...      "H1:ISI-GND_STS_ETMY_Z_BLRMS_30M_100M.rms,s-trend"],
    ...     "July 22 2021 12:00",
    ...     "July 22 2021 14:00",
    ... )
    >>> plot = data.plot(ylabel="Ground motion [nm/s]")
```

### Comparing `pydischarge-0.0.1/docs/timeseries/index.rst` & `pydischarge-0.0.2/docs/timeseries/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-.. _pdpy-timeseries:
+.. _pydischarge-timeseries:
 
-.. currentmodule:: pdpy.timeseries
+.. currentmodule:: pydischarge.timeseries
 
 ################
 Time Series data
 ################
 
 Gravitational-wave detectors are time-domain instruments, recording
 gravitational-wave amplitude as a differential change in the lengths
@@ -19,33 +19,33 @@
 
 =======================
 The :class:`TimeSeries`
 =======================
 
 .. code-block:: python
    :caption: Importing the `TimeSeries`
-   :name: pdpy-timeseries-import
+   :name: pydischarge-timeseries-import
 
-   from pdpy.timeseries import TimeSeries
+   from pydischarge.timeseries import TimeSeries
 
-PDpy provides the `TimeSeries` object as a way of representing time series
+pyDischarge provides the `TimeSeries` object as a way of representing time series
 data.
 The `TimeSeries` is built on top of the :class:`numpy.ndarray`, and so many
 methods and applications of this object should be familiar to
 :mod:`numpy` users.
 
 For example, to create a simple `TimeSeries` filled with
 :mod:`~numpy.random` data:
 
 .. code-block:: python
    :caption: Creating a `TimeSeries` with random data
-   :name: pdpy-timeseries-random
+   :name: pydischarge-timeseries-random
 
    >>> from numpy.random import random
-   >>> from pdpy.timeseries import TimeSeries
+   >>> from pydischarge.timeseries import TimeSeries
    >>> t = TimeSeries(random(1000))
    >>> print(t)
    TimeSeries([ 0.59442285, 0.61979421, 0.62968915,...,  0.98309223,
                 0.94513298, 0.1826175 ]
               unit: Unit(dimensionless),
               t0: 0.0 s,
               dt: 1.0 s,
@@ -64,15 +64,15 @@
    ~TimeSeries.name
    ~TimeSeries.channel
 
 ==================
 Associated classes
 ==================
 
-Alongside the `TimeSeries` class, `pdpy.timeseries` module provides a
+Alongside the `TimeSeries` class, `pydischarge.timeseries` module provides a
 small set of related classes for handling collections of data:
 
 .. autosummary::
    :nosignatures:
    :caption: `TimeSeries` container classes
 
    TimeSeriesDict
```

### Comparing `pydischarge-0.0.1/docs/timeseries/io.rst` & `pydischarge-0.0.2/docs/timeseries/io.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,89 +1,89 @@
 :tocdepth: 3
 
-.. currentmodule:: pdpy.timeseries
+.. currentmodule:: pydischarge.timeseries
 
-.. _pdpy-timeseries-io:
+.. _pydischarge-timeseries-io:
 
 ####################################
 Reading and writing time series data
 ####################################
 
 The `TimeSeries` object includes :meth:`~TimeSeries.read` and
 :meth:`~TimeSeries.write` methods to enable reading from and writing to files
 respectively.
 For example, to read from an ASCII file containing time and amplitude columns:
 
 .. code-block:: python
-   :name: pdpy-timeseries-io-example
+   :name: pydischarge-timeseries-io-example
 
-   >>> from pdpy.timeseries import TimeSeries
+   >>> from pydischarge.timeseries import TimeSeries
    >>> data = TimeSeries.read('my-data.txt')
 
 :meth:`TimeSeries.read` will attempt to automatically identify the file
 format based on the file extension and/or the contents of the file, however,
 the ``format`` keyword argument can be used to manually identify the input
 file-format.
 
 The :meth:`~TimeSeries.read` and :meth:`~TimeSeries.write` methods take
 different arguments and keywords based on the input/output file format,
-see :ref:`pdpy-timeseries-io-formats` for details on reading/writing for
+see :ref:`pydischarge-timeseries-io-formats` for details on reading/writing for
 each of the built-in formats.
 
-.. _pdpy-timeseries-io-discovery:
+.. _pydischarge-timeseries-io-discovery:
 
 ***************************************
 Automatic discovery of GW detector data
 ***************************************
 
 ================
 GW detector data
 ================
 
 Gravitational-wave detector data, including all engineering diagnostic data
 as well as the calibrated 'strain' data that are searched for GW signals,
-are archived in :ref:`GWF <pdpy-timeseries-io-gwf>` files stored at the
+are archived in :ref:`GWF <pydischarge-timeseries-io-gwf>` files stored at the
 relevant observatory.
 These data are available locally to authenticated users of the associated
 computing centres (typically collaboration members), but are also
-distributed using |CVMFS|_ and are available remotely using :ref:`pdpy-external-nds2`.
+distributed using |CVMFS|_ and are available remotely using :ref:`pydischarge-external-nds2`.
 Access to these data is restricted to active collaboration members.
 
 Additionally |GWOSCl|_ hosts publicly-accessible 'open' data, with *event*
 datasets made available at the same time as the relevant result publication
 and typically including ~1 hour of data around each published event detection,
 and *bulk* datasets with the entire observing run data available roughly
 18 months after the end of the run.
 
 GWOSC also hosts the |GWOSC_AUX_RELEASE|_, providing public access to
 environmental sensor data around |GW170814|_.
-These data are freely accessible using :ref:`pdpy-external-nds2`.
+These data are freely accessible using :ref:`pydischarge-external-nds2`.
 
 ======================
 Data discovery methods
 ======================
 
 .. toctree::
 
    opendata
    datafind
 
-.. _pdpy-timeseries-io-formats:
+.. _pydischarge-timeseries-io-formats:
 
 *********************
 Built-in file formats
 *********************
 
-.. _pdpy-timeseries-io-ascii:
+.. _pydischarge-timeseries-io-ascii:
 
 =====
 ASCII
 =====
 
-PDpy supports writing `TimeSeries` (and `~pdpy.frequencyseries.FrequencySeries`) data to ASCII in a two-column ``time`` and ``amplitude`` format.
+pyDischarge supports writing `TimeSeries` (and `~pydischarge.frequencyseries.FrequencySeries`) data to ASCII in a two-column ``time`` and ``amplitude`` format.
 
 Reading
 -------
 
 To read a `TimeSeries` from ASCII:
 
 .. code-block:: python
@@ -99,28 +99,28 @@
 
 .. code-block:: python
 
    >>> t.write('data.txt')
 
 See :func:`numpy.savetxt` for keyword argument options.
 
-.. _pdpy-timeseries-io-gwf:
+.. _pydischarge-timeseries-io-gwf:
 
 ===
 GWF
 ===
 
-**Additional dependencies:**  :ref:`pdpy-external-framecpp` or :ref:`pdpy-external-framel` or :ref:`pdpy-external-lalframe`
+**Additional dependencies:**  :ref:`pydischarge-external-framecpp` or :ref:`pydischarge-external-framel` or :ref:`pydischarge-external-lalframe`
 
 The raw observatory data are archived in ``.gwf`` files, a custom binary format that efficiently stores the time streams and all necessary metadata, for more details about this particular data format, take a look at the specification document |GWFSpec|_.
 
 GWF library availability
 ------------------------
 
-PDpy can use any of the three named GWF input/output libraries, and will try
+pyDischarge can use any of the three named GWF input/output libraries, and will try
 to find them in the order they are listed
 (FrameCPP first, then FrameL, then LALFrame).
 If you need to read/write GWF files, any of them will work, but re recommend
 to try and install the libraries in that order; FrameCPP provides a more
 complete Python API than the others.
 
 However, not all libraries may be available on all platforms, the linked pages
@@ -133,15 +133,15 @@
 
 .. code-block:: python
 
    >>> data = TimeSeries.read('HLV-HW100916-968654552-1.gwf', 'L1:LDAS-STRAIN')
 
 .. note::
 
-   The ``HLV-HW100916-968654552-1.gwf`` file is included with the PDpy source under `/pdpy/testing/data/ <https://github.com/pdpy-github/pdpy/tree/main/pdpy/testing/data>`_.
+   The ``HLV-HW100916-968654552-1.gwf`` file is included with the pyDischarge source under `/pydischarge/testing/data/ <https://github.com/pydischarge-github/pydischarge/tree/main/pydischarge/testing/data>`_.
 
 Reading a `StateVector` uses the same syntax:
 
 .. code-block:: python
 
    >>> data = StateVector.read('my-state-data.gwf', 'L1:GWO-STATE_VECTOR')
 
@@ -198,34 +198,34 @@
 .. note::
 
    A mix of `TimeSeries` and `StateVector` objects can be read by using only `TimeSeriesDict` class, and casting the returned data to a `StateVector` using :meth:`~TimeSeries.view`.
 
 Writing
 -------
 
-To write data held in any of the :mod:`pdpy.timeseries` classes to a GWF file, simply use:
+To write data held in any of the :mod:`pydischarge.timeseries` classes to a GWF file, simply use:
 
 .. code-block:: python
 
    >>> data.write('output.gwf')
 
 **If the output file already exists it will be overwritten.**
 
-.. _pdpy-timeseries-io-hdf5:
+.. _pydischarge-timeseries-io-hdf5:
 
 ====
 HDF5
 ====
 
-PDpy allows storing data in HDF5 format files, using a custom specification for storage of metadata.
+pyDischarge allows storing data in HDF5 format files, using a custom specification for storage of metadata.
 
 .. warning::
 
    To read GWOSC data from HDF5, please see
-   :ref:`pdpy-timeseries-io-hdf5-gwosc`.
+   :ref:`pydischarge-timeseries-io-hdf5-gwosc`.
 
 Reading
 -------
 
 To read `TimeSeries` or `StateVector` data held in HDF5 files pass the filename (or filenames) or the source, and the path of the data inside the HDF5 file:
 
 .. code-block:: python
@@ -272,27 +272,27 @@
 
 To replace an existing dataset in an existing file, while preserving other data, use *both* ``append=True`` and ``overwrite=True``:
 
 .. code-block:: python
 
    >>> data.write('output.hdf', append=True, overwrite=True)
 
-.. _pdpy-timeseries-io-hdf5-gwosc:
+.. _pydischarge-timeseries-io-hdf5-gwosc:
 
 ============
 HDF5 (GWOSC)
 ============
 
 |GWOSC|_ write data in HDF5 using a custom schema that is incompatible
 with `format='hdf5'`.
 
 Reading
 -------
 
-PDpy can read data from GWOSC HDF5 files using the `format='hdf5.gwosc'`
+pyDischarge can read data from GWOSC HDF5 files using the `format='hdf5.gwosc'`
 keyword:
 
 .. code-block:: python
 
    >>> data = TimeSeries.read(
    ...     "H-H1_GWOSC_16KHZ_R1-1187056280-4096.hdf5",
    ...     format="hdf5.gwosc",
@@ -302,15 +302,15 @@
 ``/strain/Strain`` dataset, while :meth:`StateVector.read` will return those
 of ``/quality/simple``.
 
 As with regular HDF5, the ``start`` and ``end`` keyword arguments can be used
 to downselect data to a specific ``[start, end)`` time segment when reading.
 
 
-.. _pdpy-timeseries-io-wav:
+.. _pydischarge-timeseries-io-wav:
 
 ===
 WAV
 ===
 
 Any `TimeSeries` can be written to / read from a WAV file using :meth:`TimeSeries.read`:
```

### Comparing `pydischarge-0.0.1/docs/timeseries/opendata.rst` & `pydischarge-0.0.2/docs/timeseries/opendata.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-.. currentmodule:: pdpy.timeseries
+.. currentmodule:: pydischarge.timeseries
 
-.. _pdpy-timeseries-opendata:
+.. _pydischarge-timeseries-opendata:
 
 ##############################
 Accessing Open Data from GWOSC
 ##############################
 
 ******************************************
 The Gravitational-Wave Open Science Center
@@ -16,21 +16,21 @@
 
 .. note::
 
    For full details of the available data, please see
 
    https://gwosc.org/data/
 
-.. _pdpy-timeseries-fetchopendata:
+.. _pydischarge-timeseries-fetchopendata:
 
 **********************************
 :meth:`TimeSeries.fetch_open_data`
 **********************************
 
-PDpy provides the :meth:`TimeSeries.fetch_open_data` method as an interface
+pyDischarge provides the :meth:`TimeSeries.fetch_open_data` method as an interface
 to the GWOSC data archive, requiring users to provide a minimum of
 information in order to access data.
 
 For example, to fetch 30 seconds of strain data around the first ever
 gravitational-wave detection (|GW150914|_), you need to give the prefix
 of the relevant observatory (``'H1'`` for the LIGO Hanford Observatory,
 ``'L1'`` for LIGO Livingston), and the start and end times of your query.
@@ -50,30 +50,30 @@
 Then we can call :meth:`TimeSeries.fetch_open_data` to download the
 calibrated GW strain data in that interval:
 
 .. plot::
    :include-source:
    :context:
 
-   >>> from pdpy.timeseries import TimeSeries
+   >>> from pydischarge.timeseries import TimeSeries
    >>> data = TimeSeries.fetch_open_data('L1', start, end)
 
 We can then trivially plot these data:
 
 .. plot::
    :include-source:
    :context:
 
    >>> plot = data.plot()
    >>> plot.show()
 
 .. admonition:: Plotting a `TimeSeries`
 
    For more details on plotting a `TimeSeries`, see
-   :ref:`pdpy-timeseries-plot`.
+   :ref:`pydischarge-timeseries-plot`.
 
 .. note:: :meth:`TimeSeries.fetch_open_data` keywords
 
    For more details on all of the available keyword options,
    see the documentation of :meth:`TimeSeries.fetch_open_data`.
 
 **********************************************
@@ -81,8 +81,8 @@
 **********************************************
 
 |GWOSC|_ has also published a data set containing instrumental sensor data
 in a three-hour window around |GW170814|_ and throughout the entirety of O3.
 These data cannot be loaded using :meth:`TimeSeries.fetch_open_data`,
 but can be loaded using :meth:`TimeSeries.get`
 (or :meth:`TimeSeriesDict.get`), by specifying `host="losc-nds.ligo.org"`.
-For more details, see :ref:`pdpy-timeseries-get`.
+For more details, see :ref:`pydischarge-timeseries-get`.
```

### Comparing `pydischarge-0.0.1/docs/timeseries/plot.rst` & `pydischarge-0.0.2/docs/timeseries/plot.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-.. currentmodule:: pdpy.timeseries
+.. currentmodule:: pydischarge.timeseries
 
 .. plot::
    :include-source: False
    :context: reset
    :nofigs:
 
-   >>> from pdpy.timeseries import (TimeSeries, TimeSeriesDict, StateVector, StateVectorDict)
+   >>> from pydischarge.timeseries import (TimeSeries, TimeSeriesDict, StateVector, StateVectorDict)
 
-.. _pdpy-timeseries-plot:
+.. _pydischarge-timeseries-plot:
 
 #########################
 Plotting time-domain data
 #########################
 
 =========================
 Plotting one `TimeSeries`
 =========================
 
 The `TimeSeries` class includes a :meth:`~TimeSeries.plot` method to
 trivialise visualisation of the contained data.
-Reproducing the example from :ref:`pdpy-timeseries-remote`:
+Reproducing the example from :ref:`pydischarge-timeseries-remote`:
 
 .. plot::
    :include-source:
    :context:
 
    >>> l1hoft = TimeSeries.fetch_open_data('L1', 'Sep 14 2015 09:50:29', 'Sep 14 2015 09:51:01')
    >>> plot = l1hoft.plot()
    >>> plot.show()
 
-The returned object `plot` is a :class:`~pdpy.plot.Plot`, a sub-class of
+The returned object `plot` is a :class:`~pydischarge.plot.Plot`, a sub-class of
 :class:`matplotlib.figure.Figure` adapted for GPS time-stamped data.
-Customisations of the figure or the underlying :class:`~pdpy.plot.Axes` can
+Customisations of the figure or the underlying :class:`~pydischarge.plot.Axes` can
 be done using standard :mod:`matplotlib` methods.
 For example:
 
 .. plot::
    :include-source:
    :context:
 
    >>> ax = plot.gca()
    >>> ax.set_ylabel('Gravitational-wave amplitude [strain]')
    >>> ax.set_epoch(1126259462)
    >>> ax.set_title('LIGO-Livingston strain data around GW150914')
    >>> ax.axvline(1126259462, color='orange', linestyle='--')
    >>> plot.refresh()
 
-Here the :meth:`~pdpy.plot.Axes.set_epoch` method is used to reset the
+Here the :meth:`~pydischarge.plot.Axes.set_epoch` method is used to reset the
 reference time for the x-axis.
 
 =======================================
 Plotting multiple `TimeSeries` together
 =======================================
 
 Multiple `TimeSeries` classes can be combined on a figure in a number of
@@ -77,25 +77,25 @@
    >>> combined = TimeSeriesDict()
    >>> combined['L1'] = l1hoft
    >>> combined['H1'] = h1hoft
    >>> plot = combined.plot()
    >>> plot.gca().legend()
    >>> plot.show()
 
-The third method of achieving the same result is by importing and accessing the `~pdpy.plot.Plot` object directly:
+The third method of achieving the same result is by importing and accessing the `~pydischarge.plot.Plot` object directly:
 
 .. plot::
    :include-source:
    :context: close-figs
 
-   >>> from pdpy.plot import Plot
+   >>> from pydischarge.plot import Plot
    >>> plot = Plot(l1hoft, h1hoft)
    >>> plot.show()
 
-Using the `~pdpy.plot.Plot` directly allows for greater customisation.
+Using the `~pydischarge.plot.Plot` directly allows for greater customisation.
 The ``separate=True`` keyword argument can be used to plot each `TimeSeries`
 on its own axes, with ``sharex=True`` given to link the time scales for each
 :class:`~matplotlib.axes.Axes`:
 
 .. plot::
    :include-source:
    :context: close-figs
```

### Comparing `pydischarge-0.0.1/docs/timeseries/statevector.rst` & `pydischarge-0.0.2/docs/timeseries/statevector.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-.. currentmodule:: pdpy.timeseries
+.. currentmodule:: pydischarge.timeseries
 
-.. _pdpy-statevector:
+.. _pydischarge-statevector:
 
 #############
 State vectors
 #############
 
 .. code-block:: python
 
-   >>> from pdpy.timeseries import (StateTimeSeries, StateVector)
+   >>> from pydischarge.timeseries import (StateTimeSeries, StateVector)
 
 A large quantity of important data from gravitational-wave detectors
 can be distilled into simple boolean (`True` or `False`) statements
 informing something about the state of the instrument at a given time.
 These statements can be used to identify times during which a particular
 control system was active, or when the signal in a seismometer was above
 an alarming threshold, for example.
-In PDpy, these data are represented by special cases (`sub-classes`) of
+In pyDischarge, these data are represented by special cases (`sub-classes`) of
 the `TimeSeries` object:
 
 .. autosummary::
    :nosignatures:
 
    StateTimeSeries
    StateVector
@@ -35,15 +35,15 @@
 :class:`StateTimeSeries` object, a specific type of :class:`TimeSeries`
 containing only boolean values.
 
 These arrays can be generated from simple arrays of booleans, as follows:
 
 .. code-block:: python
 
-   >>> from pdpy.timeseries import StateTimeSeries
+   >>> from pydischarge.timeseries import StateTimeSeries
    >>> state = StateTimeSeries(
    ...     [True, True, False, False, False, True, False],
    ...     sample_rate=1,
    ...     epoch=1064534416,
    ... )
    >>> print(state)
    StateTimeSeries([ True,  True, False, False, False,  True, False]
@@ -54,15 +54,15 @@
                    channel: None)
 
 Alternatively, applying a standard mathematical comparison to a regular
 :class:`TimeSeries` will return a :class:`StateTimeSeries`:
 
 .. code-block:: python
 
-   >>> from pdpy.timeseries import TimeSeries
+   >>> from pydischarge.timeseries import TimeSeries
    >>> laserpower = TimeSeries.get(
    ...     "H1:IMC-PWR_IN_OUT_DQ",
    ...     1186741850,
    ...     1186741870,
    ...     host="losc-nds.ligo.org",
    ... )
    >>> threshold = 29.2 > laserpower.unit
@@ -73,15 +73,15 @@
                    t0: 1186741850.0 s,
                    dt: 0.00048828125 s,
                    name: H1:IMC-PWR_IN_OUT_DQ > 29.2 NONE,
                    channel: H1:IMC-PWR_IN_OUT_DQ)
 
 The :class:`StateTimeSeries` includes a handy
 :meth:`StateTimeSeries.to_dqflag` method to convert the boolean array
-into a :class:`~pdpy.segments.DataQualityFlag`, where the ``active``
+into a :class:`~pydischarge.segments.DataQualityFlag`, where the ``active``
 segments represent times of `True` values:
 
 .. code-block:: python
 
    >>> segments = above_29_2.to_dqflag(round=True)
    >>> print(segments)
    <DataQualityFlag('H1:IMC-PWR_IN_OUT_DQ > 29.2 NONE',
@@ -125,15 +125,15 @@
 binary system:
 
 .. plot::
    :context: reset
    :nofigs:
 
    >>> from gwosc.datasets import event_gps
-   >>> from pdpy.timeseries import StateVector
+   >>> from pydischarge.timeseries import StateVector
    >>> gps = event_gps("GW200105_162426")
    >>> start = int(gps) - 1000
    >>> end = int(gps) + 1000
    >>> gw200105_state = StateVector.fetch_open_data("L1", start, end)
    >>> print(gw200105_state)
    StateVector([127, 127, 127, ..., 127, 127, 127]
                unit: dimensionless,
@@ -152,15 +152,15 @@
                            epoch=1262274636.0))
 
 As can be seen, the list of :attr:`~StateVector.bits` is represented
 through the :class:`BitMask` class, recording the bits as a list with
 some metdata about their purpose.
 
 The `StateVector` fetched in the above example can then be parsed into a
-series of :class:`~pdpy.segments.DataQualityFlag` objects, recording the
+series of :class:`~pydischarge.segments.DataQualityFlag` objects, recording the
 active segments for that bit in the vector:
 
 .. plot::
    :context:
    :nofigs:
 
    >>> flags = gw200105_state.to_dqflags()
@@ -219,15 +219,15 @@
    The ``insetlabels=True`` keyword was given to display the bit labels
    inside the axes (otherwise they would be cut off the side of the figure).
 
 ==================
 Associated classes
 ==================
 
-Alongside the :class:`StateVector` class, :mod:`pdpy.timeseries` provides a
+Alongside the :class:`StateVector` class, :mod:`pydischarge.timeseries` provides a
 :class:`StateVectorDict` for handling collections of bit-vector data
 (mainly to enable reading and writing multiple `StateVector` in one operation).
 
 =============
 Reference/API
 =============
```

### Comparing `pydischarge-0.0.1/examples/frequencyseries/coherence.py` & `pydischarge-0.0.2/examples/frequencyseries/coherence.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Calculating the coherence between two channels
 
 The `coherence <http://en.wikipedia.org/wiki/Coherence_(physics)>`_ between
 two channels is a measure of the frequency-domain correlation between their
 time-series data.
 
@@ -27,18 +27,18 @@
 the main differential arm-length readout.
 Here we use use the :meth:`TimeSeries.coherence` method to highlight coupling
 of motion of a beam periscope attached to the main laser table into the
 strain output of the LIGO-Hanford interferometer.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 # First, we import the `TimeSeriesDict`
-from pdpy.timeseries import TimeSeriesDict
+from pydischarge.timeseries import TimeSeriesDict
 
 # and then :meth:`~TimeSeriesDict.get` the data for the strain output
 # (``H1:GDS-CALIB_STRAIN``) and the PSL periscope accelerometer
 # (``H1:PEM-CS_ACC_PSL_PERISCOPE_X_DQ``):
 data = TimeSeriesDict.get(
     ['H1:GDS-CALIB_STRAIN', 'H1:PEM-CS_ACC_PSL_PERISCOPE_X_DQ'],
     1126260017,
@@ -48,15 +48,15 @@
 acc = data['H1:PEM-CS_ACC_PSL_PERISCOPE_X_DQ']
 
 # We can then calculate the :meth:`~TimeSeries.coherence` of one
 # `TimeSeries` with respect to the other, using an 2-second Fourier
 # transform length, with a 1-second (50%) overlap:
 coh = hoft.coherence(acc, fftlength=2, overlap=1)
 
-# Finally, we can :meth:`~pdpy.frequencyseries.FrequencySeries.plot` the
+# Finally, we can :meth:`~pydischarge.frequencyseries.FrequencySeries.plot` the
 # resulting data:
 plot = coh.plot(
     xlabel='Frequency [Hz]', xscale='log',
     ylabel='Coherence', yscale='linear', ylim=(0, 1),
 )
 plot.show()
```

### Comparing `pydischarge-0.0.1/examples/frequencyseries/hoff.py` & `pydischarge-0.0.2/examples/frequencyseries/hoff.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>
 
 """Calculating and plotting a `FrequencySeries`
 
 The LIGO Laboratory has publicly released the strain data around the time of
 the GW150914 gravitational-wave detection; we can use these to calculate
 and display the spectral sensitivity of each of the detectors at that time.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.frequencyseries'
+__currentmodule__ = 'pydischarge.frequencyseries'
 
 # In order to generate a `FrequencySeries` we need to import the
-# `~pdpy.timeseries.TimeSeries` and use
-# :meth:`~pdpy.timeseries.TimeSeries.fetch_open_data` to download the strain
+# `~pydischarge.timeseries.TimeSeries` and use
+# :meth:`~pydischarge.timeseries.TimeSeries.fetch_open_data` to download the strain
 # records:
 
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 lho = TimeSeries.fetch_open_data('H1', 1126259446, 1126259478)
 llo = TimeSeries.fetch_open_data('L1', 1126259446, 1126259478)
 
-# We can then call the :meth:`~pdpy.timeseries.TimeSeries.asd` method to
+# We can then call the :meth:`~pydischarge.timeseries.TimeSeries.asd` method to
 # calculated the amplitude spectral density for each
-# `~pdpy.timeseries.TimeSeries`:
+# `~pydischarge.timeseries.TimeSeries`:
 lhoasd = lho.asd(4, 2)
 lloasd = llo.asd(4, 2)
 
 # We can then :meth:`~FrequencySeries.plot` the spectra using the 'standard'
 # colour scheme:
 
-plot = lhoasd.plot(label='LIGO-Hanford', color='pdpy:ligo-hanford')
+plot = lhoasd.plot(label='LIGO-Hanford', color='pydischarge:ligo-hanford')
 ax = plot.gca()
-ax.plot(lloasd, label='LIGO-Livingston', color='pdpy:ligo-livingston')
+ax.plot(lloasd, label='LIGO-Livingston', color='pydischarge:ligo-livingston')
 ax.set_xlim(10, 2000)
 ax.set_ylim(5e-24, 1e-21)
 ax.legend(frameon=False, bbox_to_anchor=(1., 1.), loc='lower right', ncol=2)
 plot.show()
```

### Comparing `pydischarge-0.0.1/examples/frequencyseries/inject.py` & `pydischarge-0.0.2/examples/frequencyseries/inject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Alex Urban (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Inject a known signal into a `FrequencySeries`
 
 It can often be useful to add some known signal to inherently random
 or noisy data. For example, one might want to investigate what
 would happen if a binary black hole merger signal occured at or near
 the time of a glitch. In LIGO data analysis, this procedure is referred
@@ -27,38 +27,38 @@
 
 In the example below we will create a stream of random, white Gaussian
 noise, then inject a loud, steady sinuosoid. We will do this in the
 frequency domain because it is much easier to model a sinusoid there.
 """
 
 __author__ = "Alex Urban <alexander.urban@ligo.org>"
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 # First, we prepare one second of Gaussian noise:
 
 from numpy import random
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 noise = TimeSeries(random.normal(scale=.1, size=1024), sample_rate=1024)
 
 # To inject a signal in the frequency domain, we need to take an FFT:
 
 noisefd = noise.fft()
 
 # We can now easily inject a loud sinusoid of unit amplitude at, say,
-# 30 Hz. To do this, we use :meth:`~pdpy.types.series.Series.inject`.
+# 30 Hz. To do this, we use :meth:`~pydischarge.types.series.Series.inject`.
 
 import numpy
-from pdpy.frequencyseries import FrequencySeries
+from pydischarge.frequencyseries import FrequencySeries
 signal = FrequencySeries(numpy.array([1.]), f0=30, df=noisefd.df)
 injfd = noisefd.inject(signal)
 
 # We can then visualize the data before and after injection in the frequency
 # domain:
 
-from pdpy.plot import Plot
+from pydischarge.plot import Plot
 plot = Plot(numpy.abs(noisefd), numpy.abs(injfd), separate=True,
             sharex=True, sharey=True, xscale='log', yscale='log')
 plot.show()
 
 # Finally, for completeness we can visualize the effect before and after
 # injection back in the time domain:
```

### Comparing `pydischarge-0.0.1/examples/frequencyseries/percentiles.py` & `pydischarge-0.0.2/examples/frequencyseries/percentiles.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>
 
 """Plotting an averaged ASD with percentiles.
 
-As we have seen in :ref:`pdpy-example-frequencyseries-hoff`, the Amplitude
+As we have seen in :ref:`pydischarge-example-frequencyseries-hoff`, the Amplitude
 Spectral Density (ASD) is a key indicator of frequency-domain sensitivity for
 a gravitational-wave detector.
 
 However, the ASD doesn't allow you to see how much the sensitivity varies
 over time.
-One tool for that is the :ref:`spectrogram <pdpy-spectrogram>`, while another
+One tool for that is the :ref:`spectrogram <pydischarge-spectrogram>`, while another
 is simply to show percentiles of a number of ASD measurements.
 
 In this example we calculate the median ASD over 2048-seconds surrounding
 the GW178017 event, and also the 5th and 95th percentiles of the ASD, and
 plot them on a single figure.
 """
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 # First, as always, we get the data using :meth:`TimeSeries.fetch_open_data`:
 
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 hoft = TimeSeries.fetch_open_data('H1', 1187007040, 1187009088)
 
-# Next we calculate a :class:`~pdpy.spectrogram.Spectrogram` by calculating
-# a number of ASDs, using the :meth:`~pdpy.timeseries.TimeSeries.spectrogram2`
+# Next we calculate a :class:`~pydischarge.spectrogram.Spectrogram` by calculating
+# a number of ASDs, using the :meth:`~pydischarge.timeseries.TimeSeries.spectrogram2`
 # method:
 
 sg = hoft.spectrogram2(fftlength=4, overlap=2, window='hann') ** (1 / 2.)
 
 # From this we can trivially extract the median, 5th and 95th percentiles:
 
 median = sg.percentile(50)
 low = sg.percentile(5)
 high = sg.percentile(95)
 
-# Finally, we can make plot, using :meth:`~pdpy.plot.Axes.plot_mmm` to
+# Finally, we can make plot, using :meth:`~pydischarge.plot.Axes.plot_mmm` to
 # display the 5th and 95th percentiles as a shaded region around the median:
 
-from pdpy.plot import Plot
+from pydischarge.plot import Plot
 plot = Plot()
 ax = plot.add_subplot(
     xscale='log', xlim=(10, 1500), xlabel='Frequency [Hz]',
     yscale='log', ylim=(3e-24, 2e-20),
     ylabel=r'Strain noise [1/$\sqrt{\mathrm{Hz}}$]',
 )
-ax.plot_mmm(median, low, high, color='pdpy:ligo-hanford')
+ax.plot_mmm(median, low, high, color='pydischarge:ligo-hanford')
 ax.set_title('LIGO-Hanford strain noise variation around GW170817',
              fontsize=16)
 plot.show()
 
 # Now we can see that the ASD varies by factors of a few across most of the
 # frequency band, with notable exceptions, e.g. around the 60-Hz power line
 # harmonics (60 Hz, 120 Hz, 180 Hz, ...) where the noise is very stable.
```

### Comparing `pydischarge-0.0.1/examples/frequencyseries/rayleigh.py` & `pydischarge-0.0.2/examples/frequencyseries/rayleigh.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Plotting a Rayleigh-statistic `Spectrum`
 
 In LIGO the 'Rayleigh' statistic is a calculation of the
 `coefficient of variation
 <https://en.wikipedia.org/wiki/Coefficient_of_variation>`_ of the
 power spectral density (PSD) of a given set of data.
@@ -27,33 +27,33 @@
 indicates Gaussian behaviour, less than 1 indicates coherent variations,
 and greater than 1 indicates incoherent variation.
 It is a useful measure of the quality of the strain data being generated
 and recorded at a LIGO site.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.frequencyseries'
+__currentmodule__ = 'pydischarge.frequencyseries'
 
 # To demonstate this, we can load some data from the LIGO Livingston
 # intereferometer around the time of the GW151226 gravitational wave detection:
 
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 gwdata = TimeSeries.fetch_open_data('L1', 'Dec 26 2015 03:37',
                                     'Dec 26 2015 03:47', verbose=True)
 
 # Next, we can calculate a Rayleigh statistic `FrequencySeries` using the
-# :meth:`~pdpy.timeseries.TimeSeries.rayleigh_spectrum` method of the
-# `~pdpy.timeseries.TimeSeries` with a 2-second FFT and 1-second overlap (50%):
+# :meth:`~pydischarge.timeseries.TimeSeries.rayleigh_spectrum` method of the
+# `~pydischarge.timeseries.TimeSeries` with a 2-second FFT and 1-second overlap (50%):
 
 rayleigh = gwdata.rayleigh_spectrum(2, 1)
 
 # For easy comparison, we can calculate the spectral sensitivity ASD of the
 # strain data and plot both on the same figure:
 
-from pdpy.plot import Plot
+from pydischarge.plot import Plot
 plot = Plot(gwdata.asd(2, 1), rayleigh, geometry=(2, 1), sharex=True,
             xscale='log', xlim=(30, 1500))
 asdax, rayax = plot.axes
 
 asdax.set_yscale('log')
 asdax.set_ylim(5e-24, 1e-21)
 asdax.set_ylabel(r'[strain/$\sqrt{\mathrm{Hz}}$]')
```

### Comparing `pydischarge-0.0.1/examples/frequencyseries/transfer_function.py` & `pydischarge-0.0.2/examples/frequencyseries/transfer_function.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Plotting a transfer function
 
 I would like to study how a signal transfers from one part of the
 interferometer to another.
 
 Specifically, it is interesting to measure the amplitude transfer of
 ground motion through the HEPI system.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 if __name__ == '__main__':
     from matplotlib import pyplot
     pyplot.ion()
 
 # Before anything else, we import the objects we will need:
-from pdpy.time import tconvert
-from pdpy.timeseries import TimeSeriesDict
-from pdpy.plot import BodePlot
+from pydischarge.time import tconvert
+from pydischarge.timeseries import TimeSeriesDict
+from pydischarge.plot import BodePlot
 
 # and set the times of our query, and the channels we want:
 start = tconvert('May 27 2014 04:00')
 end = start + 1800
 gndchannel = 'L1:ISI-GND_STS_ITMY_Z_DQ'
 hpichannel = 'L1:HPI-ITMY_BLND_L4C_Z_IN1_DQ'
 
@@ -50,14 +50,14 @@
 gnd = data[gndchannel]
 hpi = data[hpichannel]
 
 # The transfer function between time series is easily computed with the
 # :meth:`~TimeSeries.transfer_function` method:
 tf = gnd.transfer_function(hpi, 100, 50)
 
-# The `~pdpy.plot.BodePlot` knows how to separate a complex-valued
-# `~pdpy.frequencyseries.FrequencySeries` into magnitude and phase:
+# The `~pydischarge.plot.BodePlot` knows how to separate a complex-valued
+# `~pydischarge.frequencyseries.FrequencySeries` into magnitude and phase:
 plot = BodePlot(tf)
 plot.maxes.set_title(
     r'L1 ITMY ground $\rightarrow$ HPI transfer function')
 plot.maxes.set_ylim(-55, 50)
 plot.show()
```

### Comparing `pydischarge-0.0.1/examples/frequencyseries/variance.py` & `pydischarge-0.0.2/examples/frequencyseries/variance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Calculating and plotting a `SpectralVariance` histogram
 
 The most common visualisation of the spectral content of a data series is
 via the power or amplitude spectral density calculations (PSD or ASD).
 However, these typically involve averaging of the data over a period, which
 can wash out transient noise (as is often desired).
 
-The `SpectralVariance` histogram provide by `pdpy.frequencyseries` allows
+The `SpectralVariance` histogram provide by `pydischarge.frequencyseries` allows
 us to look at the spectral sensitivity in a different manner, displaying
 which frequencies sit at which amplitude _most_ of the time, but also
 highlighting excursions from normal behaviour.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.frequencyseries'
+__currentmodule__ = 'pydischarge.frequencyseries'
 
 # To demonstate this, we can load some data from the LIGO Livingston
 # intereferometer around the time of the GW151226 gravitational wave detection:
 
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 llo = TimeSeries.fetch_open_data('L1', 1135136228, 1135140324, verbose=True)
 
-# We can then call the :meth:`~pdpy.timeseries.TimeSeries.spectral_variance`
-# method of the ``llo`` `~pdpy.timeseries.TimeSeries` by calculating an ASD
+# We can then call the :meth:`~pydischarge.timeseries.TimeSeries.spectral_variance`
+# method of the ``llo`` `~pydischarge.timeseries.TimeSeries` by calculating an ASD
 # every 5 seconds and counting the amount of time each frequency bin spends
 # at each ASD value:
 
 variance = llo.spectral_variance(5, fftlength=2, overlap=1, log=True,
                                  low=1e-24, high=1e-19, nbins=100)
 
 # We can then :meth:`~SpectralVariance.plot` the `SpectralVariance`
```

### Comparing `pydischarge-0.0.1/examples/miscellaneous/open-data-spectrogram.py` & `pydischarge-0.0.2/examples/miscellaneous/open-data-spectrogram.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2019-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Plotting a spectrogram of all open data for 1 day
 
 In order to study interferometer performance, it is common in LIGO to plot
 all of the data for a day, in order to determine trends, and see data-quality
 issues.
 
@@ -30,25 +30,25 @@
 This example demonstrates how to download data segments from GWOSC, then
 use those to build a day-timescale spectrogram plot of LIGO-Hanford strain
 data.
 """
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
-# .. currentmodule:: pdpy.segments
+# .. currentmodule:: pydischarge.segments
 #
 # Getting the segments
 # --------------------
 #
 # First, we need to fetch the Open Data timeline segments from GWOSC.
 # To do that we can call the :meth:`DataQualityFlag.fetch_open_data` method
 # using ``'H1_DATA'`` as the flag (for an explanation of what this means,
 # read up on `The S6 Data Release <https://gwosc.org/S6/>`__).
 
-from pdpy.segments import DataQualityFlag
+from pydischarge.segments import DataQualityFlag
 h1segs = DataQualityFlag.fetch_open_data('H1_DATA',
                                          'Sep 16 2010', 'Sep 17 2010')
 
 # For sanity, lets plot these segments:
 
 splot = h1segs.plot(figsize=[12, 3])
 splot.show()
@@ -58,33 +58,33 @@
 # majority of the day, with a few outages of ~30 minutes or so.
 
 # We can use the :func:`abs` function to display the total amount of time
 # spent taking data:
 
 print(abs(h1segs.active))
 
-# .. currentmodule:: pdpy.timeseries
+# .. currentmodule:: pydischarge.timeseries
 #
 # Working with strain data
 # ------------------------
 #
 # Now, we can loop through the active segments of ``'H1_DATA'`` and fetch the
 # strain `TimeSeries` for each segment, calculating a
-# :class:`~pdpy.spectrogram.Spectrogram` for each segment.
+# :class:`~pydischarge.spectrogram.Spectrogram` for each segment.
 
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 spectrograms = []
 for start, end in h1segs.active:
     h1strain = TimeSeries.fetch_open_data('H1', start, end, verbose=True)
     specgram = h1strain.spectrogram(30, fftlength=4) ** (1/2.)
     spectrograms.append(specgram)
 
-# Finally, we can build a :meth:`~pdpy.spectrogram.Spectrogram.plot`:
+# Finally, we can build a :meth:`~pydischarge.spectrogram.Spectrogram.plot`:
 
-from pdpy.plot import Plot
+from pydischarge.plot import Plot
 plot = Plot(figsize=(12, 6))
 ax = plot.gca()
 for specgram in spectrograms:
     ax.imshow(specgram)
 ax.set_xscale('auto-gps', epoch='Sep 16 2010')
 ax.set_xlim('Sep 16 2010', 'Sep 17 2010')
 ax.set_ylim(40, 2000)
```

### Comparing `pydischarge-0.0.1/examples/miscellaneous/range-spectrogram.py` & `pydischarge-0.0.2/examples/miscellaneous/range-spectrogram.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Alex Urban (2019-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Estimating the spectral contribution to inspiral range
 
 We have seen how the binary neutron star (BNS) inspiral range of a
 gravitational-wave detector can be measured directly from the strain
 readout. In this example, we will estimate the average spectral
 contribution to BNS range from the strain record surrounding GW170817
-using :func:`pdpy.astro.range_spectrogram`.
+using :func:`pydischarge.astro.range_spectrogram`.
 """
 
 __author__ = 'Alex Urban <alexander.urban@ligo.org>'
 
 # First, we need to load some data. As before we can `fetch` the
 # `public data <https://gwosc.org/catalog/>`__
 # around the GW170817 BNS merger:
 
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 l1 = TimeSeries.fetch_open_data('L1', 1187006834, 1187010930)
 
 # Then, we can calculate a `Spectrogram` of the inspiral range
 # amplitude spectrum:
 
-from pdpy.astro import range_spectrogram
+from pydischarge.astro import range_spectrogram
 l1spec = range_spectrogram(l1, 30, fftlength=4, fmin=15, fmax=500) ** (1./2)
 
 # We can plot this `Spectrogram` to visualise spectral variation in
 # LIGO-Livingston's sensitivity in the hour or so surrounding GW170817:
 
 plot = l1spec.plot(figsize=(12, 5))
 ax = plot.gca()
```

### Comparing `pydischarge-0.0.1/examples/miscellaneous/range-timeseries.py` & `pydischarge-0.0.2/examples/miscellaneous/range-timeseries.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2019-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Generating an inspiral range timeseries
 
 One standard figure-of-merit for the sensitivity of a gravitational-wave
 detector is the distance to which a binary neutron star (BNS) inspiral
 with two 1.4 solar mass components would be detected with a signal-to-noise
 ratio (SNR) of 8. We can estimate this using
-:func:`pdpy.astro.range_timeseries` directly from the strain readout for
+:func:`pydischarge.astro.range_timeseries` directly from the strain readout for
 a detector.
 """
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 __credits__ = 'Alex Urban <alexander.urban@ligo.org>'
 
 # First, we need to load some data. We can `fetch` the
 # `public data <https://gwosc.org/catalog/>`__
 # around the GW170817 BNS merger:
 
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 h1 = TimeSeries.fetch_open_data('H1', 1187006834, 1187010930)
 l1 = TimeSeries.fetch_open_data('L1', 1187006834, 1187010930)
 
 # Then, we can measure the inspiral range directly:
 
-from pdpy.astro import range_timeseries
+from pydischarge.astro import range_timeseries
 h1range = range_timeseries(h1, 30, fftlength=4, fmin=10)
 l1range = range_timeseries(l1, 30, fftlength=4, fmin=10)
 
 # We can now plot these trends to see the variation in LIGO
 # sensitivity over an hour or so surrounding GW170817:
 
 plot = h1range.plot(
-    label='LIGO-Hanford', color='pdpy:ligo-hanford', figsize=(12, 5))
+    label='LIGO-Hanford', color='pydischarge:ligo-hanford', figsize=(12, 5))
 ax = plot.gca()
-ax.plot(l1range, label='LIGO-Livingston', color='pdpy:ligo-livingston')
+ax.plot(l1range, label='LIGO-Livingston', color='pydischarge:ligo-livingston')
 ax.set_ylabel('Angle-averaged sensitive distance [Mpc]')
 ax.set_title('LIGO sensitivity to BNS around GW170817')
 ax.set_epoch(1187008882)  # <- set 0 on plot to GW170817
 ax.legend()
 plot.show()
 
 # Note, the extreme dip in LIGO-Livingston's sensitivity near GW170817
```

### Comparing `pydischarge-0.0.1/examples/segments/open-data.py` & `pydischarge-0.0.2/examples/segments/open-data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Plotting observing segments for O1
 
 The data from the full
 `Observing Run 1 (O1) <https://gwosc.org/O1/>`__
 have been released by |GWOSC|_.
 
 This example demonstrates how to download segment information into a
-:class:`~pdpy.segments.DataQualityFlag`, and then plot them.
+:class:`~pydischarge.segments.DataQualityFlag`, and then plot them.
 """
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
-__currentmodule__ = 'pdpy.segments'
+__currentmodule__ = 'pydischarge.segments'
 
 # All we need to do is import the `DataQualityFlag` object, and then call
 # the :meth:`DataQualityFlag.fetch_open_data` method to query for, and download
 # the segments for all of O1:
 
-from pdpy.segments import DataQualityFlag
+from pydischarge.segments import DataQualityFlag
 h1segs = DataQualityFlag.fetch_open_data('H1_DATA', 'Sep 12 2015',
                                          'Jan 19 2016')
 
 # We can then generate a plot of the times when LIGO-Hanford was operating:
 
-plot = h1segs.plot(color='pdpy:ligo-hanford')
+plot = h1segs.plot(color='pydischarge:ligo-hanford')
 plot.show()
 
 # That's a lot of segments. We can pare-down the list a little to display
 # only the segments from the first month of the run:
 
 h1month1 = DataQualityFlag.fetch_open_data('H1_DATA', 'Sep 12 2015',
                                            'Oct 12 2015')
 
 # We can also download the LIGO-Livingston segments from the same period
 # and display them alongside, as well as those segments during which both
 # interferometers were operating at the same time
-# (see :ref:`pdpy-segments-intersection` for more details on this use of the
+# (see :ref:`pydischarge-segments-intersection` for more details on this use of the
 # ``&`` operator):
 
 l1month1 = DataQualityFlag.fetch_open_data('L1_DATA', 'Sep 12 2015',
                                            'Oct 12 2015')
 bothon = h1month1 & l1month1
 plot = h1month1.plot()
 ax = plot.gca()
```

### Comparing `pydischarge-0.0.1/examples/signal/gw150914.py` & `pydischarge-0.0.2/examples/signal/gw150914.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2016-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Filtering a `TimeSeries` to detect gravitational waves
 
 The raw 'strain' output of the LIGO detectors is recorded as a `TimeSeries`
 with contributions from a large number of known and unknown noise sources,
 as well as possible gravitational wave signals.
 
 In order to uncover a real signal we need to filter out noises that otherwise
-hide the signal in the data. We can do this by using the :mod:`pdpy.signal`
+hide the signal in the data. We can do this by using the :mod:`pydischarge.signal`
 module to design a digital filter to cut out low and high frequency noise, as
 well as notch out fixed frequencies polluted by known artefacts.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 # First we download the raw strain data from the GWOSC public archive:
 
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 hdata = TimeSeries.fetch_open_data('H1', 1126259446, 1126259478)
 
 # Next we can design a zero-pole-gain filter to remove the extranious noise.
 
-# First we import the `pdpy.signal.filter_design` module and create a
-# :meth:`~pdpy.signal.filter_design.bandpass` filter to remove both low and
+# First we import the `pydischarge.signal.filter_design` module and create a
+# :meth:`~pydischarge.signal.filter_design.bandpass` filter to remove both low and
 # high frequency content
 
-from pdpy.signal import filter_design
+from pydischarge.signal import filter_design
 bp = filter_design.bandpass(50, 250, hdata.sample_rate)
 
 # Now we want to combine the bandpass with a series of
-# :meth:`~pdpy.signal.filter_design.notch` filters, so we create those
+# :meth:`~pydischarge.signal.filter_design.notch` filters, so we create those
 # for the first three harmonics of the 60 Hz AC mains power:
 
 notches = [filter_design.notch(line, hdata.sample_rate) for
            line in (60, 120, 180)]
 
 # and concatenate each of our filters together to create a single ZPK:
 
@@ -61,48 +61,48 @@
 # to filter both backwards and forwards to preserve the correct phase
 # at all frequencies
 
 hfilt = hdata.filter(zpk, filtfilt=True)
 
 # .. note::
 #
-#    The :mod:`~pdpy.signal.filter_design` methods return digital filters
+#    The :mod:`~pydischarge.signal.filter_design` methods return digital filters
 #    by default, so we apply them using `TimeSeries.filter`. If we had
 #    analogue filters (perhaps by passing `analog=True` to the filter design
 #    method), the easiest application would be `TimeSeries.zpk`
 
-# The :mod:`~pdpy.signal.filter_design` methods return infinite impulse
+# The :mod:`~pydischarge.signal.filter_design` methods return infinite impulse
 # response filters by default, which, when applied, corrupt a small amount of
 # data at the beginning and the end of our original `TimeSeries`.
 # We can discard those data using the :meth:`~TimeSeries.crop` method
 # (for consistency we apply this to both data series):
 
 hdata = hdata.crop(*hdata.span.contract(1))
 hfilt = hfilt.crop(*hfilt.span.contract(1))
 
 # Finally, we can :meth:`~TimeSeries.plot` the original and filtered data,
 # adding some code to prettify the figure:
 
-from pdpy.plot import Plot
+from pydischarge.plot import Plot
 plot = Plot(hdata, hfilt, figsize=[12, 6], separate=True, sharex=True,
-            color='pdpy:ligo-hanford')
+            color='pydischarge:ligo-hanford')
 ax1, ax2 = plot.axes
 ax1.set_title('LIGO-Hanford strain data around GW150914')
 ax1.text(1.0, 1.01, 'Unfiltered data', transform=ax1.transAxes, ha='right')
 ax1.set_ylabel('Amplitude [strain]', y=-0.2)
 ax2.set_ylabel('')
 ax2.text(1.0, 1.01, r'50-250\,Hz bandpass, notches at 60, 120, 180 Hz',
          transform=ax2.transAxes, ha='right')
 plot.show()
 plot.close()  # hide
 
 # We see now a spike around 16 seconds into the data, so let's zoom into
 # that time (and prettify):
 
-plot = hfilt.plot(color='pdpy:ligo-hanford')
+plot = hfilt.plot(color='pydischarge:ligo-hanford')
 ax = plot.gca()
 ax.set_title('LIGO-Hanford strain data around GW150914')
 ax.set_ylabel('Amplitude [strain]')
 ax.set_xlim(1126259462, 1126259462.6)
 ax.set_xscale('seconds', epoch=1126259462)
 plot.show()
 plot.close()  # hide
@@ -125,16 +125,16 @@
 lfilt.shift('6.9ms')
 lfilt *= -1
 
 # and finally make a new plot with both detectors:
 
 plot = Plot(figsize=[12, 4])
 ax = plot.gca()
-ax.plot(hfilt, label='LIGO-Hanford', color='pdpy:ligo-hanford')
-ax.plot(lfilt, label='LIGO-Livingston', color='pdpy:ligo-livingston')
+ax.plot(hfilt, label='LIGO-Hanford', color='pydischarge:ligo-hanford')
+ax.plot(lfilt, label='LIGO-Livingston', color='pydischarge:ligo-livingston')
 ax.set_title('LIGO strain data around GW150914')
 ax.set_xlim(1126259462, 1126259462.6)
 ax.set_xscale('seconds', epoch=1126259462)
 ax.set_ylabel('Amplitude [strain]')
 ax.set_ylim(-1e-21, 1e-21)
 ax.legend()
 plot.show()
```

### Comparing `pydischarge-0.0.1/examples/signal/qscan.py` & `pydischarge-0.0.2/examples/signal/qscan.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Alex Urban (2019-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Compute the raw Q-transform of a `TimeSeries`
 
 One of the most useful tools for visualising short-duration features in a
 `TimeSeries` is the `Q-transform
 <https://en.wikipedia.org/wiki/Constant-Q_transform>`_.
 This tool is routinely used by data analysts to produce time-frequency maps of
@@ -29,28 +29,28 @@
 Below we use this algorithm to visualise GW170817, a gravitational-wave
 signal from two merging neutron stars. In the LIGO-Livingston (L1) detector,
 the end of this signal coincides with a very loud glitch (`Phys. Rev. Lett.
 vol. 119, p. 161101 <http://doi.org/10.1103/PhysRevLett.119.161101>`_).
 """
 
 __author__ = "Alex Urban <alexander.urban@ligo.org>"
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 # First, we need to download the `TimeSeries` record of L1 strain measurements
 # from |GWOSC|_:
 
 from gwosc import datasets
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 gps = datasets.event_gps('GW170817')
 data = TimeSeries.fetch_open_data('L1', gps-34, gps+34)
 
 # We can Q-transform these data and scan over time-frequency planes to
 # find the one with the most significant tile near the time of merger:
 
-from pdpy.segments import Segment
+from pydischarge.segments import Segment
 qgram = data.q_gram(
     qrange=(4, 150),
     search=Segment(gps-0.25, gps+0.25),
     mismatch=0.35,
 )
 
 # .. note::
```

### Comparing `pydischarge-0.0.1/examples/spectrogram/coherence.py` & `pydischarge-0.0.2/examples/spectrogram/coherence.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Calculating the time-dependent coherence between two channels
 
 The standard coherence calculation outputs a frequency series
-(`~pdpy.frequencyseries.FrequencySeries`) giving a time-averaged measure
-of coherence. See :ref:`pdpy-example-frequencyseries-coherence` for an
+(`~pydischarge.frequencyseries.FrequencySeries`) giving a time-averaged measure
+of coherence. See :ref:`pydischarge-example-frequencyseries-coherence` for an
 example.
 
 The `TimeSeries` method :meth:`~TimeSeries.coherence_spectrogram` performs the
 same coherence calculation every ``stride``, giving a time-varying coherence
 measure.
 
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 # First, we import the `TimeSeriesDict`
-from pdpy.timeseries import TimeSeriesDict
+from pydischarge.timeseries import TimeSeriesDict
 
 # and then :meth:`~TimeSeriesDict.get` the data for the strain output
 # (``H1:GDS-CALIB_STRAIN``) and the PSL periscope accelerometer
 # (``H1:PEM-CS_ACC_PSL_PERISCOPE_X_DQ``):
 data = TimeSeriesDict.get(
     ['H1:GDS-CALIB_STRAIN', 'H1:PEM-CS_ACC_PSL_PERISCOPE_X_DQ'],
     1126260017,
@@ -48,15 +48,15 @@
 acc = data['H1:PEM-CS_ACC_PSL_PERISCOPE_X_DQ']
 
 # We can then calculate the :meth:`~TimeSeries.coherence` of one
 # `TimeSeries` with respect to the other, using an 2-second Fourier
 # transform length, with a 1-second (50%) overlap:
 coh = hoft.coherence_spectrogram(acc, 10, fftlength=.5, overlap=.25)
 
-# Finally, we can :meth:`~pdpy.spectrogram.Spectrogram.plot` the
+# Finally, we can :meth:`~pydischarge.spectrogram.Spectrogram.plot` the
 # resulting data
 plot = coh.plot()
 ax = plot.gca()
 ax.set_ylabel('Frequency [Hz]')
 ax.set_yscale('log')
 ax.set_ylim(10, 8000)
 ax.set_title(
```

### Comparing `pydischarge-0.0.1/examples/spectrogram/plot.py` & `pydischarge-0.0.2/examples/spectrogram/plot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Plotting a `Spectrogram`
 
 One of the most useful methods of visualising gravitational-wave data is to
 use a spectrogram, highlighting the frequency-domain content of some data
 over a number of time steps.
 
 For this example we can use the public data around the GW150914 detection.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 # First, we import the `TimeSeries` and call
 # :meth:`TimeSeries.fetch_open_data` the download the strain
 # data for the LIGO-Hanford interferometer
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 data = TimeSeries.fetch_open_data(
     'H1', 'Sep 14 2015 09:45', 'Sep 14 2015 09:55')
 
-# Next, we can calculate a `~pdpy.spectrogram.Spectrogram` using the
+# Next, we can calculate a `~pydischarge.spectrogram.Spectrogram` using the
 # :meth:`spectrogram` method of the `TimeSeries` over a 2-second stride
 # with a 1-second FFT and # .5-second overlap (50%):
 specgram = data.spectrogram(2, fftlength=1, overlap=.5) ** (1/2.)
 
 # .. note::
 #    :meth:`TimeSeries.spectrogram` returns a Power Spectral Density (PSD)
-#    `~pdpy.spectrogram.Spectrogram` by default, so we use the ``** (1/2.)``
+#    `~pydischarge.spectrogram.Spectrogram` by default, so we use the ``** (1/2.)``
 #    to convert this into a (more familiar) Amplitude Spectral Density.
 
 # Finally, we can make a plot using the
-# :meth:`~pdpy.spectrogram.Spectrogram.plot` method
+# :meth:`~pydischarge.spectrogram.Spectrogram.plot` method
 plot = specgram.imshow(norm='log', vmin=5e-24, vmax=1e-19)
 ax = plot.gca()
 ax.set_yscale('log')
 ax.set_ylim(10, 2000)
 ax.colorbar(
     label=r'Gravitational-wave amplitude [strain/$\sqrt{\mathrm{Hz}}$]')
 plot.show()
 
 # This shows the relative stability of the interferometer sensitivity over
 # the ten-minute span. Despite there being a gravitational-wave signal in the
 # data, the resolution (and dynamic range) of the spectrogram make it
-# impossible to see. The :ref:`next example <pdpy-example-spectrogram-ratio>`
-# shows you how to normalise a `~pdpy.spectrogram.Spectrogram` to better
+# impossible to see. The :ref:`next example <pydischarge-example-spectrogram-ratio>`
+# shows you how to normalise a `~pydischarge.spectrogram.Spectrogram` to better
 # see features in the most sensitive frequency band.
```

### Comparing `pydischarge-0.0.1/examples/spectrogram/ratio.py` & `pydischarge-0.0.2/examples/spectrogram/ratio.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Plotting a normalised `~pdpy.spectrogram.Spectrogram`
+"""Plotting a normalised `~pydischarge.spectrogram.Spectrogram`
 
-The :ref:`previous example <pdpy-example-spectrogram-plot>` showed how to
-generate and display a `~pdpy.spectrogram.Spectrogram` of the LIGO-Hanford
+The :ref:`previous example <pydischarge-example-spectrogram-plot>` showed how to
+generate and display a `~pydischarge.spectrogram.Spectrogram` of the LIGO-Hanford
 strain data around the GW150914 event.
 
 However, because of the shape of the LIGO sensitivity curve, picking out
 features in the most sensitive frequency band (a few hundred Hertz) is
 very hard.
 
-We can normalise our `~pdpy.spectrogram.Spectrogram` to highligh those
+We can normalise our `~pydischarge.spectrogram.Spectrogram` to highligh those
 features.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 # Again, we import the `TimeSeries` and call
 # :meth:`TimeSeries.fetch_open_data` the download the strain
 # data for the LIGO-Hanford interferometer
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 data = TimeSeries.fetch_open_data(
     'H1', 'Sep 14 2015 09:45', 'Sep 14 2015 09:55')
 
-# Next, we can calculate a `~pdpy.spectrogram.Spectrogram` using the
+# Next, we can calculate a `~pydischarge.spectrogram.Spectrogram` using the
 # :meth:`spectrogram` method of the `TimeSeries` over a 2-second stride
 # with a 1-second FFT and # .5-second overlap (50%):
 specgram = data.spectrogram(2, fftlength=1, overlap=.5) ** (1/2.)
 
 # and can normalise it against the overall median ASD by calling the
-# :meth:`~pdpy.spectrogram.Spectrogram.ratio` method:
+# :meth:`~pydischarge.spectrogram.Spectrogram.ratio` method:
 
 normalised = specgram.ratio('median')
 
 # Finally, we can make a plot using the
-# :meth:`~pdpy.spectrogram.Spectrogram.plot` method
+# :meth:`~pydischarge.spectrogram.Spectrogram.plot` method
 plot = normalised.plot(norm='log', vmin=.1, vmax=10, cmap='Spectral_r')
 ax = plot.gca()
 ax.set_yscale('log')
 ax.set_ylim(10, 2000)
 ax.colorbar(label='Relative amplitude')
 plot.show()
 
 # Even with a normalised spectrogram, the resolution is such that a signal
 # as short as that of GW150914 is impossible to see. The
-# :ref:`next example <pdpy-example-spectrogram-spectrogram2>` uses
+# :ref:`next example <pydischarge-example-spectrogram-spectrogram2>` uses
 # a high-resolution spectrogram method to zoom in around the exact time of
 # the signal.
```

### Comparing `pydischarge-0.0.1/examples/spectrogram/rayleigh.py` & `pydischarge-0.0.2/examples/spectrogram/rayleigh.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Plotting a `Spectrogram` of the Rayleigh statistic
 
-As described in :ref:`pdpy-example-frequencyseries-rayleigh`, the Rayleigh
+As described in :ref:`pydischarge-example-frequencyseries-rayleigh`, the Rayleigh
 statistic can be used to study non-Gaussianity in a timeseries.
 We can study the time variance of these features by plotting a
 time-frequency spectrogram where we calculate the Rayleigh statistic for
 each time bin.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.spectrogram'
+__currentmodule__ = 'pydischarge.spectrogram'
 
 # To demonstate this, we can load some data from the LIGO Livingston
 # intereferometer around the time of the GW151226 gravitational wave detection:
 
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 gwdata = TimeSeries.fetch_open_data('L1', 'Dec 26 2015 03:37',
                                     'Dec 26 2015 03:47', verbose=True)
 
 # Next, we can calculate a Rayleigh statistic `Spectrogram` using the
-# :meth:`~pdpy.timeseries.TimeSeries.rayleigh_spectrogram` method of the
-# `~pdpy.timeseries.TimeSeries` and a 5-second stride with a 2-second FFT and
+# :meth:`~pydischarge.timeseries.TimeSeries.rayleigh_spectrogram` method of the
+# `~pydischarge.timeseries.TimeSeries` and a 5-second stride with a 2-second FFT and
 # 1-second overlap (50%):
 rayleigh = gwdata.rayleigh_spectrogram(5, fftlength=2, overlap=1)
 
 # and can make a plot using the :meth:`~Spectrogram.plot` method
 plot = rayleigh.plot(norm='log', vmin=0.25, vmax=4)
 ax = plot.gca()
 ax.set_yscale('log')
```

### Comparing `pydischarge-0.0.1/examples/spectrogram/spectrogram2.py` & `pydischarge-0.0.2/examples/spectrogram/spectrogram2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Plotting an over-dense, short-duration `Spectrogram`
 
 The normal `~TimeSeries.spectrogram` method uses non-overlapping intervals
 to calculate discrete PSDs for each stride. This is fine for long-duration
 data, but give poor resolution when studying short-duration phenomena.
 
 The `~TimeSeries.spectrogram2` method allows for highly-overlapping FFT
 calculations to over-sample the frequency content of the input `TimeSeries`
 to produce a much more feature-rich output.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 # To demonstrate this, we can download some data associated with the
 # gravitational-wave event GW510914:
 
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 lho = TimeSeries.fetch_open_data('H1', 1126259458, 1126259467, verbose=True)
 
 # and can :meth:`~TimeSeries.highpass` and :meth:`~TimeSeries.whiten`
 # the remove low-frequency noise and try and enhance low-amplitude signals
 # across the middle of the frequency band:
 
 hp = lho.highpass(20)
@@ -47,15 +47,15 @@
 # .. note::
 #
 #    We chose to :meth:`~TimeSeries.crop` out the leading and trailing 2
 #    seconds of the the whitened data series here to remove any filtering
 #    artefacts that may have been introduced.
 
 # Now we can call the `~TimeSeries.spectrogram2` method of `gwdata` to
-# calculate our over-dense `~pdpy.spectrogram.Spectrogram`, using a
+# calculate our over-dense `~pydischarge.spectrogram.Spectrogram`, using a
 # 1/16-second FFT length and high overlap:
 
 specgram = white.spectrogram2(fftlength=1/16., overlap=15/256.) ** (1/2.)
 specgram = specgram.crop_frequencies(20)  # drop everything below highpass
 
 # Finally, we make a plot:
```

### Comparing `pydischarge-0.0.1/examples/table/histogram.py` & `pydischarge-0.0.2/examples/table/histogram.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Plotting an `EventTable` in a histogram
 
 I would like to study the distribution of the GW events detected to date.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.table'
+__currentmodule__ = 'pydischarge.table'
 
 # First, we can download the ``'GWTC-1-confident'`` catalogue using
 # :meth:`EventTable.fetch_open_data`:
 
-from pdpy.table import EventTable
+from pydischarge.table import EventTable
 events = EventTable.fetch_open_data(
     "GWTC-1-confident",
     columns=("mass_1_source", "mass_2_source"),
 )
 events.add_column(
     events["mass_1_source"] + events["mass_2_source"],
     name="mtotal"
 )
 
-# and can generate a new `~pdpy.plot.Plot` using the
+# and can generate a new `~pydischarge.plot.Plot` using the
 # :meth:`~EventTable.hist` method:
 
 plot = events.hist('mtotal', bins=10, range=(0, 100), histtype='stepfilled')
 ax = plot.gca()
 ax.set_xlabel(r"Total mass [M$_{\odot}$]")
 ax.set_ylabel("Number of events")
 ax.set_title("GWTC-1-confident")
```

### Comparing `pydischarge-0.0.1/examples/table/rate.py` & `pydischarge-0.0.2/examples/table/rate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Calculating (and plotting) rate versus time for an `EventTable`
 
 I would like to study the rate at which event triggers are generated by the
 `ExcessPower` gravitational-wave burst detection algorithm, over a small
 stretch of data.
 
 The data from which these events were generated contain a simulated
 gravitational-wave signal, or hardware injection, used to validate
 the performance of the LIGO detectors and downstream data analysis procedures.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.table'
+__currentmodule__ = 'pydischarge.table'
 
 # First, we import the `EventTable` object and read in a set of events from
 # a LIGO_LW-format XML file containing a
 # :class:`sngl_burst <ligo.lw.lsctables.SnglBurstTable>` table
-from pdpy.table import EventTable
+from pydischarge.table import EventTable
 events = EventTable.read('H1-LDAS_STRAIN-968654552-10.xml.gz',
                          tablename='sngl_burst', columns=['peak', 'snr'])
 
 # .. note::
 #
 #    Here we manually specify the `columns` to read in order to optimise
 #    the `read()` operation to parse only the data we actually need.
 
 # We can calculate the rate of events (in Hertz) using the
 # :meth:`~EventTable.event_rate` method:
 rate = events.event_rate(1, start=968654552, end=968654562)
 
 # The :meth:`~EventTable.event_rate` method has returned a
-# `~pdpy.timeseries.TimeSeries`, so we can display this using the
-# :meth:`~pdpy.timeseries.TimeSeries.step` method of that object:
+# `~pydischarge.timeseries.TimeSeries`, so we can display this using the
+# :meth:`~pydischarge.timeseries.TimeSeries.step` method of that object:
 plot = rate.step()
 ax = plot.gca()
 ax.set_xlim(968654552, 968654562)
 ax.set_ylabel('Event rate [Hz]')
 ax.set_title('LIGO Hanford Observatory event rate for HW100916')
 plot.show()
```

### Comparing `pydischarge-0.0.1/examples/table/rate_binned.py` & `pydischarge-0.0.2/examples/table/rate_binned.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Plotting `EventTable` rate versus time for specific column bins
 
 I would like to study the rate at which event triggers are generated by the
 `ExcessPower` gravitational-wave burst detection algorithm, over a small
 stretch of data, binned by various thresholds on signal-to-noise ratio (SNR).
 
 The data from which these events were generated contain a simulated
 gravitational-wave signal, or hardware injection, used to validate
 the performance of the LIGO detectors and downstream data analysis procedures.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.table'
+__currentmodule__ = 'pydischarge.table'
 
 # First, we import the `EventTable` object and read in a set of events from
 # a LIGO_LW-format XML file containing a
 # :class:`sngl_burst <ligo.lw.lsctables.SnglBurstTable>` table
-from pdpy.table import EventTable
+from pydischarge.table import EventTable
 events = EventTable.read('H1-LDAS_STRAIN-968654552-10.xml.gz',
                          tablename='sngl_burst', columns=['peak', 'snr'])
 
 # .. note::
 #
 #    Here we manually specify the `columns` to read in order to optimise
 #    the `read()` operation to parse only the data we actually need.
```

### Comparing `pydischarge-0.0.1/examples/table/scatter.py` & `pydischarge-0.0.2/examples/table/scatter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Plotting an `EventTable` in a scatter
 
-We can use PDpy's `EventTable` to download the catalogue of gravitational-wave
+We can use pyDischarge's `EventTable` to download the catalogue of gravitational-wave
 detections, and create a scatter plot to investigate the mass distribution
 of events.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.table'
+__currentmodule__ = 'pydischarge.table'
 
 # First, we can download the ``'GWTC-1-confident'`` catalogue using
 # :meth:`EventTable.fetch_open_data`:
 
-from pdpy.table import EventTable
+from pydischarge.table import EventTable
 events = EventTable.fetch_open_data(
     "GWTC-1-confident",
     columns=(
         "mass_1_source",
         "mass_2_source",
         "chirp_mass_source",
         "luminosity_distance"
```

### Comparing `pydischarge-0.0.1/examples/table/tiles.py` & `pydischarge-0.0.2/examples/table/tiles.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Plotting an `EventTable` as 2-d tiles
 
 I would like to study the event triggers generated by the `ExcessPower <link>`_
 gravitational-wave burst detection algorithm, over a small stretch of data.
 
 The data from which these events were generated contain a simulated
 gravitational-wave signal, or hardware injection, used to validate
 the performance of the LIGO detectors and downstream data analysis procedures.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.table'
+__currentmodule__ = 'pydischarge.table'
 
 # First, we import the `EventTable` object and read in a set of events from
 # a LIGO_LW-format XML file containing a
 # :class:`sngl_burst <ligo.lw.lsctables.SnglBurstTable>` table
-from pdpy.table import EventTable
+from pydischarge.table import EventTable
 events = EventTable.read(
     'H1-LDAS_STRAIN-968654552-10.xml.gz', tablename='sngl_burst',
     columns=['peak', 'central_freq', 'bandwidth', 'duration', 'snr'])
 
 # .. note::
 #
 #    Here we manually specify the `columns` to read in order to optimise
```

### Comparing `pydischarge-0.0.1/examples/test_examples.py` & `pydischarge-0.0.2/examples/test_examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2019-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Test suite for all examples
 """
 
 import os
 import re
 import warnings
@@ -26,16 +26,16 @@
 from functools import wraps
 from pathlib import Path
 
 import pytest
 
 from matplotlib import use
 
-from pdpy.io.nds2 import NDSWarning
-from pdpy.testing.errors import pytest_skip_network_error
+from pydischarge.io.nds2 import NDSWarning
+from pydischarge.testing.errors import pytest_skip_network_error
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
 
 use('agg')  # force non-interactive backend
 
 # find all examples
 EXAMPLE_BASE = Path(__file__).parent
@@ -107,15 +107,15 @@
     """
     @wraps(func)
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)  # run the test
         except ImportError as exc:  # pragma: no-cover
             # needs an optional dependency
-            if "pdpy" in str(exc):
+            if "pydischarge" in str(exc):
                 raise
             pytest.skip(str(exc))
 
     return wrapper
 
 
 # -- test -------------------
```

### Comparing `pydischarge-0.0.1/examples/timeseries/blrms.py` & `pydischarge-0.0.2/examples/timeseries/blrms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Comparing seismic trends between LIGO sites
 
 On Jan 16 2020 there was a series of earthquakes, that
 should have had an impact on LIGO operations, I'd like to find out.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 # First: we import the objects we need, one for getting the data:
-from pdpy.timeseries import TimeSeriesDict
+from pydischarge.timeseries import TimeSeriesDict
 # and one for plotting the data:
-from pdpy.plot import Plot
+from pydischarge.plot import Plot
 
 # Next we define the channels we want, namely the 0.03Hz-1Hz ground motion
 # band-limited RMS channels (1-second average trends).
 # We do this using string-replacement so we can substitute the interferometer
 # prefix easily when we need to:
 channels = [
     '{ifo}:ISI-GND_STS_ITMY_Z_BLRMS_30M_100M',
@@ -44,15 +44,15 @@
 lho = TimeSeriesDict.get([c.format(ifo='H1') for c in channels],
                          'Jan 16 2020 8:00', 'Jan 16 2020 14:00',
                          host='losc-nds.ligo.org')
 llo = TimeSeriesDict.get([c.format(ifo='L1') for c in channels],
                          'Jan 16 2020 8:00', 'Jan 16 2020 14:00',
                          host='losc-nds.ligo.org')
 
-# Next we can plot the data, with a separate `~pdpy.plot.Axes` for each
+# Next we can plot the data, with a separate `~pydischarge.plot.Axes` for each
 # instrument:
 plot = Plot(lho, llo, figsize=(12, 6), sharex=True, yscale='log')
 ax1, ax2 = plot.axes
 for ifo, ax in zip(('Hanford', 'Livingston'), (ax1, ax2)):
     ax.legend(['ground motion in the Z-direction'])
     ax.text(1.01, 0.5, ifo, ha='left', va='center', transform=ax.transAxes,
             fontsize=18)
```

### Comparing `pydischarge-0.0.1/examples/timeseries/correlate.py` & `pydischarge-0.0.2/examples/timeseries/correlate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Alex Urban (2019-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Cross-correlating two `TimeSeries`
 
 .. warning::
 
    This example requires LIGO.ORG credentials for data access.
 
@@ -37,18 +37,18 @@
 We demonstrate below a prominent 'whistle glitch' in the gravitational wave
 channel, which is also witnessed by a photodiode in the Pre-Stabilized Laser
 (PSL) chamber. This example uses data from the LIGO Livingston detector during
 Advanced LIGO's second observing run.
 """
 
 __author__ = "Alex Urban <alexander.urban@ligo.org>"
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 # First, we import the `TimeSeries` and :meth:`~TimeSeries.get` the data:
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 hoft = TimeSeries.get('L1:GDS-CALIB_STRAIN', 1172489751, 1172489815)
 aux = TimeSeries.get('L1:PSL-ISS_PDA_REL_OUT_DQ', 1172489751, 1172489815)
 
 # Next, we should `~TimeSeries.whiten` the data to enhance the higher-frequency
 # content and make a more faithful comparison between data streams.
 whoft = hoft.whiten(8, 4)
 waux = aux.whiten(8, 4)
```

### Comparing `pydischarge-0.0.1/examples/timeseries/filter.py` & `pydischarge-0.0.2/examples/timeseries/filter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Filtering a `TimeSeries` with a ZPK filter
 
 Several data streams read from the LIGO detectors are whitened before being
 recorded to prevent numerical errors when using single-precision data
 storage.
-In this example we read such `channel <pdpy.detector.Channel>` and undo the
+In this example we read such `channel <pydischarge.detector.Channel>` and undo the
 whitening to show the physical content of these data.
 
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 # First, we import the `TimeSeries` and :meth:`~TimeSeries.get` the data:
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 white = TimeSeries.get(
     'L1:OAF-CAL_DARM_DQ', 'March 2 2015 12:00', 'March 2 2015 12:30')
 
 # Now, we can re-calibrate these data into displacement units by first applying
 # a `highpass <TimeSeries.highpass>` filter to remove the low-frequency noise,
 # and then applying our de-whitening filter in `ZPK <TimeSeries.zpk>` format
 # with five zeros at 100 Hz and five poles at 1 Hz (giving an overall DC
 # gain of 10 :sup:`-10`:
 hp = white.highpass(4)
 displacement = hp.zpk([100]*5, [1]*5, 1e-10)
 
 # We can visualise the impact of the whitening by calculating the ASD
-# `~pdpy.frequencyseries.FrequencySeries` before and after the filter,
+# `~pydischarge.frequencyseries.FrequencySeries` before and after the filter,
 
 whiteasd = white.asd(8, 4)
 dispasd = displacement.asd(8, 4)
 
 # and plotting:
 
-from pdpy.plot import Plot
+from pydischarge.plot import Plot
 plot = Plot(whiteasd, dispasd, separate=True, sharex=True,
             xscale='log', yscale='log')
 
 # Here we have passed the two
-# `spectra <pdpy.frequencyseries.FrequencySeries>` in order,
+# `spectra <pydischarge.frequencyseries.FrequencySeries>` in order,
 # then `separate=True` to display them on separate Axes, `sharex=True` to tie
-# the `~matplotlib.axis.XAxis` of each of the `~pdpy.plot.Axes`
+# the `~matplotlib.axis.XAxis` of each of the `~pydischarge.plot.Axes`
 # together.
 #
 # Finally, we prettify our plot with some limits, and some labels:
 plot.text(0.95, 0.05, 'Preliminary', fontsize=40, color='gray',  # hide
           ha='right', rotation=45, va='bottom', alpha=0.5)  # hide
 plot.axes[0].set_ylabel('ASD [whitened]')
 plot.axes[1].set_ylabel(r'ASD [m/$\sqrt{\mathrm{Hz}}$]')
```

### Comparing `pydischarge-0.0.1/examples/timeseries/inject.py` & `pydischarge-0.0.2/examples/timeseries/inject.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Alex Urban (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Inject a known signal into a `TimeSeries`
 
 It can often be useful to add some known signal to an inherently random
 or noisy timeseries. For example, one might want to examine what
 would happen if a binary black hole merger signal occured at or near
 the time of a glitch. In LIGO data analysis, this procedure is referred
 to as an _injection_.
 
 In the example below, we will create a stream of random, white Gaussian
 noise, then inject a simulation of GW150914 into it at a known time.
 """
 
 __author__ = "Alex Urban <alexander.urban@ligo.org>"
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 # First, we prepare one second of Gaussian noise:
 
 from numpy import random
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 noise = TimeSeries(random.normal(scale=.1, size=16384), sample_rate=16384)
 
 # Then we can download a simulation of the GW150914 signal from GWOSC:
 
 from astropy.utils.data import get_readable_fileobj
 url = ("https://gwosc.org/s/events/GW150914/P150914/"
        "fig2-unfiltered-waveform-H.txt")
 with get_readable_fileobj(url) as f:
     signal = TimeSeries.read(f, format='txt')
 signal.t0 = .5  # make sure this intersects with noise time samples
 
 # Note, since this simulation cuts off before a certain time, it is
 # important to taper its ends to zero to avoid ringing artifacts.
 # We can accomplish this using the
-# :meth:`~pdpy.timeseries.TimeSeries.taper` method.
+# :meth:`~pydischarge.timeseries.TimeSeries.taper` method.
 
 signal = signal.taper()
 
 # Since the time samples overlap, we can inject this into our noise data
-# using :meth:`~pdpy.types.series.Series.inject`:
+# using :meth:`~pydischarge.types.series.Series.inject`:
 
 data = noise.inject(signal)
 
 # Finally, we can visualize the full process in the time domain:
 
-from pdpy.plot import Plot
+from pydischarge.plot import Plot
 plot = Plot(noise, signal, data, separate=True, sharex=True, sharey=True)
 plot.gca().set_epoch(0)
 plot.show()
 
 # We can clearly see that the loud GW150914-like signal has been layered
 # on top of Gaussian noise with the correct amplitude and phase evolution.
```

### Comparing `pydischarge-0.0.1/examples/timeseries/public.py` & `pydischarge-0.0.2/examples/timeseries/public.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Accessing and visualising public GW detector data
 
 Data from the current generation gravitational wave detectors are published
 by |GWOSCl| and freely available to the public.
 In this example we demonstrate how to identify times of a published
 GW detection event, and to download and visualise detector data.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = "pdpy.timeseries"
+__currentmodule__ = "pydischarge.timeseries"
 
 # Firstly, we can use the |gwosc-mod| Python package to query for the
 # time of the first gravitational-wave detection |GW150914|:
 
 from gwosc.datasets import event_gps
 gps = event_gps("GW150914")
 
-# PDpy's `TimeSeries` class provides an interface to the public |GWOSC|
+# pyDischarge's `TimeSeries` class provides an interface to the public |GWOSC|
 # data in the :meth:`~TimeSeries.fetch_open_data` method; to use it we
 # need to first import the `TimeSeries` object:
 
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 
 # then call the :meth:`~TimeSeries.fetch_open_data` method, passing it the
 # prefix for the interferometer we want (`'L1'` here for LIGO-Livingston),
 # and the GPS start and stop times of our query (based around the GPS time
 # for GW150914):
 
 data = TimeSeries.fetch_open_data('L1', gps-5, gps+5)
 
 # and then we can make a plot:
 
 plot = data.plot(
     title="LIGO Livingston Observatory data for GW150914",
     ylabel="Strain amplitude",
-    color="pdpy:ligo-livingston",
+    color="pydischarge:ligo-livingston",
     epoch=gps,
 )
 plot.show()
 
 # We can't see anything that looks like a gravitational wave signal in these
 # data, the amplitude is dominated by low-frequency detector noise.
 # Further filtering is required to be able to identify the GW150914 event
-# here, see :ref:`pdpy-example-signal-gw150914` for a more in-depth example of
+# here, see :ref:`pydischarge-example-signal-gw150914` for a more in-depth example of
 # extracting signals from noise.
```

### Comparing `pydischarge-0.0.1/examples/timeseries/pycbc-snr.py` & `pydischarge-0.0.2/examples/timeseries/pycbc-snr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Calculating the SNR associated with a given astrophysical signal model
 
-The example :ref:`pdpy-example-signal-gw150914` showed us we can visually
+The example :ref:`pydischarge-example-signal-gw150914` showed us we can visually
 extract a signal from the noise using basic signal-processing techniques.
 
 However, an actual astrophysical search algorithm detects signals by
 calculating the signal-to-noise ratio (SNR) of data for each in a large bank
 of signal models, known as templates.
 
 Using |pycbc|_ (the actual search code), we can do that.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 # First, as always, we fetch some of the public data from the LIGO Open
 # Science Center:
 
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 data = TimeSeries.fetch_open_data('H1', 1126259446, 1126259478)
 
 # and condition it by applying a highpass filter at 15 Hz
 high = data.highpass(15)
 
 # This is important to remove noise at lower frequencies that isn't
 # accurately calibrated, and swamps smaller noises at higher frequencies.
@@ -71,18 +71,18 @@
 snr = matched_filter(hp, zoom.to_pycbc(), psd=psd.to_pycbc(),
                      low_frequency_cutoff=15)
 snrts = TimeSeries.from_pycbc(snr).abs()
 
 # .. note::
 #
 #    Here we have used the :meth:`~TimeSeries.to_pycbc` methods of the
-#    `~pdpy.timeseries.TimeSeries` and `~pdpy.frequencyseries.FrequencySeries`
-#    objects to convert from PDpy objects to something that PyCBC functions
+#    `~pydischarge.timeseries.TimeSeries` and `~pydischarge.frequencyseries.FrequencySeries`
+#    objects to convert from pyDischarge objects to something that PyCBC functions
 #    can understand, and then used the :meth:`~TimeSeries.from_pycbc` method
-#    to convert back to a PDpy object.
+#    to convert back to a pyDischarge object.
 
 # We can plot the SNR `TimeSeries` around the region of interest:
 plot = snrts.plot()
 ax = plot.gca()
 ax.set_xlim(1126259461, 1126259463)
 ax.set_epoch(1126259462.427)
 ax.set_ylabel('Signal-to-noise ratio (SNR)')
```

### Comparing `pydischarge-0.0.1/examples/timeseries/qscan.py` & `pydischarge-0.0.2/examples/timeseries/qscan.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Generate the Q-transform of a `TimeSeries`
 
 One of the most useful tools for filtering and visualising short-duration
 features in a `TimeSeries` is the
 `Q-transform <https://en.wikipedia.org/wiki/Constant-Q_transform>`_.
 This is regularly used by the Detector Characterization working groups of
@@ -29,31 +29,31 @@
 
 This algorithm was used to visualise the first ever gravitational-wave
 detection GW150914, so we can reproduce `that result (bottom panel of figure 1)
 <https://doi.org/10.1103/PhysRevLett.116.061102>`_ here.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 # First, we need to download the `TimeSeries` record for the H1 strain
 # measurement from |GWOSC|_:
 
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 data = TimeSeries.fetch_open_data('H1', 1126259446, 1126259478)
 
 # Next, we generate the `~TimeSeries.q_transform` of these data:
 qspecgram = data.q_transform(outseg=(1126259462.2, 1126259462.5))
 
 # .. note::
 #    We can save memory by focusing on a specific window around the
 #    interesting time. The ``outseg`` keyword argument returns a `Spectrogram`
 #    that is only as long as we need it to be.
 
-# Now, we can plot the resulting `~pdpy.spectrogram.Spectrogram`:
+# Now, we can plot the resulting `~pydischarge.spectrogram.Spectrogram`:
 
 plot = qspecgram.plot(figsize=[8, 4])
 ax = plot.gca()
 ax.set_xscale('seconds')
 ax.set_yscale('log')
 ax.set_ylim(20, 500)
 ax.set_ylabel('Frequency [Hz]')
```

### Comparing `pydischarge-0.0.1/examples/timeseries/statevector.py` & `pydischarge-0.0.2/examples/timeseries/statevector.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Plotting segments for a `StateVector`
 
 Confident detection of gravitational-wave signals is critically dependent
 on understanding the quality of the data searched.
 Alongside the strain *h(t)* data, |GWOSC|_ also
-releases a *Data Quality* :ref:`state vector <pdpy-statevector>`.
+releases a *Data Quality* :ref:`state vector <pydischarge-statevector>`.
 We can use this to check on the quality of the data from the LIGO Livingston
 detector around |GW170817|_.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = "pdpy.timeseries"
+__currentmodule__ = "pydischarge.timeseries"
 
 # First, we can import the `StateVector` class:
-from pdpy.timeseries import StateVector
+from pydischarge.timeseries import StateVector
 
 # and download the state information surrounding GW170817:
 data = StateVector.fetch_open_data(
     "L1",
     1187008882 - 100,
     1187008882 + 100,
     verbose=True,
```

### Comparing `pydischarge-0.0.1/examples/timeseries/whiten.py` & `pydischarge-0.0.2/examples/timeseries/whiten.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Whitening a `TimeSeries`
 
 .. warning::
 
    This example requires LIGO.ORG credentials for data access.
 
@@ -33,26 +33,26 @@
 
 We demonstrate below with an auxiliary signal recording transmitted power
 in one of the interferometer arms, which recorded two large glitches with
 a frequency of around 5-50Hz.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__currentmodule__ = 'pdpy.timeseries'
+__currentmodule__ = 'pydischarge.timeseries'
 
 # First, we import the `TimeSeries` and :meth:`~TimeSeries.get` the data:
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 data = TimeSeries.get('H1:ASC-Y_TR_A_NSUM_OUT_DQ', 1123084671, 1123084703)
 
 # Now, we can `~TimeSeries.whiten` the data to enhance the higher-frequency
 # content
 white = data.whiten(4, 2)
 
 # and can `~TimeSeries.plot` both the original and whitened data
-from pdpy.plot import Plot
+from pydischarge.plot import Plot
 plot = Plot(data, white, separate=True, sharex=True)
 plot.axes[0].set_ylabel('Y-arm power [counts]', fontsize=16)
 plot.axes[1].set_ylabel('Whitened amplitude', fontsize=16)
 plot.show()
 
 # Here we see two large spikes that are completely undetected in the raw
 # `TimeSeries`, but are very obvious in the whitened data. We can also see
```

### Comparing `pydischarge-0.0.1/pdpy/__init__.py` & `pydischarge-0.0.2/pydischarge/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """A python package for gravitational-wave astrophysics
 
-PDpy is a collaboration-driven `Python <http://www.python.org>`_ package
+pyDischarge is a collaboration-driven `Python <http://www.python.org>`_ package
 providing tools for studying data from ground-based gravitational-wave
 detectors.
 
-PDpy provides a user-friendly, intuitive interface to the common time-domain
+pyDischarge provides a user-friendly, intuitive interface to the common time-domain
 and frequency-domain data produced by the `LIGO <http://www.ligo.org>`_ and
 `Virgo <http://www.ego-gw.it>`_ instruments and their analysis,
 with easy-to-follow tutorials at each step.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
 __credits__ = "The LIGO Scientific Collaboration and the Virgo Collaboration"
 
 from . import (
-    plot,  # registers pdpy.plot.Axes as default rectilinear axes
+    plot,  # registers pydischarge.plot.Axes as default rectilinear axes
 )
 
 try:
     from ._version import version as __version__
 except ModuleNotFoundError:  # development mode
     __version__ = ''
```

### Comparing `pydischarge-0.0.1/pdpy/astro/range.py` & `pydischarge-0.0.2/pydischarge/astro/range.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module provides methods to calculate the astrophysical sensitive
 distance of an instrumental power-spectral density.
 """
 
 import warnings
 
@@ -66,33 +66,33 @@
 
 
 def _get_spectrogram(hoft, **kwargs):
     """Check that the input is a spectrogram, or compute one if compatible
 
     Parameters
     ----------
-    hoft : `~pdpy.timeseries.TimeSeries` or `~pdpy.spectrogram.Spectrogram`
+    hoft : `~pydischarge.timeseries.TimeSeries` or `~pydischarge.spectrogram.Spectrogram`
         record of gravitational-wave strain output from a detector
 
     **kwargs : `dict`, optional
         additional keyword arguments to
-        `~pdpy.timeseries.TimeSeries.spectrogram`
+        `~pydischarge.timeseries.TimeSeries.spectrogram`
 
     Returns
     -------
-    hoft : `~pdpy.spectrogram.Spectrogram`
+    hoft : `~pydischarge.spectrogram.Spectrogram`
         a time-frequency `Spectrogram` of the input
     """
     if not isinstance(hoft, Spectrogram):
         try:
             hoft = hoft.spectrogram(**kwargs)
         except (AttributeError, TypeError):
             msg = ('Could not produce a spectrogram from the input, please '
-                   'pass an instance of pdpy.timeseries.TimeSeries or '
-                   'pdpy.spectrogram.Spectrogram')
+                   'pass an instance of pydischarge.timeseries.TimeSeries or '
+                   'pydischarge.spectrogram.Spectrogram')
             raise TypeError(msg)
     return hoft
 
 
 def _preformat_psd(func):
     @wraps(func)
     def decorated_func(psd, *args, **kwargs):
@@ -113,15 +113,15 @@
     which a compact binary inspiral with the given component masses would
     be detectable given the instrumental PSD. The calculation is defined in:
 
     https://dcc.ligo.org/LIGO-T030276/public
 
     Parameters
     ----------
-    psd : `~pdpy.frequencyseries.FrequencySeries`
+    psd : `~pydischarge.frequencyseries.FrequencySeries`
         the instrumental power-spectral-density data
 
     snr : `float`, optional
         the signal-to-noise ratio for which to calculate range,
         default: `8`
 
     mass1 : `float`, `~astropy.units.Quantity`, optional
@@ -134,15 +134,15 @@
 
     horizon : `bool`, optional
         if `True`, return the maximal 'horizon' sensitive distance, otherwise
         return the angle-averaged range, default: `False`
 
     Returns
     -------
-    rspec : `~pdpy.frequencyseries.FrequencySeries`
+    rspec : `~pydischarge.frequencyseries.FrequencySeries`
         the calculated inspiral sensitivity PSD [Mpc^2 / Hz]
     """
     frange = (psd.frequencies > 0)
     # compute total mass and chirp mass
     mass1 = units.Quantity(mass1, 'solMass').to('kg')
     mass2 = units.Quantity(mass2, 'solMass').to('kg')
     mtotal = mass1 + mass2
@@ -174,15 +174,15 @@
     binary inspiral with the given component masses would be detectable
     given the instrumental PSD. The calculation is as defined in:
 
     https://dcc.ligo.org/LIGO-T030276/public
 
     Parameters
     ----------
-    psd : `~pdpy.frequencyseries.FrequencySeries`
+    psd : `~pydischarge.frequencyseries.FrequencySeries`
         the instrumental power-spectral-density data
 
     snr : `float`, optional
         the signal-to-noise ratio for which to calculate range,
         default: `8`
 
     mass1 : `float`, `~astropy.units.Quantity`, optional
@@ -209,21 +209,21 @@
     range : `~astropy.units.Quantity`
         the calculated inspiral range [Mpc]
 
     Examples
     --------
     Grab some data for LIGO-Livingston around GW150914 and generate a PSD:
 
-    >>> from pdpy.timeseries import TimeSeries
+    >>> from pydischarge.timeseries import TimeSeries
     >>> hoft = TimeSeries.fetch_open_data('H1', 1126259446, 1126259478)
     >>> hoff = hoft.psd(fftlength=4)
 
     Now we can calculate the :func:`sensemon_range`:
 
-    >>> from pdpy.astro import sensemon_range
+    >>> from pydischarge.astro import sensemon_range
     >>> r = sensemon_range(hoff, fmin=30)
     >>> print(r)
     70.4612102889 Mpc
     """
     fisco = _get_isco_frequency(mass1, mass2)
     # format frequency limits
     fmin = units.Quantity(fmin or psd.df, 'Hz')  # avoid DC value
@@ -249,19 +249,19 @@
     try:
         from inspiral_range import (
             range,
             find_root_redshift,
         )
     except ModuleNotFoundError as exc:  # no inspiral-range package
         exc.msg = str(exc) + (
-            "; pdpy.astro's inspiral_range and inspiral_range_psd functions "
+            "; pydischarge.astro's inspiral_range and inspiral_range_psd functions "
             "require the extra package 'inspiral-range' to provide "
             "cosmologically-corrected distance calculations, please install "
-            "that package and try again, or install pdpy with the 'astro' "
-            "extra via `python -m pip install pdpy[astro]`"
+            "that package and try again, or install pydischarge with the 'astro' "
+            "extra via `python -m pip install pydischarge[astro]`"
         )
         raise
 
     from inspiral_range.waveform import CBCWaveform
 
     return (
         range,
@@ -280,15 +280,15 @@
     be detectable given the instrumental PSD. The calculation is defined in
     Belczynski et. al (2014):
 
     https://dx.doi.org/10.1088/0004-637x/789/2/120
 
     Parameters
     ----------
-    psd : `~pdpy.frequencyseries.FrequencySeries`
+    psd : `~pydischarge.frequencyseries.FrequencySeries`
         the instrumental power-spectral-density data
 
     snr : `float`, optional
         the signal-to-noise ratio for which to calculate range,
         default: `8`
 
     mass1 : `float`, `~astropy.units.Quantity`, optional
@@ -304,15 +304,15 @@
         return the angle-averaged comoving distance, default: `False`
 
     **kwargs : `dict`, optional
         additional keyword arguments to `~inspiral_range.waveform.CBCWaveform`
 
     Returns
     -------
-    rspec : `~pdpy.frequencyseries.FrequencySeries`
+    rspec : `~pydischarge.frequencyseries.FrequencySeries`
         the calculated inspiral sensitivity PSD [Mpc^2 / Hz]
 
     See also
     --------
     sensemon_range_psd
         for the method based on LIGO-T030276, also known as LIGO SenseMonitor
     inspiral-range
@@ -355,15 +355,15 @@
     given the instrumental PSD. The calculation is defined in Belczynski
     et. al (2014):
 
     https://dx.doi.org/10.1088/0004-637x/789/2/120
 
     Parameters
     ----------
-    psd : `~pdpy.frequencyseries.FrequencySeries`
+    psd : `~pydischarge.frequencyseries.FrequencySeries`
         the instrumental power-spectral-density data
 
     snr : `float`, optional
         the signal-to-noise ratio for which to calculate range,
         default: `8`
 
     mass1 : `float`, `~astropy.units.Quantity`, optional
@@ -393,21 +393,21 @@
     range : `~astropy.units.Quantity`
         the calculated inspiral range [Mpc]
 
     Examples
     --------
     Grab some data for LIGO-Livingston around GW150914 and generate a PSD:
 
-    >>> from pdpy.timeseries import TimeSeries
+    >>> from pydischarge.timeseries import TimeSeries
     >>> hoft = TimeSeries.fetch_open_data('H1', 1126259446, 1126259478)
     >>> hoff = hoft.psd(fftlength=4)
 
     Now, we can calculate the :func:`inspiral_range`:
 
-    >>> from pdpy.astro import inspiral_range
+    >>> from pydischarge.astro import inspiral_range
     >>> r = inspiral_range(hoff, fmin=30)
     >>> print(r)
     70.4612102889 Mpc
 
     See also
     --------
     sensemon_range
@@ -445,28 +445,28 @@
 
 @_preformat_psd
 def burst_range_spectrum(psd, snr=8, energy=1e-2):
     """Calculate the frequency-dependent GW burst range from a strain PSD
 
     Parameters
     ----------
-    psd : `~pdpy.frequencyseries.FrequencySeries`
+    psd : `~pydischarge.frequencyseries.FrequencySeries`
         the instrumental power-spectral-density data
 
     snr : `float`, optional
         the signal-to-noise ratio for which to calculate range,
         default: `8`
 
     energy : `float`, optional
         the relative energy output of the GW burst,
         default: `0.01` (GRB-like burst)
 
     Returns
     -------
-    rangespec : `~pdpy.frequencyseries.FrequencySeries`
+    rangespec : `~pydischarge.frequencyseries.FrequencySeries`
         the burst range `FrequencySeries` [Mpc (default)]
     """
     frange = (psd.frequencies > 0)
     # calculate frequency dependent range in parsecs
     a = (
         constants.G * energy * constants.M_sun * 0.4
         / (pi**2 * constants.c)
@@ -477,15 +477,15 @@
 
 
 def burst_range(psd, snr=8, energy=1e-2, fmin=100, fmax=500):
     """Calculate the integrated GRB-like GW burst range from a strain PSD
 
     Parameters
     ----------
-    psd : `~pdpy.frequencyseries.FrequencySeries`
+    psd : `~pydischarge.frequencyseries.FrequencySeries`
         the instrumental power-spectral-density data
 
     snr : `float`, optional
         the signal-to-noise ratio for which to calculate range,
         default: ``8``
 
     energy : `float`, optional
@@ -505,21 +505,21 @@
     range : `~astropy.units.Quantity`
         the GRB-like-burst sensitive range [Mpc (default)]
 
     Examples
     --------
     Grab some data for LIGO-Livingston around GW150914 and generate a PSD
 
-    >>> from pdpy.timeseries import TimeSeries
+    >>> from pydischarge.timeseries import TimeSeries
     >>> hoft = TimeSeries.fetch_open_data('H1', 1126259446, 1126259478)
     >>> hoff = hoft.psd(fftlength=4)
 
     Now we can calculate the :func:`burst_range`:
 
-    >>> from pdpy.astro import burst_range
+    >>> from pydischarge.astro import burst_range
     >>> r = burst_range(hoff, fmin=30)
     >>> print(r)
     42.5055584195 Mpc
     """
     f = psd.frequencies.to('Hz').value
     # restrict integral
     fmin = fmin or psd.df.to('Hz').value
@@ -550,15 +550,15 @@
     **rangekwargs,
 ):
     """Measure timeseries trends of astrophysical detector range (Mpc)
     directly from strain
 
     Parameters
     ----------
-    hoft : `~pdpy.timeseries.TimeSeries` or `~pdpy.spectrogram.Spectrogram`
+    hoft : `~pydischarge.timeseries.TimeSeries` or `~pydischarge.spectrogram.Spectrogram`
         record of gravitational-wave strain output from a detector
 
     stride : `float`, optional
         desired step size (seconds) of range timeseries, required if
         `hoft` is an instance of `TimeSeries`
 
     fftlength : `float`, optional
@@ -571,15 +571,15 @@
     window : `str`, `numpy.ndarray`, optional
         window function to apply to timeseries prior to FFT, see
         :func:`scipy.signal.get_window` for details on acceptable
         formats
 
     method : `str`, optional
         FFT-averaging method, defaults to median averaging, see
-        :meth:`~pdpy.timeseries.TimeSeries.spectrogram` for
+        :meth:`~pydischarge.timeseries.TimeSeries.spectrogram` for
         more details
 
     nproc : `int`, optional
         number of CPUs to use in parallel processing of FFTs, default: 1
 
     range_func : `callable`, optional
         the function to call to generate the range for each stride,
@@ -589,34 +589,34 @@
     **rangekwargs : `dict`, optional
         additional keyword arguments to :func:`burst_range` or
         :func:`inspiral_range` (see "Notes" below), defaults to
         inspiral range with `mass1 = mass2 = 1.4` solar masses
 
     Returns
     -------
-    out : `~pdpy.timeseries.TimeSeries`
+    out : `~pydischarge.timeseries.TimeSeries`
         timeseries trends of astrophysical range
 
     Notes
     -----
     This method is designed to quantify a gravitational-wave detector's
     sensitive range as a function of time. It supports the range to
     compact binary inspirals and to unmodelled GW bursts, each a class
     of transient event.
 
     See also
     --------
-    pdpy.timeseries.TimeSeries.spectrogram
+    pydischarge.timeseries.TimeSeries.spectrogram
         for the underlying power spectral density estimator
     inspiral_range
         for the function that computes inspiral range
     burst_range
         for the function that computes burst range
     range_spectrogram
-        for a `~pdpy.spectrogram.Spectrogram` of the range integrand
+        for a `~pydischarge.spectrogram.Spectrogram` of the range integrand
     """
     rangekwargs = rangekwargs or {'mass1': 1.4, 'mass2': 1.4}
     if range_func is None and "energy" in rangekwargs:
         range_func = burst_range
     elif range_func is None:
         range_func = inspiral_range
     hoft = _get_spectrogram(
@@ -644,15 +644,15 @@
     **rangekwargs,
 ):
     """Calculate the average range or range power spectrogram (Mpc or
     Mpc^2 / Hz) directly from strain
 
     Parameters
     ----------
-    hoft : `~pdpy.timeseries.TimeSeries`  or `~pdpy.spectrogram.Spectrogram`
+    hoft : `~pydischarge.timeseries.TimeSeries`  or `~pydischarge.spectrogram.Spectrogram`
         record of gravitational-wave strain output from a detector
 
     stride : `float`, optional
         number of seconds in a single PSD (i.e., step size of spectrogram),
         required if `hoft` is an instance of `TimeSeries`
 
     fftlength : `float`, optional
@@ -665,15 +665,15 @@
     window : `str`, `numpy.ndarray`, optional
         window function to apply to timeseries prior to FFT, see
         :func:`scipy.signal.get_window` for details on acceptable
         formats
 
     method : `str`, optional
         FFT-averaging method, defaults to median averaging, see
-        :meth:`~pdpy.timeseries.TimeSeries.spectrogram` for
+        :meth:`~pydischarge.timeseries.TimeSeries.spectrogram` for
         more details
 
     nproc : `int`, optional
         number of CPUs to use in parallel processing of FFTs, default: 1
 
     fmin : `float`, optional
         low frequency cut-off (Hz), defaults to `1/fftlength`
@@ -689,15 +689,15 @@
     **rangekwargs : `dict`, optional
         additional keyword arguments to :func:`burst_range_spectrum` or
         :func:`inspiral_range_psd` (see "Notes" below), defaults to
         inspiral range with `mass1 = mass2 = 1.4` solar masses
 
     Returns
     -------
-    out : `~pdpy.spectrogram.Spectrogram`
+    out : `~pydischarge.spectrogram.Spectrogram`
         time-frequency spectrogram of astrophysical range
 
     Notes
     -----
     This method is designed to show the contribution to a
     gravitational-wave detector's sensitive range across frequency bins
     as a function of time. It supports the range to compact binary
@@ -706,15 +706,15 @@
 
     If inspiral range is requested and `fmax` exceeds the frequency of the
     innermost stable circular orbit (ISCO), the output will extend only up
     to the latter.
 
     See also
     --------
-    pdpy.timeseries.TimeSeries.spectrogram
+    pydischarge.timeseries.TimeSeries.spectrogram
         for the underlying power spectral density estimator
     inspiral_range_psd
         for the function that computes inspiral range integrand
     burst_range_spectrum
         for the function that computes burst range integrand
     range_timeseries
         for `TimeSeries` trends of the astrophysical range
```

### Comparing `pydischarge-0.0.1/pdpy/astro/tests/__init__.py` & `pydischarge-0.0.2/pydischarge/frequencyseries/tests/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.astro`
+"""Tests for :mod:`pydischarge.frequencyseries`
 """
```

### Comparing `pydischarge-0.0.1/pdpy/astro/tests/test_range.py` & `pydischarge-0.0.2/pydischarge/astro/tests/test_range.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.astro.range`
+"""Unit tests for :mod:`pydischarge.astro.range`
 """
 
 from unittest import mock
 
 import pytest
 
 from astropy import units
@@ -60,29 +60,29 @@
         window=('kaiser', 24),
     )
 
 
 # -- sensemon -----------------------------------
 
 def test_sensemon_range_psd(psd):
-    """Test for :func:`pdpy.astro.sensemon_range_psd`
+    """Test for :func:`pydischarge.astro.sensemon_range_psd`
     """
     fisco = astro.range._get_isco_frequency(1.4, 1.4).value
     frange = (psd.frequencies.value < fisco)
     r = astro.sensemon_range_psd(psd[frange])
     assert isinstance(r, FrequencySeries)
     utils.assert_quantity_almost_equal(
         trapz(r, r.frequencies) ** (1/2.),
         TEST_RESULTS['sensemon_range'],
     )
     assert r.f0.value > 0
 
 
 def test_sensemon_range(psd):
-    """Test for :func:`pdpy.astro.sensemon_range`
+    """Test for :func:`pydischarge.astro.sensemon_range`
     """
     r = astro.sensemon_range(psd)
     utils.assert_quantity_almost_equal(r, TEST_RESULTS['sensemon_range'])
 
 
 # -- inspiral-range -----------------------------
 
@@ -94,53 +94,53 @@
         match="extra package 'inspiral-range'",
     ):
         astro.inspiral_range(psd)
 
 
 @pytest.mark.requires("inspiral_range")
 def test_inspiral_range_psd(psd):
-    """Test for :func:`pdpy.astro.inspiral_range_psd`
+    """Test for :func:`pydischarge.astro.inspiral_range_psd`
     """
     frange = (psd.frequencies.value < 4096)
     r = astro.inspiral_range_psd(psd[frange])
     assert isinstance(r, FrequencySeries)
     print(trapz(r, r.frequencies) ** (1/2.))
     utils.assert_quantity_almost_equal(
         trapz(r, r.frequencies) ** (1/2.),
         TEST_RESULTS['inspiral_range'],
     )
     assert r.f0.value > 0
 
 
 @pytest.mark.requires("inspiral_range")
 def test_inspiral_range(psd):
-    """Test for :func:`pdpy.astro.inspiral_range`
+    """Test for :func:`pydischarge.astro.inspiral_range`
     """
     r = astro.inspiral_range(psd)
     utils.assert_quantity_almost_equal(r, TEST_RESULTS['inspiral_range'])
 
 
 # -- burst range --------------------------------
 
 def test_burst_range_spectrum(psd):
-    """Test for :func:`pdpy.astro.burst_range_spectrum`
+    """Test for :func:`pydischarge.astro.burst_range_spectrum`
     """
     f = psd.frequencies
     frange = (f.value >= 100) & (f.value < 500)
     r = astro.burst_range_spectrum(psd[frange])
     assert isinstance(r, FrequencySeries)
     utils.assert_quantity_almost_equal(
         (trapz(r**3, f[frange]) / (400 * units.Hz)) ** (1/3.),
         TEST_RESULTS['burst_range'],
     )
     assert r.f0.value > 0
 
 
 def test_burst_range(psd):
-    """Test for :func:`pdpy.astro.burst_range`
+    """Test for :func:`pydischarge.astro.burst_range`
     """
     r = astro.burst_range(psd)
     utils.assert_quantity_almost_equal(r, TEST_RESULTS['burst_range'])
 
 
 # -- timeseries/spectrogram wrappers ------------
```

### Comparing `pydischarge-0.0.1/pdpy/cli/__init__.py` & `pydischarge-0.0.2/pydischarge/cli/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Command-line utilities for PDpy
+"""Command-line utilities for pyDischarge
 
-The `pdpy.cli` module provides methods and functionality to power the
-`pdpy-plot` command-line executable (distributed with PDpy).
+The `pydischarge.cli` module provides methods and functionality to power the
+`pydischarge-plot` command-line executable (distributed with pyDischarge).
 """
 
 from collections import OrderedDict as _od
 
 from .timeseries import TimeSeries
 from .spectrum import Spectrum
 from .spectrogram import Spectrogram
```

### Comparing `pydischarge-0.0.1/pdpy/cli/cliproduct.py` & `pydischarge-0.0.2/pydischarge/cli/cliproduct.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Joseph Areeda (2015-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Base class for CLI (`pdpy-plot`) products.
+"""Base class for CLI (`pydischarge-plot`) products.
 """
 
 import abc
 import os.path
 import re
 import time
 import sys
@@ -108,15 +108,15 @@
        an `~argparse.ArgumentParser`
     - `CliProduct.run` - executes the arguments to product one or more plots
 
     So, the basic usage is follows::
 
     >>> import argparse
     >>> parser = argparse.ArgumentParser()
-    >>> from pdpy.cli import CliProduct
+    >>> from pydischarge.cli import CliProduct
     >>> CliProduct.init_cli(parser)
     >>> product = CliProduct(parser.parse_args())
     >>> product.run()
 
     The key methods for subclassing are
 
     - `CliProduct.action` - property defines 'name' for command-line subcommand
@@ -392,15 +392,15 @@
         )
         group.add_argument(
             '--suptitle',
             help='topmost title line (larger than the others)',
         )
         group.add_argument(
             '--out',
-            default='pdpy.png',
+            default='pydischarge.png',
             help=(
                 'output filename (extension determines format: '
                 'png, pdf, svg are available)'
             ),
         )
 
         # legends match input files in position are displayed if specified.
@@ -503,15 +503,15 @@
         # pylint: disable=no-self-use
         """Sanity-check and set defaults for arguments
         """
         # this method is called by __init__ (after command-line arguments
         # have been parsed)
 
         if args.out is None:
-            args.out = "pdpy.png"
+            args.out = "pydischarge.png"
 
     def _validate_arguments(self):
         """Sanity check arguments and raise errors if required
         """
         # validate number of data sets requested
         if len(self.chan_list) < self.MIN_CHANNELS:
             raise ValueError(
```

### Comparing `pydischarge-0.0.1/pdpy/cli/coherence.py` & `pydischarge-0.0.2/pydischarge/cli/coherence.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Joseph Areeda (2015-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Coherence plots
 """
 
 from collections import OrderedDict
 
 from ..plot import Plot
```

### Comparing `pydischarge-0.0.1/pdpy/cli/coherencegram.py` & `pydischarge-0.0.2/pydischarge/cli/coherencegram.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Joseph Areeda (2015-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Coherence spectrogram
 """
 
 from .spectrogram import Spectrogram
 
 __author__ = 'Joseph Areeda <joseph.areeda@ligo.org>'
```

### Comparing `pydischarge-0.0.1/pdpy/cli/gwpy_plot.py` & `pydischarge-0.0.2/pydischarge/cli/gwpy_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) Joseph Areeda (2015-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Generate plots of GW observatory data using PDpy
+"""Generate plots of GW observatory data using pyDischarge
 """
 
 import time
 
 import os
 import sys
 from argparse import (
@@ -45,22 +45,22 @@
 PROG_START = time.time()    # verbose enough times major ops
 
 INTERACTIVE = hasattr(sys, 'ps1')
 
 EPILOG = f"""
 Examples:
 
-    $ pdpy-plot timeseries --chan H1:GDS-CALIB_STRAIN --start 1126259457
+    $ pydischarge-plot timeseries --chan H1:GDS-CALIB_STRAIN --start 1126259457
 
-    $ pdpy-plot spectrum --chan H1:GDS-CALIB_STRAIN L1:GDS-CALIB_STRAIN --chan V1:Hrec_hoft_16384Hz --start 1187008866 --duration 32 --xmin 10 --xmax 4000
+    $ pydischarge-plot spectrum --chan H1:GDS-CALIB_STRAIN L1:GDS-CALIB_STRAIN --chan V1:Hrec_hoft_16384Hz --start 1187008866 --duration 32 --xmin 10 --xmax 4000
 
-    $ pdpy-plot coherencegram --chan H1:GDS-CALIB_STRAIN H1:PEM-CS_ACC_PSL_PERISCOPE_X_DQ --start 1126260017 --duration 600
+    $ pydischarge-plot coherencegram --chan H1:GDS-CALIB_STRAIN H1:PEM-CS_ACC_PSL_PERISCOPE_X_DQ --start 1126260017 --duration 600
 
 Written by {__author__}.
-Report bugs to https://github.com/pdpy-github/pdpy/issues/.
+Report bugs to https://github.com/pydischarge-github/pydischarge/issues/.
 """  # noqa: E501
 
 
 # -- init command line --------------------------------------------------------
 
 class HelpFormatter(ArgumentDefaultsHelpFormatter, RawTextHelpFormatter):
     def _format_usage(self, usage, actions, groups, prefix):
@@ -119,15 +119,15 @@
     parser = create_parser()
     return parser.parse_args(args=args)
 
 
 # -- run ----------------------------------------------------------------------
 
 def main(args=None):
-    """Run pdpy-plot
+    """Run pydischarge-plot
 
     Returns the relevant exit code, that can be passed to :func:`sys.exit`.
     """
     # parse the command line and create a product object
     args = parse_command_line(args=args)
     prod = PRODUCTS[args.mode](args)
     prod.log(2, f'{prod.action} created')
```

### Comparing `pydischarge-0.0.1/pdpy/cli/qtransform.py` & `pydischarge-0.0.2/pydischarge/cli/qtransform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Joseph Areeda (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """ Q-transform plots
 """
 
 import os.path
 import re
 import warnings
```

### Comparing `pydischarge-0.0.1/pdpy/cli/spectrogram.py` & `pydischarge-0.0.2/pydischarge/cli/spectrogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Joseph Areeda (2015-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """ Spectrogram plots
 """
 
 from numpy import percentile
 
 from .cliproduct import (FFTMixin, TimeDomainProduct, ImageProduct)
```

### Comparing `pydischarge-0.0.1/pdpy/cli/spectrum.py` & `pydischarge-0.0.2/pydischarge/cli/spectrum.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Joseph Areeda (2015-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Spectrum plots
 """
 
 from astropy.time import Time
 import warnings
```

### Comparing `pydischarge-0.0.1/pdpy/cli/tests/__init__.py` & `pydischarge-0.0.2/pydischarge/signal/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) Duncan Macleod (2019-2020)
+# Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.cli`
+"""Tests for :mod:`pydischarge.signal`
 """
```

### Comparing `pydischarge-0.0.1/pdpy/cli/tests/base.py` & `pydischarge-0.0.2/pydischarge/cli/tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.cli`
+"""Unit tests for :mod:`pydischarge.cli`
 """
 
 from argparse import ArgumentParser
 from unittest import mock
 
 import pytest
 
@@ -77,15 +77,15 @@
 
 class _TestCliProduct(object):
     ACTION = None
     TEST_CLASS = cliproduct.CliProduct
     TEST_ARGS = [
         '--chan', 'X1:TEST-CHANNEL',
         '--start', 0,
-        '--nds2-server', 'nds.test.pdpy',
+        '--nds2-server', 'nds.test.pydischarge',
         '--dpi', 100,
         '--geometry', '640x480',
     ]
 
     # -- fixtures -------------------------------
 
     @classmethod
```

### Comparing `pydischarge-0.0.1/pdpy/cli/tests/test_coherence.py` & `pydischarge-0.0.2/pydischarge/cli/tests/test_coherence.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.cli.coherence`
+"""Unit tests for :mod:`pydischarge.cli.coherence`
 """
 
 from ... import cli
 from .base import _TestCliProduct
 from .test_spectrum import TestCliSpectrum as _TestCliSpectrum
```

### Comparing `pydischarge-0.0.1/pdpy/cli/tests/test_coherencegram.py` & `pydischarge-0.0.2/pydischarge/cli/tests/test_coherencegram.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.cli.coherencegram`
+"""Unit tests for :mod:`pydischarge.cli.coherencegram`
 """
 
 from ... import cli
 from .test_spectrogram import TestCliSpectrogram as _TestCliSpectrogram
 from .test_coherence import TestCliCoherence as _TestCliCoherence
```

### Comparing `pydischarge-0.0.1/pdpy/cli/tests/test_gwpy_plot.py` & `pydischarge-0.0.2/pydischarge/cli/tests/test_gwpy_plot.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for `pdpy-plot` command line module `pdpy.cli.pdpy_plot`
+"""Tests for `pydischarge-plot` command line module `pydischarge.cli.pydischarge_plot`
 """
 
 from unittest import mock
 
 import pytest
 
 from .. import (
     PRODUCTS,
-    pdpy_plot,
+    pydischarge_plot,
 )
 from .base import mock_nds2_connection
 
 
 @pytest.mark.parametrize("mode", [None] + list(PRODUCTS.keys()))
-def test_pdpy_plot_help(mode):
+def test_pydischarge_plot_help(mode):
     args = [mode, "--help"] if mode else ["--help"]
     with pytest.raises(SystemExit) as exc:
-        pdpy_plot.main(args)
+        pydischarge_plot.main(args)
     assert exc.value.code == 0
 
 
 @pytest.mark.requires("nds2")
-def test_pdpy_plot_timeseries(tmp_path):
+def test_pydischarge_plot_timeseries(tmp_path):
     tmp = tmp_path / "plot.png"
     with mock.patch(
         'nds2.connection',
         return_value=mock_nds2_connection()[0],
     ):
         args = [
             "timeseries",
             "--chan", "X1:TEST-CHANNEL",
             "--start", 0,
-            "--nds2-server", "nds.test.pdpy",  # don't use datafind
+            "--nds2-server", "nds.test.pydischarge",  # don't use datafind
             "--out", str(tmp),
         ]
-        exitcode = pdpy_plot.main(args)
+        exitcode = pydischarge_plot.main(args)
         assert not exitcode  # passed
         assert tmp.is_file()  # plot was created
```

### Comparing `pydischarge-0.0.1/pdpy/cli/tests/test_qtransform.py` & `pydischarge-0.0.2/pydischarge/cli/tests/test_qtransform.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.cli.qtransform`
+"""Unit tests for :mod:`pydischarge.cli.qtransform`
 """
 
 import os
 import re
 from unittest import mock
 
 import pytest
@@ -31,15 +31,15 @@
 
 
 class TestCliQtransform(_TestCliSpectrogram):
     TEST_CLASS = cli.Qtransform
     ACTION = 'qtransform'
     TEST_ARGS = [
         '--chan', 'X1:TEST-CHANNEL', '--gps', '5', '--search', '10',
-        '--nds2-server', 'nds.test.pdpy', '--outdir', os.path.curdir,
+        '--nds2-server', 'nds.test.pydischarge', '--outdir', os.path.curdir,
         '--average-method', 'median',
     ]
 
     def test_finalize_arguments(self, prod):
         assert prod.start_list == [prod.args.gps - prod.args.search/2.]
         assert prod.duration == prod.args.search
         assert prod.args.color_scale == 'linear'
```

### Comparing `pydischarge-0.0.1/pdpy/cli/tests/test_spectrogram.py` & `pydischarge-0.0.2/pydischarge/cli/tests/test_spectrogram.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.cli.spectrogram`
+"""Unit tests for :mod:`pydischarge.cli.spectrogram`
 """
 
 import pytest
 
 from ... import cli
 from .base import (_TestImageProduct, _TestTimeDomainProduct, _TestFFTMixin)
```

### Comparing `pydischarge-0.0.1/pdpy/cli/tests/test_spectrum.py` & `pydischarge-0.0.2/pydischarge/cli/tests/test_spectrum.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.cli.spectrum`
+"""Unit tests for :mod:`pydischarge.cli.spectrum`
 """
 
 from astropy.time import Time
 
 from ... import cli
 from .base import _TestFrequencyDomainProduct
```

### Comparing `pydischarge-0.0.1/pdpy/cli/tests/test_timeseries.py` & `pydischarge-0.0.2/pydischarge/cli/tests/test_timeseries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.cli.timeseries`
+"""Unit tests for :mod:`pydischarge.cli.timeseries`
 """
 
 from ... import cli
 from .base import (_TestTimeDomainProduct, update_namespace)
 
 
 class TestCliTimeSeries(_TestTimeDomainProduct):
```

### Comparing `pydischarge-0.0.1/pdpy/cli/tests/test_transferfunction.py` & `pydischarge-0.0.2/pydischarge/cli/tests/test_transferfunction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Evan Goetz (2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.cli.transferfunction`
+"""Unit tests for :mod:`pydischarge.cli.transferfunction`
 """
 
 from astropy.time import Time
 
 from ... import cli
 from .base import _TestCliProduct, _TestTransferFunctionProduct
```

### Comparing `pydischarge-0.0.1/pdpy/cli/timeseries.py` & `pydischarge-0.0.2/pydischarge/cli/timeseries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Joseph Areeda (2015-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """The timeseries CLI product
 """
 
 from .cliproduct import TimeDomainProduct
 from ..plot import Plot
 from ..plot.tex import label_to_latex
```

### Comparing `pydischarge-0.0.1/pdpy/cli/transferfunction.py` & `pydischarge-0.0.2/pydischarge/cli/transferfunction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Evan Goetz (2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Transfer function plots
 """
 
 from astropy.time import Time
 from collections import OrderedDict
 import numpy as np
```

### Comparing `pydischarge-0.0.1/pdpy/conftest.py` & `pydischarge-0.0.2/pydischarge/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Test setup for pdpy
+"""Test setup for pydischarge
 """
 
 import warnings
 
 import numpy
 
 from matplotlib import (use, rcParams)
@@ -39,15 +39,15 @@
 # -- plotting options
 
 # ignore errors due from pyplot.show() using Agg
 warnings.filterwarnings('ignore', message=".*non-GUI backend.*")
 
 # force simpler rcParams for all tests
 # (fixtures or tests may update these individually)
-# NOTE: this most-likely happens _after_ pdpy.plot has
+# NOTE: this most-likely happens _after_ pydischarge.plot has
 #       updated the rcParams once, so these settings should persist
 rcParams.update({
     'text.usetex': False,  # TeX is slow most of the time
 })
 
 
 # -- pytest configuration
```

### Comparing `pydischarge-0.0.1/pdpy/detector/__init__.py` & `pydischarge-0.0.2/pydischarge/detector/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""This module defines the :class:`~pdpy.detector.Channel`.
+"""This module defines the :class:`~pydischarge.detector.Channel`.
 """
 
 # This module used to define the `LaserInterferometer` class, but it was
 # removed # pre-release because it never got used, or implemented properly.
 
 import datetime
```

### Comparing `pydischarge-0.0.1/pdpy/detector/channel.py` & `pydischarge-0.0.2/pydischarge/detector/channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module defines the `Channel` and `ChannelList` classes.
 """
 
 import re
 from copy import copy
 from math import ceil
@@ -845,33 +845,33 @@
         Parameters
         ----------
         channels : `list`
             list of `Channel` or `str` for which to search
 
         start : `int`
             GPS start time of search, or any acceptable input to
-            :meth:`~pdpy.time.to_gps`
+            :meth:`~pydischarge.time.to_gps`
 
         end : `int`
             GPS end time of search, or any acceptable input to
-            :meth:`~pdpy.time.to_gps`
+            :meth:`~pydischarge.time.to_gps`
 
         connection : `nds2.connection`, optional
             open connection to an NDS(2) server, if not given, one will be
             created based on ``host`` and ``port`` keywords
 
         host : `str`, optional
             name of NDS server host
 
         port : `int`, optional
             port number for NDS connection
 
         Returns
         -------
-        segdict : `~pdpy.segments.SegmentListDict`
+        segdict : `~pydischarge.segments.SegmentListDict`
             dict of ``(name, SegmentList)`` pairs
         """
         start = int(to_gps(start))
         end = int(ceil(to_gps(end)))
         chans = io_nds2.find_channels(channels, connection=connection,
                                       unique=True, epoch=(start, end),
                                       type=ctype)
```

### Comparing `pydischarge-0.0.1/pdpy/detector/io/__init__.py` & `pydischarge-0.0.2/pydischarge/segments/io/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Input/Output routines for Channel and ChannelList
+"""Input/output routines for the `pydischarge.segments` classes
 """
 
 from . import (  # pylint: disable=unused-import
-    cis,  # querying Channel Information System (cis.ligo.org)
-    clf,  # LIGO Channel List File (clf) format
-    omega,  # Omega pipeline scan configurations
+    ligolw,  # LIGO_LW XML
+    segwizard,  # LIGO SegWizard ASCII
+    hdf5,  # HDF5
+    json,  # segments-web.ligo.org JSON
 )
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
```

### Comparing `pydischarge-0.0.1/pdpy/detector/io/cis.py` & `pydischarge-0.0.2/pydischarge/detector/io/cis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Interface to the LIGO Channel Information System
 """
 
 import numpy
 
 from .. import (Channel, ChannelList)
@@ -39,29 +39,29 @@
 
 def query(name, kerberos=None, **kwargs):
     """Query the Channel Information System for details on the given
     channel name
 
     Parameters
     ----------
-    name : `~pdpy.detector.Channel`, or `str`
+    name : `~pydischarge.detector.Channel`, or `str`
         Name of the channel of interest
 
     kerberos : `bool`, optional
         use an existing Kerberos ticket as the authentication credential,
         default behaviour will check for credentials and request username
         and password if none are found (`None`)
 
     kwargs
         other keyword arguments are passed directly to
         :func:`ciecplib.get`
 
     Returns
     -------
-    channel : `~pdpy.detector.Channel`
+    channel : `~pydischarge.detector.Channel`
         Channel with all details as acquired from the CIS
     """
     url = f"{CIS_API_URL}/?q={name}"
     more = True
     out = ChannelList()
     while more:
         reply = _get(url, kerberos=kerberos, **kwargs)
```

### Comparing `pydischarge-0.0.1/pdpy/detector/io/clf.py` & `pydischarge-0.0.2/pydischarge/detector/io/clf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2015-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 Channel List Files
 ==================
 
 The Channel List File (CLF) is a schema of the INI configuration file format
 designed to hold lists of interferometer data channels for bulk processing.
@@ -86,15 +86,15 @@
     r"(?:\s+(?P<sample_rate>[0-9.]+))?"
     r"(?:\s+(?P<safe>(safe|unsafe|unsafeabove2kHz|unknown)))?"
     r"(?:\s+(?P<fidelity>(clean|flat|glitchy|unknown)))?"
 )
 
 
 def read_channel_list_file(*source):
-    """Read a `~pdpy.detector.ChannelList` from a Channel List File
+    """Read a `~pydischarge.detector.ChannelList` from a Channel List File
     """
     # read file(s)
     config = configparser.ConfigParser(dict_type=OrderedDict)
     source = file_list(source)
     success_ = config.read(*source)
     if len(success_) != len(source):
         raise IOError("Failed to read one or more CLF files")
@@ -136,15 +136,15 @@
                 setattr(channel, key, channel.params.pop(key, None))
             append(channel)
     return out
 
 
 @with_open(mode="w", pos=1)
 def write_channel_list_file(channels, fobj):
-    """Write a `~pdpy.detector.ChannelList` to a INI-format channel list file
+    """Write a `~pydischarge.detector.ChannelList` to a INI-format channel list file
     """
     out = configparser.ConfigParser(dict_type=OrderedDict)
     for channel in channels:
         group = channel.group
         if not out.has_section(group):
             out.add_section(group)
         for param, value in channel.params.items():
```

### Comparing `pydischarge-0.0.1/pdpy/detector/io/omega.py` & `pydischarge-0.0.2/pydischarge/detector/io/omega.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2015-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """I/O routines for parsing Omega pipeline scan channel lists
 """
 
 import sys
 import os
 from collections import OrderedDict
@@ -125,15 +125,15 @@
 
     This method is dumb and assumes the channels are sorted in the right
     order already
     """
     # print header
     if header:
         print('# Q Scan configuration file', file=fobj)
-        print('# Generated with PDpy from a ChannelList', file=fobj)
+        print('# Generated with pyDischarge from a ChannelList', file=fobj)
     group = None
     for channel in channellist:
         # print header
         if channel.group != group:
             group = channel.group
             print(f'\n[{group}]', file=fobj)
         print("", file=fobj)
```

### Comparing `pydischarge-0.0.1/pdpy/detector/tests/__init__.py` & `pydischarge-0.0.2/pydischarge/detector/tests/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.detector`
+"""Tests for :mod:`pydischarge.detector`
 """
```

### Comparing `pydischarge-0.0.1/pdpy/detector/tests/test_channel.py` & `pydischarge-0.0.2/pydischarge/detector/tests/test_channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Unit test for detector module
 """
 
 from unittest import mock
 
 import pytest
```

### Comparing `pydischarge-0.0.1/pdpy/detector/tests/test_units.py` & `pydischarge-0.0.2/pydischarge/detector/tests/test_units.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.detector.units`
+"""Unit tests for :mod:`pydischarge.detector.units`
 """
 
 import pytest
 
 from astropy import units
 
 from ..units import parse_unit
```

### Comparing `pydischarge-0.0.1/pdpy/detector/units.py` & `pydischarge-0.0.2/pydischarge/detector/units.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module registers a number of custom units used in GW astronomy.
 """
 
 import re
 import warnings
 
@@ -30,26 +30,26 @@
 
 # container for new units (so that each one only gets created once)
 UNRECOGNIZED_UNITS = {}
 
 
 # -- parser to handle any unit ------------------------------------------------
 
-class PDpyFormat(Generic):
+class pydischargeFormat(Generic):
     """Sub-class of the `Generic` unit parser that is more forgiving
 
     This format tries to work around 'human' errors in unit naming,
     including plurals, and capitalisation, and if nothing else works
     it just defines a new unit matching the given string.
 
     New units are not registered, so cannot be referred to later, but are
     created so that mathematical operations will work. Conversions to other
     units will explicitly not work.
     """
-    name = 'pdpy'
+    name = 'pydischarge'
     re_closest_unit = re.compile(r'Did you mean (.*)\?\Z')
     re_closest_unit_delim = re.compile('(, | or )')
     warn = True
 
     @classmethod
     def _get_unit(cls, t):
         # match as normal
@@ -91,15 +91,15 @@
                     u = UNRECOGNIZED_UNITS[name] = units.def_unit(
                         name, doc='Unrecognized unit')
                     return u
             return cls._parse_unit(alt)
 
 
 # pylint: disable=redefined-builtin
-def parse_unit(name, parse_strict='warn', format='pdpy'):
+def parse_unit(name, parse_strict='warn', format='pydischarge'):
     """Attempt to intelligently parse a `str` as a `~astropy.units.Unit`
 
     Parameters
     ----------
     name : `str`
         unit name to parse
 
@@ -132,18 +132,18 @@
         except ValueError as exc:
             if (
                 parse_strict == 'raise'
                 or 'did not parse as unit' not in str(exc)
             ):
                 raise
             # try again using out own lenient parser
-            PDpyFormat.warn = parse_strict != 'silent'
+            pydischargeFormat.warn = parse_strict != 'silent'
             return units.Unit(name, parse_strict='silent', format=format)
         finally:
-            PDpyFormat.warn = True
+            pydischargeFormat.warn = True
 
 
 # -- custom units -------------------------------------------------------------
 # pylint: disable=no-member,invalid-name
 
 # enable imperial units
 units.add_enabled_units(units_imperial)
```

### Comparing `pydischarge-0.0.1/pdpy/frequencyseries/__init__.py` & `pydischarge-0.0.2/pydischarge/spectrogram/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Create, manipulate, read, and write spectrum data
+"""Create, manipulate, read, and write spectrogram data
 """
 
-# import objects
-from .frequencyseries import FrequencySeries
-from .hist import SpectralVariance
+from .spectrogram import (Spectrogram, SpectrogramList)
 
-# import unified I/O
-from . import io  # pylint: disable=unused-import
+from . import io  # register I/O
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
```

### Comparing `pydischarge-0.0.1/pdpy/frequencyseries/_fdcommon.py` & `pydischarge-0.0.2/pydischarge/frequencyseries/_fdcommon.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Common utilities for frequency-domain operations
 
 This module holds code used by both the `FrequencySeries` and `Spectrogram`.
 """
 
 import numpy
@@ -31,16 +31,16 @@
 
 
 def fdfilter(data, *filt, **kwargs):
     """Filter a frequency-domain data object
 
     See also
     --------
-    pdpy.frequencyseries.FrequencySeries.filter
-    pdpy.spectrogram.Spectrogram.filter
+    pydischarge.frequencyseries.FrequencySeries.filter
+    pydischarge.spectrogram.Spectrogram.filter
     """
     # parse keyword args
     inplace = kwargs.pop('inplace', False)
     analog = kwargs.pop('analog', False)
     fs = kwargs.pop('sample_rate', None)
     if kwargs:
         raise TypeError(
```

### Comparing `pydischarge-0.0.1/pdpy/frequencyseries/frequencyseries.py` & `pydischarge-0.0.2/pydischarge/frequencyseries/frequencyseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Representation of a frequency series
 """
 
 import warnings
 
 import numpy
@@ -52,22 +52,22 @@
         frequency resolution for these data
 
     frequencies : `array-like`
         the complete array of frequencies indexing the data.
         This argument takes precedence over `f0` and `df` so should
         be given in place of these if relevant, not alongside
 
-    epoch : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+    epoch : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
         GPS epoch associated with these data,
-        any input parsable by `~pdpy.time.to_gps` is fine
+        any input parsable by `~pydischarge.time.to_gps` is fine
 
     name : `str`, optional
         descriptive title for this array
 
-    channel : `~pdpy.detector.Channel`, `str`, optional
+    channel : `~pydischarge.detector.Channel`, `str`, optional
         source data stream for these data
 
     dtype : `~numpy.dtype`, optional
         input data type
 
     copy : `bool`, optional, default: `False`
         choose to copy the input data to new memory
@@ -203,15 +203,15 @@
 
     def ifft(self):
         """Compute the one-dimensional discrete inverse Fourier
         transform of this `FrequencySeries`.
 
         Returns
         -------
-        out : :class:`~pdpy.timeseries.TimeSeries`
+        out : :class:`~pydischarge.timeseries.TimeSeries`
             the normalised, real-valued `TimeSeries`.
 
         See also
         --------
         numpy.fft.irfft : The inverse (real) FFT function
 
         Notes
@@ -415,15 +415,15 @@
 
         copy : `bool`, optional, default: `True`
             if `True`, copy these data to a new array
 
         Returns
         -------
         spectrum : `FrequencySeries`
-            a PDpy version of the input frequency series
+            a pyDischarge version of the input frequency series
         """
         return cls(fs.data, f0=0, df=fs.delta_f, epoch=fs.epoch, copy=copy)
 
     def to_pycbc(self, copy=True):
         """Convert this `FrequencySeries` into a
         `~pycbc.types.frequencyseries.FrequencySeries`
```

### Comparing `pydischarge-0.0.1/pdpy/frequencyseries/hist.py` & `pydischarge-0.0.2/pydischarge/frequencyseries/hist.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module provides a spectral-variation histogram class
 """
 
 import numpy
 
 from astropy.io import registry as io_registry
@@ -217,19 +217,19 @@
             return super().__getitem__(item)
         raise NotImplementedError("cannot slice SpectralVariance across bins")
     __getitem__.__doc__ = Array2D.__getitem__.__doc__
 
     @classmethod
     def from_spectrogram(cls, *spectrograms, **kwargs):
         """Calculate a new `SpectralVariance` from a
-        :class:`~pdpy.spectrogram.Spectrogram`
+        :class:`~pydischarge.spectrogram.Spectrogram`
 
         Parameters
         ----------
-        spectrogram : `~pdpy.spectrogram.Spectrogram`
+        spectrogram : `~pydischarge.spectrogram.Spectrogram`
             input `Spectrogram` data
 
         bins : `~numpy.ndarray`, optional
             array of histogram bin edges, including the rightmost edge
 
         low : `float`, optional
             left edge of lowest amplitude bin, only read
@@ -321,15 +321,15 @@
         Parameters
         ----------
         percentile : `float`
             percentile (0 - 100) of the bins to compute
 
         Returns
         -------
-        spectrum : `~pdpy.frequencyseries.FrequencySeries`
+        spectrum : `~pydischarge.frequencyseries.FrequencySeries`
             the given percentile `FrequencySeries` calculated from this
             `SpectralVaraicence`
         """
         rows, columns = self.shape
         out = numpy.zeros(rows)
         # Loop over frequencies
         for i in range(rows):
```

### Comparing `pydischarge-0.0.1/pdpy/frequencyseries/io/__init__.py` & `pydischarge-0.0.2/pydischarge/types/io/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Input/Output routines for pdpy.frequencyseries
+"""Input/Output routines for the Array and its sub-classes.
 """
 
 from . import (  # pylint: disable=unused-import
-    ascii,
     hdf5,
-    ligolw,
+    ascii,
 )
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
```

### Comparing `pydischarge-0.0.1/pdpy/frequencyseries/io/ascii.py` & `pydischarge-0.0.2/pydischarge/frequencyseries/io/ascii.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""ASCII I/O registrations for pdpy.frequencyseries objects
+"""ASCII I/O registrations for pydischarge.frequencyseries objects
 """
 
 from ...types.io.ascii import register_ascii_series_io
 from .. import FrequencySeries
 
 # -- registration -------------------------------------------------------------
```

### Comparing `pydischarge-0.0.1/pdpy/frequencyseries/io/hdf5.py` & `pydischarge-0.0.2/pydischarge/frequencyseries/io/hdf5.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module attaches the HDF5 input output methods to the FrequencySeries.
 """
 
 from ...types.io.hdf5 import register_hdf5_array_io
 from .. import (FrequencySeries, SpectralVariance)
```

### Comparing `pydischarge-0.0.1/pdpy/frequencyseries/io/ligolw.py` & `pydischarge-0.0.2/pydischarge/frequencyseries/io/ligolw.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""LIGO_LW I/O registrations for pdpy.frequencyseries objects
+"""LIGO_LW I/O registrations for pydischarge.frequencyseries objects
 """
 
 from ...io import registry as io_registry
 from ...io.ligolw import is_ligolw
 from ...types.io.ligolw import read_series
 from .. import FrequencySeries
```

### Comparing `pydischarge-0.0.1/pdpy/frequencyseries/tests/__init__.py` & `pydischarge-0.0.2/pydischarge/spectrogram/tests/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.frequencyseries`
+"""Tests for :mod:`pydischarge.spectrogram`
 """
```

### Comparing `pydischarge-0.0.1/pdpy/frequencyseries/tests/test_frequencyseries.py` & `pydischarge-0.0.2/pydischarge/frequencyseries/tests/test_frequencyseries.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Unit test for frequencyseries module
 """
 
 from io import BytesIO
 
 import pytest
```

### Comparing `pydischarge-0.0.1/pdpy/frequencyseries/tests/test_hist.py` & `pydischarge-0.0.2/pydischarge/frequencyseries/tests/test_hist.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Unit test for frequencyseries module
 """
 
 from io import BytesIO
 
 import pytest
```

### Comparing `pydischarge-0.0.1/pdpy/io/__init__.py` & `pydischarge-0.0.2/pydischarge/astro/tests/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) Duncan Macleod (2014-2020)
+# Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Utilities for data input/output in standard GW formats.
+"""Tests for :mod:`pydischarge.astro`
 """
-
-__author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
```

### Comparing `pydischarge-0.0.1/pdpy/io/_framecpp.py` & `pydischarge-0.0.2/pydischarge/io/_framecpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """GWF I/O utilities for frameCPP
 
 This module is where all constants and variables that require
 frameCPP should go, as opposed to functions which can import
 the necessary objects at runtime.
 """
```

### Comparing `pydischarge-0.0.1/pdpy/io/cache.py` & `pydischarge-0.0.2/pydischarge/io/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Input/Output utilities for GW Cache files.
 
 A cache file is a specially-formatted ASCII file that contains file paths
 and associated metadata for those files, designed to make identifying
 relevant data, and sieving large file lists, easier for the user.
 """
@@ -169,15 +169,15 @@
 
     coltype : `LIGOTimeGPS`, `int`, optional
         Type for GPS times.
 
     sort : `callable`, optional
         A callable key function by which to sort the output list of file paths
 
-    segment : `pdpy.segments.Segment`, optional
+    segment : `pydischarge.segments.Segment`, optional
         A GPS `[start, stop)` interval, if given only files overlapping this
         interval will be returned.
 
     strict : `bool`, optional
         If `False` warn about entries that don't follow the LIGO-T050017
         standard, then skip them; if `True` all errors are raised as
         exceptions.
@@ -222,15 +222,15 @@
         if the line cannot be parsed successfully
     """
     return _CacheEntry.parse(line, gpstype=gpstype).path
 
 
 def open_cache(*args, **kwargs):  # pragma: no cover
     # pylint: disable=missing-docstring
-    warnings.warn("pdpy.io.cache.open_cache was renamed read_cache",
+    warnings.warn("pydischarge.io.cache.open_cache was renamed read_cache",
                   DeprecationWarning)
     return read_cache(*args, **kwargs)
 
 
 @with_open(mode="w", pos=1)
 def write_cache(cache, fobj, format=None):
     """Write a `list` of cache entries to a file
@@ -340,26 +340,26 @@
     -------
     obs : `str`
         the observatory metadata
 
     tag : `str`
         the file tag
 
-    segment : `pdpy.segments.Segment`
+    segment : `pydischarge.segments.Segment`
         the GPS ``[float, float)`` interval for this file
 
     Notes
     -----
     `LIGO-T050017 <https://dcc.ligo.org/LIGO-T050017>`__ declares a
     file naming convention that includes documenting the GPS start integer
     and integer duration of a file, see that document for more details.
 
     Examples
     --------
-    >>> from pdpy.io.cache import filename_metadata
+    >>> from pydischarge.io.cache import filename_metadata
     >>> filename_metadata("A-B-0-1.txt")
     ('A', 'B', Segment(0, 1))
     >>> filename_metadata("A-B-0.456-1.345.txt")
     ("A", "B", Segment(0.456, 1.801))
     """
     from ..segments import Segment
     name = os.path.basename(filename)
@@ -390,15 +390,15 @@
     Parameters
     ---------
     filename : `str`, :class:`~lal.utils.CacheEntry`
         the path name of a file
 
     Returns
     -------
-    segment : `~pdpy.segments.Segment`
+    segment : `~pydischarge.segments.Segment`
         the ``[start, stop)`` GPS segment covered by the given file
 
     Notes
     -----
     |LIGO-T050017|_ declares a filenaming convention that includes
     documenting the GPS start integer and integer duration of a file,
     see that document for more details.
@@ -417,15 +417,15 @@
     ----------
     *caches : `list`
         One or more lists of file paths
         (`str` or :class:`~lal.utils.CacheEntry`).
 
     Returns
     -------
-    segments : `~pdpy.segments.SegmentList`
+    segments : `~pydischarge.segments.SegmentList`
         A list of segments for when data should be available
     """
     from ..segments import SegmentList
     out = SegmentList()
     for cache in caches:
         out.extend(file_segment(e) for e in cache)
     return out.coalesce()
@@ -472,15 +472,15 @@
     """Filter the cache to find those entries that overlap ``segment``
 
     Parameters
     ----------
     cache : `list`
         Input list of file paths
 
-    segment : `~pdpy.segments.Segment`
+    segment : `~pydischarge.segments.Segment`
         The ``[start, stop)`` interval to match against.
 
     strict : `bool`, optional
         If `True` raise all exceptions, if `False` emit warnings when
         the file segment cannot be determined.
 
     Warns
@@ -506,17 +506,17 @@
     return out
 
 
 # -- moved functions ----------------------------------------------------------
 
 def file_name(*args, **kwargs):
     from .utils import file_path
-    warnings.warn("this function has been moved to pdpy.io.utils.file_path",
+    warnings.warn("this function has been moved to pydischarge.io.utils.file_path",
                   DeprecationWarning)
     return file_path(*args, **kwargs)
 
 
 def file_list(*args, **kwargs):
     from .utils import file_list
-    warnings.warn("this function has been moved to pdpy.io.utils.file_list",
+    warnings.warn("this function has been moved to pydischarge.io.utils.file_list",
                   DeprecationWarning)
     return file_list(*args, **kwargs)
```

### Comparing `pydischarge-0.0.1/pdpy/io/datafind.py` & `pydischarge-0.0.2/pydischarge/io/datafind.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utilities for auto-discovery of GW data files.
 
 Automatic discovery of file paths for both LIGO and Virgo index solutions
 (``gwdatafind`` or ``ffl``, respectvely) is supported.
 
 The functions in this module are highly reliant on having local access to
 files (either directly, or via NFS, or CVMFS).
 
 Data discovery using the DataFind service requires the `gwdatafind` Python
-package (a dependency of ``pdpy``), and either the ``GW_DATAFIND_SERVER``
+package (a dependency of ``pydischarge``), and either the ``GW_DATAFIND_SERVER``
 (or legacy ``LIGO_DATAFIND_SERVER``) environment variable to be set,
 or the ``host`` keyword must be passed to :func:`find_urls` and friends.
 
 Data discovery using the Virgo FFL system requires the ``FFLPATH`` environment
 variable to point to the directory containing FFL files, **or** the
 ``VIRGODATA`` environment variable to point to a directory containing an
 ``ffl` subdirectory, which contains FFL files.
@@ -129,15 +129,15 @@
             return False
     return False
 
 
 def _gwdatafind_module(**datafind_kw):
     """Return the appropriate GWDataFind-like API based on the environment
 
-    This allows switching to the hacky `pdpy.io.ffldatafind` replacement
+    This allows switching to the hacky `pydischarge.io.ffldatafind` replacement
     module to enable a GWDataFind-like interface for direct FFL data
     discovery at Virgo.
     """
     # GWDataFind
     if (
         os.getenv('GWDATAFIND_SERVER')
         or os.getenv('LIGO_DATAFIND_SERVER')
@@ -155,15 +155,15 @@
     return ffldatafind
 
 
 def _select_gwdatafind_mod(func):
     """Decorate a function to see the right ``gwdatafind`` API.
 
     This exists only to allow on-the-fly replacing of the actual `gwdatafind`
-    with :mod:`pdpy.io.ffldatafind` if it looks like we are trying to find
+    with :mod:`pydischarge.io.ffldatafind` if it looks like we are trying to find
     data from FFL files.
     """
     @wraps(func)
     def wrapped(*args, **kwargs):
         # replace the 'gwdatafind' module in the function namespace
         # with the API we need for this call
         with mock.patch.dict(func.__globals__):
@@ -248,15 +248,15 @@
 def find_frametype(channel, gpstime=None, frametype_match=None,
                    host=None, port=None, return_all=False, allow_tape=False,
                    on_gaps='error'):
     """Find the frametype(s) that hold data for a given channel
 
     Parameters
     ----------
-    channel : `str`, `~pdpy.detector.Channel`
+    channel : `str`, `~pydischarge.detector.Channel`
         the channel to be found
 
     gpstime : `int`, optional
         target GPS time at which to find correct type
 
     frametype_match : `str`, optional
         regular expression to use for frametype `str` matching
@@ -293,15 +293,15 @@
         the list of all matching frame types
 
     If multiple names are given, the above return types are wrapped into a
     `dict` of `(channel, type_or_list)` pairs.
 
     Examples
     --------
-    >>> from pdpy.io import datafind as io_datafind
+    >>> from pydischarge.io import datafind as io_datafind
     >>> io_datafind.find_frametype('H1:IMC-PWR_IN_OUTPUT', gpstime=1126259462)
     'H1_R'
     >>> io_datafind.find_frametype('H1:IMC-PWR_IN_OUTPUT', gpstime=1126259462,
     ...                            return_all=True)
     ['H1_R', 'H1_C']
     >>> io_datafind.find_frametype(
     ...     ('H1:IMC-PWR_IN_OUTPUT', 'H1:OMC-DCPD_SUM_OUTPUT',
@@ -431,24 +431,24 @@
 def find_best_frametype(channel, start, end,
                         frametype_match=None, allow_tape=True,
                         host=None, port=None):
     """Intelligently select the best frametype from which to read this channel
 
     Parameters
     ----------
-    channel : `str`, `~pdpy.detector.Channel`
+    channel : `str`, `~pydischarge.detector.Channel`
         the channel to be found
 
-    start : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+    start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
         GPS start time of period of interest,
-        any input parseable by `~pdpy.time.to_gps` is fine
+        any input parseable by `~pydischarge.time.to_gps` is fine
 
-    end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+    end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
         GPS end time of period of interest,
-        any input parseable by `~pdpy.time.to_gps` is fine
+        any input parseable by `~pydischarge.time.to_gps` is fine
 
     host : `str`, optional
         name of datafind host to use
 
     port : `int`, optional
         port on datafind host to use
 
@@ -468,15 +468,15 @@
     Raises
     ------
     ValueError
         if no valid frametypes are found
 
     Examples
     --------
-    >>> from pdpy.io.datafind import find_best_frametype
+    >>> from pydischarge.io.datafind import find_best_frametype
     >>> find_best_frametype('L1:GDS-CALIB_STRAIN', 1126259460, 1126259464)
     'L1_HOFT_C00'
     """
     try:
         return find_frametype(channel, gpstime=(start, end),
                               frametype_match=frametype_match,
                               allow_tape=allow_tape, on_gaps='error',
```

### Comparing `pydischarge-0.0.1/pdpy/io/ffldatafind.py` & `pydischarge-0.0.2/pydischarge/io/ffldatafind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Cardiff University (2022)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """GWDataFind UI for FFL cache files.
 
 This module is used to replace the proper GWDataFind interface
 on-the-fly when FFL data access is inferred.
 As such this module is required to emulate those functions
-from `gwdatafind` used in :mod:`pdpy.io.datafind`.
+from `gwdatafind` used in :mod:`pydischarge.io.datafind`.
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
 
 import os
 import re
 from warnings import warn
```

### Comparing `pydischarge-0.0.1/pdpy/io/gwf.py` & `pydischarge-0.0.2/pydischarge/io/gwf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """I/O utilities for GWF files using the lalframe or frameCPP APIs
 """
 
 import warnings
 
 import numpy
@@ -136,15 +136,15 @@
     if isinstance(frames, frameCPP.FrameH):
         frames = [frames]
     for frame in frames:
         stream.WriteFrame(frame, int(compression), int(compression_level))
     # stream auto-closes (apparently)
 
 
-def create_frame(time=0, duration=None, name='pdpy', run=-1, ifos=None):
+def create_frame(time=0, duration=None, name='pydischarge', run=-1, ifos=None):
     """Create a new :class:`~LDAStools.frameCPP.FrameH`
 
     **Requires:** |LDAStools.frameCPP|_
 
     Parameters
     ----------
     time : `float`, optional
@@ -193,23 +193,23 @@
     frame.SetRun(run)
 
     return frame
 
 
 def create_fradcdata(series, frame_epoch=0,
                      channelgroup=0, channelid=0, nbits=16):
-    """Create a `~frameCPP.FrAdcData` from a `~pdpy.types.Series`
+    """Create a `~frameCPP.FrAdcData` from a `~pydischarge.types.Series`
 
     .. note::
 
        Currently this method is restricted to 1-dimensional arrays.
 
     Parameters
     ----------
-    series : `~pdpy.types.Series`
+    series : `~pydischarge.types.Series`
         the input data array to store
 
     frame_epoch : `float`, `int`, optional
         the GPS start epoch of the `Frame` that will contain this
         data structure
 
     Returns
@@ -254,23 +254,23 @@
         return abs(series.yspan)
     return 0
 
 
 def create_frprocdata(series, frame_epoch=0, comment=None,
                       type=None, subtype=None, trange=None,
                       fshift=0, phase=0, frange=None, bandwidth=0):
-    """Create a `~frameCPP.FrAdcData` from a `~pdpy.types.Series`
+    """Create a `~frameCPP.FrAdcData` from a `~pydischarge.types.Series`
 
     .. note::
 
        Currently this method is restricted to 1-dimensional arrays.
 
     Parameters
     ----------
-    series : `~pdpy.types.Series`
+    series : `~pydischarge.types.Series`
         the input data array to store
 
     frame_epoch : `float`, `int`, optional
         the GPS start epoch of the `Frame` that will contain this
         data structure
 
     comment : `str`, optional
@@ -326,23 +326,23 @@
         phase,
         frange,
         bandwidth,
     )
 
 
 def create_frsimdata(series, frame_epoch=0, comment=None, fshift=0, phase=0):
-    """Create a `~frameCPP.FrAdcData` from a `~pdpy.types.Series`
+    """Create a `~frameCPP.FrAdcData` from a `~pydischarge.types.Series`
 
     .. note::
 
        Currently this method is restricted to 1-dimensional arrays.
 
     Parameters
     ----------
-    series : `~pdpy.types.Series`
+    series : `~pydischarge.types.Series`
         the input data array to store
 
     frame_epoch : `float`, `int`, optional
         the GPS start epoch of the `Frame` that will contain this
         data structure
 
     fshift : `float`, optional
@@ -374,23 +374,23 @@
         float(to_gps(series.x0.value) - to_gps(frame_epoch)),
         fshift,
         phase,
     )
 
 
 def create_frvect(series):
-    """Create a `~frameCPP.FrVect` from a `~pdpy.types.Series`
+    """Create a `~frameCPP.FrVect` from a `~pydischarge.types.Series`
 
     .. note::
 
        Currently this method is restricted to 1-dimensional arrays.
 
     Parameters
     ----------
-    series : `~pdpy.types.Series`
+    series : `~pydischarge.types.Series`
         the input data array to store
 
     Returns
     -------
     frvect : `~frameCPP.FrVect`
         the newly created data vector
     """
@@ -444,15 +444,15 @@
 def get_channel_type(channel, framefile):
     """Find the channel type in a given GWF file
 
     **Requires:** |LDAStools.frameCPP|_
 
     Parameters
     ----------
-    channel : `str`, `~pdpy.detector.Channel`
+    channel : `str`, `~pydischarge.detector.Channel`
         name of data channel to find
 
     framefile : `str`
         path of GWF file in which to search
 
     Returns
     -------
@@ -580,15 +580,15 @@
         the name to check in each frame
 
     warn : `bool`, optional
         emit a `UserWarning` when a channel is not found in a frame
 
     Returns
     -------
-    segments : `~pdpy.segments.SegmentList`
+    segments : `~pydischarge.segments.SegmentList`
         the list of segments containing data
     """
     segments = SegmentList()
     for path in paths:
         segments.extend(_gwf_channel_segments(path, channel, warn=warn))
     return segments.coalesce()
 
@@ -686,15 +686,15 @@
 def _series_name(series):
     """Returns the 'name' of a `Series` that should be written to GWF
 
     This is basically `series.name or str(series.channel) or ""`
 
     Parameters
     ----------
-    series : `pdpy.types.Series`
+    series : `pydischarge.types.Series`
         the input series that will be written
 
     Returns
     -------
     name : `str`
         the name to use when storing this series
     """
```

### Comparing `pydischarge-0.0.1/pdpy/io/hdf5.py` & `pydischarge-0.0.2/pydischarge/io/hdf5.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Write PDpy objects to HDF5 files
+"""Write pyDischarge objects to HDF5 files
 """
 
 import os.path
 from functools import wraps
 
 # pylint: disable=unused-import
 from astropy.io.misc.hdf5 import is_hdf5 as identify_hdf5  # noqa: F401
```

### Comparing `pydischarge-0.0.1/pdpy/io/kerberos.py` & `pydischarge-0.0.2/pydischarge/io/kerberos.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utility module to initialise a kerberos ticket for NDS2 connections
 
 This module provides a lazy-mans python version of the 'kinit'
 command-line tool, with internal guesswork using keytabs
 
 See the documentation of the `kinit` function for example usage
@@ -190,15 +190,15 @@
     -------
     creds : `list` of `tuple`
         the (unique) list of `(username, realm, kvno)` as read from the
         keytab file
 
     Examples
     --------
-    >>> from pdpy.io.kerberos import parse_keytab
+    >>> from pydischarge.io.kerberos import parse_keytab
     >>> print(parse_keytab("creds.keytab"))
     [('albert.einstein', 'LIGO.ORG', 1)]
     """
     try:
         out = subprocess.check_output(['klist', '-k', keytab],
                                       stderr=subprocess.PIPE)
     except OSError:
```

### Comparing `pydischarge-0.0.1/pdpy/io/ligolw.py` & `pydischarge-0.0.2/pydischarge/io/ligolw.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Basic utilities for reading/writing LIGO_LW-format XML files.
 
 All specific unified input/output for class objects should be placed in
 an 'io' subdirectory of the containing directory for that class.
 """
 
@@ -341,15 +341,15 @@
     columns : `list`, optional
         list of column name strings to read, default all.
 
     contenthandler : `~xml.sax.handler.ContentHandler`, optional
         SAX content handler for parsing LIGO_LW documents.
 
     **kwargs
-        other keyword arguments are passed to `~pdpy.io.ligolw.read_ligolw`
+        other keyword arguments are passed to `~pydischarge.io.ligolw.read_ligolw`
 
     Returns
     -------
     table : :class:`~ligo.lw.table.Table`
         `Table` of data
     """
     from ligo.lw.ligolw import Document
@@ -619,15 +619,15 @@
     Parameters
     ----------
     source : `file`, `str`, :class:`~ligo.lw.ligolw.Document`, `list`
         one or more open files, file paths, or LIGO_LW `Document`s
 
     Examples
     --------
-    >>> from pdpy.io.ligolw import list_tables
+    >>> from pydischarge.io.ligolw import list_tables
     >>> print(list_tables('H1-LDAS_STRAIN-968654552-10.xml.gz'))
     ['process', 'process_params', 'sngl_burst', 'search_summary', 'segment_definer', 'segment_summary', 'segment']
     """  # noqa: E501
     return [tbl.TableName(tbl.Name) for tbl in iter_tables(source)]
 
 
 def to_table_type(val, cls, colname):
@@ -650,15 +650,15 @@
     Returns
     -------
     obj : `object`
         The input ``val`` cast to the correct type
 
     Examples
     --------
-    >>> from pdpy.io.ligolw import to_table_type as to_ligolw_type
+    >>> from pydischarge.io.ligolw import to_table_type as to_ligolw_type
     >>> from ligo.lw.lsctables import SnglBurstTable
     >>> x = to_ligolw_type(1.0, SnglBurstTable, 'central_freq'))
     >>> print(type(x), x)
     <class 'numpy.float32'> 1.0
     """
     from ligo.lw.types import (
         ToNumPyType as numpytypes,
```

### Comparing `pydischarge-0.0.1/pdpy/io/mp.py` & `pydischarge-0.0.2/pydischarge/io/mp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Multi-processing utilities for input/output
 
 This module provides the `read_multi` method, which enables spreading
 reading multiple files across multiple cores, returning a flattened result.
 """
 
@@ -101,15 +101,15 @@
     return flatten(out)
 
 
 def _read_single_file(bundle):
     """Reads a single file and returns the output
 
     This is designed only to be passed to
-    :func:`pdpy.utils.mp.multiprocess_with_queues`
+    :func:`pydischarge.utils.mp.multiprocess_with_queues`
 
     Returns
     -------
     f, output :
         the input file (object) that was (attempted to be) read, and
         the result of the read operation, which may be an exception
         object.
```

### Comparing `pydischarge-0.0.1/pdpy/io/nds2.py` & `pydischarge-0.0.2/pydischarge/io/nds2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Wrapper to the nds2-client package, providing network access
 to LIGO data.
 """
 
 import enum
 import operator
@@ -186,17 +186,17 @@
 
 # -- query utilities ----------------------------------------------------------
 
 def _get_nds2_name(channel):
     """Returns the NDS2-formatted name for a channel
 
     Understands how to format NDS name strings from
-    `pdpy.detector.Channel` and `nds2.channel` objects
+    `pydischarge.detector.Channel` and `nds2.channel` objects
     """
-    if hasattr(channel, 'ndsname'):  # pdpy.detector.Channel
+    if hasattr(channel, 'ndsname'):  # pydischarge.detector.Channel
         return channel.ndsname
     if hasattr(channel, 'channel_type'):  # nds2.channel
         return ",".join((
             channel.name,
             channel.channel_type_to_string(channel.channel_type),
         ))
     return str(channel)
@@ -249,15 +249,15 @@
     ifo : `str`
         prefix for IFO of interest
     env : `str`, optional
         environment variable name to use for server order,
         default ``'NDSSERVER'``. The contents of this variable should
         be a comma-separated list of `host:port` strings, e.g.
         ``'nds1.server.com:80,nds2.server.com:80'``
-    epoch : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+    epoch : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
         GPS epoch of data requested
     lookback : `float`
         duration of spinning-disk cache. This value triggers defaulting to
         the CIT NDS2 server over those at the LIGO sites
 
     Returns
     -------
@@ -445,15 +445,15 @@
     See also
     --------
     nds2.connection.find_channels
         for documentation on the underlying query method
 
     Examples
     --------
-    >>> from pdpy.io.nds2 import find_channels
+    >>> from pydischarge.io.nds2 import find_channels
     >>> find_channels(['G1:DER_DATA_H'], host='nds.ligo.caltech.edu')
     [<G1:DER_DATA_H (16384Hz, RDS, FLOAT64)>]
     """
     # set epoch
     if not isinstance(epoch, tuple):
         epoch = (epoch or 'ALL',)
     connection.set_epoch(*epoch)
@@ -579,15 +579,15 @@
         given
 
     port : `int`, optional
         port number on host to use for NDS2 connection
 
     Returns
     -------
-    segdict : `~pdpy.segments.SegmentListDict`
+    segdict : `~pydischarge.segments.SegmentListDict`
         dict of ``(name, SegmentList)`` pairs
 
     Raises
     ------
     ValueError
         if the given channel name cannot be mapped uniquely to a name
         in the NDS server database.
```

### Comparing `pydischarge-0.0.1/pdpy/io/registry.py` & `pydischarge-0.0.2/pydischarge/io/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """I/O registry extensions on top of `astropy.io.registry`
 
 This module imports a subset of the useful functions from
 :mod:`astropy.io.registry` for convenience.
 """
```

### Comparing `pydischarge-0.0.1/pdpy/io/tests/__init__.py` & `pydischarge-0.0.2/pydischarge/table/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.io`
+"""Tests for :mod:`pydischarge.table`
 """
```

### Comparing `pydischarge-0.0.1/pdpy/io/tests/test_cache.py` & `pydischarge-0.0.2/pydischarge/io/tests/test_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Unit test for `io` module
 """
 
 import os.path
 import tempfile
 from copy import deepcopy
@@ -137,30 +137,30 @@
         numpy.savetxt(f, a)
         f.seek(0)
         assert io_cache.is_cache(f) is False
 
 
 @pytest.mark.requires("lal.utils")
 def test_is_cache_file(tmp_path):
-    """Check that `pdpy.io.cache.is_cache` returns `True` when it should
+    """Check that `pydischarge.io.cache.is_cache` returns `True` when it should
     """
     # write a cache file
     e = io_cache.CacheEntry.from_T050017('/tmp/A-B-12345-6.txt')
     tmp = tmp_path / "tmpfile"
     io_cache.write_cache([e], tmp)
 
     # check that we can identify it properly
     assert io_cache.is_cache(tmp)  # file name
     with tmp.open("r") as tmpf:
         assert io_cache.is_cache(tmpf)  # open file object
 
 
 @pytest.mark.requires("lal.utils")
 def test_is_cache_file_empty(tmp_path):
-    """Check that `pdpy.io.cache.is_cache` returns False when it should
+    """Check that `pydischarge.io.cache.is_cache` returns False when it should
     """
     tmp = tmp_path / "tmpfile"
     assert not io_cache.is_cache(tmp)  # FileNotFoundError
     tmp.touch()
     assert not io_cache.is_cache(tmp)  # empty file
 
 
@@ -172,15 +172,15 @@
     except AttributeError:
         pass
     else:
         assert io_cache.is_cache_entry(e)
 
 
 def test_cache_segments(cache, segments):
-    """Test :func:`pdpy.io.cache.cache_segments`
+    """Test :func:`pydischarge.io.cache.cache_segments`
     """
     # check empty input
     sl = io_cache.cache_segments()
     assert isinstance(sl, SegmentList)
     assert len(sl) == 0
 
     # check simple cache
@@ -194,15 +194,15 @@
 
 
 @pytest.mark.parametrize("path, metadata", [
     ("A-B-0-1.txt", ('A', 'B', Segment(0, 1))),
     ("/path/to/A-B-0.456-1.345.txt.gz", ("A", "B", Segment(0.456, 1.801))),
 ])
 def test_filename_metadata(path, metadata):
-    """Test :func:`pdpy.io.cache.filename_metadata`
+    """Test :func:`pydischarge.io.cache.filename_metadata`
     """
     assert io_cache.filename_metadata(path) == metadata
 
 
 def test_filename_metadata_error():
     with pytest.raises(ValueError):
         io_cache.filename_metadata("A-B-0-4xml.gz")
@@ -213,53 +213,53 @@
     ("A-B-1-2.ext", Segment(1, 3)),
     # multiple file extensions
     ("A-B-1-2.ext.gz", Segment(1, 3)),
     # non-integer
     ("A-B-1.23-4.ext.gz", Segment(1.23, 5.23)),
 ])
 def test_file_segment(filename, seg):
-    """Test :func:`pdpy.io.cache.file_segment`
+    """Test :func:`pydischarge.io.cache.file_segment`
     """
     fs = io_cache.file_segment(filename)
     assert isinstance(fs, Segment)
     assert fs == seg
 
     # check mutliple file extensions
     assert io_cache.file_segment('A-B-1-2.ext.gz') == (1, 3)
 
     # check floats (and multiple file extensions)
     assert io_cache.file_segment('A-B-1.23-4.ext.gz') == (1.23, 5.23)
 
 
 def test_file_segment_errors():
-    """Test :func:`pdpy.io.cache.file_segment` error handling.
+    """Test :func:`pydischarge.io.cache.file_segment` error handling.
     """
     with pytest.raises(
         ValueError,
         match="^Failed to parse 'blah' as a LIGO-T050017-compatible filename$"
     ):
         io_cache.file_segment('blah')
 
 
 def test_flatten(cache):
-    """Test :func:`pdpy.io.cache.flatten`
+    """Test :func:`pydischarge.io.cache.flatten`
     """
     # check flattened version of single cache is unchanged
     assert io_cache.flatten(cache) == cache
     assert io_cache.flatten(cache, cache) == cache
 
     # check two caches get concatenated properly
     a = cache
     b = [e.replace('A-B-', 'A-B-1') for e in cache]
     c = a + b
     assert io_cache.flatten(a, b) == c
 
 
 def test_find_contiguous(cache, segments):
-    """Test :func:`pdpy.io.cache.find_contiguous`
+    """Test :func:`pydischarge.io.cache.find_contiguous`
     """
     for i, cache in enumerate(io_cache.find_contiguous(cache)):
         io_cache.cache_segments(cache).extent() == segments[i]
 
     assert not list(io_cache.find_contiguous())
```

### Comparing `pydischarge-0.0.1/pdpy/io/tests/test_datafind.py` & `pydischarge-0.0.2/pydischarge/io/tests/test_datafind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.io.datafind`
+"""Unit tests for :mod:`pydischarge.io.datafind`
 """
 
 import os
 from unittest import mock
 
 import pytest
 
@@ -33,15 +33,15 @@
 from ...testing.utils import (
     TEST_GWF_FILE,
 )
 from .. import datafind as io_datafind
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
-GWDATAFIND_PATH = "pdpy.io.datafind.gwdatafind"
+GWDATAFIND_PATH = "pydischarge.io.datafind.gwdatafind"
 MOCK_ENV = {
     'VIRGODATA': 'tmp',
     'GWDATAFIND_SERVER': 'test:80',
 }
 
 
 def _mock_gwdatafind(func):
@@ -59,19 +59,19 @@
         mock.MagicMock(return_value=[TEST_GWF_FILE]),
     )
     @mock.patch(
         f"{GWDATAFIND_PATH}.find_latest",
         mock.MagicMock(return_value=[TEST_GWF_FILE]),
     )
     @mock.patch(
-        'pdpy.io.datafind.iter_channel_names',
+        'pydischarge.io.datafind.iter_channel_names',
         mock.MagicMock(return_value=['L1:LDAS-STRAIN', 'H1:LDAS-STRAIN']),
     )
     @mock.patch(
-        'pdpy.io.datafind.num_channels',
+        'pydischarge.io.datafind.num_channels',
         mock.MagicMock(return_value=1),
     )
     def wrapper(*args, **kwargs):
         return func(*args, **kwargs)
 
     return wrapper
 
@@ -181,15 +181,15 @@
 
 @_mock_gwdatafind
 def test_find_frametype_error_files_on_tape():
     """Test that `find_frametype` raises the right error when the only
     discovered data are on tape, and we asked for not on tape.
     """
     # check that allow_tape errors get handled properly
-    patch = mock.patch('pdpy.io.datafind.on_tape', return_value=True)
+    patch = mock.patch('pydischarge.io.datafind.on_tape', return_value=True)
     raises = pytest.raises(
         ValueError,
         match=r"\[files on tape have not been checked",
     )
     with patch, raises:
         io_datafind.find_frametype('X1:TEST', allow_tape=False)
```

### Comparing `pydischarge-0.0.1/pdpy/io/tests/test_ffldatafind.py` & `pydischarge-0.0.2/pydischarge/io/tests/test_ffldatafind.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Cardiff University (2022)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.io.ffldatafind`
+"""Unit tests for :mod:`pydischarge.io.ffldatafind`
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
 
 import os
 from contextlib import nullcontext
 from pathlib import Path
@@ -206,29 +206,29 @@
         assert ffldatafind.find_latest(
             "BAD",
             "BAD",
             on_missing=on_missing,
         ) == []
 
 
-# -- test pdpy.io.datafind interface
+# -- test pydischarge.io.datafind interface
 
 @mock.patch(
-    "pdpy.io.datafind.iter_channel_names",
+    "pydischarge.io.datafind.iter_channel_names",
     mock.MagicMock(return_value=["Y1:TEST-CHANNEL"]),
 )
 @mock.patch(
-    "pdpy.io.datafind.on_tape",
+    "pydischarge.io.datafind.on_tape",
     mock.MagicMock(return_value=False),
 )
 @mock.patch(
-    'pdpy.io.datafind.num_channels',
+    'pydischarge.io.datafind.num_channels',
     mock.MagicMock(return_value=1),
 )
 def test_datafind_find_frametype():
-    """Test that pdpy.io.datafind.find_frametype ends up calling out
+    """Test that pydischarge.io.datafind.find_frametype ends up calling out
     to ffldatafind under the right circumstances.
     """
     assert io_datafind.find_frametype(
         "Y1:TEST-CHANNEL",
         allow_tape=True,
     ) == "test3"
```

### Comparing `pydischarge-0.0.1/pdpy/io/tests/test_gwf.py` & `pydischarge-0.0.2/pydischarge/io/tests/test_gwf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.io.gwf`
+"""Unit tests for :mod:`pydischarge.io.gwf`
 """
 
 import pytest
 
 from ...testing.utils import (
     TEST_GWF_FILE,
     assert_segmentlist_equal,
```

### Comparing `pydischarge-0.0.1/pdpy/io/tests/test_kerberos.py` & `pydischarge-0.0.2/pydischarge/io/tests/test_kerberos.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.io.kerberos`
+"""Unit tests for :mod:`pydischarge.io.kerberos`
 """
 
 import os
 import subprocess
 from unittest import mock
 
 import pytest
@@ -55,15 +55,15 @@
 def teardown_module():
     if MOCK_ENV is not None:
         MOCK_ENV.stop()
 
 
 @mock.patch('subprocess.check_output', return_value=KLIST)
 def test_parse_keytab(check_output):
-    """Test `pdpy.io.kerberos.parse_keytab.
+    """Test `pydischarge.io.kerberos.parse_keytab.
     """
     # assert principals get extracted correctly
     principals = io_kerberos.parse_keytab('test.keytab')
     assert principals == [('albert.einstein', 'LIGO.ORG', 1),
                           ('ronald.drever', 'LIGO.ORG', 2)]
 
 
@@ -72,27 +72,27 @@
     (OSError, "^Failed to locate klist, cannot read keytab$"),
     (
         subprocess.CalledProcessError(1, "error"),
         "Cannot read keytab 'test.keytab'",
     ),
 ])
 def test_parse_keytab_oserror(mock_check_output, se, match):
-    """Test `pdpy.io.kerberos.parse_keytab` fails appropriately.
+    """Test `pydischarge.io.kerberos.parse_keytab` fails appropriately.
     """
     mock_check_output.side_effect = se
     with pytest.raises(io_kerberos.KerberosError, match=match):
         io_kerberos.parse_keytab('test.keytab')
 
 
 @mock.patch('sys.stdout.isatty', return_value=True)
-@mock.patch('pdpy.io.kerberos.input', return_value='rainer.weiss')
+@mock.patch('pydischarge.io.kerberos.input', return_value='rainer.weiss')
 @mock.patch('getpass.getpass', return_value='test')
 @mock.patch('subprocess.Popen')
 def test_kinit_up(popen, getpass, input_, _, capsys):
-    """Test `pdpy.io.kerberos.kinit` with username and password given
+    """Test `pydischarge.io.kerberos.kinit` with username and password given
     """
     proc = popen.return_value
     proc.poll.return_value = 0
 
     # basic call should prompt for username and password
     io_kerberos.kinit()
     input_.assert_called_with(
@@ -106,19 +106,19 @@
         stdin=-1,
         stdout=-1,
         env=None,
     )
     proc.communicate.aossert_called_with(b'test')
 
 
-@mock.patch('pdpy.io.kerberos.input')
+@mock.patch('pydischarge.io.kerberos.input')
 @mock.patch('getpass.getpass')
 @mock.patch('subprocess.Popen')
 def test_kinit_up_kwargs(popen, getpass, input_):
-    """Test `pdpy.io.kerberos.kinit` with username and password given
+    """Test `pydischarge.io.kerberos.kinit` with username and password given
     """
     proc = popen.return_value
     proc.poll.return_value = 0
 
     io_kerberos.kinit(
         username='albert.einstein',
         password='test',
@@ -131,18 +131,18 @@
         stdin=-1,
         stdout=-1,
         env=None,
     )
     popen.return_value.communicate.assert_called_with(b'test')
 
 
-@mock.patch('pdpy.io.kerberos.parse_keytab')
+@mock.patch('pydischarge.io.kerberos.parse_keytab')
 @mock.patch('subprocess.Popen')
 def test_kinit_keytab_dne(popen, parse_keytab):
-    """Test `pdpy.io.kerberos.kinit` with a non-existent keytab
+    """Test `pydischarge.io.kerberos.kinit` with a non-existent keytab
     """
     proc = popen.return_value
     proc.poll.return_value = 0
 
     # test keytab from environment not found (default) prompts user
     io_kerberos.kinit(username='test', password='passwd',
                       exe='/bin/kinit')
@@ -154,20 +154,20 @@
         env=None,
     )
 
 
 @mock.patch.dict(os.environ, {'KRB5_KTNAME': '/test.keytab'})
 @mock.patch('os.path.isfile', return_value=True)
 @mock.patch(
-    'pdpy.io.kerberos.parse_keytab',
+    'pydischarge.io.kerberos.parse_keytab',
     return_value=[['rainer.weiss', 'LIGO.ORG']],
 )
 @mock.patch('subprocess.Popen')
 def test_kinit_keytab(popen, *unused_mocks):
-    """Test `pdpy.io.kerberos.kinit` can handle keytabs properly
+    """Test `pydischarge.io.kerberos.kinit` can handle keytabs properly
     """
     proc = popen.return_value
     proc.poll.return_value = 0
 
     # test keytab kwarg
     io_kerberos.kinit(keytab='test.keytab', exe='/bin/kinit')
     popen.assert_called_with(
@@ -185,15 +185,15 @@
         stdout=-1,
         env=None,
     )
 
 
 @mock.patch('subprocess.Popen')
 def test_kinit_krb5ccname(popen):
-    """Test `pdpy.io.kerberos.kinit` passes `KRB5CCNAME` to /bin/kinit
+    """Test `pydischarge.io.kerberos.kinit` passes `KRB5CCNAME` to /bin/kinit
     """
     # test using krb5ccname (credentials cache)
     # this will raise error because we haven't patched the poll() method
     # to return 0, but will test that we get the right error
     with pytest.raises(subprocess.CalledProcessError):
         io_kerberos.kinit(username='test', password='test',
                           krb5ccname='/test_cc.krb5', exe='/bin/kinit')
@@ -202,15 +202,15 @@
         stdin=-1,
         stdout=-1,
         env={'KRB5CCNAME': '/test_cc.krb5'},
     )
 
 
 def test_kinit_notty():
-    """Test `pdpy.io.kerberos.kinit` raises an error in a non-interactive
+    """Test `pydischarge.io.kerberos.kinit` raises an error in a non-interactive
     session if it needs to prompt for information.
 
     By default all tests are executed by pytest in a non-interactive session
     so we don't have to mock anything!
     """
     with pytest.raises(io_kerberos.KerberosError):
         io_kerberos.kinit(exe='/bin/kinit')
```

### Comparing `pydischarge-0.0.1/pdpy/io/tests/test_ligolw.py` & `pydischarge-0.0.2/pydischarge/io/tests/test_ligolw.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit test for `pdpy.io.ligolw` module
+"""Unit test for `pydischarge.io.ligolw` module
 """
 
 import tempfile
 from pathlib import Path
 
 import pytest
 
@@ -132,15 +132,15 @@
     with open(xmlpath, "w") as f:
         f.write(OLD_FORMAT_LIGO_LW_XML)
     tab = io_ligolw.read_table(xmlpath, tablename="sngl_burst")
     assert len(tab) == 3
 
 
 def test_read_table_multiple(llwdoc_with_tables):
-    """Check that `pdpy.io.ligolw.read_table` correctly errors on ambiguity.
+    """Check that `pydischarge.io.ligolw.read_table` correctly errors on ambiguity.
     """
     with pytest.raises(
         ValueError,
         match="^Multiple tables .* 'process', 'sngl_ringdown'",
     ):
         io_ligolw.read_table(llwdoc_with_tables)
 
@@ -255,15 +255,15 @@
     stab = new_table(
         'segment',
         [{'segment': (1, 2)}, {'segment': (3, 4)}, {'segment': (5, 6)}],
         columns=('start_time', 'start_time_ns', 'end_time', 'end_time_ns'),
     )
     ptab = new_table(
         'process',
-        [{'program': 'pdpy'}],
+        [{'program': 'pydischarge'}],
         columns=('program',),
     )
 
     tmp = tmp_path / "test.xml"
 
     # write writing works
     io_ligolw.write_tables(tmp, [stab, ptab])
```

### Comparing `pydischarge-0.0.1/pdpy/io/tests/test_mp.py` & `pydischarge-0.0.2/pydischarge/io/tests/test_mp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2019-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.io.mp`
+"""Unit tests for :mod:`pydischarge.io.mp`
 """
 
 import pytest
 
 from astropy.table import (Table, vstack)
 
 from ...testing.utils import assert_table_equal
```

### Comparing `pydischarge-0.0.1/pdpy/io/tests/test_nds2.py` & `pydischarge-0.0.2/pydischarge/io/tests/test_nds2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.io.nds2`
+"""Unit tests for :mod:`pydischarge.io.nds2`
 """
 
 import os
 from unittest import mock
 
 import pytest
 
@@ -36,25 +36,25 @@
 class _TestNds2Enum(object):
     TEST_CLASS = None
 
     def test_any(self):
         assert self.TEST_CLASS.any() == 2 * max(self.TEST_CLASS).value - 1
 
     def test_find_errors(self):
-        """Test error raising for :meth:`pdpy.io.nds2.Nds2ChannelType.find`
+        """Test error raising for :meth:`pydischarge.io.nds2.Nds2ChannelType.find`
         """
         with pytest.raises(
             ValueError,
             match=f"'blah' is not a valid {self.TEST_CLASS.__name__}",
         ):
             self.TEST_CLASS.find('blah')
 
 
 class TestNds2ChannelType(_TestNds2Enum):
-    """Tests of :class:`pdpy.io.nds2.Nds2DataType`
+    """Tests of :class:`pydischarge.io.nds2.Nds2DataType`
     """
     TEST_CLASS = io_nds2.Nds2ChannelType
 
     def test_nds2name(self):
         assert self.TEST_CLASS.MTREND.nds2name == 'm-trend'
 
     def test_nds2names(self):
@@ -71,21 +71,21 @@
         ('mtrend', TEST_CLASS.MTREND),
         ('rds', TEST_CLASS.RDS),
         ('RDS', TEST_CLASS.RDS),
         ('reduced', TEST_CLASS.RDS),
         ('REDUCED', TEST_CLASS.RDS),
     ))
     def test_find(self, input_, expected):
-        """Test :meth:`pdpy.io.nds2.Nds2ChannelType.find`
+        """Test :meth:`pydischarge.io.nds2.Nds2ChannelType.find`
         """
         assert self.TEST_CLASS.find(input_) == expected
 
 
 class TestNds2DataType(_TestNds2Enum, _TestNumpyTypeEnum):
-    """Tests of :class:`pdpy.io.nds2.Nds2DataType`
+    """Tests of :class:`pydischarge.io.nds2.Nds2DataType`
     """
     TEST_CLASS = io_nds2.Nds2DataType
 
 
 @pytest.mark.parametrize('key, value, hosts', [
     ('NDSSERVER',
      'test1.ligo.org:80,test2.ligo.org:43',
@@ -95,50 +95,50 @@
      [('test1.ligo.org', 80), ('test2.ligo.org', 43),
       ('test.ligo.org', None)]),
     ('TESTENV',
      'test1.ligo.org:80,test2.ligo.org:43',
      [('test1.ligo.org', 80), ('test2.ligo.org', 43)]),
 ])
 def test_parse_nds_env(key, value, hosts):
-    """Test `pdpy.io.nds2.parse_nds_env`
+    """Test `pydischarge.io.nds2.parse_nds_env`
     """
     with mock.patch.dict(os.environ, {key: value}):
         assert io_nds2.parse_nds_env(env=key) == hosts
 
 
 @pytest.mark.parametrize('ifo, hosts', [
     (None, [('nds.ligo.caltech.edu', 31200)]),
     ('L1', [('nds.ligo-la.caltech.edu', 31200),
             ('nds.ligo.caltech.edu', 31200)]),
 ])
 def test_host_resolution_order(ifo, hosts):
-    """Test `pdpy.io.nds2.host_resolution_order` basic usage
+    """Test `pydischarge.io.nds2.host_resolution_order` basic usage
     """
     assert io_nds2.host_resolution_order(ifo, env=None) == hosts
 
 
 @mock.patch.dict(os.environ,
                  {'NDSSERVER': 'test1.ligo.org:80,test2.ligo.org:43'})
 @pytest.mark.parametrize('ifo, hosts', [
     (None, [('test1.ligo.org', 80), ('test2.ligo.org', 43),
             ('nds.ligo.caltech.edu', 31200)]),
     ('L1', [('test1.ligo.org', 80), ('test2.ligo.org', 43),
             ('nds.ligo-la.caltech.edu', 31200),
             ('nds.ligo.caltech.edu', 31200)]),
 ])
 def test_host_resolution_order_env(ifo, hosts):
-    """Test `pdpy.io.nds2.host_resolution_order` environment parsing
+    """Test `pydischarge.io.nds2.host_resolution_order` environment parsing
     """
     assert io_nds2.host_resolution_order(ifo) == hosts
 
 
 @mock.patch.dict(os.environ,
                  {'TESTENV': 'test1.ligo.org:80,test2.ligo.org:43'})
 def test_host_resolution_order_named_env():
-    """Test `pdpy.io.nds2.host_resolution_order` environment parsing
+    """Test `pydischarge.io.nds2.host_resolution_order` environment parsing
     with a named environment variable
     """
     hro = io_nds2.host_resolution_order(None, env='TESTENV')
     assert hro == [('test1.ligo.org', 80), ('test2.ligo.org', 43),
                    ('nds.ligo.caltech.edu', 31200)]
 
 
@@ -148,93 +148,93 @@
     ('L1', 'Jan 1 2015', None,
      [('nds.ligo.caltech.edu', 31200), ('nds.ligo-la.caltech.edu', 31200)]),
     ('L1', 'now', 'TESTENV',
      [('test1.ligo.org', 80), ('test2.ligo.org', 43),
       ('nds.ligo-la.caltech.edu', 31200), ('nds.ligo.caltech.edu', 31200)]),
 ])
 def test_host_resolution_order_epoch(ifo, epoch, env, hosts):
-    """Test `pdpy.io.nds2.host_resolution_order` epoch parsing
+    """Test `pydischarge.io.nds2.host_resolution_order` epoch parsing
     """
     assert io_nds2.host_resolution_order(ifo, epoch=epoch, env=env) == hosts
 
 
 @mock.patch.dict(os.environ,
                  {'TESTENV': 'test1.ligo.org:80,test2.ligo.org:43'})
 def test_host_resolution_order_warning():
-    """Test `pdpy.io.nds2.host_resolution_order` warnings
+    """Test `pydischarge.io.nds2.host_resolution_order` warnings
     """
     # test warnings for unknown IFO
     with pytest.warns(UserWarning) as record:
         # should produce warning
         hro = io_nds2.host_resolution_order('X1', env=None)
         assert hro == [('nds.ligo.caltech.edu', 31200)]
         # should _not_ produce warning
         hro = io_nds2.host_resolution_order('X1', env='TESTENV')
     assert len(record) == 1  # make sure only one warning was emitted
 
 
 @pytest.mark.requires("nds2")
 @pytest.mark.parametrize('host, port, callport', [
-    ('nds.test.pdpy', None, None),
-    ('nds.test.pdpy', 31200, 31200),
+    ('nds.test.pydischarge', None, None),
+    ('nds.test.pydischarge', 31200, 31200),
     ('x1nds9', None, 8088),
 ])
 @mock.patch('nds2.connection')
 def test_connect(connector, host, port, callport):
-    """Test `pdpy.io.nds2.connect`
+    """Test `pydischarge.io.nds2.connect`
     """
     io_nds2.connect(host, port=port)
     if callport is None:
         connector.assert_called_once_with(host)
     else:
         connector.assert_called_once_with(host, callport)
 
 
 @pytest.mark.requires("nds2")
-@mock.patch('pdpy.io.nds2.connect')
+@mock.patch('pydischarge.io.nds2.connect')
 def test_auth_connect(connect):
-    """Test `pdpy.io.nds2.auth_connect`
+    """Test `pydischarge.io.nds2.auth_connect`
     """
     io_nds2.auth_connect('host', 'port')
     connect.assert_called_once_with('host', 'port')
 
 
 @pytest.mark.requires("nds2")
-@mock.patch('pdpy.io.nds2.kinit')
+@mock.patch('pydischarge.io.nds2.kinit')
 @mock.patch(
-    'pdpy.io.nds2.connect',
+    'pydischarge.io.nds2.connect',
     side_effect=(
         RuntimeError('Request SASL authentication something something'),
         True,
     ),
 )
 def test_auth_connect_kinit(connect, kinit):
-    """Test `pdpy.io.nds2.auth_connect` with a callout to
-    `pdpy.io.kerberos.kinit`
+    """Test `pydischarge.io.nds2.auth_connect` with a callout to
+    `pydischarge.io.kerberos.kinit`
     """
     with pytest.warns(io_nds2.NDSWarning):
         assert io_nds2.auth_connect('host', 'port')
     kinit.assert_called_with()
     assert connect.call_count == 2
     connect.assert_called_with('host', 'port')
 
 
 @pytest.mark.requires("nds2")
-@mock.patch('pdpy.io.nds2.connect', side_effect=RuntimeError('Anything else'))
+@mock.patch('pydischarge.io.nds2.connect', side_effect=RuntimeError('Anything else'))
 def test_auth_connect_error(connect):
-    """Test errors from `pdpy.io.nds2.auth_connect`
+    """Test errors from `pydischarge.io.nds2.auth_connect`
     """
     with pytest.raises(RuntimeError, match="Anything else"):
         io_nds2.auth_connect('host', 'port')
     connect.assert_called_once_with("host", "port")
 
 
-@mock.patch('pdpy.io.nds2.auth_connect', return_value=1)
+@mock.patch('pydischarge.io.nds2.auth_connect', return_value=1)
 def test_open_connection(auth_connect):
-    """Test the `pdpy.io.nds2.open_connection` decorator
+    """Test the `pydischarge.io.nds2.open_connection` decorator
     """
     @io_nds2.open_connection
     def new_func(arg1, connection=None):
         return arg1, connection
 
     with pytest.raises(TypeError):
         new_func(0)
@@ -244,15 +244,15 @@
     # check that auth_connect was called with the right arguments
     auth_connect.assert_called_once_with('test', None)
 
 
 @pytest.mark.requires("nds2")
 @mock.patch('nds2.connection')
 def test_find_channels(connection):
-    """Test `pdpy.io.nds2.find_channels`
+    """Test `pydischarge.io.nds2.find_channels`
     """
     # set up connection.find_channels
     chan = mocks.nds2_channel('X1:test', 16, 'm')
     conn = mock.MagicMock()
     connection.return_value = conn
     conn.find_channels.return_value = [chan]
 
@@ -294,18 +294,18 @@
         ValueError,
         match="^unique NDS2 channel match not found for 'X1:test'$",
     ):
         io_nds2.find_channels(['X1:test'], host='test', unique=True)
 
 
 @pytest.mark.requires("nds2")
-@mock.patch('pdpy.io.nds2.find_channels', return_value=['X1:test'])
-@mock.patch('pdpy.io.nds2.auth_connect')
+@mock.patch('pydischarge.io.nds2.find_channels', return_value=['X1:test'])
+@mock.patch('pydischarge.io.nds2.auth_connect')
 def test_get_availability(auth_connect, _):
-    """Test `pdpy.io.nds2.get_availability`
+    """Test `pydischarge.io.nds2.get_availability`
     """
     # setup mocks
     conn = mock.MagicMock()
     auth_connect.return_value = conn
     conn.get_availability.return_value = [
         mocks.nds2_availability('X1:test', [(0, 1), (2, 3)]),
     ]
@@ -330,35 +330,35 @@
     (0, 60, (0, 60)),  # no change
     (1, 60, (0, 60)),  # expand at start
     (0, 61, (0, 120)),  # expand at end
     (59, 61, (0, 120)),  # expand both
     (1167264018, 1198800018, (1167264000, 1198800060)),  # expand both
 ])
 def test_minute_trend_times(start, end, out):
-    """Test `pdpy.io.nds2.minute_trend_times`
+    """Test `pydischarge.io.nds2.minute_trend_times`
     """
     assert io_nds2.minute_trend_times(start, end) == out
 
 
 @pytest.mark.requires("nds2")
 def test_get_nds2_name():
-    """Test `pdpy.io.nds2._get_nds2_name`
+    """Test `pydischarge.io.nds2._get_nds2_name`
     """
     # we can't use parametrize because mocks.nds2_channel requires
     # the nds2-client and is executed _before_ the skip decorator is
     # applied
     for channel, name in [
         ('test', 'test'),
         (Channel('X1:TEST', type='m-trend'), 'X1:TEST,m-trend'),
         (mocks.nds2_channel('X1:TEST', 16, 'NONE'), 'X1:TEST,raw'),
     ]:
         assert io_nds2._get_nds2_name(channel) == name
 
 
 @pytest.mark.requires("nds2")
 def test_get_nds2_names():
-    """Test `pdpy.io.nds2._get_nds2_names`
+    """Test `pydischarge.io.nds2._get_nds2_names`
     """
     channels = ['test', Channel('X1:TEST', type='m-trend'),
                 mocks.nds2_channel('X1:TEST', 16, 'NONE')]
     names = ['test', 'X1:TEST,m-trend', 'X1:TEST,raw']
     assert list(io_nds2._get_nds2_names(channels)) == names
```

### Comparing `pydischarge-0.0.1/pdpy/io/tests/test_utils.py` & `pydischarge-0.0.2/pydischarge/io/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.io.utils`
+"""Unit tests for :mod:`pydischarge.io.utils`
 """
 
 import gzip
 import tempfile
 from pathlib import Path
 
 import pytest
@@ -106,26 +106,26 @@
     (Path("test.txt"), "test.txt"),
 ))
 def test_file_path(input_, expected):
     assert io_utils.file_path(input_) == expected
 
 
 def test_file_path_file():
-    """Check that :func:`pdpy.io.utils.file_path` can handle open files
+    """Check that :func:`pydischarge.io.utils.file_path` can handle open files
     """
     with tempfile.NamedTemporaryFile() as f:
         assert io_utils.file_path(f) == f.name
 
 
 @pytest.mark.parametrize("badthing", (
     1,
     ["test.txt"],
 ))
 def test_file_path_errors(badthing):
-    """Check that :func:`pdpy.io.utils.file_path` fails when expected
+    """Check that :func:`pydischarge.io.utils.file_path` fails when expected
     """
     with pytest.raises(
         ValueError,
         match="^Cannot parse file name for ",
     ):
         io_utils.file_path(badthing)
```

### Comparing `pydischarge-0.0.1/pdpy/io/utils.py` & `pydischarge-0.0.2/pydischarge/io/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utilities for unified input/output
 """
 
 import gzip
 import os
 import tempfile
@@ -222,15 +222,15 @@
     Raises
     ------
     ValueError
         if a file path cannnot be determined
 
     Examples
     --------
-    >>> from pdpy.io.utils import file_path
+    >>> from pydischarge.io.utils import file_path
     >>> import pathlib
     >>> file_path("test.txt")
     'test.txt'
     >>> file_path(pathlib.Path('dir') / 'test.txt')
     'dir/test.txt'
     >>> file_path(open("test.txt", "r"))
     'test.txt'
```

### Comparing `pydischarge-0.0.1/pdpy/plot/__init__.py` & `pydischarge-0.0.2/pydischarge/plot/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module provides plotting utilities for visualising GW data
 
 The standard data types (`TimeSeries`, `Table`, `DataQualityFlag`, ...) can
 all be easily visualised using the relevant plotting objects, with
 many configurable parameters both interactive, and in saving to disk.
 """
```

### Comparing `pydischarge-0.0.1/pdpy/plot/axes.py` & `pydischarge-0.0.2/pydischarge/plot/axes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Cardiff University (2018-2022)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Extension of `~matplotlib.axes.Axes` for pdpy
+"""Extension of `~matplotlib.axes.Axes` for pydischarge
 """
 
 import warnings
 from functools import wraps
 from math import log
 from numbers import Number
 
@@ -45,26 +45,26 @@
 from .legend import HandlerLine2D
 from ..time import to_gps
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 
 def log_norm(func):
-    """Wrap ``func`` to handle custom pdpy keywords for a LogNorm colouring
+    """Wrap ``func`` to handle custom pydischarge keywords for a LogNorm colouring
     """
     @wraps(func)
     def decorated_func(*args, **kwargs):
         norm, kwargs = format_norm(kwargs)
         kwargs['norm'] = norm
         return func(*args, **kwargs)
     return decorated_func
 
 
 def xlim_as_gps(func):
-    """Wrap ``func`` to handle pass limit inputs through `pdpy.time.to_gps`
+    """Wrap ``func`` to handle pass limit inputs through `pydischarge.time.to_gps`
     """
     @wraps(func)
     def wrapped_func(self, left=None, right=None, **kw):
         if right is None and numpy.iterable(left):
             left, right = left
         kw['left'] = left
         kw['right'] = right
@@ -124,15 +124,15 @@
     """
     @wraps(func)
     def wrapped(self, *args, **kwargs):
         if "c_sort" in kwargs:
             warnings.warn(
                 f"the `c_sort` keyword for {func.__name__} was "
                 "renamed `sortbycolor`, this warning will result "
-                "in an error in future versions of PDpy",
+                "in an error in future versions of pyDischarge",
                 DeprecationWarning,
             )
             kwargs.setdefault(
                 "sortbycolor",
                 kwargs.pop("c_sort"),
             )
         return func(self, *args, **kwargs)
@@ -203,30 +203,30 @@
 
     set_xlim = xlim_as_gps(_Axes.set_xlim)
 
     def set_epoch(self, epoch):
         """Set the epoch for the current GPS scale.
 
         This method will fail if the current X-axis scale isn't one of
-        the GPS scales. See :ref:`pdpy-plot-gps` for more details.
+        the GPS scales. See :ref:`pydischarge-plot-gps` for more details.
 
         Parameters
         ----------
         epoch : `float`, `str`
             GPS-compatible time or date object, anything parseable by
-            :func:`~pdpy.time.to_gps` is fine.
+            :func:`~pydischarge.time.to_gps` is fine.
         """
         scale = self.get_xscale()
         return self.set_xscale(scale, epoch=epoch)
 
     def get_epoch(self):
         """Return the epoch for the current GPS scale/
 
         This method will fail if the current X-axis scale isn't one of
-        the GPS scales. See :ref:`pdpy-plot-gps` for more details.
+        the GPS scales. See :ref:`pydischarge-plot-gps` for more details.
         """
         return self.get_xaxis().get_transform().get_epoch()
 
     # -- overloaded plotting methods ------------
 
     @deprecate_c_sort
     def scatter(self, x, y, s=None, c=None, **kwargs):
@@ -254,16 +254,16 @@
         'marker :',
     )
 
     @log_norm
     def imshow(self, array, *args, **kwargs):
         """Display an image, i.e. data on a 2D regular raster.
 
-        If ``array`` is a :class:`~pdpy.types.Array2D` (e.g. a
-        :class:`~pdpy.spectrogram.Spectrogram`), then the defaults are
+        If ``array`` is a :class:`~pydischarge.types.Array2D` (e.g. a
+        :class:`~pydischarge.spectrogram.Spectrogram`), then the defaults are
         _different_ to those in the upstream
         :meth:`~matplotlib.axes.Axes.imshow` method. Namely, the defaults are
 
         - ``origin='lower'`` (coordinates start in lower-left corner)
         - ``aspect='auto'`` (pixels are not forced to be square)
         - ``interpolation='none'`` (no image interpolation is used)
 
@@ -289,15 +289,15 @@
 
         image = super().imshow(array, *args, **kwargs)
         self.autoscale(enable=None, axis='both', tight=None)
         return image
 
     def _imshow_array2d(self, array, origin='lower', interpolation='none',
                         aspect='auto', **kwargs):
-        """Render an `~pdpy.types.Array2D` using `Axes.imshow`
+        """Render an `~pydischarge.types.Array2D` using `Axes.imshow`
         """
         # NOTE: If you change the defaults for this method, please update
         #       the docstring for `imshow` above.
 
         # calculate extent
         extent = tuple(array.xspan) + tuple(array.yspan)
         if self.get_xscale() == 'log' and extent[0] == 0.:
@@ -310,16 +310,16 @@
                            interpolation=interpolation, **kwargs)
 
     @restore_grid
     @log_norm
     def pcolormesh(self, *args, **kwargs):
         """Create a pseudocolor plot with a non-regular rectangular grid.
 
-        When using PDpy, this method can be called with a single argument
-        that is an :class:`~pdpy.types.Array2D`, for which the ``X`` and ``Y``
+        When using pyDischarge, this method can be called with a single argument
+        that is an :class:`~pydischarge.types.Array2D`, for which the ``X`` and ``Y``
         coordinate arrays will be determined from the indexing.
 
         In all other usage, all ``args`` and ``kwargs`` are passed directly
         to :meth:`~matplotlib.axes.Axes.pcolormesh`.
 
         Notes
         -----
@@ -331,15 +331,15 @@
         matplotlib.axes.Axes.pcolormesh
         """
         if len(args) == 1 and hasattr(args[0], "yindex"):  # Array2D
             return self._pcolormesh_array2d(*args, **kwargs)
         return super().pcolormesh(*args, **kwargs)
 
     def _pcolormesh_array2d(self, array, *args, **kwargs):
-        """Render an `~pdpy.types.Array2D` using `Axes.pcolormesh`
+        """Render an `~pydischarge.types.Array2D` using `Axes.pcolormesh`
         """
         x = numpy.concatenate((array.xindex.value, array.xspan[-1:]))
         y = numpy.concatenate((array.yindex.value, array.yspan[-1:]))
         xcoord, ycoord = numpy.meshgrid(x, y, copy=False, sparse=True)
         return self.pcolormesh(xcoord, ycoord, array.value.T, *args, **kwargs)
 
     def hist(self, x, *args, **kwargs):
@@ -397,21 +397,21 @@
         `Series` are plotted lightly below and above, with a fill
         between them and the ``data``.
 
         All three `Series` should have the same `~Series.index` array.
 
         Parameters
         ----------
-        data : `~pdpy.types.Series`
+        data : `~pydischarge.types.Series`
             Data to plot normally.
 
-        lower : `~pdpy.types.Series`
+        lower : `~pydischarge.types.Series`
             Lower boundary (on Y-axis) for shade.
 
-        upper : `~pdpy.types.Series`
+        upper : `~pydischarge.types.Series`
             Upper boundary (on Y-axis) for shade.
 
         **kwargs
             Any other keyword arguments acceptable for
             :meth:`~matplotlib.Axes.plot`.
 
         Returns
@@ -492,15 +492,15 @@
         collection : `~matplotlib.collections.PolyCollection`
             the collection of tiles drawn
 
         Examples
         --------
         >>> import numpy
         >>> from matplotlib import pyplot
-        >>> import pdpy.plot  # to get pdpy's Axes
+        >>> import pydischarge.plot  # to get pydischarge's Axes
 
         >>> x = numpy.arange(10)
         >>> y = numpy.arange(x.size)
         >>> w = numpy.ones_like(x) * .8
         >>> h = numpy.ones_like(x) * .8
 
         >>> fig = pyplot.figure()
@@ -567,15 +567,15 @@
         "Call signatures",
         """.. note::
 
    This method uses a custom default legend handler for
    `~matplotlib.lines.Line2D` objects, with increased linewidth relative
    to the upstream :meth:`~matplotlib.axes.Axes.legend` method.
    To disable this, pass ``handler_map=None``, or create and pass your
-   own handler class.  See :ref:`pdpy-plot-legend` for more details.
+   own handler class.  See :ref:`pydischarge-plot-legend` for more details.
 
 Call signatures""",
     )
 
     def colorbar(self, mappable=None, **kwargs):
         """Add a `~matplotlib.colorbar.Colorbar` to these `Axes`
```

### Comparing `pydischarge-0.0.1/pdpy/plot/bode.py` & `pydischarge-0.0.2/pydischarge/plot/bode.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Definition of a BodePlot
 """
 
 from math import pi
 
 import numpy
@@ -54,24 +54,24 @@
 
 
 class BodePlot(Plot):
     """A `Plot` class for visualising transfer functions
 
     Parameters
     ----------
-    *filters : `~scipy.signal.lti`, `~pdpy.frequencyseries.FrequencySeries`
+    *filters : `~scipy.signal.lti`, `~pydischarge.frequencyseries.FrequencySeries`
         any number of the following:
 
         - linear time-invariant filters, either
           `~scipy.signal.lti` or `tuple` of the following length and form:
           - 2: (numerator, denominator)
           - 3: (zeros, poles, gain)
           - 4: (A, B, C, D)
 
-        - complex-valued `spectra <pdpy.frequencyseries.FrequencySeries>`
+        - complex-valued `spectra <pydischarge.frequencyseries.FrequencySeries>`
           representing a transfer function
 
     frequencies : `numpy.ndarray`, optional
         list of frequencies (in Hertz) at which to plot
 
     dB : `bool`, optional, default: `True`
         if `True`, display magnitude in decibels, otherwise display
@@ -191,15 +191,15 @@
 
         Returns
         -------
         mag, phase : `tuple` of `lines <matplotlib.lines.Line2D>`
             the lines drawn for the magnitude and phase of the filter.
         """
         from scipy.signal import (lti, dlti)
-        from pdpy.signal.filter_design import parse_filter
+        from pydischarge.signal.filter_design import parse_filter
 
         if not analog:
             if not sample_rate:
                 raise ValueError("Must give sample_rate frequency to display "
                                  "digital (analog=False) filter")
             sample_rate = Quantity(sample_rate, 'Hz').value
             dt = 2 * pi / sample_rate
@@ -227,15 +227,15 @@
         return mline, pline
 
     def add_frequencyseries(self, spectrum, dB=True, power=False, **kwargs):
         """Plot the magnitude and phase of a complex-valued `FrequencySeries`
 
         Parameters
         ----------
-        spectrum : `~pdpy.frequencyseries.FrequencySeries`
+        spectrum : `~pydischarge.frequencyseries.FrequencySeries`
             the (complex-valued) `FrequencySeries` to display
 
         db : `bool`, optional, default: `True`
             if `True`, display magnitude in decibels, otherwise display
             amplitude.
 
         power : `bool`, optional, default: `False`
```

### Comparing `pydischarge-0.0.1/pdpy/plot/colorbar.py` & `pydischarge-0.0.2/pydischarge/plot/colorbar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2017)
 #               Cardiff University (2017-2022)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utilities for generating colour bars for figures
 """
 
 from matplotlib.axes import SubplotBase
 from matplotlib.colors import LogNorm
 from matplotlib.legend import Legend
```

### Comparing `pydischarge-0.0.1/pdpy/plot/colors.py` & `pydischarge-0.0.2/pydischarge/plot/colors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2017)
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Colour customisations for visualisation in PDpy
+"""Colour customisations for visualisation in pyDischarge
 """
 
 import numpy
 
 from matplotlib import colors
 from matplotlib.colors import (_colors_full_map as color_map, to_rgb)
 
@@ -48,16 +48,16 @@
     'ligo-india': 'I1',
     'ligo-livingston': 'L1',
     'virgo': 'V1',
 }
 GW_OBSERVATORY_COLORS = {_GWO_PREFIX[n]: GWPY_COLORS[n] for n in GWPY_COLORS}
 
 # set named colour upstream in matplotlib, so users can specify as
-# e.g. plot(..., color='pdpy:ligo-hanford')
-color_map.update({f"pdpy:{name}": col for name, col in GWPY_COLORS.items()})
+# e.g. plot(..., color='pydischarge:ligo-hanford')
+color_map.update({f"pydischarge:{name}": col for name, col in GWPY_COLORS.items()})
 
 
 # -- colour utilities ---------------------------------------------------------
 
 def tint(col, factor=1.0):
     """Tint a color (make it darker), returning a new RGB array
     """
```

### Comparing `pydischarge-0.0.1/pdpy/plot/gps.py` & `pydischarge-0.0.2/pydischarge/plot/gps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module defines locators/formatters and a scale for GPS data.
 """
 
 from decimal import Decimal
 from numbers import Number
```

### Comparing `pydischarge-0.0.1/pdpy/plot/legend.py` & `pydischarge-0.0.2/pydischarge/plot/legend.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Cardiff University (2019-2022)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Extensions of `~matplotlib.legend` for pdpy
+"""Extensions of `~matplotlib.legend` for pydischarge
 """
 
 from matplotlib import legend_handler
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
```

### Comparing `pydischarge-0.0.1/pdpy/plot/log.py` & `pydischarge-0.0.2/pydischarge/plot/log.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module redefines the matplotlib log scale to give a more
 helpful set of major and minor ticks.
 """
 
 from math import (ceil, floor, isclose, log)
 
@@ -129,17 +129,17 @@
         if fmt:
             return _math(sign + fmt % x)
 
         return super().__call__(x, pos=pos)
 
 
 class LogScale(_LogScale):
-    """PDpy version of the matplotlib `LogScale`.
+    """pyDischarge version of the matplotlib `LogScale`.
 
-    This scale overrides the default to use the new PDpy formatters
+    This scale overrides the default to use the new pyDischarge formatters
     for major and minor ticks.
     """
     def set_default_locators_and_formatters(self, axis):
         axis.set_major_locator(mticker.LogLocator(self.base))
         axis.set_major_formatter(LogFormatter(self.base))
         axis.set_minor_locator(mticker.LogLocator(self.base, self.subs))
         axis.set_minor_formatter(
```

### Comparing `pydischarge-0.0.1/pdpy/plot/plot.py` & `pydischarge-0.0.2/pydischarge/plot/plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2022)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Extension of the basic matplotlib Figure for PDpy
+"""Extension of the basic matplotlib Figure for pyDischarge
 """
 
 import itertools
 import importlib
 from collections.abc import (KeysView, ValuesView)
 from itertools import zip_longest
 
@@ -68,15 +68,15 @@
     Returns
     -------
     backend_mod: `module`
         the module as returned by :func:`importlib.import_module`
 
     Examples
     --------
-    >>> from pdpy.plot.plot import get_backend_mod
+    >>> from pydischarge.plot.plot import get_backend_mod
     >>> print(get_backend_mod('agg'))
     <module 'matplotlib.backends.backend_agg' from ... >
     """
     if name is None:
         name = get_backend()
     backend_name = (
         name[9:] if name.startswith("module://")
@@ -85,15 +85,15 @@
     return importlib.import_module(backend_name)
 
 
 class Plot(figure.Figure):
     """An extension of the core matplotlib `~matplotlib.figure.Figure`
 
     The `Plot` provides a number of methods to simplify generating
-    figures from PDpy data objects, and modifying them on-the-fly in
+    figures from pyDischarge data objects, and modifying them on-the-fly in
     interactive mode.
     """
     def __init__(self, *data, **kwargs):
 
         # get default x-axis scale if all axes have the same x-axis units
         kwargs.setdefault('xscale', _parse_xscale(
             _group_axes_data(data, flat=True)))
@@ -398,15 +398,15 @@
         --------
         matplotlib.figure.Figure.colorbar
         matplotlib.colorbar.Colorbar
 
         Examples
         --------
         >>> import numpy
-        >>> from pdpy.plot import Plot
+        >>> from pydischarge.plot import Plot
 
         To plot a simple image and add a colorbar:
 
         >>> plot = Plot()
         >>> ax = plot.gca()
         >>> ax.imshow(numpy.random.randn(120).reshape((10, 12)))
         >>> plot.colorbar(label='Value')
@@ -426,15 +426,15 @@
             self, mappable, ax, cax=cax, fraction=fraction, **kwargs)
 
         # generate colour bar
         cbar = super().colorbar(mappable, **kwargs)
 
         # force the minor ticks to be the same as the major ticks
         # in practice, this normally swaps out LogFormatterSciNotation to
-        # pdpy's LogFormatter; # this is hacky, and would be improved using a
+        # pydischarge's LogFormatter; # this is hacky, and would be improved using a
         # subclass of Colorbar in the first place, but matplotlib's
         # cbar_factory doesn't support that
         longaxis = (cbar.ax.yaxis if cbar.orientation == "vertical" else
                     cbar.ax.xaxis)
         if (
                 isinstance(cbar.formatter, LogFormatter)
                 and isinstance(
@@ -466,15 +466,15 @@
 
         By default, segments are displayed in a thin horizontal set of Axes
         sitting immediately below the x-axis of the main,
         similarly to a colorbar.
 
         Parameters
         ----------
-        segments : `~pdpy.segments.DataQualityFlag`
+        segments : `~pydischarge.segments.DataQualityFlag`
             A data-quality flag, or `SegmentList` denoting state segments
             about this Plot
 
         ax : `Axes`, optional
             Specific `Axes` relative to which to position new `Axes`,
             defaults to :func:`~matplotlib.pyplot.gca()`
 
@@ -491,15 +491,15 @@
 
         location : `str`, optional
             Location for new segment axes, defaults to ``'bottom'``,
             acceptable values are ``'top'`` or ``'bottom'``.
 
         **plotargs
             extra keyword arguments are passed to
-            :meth:`~pdpy.plot.SegmentAxes.plot`
+            :meth:`~pydischarge.plot.SegmentAxes.plot`
         """
         # get axes to anchor against
         if not ax:
             ax = self.gca()
 
         # set options for new axes
         axes_kw = {
@@ -577,15 +577,15 @@
     - if a `list` of data arrays are given, and `separate=True`, use N `Axes,
       one for each data array
     - if a nested `list` of data arrays are given, ignore `sep` and
       use one `Axes` for each group of arrays.
 
     Examples
     --------
-    >>> from pdpy.plot import Plot
+    >>> from pydischarge.plot import Plot
     >>> Plot._group_axes_data([1, 2], separate=False)
     [[1, 2]]
     >>> Plot._group_axes_data([1, 2], separate=True)
     [[1], [2]]
     >>> Plot._group_axes_data([[1, 2], 3])
     [[1, 2], [3]]
     """
```

### Comparing `pydischarge-0.0.1/pdpy/plot/rc.py` & `pydischarge-0.0.2/pydischarge/plot/rc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Custom default figure configuration
 """
 
 from matplotlib import (rcParams, rc_params, RcParams)
 
 from . import tex
@@ -77,19 +77,19 @@
     'font.size': 16,
     # don't use mathtext for offset
     'axes.formatter.use_mathtext': False,
 })
 
 
 def rc_params(usetex=None):
-    """Returns a new `matplotlib.RcParams` with updated PDpy parameters
+    """Returns a new `matplotlib.RcParams` with updated pyDischarge parameters
 
     The updated parameters are globally stored as
-    `pdpy.plot.rc.GWPY_RCPARAMS`, with the updated TeX parameters as
-    `pdpy.plot.rc.GWPY_TEX_RCPARAMS`.
+    `pydischarge.plot.rc.GWPY_RCPARAMS`, with the updated TeX parameters as
+    `pydischarge.plot.rc.GWPY_TEX_RCPARAMS`.
 
     .. note::
 
        This function doesn't apply the new `RcParams` in any way, just
        creates something that can be used to set `matplotlib.rcParams`.
 
     Parameters
@@ -99,26 +99,26 @@
         using the ``GWPY_USETEX`` environment variable, and whether `tex`
         is available on the system. If `True` is given (or determined)
         a number of other parameters are updated to improve TeX formatting.
 
     Examples
     --------
     >>> import matplotlib
-    >>> from pdpy.plot.rc import rc_params as pdpy_rc_params()
-    >>> matplotlib.rcParams.update(pdpy_rc_params(usetex=False))
+    >>> from pydischarge.plot.rc import rc_params as pydischarge_rc_params()
+    >>> matplotlib.rcParams.update(pydischarge_rc_params(usetex=False))
     """
     # if user didn't specify to use tex or not, guess based on
     # the `GWPY_USETEX` environment variable, or whether tex is
     # installed at all.
     if usetex is None:
         usetex = bool_env(
             'GWPY_USETEX',
             default=rcParams['text.usetex'] or tex.has_tex())
 
-    # build RcParams from matplotlib.rcParams with PDpy extras
+    # build RcParams from matplotlib.rcParams with pyDischarge extras
     rcp = GWPY_RCPARAMS.copy()
     if usetex:
         rcp.update(GWPY_TEX_RCPARAMS)
     return rcp
 
 
 # -- dynamic subplot positioning ----------------------------------------------
```

### Comparing `pydischarge-0.0.1/pdpy/plot/segments.py` & `pydischarge-0.0.2/pydischarge/plot/segments.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2022)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Plotting utilities for segments
 """
 
 from matplotlib.artist import allow_rasterization
 from matplotlib.colors import is_color_like
 from matplotlib.ticker import (Formatter, MultipleLocator)
@@ -39,29 +39,29 @@
 
 
 class SegmentAxes(Axes):
     """Custom `Axes` to display segments.
 
     This `SegmentAxes` provides custom methods for displaying any of
 
-    - `~pdpy.segments.DataQualityFlag`
-    - `~pdpy.segments.Segment` or :class:`ligo.segments.segment`
-    - `~pdpy.segments.SegmentList` or :class:`ligo.segments.segmentlist`
-    - `~pdpy.segments.SegmentListDict` or
+    - `~pydischarge.segments.DataQualityFlag`
+    - `~pydischarge.segments.Segment` or :class:`ligo.segments.segment`
+    - `~pydischarge.segments.SegmentList` or :class:`ligo.segments.segmentlist`
+    - `~pydischarge.segments.SegmentListDict` or
       :class:`ligo.segments.segmentlistdict`
 
     Parameters
     ----------
     insetlabels : `bool`, default: `False`
         display segment labels inside the axes. Prevents very long segment
         names from getting squeezed off the end of a standard figure
 
     See also
     --------
-    pdpy.plot.Axes
+    pydischarge.plot.Axes
         for documentation of other args and kwargs
     """
     name = 'segments'
 
     def __init__(self, *args, **kwargs):
         # default to auto-gps scale on the X-axis
         kwargs.setdefault('xscale', 'auto-gps')
@@ -97,18 +97,18 @@
         """Plot data onto these axes
 
         Parameters
         ----------
         args
             a single instance of
 
-                - `~pdpy.segments.DataQualityFlag`
-                - `~pdpy.segments.Segment`
-                - `~pdpy.segments.SegmentList`
-                - `~pdpy.segments.SegmentListDict`
+                - `~pydischarge.segments.DataQualityFlag`
+                - `~pydischarge.segments.Segment`
+                - `~pydischarge.segments.SegmentList`
+                - `~pydischarge.segments.SegmentListDict`
 
             or equivalent types upstream from :mod:`ligo.segments`
 
         kwargs
             keyword arguments applicable to `~matplotib.axes.Axes.plot`
 
         Returns
@@ -132,19 +132,19 @@
             args.pop(0)
         if args:
             out.extend(super().plot(*args, **kwargs))
         self.autoscale(enable=None, axis='both', tight=False)
         return out
 
     def plot_dict(self, flags, label='key', known='x', **kwargs):
-        """Plot a `~pdpy.segments.DataQualityDict` onto these axes
+        """Plot a `~pydischarge.segments.DataQualityDict` onto these axes
 
         Parameters
         ----------
-        flags : `~pdpy.segments.DataQualityDict`
+        flags : `~pydischarge.segments.DataQualityDict`
             data-quality dict to display
 
         label : `str`, optional
             labelling system to use, or fixed label for all `DataQualityFlags`.
             Special values include
 
             - ``'key'``: use the key of the `DataQualityDict`,
@@ -174,19 +174,19 @@
             elif label.lower() != 'key':
                 lab = label
             out.append(self.plot_flag(flag, label=to_string(lab), known=known,
                                       **kwargs))
         return out
 
     def plot_flag(self, flag, y=None, **kwargs):
-        """Plot a `~pdpy.segments.DataQualityFlag` onto these axes.
+        """Plot a `~pydischarge.segments.DataQualityFlag` onto these axes.
 
         Parameters
         ----------
-        flag : `~pdpy.segments.DataQualityFlag`
+        flag : `~pydischarge.segments.DataQualityFlag`
             Data-quality flag to display.
 
         y : `float`, optional
             Y-axis value for new segments.
 
         height : `float`, optional,
             Height for each segment, default: `0.8`.
@@ -249,19 +249,19 @@
                                 height=kwargs.get('height', .8)*.5)
             self.plot_segmentlist(flag.known, y=y, label=name, **known_kw)
 
         return coll  # return active collection
 
     def plot_segmentlist(self, segmentlist, y=None, height=.8, label=None,
                          collection=True, rasterized=None, **kwargs):
-        """Plot a `~pdpy.segments.SegmentList` onto these axes
+        """Plot a `~pydischarge.segments.SegmentList` onto these axes
 
         Parameters
         ----------
-        segmentlist : `~pdpy.segments.SegmentList`
+        segmentlist : `~pydischarge.segments.SegmentList`
             list of segments to display
 
         y : `float`, optional
             y-axis value for new segments
 
         collection : `bool`, default: `True`
             add all patches as a
@@ -314,21 +314,21 @@
                 patch.set_rasterized(rasterized)
                 label = ''
                 out.append(self.add_patch(patch))
         self.autoscale(enable=None, axis='both', tight=False)
         return out
 
     def plot_segmentlistdict(self, segmentlistdict, y=None, dy=1, **kwargs):
-        """Plot a `~pdpy.segments.SegmentListDict` onto
+        """Plot a `~pydischarge.segments.SegmentListDict` onto
         these axes
 
         Parameters
         ----------
-        segmentlistdict : `~pdpy.segments.SegmentListDict`
-            (name, `~pdpy.segments.SegmentList`) dict
+        segmentlistdict : `~pydischarge.segments.SegmentListDict`
+            (name, `~pydischarge.segments.SegmentList`) dict
 
         y : `float`, optional
             starting y-axis value for new segmentlists
 
         **kwargs
             any other keyword arguments acceptable for
             `~matplotlib.patches.Rectangle`
@@ -451,15 +451,15 @@
 
 class SegmentRectangle(Rectangle):
     def __init__(self, segment, y, height=.8, valign='center', **kwargs):
         """Build a `~matplotlib.patches.Rectangle` from a segment
 
         Parameters
         ----------
-        segment : `~pdpy.segments.Segment`
+        segment : `~pydischarge.segments.Segment`
             ``[start, stop)`` GPS segment
 
         y : `float`
             y-axis position for segment
 
         height : `float`, optional, default: 1
             height (in y-axis units) for segment
```

### Comparing `pydischarge-0.0.1/pdpy/plot/tests/__init__.py` & `pydischarge-0.0.2/pydischarge/timeseries/tests/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for `pdpy.plot`
+"""Tests for :mod:`pydischarge.timeseries`
 """
```

### Comparing `pydischarge-0.0.1/pdpy/plot/tests/test_axes.py` & `pydischarge-0.0.2/pydischarge/plot/tests/test_axes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Cardiff University (2018-2022)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.plot`
+"""Unit tests for :mod:`pydischarge.plot`
 """
 
 import pytest
 
 import numpy
 
 from matplotlib import rcParams
@@ -118,15 +118,15 @@
 
     @pytest.mark.parametrize('sortbycolor', (False, True))
     def test_scatter_errors(self, ax, sortbycolor):
         # check that errors are handled properly
         x = 1
         y = 'B'
         c = 'something else'
-        if sortbycolor:  # pdpy error
+        if sortbycolor:  # pydischarge error
             match = "^Axes.scatter argument 'sortbycolor'"
         else:  # matplotlib error
             match = "^'c' argument must be a "
         with pytest.raises(ValueError, match=match):
             ax.scatter(x, y, c=c, sortbycolor=sortbycolor)
 
     def test_imshow(self, ax):
```

### Comparing `pydischarge-0.0.1/pdpy/plot/tests/test_bode.py` & `pydischarge-0.0.2/pydischarge/plot/tests/test_bode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for `pdpy.plot.filter`
+"""Tests for `pydischarge.plot.filter`
 """
 
 import numpy
 from numpy import testing as nptest
 
 from scipy import signal
```

### Comparing `pydischarge-0.0.1/pdpy/plot/tests/test_colors.py` & `pydischarge-0.0.2/pydischarge/plot/tests/test_colors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for `pdpy.plot.colors`
+"""Tests for `pydischarge.plot.colors`
 """
 
 import pytest
 
 from numpy.testing import assert_array_equal
 
 from matplotlib.colors import (Normalize, LogNorm)
```

### Comparing `pydischarge-0.0.1/pdpy/plot/tests/test_gps.py` & `pydischarge-0.0.2/pydischarge/plot/tests/test_gps.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for `pdpy.plot.gps`
+"""Tests for `pydischarge.plot.gps`
 """
 
 from decimal import Decimal
 
 import pytest
 
 import numpy
```

### Comparing `pydischarge-0.0.1/pdpy/plot/tests/test_log.py` & `pydischarge-0.0.2/pydischarge/plot/tests/test_log.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for `pdpy.plot.log`
+"""Tests for `pydischarge.plot.log`
 """
 
 from unittest import mock
 
 import pytest
 
 from matplotlib import (
@@ -33,15 +33,15 @@
 class TestLogFormatter(object):
     TEST_CLASS = plot_log.LogFormatter
 
     @classmethod
     @pytest.fixture
     def formatter(cls):
         with mock.patch(
-            "pdpy.plot.log.LogFormatter._num_ticks",
+            "pydischarge.plot.log.LogFormatter._num_ticks",
             return_value=2,
         ):
             yield cls.TEST_CLASS()
 
     @pytest.mark.parametrize('x, fmt, result, texresult', [
         pytest.param(
             0.,
@@ -68,27 +68,27 @@
     def test_call(self, formatter, x, fmt, result, texresult):
         with rc_context(rc={'text.usetex': False}):
             assert formatter(x, fmt=fmt) == result
         with rc_context(rc={'text.usetex': True}):
             assert formatter(x, fmt=fmt) == texresult
 
     @mock.patch(  # we don't need this function for this test
-        "pdpy.plot.log.LogFormatter.set_locs",
+        "pydischarge.plot.log.LogFormatter.set_locs",
         mock.MagicMock(),
     )
     @pytest.mark.parametrize("values, result", [
         # normal output
         pytest.param(
             [1e-1, 1e2, 1e5, 1e8],
             [plot_log._math(x) for x in
              ("10^{-1}", "10^{2}", "10^{5}", "10^{8}")],
             id="mpl",
         ),
         # custom output
         pytest.param(
             [1e-1, 1e0, 1e1, 1e2],
             [plot_log._math(x) for x in ("0.1", "1", "10", "100")],
-            id="pdpy",
+            id="pydischarge",
         ),
     ])
     def test_format_ticks(self, formatter, values, result):
         assert formatter.format_ticks(values) == result
```

### Comparing `pydischarge-0.0.1/pdpy/plot/tests/test_plot.py` & `pydischarge-0.0.2/pydischarge/plot/tests/test_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Cardiff University (2018-2022)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.plot`
+"""Unit tests for :mod:`pydischarge.plot`
 """
 
 import pytest
 
 import numpy
 
 from ...segments import (Segment, SegmentList)
```

### Comparing `pydischarge-0.0.1/pdpy/plot/tests/test_rc.py` & `pydischarge-0.0.2/pydischarge/plot/tests/test_rc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Cardiff University (2018-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for `pdpy.plot.rc`
+"""Tests for `pydischarge.plot.rc`
 """
 
 import pytest
 
 from matplotlib import rcParams
 
 from .. import rc as plot_rc
```

### Comparing `pydischarge-0.0.1/pdpy/plot/tests/test_segments.py` & `pydischarge-0.0.2/pydischarge/plot/tests/test_segments.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for `pdpy.plot.segments`
+"""Tests for `pydischarge.plot.segments`
 """
 
 import pytest
 
 import numpy
 
 from matplotlib import rcParams
```

### Comparing `pydischarge-0.0.1/pdpy/plot/tests/test_tex.py` & `pydischarge-0.0.2/pydischarge/plot/tests/test_tex.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for `pdpy.plot.tex`
+"""Tests for `pydischarge.plot.tex`
 """
 
 from unittest import mock
 
 import pytest
 
 from .. import tex as plot_tex
@@ -30,34 +30,34 @@
     """Fake which to force pdflatex to being not found
     """
     if arg == "pdflatex":
         return None
     return arg
 
 
-@mock.patch("pdpy.plot.tex.which", _which)
+@mock.patch("pydischarge.plot.tex.which", _which)
 def test_has_tex_missing_exe():
-    """Test that `pdpy.plot.tex.has_tex` returns `False` when
+    """Test that `pydischarge.plot.tex.has_tex` returns `False` when
     any one of the necessary executables is missing.
     """
     assert not plot_tex.has_tex()
 
 
-@mock.patch("pdpy.plot.tex._test_usetex", side_effect=RuntimeError)
+@mock.patch("pydischarge.plot.tex._test_usetex", side_effect=RuntimeError)
 def test_has_tex_bad_latex(_):
-    """Test that `pdpy.plot.tex.has_tex` returns `False` when
+    """Test that `pydischarge.plot.tex.has_tex` returns `False` when
     the LaTeX figure fails to render.
     """
     assert not plot_tex.has_tex()
 
 
-@mock.patch("pdpy.plot.tex.which", return_value="path")
-@mock.patch("pdpy.plot.tex._test_usetex")
+@mock.patch("pydischarge.plot.tex.which", return_value="path")
+@mock.patch("pydischarge.plot.tex._test_usetex")
 def test_has_tex_true(_which_, _test_usetex):
-    """Test that `pdpy.plot.tex.has_tex` returns `True` when
+    """Test that `pydischarge.plot.tex.has_tex` returns `True` when
     all of the necessary executables are found, and the LaTeX figure
     doesn't raise an exception.
     """
     assert plot_tex.has_tex()
 
 
 @pytest.mark.parametrize('in_, out', [
```

### Comparing `pydischarge-0.0.1/pdpy/plot/tests/test_text.py` & `pydischarge-0.0.2/pydischarge/plot/tests/test_text.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for `pdpy.plot.text`
+"""Tests for `pydischarge.plot.text`
 """
 
 import pytest
 
 from matplotlib import rc_context
 
 from astropy.units import Unit
```

### Comparing `pydischarge-0.0.1/pdpy/plot/tests/test_utils.py` & `pydischarge-0.0.2/pydischarge/plot/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for `pdpy.plot.text`
+"""Tests for `pydischarge.plot.text`
 """
 
 import itertools
 
 from matplotlib import (
     colors as mpl_colors,
 )
```

### Comparing `pydischarge-0.0.1/pdpy/plot/tests/utils.py` & `pydischarge-0.0.2/pydischarge/plot/tests/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Utilities for testing `pdpy.plot`
+"""Utilities for testing `pydischarge.plot`
 """
 
 from io import BytesIO
 
 import pytest
 
 from matplotlib import pyplot
```

### Comparing `pydischarge-0.0.1/pdpy/plot/tex.py` & `pydischarge-0.0.2/pydischarge/plot/tex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Handle TeX formatting for matplotlib output
 """
 
 import re
 from shutil import which
 
@@ -96,15 +96,15 @@
     Returns
     -------
     tex : `str`
         a TeX representation of the input
 
     Examples
     --------
-    >>> from pdpy.plot.tex import float_to_latex
+    >>> from pydischarge.plot.tex import float_to_latex
     >>> float_to_latex(1)
     '1'
     >>> float_to_latex(2000)
     '2\times 10^{3}'
     >>> float_to_latex(100)
     '10^{2}'
     >>> float_to_latex(-500)
@@ -143,15 +143,15 @@
     -------
     tex : `str`
         a modified version of the input text with all unescaped reserved
         latex characters escaped
 
     Examples
     --------
-    >>> from pdpy.plot.tex import label_to_latex
+    >>> from pydischarge.plot.tex import label_to_latex
     >>> label_to_latex('normal text')
     'normal text'
     >>> label_to_latex('$1 + 2 = 3$')
     '$1 + 2 = 3$'
     >>> label_to_latex('H1:ABC-DEF_GHI')
     'H1:ABC-DEF\\_GHI'
     >>> label_to_latex('H1:ABC-DEF\_GHI')
```

### Comparing `pydischarge-0.0.1/pdpy/plot/text.py` & `pydischarge-0.0.2/pydischarge/plot/text.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Text formatting for PDpy plots
+"""Text formatting for pyDischarge plots
 """
 
 from matplotlib import rcParams
 
 from astropy import units
 
 from . import tex
```

### Comparing `pydischarge-0.0.1/pdpy/plot/units.py` & `pydischarge-0.0.2/pydischarge/plot/units.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Support for plotting with units
 """
 
 from astropy.units.format import LatexInline
```

### Comparing `pydischarge-0.0.1/pdpy/plot/utils.py` & `pydischarge-0.0.2/pydischarge/plot/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Helper functions for plotting data with matplotlib and LAL
 """
 
 import itertools
 
 from matplotlib import rcParams
@@ -29,15 +29,15 @@
 FIGURE_PARAMS = [
     'figsize', 'dpi',
 ]
 AXES_PARAMS = [
     'projection', 'title',  # standard options
     'sharex', 'xlim', 'xlabel', 'xscale',  # X-axis params
     'sharey', 'ylim', 'ylabel', 'yscale',  # Y-axis params
-    'epoch', 'insetlabels',  # special PDpy extras
+    'epoch', 'insetlabels',  # special pyDischarge extras
 ]
 
 
 def color_cycle(colors=None):
     """An infinite iterator of the given (or default) colors
     """
     if colors:
```

### Comparing `pydischarge-0.0.1/pdpy/segments/__init__.py` & `pydischarge-0.0.2/pydischarge/segments/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module provides classes for generating and manipulating
 data segments of the form [gps_start, gps_end).
 
 The core of this module is adapted from |ligo-segments|_.
 """
```

### Comparing `pydischarge-0.0.1/pdpy/segments/flag.py` & `pydischarge-0.0.2/pydischarge/segments/flag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module defines the `DataQualityFlag` and `DataQualityDict`.
 
 The `DataQualityFlag` represents an annotated set of data-quality segments
 indicating something about the state of a laser-interferometer
 gravitational-wave detector in a given time interval.
 
@@ -448,15 +448,15 @@
         Returns
         -------
         flag : `DataQualityFlag`
             a new flag with `active` segments filled from Open Data
 
         Examples
         --------
-        >>> from pdpy.segments import DataQualityFlag
+        >>> from pydischarge.segments import DataQualityFlag
         >>> print(DataQualityFlag.fetch_open_data('H1_DATA', 'Jan 1 2010',
         ...                                       'Jan 2 2010'))
         <DataQualityFlag('H1:DATA',
                          known=[[946339215 ... 946425615)],
                          active=[[946340946 ... 946351800)
                                  [946356479 ... 946360620)
                                  [946362652 ... 946369150)
@@ -797,30 +797,30 @@
     def plot(self, figsize=(12, 4), xscale='auto-gps', **kwargs):
         """Plot this flag on a segments projection.
 
         Parameters
         ----------
         **kwargs
             all keyword arguments are passed to the
-            :class:`~pdpy.plot.Plot` constructor.
+            :class:`~pydischarge.plot.Plot` constructor.
 
         Returns
         -------
         figure : `~matplotlib.figure.Figure`
             the newly created figure, with populated Axes.
 
         See also
         --------
         matplotlib.pyplot.figure
             for documentation of keyword arguments used to create the
             figure
         matplotlib.figure.Figure.add_subplot
             for documentation of keyword arguments used to create the
             axes
-        pdpy.plot.SegmentAxes.plot_segmentlist
+        pydischarge.plot.SegmentAxes.plot_segmentlist
             for documentation of keyword arguments used in rendering the data
         """
         from matplotlib import rcParams
         from ..plot import Plot
 
         if self.label:
             kwargs.setdefault('label', self.label)
@@ -1125,17 +1125,17 @@
                                format='ligolw'):
         """Read a `DataQualityDict` from a LIGO_LW XML VetoDefinerTable.
 
         Parameters
         ----------
         fp : `str`
             path of veto definer file to read
-        start : `~pdpy.time.LIGOTimeGPS`, `int`, optional
+        start : `~pydischarge.time.LIGOTimeGPS`, `int`, optional
             GPS start time at which to restrict returned flags
-        end : `~pdpy.time.LIGOTimeGPS`, `int`, optional
+        end : `~pydischarge.time.LIGOTimeGPS`, `int`, optional
             GPS end time at which to restrict returned flags
         ifo : `str`, optional
             interferometer prefix whose flags you want to read
         format : `str`, optional
             format of file to read, currently only 'ligolw' is supported
 
         Returns
@@ -1211,15 +1211,15 @@
 
         names : `list` of `str`, optional
             a list of flag names to read, defaults to returning all
 
         gpstype : `type`, `callable`, optional
             class to use for GPS times in returned objects, can be a function
             to convert GPS time to something else, default is
-            `~pdpy.time.LIGOTimeGPS`
+            `~pydischarge.time.LIGOTimeGPS`
 
         on_missing : `str`, optional
             action to take when a one or more ``names`` are not found in
             the ``segment_definer`` table, one of
 
             - ``'ignore'`` : do nothing
             - ``'warn'`` : print a warning
@@ -1575,30 +1575,30 @@
             - ``'key'``: use the key of the `DataQualityDict`,
             - ``'name'``: use the :attr:`~DataQualityFlag.name` of the flag
 
             If anything else, that fixed label will be used for all lines.
 
         **kwargs
             all keyword arguments are passed to the
-            :class:`~pdpy.plot.Plot` constructor.
+            :class:`~pydischarge.plot.Plot` constructor.
 
         Returns
         -------
         figure : `~matplotlib.figure.Figure`
             the newly created figure, with populated Axes.
 
         See also
         --------
         matplotlib.pyplot.figure
             for documentation of keyword arguments used to create the
             figure
         matplotlib.figure.Figure.add_subplot
             for documentation of keyword arguments used to create the
             axes
-        pdpy.plot.SegmentAxes.plot_segmentlist
+        pydischarge.plot.SegmentAxes.plot_segmentlist
             for documentation of keyword arguments used in rendering the data
         """
         # make plot
         from ..plot import Plot
         plot = Plot(self, projection='segments', **kwargs)
 
         # update labels
```

### Comparing `pydischarge-0.0.1/pdpy/segments/io/__init__.py` & `pydischarge-0.0.2/pydischarge/testing/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) Duncan Macleod (2014-2020)
+# Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Input/output routines for the `pdpy.segments` classes
+"""Testing utilities for pyDischarge
 """
-
-from . import (  # pylint: disable=unused-import
-    ligolw,  # LIGO_LW XML
-    segwizard,  # LIGO SegWizard ASCII
-    hdf5,  # HDF5
-    json,  # segments-web.ligo.org JSON
-)
-
-__author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
```

### Comparing `pydischarge-0.0.1/pdpy/segments/io/hdf5.py` & `pydischarge-0.0.2/pydischarge/segments/io/hdf5.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module attaches the HDF5 input output methods to the DataQualityFlag.
 
 While these methods are avialable as methods of the class itself,
 this module attaches them to the unified I/O registry, making it a bit
 cleaner.
 """
```

### Comparing `pydischarge-0.0.1/pdpy/segments/io/json.py` & `pydischarge-0.0.2/pydischarge/segments/io/json.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read/write segments and flags from DQSEGDB-format JSON
 """
 
 import json
 
 from ...io import registry
```

### Comparing `pydischarge-0.0.1/pdpy/segments/io/ligolw.py` & `pydischarge-0.0.2/pydischarge/segments/io/ligolw.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read/write segment XML in LIGO_LW format into DataQualityFlags
 """
 
 import operator
 from functools import reduce
 
@@ -105,28 +105,28 @@
 
 def write_ligolw(flags, target, attrs=None, **kwargs):
     """Write this `DataQualityFlag` to the given LIGO_LW Document
 
     Parameters
     ----------
     flags : `DataQualityFlag`, `DataQualityDict`
-        `pdpy.segments` object to write
+        `pydischarge.segments` object to write
 
     target : `str`, `file`, :class:`~ligo.lw.ligolw.Document`
         the file or document to write into
 
     attrs : `dict`, optional
         extra attributes to write into segment tables
 
     **kwargs
         keyword arguments to use when writing
 
     See also
     --------
-    pdpy.io.ligolw.write_ligolw_tables
+    pydischarge.io.ligolw.write_ligolw_tables
         for details of acceptable keyword arguments
     """
     if isinstance(flags, DataQualityFlag):
         flags = DataQualityDict({flags.name: flags})
     return write_tables(
         target,
         flags.to_ligolw_tables(**attrs or dict()),
```

### Comparing `pydischarge-0.0.1/pdpy/segments/io/segwizard.py` & `pydischarge-0.0.2/pydischarge/segments/io/segwizard.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read SegmentLists from seg-wizard format ASCII files
 """
 
 import re
 
 from .. import (Segment, SegmentList)
@@ -60,15 +60,15 @@
 
     strict : `bool`, optional
         Check that recorded duration matches ``end-start`` for all segments;
         only used when reading from a 3+-column file.
 
     Returns
     -------
-    segments : `~pdpy.segments.SegmentList`
+    segments : `~pydischarge.segments.SegmentList`
         The list of segments as parsed from the file.
 
     Notes
     -----
     This method is adapted from original code written by Kipp Cannon and
     distributed under GPLv3.
     """
@@ -116,15 +116,15 @@
 
 @with_open(mode="w", pos=1)
 def to_segwizard(segs, target, header=True, coltype=LIGOTimeGPS):
     """Write the given `SegmentList` to a file in SegWizard format.
 
     Parameters
     ----------
-    segs : :class:`~pdpy.segments.SegmentList`
+    segs : :class:`~pydischarge.segments.SegmentList`
         The list of segments to write.
 
     target : `file`, `str`
         An open file, or file path, to which to write.
 
     header : `bool`, optional
         Print a column header into the file, default: `True`.
```

### Comparing `pydischarge-0.0.1/pdpy/segments/segments.py` & `pydischarge-0.0.2/pydischarge/segments/segments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """A `Segment` is a interval of time marked by a GPS [start, stop)
 semi-open interval. These typically represent periods when a
 gravitational-wave laser interferometer was operating in a specific
 configuration.
 """
 
@@ -180,15 +180,15 @@
 
         coalesce : `bool`, optional
             if `True` coalesce the segment list before returning,
             otherwise return exactly as contained in file(s).
 
         **kwargs
             other keyword arguments depend on the format, see the online
-            documentation for details (:ref:`pdpy-segments-io`)
+            documentation for details (:ref:`pydischarge-segments-io`)
 
         Returns
         -------
         segmentlist : `SegmentList`
             `SegmentList` active and known segments read from file.
 
         Raises
```

### Comparing `pydischarge-0.0.1/pdpy/segments/tests/__init__.py` & `pydischarge-0.0.2/pydischarge/cli/tests/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) Duncan Macleod (2018-2020)
+# Copyright (C) Duncan Macleod (2019-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.segments`
+"""Tests for :mod:`pydischarge.cli`
 """
```

### Comparing `pydischarge-0.0.1/pdpy/segments/tests/test_flag.py` & `pydischarge-0.0.2/pydischarge/segments/tests/test_flag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.segments`
+"""Tests for :mod:`pydischarge.segments`
 """
 
 import re
 import warnings
 from io import BytesIO
 from unittest import mock
 from urllib.error import HTTPError
@@ -410,15 +410,15 @@
         utils.assert_segmentlist_equal(f.known, [(0, float('inf'))])
 
         a = veto_def('X1', 'TEST-FLAG', None, start_time=0, end_time=1)
         f = self.TEST_CLASS.from_veto_def(a)
         assert f.name == 'X1:TEST-FLAG'
         assert f.version is None
 
-    @mock.patch("pdpy.segments.flag.query_segments", mock_query_segments)
+    @mock.patch("pydischarge.segments.flag.query_segments", mock_query_segments)
     def test_populate(self):
         name = QUERY_FLAGS[0]
         flag = self.TEST_CLASS(name, known=QUERY_RESULT[name].known)
         flag.populate()
         utils.assert_flag_equal(flag, QUERY_RESULTC[name])
 
     # -- test I/O -------------------------------
@@ -475,39 +475,39 @@
             assert_equal=utils.assert_flag_equal,
             autoidentify=False,
             read_kw={},
         )
 
     @pytest.mark.requires("ligo.lw.lsctables")
     def test_write_ligolw_attrs(self, tmp_path, flag):
-        from pdpy.io.ligolw import read_table
+        from pydischarge.io.ligolw import read_table
         tmp = tmp_path / "tmp.xml"
         flag.write(
             tmp,
             format='ligolw',
             attrs={'process_id': 100},
         )
         segdeftab = read_table(tmp, 'segment_definer')
         assert int(segdeftab[0].process_id) == 100
 
     # -- test queries ---------------------------
 
-    @mock.patch("pdpy.segments.flag.query_segments", mock_query_segments)
+    @mock.patch("pydischarge.segments.flag.query_segments", mock_query_segments)
     def test_query(self):
         result = self.TEST_CLASS.query(QUERY_FLAGS[0], 0, 10)
         assert isinstance(result, self.TEST_CLASS)
         RESULT = QUERY_RESULT[QUERY_FLAGS[0]].copy().coalesce()
         utils.assert_segmentlist_equal(result.known, RESULT.known)
         utils.assert_segmentlist_equal(result.active, RESULT.active)
 
     @pytest.mark.parametrize('name, flag', [
         (QUERY_FLAGS[0], QUERY_FLAGS[0]),  # regular query
         (QUERY_FLAGS[0].rsplit(':', 1)[0], QUERY_FLAGS[0]),  # versionless
     ])
-    @mock.patch('pdpy.segments.flag.query_segments', mock_query_segments)
+    @mock.patch('pydischarge.segments.flag.query_segments', mock_query_segments)
     def test_query_dqsegdb(self, name, flag):
         # standard query
         result = self.TEST_CLASS.query_dqsegdb(name, 0, 10)
         RESULT = QUERY_RESULTC[flag]
         assert isinstance(result, self.TEST_CLASS)
         utils.assert_segmentlist_equal(result.known, RESULT.known)
         utils.assert_segmentlist_equal(result.active, RESULT.active)
@@ -534,15 +534,15 @@
 
         # bad syntax
         with pytest.raises(ValueError):
             self.TEST_CLASS.query_dqsegdb(QUERY_FLAGS[0], 1, 2, 3)
         with pytest.raises(ValueError):
             self.TEST_CLASS.query_dqsegdb(QUERY_FLAGS[0], (1, 2, 3))
 
-    @mock.patch('pdpy.segments.flag.query_segments', mock_query_segments)
+    @mock.patch('pydischarge.segments.flag.query_segments', mock_query_segments)
     def test_query_dqsegdb_multi(self):
         segs = SegmentList([Segment(0, 2), Segment(8, 10)])
         result = self.TEST_CLASS.query_dqsegdb(QUERY_FLAGS[0], segs)
         RESULT = QUERY_RESULTC[QUERY_FLAGS[0]]
 
         assert isinstance(result, self.TEST_CLASS)
         utils.assert_segmentlist_equal(result.known, RESULT.known & segs)
@@ -771,23 +771,23 @@
         tables = instance.to_ligolw_tables()
         assert len(tables[0]) == len(instance)  # segdef
         assert len(tables[1]) == sum(len(x.known) for x in instance.values())
         assert len(tables[2]) == sum(len(x.active) for x in instance.values())
 
     # -- test queries ---------------------------
 
-    @mock.patch('pdpy.segments.flag.query_segments', mock_query_segments)
+    @mock.patch('pydischarge.segments.flag.query_segments', mock_query_segments)
     def test_query(self):
         result = self.TEST_CLASS.query(QUERY_FLAGS, 0, 10)
         RESULT = QUERY_RESULT.copy().coalesce()
 
         assert isinstance(result, self.TEST_CLASS)
         utils.assert_dict_equal(result, RESULT, utils.assert_flag_equal)
 
-    @mock.patch('pdpy.segments.flag.query_segments', mock_query_segments)
+    @mock.patch('pydischarge.segments.flag.query_segments', mock_query_segments)
     def test_query_dqsegdb(self):
         result = self.TEST_CLASS.query_dqsegdb(QUERY_FLAGS, 0, 10)
         RESULT = QUERY_RESULTC
         assert isinstance(result, self.TEST_CLASS)
         utils.assert_dict_equal(result, RESULT, utils.assert_flag_equal)
 
         # check all values of on_error
@@ -797,15 +797,15 @@
             result = self.TEST_CLASS.query_dqsegdb(
                 QUERY_FLAGS + ['X1:BLAHBLAH:1'], 0, 10, on_error='ignore')
         utils.assert_dict_equal(result, RESULT, utils.assert_flag_equal)
         assert len(record) == 1  # check on_error='ignore' didn't warn
         with pytest.raises(ValueError):
             self.TEST_CLASS.query_dqsegdb(QUERY_FLAGS, 0, 10, on_error='blah')
 
-    @mock.patch('pdpy.segments.flag.query_segments', mock_query_segments)
+    @mock.patch('pydischarge.segments.flag.query_segments', mock_query_segments)
     def test_populate(self):
         def fake():
             return self.TEST_CLASS({
                 x: self.ENTRY_CLASS(name=x, known=y.known) for
                 x, y in QUERY_RESULT.items()})
 
         # build fake veto definer file
```

### Comparing `pydischarge-0.0.1/pdpy/segments/tests/test_segments.py` & `pydischarge-0.0.2/pydischarge/segments/tests/test_segments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.segments.segments`
+"""Tests for :mod:`pydischarge.segments.segments`
 """
 
 import pytest
 
 import h5py
 
 from astropy.table import Table
@@ -68,15 +68,15 @@
     @pytest.fixture()
     def segmentlist(cls):
         return cls.create((1, 2), (3, 4), (4, 6), (8, 10))
 
     # -- test methods ---------------------------
 
     def test_extent(self, segmentlist):
-        """Test `pdpy.segments.SegmentList.extent returns the right type
+        """Test `pydischarge.segments.SegmentList.extent returns the right type
         """
         extent = segmentlist.extent()
         assert isinstance(extent, self.ENTRY_CLASS)
         assert extent == Segment(1, 10)
 
     def test_coalesce(self):
         segmentlist = self.create((1, 2), (3, 4), (4, 5))
```

### Comparing `pydischarge-0.0.1/pdpy/signal/__init__.py` & `pydischarge-0.0.2/pydischarge/frequencyseries/io/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) Duncan Macleod (2016-2020)
+# Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""The `gwpy.signal` module provides signal-processing utilities that
-extend the functionality of `scipy.signal` (and others) for specific GW data
-applications.
-
-See the sub-modules for more details.
+"""Input/Output routines for pydischarge.frequencyseries
 """
 
-__author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
+from . import (  # pylint: disable=unused-import
+    ascii,
+    hdf5,
+    ligolw,
+)
+
+__author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
```

### Comparing `pydischarge-0.0.1/pdpy/signal/fft.py` & `pydischarge-0.0.2/pydischarge/signal/fft.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2019-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""This module has been renamed `pdpy.signal.spectral`.
+"""This module has been renamed `pydischarge.signal.spectral`.
 
 DO NOT USE THIS MODULE.
 """
 
 import warnings
 
 # import things as they were named before
@@ -31,11 +31,11 @@
     _registry as registry,
     _scipy as scipy,
     _ui as ui,
     _utils as utils,
 )
 
 warnings.warn(
-    "this module has been renamed pdpy.signal.spectral and will be "
+    "this module has been renamed pydischarge.signal.spectral and will be "
     "removed in a future release",
     DeprecationWarning,
 )
```

### Comparing `pydischarge-0.0.1/pdpy/signal/filter_design.py` & `pydischarge-0.0.2/pydischarge/signal/filter_design.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Custom filtering utilities for the `TimeSeries`
 """
 
 import operator
 from functools import reduce
 from math import (pi, log10)
@@ -167,15 +167,15 @@
     Notes
     -----
     By default, the input transfer function will have five samples tapered
     off at the left and right boundaries. If `ncorner` is not `None`, then
     `ncorner` extra samples will be zeroed on the left as a hard highpass
     filter.
 
-    See :func:`~pdpy.signal.window.planck` for more information.
+    See :func:`~pydischarge.signal.window.planck` for more information.
     """
     nsamp = transfer.size
     ncorner = ncorner if ncorner else 0
     out = transfer.copy()
     out[0:ncorner] = 0
     out[ncorner:nsamp] *= planck(nsamp-ncorner, nleft=5, nright=5)
     return out
@@ -409,20 +409,20 @@
     By default a digital filter is returned, meaning the zeros and poles
     are given in the Z-domain in units of radians/sample.
 
     Examples
     --------
     To create a low-pass filter at 1000 Hz for 4096 Hz-sampled data:
 
-    >>> from pdpy.signal.filter_design import lowpass
+    >>> from pydischarge.signal.filter_design import lowpass
     >>> lp = lowpass(1000, 4096)
 
-    To view the filter, you can use the `~pdpy.plot.BodePlot`:
+    To view the filter, you can use the `~pydischarge.plot.BodePlot`:
 
-    >>> from pdpy.plot import BodePlot
+    >>> from pydischarge.plot import BodePlot
     >>> plot = BodePlot(lp, sample_rate=4096)
     >>> plot.show()
     """
     sample_rate = _as_float(sample_rate)
     frequency = _as_float(frequency)
     if fstop is None:
         fstop = min(frequency * 1.5, sample_rate/2.)
@@ -471,20 +471,20 @@
     By default a digital filter is returned, meaning the zeros and poles
     are given in the Z-domain in units of radians/sample.
 
     Examples
     --------
     To create a high-pass filter at 100 Hz for 4096 Hz-sampled data:
 
-    >>> from pdpy.signal.filter_design import highpass
+    >>> from pydischarge.signal.filter_design import highpass
     >>> hp = highpass(100, 4096)
 
-    To view the filter, you can use the `~pdpy.plot.BodePlot`:
+    To view the filter, you can use the `~pydischarge.plot.BodePlot`:
 
-    >>> from pdpy.plot import BodePlot
+    >>> from pydischarge.plot import BodePlot
     >>> plot = BodePlot(hp, sample_rate=4096)
     >>> plot.show()
     """
     sample_rate = _as_float(sample_rate)
     frequency = _as_float(frequency)
     if fstop is None:
         fstop = frequency * 2/3.
@@ -537,20 +537,20 @@
     By default a digital filter is returned, meaning the zeros and poles
     are given in the Z-domain in units of radians/sample.
 
     Examples
     --------
     To create a band-pass filter for 100-1000 Hz for 4096 Hz-sampled data:
 
-    >>> from pdpy.signal.filter_design import bandpass
+    >>> from pydischarge.signal.filter_design import bandpass
     >>> bp = bandpass(100, 1000, 4096)
 
-    To view the filter, you can use the `~pdpy.plot.BodePlot`:
+    To view the filter, you can use the `~pydischarge.plot.BodePlot`:
 
-    >>> from pdpy.plot import BodePlot
+    >>> from pydischarge.plot import BodePlot
     >>> plot = BodePlot(bp, sample_rate=4096)
     >>> plot.show()
     """
     sample_rate = _as_float(sample_rate)
     flow = _as_float(flow)
     fhigh = _as_float(fhigh)
     if fstop is None:
@@ -597,20 +597,20 @@
     By default a digital filter is returned, meaning the zeros and poles
     are given in the Z-domain in units of radians/sample.
 
     Examples
     --------
     To create a low-pass filter at 1000 Hz for 4096 Hz-sampled data:
 
-    >>> from pdpy.signal.filter_design import notch
+    >>> from pydischarge.signal.filter_design import notch
     >>> n = notch(100, 4096)
 
-    To view the filter, you can use the `~pdpy.plot.BodePlot`:
+    To view the filter, you can use the `~pydischarge.plot.BodePlot`:
 
-    >>> from pdpy.plot import BodePlot
+    >>> from pydischarge.plot import BodePlot
     >>> plot = BodePlot(n, sample_rate=4096)
     >>> plot.show()
     """
     frequency = Quantity(frequency, 'Hz').value
     sample_rate = Quantity(sample_rate, 'Hz').value
     nyq = 0.5 * sample_rate
     df = 1.0  # pylint: disable=invalid-name
@@ -648,23 +648,23 @@
     gain : `float`
         the overall gain
 
     Examples
     --------
     Create a lowpass and a highpass filter, and combine them:
 
-    >>> from pdpy.signal.filter_design import (
+    >>> from pydischarge.signal.filter_design import (
     ...     highpass, lowpass, concatenate_zpks)
     >>> hp = highpass(100, 4096)
     >>> lp = lowpass(1000, 4096)
     >>> zpk = concatenate_zpks(hp, lp)
 
     Plot the filter:
 
-    >>> from pdpy.plot import BodePlot
+    >>> from pydischarge.plot import BodePlot
     >>> plot = BodePlot(zpk, sample_rate=4096)
     >>> plot.show()
     """
     zeros, poles, gains = zip(*zpks)
     return (numpy.concatenate(zeros),
             numpy.concatenate(poles),
             reduce(operator.mul, gains, 1))
```

### Comparing `pydischarge-0.0.1/pdpy/signal/qtransform.py` & `pydischarge-0.0.2/pydischarge/signal/qtransform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2016-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Python implementation of the tiled Q-transform scan.
 
 This is a re-implementation of the original Q-transform scan from the Omega
 pipeline, all credits for the original algorithm go to its
 authors.
 """
@@ -161,15 +161,15 @@
 
     def transform(self, fseries, **kwargs):
         """Compute the time-frequency plane at fixed Q with the most
         significant tile
 
         Parameters
         ----------
-        fseries : `~pdpy.timeseries.FrequencySeries`
+        fseries : `~pydischarge.timeseries.FrequencySeries`
             the complex FFT of a time-series data set
 
         **kwargs
             other keyword arguments to pass to `QPlane.transform`
 
         Returns
         -------
@@ -288,28 +288,28 @@
                               base=2, which=None)
 
     def transform(self, fseries, norm=True, epoch=None, search=None):
         """Calculate the energy `TimeSeries` for the given `fseries`
 
         Parameters
         ----------
-        fseries : `~pdpy.frequencyseries.FrequencySeries`
+        fseries : `~pydischarge.frequencyseries.FrequencySeries`
             the complex FFT of a time-series data set
 
         norm : `bool`, `str`, optional
             normalize the energy of the output by the median (if `True` or
             ``'median'``) or the ``'mean'``, if `False` the output
             is the complex `~numpy.fft.ifft` output of the Q-tranform
 
-        epoch : `~pdpy.time.LIGOTimeGPS`, `float`, optional
+        epoch : `~pydischarge.time.LIGOTimeGPS`, `float`, optional
             the epoch of these data, only used for metadata in the output
             `TimeSeries`, and not requires if the input `fseries` has the
             epoch populated.
 
-        search : `~pdpy.segments.Segment`, optional
+        search : `~pydischarge.segments.Segment`, optional
             search window of interest to determine the loudest Q-plane
 
         Returns
         -------
         results : `QGram`
             the complex energies of the Q-transform of the input `fseries`
             at each frequency
@@ -399,30 +399,30 @@
         return (int((pad - 1)/2.), int((pad + 1)/2.))
 
     def transform(self, fseries, norm=True, epoch=None):
         """Calculate the energy `TimeSeries` for the given fseries
 
         Parameters
         ----------
-        fseries : `~pdpy.frequencyseries.FrequencySeries`
+        fseries : `~pydischarge.frequencyseries.FrequencySeries`
             the complex FFT of a time-series data set
 
         norm : `bool`, `str`, optional
             normalize the energy of the output by the median (if `True` or
             ``'median'``) or the ``'mean'``, if `False` the output
             is the energy (power) of the Q-tranform
 
-        epoch : `~pdpy.time.LIGOTimeGPS`, `float`, optional
+        epoch : `~pydischarge.time.LIGOTimeGPS`, `float`, optional
             the epoch of these data, only used for metadata in the output
             `TimeSeries`, and not requires if the input `fseries` has the
             epoch populated.
 
         Returns
         -------
-        energy : `~pdpy.timeseries.TimeSeries`
+        energy : `~pydischarge.timeseries.TimeSeries`
             a `TimeSeries` of the energy from the Q-transform of
             this tile against the data.
         """
         from ..timeseries import TimeSeries
 
         windowed = fseries[self.get_data_indices()] * self.get_window()
         # pad data, move negative frequencies to the end, and IFFT
@@ -457,15 +457,15 @@
     ----------
     plane : `QPlane`
         the time-frequency plane over which to populate
 
     energies : `list` of `TimeSeries`
         a list of signal energies for each row of tiles
 
-    search : `~pdpy.segments.Segment`, optional
+    search : `~pydischarge.segments.Segment`, optional
         search window of interest to determine the loudest tile
     """
     def __init__(self, plane, energies, search):
         self.plane = plane
         self.energies = energies
         self.peak = self._find_peak(search)
 
@@ -501,21 +501,21 @@
             give `None` to skip this step and return the original resolution,
             default is 0.5 Hz or 500 frequency samples
 
         logf : `bool`, optional
             boolean switch to enable (`True`) or disable (`False`) use of
             log-sampled frequencies in the output `Spectrogram`
 
-        outseg : `~pdpy.segments.Segment`, optional
+        outseg : `~pydischarge.segments.Segment`, optional
             GPS `[start, stop)` segment for output `Spectrogram`,
             default is the full duration of the input
 
         Returns
         -------
-        out : `~pdpy.spectrogram.Spectrogram`
+        out : `~pydischarge.spectrogram.Spectrogram`
             output `Spectrogram` of normalised Q energy
 
         See also
         --------
         scipy.interpolate
             this method uses `~scipy.interpolate.InterpolatedUnivariateSpline`
             to cast all frequency rows to a common time-axis, and then
@@ -524,15 +524,15 @@
 
         Notes
         -----
         This method will return a `Spectrogram` of dtype ``float32`` if
         ``norm`` is given, and ``float64`` otherwise.
 
         To optimize plot rendering with `~matplotlib.axes.Axes.pcolormesh`,
-        the output `~pdpy.spectrogram.Spectrogram` can be given a log-sampled
+        the output `~pydischarge.spectrogram.Spectrogram` can be given a log-sampled
         frequency axis by passing `logf=True` at runtime. The `fres` argument
         is then the number of points on the frequency axis. Note, this is
         incompatible with `~matplotlib.axes.Axes.imshow`.
 
         It is also highly recommended to use the `outseg` keyword argument
         when only a small window around a given GPS time is of interest.
         """
@@ -599,15 +599,15 @@
         ----------
         snrthresh : `float`, optional
             lower inclusive threshold on individual tile SNR to keep in the
             table, default: 5.5
 
         Returns
         -------
-        out : `~pdpy.table.EventTable`
+        out : `~pydischarge.table.EventTable`
             a table of time-frequency tiles on this `QPlane`
 
         Notes
         -----
         Only tiles with signal energy greater than or equal to
         `snrthresh ** 2 / 2` will be stored in the output `EventTable`.
         """
@@ -639,19 +639,19 @@
 def q_scan(data, mismatch=DEFAULT_MISMATCH, qrange=DEFAULT_QRANGE,
            frange=DEFAULT_FRANGE, duration=None, sampling=None,
            **kwargs):
     """Transform data by scanning over a `QTiling`
 
     This utility is provided mainly to allow direct manipulation of the
     `QTiling.transform` output. Most users probably just want to use
-    :meth:`~pdpy.timeseries.TimeSeries.q_transform`, which wraps around this.
+    :meth:`~pydischarge.timeseries.TimeSeries.q_transform`, which wraps around this.
 
     Parameters
     ----------
-    data : `~pdpy.timeseries.TimeSeries` or `ndarray`
+    data : `~pydischarge.timeseries.TimeSeries` or `ndarray`
         the time- or frequency-domain input data
 
     mismatch : `float`, optional
         maximum allowed fractional mismatch between neighbouring tiles
 
     qrange : `tuple` of `float`, optional
         `(low, high)` range of Qs to scan
@@ -674,15 +674,15 @@
     qgram : `QGram`
         the raw output of :meth:`QTiling.transform`
 
     far : `float`
         expected false alarm rate (Hertz) of white Gaussian noise with the
         same peak energy and total duration as `qgram`
     """
-    from pdpy.timeseries import TimeSeries
+    from pydischarge.timeseries import TimeSeries
     # prepare input
     if isinstance(data, TimeSeries):
         duration = abs(data.span)
         sampling = data.sample_rate.to('Hz').value
         kwargs.update({'epoch': data.t0.value})
         data = data.fft().value
     # return a raw Q-transform and its significance
```

### Comparing `pydischarge-0.0.1/pdpy/signal/spectral/__init__.py` & `pydischarge-0.0.2/pydischarge/signal/spectral/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""FFT routines for PDpy
+"""FFT routines for pyDischarge
 
 This sub-package provides PSD estimation routines based on functionality
 provided by :mod:`scipy.signal`.
 
 The methods provided here aren't meant to be called directly by the user,
-but rather via instance methods of the :class:`~pdpy.timeseries.TimeSeries`
+but rather via instance methods of the :class:`~pydischarge.timeseries.TimeSeries`
 object.
 """
 
 from ...utils.decorators import deprecated_function
 from ._registry import (get_method, register_method)
 from ._scipy import (
     bartlett,
@@ -48,17 +48,17 @@
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 
 @deprecated_function
 def get_default_fft_api():
     """Return the preferred FFT-API library
 
-    As of pdpy > 0.14.0|1.0.0 this always returns 'scipy'
+    As of pydischarge > 0.14.0|1.0.0 this always returns 'scipy'
     This is referenced to set the default methods for
-    `~pdpy.timeseries.TimeSeries` methods (amongst others)
+    `~pydischarge.timeseries.TimeSeries` methods (amongst others)
 
     Examples
     --------
     >>> get_default_fft_api()
     'scipy'
     """
     return 'scipy'
```

### Comparing `pydischarge-0.0.1/pdpy/signal/spectral/_lal.py` & `pydischarge-0.0.2/pydischarge/signal/spectral/_lal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""PDpy API to the LAL FFT routines
+"""pyDischarge API to the LAL FFT routines
 
 See the `LAL TimeFreqFFT.h documentation
 <http://software.ligo.org/docs/lalsuite/lal/group___time_freq_f_f_t__h.html>`_
 for more details
 
 This module is deprecated and will be removed in a future release.
 """
@@ -154,15 +154,15 @@
 
 def _lal_spectrum(timeseries, segmentlength, noverlap=None, method='welch',
                   window=None, plan=None):
     """Generate a PSD `FrequencySeries` using |lal|_
 
     Parameters
     ----------
-    timeseries : `~pdpy.timeseries.TimeSeries`
+    timeseries : `~pydischarge.timeseries.TimeSeries`
         input `TimeSeries` data.
 
     segmentlength : `int`
         number of samples in single average.
 
     method : `str`
         average PSD method
@@ -174,15 +174,15 @@
         window to apply to timeseries prior to FFT
 
     plan : `lal.REAL8FFTPlan`, optional
         LAL FFT plan to use when generating average spectrum
 
     Returns
     -------
-    spectrum : `~pdpy.frequencyseries.FrequencySeries`
+    spectrum : `~pydischarge.frequencyseries.FrequencySeries`
         average power `FrequencySeries`
     """
     import lal
     from ...utils.lal import find_typed_function
 
     # default to 50% overlap
     if noverlap is None:
@@ -245,15 +245,15 @@
 
 
 def welch(timeseries, segmentlength, noverlap=None, window=None, plan=None):
     """Calculate an PSD of this `TimeSeries` using Welch's method
 
     Parameters
     ----------
-    timeseries : `~pdpy.timeseries.TimeSeries`
+    timeseries : `~pydischarge.timeseries.TimeSeries`
         input `TimeSeries` data.
 
     segmentlength : `int`
         number of samples in single average.
 
     noverlap : `int`
         number of samples to overlap between segments, defaults to 50%.
@@ -262,15 +262,15 @@
         window parameters to apply to timeseries prior to FFT
 
     plan : `REAL8FFTPlan`, optional
         LAL FFT plan to use when generating average spectrum
 
     Returns
     -------
-    spectrum : `~pdpy.frequencyseries.FrequencySeries`
+    spectrum : `~pydischarge.frequencyseries.FrequencySeries`
         average power `FrequencySeries`
 
     See also
     --------
     lal.REAL8AverageSpectrumWelch
     """
     return _lal_spectrum(timeseries, segmentlength, noverlap=noverlap,
@@ -279,15 +279,15 @@
 
 def bartlett(timeseries, segmentlength, noverlap=None, window=None, plan=None):
     # pylint: disable=unused-argument
     """Calculate an PSD of this `TimeSeries` using Bartlett's method
 
     Parameters
     ----------
-    timeseries : `~pdpy.timeseries.TimeSeries`
+    timeseries : `~pydischarge.timeseries.TimeSeries`
         input `TimeSeries` data.
 
     segmentlength : `int`
         number of samples in single average.
 
     noverlap : `int`
         number of samples to overlap between segments, defaults to 50%.
@@ -296,15 +296,15 @@
         window parameters to apply to timeseries prior to FFT
 
     plan : `REAL8FFTPlan`, optional
         LAL FFT plan to use when generating average spectrum
 
     Returns
     -------
-    spectrum : `~pdpy.frequencyseries.FrequencySeries`
+    spectrum : `~pydischarge.frequencyseries.FrequencySeries`
         average power `FrequencySeries`
 
     See also
     --------
     lal.REAL8AverageSpectrumWelch
     """
     return _lal_spectrum(timeseries, segmentlength, noverlap=0,
@@ -315,15 +315,15 @@
     """Calculate a PSD of this `TimeSeries` using a median average method
 
     The median average is similar to Welch's method, using a median average
     rather than mean.
 
     Parameters
     ----------
-    timeseries : `~pdpy.timeseries.TimeSeries`
+    timeseries : `~pydischarge.timeseries.TimeSeries`
         input `TimeSeries` data.
 
     segmentlength : `int`
         number of samples in single average.
 
     noverlap : `int`
         number of samples to overlap between segments, defaults to 50%.
@@ -332,15 +332,15 @@
         window parameters to apply to timeseries prior to FFT
 
     plan : `REAL8FFTPlan`, optional
         LAL FFT plan to use when generating average spectrum
 
     Returns
     -------
-    spectrum : `~pdpy.frequencyseries.FrequencySeries`
+    spectrum : `~pydischarge.frequencyseries.FrequencySeries`
         average power `FrequencySeries`
 
     See also
     --------
     lal.REAL8AverageSpectrumMedian
     """
     return _lal_spectrum(timeseries, segmentlength, noverlap=noverlap,
@@ -354,15 +354,15 @@
     The median-mean average method divides overlapping segments into "even"
     and "odd" segments, and computes the bin-by-bin median of the "even"
     segments and the "odd" segments, and then takes the bin-by-bin average
     of these two median averages.
 
     Parameters
     ----------
-    timeseries : `~pdpy.timeseries.TimeSeries`
+    timeseries : `~pydischarge.timeseries.TimeSeries`
         input `TimeSeries` data.
 
     segmentlength : `int`
         number of samples in single average.
 
     noverlap : `int`
         number of samples to overlap between segments, defaults to 50%.
@@ -371,15 +371,15 @@
         window parameters to apply to timeseries prior to FFT
 
     plan : `REAL8FFTPlan`, optional
         LAL FFT plan to use when generating average spectrum
 
     Returns
     -------
-    spectrum : `~pdpy.frequencyseries.FrequencySeries`
+    spectrum : `~pydischarge.frequencyseries.FrequencySeries`
         average power `FrequencySeries`
 
     See also
     --------
     lal.REAL8AverageSpectrumMedianMean
     """
     return _lal_spectrum(timeseries, segmentlength, noverlap=noverlap,
```

### Comparing `pydischarge-0.0.1/pdpy/signal/spectral/_median_mean.py` & `pydischarge-0.0.2/pydischarge/signal/spectral/_median_mean.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Hacky registration of median-mean
 
 `scipy.signal` doesn't support median-mean averages, so this module
 maps that name to an actual method provided by one of the other
 FFT-API libraries (e.g. `pycbc`).
```

### Comparing `pydischarge-0.0.1/pdpy/signal/spectral/_pycbc.py` & `pydischarge-0.0.2/pydischarge/signal/spectral/_pycbc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""PDpy API to the pycbc.psd FFT routines
+"""pyDischarge API to the pycbc.psd FFT routines
 
 This module is deprecated and will be removed in a future release.
 """
 
 from contextlib import nullcontext
 
 from ...frequencyseries import FrequencySeries
@@ -31,15 +31,15 @@
 
 
 def welch(timeseries, segmentlength, noverlap=None, scheme=None, **kwargs):
     """Calculate a PSD using Welch's method with a mean average
 
     Parameters
     ----------
-    timeseries : `~pdpy.timeseries.TimeSeries`
+    timeseries : `~pydischarge.timeseries.TimeSeries`
         input `TimeSeries` data.
 
     segmentlength : `int`
         number of samples in single average.
 
     noverlap : `int`
         number of samples to overlap between segments, defaults to 50%.
@@ -48,15 +48,15 @@
         processing scheme in which to execute FFT, default: `None`
 
     **kwargs
         other keyword arguments to pass to :func:`pycbc.psd.welch`
 
     Returns
     -------
-    spectrum : `~pdpy.frequencyseries.FrequencySeries`
+    spectrum : `~pydischarge.frequencyseries.FrequencySeries`
         average power `FrequencySeries`
 
     See also
     --------
     pycbc.psd.welch
     """
     from pycbc.psd import welch as pycbc_welch
@@ -71,15 +71,15 @@
     # generate pycbc FrequencySeries
     with scheme:
         pycbc_fseries = pycbc_welch(timeseries.to_pycbc(copy=False),
                                     seg_len=segmentlength,
                                     seg_stride=segmentlength-noverlap,
                                     **kwargs)
 
-    # return PDpy FrequencySeries
+    # return pyDischarge FrequencySeries
     fseries = FrequencySeries.from_pycbc(pycbc_fseries, copy=False)
     fseries.name = timeseries.name
     fseries.override_unit(scale_timeseries_unit(
         timeseries.unit, scaling='density'))
     return fseries
```

### Comparing `pydischarge-0.0.1/pdpy/signal/spectral/_registry.py` & `pydischarge-0.0.2/pydischarge/signal/spectral/_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2013-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Registry for FFT averaging methods
 """
 
 from collections import OrderedDict
 
 from ...utils.decorators import deprecated_function
```

### Comparing `pydischarge-0.0.1/pdpy/signal/spectral/_scipy.py` & `pydischarge-0.0.2/pydischarge/signal/spectral/_scipy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""PDpy API to the scipy.signal FFT routines
+"""pyDischarge API to the scipy.signal FFT routines
 """
 
 import numpy
 
 import scipy.signal
 
 from ...frequencyseries import FrequencySeries
@@ -91,15 +91,15 @@
 # -- others -------------------------------------------------------------------
 
 def rayleigh(timeseries, segmentlength, noverlap=0, window='hann'):
     """Calculate a Rayleigh statistic spectrum
 
     Parameters
     ----------
-    timeseries : `~pdpy.timeseries.TimeSeries`
+    timeseries : `~pydischarge.timeseries.TimeSeries`
         input `TimeSeries` data.
 
     segmentlength : `int`
         number of samples in single average.
 
     noverlap : `int`
         number of samples to overlap between segments, passing `None` will
@@ -108,15 +108,15 @@
     window : `str`, `numpy.ndarray`, optional
         window function to apply to ``timeseries`` prior to FFT,
         see :func:`scipy.signal.get_window` for details on acceptable
         formats
 
     Returns
     -------
-    spectrum : `~pdpy.frequencyseries.FrequencySeries`
+    spectrum : `~pydischarge.frequencyseries.FrequencySeries`
         average power `FrequencySeries`
     """
     stepsize = segmentlength - noverlap
     if noverlap:
         numsegs = 1 + int((timeseries.size - segmentlength) / float(noverlap))
     else:
         numsegs = int(timeseries.size // segmentlength)
@@ -135,32 +135,32 @@
 
 
 def csd(timeseries, other, segmentlength, noverlap=None, **kwargs):
     """Calculate the CSD of two `TimeSeries` using Welch's method
 
     Parameters
     ----------
-    timeseries : `~pdpy.timeseries.TimeSeries`
+    timeseries : `~pydischarge.timeseries.TimeSeries`
         time-series of data
 
-    other : `~pdpy.timeseries.TimeSeries`
+    other : `~pydischarge.timeseries.TimeSeries`
         time-series of data
 
     segmentlength : `int`
         number of samples in single average.
 
     noverlap : `int`
         number of samples to overlap between segments, defaults to 50%.
 
     **kwargs
         other keyword arguments are passed to :meth:`scipy.signal.csd`
 
     Returns
     -------
-    spectrum : `~pdpy.frequencyseries.FrequencySeries`
+    spectrum : `~pydischarge.frequencyseries.FrequencySeries`
         average power `FrequencySeries`
 
     See also
     --------
     scipy.signal.csd
     """
     # calculate CSD
@@ -172,32 +172,32 @@
 
 
 def coherence(timeseries, other, segmentlength, noverlap=None, **kwargs):
     """Calculate the coherence between two `TimeSeries` using Welch's method
 
     Parameters
     ----------
-    timeseries : `~pdpy.timeseries.TimeSeries`
+    timeseries : `~pydischarge.timeseries.TimeSeries`
         time-series of data
 
-    other : `~pdpy.timeseries.TimeSeries`
+    other : `~pydischarge.timeseries.TimeSeries`
         time-series of data
 
     segmentlength : `int`
         number of samples in single average.
 
     noverlap : `int`
         number of samples to overlap between segments, defaults to 50%.
 
     **kwargs
         other keyword arguments are passed to :meth:`scipy.signal.coherence`
 
     Returns
     -------
-    spectrum : `~pdpy.frequencyseries.FrequencySeries`
+    spectrum : `~pydischarge.frequencyseries.FrequencySeries`
         average power `FrequencySeries`
 
     See also
     --------
     scipy.signal.coherence
     """
     # calculate CSD
```

### Comparing `pydischarge-0.0.1/pdpy/signal/spectral/_ui.py` & `pydischarge-0.0.2/pydischarge/signal/spectral/_ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""User-interface to FFT routines for PDpy
+"""User-interface to FFT routines for pyDischarge
 
 This module provides the methods that eventually get called by TimeSeries.xxx,
 so isn't really for direct user interaction.
 """
 
 from functools import wraps
 
@@ -84,27 +84,27 @@
     recommended overlap for that window type, if ``overlap`` is not given.
 
     If a ``window`` is given as a `str`, it will be converted to a
     `numpy.ndarray` containing the correct window (of the correct length).
 
     Parameters
     ----------
-    series : `pdpy.timeseries.TimeSeries`
+    series : `pydischarge.timeseries.TimeSeries`
         the data that will be processed using an FFT-based method
 
     kwargs : `dict`
         the dict of keyword arguments passed by the user
 
     func : `callable`, optional
         the FFT method that will be called
 
     Examples
     --------
     >>> from numpy.random import normal
-    >>> from pdpy.timeseries import TimeSeries
+    >>> from pydischarge.timeseries import TimeSeries
     >>> normalize_fft_params(TimeSeries(normal(size=1024), sample_rate=256))
     {'nfft': 1024, 'noverlap': 0}
     >>> normalize_fft_params(TimeSeries(normal(size=1024), sample_rate=256),
     ...                      {'window': 'hann'})
     {'window': array([  0.00000000e+00,   9.41235870e-06, ...,
          3.76490804e-05,   9.41235870e-06]), 'noverlap': 0, 'nfft': 1024}
     """
@@ -245,15 +245,15 @@
 def psd(timeseries, method_func, *args, **kwargs):
     """Generate a PSD using a method function
 
     All arguments are presumed to be given in physical units
 
     Parameters
     ----------
-    timeseries : `~pdpy.timeseries.TimeSeries`, `tuple`
+    timeseries : `~pydischarge.timeseries.TimeSeries`, `tuple`
         the data to process, or a 2-tuple of series to correlate
 
     method_func : `callable`
         the function that will be called to perform the signal processing
 
     *args, **kwargs
         other arguments to pass to ``method_func`` when calling
@@ -265,15 +265,15 @@
 def _psdn(timeseries, method_func, *args, **kwargs):
     """Generate a PSD using a method function with FFT arguments in samples
 
     All arguments are presumed to be in sample counts, not physical units
 
     Parameters
     ----------
-    timeseries : `~pdpy.timeseries.TimeSeries`, `tuple`
+    timeseries : `~pydischarge.timeseries.TimeSeries`, `tuple`
         the data to process, or a 2-tuple of series to correlate
 
     method_func : `callable`
         the function that will be called to perform the signal processing
 
     *args, **kwargs
         other arguments to pass to ``method_func`` when calling
```

### Comparing `pydischarge-0.0.1/pdpy/signal/spectral/_utils.py` & `pydischarge-0.0.2/pydischarge/signal/spectral/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utilities for FFT routines
 """
 
 from astropy import units
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
```

### Comparing `pydischarge-0.0.1/pdpy/signal/tests/__init__.py` & `pydischarge-0.0.2/pydischarge/utils/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) Duncan Macleod (2018-2020)
+# Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.signal`
+"""Miscellaneous utilties for pyDischarge
 """
+
+from sys import stdout
+
+from .misc import (
+    gprint,
+    if_not_none,
+    null_context,
+    round_to_power,
+    unique,
+)
+
+__author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
```

### Comparing `pydischarge-0.0.1/pdpy/signal/tests/test_filter_design.py` & `pydischarge-0.0.2/pydischarge/signal/tests/test_filter_design.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.signal.filter_design`
+"""Unit tests for :mod:`pydischarge.signal.filter_design`
 """
 
 import pytest
 
 import numpy
 
 from scipy import signal
```

### Comparing `pydischarge-0.0.1/pdpy/signal/tests/test_qtransform.py` & `pydischarge-0.0.2/pydischarge/signal/tests/test_qtransform.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Alex Urban (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.signal.qtransform`
+"""Unit tests for :mod:`pydischarge.signal.qtransform`
 """
 
 import numpy
 from numpy import testing as nptest
 from scipy.signal import gausspulse
 
 from .. import qtransform
```

### Comparing `pydischarge-0.0.1/pdpy/signal/tests/test_spectral_lal.py` & `pydischarge-0.0.2/pydischarge/signal/tests/test_spectral_lal.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2013-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Unit test for signal module
 """
 
 import pytest
 
 from ..spectral import _lal as fft_lal
 
 lal = pytest.importorskip("lal")
 
 
 def test_generate_window():
-    """Test :func:`pdpy.signal.spectral.lal.generate_window`
+    """Test :func:`pydischarge.signal.spectral.lal.generate_window`
     """
     # test default arguments
     w = fft_lal.generate_window(128)
     assert isinstance(w, lal.REAL8Window)
     assert w.data.data.size == 128
     assert w.sum == 32.31817089602309
     # test generating the same window again returns the same object
@@ -44,15 +44,15 @@
     with pytest.raises(ValueError):
         fft_lal.generate_window(128, 'unknown')
     with pytest.raises(AttributeError):
         fft_lal.generate_window(128, dtype=int)
 
 
 def test_generate_fft_plan():
-    """Test :func:`pdpy.signal.spectral.lal.generate_fft_plan`
+    """Test :func:`pydischarge.signal.spectral.lal.generate_fft_plan`
     """
     # test default arguments
     plan = fft_lal.generate_fft_plan(128)
     assert isinstance(plan, lal.REAL8FFTPlan)
     # test generating the same fft_plan again returns the same object
     assert fft_lal.generate_fft_plan(128) is plan
     # test dtype works
```

### Comparing `pydischarge-0.0.1/pdpy/signal/tests/test_spectral_median_mean.py` & `pydischarge-0.0.2/pydischarge/signal/tests/test_spectral_median_mean.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit test for :mod:`pdpy.signal.spectral._median_mean`
+"""Unit test for :mod:`pydischarge.signal.spectral._median_mean`
 """
 
 from unittest import mock
 
 import pytest
 
 from ..spectral import _median_mean as fft_median_mean
 
 
 @pytest.mark.requires("lal", "pycbc.psd")
 @mock.patch(
-    "pdpy.signal.spectral._pycbc.welch",
+    "pydischarge.signal.spectral._pycbc.welch",
     side_effect=(None, ImportError, ImportError),
 )
 @mock.patch(
-    "pdpy.signal.spectral._lal._lal_spectrum",
+    "pydischarge.signal.spectral._lal._lal_spectrum",
     side_effect=(None, ImportError),
 )
 def test_median_mean(lal_func, pycbc_func):
     """Check that the registered "median-mean" method works
 
     Should resolve in this order to
```

### Comparing `pydischarge-0.0.1/pdpy/signal/tests/test_spectral_pycbc.py` & `pydischarge-0.0.2/pydischarge/signal/tests/test_spectral_pycbc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2019-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.signal.spectral.pycbc`
+"""Tests for :mod:`pydischarge.signal.spectral.pycbc`
 
 Here we check `welch` thoroughly, and the others less so, because
 they just call out to that method anyway.
 """
 
 import pytest
```

### Comparing `pydischarge-0.0.1/pdpy/signal/tests/test_spectral_registry.py` & `pydischarge-0.0.2/pydischarge/signal/tests/test_spectral_registry.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2019-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.signal.spectral.registry`
+"""Tests for :mod:`pydischarge.signal.spectral.registry`
 """
 
 import pytest
 
 from ..spectral import _registry as fft_registry
 
 
@@ -28,15 +28,15 @@
     # remove test methods from registry
     # otherwise they will impact other tests, and test ordering
     # is annoying to predict
     fft_registry.METHODS.pop('fake_method', '')
 
 
 def test_register_get():
-    """Test :mod:`pdpy.signal.spectral.registry`
+    """Test :mod:`pydischarge.signal.spectral.registry`
     """
     def fake_method():
         pass
 
     # test register
     fft_registry.register_method(fake_method)
     assert 'fake_method' in fft_registry.METHODS
```

### Comparing `pydischarge-0.0.1/pdpy/signal/tests/test_spectral_scipy.py` & `pydischarge-0.0.2/pydischarge/signal/tests/test_spectral_scipy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2019-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.signal.spectral.scipy`
+"""Tests for :mod:`pydischarge.signal.spectral.scipy`
 
 Here we check `welch` thoroughly, and the others less so, because
 they just call out to the same method anyway.
 """
 
 import pytest
```

### Comparing `pydischarge-0.0.1/pdpy/signal/tests/test_spectral_ui.py` & `pydischarge-0.0.2/pydischarge/signal/tests/test_spectral_ui.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2013-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Unit test for signal module
 """
 
 import numpy
 
 import pytest
@@ -32,24 +32,24 @@
     assert_quantity_sub_equal,
 )
 from ...timeseries import TimeSeries
 from ..spectral import _ui as fft_ui
 
 
 def test_seconds_to_samples():
-    """Test :func:`pdpy.signal.spectral.ui.seconds_to_samples`
+    """Test :func:`pydischarge.signal.spectral.ui.seconds_to_samples`
     """
     assert fft_ui.seconds_to_samples(4, 256) == 1024
     assert fft_ui.seconds_to_samples(1 * units.minute, 16) == 960
     assert fft_ui.seconds_to_samples(
         4 * units.second, 16.384 * units.kiloHertz) == 65536
 
 
 def test_normalize_fft_params():
-    """Test :func:`pdpy.signal.spectral.ui.normalize_fft_params`
+    """Test :func:`pydischarge.signal.spectral.ui.normalize_fft_params`
     """
     ftp = fft_ui.normalize_fft_params(
         TimeSeries(numpy.zeros(1024), sample_rate=256))
     assert ftp == {'nfft': 1024, 'noverlap': 0}
 
 
 def test_normalize_fft_params_window_str():
@@ -75,25 +75,25 @@
 @pytest.mark.requires("lal")
 @pytest.mark.parametrize("win", [
     "hann",
     signal.get_window(("kaiser", 14), 1024),
 ])
 def test_normalize_fft_params_window_lal(win):
     import lal
-    from pdpy.signal.spectral._lal import welch
+    from pydischarge.signal.spectral._lal import welch
     ftp = fft_ui.normalize_fft_params(
         TimeSeries(numpy.zeros(1024, dtype="float32"), sample_rate=256),
         kwargs={'window': win},
         func=welch,
     )
     assert isinstance(ftp.pop("window"), lal.REAL4Window)
 
 
 def test_chunk_timeseries():
-    """Test :func:`pdpy.signal.spectral.ui._chunk_timeseries`
+    """Test :func:`pydischarge.signal.spectral.ui._chunk_timeseries`
     """
     a = TimeSeries(numpy.arange(400))
     chunks = list(fft_ui._chunk_timeseries(a, 100, 50))
     for i, (idxa, idxb) in enumerate([
             (None, 150),
             (75, 225),
             (175, 325),
```

### Comparing `pydischarge-0.0.1/pdpy/signal/tests/test_spectral_utils.py` & `pydischarge-0.0.2/pydischarge/signal/tests/test_spectral_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2013-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Unit test for signal module
 """
 
 import pytest
 
 from astropy import units
 
 from ..spectral import _utils as fft_utils
 
 
 def test_scale_timeseries_unit():
-    """Test :func:`pdpy.signal.spectral.utils.scale_timeseries_units`
+    """Test :func:`pydischarge.signal.spectral.utils.scale_timeseries_units`
     """
     scale_ = fft_utils.scale_timeseries_unit
     u = units.Unit('m')
     # check default
     assert scale_(u) == units.Unit('m^2/Hz')
     # check scaling='density'
     assert scale_(u, scaling='density') == units.Unit('m^2/Hz')
```

### Comparing `pydischarge-0.0.1/pdpy/signal/tests/test_window.py` & `pydischarge-0.0.2/pydischarge/signal/tests/test_window.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.signal.window`
+"""Unit tests for :mod:`pydischarge.signal.window`
 """
 
 import numpy
 import pytest
 
 from scipy.signal import get_window as scipy_get_window
```

### Comparing `pydischarge-0.0.1/pdpy/signal/window.py` & `pydischarge-0.0.2/pydischarge/signal/window.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utilities for signal-processing with windows
 """
 
 from functools import wraps
 from math import ceil
 
@@ -70,15 +70,15 @@
     Raises
     -------
     ValueError
         if ``name`` cannot be resolved to a window function in `scipy.signal`
 
     Examples
     --------
-    >>> from pdpy.signal.window import canonical_name
+    >>> from pydischarge.signal.window import canonical_name
     >>> canonical_name('hann')
     'hann'
     >>> canonical_name('ksr')
     'kaiser'
     """
     if name.lower() == 'planck':  # make sure to handle the Planck window
         return 'planck'
@@ -123,15 +123,15 @@
     -------
     rov : `float`, `int`
         the recommended overlap (ROV) for the given window, in samples if
         ``nfft` is given (`int`), otherwise fractional (`float`)
 
     Examples
     --------
-    >>> from pdpy.signal.window import recommended_overlap
+    >>> from pydischarge.signal.window import recommended_overlap
     >>> recommended_overlap('hann')
     0.5
     >>> recommended_overlap('blackmanharris', nfft=128)
     85
     """
     try:
         name = canonical_name(name)
@@ -170,15 +170,15 @@
         The window, with the maximum value normalized to 1 and at least one
         end tapered smoothly to 0.
 
     Examples
     --------
     To taper 0.1 seconds on both ends of one second of data sampled at 2048 Hz:
 
-    >>> from pdpy.signal.window import planck
+    >>> from pydischarge.signal.window import planck
     >>> w = planck(2048, nleft=205, nright=205)
 
     References
     ----------
     .. [1] McKechan, D.J.A., Robinson, C., and Sathyaprakash, B.S. (April
            2010). "A tapering window for time-domain templates and simulated
            signals in the detection of gravitational waves from coalescing
```

### Comparing `pydischarge-0.0.1/pdpy/spectrogram/__init__.py` & `pydischarge-0.0.2/pydischarge/utils/sphinx/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Create, manipulate, read, and write spectrogram data
+"""Extension for sphinx documentation specific to pyDischarge
 """
-
-from .spectrogram import (Spectrogram, SpectrogramList)
-
-from . import io  # register I/O
-
-__author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
```

### Comparing `pydischarge-0.0.1/pdpy/spectrogram/coherence.py` & `pydischarge-0.0.2/pydischarge/spectrogram/coherence.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module contains the relevant methods to generate a
 time-frequency coherence spectrogram from a pair of time-series.
 """
 
 from multiprocessing import (Process, Queue as ProcessQueue)
 from math import ceil
@@ -29,18 +29,18 @@
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
 
 
 def _from_timeseries(ts1, ts2, stride, fftlength=None, overlap=None,
                      window=None, **kwargs):
     """Generate a time-frequency coherence
-    :class:`~pdpy.spectrogram.Spectrogram` from a pair of
-    :class:`~pdpy.timeseries.TimeSeries`.
+    :class:`~pydischarge.spectrogram.Spectrogram` from a pair of
+    :class:`~pydischarge.timeseries.TimeSeries`.
 
-    For each `stride`, a PSD :class:`~pdpy.frequencyseries.FrequencySeries`
+    For each `stride`, a PSD :class:`~pydischarge.frequencyseries.FrequencySeries`
     is generated, with all resulting spectra stacked in time and returned.
     """
     # check sampling rates
     if ts1.sample_rate.to('Hertz') != ts2.sample_rate.to('Hertz'):
         sampling = min(ts1.sample_rate.value, ts2.sample_rate.value)
         # resample higher rate series
         if ts1.sample_rate.value == sampling:
@@ -86,15 +86,15 @@
 
 def from_timeseries(ts1, ts2, stride, fftlength=None, overlap=None,
                     window=None, nproc=1, **kwargs):
     """Calculate the coherence `Spectrogram` between two `TimeSeries`.
 
     Parameters
     ----------
-    timeseries : :class:`~pdpy.timeseries.TimeSeries`
+    timeseries : :class:`~pydischarge.timeseries.TimeSeries`
         input time-series to process.
     stride : `float`
         number of seconds in single PSD (column of spectrogram).
     fftlength : `float`
         number of seconds in single FFT.
     overlap : `int`, optiona, default: fftlength
         number of seconds of overlap between FFTs, defaults to no overlap
@@ -102,15 +102,15 @@
         window function to apply to timeseries prior to FFT.
     nproc : `int`, default: ``1``
         maximum number of independent frame reading processes, default
         is set to single-process file reading.
 
     Returns
     -------
-    spectrogram : :class:`~pdpy.spectrogram.Spectrogram`
+    spectrogram : :class:`~pydischarge.spectrogram.Spectrogram`
         time-frequency power spectrogram as generated from the
         input time-series.
     """
     # format FFT parameters
     if fftlength is None:
         fftlength = stride / 2.
```

### Comparing `pydischarge-0.0.1/pdpy/spectrogram/io/__init__.py` & `pydischarge-0.0.2/pydischarge/segments/tests/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) Duncan Macleod (2014-2020)
+# Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Input/Output routines for the Spectrogram.
+"""Tests for :mod:`pydischarge.segments`
 """
-
-from . import (
-    hdf5
-)
-
-__author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
```

### Comparing `pydischarge-0.0.1/pdpy/spectrogram/io/hdf5.py` & `pydischarge-0.0.2/pydischarge/utils/tests/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) Duncan Macleod (2014-2020)
+# Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""This module attaches the HDF5 input output methods to the Spectrogram.
+"""Tests for :mod:`pydischarge.utils`
 """
-
-from ...types.io.hdf5 import register_hdf5_array_io
-from .. import Spectrogram
-
-__author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
-
-register_hdf5_array_io(Spectrogram)
```

### Comparing `pydischarge-0.0.1/pdpy/spectrogram/spectrogram.py` & `pydischarge-0.0.2/pydischarge/spectrogram/spectrogram.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2022)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Spectrogram object
 """
 
 import warnings
 
 import numpy
@@ -66,17 +66,17 @@
     ----------
     value : array-like
         input data array
 
     unit : `~astropy.units.Unit`, optional
         physical unit of these data
 
-    epoch : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+    epoch : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
         GPS epoch associated with these data,
-        any input parsable by `~pdpy.time.to_gps` is fine
+        any input parsable by `~pydischarge.time.to_gps` is fine
 
     sample_rate : `float`, `~astropy.units.Quantity`, optional, default: `1`
         the rate of samples per second (Hertz)
 
     times : `array-like`
         the complete array of GPS times accompanying the data for this series.
         This argument takes precedence over `epoch` and `sample_rate` so should
@@ -89,22 +89,22 @@
         frequency resolution for these data
 
     frequencies : `array-like`
         the complete array of frequencies indexing the data.
         This argument takes precedence over `f0` and `df` so should
         be given in place of these if relevant, not alongside
 
-    epoch : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+    epoch : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
         GPS epoch associated with these data,
-        any input parsable by `~pdpy.time.to_gps` is fine
+        any input parsable by `~pydischarge.time.to_gps` is fine
 
     name : `str`, optional
         descriptive title for this array
 
-    channel : `~pdpy.detector.Channel`, `str`, optional
+    channel : `~pydischarge.detector.Channel`, `str`, optional
         source data stream for these data
 
     dtype : `~numpy.dtype`, optional
         input data type
 
     copy : `bool`, optional, default: `False`
         choose to copy the input data to new memory
@@ -163,15 +163,15 @@
 
     # -- Spectrogram properties -----------------
 
     epoch = property(TimeSeries.epoch.__get__, TimeSeries.epoch.__set__,
                      TimeSeries.epoch.__delete__,
                      """Starting GPS epoch for this `Spectrogram`
 
-                     :type: `~pdpy.segments.Segment`
+                     :type: `~pydischarge.segments.Segment`
                      """)
 
     t0 = property(TimeSeries.t0.__get__, TimeSeries.t0.__set__,
                   TimeSeries.t0.__delete__,
                   """GPS time of first time bin
 
                   :type: `~astropy.units.Quantity` in seconds
@@ -184,15 +184,15 @@
                   :type: `~astropy.units.Quantity` in seconds
                   """)
 
     span = property(TimeSeries.span.__get__, TimeSeries.span.__set__,
                     TimeSeries.span.__delete__,
                     """GPS [start, stop) span for this `Spectrogram`
 
-                    :type: `~pdpy.segments.Segment`
+                    :type: `~pydischarge.segments.Segment`
                     """)
 
     f0 = property(Array2D.y0.__get__, Array2D.y0.__set__,
                   Array2D.y0.__delete__,
                   """Starting frequency for this `Spectrogram`
 
                   :type: `~astropy.units.Quantity` in Hertz
@@ -284,15 +284,15 @@
 
     def ratio(self, operand):
         """Calculate the ratio of this `Spectrogram` against a reference
 
         Parameters
         ----------
         operand : `str`, `FrequencySeries`, `Quantity`
-            a `~pdpy.frequencyseries.FrequencySeries` or
+            a `~pydischarge.frequencyseries.FrequencySeries` or
             `~astropy.units.Quantity` to weight against, or one of
 
             - ``'mean'`` : weight against the mean of each spectrum
               in this Spectrogram
             - ``'median'`` : weight against the median of each spectrum
               in this Spectrogram
 
@@ -341,27 +341,27 @@
 
         **kwargs
             all keyword arguments are passed along to underlying
             functions, see below for references
 
         Returns
         -------
-        plot : `~pdpy.plot.Plot`
+        plot : `~pydischarge.plot.Plot`
             the `Plot` containing the data
 
         See also
         --------
         matplotlib.pyplot.figure
             for documentation of keyword arguments used to create the
             figure
         matplotlib.figure.Figure.add_subplot
             for documentation of keyword arguments used to create the
             axes
-        pdpy.plot.Axes.imshow
-        pdpy.plot.Axes.pcolormesh
+        pydischarge.plot.Axes.imshow
+        pydischarge.plot.Axes.pcolormesh
             for documentation of keyword arguments used in rendering the
             `Spectrogram` data
         """
         return super().plot(
             method=method,
             figsize=figsize,
             xscale=xscale,
@@ -371,28 +371,28 @@
     @classmethod
     def from_spectra(cls, *spectra, **kwargs):
         """Build a new `Spectrogram` from a list of spectra.
 
         Parameters
         ----------
         *spectra
-            any number of `~pdpy.frequencyseries.FrequencySeries` series
+            any number of `~pydischarge.frequencyseries.FrequencySeries` series
         dt : `float`, `~astropy.units.Quantity`, optional
             stride between given spectra
 
         Returns
         -------
         Spectrogram
             a new `Spectrogram` from a vertical stacking of the spectra
             The new object takes the metadata from the first given
-            `~pdpy.frequencyseries.FrequencySeries` if not given explicitly
+            `~pydischarge.frequencyseries.FrequencySeries` if not given explicitly
 
         Notes
         -----
-        Each `~pdpy.frequencyseries.FrequencySeries` passed to this
+        Each `~pydischarge.frequencyseries.FrequencySeries` passed to this
         constructor must be the same length.
         """
         data = numpy.vstack([s.value for s in spectra])
         spec1 = list(spectra)[0]
         if not all(s.f0 == spec1.f0 for s in spectra):
             raise ValueError("Cannot stack spectra with different f0")
         if not all(s.df == spec1.df for s in spectra):
@@ -417,15 +417,15 @@
         Parameters
         ----------
         percentile : `float`
             percentile (0 - 100) of the bins to compute
 
         Returns
         -------
-        spectrum : `~pdpy.frequencyseries.FrequencySeries`
+        spectrum : `~pydischarge.frequencyseries.FrequencySeries`
             the given percentile `FrequencySeries` calculated from this
             `SpectralVaraicence`
         """
         out = numpy.percentile(self.value, percentile, axis=0)
         if self.name is not None:
             name = '{}: {} percentile'.format(self.name, _ordinal(percentile))
         else:
```

### Comparing `pydischarge-0.0.1/pdpy/spectrogram/tests/test_spectrogram.py` & `pydischarge-0.0.2/pydischarge/spectrogram/tests/test_spectrogram.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.spectrogram.spectrogram`
+"""Unit tests for :mod:`pydischarge.spectrogram.spectrogram`
 """
 
 from io import BytesIO
 
 import pytest
 
 import numpy
@@ -35,15 +35,15 @@
 from ...types.tests.test_array2d import TestArray2D as _TestArray2D
 from .. import Spectrogram
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 
 class TestSpectrogram(_TestArray2D):
-    """Tests of `pdpy.spectrogram.Spectrogram`
+    """Tests of `pydischarge.spectrogram.Spectrogram`
     """
     TEST_CLASS = Spectrogram
 
     def test_new(self):
         super().test_new()
 
         # check handling of epoch vs t0
```

### Comparing `pydischarge-0.0.1/pdpy/table/__init__.py` & `pydischarge-0.0.2/pydischarge/table/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module extends the functionality of the :mod:`astropy.table`
 library for reading/writing/manipulating hetergeneous data tables.
 
 Importing the `~astropy.table.Table` object from here via
 
-    >>> from pdpy.table import Table
+    >>> from pydischarge.table import Table
 
 loads extra input/output definitions available for
 :meth:`~astropy.table.Table.read` and :meth:`~astropy.table.Table.write`.
 
 Additionally, the `EventTable` object is provided to simplify working with
 tables of time-stamped GW (or other) events.
 """
```

### Comparing `pydischarge-0.0.1/pdpy/table/filter.py` & `pydischarge-0.0.2/pydischarge/table/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utilies for filtering a `Table` using column slice definitions
 """
 
 import operator
 import re
 import token
@@ -244,15 +244,15 @@
 
     Examples
     --------
     >>> filter(my_table, 'snr>10', 'frequency<1000')
 
     custom operations can be defined using filter tuple definitions:
 
-    >>> from pdpy.table.filters import in_segmentlist
+    >>> from pydischarge.table.filters import in_segmentlist
     >>> filter(my_table, ('time', in_segmentlist, segs))
     """
     keep = numpy.ones(len(table), dtype=bool)
     for name, op_func, operand in parse_column_filters(*column_filters):
         col = table[name]
         keep &= op_func(col, operand)
     return table[keep]
```

### Comparing `pydischarge-0.0.1/pdpy/table/filters.py` & `pydischarge-0.0.2/pydischarge/table/filters.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Filter functions for use with :meth:`EventTable.filter`
 
 Each of these functions has the same input and output format.
 The inputs must be
 
 - ``columns`` (`str`) : the name of the column to use
@@ -33,15 +33,15 @@
 
 import numpy
 
 
 def in_segmentlist(column, segmentlist):
     """Return the index of values lying inside the given segmentlist
 
-    A `~pdpy.segments.Segment` represents a semi-open interval,
+    A `~pydischarge.segments.Segment` represents a semi-open interval,
     so for any segment `[a, b)`, a value `x` is 'in' the segment if
 
     a <= x < b
     """
     segmentlist = type(segmentlist)(segmentlist).coalesce()
     idx = column.argsort()
     contains = numpy.zeros(column.shape[0], dtype=bool)
@@ -72,10 +72,10 @@
         i += 1
     return contains
 
 
 def not_in_segmentlist(column, segmentlist):
     """Return the index of values not lying inside the given segmentlist
 
-    See :func:`~pdpy.table.filters.in_segmentlist` for more details
+    See :func:`~pydischarge.table.filters.in_segmentlist` for more details
     """
     return in_segmentlist(column, ~segmentlist)
```

### Comparing `pydischarge-0.0.1/pdpy/table/gravityspy.py` & `pydischarge-0.0.2/pydischarge/table/gravityspy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Scott Coughlin (2017-2021)
 #               Cardiff University (2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Extend :mod:`astropy.table` with the `GravitySpyTable`
 """
 
 import re
 from json import JSONDecodeError
 from pathlib import Path
```

### Comparing `pydischarge-0.0.1/pdpy/table/io/__init__.py` & `pydischarge-0.0.2/pydischarge/table/io/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Input/output methods for tabular data.
 """
 
 # utils.py provides some decorators, but importantly applies those
 # decorators _automatically_ to the existing registered readers
 # provided by astropy, so this needs to come first.
```

### Comparing `pydischarge-0.0.1/pdpy/table/io/cwb.py` & `pydischarge-0.0.2/pydischarge/table/io/cwb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read events from Coherent Wave-Burst (cWB)-format ROOT files.
 """
 
 import re
 
 from astropy.io.ascii import core
```

### Comparing `pydischarge-0.0.1/pdpy/table/io/fetch.py` & `pydischarge-0.0.2/pydischarge/table/io/fetch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Fetch registration for database queries
 """
 
 import re
 
 from astropy.io import registry as io_registry
```

### Comparing `pydischarge-0.0.1/pdpy/table/io/gravityspy.py` & `pydischarge-0.0.2/pydischarge/table/io/gravityspy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Scott Coughlin (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Input/output methods for tabular data.
 
 Access to GravitySpy and O1GlitchClassification triggers requires access
 to a PostgresSQL database. Users can set the username and password for
 connections in the following environment variables
```

### Comparing `pydischarge-0.0.1/pdpy/table/io/gstlal.py` & `pydischarge-0.0.2/pydischarge/table/io/gstlal.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) California Institute of Technology (2019-2022)
 #               Pensylvania State University (2019)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read events from the GstLAL online GW search
 """
 
 import re
 from os.path import basename
 
@@ -49,17 +49,17 @@
         one or more open files, file paths, or LIGO_LW `Document` objects
 
     **kwargs
         keyword arguments for the read, or conversion functions
 
     See also
     --------
-    pdpy.io.ligolw.read_table
+    pydischarge.io.ligolw.read_table
         for details of keyword arguments for the read operation
-    pdpy.table.io.ligolw.to_astropy_table
+    pydischarge.table.io.ligolw.to_astropy_table
         for details of keyword arguments for the conversion operation
     """
     from ligo.lw import lsctables
     extra_cols = []
     derived_cols = []
     val_col = lsctables.TableByName['sngl_inspiral'].validcolumns
     if 'columns' in kwargs:
@@ -95,17 +95,17 @@
         one or more open files, file paths, or LIGO_LW `Document` objects
 
     **kwargs
         keyword arguments for the read, or conversion functions
 
     See also
     --------
-    pdpy.io.ligolw.read_table
+    pydischarge.io.ligolw.read_table
         for details of keyword arguments for the read operation
-    pdpy.table.io.ligolw.to_astropy_table
+    pydischarge.table.io.ligolw.to_astropy_table
         for details of keyword arguments for the conversion operation
     """
     from ligo.lw import lsctables
     extra_cols = []
     if 'columns' in kwargs:
         columns = kwargs['columns']
         kwargs.pop('columns')
@@ -153,17 +153,17 @@
         'coinc' for coincident trigger information
 
     **kwargs
         keyword arguments for the read, or conversion functions
 
     See also
     --------
-    pdpy.io.ligolw.read_table
+    pydischarge.io.ligolw.read_table
         for details of keyword arguments for the read operation
-    pdpy.table.io.ligolw.to_astropy_table
+    pydischarge.table.io.ligolw.to_astropy_table
         for details of keyword arguments for the conversion operation
     """
 
     if triggers == 'sngl':
         return read_gstlal_sngl(source, **kwargs)
     if triggers == 'coinc':
         return read_gstlal_coinc(source, **kwargs)
@@ -188,15 +188,15 @@
 register_reader(GSTLAL_FORMAT, EventTable, read_gstlal)
 
 # -- processed columns --------------------------------------------------------
 #
 # Here we define methods required to build commonly desired columns that
 # are just a combination of the basic columns.
 #
-# Each method should take in a `~pdpy.table.Table` and return a `numpy.ndarray`
+# Each method should take in a `~pydischarge.table.Table` and return a `numpy.ndarray`
 
 GET_COLUMN = {}
 GET_COLUMN_EXTRA = {}
 
 
 def get_snr_chi(events, snr_pow=2., chi_pow=2.):
     """Calculate the 'SNR chi' column for this GstLAL ligolw table group
```

### Comparing `pydischarge-0.0.1/pdpy/table/io/gwf.py` & `pydischarge-0.0.2/pydischarge/table/io/gwf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read events from GWF FrEvent structures into a Table
 """
 
 from astropy.table import Table
 from astropy.io import registry as io_registry
 
@@ -124,16 +124,16 @@
         the name of the file to write into
 
     **kwargs
         other keyword arguments (see below for references)
 
     See also
     --------
-    pdpy.io.gwf.create_frame
-    pdpy.io.gwf.write_frames
+    pydischarge.io.gwf.create_frame
+    pydischarge.io.gwf.write_frames
         for documentation of keyword arguments
     """
     from LDAStools.frameCPP import (FrEvent, GPSTime)
 
     # create frame
     write_kw = {key: kwargs.pop(key) for
                 key in ('compression', 'compression_level') if key in kwargs}
```

### Comparing `pydischarge-0.0.1/pdpy/table/io/hacr.py` & `pydischarge-0.0.2/pydischarge/table/io/hacr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Input/output methods for tabular data.
 
 Access to HACR triggers requires local access to the MySQL database. Users
 can set the IP address of the server, and the username and password for
 connections in the following environment variables
```

### Comparing `pydischarge-0.0.1/pdpy/table/io/ligolw.py` & `pydischarge-0.0.2/pydischarge/table/io/ligolw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read LIGO_LW documents into :class:`~ligo.lw.table.Table` objects.
 """
 
 import numpy
 
 try:
@@ -319,17 +319,17 @@
         be returned if only one exists in the document(s)
 
     **kwargs
         keyword arguments for the read, or conversion functions
 
     See also
     --------
-    pdpy.io.ligolw.read_table
+    pydischarge.io.ligolw.read_table
         for details of keyword arguments for the read operation
-    pdpy.table.io.ligolw.to_astropy_table
+    pydischarge.table.io.ligolw.to_astropy_table
         for details of keyword arguments for the conversion operation
     """
     from ligo.lw import table as ligolw_table
     from ligo.lw.lsctables import TableByName
 
     # -- keyword handling -----------------------
```

### Comparing `pydischarge-0.0.1/pdpy/table/io/losc.py` & `pydischarge-0.0.2/pydischarge/table/io/losc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2019-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Fetch and parse an event catalog from GWOSC.
 """
 import numbers
 from collections import OrderedDict
 
 import numpy
```

### Comparing `pydischarge-0.0.1/pdpy/table/io/omega.py` & `pydischarge-0.0.2/pydischarge/table/io/omega.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read events from an Omega-format ASCII file.
 """
 
 import re
 
 from astropy.io.ascii import core
```

### Comparing `pydischarge-0.0.1/pdpy/table/io/omicron.py` & `pydischarge-0.0.2/pydischarge/table/io/omicron.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read events from an Omicron-format ROOT file.
 """
 
 from ...io import registry
 from .. import EventTable
```

### Comparing `pydischarge-0.0.1/pdpy/table/io/pycbc.py` & `pydischarge-0.0.2/pydischarge/table/io/pycbc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read events from the PyCBC live online GW search
 """
 
 import re
 from os.path import basename
 
@@ -64,15 +64,15 @@
 
     extended_metadata : `bool`, optional
         record non-column datasets found in the H5 group (e.g. ``'psd'``)
         in the ``meta`` dict, default: `True`
 
     Returns
     -------
-    table : `~pdpy.table.EventTable`
+    table : `~pydischarge.table.EventTable`
     """
     # find group
     if isinstance(source, h5py.File):
         source, ifo = _find_table_group(source, ifo=ifo)
 
     # -- by this point 'source' is guaranteed to be an h5py.Group
 
@@ -167,15 +167,15 @@
 
     # get PSD
     try:
         psd = h5group['psd']
     except KeyError:
         pass
     else:
-        from pdpy.frequencyseries import FrequencySeries
+        from pydischarge.frequencyseries import FrequencySeries
         meta['psd'] = FrequencySeries(
             psd[:], f0=0, df=psd.attrs['delta_f'], name='pycbc_live')
 
     # get everything else
     for key in META_COLUMNS - {'psd'}:
         try:
             value = h5group[key][:]
```

### Comparing `pydischarge-0.0.1/pdpy/table/io/root.py` & `pydischarge-0.0.2/pydischarge/table/io/root.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read events from ROOT trees into Tables
 """
 
 from ...io import registry
 from ...io.utils import (file_path, identify_factory)
 from .. import (Table, EventTable)
```

### Comparing `pydischarge-0.0.1/pdpy/table/io/snax.py` & `pydischarge-0.0.2/pydischarge/table/io/snax.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Patrick Godwin (2019-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read events from SNAX
 """
 
 import warnings
 
 from astropy.io.misc.hdf5 import read_table_hdf5
@@ -56,15 +56,15 @@
     compact : `bool`, optional, default: False
         whether to store a compact integer representation in the channel
         column rather than the full channel name, instead storing a mapping
         (`channel_map`) in the table metadata.
 
     Returns
     -------
-    table : `~pdpy.table.EventTable`
+    table : `~pydischarge.table.EventTable`
     """
     # format channels appropriately
     if isinstance(channels, str):
         channels = [channels]
 
     # only query channels contained in file
     # if channels not specified, load all of them
```

### Comparing `pydischarge-0.0.1/pdpy/table/io/sql.py` & `pydischarge-0.0.2/pydischarge/table/io/sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Scott Coughlin (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utilities for database queries
 """
 
 from astropy.table import Table
 
 from ..filter import (OPERATORS, parse_column_filters)
```

### Comparing `pydischarge-0.0.1/pdpy/table/io/utils.py` & `pydischarge-0.0.2/pydischarge/table/io/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utilities for Table I/O
 """
 
 import functools
 
 from astropy.io import registry
@@ -82,15 +82,15 @@
 
 def decorate_registered_reader(
         name,
         data_class=EventTable,
         columns=True,
         selection=True,
 ):
-    """Wrap an existing registered reader to use PDpy's input decorators
+    """Wrap an existing registered reader to use pyDischarge's input decorators
 
     Parameters
     ----------
     name : `str`
         the name of the registered format
 
     data_class : `type`, optional
```

### Comparing `pydischarge-0.0.1/pdpy/table/table.py` & `pydischarge-0.0.2/pydischarge/table/table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2017)
 #               Cardiff University (2017-2022)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Extend :mod:`astropy.table` with the `EventTable`
 """
 
 import warnings
 from functools import wraps
 from operator import attrgetter
@@ -129,15 +129,15 @@
 
     def _is_time_column(self, name):
         """Return `True` if a column in this table represents 'time'
 
         This method checks the name of the column against a hardcoded list
         of time-like names, then checks the `dtype` of the column (or the
         first element in the column) against a hardcoded list of time-like
-        dtypes (`pdpy.time.gps_types`).
+        dtypes (`pydischarge.time.gps_types`).
         """
         # if the name looks like a time column, accept that
         if name.lower() in TIME_LIKE_COLUMN_NAMES:
             return True
 
         # if the dtype of this column looks right, accept that
         if self[name].dtype in gps_types:
@@ -296,15 +296,15 @@
         Returns
         -------
         table : `EventTable`
             a table of events recovered from the remote database
 
         Examples
         --------
-        >>> from pdpy.table import EventTable
+        >>> from pydischarge.table import EventTable
 
         To download a table of all blip glitches from the Gravity Spy database:
 
         >>> EventTable.fetch(
         ...     'gravityspy',
         ...     'glitches',
         ...     selection=['ml_label=Blip', 'ml_confidence>0.9'],
@@ -402,58 +402,58 @@
         """
         return self[name]
 
     # -- extensions -----------------------------
 
     @_rates_preprocess
     def event_rate(self, stride, start=None, end=None, timecolumn=None):
-        """Calculate the rate `~pdpy.timeseries.TimeSeries` for this `Table`.
+        """Calculate the rate `~pydischarge.timeseries.TimeSeries` for this `Table`.
 
         Parameters
         ----------
         stride : `float`
             size (seconds) of each time bin
 
-        start : `float`, `~pdpy.time.LIGOTimeGPS`, optional
-            GPS start epoch of rate `~pdpy.timeseries.TimeSeries`
+        start : `float`, `~pydischarge.time.LIGOTimeGPS`, optional
+            GPS start epoch of rate `~pydischarge.timeseries.TimeSeries`
 
-        end : `float`, `~pdpy.time.LIGOTimeGPS`, optional
-            GPS end time of rate `~pdpy.timeseries.TimeSeries`.
+        end : `float`, `~pydischarge.time.LIGOTimeGPS`, optional
+            GPS end time of rate `~pydischarge.timeseries.TimeSeries`.
             This value will be rounded up to the nearest sample if needed.
 
         timecolumn : `str`, optional
             name of time-column to use when binning events, attempts
             are made to guess this
 
         Returns
         -------
-        rate : `~pdpy.timeseries.TimeSeries`
+        rate : `~pydischarge.timeseries.TimeSeries`
             a `TimeSeries` of events per second (Hz)
 
         Raises
         ------
         ValueError
             if the ``timecolumn`` cannot be guessed from the table contents
         """
         # NOTE: decorator sets timecolumn, start, end to non-None values
-        from pdpy.timeseries import TimeSeries
+        from pydischarge.timeseries import TimeSeries
         times = self[timecolumn]
         if times.dtype.name == 'object':  # cast to ufuncable type
             times = times.astype('longdouble', copy=False)
         nsamp = int(ceil((end - start) / stride))
         timebins = numpy.arange(nsamp + 1) * stride + start
         # create histogram
         return TimeSeries(
             numpy.histogram(times, bins=timebins)[0] / float(stride),
             t0=start, dt=stride, unit='Hz', name='Event rate')
 
     @_rates_preprocess
     def binned_event_rates(self, stride, column, bins, operator='>=',
                            start=None, end=None, timecolumn=None):
-        """Calculate an event rate `~pdpy.timeseries.TimeSeriesDict` over
+        """Calculate an event rate `~pydischarge.timeseries.TimeSeriesDict` over
         a number of bins.
 
         Parameters
         ----------
         stride : `float`
             size (seconds) of each time bin
 
@@ -475,33 +475,33 @@
               against the bin value and returns a boolean.
 
             .. note::
 
                If ``bins`` is given as a list of tuples, this argument
                is ignored.
 
-        start : `float`, `~pdpy.time.LIGOTimeGPS`, optional
-            GPS start epoch of rate `~pdpy.timeseries.TimeSeries`.
+        start : `float`, `~pydischarge.time.LIGOTimeGPS`, optional
+            GPS start epoch of rate `~pydischarge.timeseries.TimeSeries`.
 
-        end : `float`, `~pdpy.time.LIGOTimeGPS`, optional
-            GPS end time of rate `~pdpy.timeseries.TimeSeries`.
+        end : `float`, `~pydischarge.time.LIGOTimeGPS`, optional
+            GPS end time of rate `~pydischarge.timeseries.TimeSeries`.
             This value will be rounded up to the nearest sample if needed.
 
         timecolumn : `str`, optional, default: ``time``
             name of time-column to use when binning events
 
         Returns
         -------
-        rates : ~pdpy.timeseries.TimeSeriesDict`
-            a dict of (bin, `~pdpy.timeseries.TimeSeries`) pairs describing a
+        rates : ~pydischarge.timeseries.TimeSeriesDict`
+            a dict of (bin, `~pydischarge.timeseries.TimeSeries`) pairs describing a
             rate of events per second (Hz) for each of the bins.
         """
         # NOTE: decorator sets timecolumn, start, end to non-None values
 
-        from pdpy.timeseries import TimeSeriesDict
+        from pydischarge.timeseries import TimeSeriesDict
 
         # generate column bins
         if not bins:
             bins = [(-numpy.inf, numpy.inf)]
         if operator == 'in' and not isinstance(bins[0], tuple):
             bins = [(bin_, bins[i+1]) for i, bin_ in enumerate(bins[:-1])]
         elif isinstance(operator, str):
@@ -547,26 +547,26 @@
             name of column by which to color markers
 
         **kwargs
             any other keyword arguments, see below
 
         Returns
         -------
-        plot : `~pdpy.plot.Plot`
+        plot : `~pydischarge.plot.Plot`
             the newly created figure
 
         See also
         --------
         matplotlib.pyplot.figure
             for documentation of keyword arguments used to create the
             figure
         matplotlib.figure.Figure.add_subplot
             for documentation of keyword arguments used to create the
             axes
-        pdpy.plot.Axes.scatter
+        pydischarge.plot.Axes.scatter
             for documentation of keyword arguments used to display the table
         """
         color = kwargs.pop('color', None)
         if color is not None:
             kwargs['c'] = self[color]
         return self._plot('scatter', self[x], self[y], **kwargs)
 
@@ -591,26 +591,26 @@
             name of column by which to color markers
 
         **kwargs
             any other keyword arguments, see below
 
         Returns
         -------
-        plot : `~pdpy.plot.Plot`
+        plot : `~pydischarge.plot.Plot`
             the newly created figure
 
         See also
         --------
         matplotlib.pyplot.figure
             for documentation of keyword arguments used to create the
             figure
         matplotlib.figure.Figure.add_subplot
             for documentation of keyword arguments used to create the
             axes
-        pdpy.plot.Axes.tile
+        pydischarge.plot.Axes.tile
             for documentation of keyword arguments used to display the table
         """
         color = kwargs.pop('color', None)
         if color is not None:
             kwargs['color'] = self[color]
         return self._plot('tile', self[x], self[y], self[w], self[h], **kwargs)
 
@@ -656,26 +656,26 @@
             histogram, default: ``'hist'``.
 
         **kwargs
             Any other keyword arguments, see below.
 
         Returns
         -------
-        plot : `~pdpy.plot.Plot`
+        plot : `~pydischarge.plot.Plot`
             The newly created figure.
 
         See also
         --------
         matplotlib.pyplot.figure
             for documentation of keyword arguments used to create the
             figure.
         matplotlib.figure.Figure.add_subplot
             for documentation of keyword arguments used to create the
             axes.
-        pdpy.plot.Axes.hist
+        pydischarge.plot.Axes.hist
             for documentation of keyword arguments used to display the
             histogram, if the ``method`` keyword is given, this method
             might not actually be the one used.
         """
         from ..plot import Plot
         return Plot(self[column], method='hist', **kwargs)
 
@@ -689,15 +689,15 @@
         ----------
         column_filter : `str`, `tuple`
             a column slice filter definition, e.g. ``'snr > 10``, or
             a filter tuple definition, e.g. ``('snr', <my_func>, <arg>)``
 
         Notes
         -----
-        See :ref:`pdpy-table-filter` for more details on using filter tuples
+        See :ref:`pydischarge-table-filter` for more details on using filter tuples
 
         Returns
         -------
         table : `EventTable`
             a new table with only those rows matching the filters
 
         Examples
@@ -706,15 +706,15 @@
         rows with ``snr`` greater than `10`, and ``frequency`` less than
         `1000`:
 
         >>> table.filter('snr>10', 'frequency<1000')
 
         Custom operations can be defined using filter tuple definitions:
 
-        >>> from pdpy.table.filters import in_segmentlist
+        >>> from pydischarge.table.filters import in_segmentlist
         >>> table.filter(('time', in_segmentlist, segs))
         """
         return filter_table(self, *column_filters)
 
     def cluster(self, index, rank, window):
         """Cluster this `EventTable` over a given column, `index`, maximizing
         over a specified column in the table, `rank`.
```

### Comparing `pydischarge-0.0.1/pdpy/table/tests/__init__.py` & `pydischarge-0.0.2/pydischarge/io/tests/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.table`
+"""Tests for :mod:`pydischarge.io`
 """
```

### Comparing `pydischarge-0.0.1/pdpy/table/tests/test_gravityspy.py` & `pydischarge-0.0.2/pydischarge/table/tests/test_gravityspy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for `pdpy.table.gravityspy`
+"""Unit tests for `pydischarge.table.gravityspy`
 """
 
 import pytest
 
 import requests
 
 from ...testing.errors import pytest_skip_network_error
```

### Comparing `pydischarge-0.0.1/pdpy/table/tests/test_io_gstlal.py` & `pydischarge-0.0.2/pydischarge/table/tests/test_io_gstlal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) California Institute of Technology (2022)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.table.io.gstlal`
+"""Tests for :mod:`pydischarge.table.io.gstlal`
 """
 
 import pytest
 
 from numpy import testing as nptest
 from numpy import float32
 
 from ..io import gstlal as gstlalio
-from pdpy.table import EventTable
+from pydischarge.table import EventTable
 
 __author__ = 'Derek Davis <derek.davis@ligo.org>'
 
 
 # -- gstlal file fixture -----------------------------------------------------
```

### Comparing `pydischarge-0.0.1/pdpy/table/tests/test_io_ligolw.py` & `pydischarge-0.0.2/pydischarge/table/tests/test_io_ligolw.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.table.io.ligolw`
+"""Tests for :mod:`pydischarge.table.io.ligolw`
 """
 
 import pytest
 
 import numpy
 from numpy.testing import assert_array_equal
 
@@ -71,15 +71,15 @@
     assert set(tab.colnames) == {"peak", "ifo"}
     assert tab['peak'].dtype.type is numpy.object_
     assert tab['ifo'].dtype.type is numpy.unicode_
 
 
 @pytest.mark.requires("ligo.lw.lsctables")
 def test_read_process_table():
-    """Regression test against pdpy/pdpy#1367
+    """Regression test against pydischarge/pydischarge#1367
     """
     from ligo.lw.lsctables import (New, ProcessTable)
     llwtable = New(
         ProcessTable,
         columns=["ifos", "username"],
     )
     llwtable.appendRow(instruments=("G1", "H1"), username="testuser")
```

### Comparing `pydischarge-0.0.1/pdpy/table/tests/test_io_pycbc.py` & `pydischarge-0.0.2/pydischarge/table/tests/test_io_pycbc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Cardiff University (2019-2022)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.table.io.pycbc` and its integration with `EventTable`.
+"""Tests for :mod:`pydischarge.table.io.pycbc` and its integration with `EventTable`.
 """
 
 import pytest
 
 import numpy
 from numpy.random import randn
 
@@ -285,15 +285,15 @@
     )
 
 
 def test_read_pycbc_live_regression_1081(
     pycbclivetable,
     pycbclivefile,
 ):
-    """Check against regression of pdpy/pdpy#1081.
+    """Check against regression of pydischarge/pydischarge#1081.
     """
     table = EventTable.read(
         pycbclivefile,
         format='hdf5.pycbc_live',
         ifo='X1',
         selection='snr>.5',
         columns=("a", "b", "snr"),
```

### Comparing `pydischarge-0.0.1/pdpy/table/tests/test_table.py` & `pydischarge-0.0.2/pydischarge/table/tests/test_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for `pdpy.table`
+"""Unit tests for `pydischarge.table`
 """
 
 import os.path
 import re
 from io import BytesIO
 from unittest import mock
 
@@ -83,15 +83,15 @@
 
     # create connection
     conn = mock.MagicMock()
     conn.cursor.return_value = cursor
     return conn
 
 
-# -- pdpy.table.Table (astropy.table.Table) -----------------------------------
+# -- pydischarge.table.Table (astropy.table.Table) -----------------------------------
 
 class TestTable(object):
     TABLE = Table
 
     @classmethod
     def create(cls, n, names, dtypes=None):
         data = []
@@ -518,15 +518,15 @@
         )
         utils.assert_table_equal(
             table,
             table.filter(('time', filters.not_in_segmentlist, SegmentList())),
         )
 
     def test_event_rates(self, table):
-        """Test :meth:`pdpy.table.EventTable.event_rate`
+        """Test :meth:`pydischarge.table.EventTable.event_rate`
         """
         rate = table.event_rate(1)
         assert isinstance(rate, TimeSeries)
         assert rate.sample_rate == 1 * units.Hz
 
     @pytest.mark.requires("lal")
     def test_event_rates_gpsobject(self, table):
```

### Comparing `pydischarge-0.0.1/pdpy/testing/__init__.py` & `pydischarge-0.0.2/pydischarge/types/tests/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Testing utilities for PDpy
+"""Tests for :mod:`pydischarge.types`
 """
```

### Comparing `pydischarge-0.0.1/pdpy/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz` & `pydischarge-0.0.2/pydischarge/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.1/pdpy/testing/data/HLV-HW100916-968654552-1.gwf` & `pydischarge-0.0.2/pydischarge/testing/data/HLV-HW100916-968654552-1.gwf`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.1/pdpy/testing/data/HLV-HW100916-968654552-1.hdf` & `pydischarge-0.0.2/pydischarge/testing/data/HLV-HW100916-968654552-1.hdf`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.1/pdpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.xml.gz` & `pydischarge-0.0.2/pydischarge/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.xml.gz`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.1/pdpy/testing/errors.py` & `pydischarge-0.0.2/pydischarge/testing/errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Cardiff University (2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Error handling for the PDpy test suite
+"""Error handling for the pyDischarge test suite
 """
 
 import socket
 from functools import wraps
 from ssl import SSLError
 from urllib.error import URLError
 
@@ -75,15 +75,15 @@
     return wrapper
 
 
 def pytest_skip_cvmfs_read_error(func):
     """Execute `func` but skip if a CVMFS file fails to open
 
     This is most likely indicative of a broken CVMFS mount, which is not
-    PDpy's problem.
+    pyDischarge's problem.
     """
     @wraps(func)
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except RuntimeError as exc:  # pragma: no cover
             # if function failed to read a CVMFS file, skip
```

### Comparing `pydischarge-0.0.1/pdpy/testing/fixtures.py` & `pydischarge-0.0.2/pydischarge/testing/fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Custom pytest fixtures for PDpy
+"""Custom pytest fixtures for pyDischarge
 
-This module is imported in pdpy.conftest such that all fixtures declared
+This module is imported in pydischarge.conftest such that all fixtures declared
 here are available to test functions/methods by default.
 
 Developer note: **none of the fixtures here should declare autouse=True**.
 """
 
 import pytest
 
@@ -79,15 +79,15 @@
     pytest.param(False, id='no-tex'),
     pytest.param(True, id='usetex', marks=SKIP_TEX)
 ])
 def usetex(request):
     """Repeat a test with matplotlib's `text.usetex` param False and True.
 
     If TeX is not available on the test machine (determined by
-    `pdpy.plot.tex.has_tex()`), the usetex=True tests will be skipped.
+    `pydischarge.plot.tex.has_tex()`), the usetex=True tests will be skipped.
     """
     use_ = request.param
     with rc_context(rc={'text.usetex': use_}):
         yield use_
 
 
 # -- various useful mock data series -----------------------------------------
```

### Comparing `pydischarge-0.0.1/pdpy/testing/marks.py` & `pydischarge-0.0.2/pydischarge/testing/marks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Cardiff University (2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Custom pytest marks for PDpy
+"""Custom pytest marks for pyDischarge
 
 This is mainly to allow downstream users/builders/packagers to skip tests
 that require annoying/flaky configuration, or just take too long, e.g.
 tests that use CVMFS could be skipped via
 
-    $ python -m pytest --pyargs pdpy -m 'not cvmfs'
+    $ python -m pytest --pyargs pydischarge -m 'not cvmfs'
 
-This module is imported in :mod:`pdpy.conftest` such that all marks are
-registered up front and visible via ``python -m pytest pdpy --markers``.
+This module is imported in :mod:`pydischarge.conftest` such that all marks are
+registered up front and visible via ``python -m pytest pydischarge --markers``.
 """
 
 MARKS = {
     "cvmfs": "mark a test as requiring CVMFS",
 }
 
 
 def _register_marks(config):
-    """Register all marks for PDpy
+    """Register all marks for pyDischarge
 
-    This function is designed to be called from :mod:`pdpy.conftest`.
+    This function is designed to be called from :mod:`pydischarge.conftest`.
     """
     for name, doc in MARKS.items():
         config.addinivalue_line(
             "markers",
             "{}: {}".format(name, doc),
         )
```

### Comparing `pydischarge-0.0.1/pdpy/testing/mocks.py` & `pydischarge-0.0.2/pydischarge/testing/mocks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Mock objects for PDpy tests
+"""Mock objects for pyDischarge tests
 """
 
 import inspect
 from unittest import mock
 
 from ..detector import Channel
 from ..time import LIGOTimeGPS
@@ -63,15 +63,15 @@
     channel.data_type = 8
     for attr, value in inspect.getmembers(
             nds2.channel, predicate=lambda x: isinstance(x, int)):
         setattr(channel, attr, value)
     return channel
 
 
-def nds2_connection(host='nds.test.pdpy', port=31200, buffers=[], protocol=2):
+def nds2_connection(host='nds.test.pydischarge', port=31200, buffers=[], protocol=2):
     import nds2
     NdsConnection = mock.create_autospec(nds2.connection)
     try:
         NdsConnection.get_parameter.return_value = False
     except AttributeError:
         # nds2-client < 0.12 doesn't have {get,set}_parameter
         pass
```

### Comparing `pydischarge-0.0.1/pdpy/testing/utils.py` & `pydischarge-0.0.2/pydischarge/testing/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Utilties for the PDpy test suite
+"""Utilties for the pyDischarge test suite
 """
 
 import os.path
 import subprocess
 import tempfile
 from contextlib import contextmanager
 from distutils.version import LooseVersion
@@ -43,16 +43,16 @@
 TEST_GWF_FILE = os.path.join(TEST_DATA_DIR, 'HLV-HW100916-968654552-1.gwf')
 TEST_HDF5_FILE = os.path.join(TEST_DATA_DIR, 'HLV-HW100916-968654552-1.hdf')
 
 
 # -- dependencies -------------------------------------------------------------
 
 @deprecated_function(message=(
-    "pdpy.testing.utils.has is deprecated and will "
-    "be removed in PDpy 3.1.0",
+    "pydischarge.testing.utils.has is deprecated and will "
+    "be removed in pyDischarge 3.1.0",
 ))
 def has(module):  # pragma: no cover
     """Test whether a module is available
 
     Returns `True` if `import module` succeeded, otherwise `False`
     """
     try:
@@ -60,40 +60,40 @@
     except ImportError:
         return False
     else:
         return True
 
 
 @deprecated_function(message=(
-    "pdpy.testing.utils.skip_missing_dependency is deprecated and will "
-    "be removed in PDpy 3.1.0, please update your code to use "
+    "pydischarge.testing.utils.skip_missing_dependency is deprecated and will "
+    "be removed in pyDischarge 3.1.0, please update your code to use "
     "pytest.mark.requires from the pytest-requires package",
 ))
 def skip_missing_dependency(module):  # pragma: no cover
     """Returns a mark generator to skip a test if the dependency is missing
 
     .. deprecated:: 3.0.0
        Use `pytest.mark.requires` from pytest-requires instead.
     """
     return pytest.mark.skipif(not has(module),
                               reason='No module named %s' % module)
 
 
 @deprecated_function(message=(
-    "pdpy.testing.utils.module_older_than is deprecated and will "
-    "be removed in PDpy 3.1.0",
+    "pydischarge.testing.utils.module_older_than is deprecated and will "
+    "be removed in pyDischarge 3.1.0",
 ))
 def module_older_than(module, minversion):  # pragma: no cover
     mod = import_module(module)
     return LooseVersion(mod.__version__) < LooseVersion(minversion)
 
 
 @deprecated_function(message=(
-    "pdpy.testing.utils.skip_minimum_version is deprecated and will "
-    "be removed in PDpy 3.1.0",
+    "pydischarge.testing.utils.skip_minimum_version is deprecated and will "
+    "be removed in pyDischarge 3.1.0",
 ))
 def skip_minimum_version(module, minversion):  # pragma: no cover
     """Returns a mark generator to skip a test if the dependency is too old
 
     .. deprecated:: 3.0.0
     """
     return pytest.mark.skipif(
@@ -145,19 +145,19 @@
 
 def _assert_quantity(q1, q2, array_assertion=assert_array_equal):
     assert q1.unit == q2.unit, "%r != %r" % (q1.unit, q2.unit)
     array_assertion(q1.value, q2.value)
 
 
 def assert_quantity_sub_equal(a, b, *attrs, **kwargs):
-    """Assert that two `~pdpy.types.Array` objects are the same (or almost)
+    """Assert that two `~pydischarge.types.Array` objects are the same (or almost)
 
     Parameters
     ----------
-    a, b : `~pdpy.types.Array`
+    a, b : `~pydischarge.types.Array`
         the arrays two be tested (can be subclasses)
 
     *attrs
         the list of attributes to test, defaults to all
 
     almost_equal : `bool`, optional
         allow the numpy array's to be 'almost' equal, default: `False`,
```

### Comparing `pydischarge-0.0.1/pdpy/time/__init__.py` & `pydischarge-0.0.2/pydischarge/time/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module provides time conversion utilities.
 
 The :class:`~astropy.time.core.Time` object from the astropy package
 is imported for user convenience, and a GPS time conversion function
 is provided.
```

### Comparing `pydischarge-0.0.1/pdpy/time/__main__.py` & `pydischarge-0.0.2/pydischarge/time/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Primitive command-line interface to `pdpy.time.tconvert`.
+"""Primitive command-line interface to `pydischarge.time.tconvert`.
 
 Either pass a GPS time to convert to a date string, or a date string
 to convert to a GPS time.
 """
 
 import argparse
 import datetime
```

### Comparing `pydischarge-0.0.1/pdpy/time/_tconvert.py` & `pydischarge-0.0.2/pydischarge/time/_tconvert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """tconvert: a utility to convert to and from GPS times.
 
 This method is inspired by the original tconvert utility, written by
 Peter Shawhan.
 """
 
@@ -63,27 +63,27 @@
        so you should consider using `astropy.time.Time` directly.
 
     Examples
     --------
     Integers and floats are automatically converted from GPS to
     `datetime.datetime`:
 
-    >>> from pdpy.time import tconvert
+    >>> from pydischarge.time import tconvert
     >>> tconvert(0)
     datetime.datetime(1980, 1, 6, 0, 0)
     >>> tconvert(1126259462.3910)
     datetime.datetime(2015, 9, 14, 9, 50, 45, 391000)
 
-    while strings are automatically converted to `~pdpy.time.LIGOTimeGPS`:
+    while strings are automatically converted to `~pydischarge.time.LIGOTimeGPS`:
 
     >>> to_gps('Sep 14 2015 09:50:45.391')
     LIGOTimeGPS(1126259462, 391000000)
 
     Additionally, a few special-case words as supported, which all return
-    `~pdpy.time.LIGOTimeGPS`:
+    `~pydischarge.time.LIGOTimeGPS`:
 
     >>> tconvert('now')
     >>> tconvert('today')
     >>> tconvert('tomorrow')
     >>> tconvert('yesterday')
     """
     # convert from GPS into datetime
```

### Comparing `pydischarge-0.0.1/pdpy/time/tests/__init__.py` & `pydischarge-0.0.2/pydischarge/io/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) Duncan Macleod (2018-2020)
+# Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.time`
+"""Utilities for data input/output in standard GW formats.
 """
+
+__author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
```

### Comparing `pydischarge-0.0.1/pdpy/time/tests/test_main.py` & `pydischarge-0.0.2/pydischarge/spectrogram/io/hdf5.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,27 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) Duncan Macleod (2019-2020)
+# Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for the `pdpy.time` command-line interface
+"""This module attaches the HDF5 input output methods to the Spectrogram.
 """
 
-from unittest import mock
+from ...types.io.hdf5 import register_hdf5_array_io
+from .. import Spectrogram
 
-import pytest
-from dateutil import tz
+__author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
-from .. import __main__ as pdpy_time_cli
-
-
-@pytest.mark.parametrize('args, result', [
-    (['Jan 1 2010'], 946339215),
-    (['Jan', '1', '2010'], 946339215),
-    (['946339215'], '2010-01-01 00:00:00.000000 UTC'),
-    (['1161887657', '--local'], '2016-10-30 13:34:00.000000 CDT'),
-])
-@mock.patch('dateutil.tz.tzlocal', return_value=tz.gettz('America/Chicago'))
-def test_main(tzlocal, args, result, capsys):
-    pdpy_time_cli.main(args)
-    out, err = capsys.readouterr()
-    assert not err
-    assert out.rstrip() == str(result)
+register_hdf5_array_io(Spectrogram)
```

### Comparing `pydischarge-0.0.1/pdpy/time/tests/test_time.py` & `pydischarge-0.0.2/pydischarge/time/tests/test_time.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.time`
+"""Tests for :mod:`pydischarge.time`
 """
 
 from contextlib import nullcontext
 from datetime import datetime
 from decimal import Decimal
 from operator import attrgetter
 from unittest import mock
@@ -95,25 +95,25 @@
 
 
 @pytest.mark.requires("maya")
 @pytest.mark.parametrize(("in_", "out"), [
     ('Oct 30 2016 12:34 CST', 1161887657),
 ])
 def test_to_gps_maya(in_, out):
-    """Test that :func:`pdpy.time.to_gps` works with maya.
+    """Test that :func:`pydischarge.time.to_gps` works with maya.
     """
     assert time.to_gps(in_) == out
 
 
 @pytest.mark.parametrize(("in_", "err"), [
     (Quantity(1, 'm'), UnitConversionError),
     ('random string', (ValueError, TypeError)),
 ])
 def test_to_gps_error(in_, err):
-    """Test that :func:`pdpy.time.to_gps` errors when it should.
+    """Test that :func:`pydischarge.time.to_gps` errors when it should.
     """
     with pytest.raises(err):
         time.to_gps(in_)
 
 
 @mock.patch.dict("sys.modules", {"maya": None})
 def test_to_gps_dateparser_error_propagation_nomaya():
@@ -144,25 +144,25 @@
     pytest.param(
         GlueGPS(GW150914.gpsSeconds, GW150914.gpsNanoSeconds),
         GW150914_DT,
         marks=pytest.mark.requires("glue"),
     ),
 ])
 def test_from_gps(in_, out):
-    """Test that :func:`pdpy.time.from_gps` works.
+    """Test that :func:`pydischarge.time.from_gps` works.
     """
     assert time.from_gps(in_) == out
 
 
 @pytest.mark.parametrize(("in_", "err"), [
     ('test', ValueError),
-    (1167264017, ValueError),  # pdpy/pdpy#1021
+    (1167264017, ValueError),  # pydischarge/pydischarge#1021
 ])
 def test_from_gps_error(in_, err):
-    """Test that :func:`pdpy.time.from_gps` errors when it should.
+    """Test that :func:`pydischarge.time.from_gps` errors when it should.
     """
     with pytest.raises(err):
         time.from_gps(in_)
 
 
 @pytest.mark.freeze_time(FREEZE)
 @pytest.mark.parametrize('in_, out', [
@@ -176,15 +176,15 @@
     ),
     ('now', NOW),
     ('today', TODAY),
     ('tomorrow', TOMORROW),
     ('yesterday', YESTERDAY),
 ])
 def test_tconvert(in_, out):
-    """Test :func:`pdpy.time.tconvert`
+    """Test :func:`pydischarge.time.tconvert`
     """
     assert time.tconvert(in_) == out
 
 
 @pytest.mark.parametrize('gpstype', time.gps_types,
                          ids=attrgetter('__module__'))
 def test_gps_types(gpstype):
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/core.py` & `pydischarge-0.0.2/pydischarge/timeseries/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 The TimeSeriesBase
 ==================
 
 This module defines the following classes
 
@@ -120,17 +120,17 @@
     ----------
     value : array-like
         input data array
 
     unit : `~astropy.units.Unit`, optional
         physical unit of these data
 
-    t0 : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+    t0 : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
         GPS epoch associated with these data,
-        any input parsable by `~pdpy.time.to_gps` is fine
+        any input parsable by `~pydischarge.time.to_gps` is fine
 
     dt : `float`, `~astropy.units.Quantity`, optional, default: `1`
         time between successive samples (seconds), can also be given inversely
         via `sample_rate`
 
     sample_rate : `float`, `~astropy.units.Quantity`, optional, default: `1`
         the rate of samples per second (Hertz), can also be given inversely
@@ -140,15 +140,15 @@
         the complete array of GPS times accompanying the data for this series.
         This argument takes precedence over `t0` and `dt` so should be given
         in place of these if relevant, not alongside
 
     name : `str`, optional
         descriptive title for this array
 
-    channel : `~pdpy.detector.Channel`, `str`, optional
+    channel : `~pydischarge.detector.Channel`, `str`, optional
         source data stream for these data
 
     dtype : `~numpy.dtype`, optional
         input data type
 
     copy : `bool`, optional, default: `False`
         choose to copy the input data to new memory
@@ -271,24 +271,24 @@
         source : `str`, `list`
             Source of data, any of the following:
 
             - `str` path of single data file,
             - `str` path of LAL-format cache file,
             - `list` of paths.
 
-        name : `str`, `~pdpy.detector.Channel`
+        name : `str`, `~pydischarge.detector.Channel`
             the name of the channel to read, or a `Channel` object.
 
-        start : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+        start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
             GPS start time of required data, defaults to start of data found;
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
-        end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+        end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
             GPS end time of required data, defaults to end of data found;
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
         format : `str`, optional
             source format identifier. If not given, the format will be
             detected if possible. See below for list of acceptable
             formats.
 
         nproc : `int`, optional
@@ -330,24 +330,24 @@
     def fetch(cls, channel, start, end, host=None, port=None, verbose=False,
               connection=None, verify=False, pad=None, allow_tape=None,
               scaled=None, type=None, dtype=None):
         """Fetch data from NDS
 
         Parameters
         ----------
-        channel : `str`, `~pdpy.detector.Channel`
+        channel : `str`, `~pydischarge.detector.Channel`
             the data channel for which to query
 
-        start : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+        start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
             GPS start time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
-        end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+        end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
             GPS end time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
         host : `str`, optional
             URL of NDS server to use, if blank will try any server
             (in a relatively sensible order) to get the data
 
         port : `int`, optional
             port number for NDS server query, must be given with `host`
@@ -387,21 +387,21 @@
 
         Parameters
         ----------
         ifo : `str`
             the two-character prefix of the IFO in which you are interested,
             e.g. `'L1'`
 
-        start : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+        start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
             GPS start time of required data, defaults to start of data found;
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
-        end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+        end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
             GPS end time of required data, defaults to end of data found;
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
         sample_rate : `float`, optional,
             the sample rate of desired data; most data are stored
             by GWOSC at 4096 Hz, however there may be event-related
             data releases with a 16384 Hz rate, default: `4096`
 
         version : `int`, optional
@@ -427,15 +427,15 @@
 
         **kwargs
             any other keyword arguments are passed to the `TimeSeries.read`
             method that parses the file that was downloaded
 
         Examples
         --------
-        >>> from pdpy.timeseries import (TimeSeries, StateVector)
+        >>> from pydischarge.timeseries import (TimeSeries, StateVector)
         >>> print(TimeSeries.fetch_open_data('H1', 1126259446, 1126259478))
         TimeSeries([  2.17704028e-19,  2.08763900e-19,  2.39681183e-19,
                     ...,   3.55365541e-20,  6.33533516e-20,
                       7.58121195e-20]
                    unit: Unit(dimensionless),
                    t0: 1126259446.0 s,
                    dt: 0.000244140625 s,
@@ -486,24 +486,24 @@
     @classmethod
     def find(cls, channel, start, end, frametype=None, pad=None,
              scaled=None, nproc=1, verbose=False, **readargs):
         """Find and read data from frames for a channel
 
         Parameters
         ----------
-        channel : `str`, `~pdpy.detector.Channel`
+        channel : `str`, `~pydischarge.detector.Channel`
             the name of the channel to read, or a `Channel` object.
 
-        start : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+        start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
             GPS start time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
-        end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+        end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
             GPS end time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
         frametype : `str`, optional
             name of frametype in which this channel is stored, will search
             for containing frame types if necessary
 
         nproc : `int`, optional, default: `1`
             number of parallel processes to use, serial process by
@@ -540,24 +540,24 @@
         """Get data for this channel from frames or NDS
 
         This method dynamically accesses either frames on disk, or a
         remote NDS2 server to find and return data for the given interval
 
         Parameters
         ----------
-        channel : `str`, `~pdpy.detector.Channel`
+        channel : `str`, `~pydischarge.detector.Channel`
             the name of the channel to read, or a `Channel` object.
 
-        start : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+        start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
             GPS start time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
-        end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+        end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
             GPS end time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
         pad : `float`, optional
             value with which to fill gaps in the source data,
             by default gaps will result in a `ValueError`.
 
         scaled : `bool`, optional
             apply slope and bias calibration to ADC data, for non-ADC data
@@ -752,15 +752,15 @@
 
         copy : `bool`, optional, default: `True`
             if `True`, copy these data to a new array
 
         Returns
         -------
         timeseries : `TimeSeries`
-            a PDpy version of the input timeseries
+            a pyDischarge version of the input timeseries
         """
         return cls(pycbcseries.data, t0=pycbcseries.start_time,
                    dt=pycbcseries.delta_t, copy=copy)
 
     def to_pycbc(self, copy=True):
         """Convert this `TimeSeries` into a PyCBC
         `~pycbc.types.timeseries.TimeSeries`
@@ -839,15 +839,15 @@
     """
     EntryClass = TimeSeriesBase
 
     @property
     def span(self):
         """The GPS ``[start, stop)`` extent of data in this `dict`
 
-        :type: `~pdpy.segments.Segment`
+        :type: `~pydischarge.segments.Segment`
         """
         span = SegmentList()
         for value in self.values():
             span.append(value.span)
         try:
             return span.extent()
         except ValueError as exc:  # empty list
@@ -866,24 +866,24 @@
         source : `str`, `list`
             Source of data, any of the following:
 
             - `str` path of single data file,
             - `str` path of LAL-format cache file,
             - `list` of paths.
 
-        channels : `~pdpy.detector.channel.ChannelList`, `list`
+        channels : `~pydischarge.detector.channel.ChannelList`, `list`
             a list of channels to read from the source.
 
-        start : `~pdpy.time.LIGOTimeGPS`, `float`, `str` optional
+        start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str` optional
             GPS start time of required data, anything parseable by
-            :func:`~pdpy.time.to_gps` is fine
+            :func:`~pydischarge.time.to_gps` is fine
 
-        end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+        end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
             GPS end time of required data, anything parseable by
-            :func:`~pdpy.time.to_gps` is fine
+            :func:`~pydischarge.time.to_gps` is fine
 
         format : `str`, optional
             source format identifier. If not given, the format will be
             detected if possible. See below for list of acceptable
             formats.
 
         nproc : `int`, optional
@@ -996,21 +996,21 @@
         """Crop each entry of this `dict`
 
         This method calls the :meth:`crop` method of all entries and
         modifies this dict in place.
 
         Parameters
         ----------
-        start : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+        start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
             GPS start time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
-        end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+        end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
             GPS end time of required data, defaults to end of data found;
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
         See also
         --------
         TimeSeries.crop
             for more details
         """
         for key, val in self.items():
@@ -1046,21 +1046,21 @@
         """Fetch data from NDS for a number of channels.
 
         Parameters
         ----------
         channels : `list`
             required data channels.
 
-        start : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+        start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
             GPS start time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
-        end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+        end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
             GPS end time of required data, defaults to end of data found;
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
         host : `str`, optional
             URL of NDS server to use, if blank will try any server
             (in a relatively sensible order) to get the data
 
         port : `int`, optional
             port number for NDS server query, must be given with `host`.
@@ -1090,15 +1090,15 @@
             NDS2 channel type integer or string name to match.
 
         dtype : `numpy.dtype`, `str`, `type`, or `dict`
             NDS2 data type to match
 
         Returns
         -------
-        data : :class:`~pdpy.timeseries.TimeSeriesBaseDict`
+        data : :class:`~pydischarge.timeseries.TimeSeriesBaseDict`
             a new `TimeSeriesBaseDict` of (`str`, `TimeSeries`) pairs fetched
             from NDS.
         """
         from ..io import nds2 as io_nds2
         from .io.nds2 import (print_verbose, fetch)
 
         if dtype is None:
@@ -1182,21 +1182,21 @@
         """Find and read data from frames for a number of channels.
 
         Parameters
         ----------
         channels : `list`
             required data channels.
 
-        start : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+        start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
             GPS start time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
-        end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+        end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
             GPS end time of required data, defaults to end of data found;
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
         frametype : `str`, optional
             name of frametype in which this channel is stored, by default
             will search for all required frame types
 
         frametype_match : `str`, optional
             regular expression to use for frametype matching
@@ -1297,21 +1297,21 @@
         remote NDS2 server to find and return data for the given interval
 
         Parameters
         ----------
         channels : `list`
             required data channels.
 
-        start : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+        start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
             GPS start time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
-        end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+        end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
             GPS end time of required data, defaults to end of data found;
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
         frametype : `str`, optional
             name of frametype in which this channel is stored, by default
             will search for all required frame types
 
         pad : `float`, optional
             value with which to fill gaps in the source data,
@@ -1588,15 +1588,15 @@
             - ``'pad'`` - pad gap with zeros
 
             If `pad` is given and is not `None`, the default is ``'pad'``,
             otherwise ``'raise'``.
 
         Returns
         -------
-        series : `pdpy.types.TimeSeriesBase` subclass
+        series : `pydischarge.types.TimeSeriesBase` subclass
              a single series containing all data from each entry in this list
 
         See also
         --------
         TimeSeries.append
             for details on how the individual series are concatenated together
         """
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/io/__init__.py` & `pydischarge-0.0.2/pydischarge/timeseries/io/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Input/Output routines for the TimeSeries and its sub-classes.
 """
 
 from . import (  # pylint: disable=unused-import
     ascii,
     gwf,
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/io/ascii.py` & `pydischarge-0.0.2/pydischarge/timeseries/io/ascii.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""ASCII I/O registrations for pdpy.timeseries objects
+"""ASCII I/O registrations for pydischarge.timeseries objects
 """
 
 from ...types.io.ascii import register_ascii_series_io
 from .. import (TimeSeries, StateVector)
 
 # -- registration -------------------------------------------------------------
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/io/cache.py` & `pydischarge-0.0.2/pydischarge/timeseries/io/cache.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """I/O utilities for reading `TimeSeries` from a `list` of file paths.
 """
 
 from ...io.cache import (FILE_LIKE, read_cache, file_segment, sieve)
 from ...segments import Segment
 
@@ -32,21 +32,21 @@
     - sieve the cache to only include data we need
 
     Parameters
     ----------
     cache : `list`, `str`
         List of file paths, or path to a LAL-format cache file on disk.
 
-    start : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+    start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
         GPS start time of required data, defaults to start of data found;
-        any input parseable by `~pdpy.time.to_gps` is fine.
+        any input parseable by `~pydischarge.time.to_gps` is fine.
 
-    end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+    end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
         GPS end time of required data, defaults to end of data found;
-        any input parseable by `~pdpy.time.to_gps` is fine.
+        any input parseable by `~pydischarge.time.to_gps` is fine.
 
     Returns
     -------
     modcache : `list`
         A parsed, sieved list of paths based on the input arguments.
     """
     # open cache file
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/io/core.py` & `pydischarge-0.0.2/pydischarge/timeseries/io/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Basic I/O routines for :mod:`pdpy.timeseries`
+"""Basic I/O routines for :mod:`pydischarge.timeseries`
 """
 
 from ...io import cache as io_cache
 from ...io.mp import read_multi as io_read_multi
 
 
 def read(cls, source, *args, **kwargs):
-    """Read data from a source into a `pdpy.timeseries` object.
+    """Read data from a source into a `pydischarge.timeseries` object.
 
     This method is just the internal worker for `TimeSeries.read`, and
     `TimeSeriesDict.read`, and isn't meant to be called directly.
     """
     # if reading a cache, read it now and sieve
     if io_cache.is_cache(source):
         from .cache import preformat_cache
@@ -92,15 +92,15 @@
 def _pad_series(ts, pad, start=None, end=None, error=False):
     """Pad a timeseries to match the specified [start, end) limits
 
     To cover a gap in data returned from a data source.
 
     Parameters
     ----------
-    ts : `pdpy.types.Series`
+    ts : `pydischarge.types.Series`
         the input series
 
     pad : `float`, `astropy.units.Quantity`
         the value with which to pad
 
     start : `float`, `astropy.units.Quantity`, optional
         the desired start point of the X-axis, defaults to
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/io/gwf/__init__.py` & `pydischarge-0.0.2/pydischarge/timeseries/io/gwf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2022)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Input/output routines for gravitational-wave frame (GWF) format files.
 
 The frame format is defined in LIGO-T970130 available from dcc.ligo.org.
 
 Currently supported are two separate libraries:
 
@@ -118,15 +118,15 @@
 def get_default_gwf_api():
     """Return the preferred GWF library
 
     Examples
     --------
     If you have |LDAStools.frameCPP|_ installed:
 
-    >>> from pdpy.timeseries.io.gwf import get_default_gwf_api
+    >>> from pydischarge.timeseries.io.gwf import get_default_gwf_api
     >>> get_default_gwf_api()
     'framecpp'
 
     Or, if you don't have |lalframe|_:
 
     >>> get_default_gwf_api()
     'lalframe'
@@ -190,29 +190,29 @@
             - `str` path of single data file,
             - `str` path of LAL-format cache file,
             - `list` of paths.
 
         channels : `list`
             list of channel names (or `Channel` objects) to read from frame.
 
-        start : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+        start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
             GPS start time of required data, defaults to start of data found;
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
-        end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+        end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
             GPS end time of required data, defaults to end of data found;
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
         pad : `float`, optional
             value with which to fill gaps in the source data, if not
             given gaps will result in an exception being raised
 
         Returns
         -------
-        dict : :class:`~pdpy.timeseries.TimeSeriesDict`
+        dict : :class:`~pydischarge.timeseries.TimeSeriesDict`
             dict of (channel, `TimeSeries`) data pairs
         """
         # import the frame library here to have any ImportErrors occur early
         import_gwf_library(library)
 
         # -- from here read data
 
@@ -302,21 +302,21 @@
         ----------
         tsdict : `TimeSeriesDict`
             the data to write
 
         outfile : `str`
             the path of the output frame file
 
-        start : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+        start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
             GPS start time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
-        end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+        end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
             GPS end time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
         type : `str`, optional
             the type of the channel, one of 'adc', 'proc', 'sim', default
             is 'proc' unless stored in the channel structure
 
         name : `str`, optional
             name of the project that created this GWF
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/io/gwf/framecpp.py` & `pydischarge-0.0.2/pydischarge/timeseries/io/gwf/framecpp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read data from gravitational-wave frame (GWF) files using
 |LDAStools.frameCPP|__.
 """
 
 import re
 from math import ceil
@@ -69,38 +69,38 @@
     source : `str`, `list`
         Source of data, any of the following:
 
         - `str` path of single data file,
         - `str` path of cache file,
         - `list` of paths.
 
-    channels : `~pdpy.detector.ChannelList`, `list`
+    channels : `~pydischarge.detector.ChannelList`, `list`
         a list of channels to read from the source.
 
-    start : `~pdpy.time.LIGOTimeGPS`, `float`, `str` optional
+    start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str` optional
         GPS start time of required data, anything parseable by
-        :func:`~pdpy.time.to_gps` is fine.
+        :func:`~pydischarge.time.to_gps` is fine.
 
-    end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+    end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
         GPS end time of required data, anything parseable by
-        :func:`~pdpy.time.to_gps` is fine.
+        :func:`~pydischarge.time.to_gps` is fine.
 
     scaled : `bool`, optional
         apply slope and bias calibration to ADC data.
 
     type : `dict`, optional
         a `dict` of ``(name, channel-type)`` pairs, where ``channel-type``
         can be one of ``'adc'``, ``'proc'``, or ``'sim'``.
 
     series_class : `type`, optional
         the `Series` sub-type to return.
 
     Returns
     -------
-    data : `~pdpy.timeseries.TimeSeriesDict` or similar
+    data : `~pydischarge.timeseries.TimeSeriesDict` or similar
         a dict of ``(channel, series)`` pairs read from the GWF source(s).
     """
     # parse input source
     source = file_list(source)
 
     # parse type
     ctype = channel_dict_kwarg(type, channels, (str,))
@@ -123,38 +123,38 @@
     """Read a dict of series data from a single GWF file
 
     Parameters
     ----------
     filename : `str`
         the GWF path from which to read
 
-    channels : `~pdpy.detector.ChannelList`, `list`
+    channels : `~pydischarge.detector.ChannelList`, `list`
         a list of channels to read from the source.
 
-    start : `~pdpy.time.LIGOTimeGPS`, `float`, `str` optional
+    start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str` optional
         GPS start time of required data, anything parseable by
-        :func:`~pdpy.time.to_gps` is fine.
+        :func:`~pydischarge.time.to_gps` is fine.
 
-    end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+    end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
         GPS end time of required data, anything parseable by
-        :func:`~pdpy.time.to_gps` is fine.
+        :func:`~pydischarge.time.to_gps` is fine.
 
     scaled : `bool`, optional
         apply slope and bias calibration to ADC data.
 
     type : `dict`, optional
         a `dict` of ``(name, channel-type)`` pairs, where ``channel-type``
         can be one of ``'adc'``, ``'proc'``, or ``'sim'``.
 
     series_class : `type`, optional
         the `Series` sub-type to return.
 
     Returns
     -------
-    data : `~pdpy.timeseries.TimeSeriesDict` or similar
+    data : `~pydischarge.timeseries.TimeSeriesDict` or similar
         a dict of ``(channel, series)`` pairs read from the GWF file.
     """
     # parse kwargs
     if not start:
         start = 0
     if not end:
         end = 0
@@ -281,15 +281,15 @@
         apply slope and bias calibration to ADC data.
 
     series_class : `type`, optional
         the `Series` sub-type to return.
 
     Returns
     -------
-    series : `~pdpy.timeseries.TimeSeriesBase`
+    series : `~pydischarge.timeseries.TimeSeriesBase`
         the formatted data series
 
     Raises
     ------
     _Skip
         if this data structure doesn't overlap with the requested
         ``[start, end)`` interval.
@@ -374,15 +374,15 @@
         to ignore ``FrVect`` structures containing other information
 
     series_class : `type`, optional
         the `Series` sub-type to return.
 
     Returns
     -------
-    series : `~pdpy.timeseries.TimeSeriesBase`
+    series : `~pydischarge.timeseries.TimeSeriesBase`
         the formatted data series
 
     Raises
     ------
     _Skip
         if this vect doesn't overlap with the requested
         ``[start, end)`` interval, or the name doesn't match.
@@ -440,15 +440,15 @@
 
 
 # -- write --------------------------------------------------------------------
 
 def write(tsdict, outfile,
           start=None, end=None,
           type=None,
-          name='pdpy', run=0,
+          name='pydischarge', run=0,
           compression='GZIP', compression_level=None):
     """Write data to a GWF file using the frameCPP API
 
     Parameters
     ----------
     tsdict : `TimeSeriesDict`
         dict of data to write
@@ -550,17 +550,17 @@
 
     **kwargs
         other keyword arguments are passed to the relevant
         `create_xxx` function
 
     See also
     --------
-    pdpy.io.gwf.create_fradcdata
-    pdpy.io.gwf.create_frprocdata
-    pdpy.io.gwf_create_frsimdata
+    pydischarge.io.gwf.create_fradcdata
+    pydischarge.io.gwf.create_frprocdata
+    pydischarge.io.gwf_create_frsimdata
         for details of the data structure creation, and associated available
         arguments
     """
     epoch = LIGOTimeGPS(*frame.GetGTime())
 
     # create the data container
     if type.lower() == 'adc':
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/io/gwf/framel.py` & `pydischarge-0.0.2/pydischarge/timeseries/io/gwf/framel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Cardiff University (2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read gravitational-wave frame (GWF) files using the FrameL API
 
 The frame foramt is defined in LIGO-T970130 available from dcc.ligo.org
 """
 
 import warnings
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/io/gwf/lalframe.py` & `pydischarge-0.0.2/pydischarge/timeseries/io/gwf/lalframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read gravitational-wave frame (GWF) files using the LALFrame API
 
 The frame format is defined in LIGO-T970130 available from dcc.ligo.org.
 """
 
 import os.path
@@ -173,15 +173,15 @@
 
 # -- write --------------------------------------------------------------------
 
 def write(
         tsdict, outfile,
         start=None, end=None,
         type=None,
-        name='pdpy', run=0,
+        name='pydischarge', run=0,
 ):
     """Write data to a GWF file using the LALFrame API
     """
     if not start:
         start = list(tsdict.values())[0].xspan[0]
     if not end:
         end = list(tsdict.values())[0].xspan[1]
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/io/hdf5.py` & `pydischarge-0.0.2/pydischarge/timeseries/io/hdf5.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module attaches the HDF5 input output methods to the TimeSeries.
 """
 
 from astropy import units
 
 from ...io import registry as io_registry
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/io/losc.py` & `pydischarge-0.0.2/pydischarge/timeseries/io/losc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2022)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read and write HDF5 files in the LIGO Open Science Center format
 
-For more details, see :ref:`pdpy-table-io`.
+For more details, see :ref:`pydischarge-table-io`.
 """
 
 import os.path
 import re
 from math import ceil
 from urllib.parse import urlparse
 
@@ -206,15 +206,15 @@
         path of HDF5 file, or open `H5File`
 
     path : `str`
         name of HDF5 dataset to read.
 
     Returns
     -------
-    data : `~pdpy.timeseries.TimeSeries`
+    data : `~pydischarge.timeseries.TimeSeries`
         a new `TimeSeries` containing the data read from disk
     """
     dataset = io_hdf5.find_dataset(h5f, path)
     # read data
     nddata = dataset[()]
     # read metadata
     xunit = parse_unit(dataset.attrs['Xunits'])
@@ -241,26 +241,26 @@
     ----------
     f : `str`, `h5py.HLObject`
         path of HDF5 file, or open `H5File`
 
     path : `str`
         path of HDF5 dataset to read.
 
-    start : `Time`, `~pdpy.time.LIGOTimeGPS`, optional
+    start : `Time`, `~pydischarge.time.LIGOTimeGPS`, optional
         start GPS time of desired data
 
-    end : `Time`, `~pdpy.time.LIGOTimeGPS`, optional
+    end : `Time`, `~pydischarge.time.LIGOTimeGPS`, optional
         end GPS time of desired data
 
     copy : `bool`, default: `False`
         create a fresh-memory copy of the underlying array
 
     Returns
     -------
-    data : `~pdpy.timeseries.TimeSeries`
+    data : `~pydischarge.timeseries.TimeSeries`
         a new `TimeSeries` containing the data read from disk
     """
     # find data
     dataset = io_hdf5.find_dataset(f, '%s/DQmask' % path)
     maskset = io_hdf5.find_dataset(f, '%s/DQDescriptions' % path)
     # read data
     nddata = dataset[()]
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/io/nds2.py` & `pydischarge-0.0.2/pydischarge/timeseries/io/nds2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """NDS2 data query routines for the TimeSeries
 """
 
 import operator
 import warnings
 from functools import reduce
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/io/wav.py` & `pydischarge-0.0.2/pydischarge/timeseries/io/wav.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read/write WAV files using `scipy.signal.wavfile`
 """
 
 import struct
 import wave
 
@@ -46,15 +46,15 @@
     See also
     --------
     scipy.io.wavfile.read
         for details on how the WAV file is actually read
 
     Examples
     --------
-    >>> from pdpy.timeseries import TimeSeries
+    >>> from pydischarge.timeseries import TimeSeries
     >>> t = TimeSeries.read('test.wav')
     """
     fsamp, arr = wavfile.read(fobj, **kwargs)
     return TimeSeries(arr, sample_rate=fsamp)
 
 
 def write(series, output, scale=None):
@@ -76,15 +76,15 @@
     See also
     --------
     scipy.io.wavfile.write
         for details on how the WAV file is actually written
 
     Examples
     --------
-    >>> from pdpy.timeseries import TimeSeries
+    >>> from pydischarge.timeseries import TimeSeries
     >>> t = TimeSeries([1, 2, 3, 4, 5])
     >>> t = TimeSeries.write('test.wav')
     """
     fsamp = int(series.sample_rate.decompose().value)
     if scale is None:
         scale = 1 / numpy.abs(series.value).max()
     data = (series.value * scale).astype('float32')
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/statevector.py` & `pydischarge-0.0.2/pydischarge/timeseries/statevector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module defines the Boolean array representing the state of some data
 
 Such states are typically the comparison of a `TimeSeries` against some
 threshold, where sub-threshold is good and sup-threshold is bad,
 for example.
 
@@ -118,17 +118,17 @@
     """Boolean array representing a good/bad state determination
 
     Parameters
     ----------
     value : array-like
         input data array
 
-    t0 : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+    t0 : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
         GPS epoch associated with these data,
-        any input parsable by `~pdpy.time.to_gps` is fine
+        any input parsable by `~pydischarge.time.to_gps` is fine
 
     dt : `float`, `~astropy.units.Quantity`, optional, default: `1`
         time between successive samples (seconds), can also be given inversely
         via `sample_rate`
 
     sample_rate : `float`, `~astropy.units.Quantity`, optional, default: `1`
         the rate of samples per second (Hertz), can also be given inversely
@@ -138,15 +138,15 @@
         the complete array of GPS times accompanying the data for this series.
         This argument takes precedence over `t0` and `dt` so should be given
         in place of these if relevant, not alongside
 
     name : `str`, optional
         descriptive title for this array
 
-    channel : `~pdpy.detector.Channel`, `str`, optional
+    channel : `~pydischarge.detector.Channel`, `str`, optional
         source data stream for these data
 
     dtype : `~numpy.dtype`, optional
         input data type
 
     copy : `bool`, optional, default: `False`
         choose to copy the input data to new memory
@@ -221,48 +221,48 @@
     def all(self, axis=None, out=None):
         return numpy.all(self.value, axis=axis, out=out)
 
     # -- useful methods -------------------------
 
     def to_dqflag(self, name=None, minlen=1, dtype=None, round=False,
                   label=None, description=None):
-        """Convert this series into a `~pdpy.segments.DataQualityFlag`.
+        """Convert this series into a `~pydischarge.segments.DataQualityFlag`.
 
         Each contiguous set of `True` values are grouped as a
-        `~pdpy.segments.Segment` running from the GPS time the first
+        `~pydischarge.segments.Segment` running from the GPS time the first
         found `True`, to the GPS time of the next `False` (or the end
         of the series)
 
         Parameters
         ----------
         minlen : `int`, optional
             minimum number of consecutive `True` values to identify as a
-            `~pdpy.segments.Segment`. This is useful to ignore single
+            `~pydischarge.segments.Segment`. This is useful to ignore single
             bit flips, for example.
 
         dtype : `type`, `callable`
             output segment entry type, can pass either a type for simple
             casting, or a callable function that accepts a float and returns
             another numeric type, defaults to the `dtype` of the time index
 
         round : `bool`, optional
-            choose to round each `~pdpy.segments.Segment` to its
+            choose to round each `~pydischarge.segments.Segment` to its
             inclusive integer boundaries
 
         label : `str`, optional
-            the :attr:`~pdpy.segments.DataQualityFlag.label` for the
+            the :attr:`~pydischarge.segments.DataQualityFlag.label` for the
             output flag.
 
         description : `str`, optional
-            the :attr:`~pdpy.segments.DataQualityFlag.description` for the
+            the :attr:`~pydischarge.segments.DataQualityFlag.description` for the
             output flag.
 
         Returns
         -------
-        dqflag : `~pdpy.segments.DataQualityFlag`
+        dqflag : `~pydischarge.segments.DataQualityFlag`
             a segment representation of this `StateTimeSeries`, the span
             defines the `known` segments, while the contiguous `True`
             sets defined each of the `active` segments
         """
         from ..segments import DataQualityFlag
 
         # format dtype
@@ -444,17 +444,17 @@
     ----------
     value : array-like
         input data array
 
     bits : `Bits`, `list`, optional
         list of bits defining this `StateVector`
 
-    t0 : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+    t0 : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
         GPS epoch associated with these data,
-        any input parsable by `~pdpy.time.to_gps` is fine
+        any input parsable by `~pydischarge.time.to_gps` is fine
 
     dt : `float`, `~astropy.units.Quantity`, optional, default: `1`
         time between successive samples (seconds), can also be given inversely
         via `sample_rate`
 
     sample_rate : `float`, `~astropy.units.Quantity`, optional, default: `1`
         the rate of samples per second (Hertz), can also be given inversely
@@ -464,15 +464,15 @@
         the complete array of GPS times accompanying the data for this series.
         This argument takes precedence over `t0` and `dt` so should be given
         in place of these if relevant, not alongside
 
     name : `str`, optional
         descriptive title for this array
 
-    channel : `~pdpy.detector.Channel`, `str`, optional
+    channel : `~pydischarge.detector.Channel`, `str`, optional
         source data stream for these data
 
     dtype : `~numpy.dtype`, optional
         input data type
 
     copy : `bool`, optional, default: `False`
         choose to copy the input data to new memory
@@ -613,24 +613,24 @@
         source : `str`, `list`
             Source of data, any of the following:
 
             - `str` path of single data file,
             - `str` path of LAL-format cache file,
             - `list` of paths.
 
-        channel : `str`, `~pdpy.detector.Channel`
+        channel : `str`, `~pydischarge.detector.Channel`
             the name of the channel to read, or a `Channel` object.
 
-        start : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+        start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
             GPS start time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
-        end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+        end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
             GPS end time of required data, defaults to end of data found;
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
         bits : `list`, optional
             list of bits names for this `StateVector`, give `None` at
             any point in the list to mask that bit
 
         format : `str`, optional
             source format identifier. If not given, the format will be
@@ -685,18 +685,18 @@
         before any further operations.
 
         Notes
         -----"""
         return super().read(source, *args, **kwargs)
 
     def to_dqflags(self, bits=None, minlen=1, dtype=float, round=False):
-        """Convert this `StateVector` into a `~pdpy.segments.DataQualityDict`
+        """Convert this `StateVector` into a `~pydischarge.segments.DataQualityDict`
 
         The `StateTimeSeries` for each bit is converted into a
-        `~pdpy.segments.DataQualityFlag` with the bits combined into a dict.
+        `~pydischarge.segments.DataQualityFlag` with the bits combined into a dict.
 
         Parameters
         ----------
         minlen : `int`, optional, default: 1
            minimum number of consecutive `True` values to identify as a
            `Segment`. This is useful to ignore single bit flips,
            for example.
@@ -704,15 +704,15 @@
         bits : `list`, optional
             a list of bit indices or bit names to select, defaults to
             `~StateVector.bits`
 
         Returns
         -------
         DataQualityFlag list : `list`
-            a list of `~pdpy.segments.flag.DataQualityFlag`
+            a list of `~pydischarge.segments.flag.DataQualityFlag`
             reprensentations for each bit in this `StateVector`
 
         See also
         --------
         StateTimeSeries.to_dqflag
             for details on the segment representation method for
             `StateVector` bits
@@ -729,24 +729,24 @@
     @classmethod
     def fetch(cls, channel, start, end, bits=None, host=None, port=None,
               verbose=False, connection=None, type=Nds2ChannelType.any()):
         """Fetch data from NDS into a `StateVector`.
 
         Parameters
         ----------
-        channel : `str`, `~pdpy.detector.Channel`
+        channel : `str`, `~pydischarge.detector.Channel`
             the name of the channel to read, or a `Channel` object.
 
-        start : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+        start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
             GPS start time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
-        end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+        end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
             GPS end time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
         bits : `Bits`, `list`, optional
             definition of bits for this `StateVector`
 
         host : `str`, optional
             URL of NDS server to use, defaults to observatory site host
 
@@ -777,24 +777,24 @@
 
     @classmethod
     def get(cls, channel, start, end, bits=None, **kwargs):
         """Get data for this channel from frames or NDS
 
         Parameters
         ----------
-        channel : `str`, `~pdpy.detector.Channel`
+        channel : `str`, `~pydischarge.detector.Channel`
             the name of the channel to read, or a `Channel` object.
 
-        start : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+        start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
             GPS start time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
-        end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
+        end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
             GPS end time of required data,
-            any input parseable by `~pdpy.time.to_gps` is fine
+            any input parseable by `~pydischarge.time.to_gps` is fine
 
         bits : `Bits`, `list`, optional
             definition of bits for this `StateVector`
 
         pad : `float`, optional
             value with which to fill gaps in the source data, only used if
             gap is not given, or ``gap='pad'`` is given
@@ -840,32 +840,32 @@
         bits : `list`, optional
             A list of bit indices or bit names, defaults to
             `~StateVector.bits`. This argument is ignored if ``format`` is
             not ``'segments'``
 
         **kwargs
             Other keyword arguments to be passed to either
-            `~pdpy.plot.SegmentAxes.plot` or
-            `~pdpy.plot.Axes.plot`, depending
+            `~pydischarge.plot.SegmentAxes.plot` or
+            `~pydischarge.plot.Axes.plot`, depending
             on ``format``.
 
         Returns
         -------
-        plot : `~pdpy.plot.Plot`
+        plot : `~pydischarge.plot.Plot`
             output plot object
 
         See also
         --------
         matplotlib.pyplot.figure
             for documentation of keyword arguments used to create the
             figure
         matplotlib.figure.Figure.add_subplot
             for documentation of keyword arguments used to create the
             axes
-        pdpy.plot.SegmentAxes.plot_flag
+        pydischarge.plot.SegmentAxes.plot_flag
             for documentation of keyword arguments used in rendering each
             statevector flag.
         """
         if format == 'timeseries':
             return super().plot(**kwargs)
         if format == 'segments':
             from ..plot import Plot
@@ -966,24 +966,24 @@
         source : `str`, `list`
             Source of data, any of the following:
 
             - `str` path of single data file,
             - `str` path of LAL-format cache file,
             - `list` of paths.
 
-        channels : `~pdpy.detector.channel.ChannelList`, `list`
+        channels : `~pydischarge.detector.channel.ChannelList`, `list`
             a list of channels to read from the source.
 
-        start : `~pdpy.time.LIGOTimeGPS`, `float`, `str` optional
+        start : `~pydischarge.time.LIGOTimeGPS`, `float`, `str` optional
             GPS start time of required data, anything parseable by
-            :meth:`~pdpy.time.to_gps` is fine
+            :meth:`~pydischarge.time.to_gps` is fine
 
-        end : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+        end : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
             GPS end time of required data, anything parseable by
-            :meth:`~pdpy.time.to_gps` is fine
+            :meth:`~pydischarge.time.to_gps` is fine
 
         bits : `list` of `lists`, `dict`, optional
             the ordered list of interesting bit lists for each channel,
             or a `dict` of (`channel`, `list`) pairs
 
         format : `str`, optional
             source format identifier. If not given, the format will be
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/tests/__init__.py` & `pydischarge-0.0.2/pydischarge/spectrogram/io/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) Duncan Macleod (2018-2020)
+# Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.timeseries`
+"""Input/Output routines for the Spectrogram.
 """
+
+from . import (
+    hdf5
+)
+
+__author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/tests/test_core.py` & `pydischarge-0.0.2/pydischarge/timeseries/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Unit test for timeseries module
 """
 
 import operator
 from functools import reduce
 from io import BytesIO
@@ -47,50 +47,50 @@
 
 # -- TimeSeriesBase -----------------------------------------------------------
 
 class TestTimeSeriesBase(_TestSeries):
     TEST_CLASS = TimeSeriesBase
 
     def test_new(self):
-        """Test `pdpy.timeseries.TimeSeriesBase` constructor
+        """Test `pydischarge.timeseries.TimeSeriesBase` constructor
         """
         array = super().test_new()
 
         # check time-domain metadata
         assert array.epoch == GPS_EPOCH
         assert array.sample_rate == units.Quantity(1, 'Hertz')
         assert array.dt == units.Quantity(1, 'second')
 
     def test_new_epoch_t0(self):
-        """Test `pdpy.timeseries.TimeSeriesBase` handling of epoch vs t0.
+        """Test `pydischarge.timeseries.TimeSeriesBase` handling of epoch vs t0.
         """
         a = self.create(epoch=10)
         b = self.create(t0=10)
         utils.assert_quantity_sub_equal(a, b)
         with pytest.raises(
             ValueError,
             match="^give only one of epoch or t0$",
         ):
             self.TEST_CLASS(self.data, epoch=1, t0=1)
 
     def test_new_sample_rate_dt(self):
-        """Test `pdpy.timeseries.TimeSeriesBase` handling of sample_rate vs dt.
+        """Test `pydischarge.timeseries.TimeSeriesBase` handling of sample_rate vs dt.
         """
         # check handling of sample_rate vs dt
         a = self.create(sample_rate=100)
         b = self.create(dt=0.01)
         utils.assert_quantity_sub_equal(a, b)
         with pytest.raises(
             ValueError,
             match="^give only one of sample_rate or dt$",
         ):
             self.TEST_CLASS(self.data, sample_rate=1, dt=1)
 
     def test_epoch(self):
-        """Test `pdpy.timeseries.TimeSeriesBase.epoch`
+        """Test `pydischarge.timeseries.TimeSeriesBase.epoch`
         """
         # check basic conversion from t0 -> epoch
         a = self.create(t0=1126259462)
         assert a.epoch == Time('2015-09-14 09:50:45', format='iso')
 
         # test that we can't delete epoch
         with pytest.raises(AttributeError):
@@ -103,15 +103,15 @@
 
         # check other types
         a.epoch = Time('2015-09-14 09:50:45', format='iso')
         utils.assert_quantity_almost_equal(
             a.t0, units.Quantity(1126259462, 's'))
 
     def test_sample_rate(self):
-        """Test `pdpy.timeseries.TimeSeriesBase.sample_rate`
+        """Test `pydischarge.timeseries.TimeSeriesBase.sample_rate`
         """
         # check basic conversion from dt -> sample_rate
         a = self.create(dt=0.5)
         assert a.sample_rate == 2 * units.Hz
 
         # test that we can't delete sample_rate
         with pytest.raises(AttributeError):
@@ -441,15 +441,15 @@
     def instance(self):
         return self.create()
 
     def test_series_link(self):
         assert self.TEST_CLASS.EntryClass is self.ENTRY_CLASS
 
     def test_segments(self, instance):
-        """Test :attr:`pdpy.timeseries.TimeSeriesBaseList.segments`
+        """Test :attr:`pydischarge.timeseries.TimeSeriesBaseList.segments`
         """
         sl = instance.segments
         assert isinstance(sl, SegmentList)
         assert all(isinstance(s, Segment) for s in sl)
         assert sl == [(0, 100), (101, 1101)]
 
     def test_append(self, instance):
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/tests/test_io_gwf_framecpp.py` & `pydischarge-0.0.2/pydischarge/timeseries/tests/test_io_gwf_framecpp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.timeseries.io.gwf.framecpp`
+"""Tests for :mod:`pydischarge.timeseries.io.gwf.framecpp`
 """
 
 import pytest
 
 import numpy
 
 from ...detector import Channel
@@ -59,15 +59,15 @@
     int32ts.write(tmp, format="gwf.framecpp", type="adc")
     new = type(int32ts).read(tmp, "test", type="adc")
     assert new.dtype == numpy.dtype("float64")
     assert_quantity_sub_equal(int32ts, new)
 
 
 def test_read_write_frvect_name(tmp_path):
-    """Test against regression of https://github.com/pdpy-github/pdpy/issues/1206
+    """Test against regression of https://github.com/pydischarge-github/pydischarge/issues/1206
     """
     data = TimeSeries(
         numpy.random.random(10),
         channel="X1:TEST",
         name="test",
     )
     tmp = tmp_path / "test.gwf"
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/tests/test_io_gwf_lalframe.py` & `pydischarge-0.0.2/pydischarge/timeseries/tests/test_io_gwf_lalframe.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.timeseries.io.gwf.lalframe`
+"""Tests for :mod:`pydischarge.timeseries.io.gwf.lalframe`
 """
 
 from pathlib import Path
 from urllib.parse import urlparse
 
 import pytest
 import numpy
@@ -34,15 +34,15 @@
     TEST_GWF_FILE,
 )
 from ...timeseries import TimeSeries
 
 # import optional dependencies
 lal_utils = pytest.importorskip("lal.utils")
 lalframe = pytest.importorskip("lalframe")
-pdpy_lalframe = pytest.importorskip("pdpy.timeseries.io.gwf.lalframe")
+pydischarge_lalframe = pytest.importorskip("pydischarge.timeseries.io.gwf.lalframe")
 
 # get URI to test against
 TEST_GWF_PATH = Path(TEST_GWF_FILE).absolute()
 TEST_GWF_URL = TEST_GWF_PATH.as_uri()
 
 # get info corresponding to this file
 TEST_GWF_SEGMENT = file_segment(TEST_GWF_FILE)
@@ -56,15 +56,15 @@
 def stream():
     return lalframe.FrStreamOpen(str(TEST_GWF_PATH.parent), TEST_GWF_PATH.name)
 
 
 def _test_open_data_source(source):
     """This function actually performs the test
     """
-    stream = pdpy_lalframe.open_data_source(source)
+    stream = pydischarge_lalframe.open_data_source(source)
     assert stream.epoch == TEST_GWF_SEGMENT[0]
     assert Path(urlparse(stream.cache.list.url).path).samefile(TEST_GWF_PATH)
 
 
 @pytest.mark.parametrize("source", [
     TEST_GWF_FILE,
     TEST_GWF_URL,
@@ -90,30 +90,30 @@
 
 
 def test_open_data_source_error():
     with pytest.raises(
         ValueError,
         match=f"^Don't know how to open data source of type {type(None)}$",
     ):
-        pdpy_lalframe.open_data_source(None)
+        pydischarge_lalframe.open_data_source(None)
 
 
 def test_get_stream_duration(stream):
-    assert pdpy_lalframe.get_stream_duration(stream) == 1.
+    assert pydischarge_lalframe.get_stream_duration(stream) == 1.
 
 
 @pytest.mark.parametrize("start, end", [
     (None, None),
     (None, TEST_GWF_SEGMENT[0] + .5),
     (TEST_GWF_SEGMENT[0] + .5, None),
     (TEST_GWF_SEGMENT[0] + .25, TEST_GWF_SEGMENT[1] - .25),
     (TEST_GWF_SEGMENT[1] - TEST_GWF_DELTA_T / 2, None),
 ])
 def test_read(start, end):
-    data = pdpy_lalframe.read(
+    data = pydischarge_lalframe.read(
         TEST_GWF_FILE,
         CHANNELS,
         start=start,
         end=end,
     )
     assert isinstance(data, dict)
 
@@ -131,39 +131,39 @@
 
 
 def test_read_channel_error():
     with pytest.raises(
         RuntimeError,
         match="^channel 'bad' not found$",
     ):
-        pdpy_lalframe.read(TEST_GWF_FILE, ["bad"])
+        pydischarge_lalframe.read(TEST_GWF_FILE, ["bad"])
 
 
 def test_read_deprecated_scaled():
     with pytest.warns(UserWarning):
-        pdpy_lalframe.read(
+        pydischarge_lalframe.read(
             TEST_GWF_FILE,
             ["L1:LDAS-STRAIN"],
             scaled=True,
         )
 
 
 def test_write(tmp_path):
     # read the data first
-    data = pdpy_lalframe.read(TEST_GWF_FILE, CHANNELS)
+    data = pydischarge_lalframe.read(TEST_GWF_FILE, CHANNELS)
 
     # write the data
     tmp = tmp_path / "test.gwf"
-    pdpy_lalframe.write(
+    pydischarge_lalframe.write(
         data,
         tmp,
     )
 
     # read it back and check things
-    data2 = pdpy_lalframe.read(tmp, CHANNELS)
+    data2 = pydischarge_lalframe.read(tmp, CHANNELS)
     assert_dict_equal(data, data2, assert_quantity_sub_equal)
 
 
 @pytest.mark.parametrize(
     'data',
     [
         pytest.param(
@@ -176,11 +176,11 @@
         [1, 2, 3, 4, 5],
     ]
 )
 def test_write_no_ifo(tmp_path, data):
     # create timeseries with no IFO
     data = TimeSeries(data, dtype=float)
     tmp = tmp_path / "test.gwf"
-    pdpy_lalframe.write(
+    pydischarge_lalframe.write(
         {None: data},
         tmp
     )
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/tests/test_io_losc.py` & `pydischarge-0.0.2/pydischarge/timeseries/tests/test_io_losc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Cardiff University (2021-2022)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.timeseries.io.losc`
+"""Tests for :mod:`pydischarge.timeseries.io.losc`
 """
 
 import pytest
 
 from astropy.utils.data import download_file
 
 from gwosc.locate import get_event_urls
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/tests/test_statevector.py` & `pydischarge-0.0.2/pydischarge/timeseries/tests/test_statevector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Unit test for timeseries module
 """
 
 from io import BytesIO
 
 import pytest
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/tests/test_timeseries.py` & `pydischarge-0.0.2/pydischarge/timeseries/tests/test_timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Unit test for timeseries module
 """
 
 import os.path
 import warnings
 from contextlib import nullcontext
@@ -178,15 +178,15 @@
             array, format,
             assert_equal=utils.assert_quantity_sub_equal,
             assert_kw={'exclude': ['name', 'channel', 'unit']})
 
     def test_read_ascii_header(self, tmpdir):
         """Check that ASCII files with headers are read without extra options
 
-        [regression: https://github.com/pdpy-github/pdpy/issues/1473]
+        [regression: https://github.com/pydischarge-github/pydischarge/issues/1473]
         """
         txt = tmpdir / "text.txt"
         txt.write_text(
             "# time (s)\tdata (strain)\n0\t1\n1\t2\n2\t3",
             encoding="utf-8",
         )
         data = self.TEST_CLASS.read(txt, format="txt")
@@ -260,15 +260,15 @@
 
     @pytest.mark.parametrize('api', GWF_APIS)
     @pytest.mark.parametrize('nproc', (1, 2))
     def test_read_write_gwf_multiple(self, tmp_path, api, nproc):
         """Check that each GWF API can read a series of files, either in
         a single process, or in multiple processes
 
-        Regression: https://github.com/pdpy-github/pdpy/issues/1486
+        Regression: https://github.com/pydischarge-github/pydischarge/issues/1486
         """
         fmt = "gwf" if api is None else "gwf." + api
         a1 = self.create(name='TEST')
         a2 = self.create(name='TEST', t0=a1.span[1], dt=a1.dx)
 
         tmp1 = tmp_path / "test1.gwf"
         tmp2 = tmp_path / "test3.gwf"
@@ -488,17 +488,17 @@
             b,
         )
 
     def test_read_pad_raise(self):
         """Check that `TimeSeries.read` with `gap='raise'` actually
         raises appropriately.
 
-        [regression: https://github.com/pdpy-github/pdpy/issues/1211]
+        [regression: https://github.com/pydischarge-github/pydischarge/issues/1211]
         """
-        from pdpy.io.cache import file_segment
+        from pydischarge.io.cache import file_segment
         span = file_segment(utils.TEST_HDF5_FILE)
         with pytest.raises(ValueError):
             self.TEST_CLASS.read(
                 utils.TEST_HDF5_FILE,
                 "H1:LDAS-STRAIN",
                 pad=0.,
                 start=span[0],
@@ -616,19 +616,19 @@
 
         nds_connection.find_channels = find_channels
 
         # run fetch and assert error
         with mock.patch('nds2.connection') as mock_connection:
             mock_connection.return_value = nds_connection
             with pytest.raises(RuntimeError, match="no data received"):
-                self.TEST_CLASS.fetch('L1:TEST', 0, 1, host='nds.pdpy')
+                self.TEST_CLASS.fetch('L1:TEST', 0, 1, host='nds.pydischarge')
 
     @pytest.mark.requires("nds2")
     @mock.patch(
-        "pdpy.io.nds2.host_resolution_order",
+        "pydischarge.io.nds2.host_resolution_order",
         return_value=(["nds.example.com", 31200],),
     )
     def test_fetch_warning_message(self, _):
         """Test that TimeSeries.fetch emits a useful warning on NDS2 issues.
         """
         with \
                 pytest.raises(
@@ -1084,15 +1084,15 @@
             fftlength=0.25,
             overlap=0.125,
             nproc=2,
         )
         utils.assert_quantity_sub_equal(sg, sg2)
 
     def test_resample(self, gw150914):
-        """Test :meth:`pdpy.timeseries.TimeSeries.resample`
+        """Test :meth:`pydischarge.timeseries.TimeSeries.resample`
         """
         # test IIR decimation
         l2 = gw150914.resample(1024, ftype='iir')
         # FIXME: this test needs to be more robust
         assert l2.sample_rate == 1024 * units.Hz
 
     def test_resample_noop(self):
@@ -1101,15 +1101,15 @@
             new = data.resample(data.sample_rate)
             assert data is new
 
     def test_rms(self, gw150914):
         rms = gw150914.rms(1.)
         assert rms.sample_rate == 1 * units.Hz
 
-    @mock.patch('pdpy.segments.DataQualityFlag.query',
+    @mock.patch('pydischarge.segments.DataQualityFlag.query',
                 return_value=LIVETIME)
     def test_mask(self, dqflag):
         # craft a timeseries of ones that can be easily tested against
         # a few interesting corner cases
         data = TimeSeries(numpy.ones(8192), sample_rate=128)
         masked = data.mask(flag='X1:TEST-FLAG:1')
```

### Comparing `pydischarge-0.0.1/pdpy/timeseries/timeseries.py` & `pydischarge-0.0.2/pydischarge/timeseries/timeseries.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Array with metadata
 """
 
 import math
 import warnings
 
@@ -66,17 +66,17 @@
     ----------
     value : array-like
         input data array
 
     unit : `~astropy.units.Unit`, optional
         physical unit of these data
 
-    t0 : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+    t0 : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
         GPS epoch associated with these data,
-        any input parsable by `~pdpy.time.to_gps` is fine
+        any input parsable by `~pydischarge.time.to_gps` is fine
 
     dt : `float`, `~astropy.units.Quantity`, optional
         time between successive samples (seconds), can also be given inversely
         via `sample_rate`
 
     sample_rate : `float`, `~astropy.units.Quantity`, optional
         the rate of samples per second (Hertz), can also be given inversely
@@ -86,15 +86,15 @@
         the complete array of GPS times accompanying the data for this series.
         This argument takes precedence over `t0` and `dt` so should be given
         in place of these if relevant, not alongside
 
     name : `str`, optional
         descriptive title for this array
 
-    channel : `~pdpy.detector.Channel`, `str`, optional
+    channel : `~pydischarge.detector.Channel`, `str`, optional
         source data stream for these data
 
     dtype : `~numpy.dtype`, optional
         input data type
 
     copy : `bool`, optional
         choose to copy the input data to new memory
@@ -105,20 +105,20 @@
     Notes
     -----
     The necessary metadata to reconstruct timing information are recorded
     in the `epoch` and `sample_rate` attributes. This time-stamps can be
     returned via the :attr:`~TimeSeries.times` property.
 
     All comparison operations performed on a `TimeSeries` will return a
-    `~pdpy.timeseries.StateTimeSeries` - a boolean array
+    `~pydischarge.timeseries.StateTimeSeries` - a boolean array
     with metadata copied from the starting `TimeSeries`.
 
     Examples
     --------
-    >>> from pdpy.timeseries import TimeSeries
+    >>> from pydischarge.timeseries import TimeSeries
 
     To create an array of random numbers, sampled at 100 Hz, in units of
     'metres':
 
     >>> from numpy import random
     >>> series = TimeSeries(random.random(1000), sample_rate=100, unit='m')
 
@@ -137,26 +137,26 @@
             length of the desired Fourier transform, input will be
             cropped or padded to match the desired length.
             If nfft is not given, the length of the `TimeSeries`
             will be used
 
         Returns
         -------
-        out : `~pdpy.frequencyseries.FrequencySeries`
+        out : `~pydischarge.frequencyseries.FrequencySeries`
             the normalised, complex-valued FFT `FrequencySeries`.
 
         See also
         --------
         numpy.fft.rfft : The FFT implementation used in this method.
 
         Notes
         -----
         This method, in constrast to the :func:`numpy.fft.rfft` method
         it calls, applies the necessary normalisation such that the
-        amplitude of the output `~pdpy.frequencyseries.FrequencySeries` is
+        amplitude of the output `~pydischarge.frequencyseries.FrequencySeries` is
         correct.
         """
         from ..frequencyseries import FrequencySeries
         if nfft is None:
             nfft = self.size
         dft = npfft.rfft(self.value, n=nfft) / nfft
         dft[1:] *= 2.0
@@ -189,24 +189,24 @@
         window : `str`, `numpy.ndarray`, optional
             window function to apply to timeseries prior to FFT,
             see :func:`scipy.signal.get_window` for details on acceptable
             formats
 
         Returns
         -------
-        out : complex-valued `~pdpy.frequencyseries.FrequencySeries`
+        out : complex-valued `~pydischarge.frequencyseries.FrequencySeries`
             the transformed output, with populated frequencies array
             metadata
 
         See also
         --------
         TimeSeries.fft
            The FFT method used.
         """
-        from pdpy.spectrogram import Spectrogram
+        from pydischarge.spectrogram import Spectrogram
         # format lengths
         if fftlength is None:
             fftlength = self.duration
         if isinstance(fftlength, units.Quantity):
             fftlength = fftlength.value
         nfft = int((fftlength * self.sample_rate).decompose().value)
         noverlap = int((overlap * self.sample_rate).decompose().value)
@@ -269,15 +269,15 @@
 
         **kwargs
             other keyword arguments are passed to the underlying
             PSD-generation method
 
         Returns
         -------
-        psd :  `~pdpy.frequencyseries.FrequencySeries`
+        psd :  `~pydischarge.frequencyseries.FrequencySeries`
             a data series containing the PSD.
 
         Notes
         -----
         The accepted ``method`` arguments are:
 
         - ``'bartlett'`` : a mean average of non-overlapping periodograms
@@ -312,15 +312,15 @@
 
         method : `str`, optional
             FFT-averaging method (default: ``'median'``),
             see *Notes* for more details
 
         Returns
         -------
-        asd :  `~pdpy.frequencyseries.FrequencySeries`
+        asd :  `~pydischarge.frequencyseries.FrequencySeries`
             a data series containing the ASD
 
         See also
         --------
         TimeSeries.psd
 
         Notes
@@ -354,15 +354,15 @@
         window : `str`, `numpy.ndarray`, optional
             window function to apply to timeseries prior to FFT,
             see :func:`scipy.signal.get_window` for details on acceptable
             formats
 
         Returns
         -------
-        csd :  `~pdpy.frequencyseries.FrequencySeries`
+        csd :  `~pydischarge.frequencyseries.FrequencySeries`
             a data series containing the CSD.
         """
         return spectral.psd(
             (self, other),
             spectral.csd,
             fftlength=fftlength,
             overlap=overlap,
@@ -374,15 +374,15 @@
                     method=DEFAULT_FFT_METHOD, nproc=1, **kwargs):
         """Calculate the average power spectrogram of this `TimeSeries`
         using the specified average spectrum method.
 
         Each time-bin of the output `Spectrogram` is calculated by taking
         a chunk of the `TimeSeries` in the segment
         `[t - overlap/2., t + stride + overlap/2.)` and calculating the
-        :meth:`~pdpy.timeseries.TimeSeries.psd` of those data.
+        :meth:`~pydischarge.timeseries.TimeSeries.psd` of those data.
 
         As a result, each time-bin is calculated using `stride + overlap`
         seconds of data.
 
         Parameters
         ----------
         stride : `float`
@@ -405,15 +405,15 @@
             see *Notes* for more details
 
         nproc : `int`
             number of CPUs to use in parallel processing of FFTs
 
         Returns
         -------
-        spectrogram : `~pdpy.spectrogram.Spectrogram`
+        spectrogram : `~pydischarge.spectrogram.Spectrogram`
             time-frequency power spectrogram as generated from the
             input time-series.
 
         Notes
         -----
         The accepted ``method`` arguments are:
 
@@ -461,15 +461,15 @@
 
         **kwargs
             other parameters to be passed to `scipy.signal.periodogram` for
             each column of the `Spectrogram`
 
         Returns
         -------
-        spectrogram: `~pdpy.spectrogram.Spectrogram`
+        spectrogram: `~pydischarge.spectrogram.Spectrogram`
             a power `Spectrogram` with `1/fftlength` frequency resolution and
             (fftlength - overlap) time resolution.
 
         See also
         --------
         scipy.signal.periodogram
             for documentation on the Fourier methods used in this calculation
@@ -645,15 +645,15 @@
         window : `str`, `numpy.ndarray`, optional
             window function to apply to timeseries prior to FFT,
             see :func:`scipy.signal.get_window` for details on acceptable
             formats
 
         Returns
         -------
-        psd :  `~pdpy.frequencyseries.FrequencySeries`
+        psd :  `~pydischarge.frequencyseries.FrequencySeries`
             a data series containing the PSD.
         """
         return spectral.psd(
             self,
             spectral.rayleigh,
             fftlength=fftlength,
             overlap=overlap,
@@ -683,15 +683,15 @@
 
         nproc : `int`, optional
             maximum number of independent frame reading processes, default
             default: ``1``
 
         Returns
         -------
-        spectrogram : `~pdpy.spectrogram.Spectrogram`
+        spectrogram : `~pydischarge.spectrogram.Spectrogram`
             time-frequency Rayleigh spectrogram as generated from the
             input time-series.
 
         See also
         --------
         TimeSeries.rayleigh
             for details of the statistic calculation
@@ -712,15 +712,15 @@
     def csd_spectrogram(self, other, stride, fftlength=None, overlap=0,
                         window='hann', nproc=1, **kwargs):
         """Calculate the cross spectral density spectrogram of this
            `TimeSeries` with 'other'.
 
         Parameters
         ----------
-        other : `~pdpy.timeseries.TimeSeries`
+        other : `~pydischarge.timeseries.TimeSeries`
             second time-series for cross spectral density calculation
 
         stride : `float`
             number of seconds in single PSD (column of spectrogram).
 
         fftlength : `float`
             number of seconds in single FFT.
@@ -736,15 +736,15 @@
 
         nproc : `int`
             maximum number of independent frame reading processes, default
             is set to single-process file reading.
 
         Returns
         -------
-        spectrogram : `~pdpy.spectrogram.Spectrogram`
+        spectrogram : `~pydischarge.spectrogram.Spectrogram`
             time-frequency cross spectrogram as generated from the
             two input time-series.
         """
         return spectral.average_spectrogram(
             (self, other),
             spectral.csd,
             stride,
@@ -776,24 +776,24 @@
             stop-band edge frequency, defaults to `frequency * 1.5`
 
         type : `str`
             the filter type, either ``'iir'`` or ``'fir'``
 
         **kwargs
             other keyword arguments are passed to
-            :func:`pdpy.signal.filter_design.highpass`
+            :func:`pydischarge.signal.filter_design.highpass`
 
         Returns
         -------
         hpseries : `TimeSeries`
             a high-passed version of the input `TimeSeries`
 
         See also
         --------
-        pdpy.signal.filter_design.highpass
+        pydischarge.signal.filter_design.highpass
             for details on the filter design
         TimeSeries.filter
             for details on how the filter is applied
         """
         # design filter
         filt = filter_design.highpass(frequency, self.sample_rate,
                                       fstop=fstop, gpass=gpass, gstop=gstop,
@@ -820,24 +820,24 @@
             stop-band edge frequency, defaults to `frequency * 1.5`
 
         type : `str`
             the filter type, either ``'iir'`` or ``'fir'``
 
         **kwargs
             other keyword arguments are passed to
-            :func:`pdpy.signal.filter_design.lowpass`
+            :func:`pydischarge.signal.filter_design.lowpass`
 
         Returns
         -------
         lpseries : `TimeSeries`
             a low-passed version of the input `TimeSeries`
 
         See also
         --------
-        pdpy.signal.filter_design.lowpass
+        pydischarge.signal.filter_design.lowpass
             for details on the filter design
         TimeSeries.filter
             for details on how the filter is applied
         """
         # design filter
         filt = filter_design.lowpass(frequency, self.sample_rate,
                                      fstop=fstop, gpass=gpass, gstop=gstop,
@@ -867,24 +867,24 @@
             `(low, high)` edge-frequencies of stop band
 
         type : `str`
             the filter type, either ``'iir'`` or ``'fir'``
 
         **kwargs
             other keyword arguments are passed to
-            :func:`pdpy.signal.filter_design.bandpass`
+            :func:`pydischarge.signal.filter_design.bandpass`
 
         Returns
         -------
         bpseries : `TimeSeries`
             a band-passed version of the input `TimeSeries`
 
         See also
         --------
-        pdpy.signal.filter_design.bandpass
+        pydischarge.signal.filter_design.bandpass
             for details on the filter design
         TimeSeries.filter
             for details on how the filter is applied
         """
         # design filter
         filt = filter_design.bandpass(flow, fhigh, self.sample_rate,
                                       fstop=fstop, gpass=gpass, gstop=gstop,
@@ -1049,32 +1049,32 @@
         ------
         ValueError
             if ``filt`` arguments cannot be interpreted properly
 
         Examples
         --------
         We can design an arbitrarily complicated filter using
-        :mod:`pdpy.signal.filter_design`
+        :mod:`pydischarge.signal.filter_design`
 
-        >>> from pdpy.signal import filter_design
+        >>> from pydischarge.signal import filter_design
         >>> bp = filter_design.bandpass(50, 250, 4096.)
         >>> notches = [filter_design.notch(f, 4096.) for f in (60, 120, 180)]
         >>> zpk = filter_design.concatenate_zpks(bp, *notches)
 
         And then can download some data from GWOSC to apply it using
         `TimeSeries.filter`:
 
-        >>> from pdpy.timeseries import TimeSeries
+        >>> from pydischarge.timeseries import TimeSeries
         >>> data = TimeSeries.fetch_open_data('H1', 1126259446, 1126259478)
         >>> filtered = data.filter(zpk, filtfilt=True)
 
         We can plot the original signal, and the filtered version, cutting
         off either end of the filtered data to remove filter-edge artefacts
 
-        >>> from pdpy.plot import Plot
+        >>> from pydischarge.plot import Plot
         >>> plot = Plot(data, filtered[128:-128], separate=True)
         >>> plot.show()
         """
         # parse keyword arguments
         filtfilt = kwargs.pop('filtfilt', False)
 
         # parse filter
@@ -1134,15 +1134,15 @@
 
         **kwargs
             any other keyword arguments accepted by
             :meth:`TimeSeries.csd` or :meth:`TimeSeries.psd`
 
         Returns
         -------
-        transfer_function : `~pdpy.frequencyseries.FrequencySeries`
+        transfer_function : `~pydischarge.frequencyseries.FrequencySeries`
             the transfer function `FrequencySeries` of this `TimeSeries`
             with the other
 
         Notes
         -----
         If `self` and `other` have difference
         :attr:`TimeSeries.sample_rate` values, the higher sampled
@@ -1187,15 +1187,15 @@
             any other keyword arguments accepted by
             :func:`matplotlib.mlab.cohere` except ``NFFT``, ``window``,
             and ``noverlap`` which are superceded by the above keyword
             arguments
 
         Returns
         -------
-        coherence : `~pdpy.frequencyseries.FrequencySeries`
+        coherence : `~pydischarge.frequencyseries.FrequencySeries`
             the coherence `FrequencySeries` of this `TimeSeries`
             with the other
 
         Notes
         -----
         If `self` and `other` have difference
         :attr:`TimeSeries.sample_rate` values, the higher sampled
@@ -1247,15 +1247,15 @@
             any other keyword arguments accepted by
             :func:`matplotlib.mlab.cohere` except ``NFFT``, ``window``,
             and ``noverlap`` which are superceded by the above keyword
             arguments
 
         Returns
         -------
-        coherence : `~pdpy.frequencyseries.FrequencySeries`
+        coherence : `~pydischarge.frequencyseries.FrequencySeries`
             the coherence `FrequencySeries` of this `TimeSeries`
             with the other
 
         Notes
         -----
         The :meth:`TimeSeries.auto_coherence` will perform best when
         ``dt`` is approximately ``fftlength / 2``.
@@ -1300,15 +1300,15 @@
 
         nproc : `int`
             number of parallel processes to use when calculating
             individual coherence spectra.
 
         Returns
         -------
-        spectrogram : `~pdpy.spectrogram.Spectrogram`
+        spectrogram : `~pydischarge.spectrogram.Spectrogram`
             time-frequency coherence spectrogram as generated from the
             input time-series.
         """
         from ..spectrogram.coherence import from_timeseries
         return from_timeseries(self, other, stride, fftlength=fftlength,
                                overlap=overlap, window=window,
                                nproc=nproc)
@@ -1368,16 +1368,16 @@
 
         tpad : `float`, optional
             length of time (in seconds) over which to taper off data at
             mask segment boundaries, default: 0.5 seconds
 
         **kwargs : `dict`, optional
             additional keyword arguments to
-            `~pdpy.segments.DataQualityFlag.query` or
-            `~pdpy.segments.DataQualityFlag.fetch_open_data`,
+            `~pydischarge.segments.DataQualityFlag.query` or
+            `~pydischarge.segments.DataQualityFlag.fetch_open_data`,
             see "Notes" below
 
         Returns
         -------
         out : `TimeSeries`
             the masked version of this `TimeSeries`
 
@@ -1387,28 +1387,28 @@
         ramp data down to zero over a timescale `tpad` approaching every
         segment boundary in `deadtime`. However, this does not apply to
         the left or right bounds of the original `TimeSeries`.
 
         The `deadtime` segment list will always be coalesced and restricted to
         the limits of `self.span`. In particular, when querying a data-quality
         flag, this means the `start` and `end` arguments to
-        `~pdpy.segments.DataQualityFlag.query` will effectively be reset and
+        `~pydischarge.segments.DataQualityFlag.query` will effectively be reset and
         therefore need not be given.
 
         If `flag` is interpreted positively, i.e. if `flag` being active
         corresponds to a "good" state, then its complement in `self.span`
         will be used to define the deadtime for masking.
 
         See also
         --------
-        pdpy.segments.DataQualityFlag.query
+        pydischarge.segments.DataQualityFlag.query
             for the method to query segments of a given data-quality flag
-        pdpy.segments.DataQualityFlag.fetch_open_data
+        pydischarge.segments.DataQualityFlag.fetch_open_data
             for the method to query data-quality flags from the GWOSC database
-        pdpy.signal.window.planck
+        pydischarge.signal.window.planck
             for the generic Planck-taper window
         """
         query_method = (DataQualityFlag.fetch_open_data if query_open_data
                         else DataQualityFlag.query)
         (tstart, tend) = self.span
         span = SegmentList([self.span])
         sample = self.sample_rate.to('Hz').value
@@ -1472,26 +1472,26 @@
         Examples
         --------
         Demodulation is useful when trying to examine steady sinusoidal
         signals we know to be contained within data. For instance,
         we can download some data from GWOSC to look at trends of the
         amplitude and phase of LIGO Livingston's calibration line at 331.3 Hz:
 
-        >>> from pdpy.timeseries import TimeSeries
+        >>> from pydischarge.timeseries import TimeSeries
         >>> data = TimeSeries.fetch_open_data('L1', 1131350417, 1131357617)
 
         We can demodulate the `TimeSeries` at 331.3 Hz with a stride of one
         minute:
 
         >>> amp, phase = data.demodulate(331.3, stride=60)
 
         We can then plot these trends to visualize fluctuations in the
         amplitude of the calibration line:
 
-        >>> from pdpy.plot import Plot
+        >>> from pydischarge.plot import Plot
         >>> plot = Plot(amp)
         >>> ax = plot.gca()
         >>> ax.set_ylabel('Strain Amplitude at 331.3 Hz')
         >>> plot.show()
 
         See also
         --------
@@ -1535,19 +1535,19 @@
         -------
         out : `TimeSeries`
             magnitude and phase trends, represented as
             `mag * exp(1j*phase)` with `dt=stride`
 
         Notes
         -----
-        This is similar to the :meth:`~pdpy.timeseries.TimeSeries.demodulate`
+        This is similar to the :meth:`~pydischarge.timeseries.TimeSeries.demodulate`
         method, but is more general in that it accepts a varying phase
         evolution, rather than a fixed frequency.
 
-        Unlike :meth:`~pdpy.timeseries.TimeSeries.demodulate`, the complex
+        Unlike :meth:`~pydischarge.timeseries.TimeSeries.demodulate`, the complex
         output is double-sided by default, so is not multiplied by 2.
 
         Examples
         --------
         Heterodyning can be useful in analysing quasi-monochromatic signals
         with a known phase evolution, such as continuous-wave signals
         from rapidly rotating neutron stars. These sources radiate at a
@@ -1556,15 +1556,15 @@
 
         To see an example of heterodyning in action, we can simulate a signal
         whose phase evolution is described by the frequency and its first
         derivative with respect to time. We can download some O1 era
         LIGO-Livingston data from GWOSC, inject the simulated signal, and
         recover its amplitude.
 
-        >>> from pdpy.timeseries import TimeSeries
+        >>> from pydischarge.timeseries import TimeSeries
         >>> data = TimeSeries.fetch_open_data('L1', 1131350417, 1131354017)
 
         We now need to set the signal parameters, generate the expected
         phase evolution, and create the signal:
 
         >>> import numpy
         >>> f0 = 123.456789  # signal frequency (Hz)
@@ -1650,34 +1650,34 @@
 
         Examples
         --------
         To see the effect of the Planck-taper window, we can taper a
         sinusoidal `TimeSeries` at both ends:
 
         >>> import numpy
-        >>> from pdpy.timeseries import TimeSeries
+        >>> from pydischarge.timeseries import TimeSeries
         >>> t = numpy.linspace(0, 1, 2048)
         >>> series = TimeSeries(numpy.cos(10.5*numpy.pi*t), times=t)
         >>> tapered = series.taper()
 
         We can plot it to see how the ends now vary smoothly from 0 to 1:
 
-        >>> from pdpy.plot import Plot
+        >>> from pydischarge.plot import Plot
         >>> plot = Plot(series, tapered, separate=True, sharex=True)
         >>> plot.show()
 
         Notes
         -----
         The :meth:`TimeSeries.taper` automatically tapers from the second
         stationary point (local maximum or minimum) on the specified side
         of the input. However, the method will never taper more than half
         the full width of the `TimeSeries`, and will fail if there are no
         stationary points.
 
-        See :func:`~pdpy.signal.window.planck` for the generic Planck taper
+        See :func:`~pydischarge.signal.window.planck` for the generic Planck taper
         window, and see :func:`scipy.signal.get_window` for other common
         window formats.
         """
         # check window properties
         if side not in ('left', 'right', 'leftright'):
             raise ValueError("side must be one of 'left', 'right', "
                              "or 'leftright'")
@@ -1724,15 +1724,15 @@
             see :func:`scipy.signal.get_window` for details on acceptable
             formats
 
         detrend : `str`, optional
             type of detrending to do before FFT (see `~TimeSeries.detrend`
             for more details), default: ``'constant'``
 
-        asd : `~pdpy.frequencyseries.FrequencySeries`, optional
+        asd : `~pydischarge.frequencyseries.FrequencySeries`, optional
             the amplitude spectral density using which to whiten the data,
             overrides other ASD arguments, default: `None`
 
         fduration : `float`, optional
             duration (in seconds) of the time-domain FIR whitening filter,
             must be no longer than `fftlength`, default: 2 seconds
 
@@ -1753,15 +1753,15 @@
 
         See also
         --------
         TimeSeries.asd
             for details on the ASD calculation
         TimeSeries.convolve
             for details on convolution with the overlap-save method
-        pdpy.signal.filter_design.fir_from_transfer
+        pydischarge.signal.filter_design.fir_from_transfer
             for FIR filter design through spectrum truncation
 
         Notes
         -----
         The accepted ``method`` arguments are:
 
         - ``'bartlett'`` : a mean average of non-overlapping periodograms
@@ -1826,15 +1826,15 @@
         **whiten_kwargs
             other keyword arguments that will be passed to the
             `TimeSeries.whiten` method if it is being used when discovering
             gating points
 
         Returns
         -------
-        out : `~pdpy.segments.SegmentList`
+        out : `~pydischarge.segments.SegmentList`
             a list of segments that should be gated based on the
             provided parameters
 
         See also
         --------
         TimeSeries.gate
             for a method that applies the identified gates
@@ -1882,23 +1882,23 @@
         **whiten_kwargs
             other keyword arguments that will be passed to the
             `TimeSeries.whiten` method if it is being used when discovering
             gating points
 
         Returns
         -------
-        out : `~pdpy.timeseries.TimeSeries`
+        out : `~pydischarge.timeseries.TimeSeries`
             a copy of the original `TimeSeries` that has had gating windows
             applied
 
         Examples
         --------
         Read data into a `TimeSeries`
 
-        >>> from pdpy.timeseries import TimeSeries
+        >>> from pydischarge.timeseries import TimeSeries
         >>> data = TimeSeries.fetch_open_data('H1', 1135148571, 1135148771)
 
         Apply gating using custom arguments
 
         >>> gated = data.gate(tzero=1.0, tpad=1.0, threshold=10.0,
                               fftlength=4, overlap=2, method='median')
 
@@ -2177,17 +2177,17 @@
             a table of time-frequency tiles on the most significant `QPlane`
 
         See also
         --------
         TimeSeries.q_transform
             for a method to interpolate the raw Q-transform over a regularly
             gridded spectrogram
-        pdpy.signal.qtransform
+        pydischarge.signal.qtransform
             for code and documentation on how the Q-transform is implemented
-        pdpy.table.EventTable.tile
+        pydischarge.table.EventTable.tile
             to render this `EventTable` as a collection of polygons
 
         Notes
         -----
         Only tiles with signal energy greater than or equal to
         `snrthresh ** 2 / 2` will be stored in the output `EventTable`. The
         table columns are ``'time'``, ``'duration'``, ``'frequency'``,
@@ -2257,21 +2257,21 @@
             whether to normalize the returned Q-transform output, or how,
             default: `True` (``'median'``), other options: `False`,
             ``'mean'``
 
         mismatch : `float`
             maximum allowed fractional mismatch between neighbouring tiles
 
-        outseg : `~pdpy.segments.Segment`, optional
+        outseg : `~pydischarge.segments.Segment`, optional
             GPS `[start, stop)` segment for output `Spectrogram`,
             default is the full duration of the input
 
-        whiten : `bool`, `~pdpy.frequencyseries.FrequencySeries`, optional
+        whiten : `bool`, `~pydischarge.frequencyseries.FrequencySeries`, optional
             boolean switch to enable (`True`) or disable (`False`) data
-            whitening, or an ASD `~pdpy.freqencyseries.FrequencySeries`
+            whitening, or an ASD `~pydischarge.freqencyseries.FrequencySeries`
             with which to whiten the data
 
         fduration : `float`, optional
             duration (in seconds) of the time-domain FIR whitening filter,
             only used if `whiten` is not `False`, defaults to 2 seconds
 
         highpass : `float`, optional
@@ -2280,33 +2280,33 @@
 
         **asd_kw
             keyword arguments to pass to `TimeSeries.asd` to generate
             an ASD to use when whitening the data
 
         Returns
         -------
-        out : `~pdpy.spectrogram.Spectrogram`
+        out : `~pydischarge.spectrogram.Spectrogram`
             output `Spectrogram` of normalised Q energy
 
         See also
         --------
         TimeSeries.asd
             for documentation on acceptable `**asd_kw`
         TimeSeries.whiten
             for documentation on how the whitening is done
-        pdpy.signal.qtransform
+        pydischarge.signal.qtransform
             for code and documentation on how the Q-transform is implemented
 
         Notes
         -----
         This method will return a `Spectrogram` of dtype ``float32`` if
         ``norm`` is given, and ``float64`` otherwise.
 
         To optimize plot rendering with `~matplotlib.axes.Axes.pcolormesh`,
-        the output `~pdpy.spectrogram.Spectrogram` can be given a log-sampled
+        the output `~pydischarge.spectrogram.Spectrogram` can be given a log-sampled
         frequency axis by passing `logf=True` at runtime. The `fres` argument
         is then the number of points on the frequency axis. Note, this is
         incompatible with `~matplotlib.axes.Axes.imshow`.
 
         It is also highly recommended to use the `outseg` keyword argument
         when only a small window around a given GPS time is of interest. This
         will speed up this method a little, but can greatly speed up
@@ -2314,15 +2314,15 @@
 
         If you aren't going to use `pcolormesh` in the end, don't worry.
 
         Examples
         --------
         >>> from numpy.random import normal
         >>> from scipy.signal import gausspulse
-        >>> from pdpy.timeseries import TimeSeries
+        >>> from pydischarge.timeseries import TimeSeries
 
         Generate a `TimeSeries` containing Gaussian noise sampled at 4096 Hz,
         centred on GPS time 0, with a sine-Gaussian pulse ('glitch') at
         500 Hz:
 
         >>> noise = TimeSeries(normal(loc=1, size=4096*4), sample_rate=4096, epoch=-2)
         >>> glitch = TimeSeries(gausspulse(noise.times.value, fc=500) * 4, sample_rate=4096)
```

### Comparing `pydischarge-0.0.1/pdpy/types/__init__.py` & `pydischarge-0.0.2/pydischarge/signal/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) Duncan Macleod (2014-2020)
+# Copyright (C) Duncan Macleod (2016-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""This module provides the core `Array` object and direct subclasses.
+"""The `gwpy.signal` module provides signal-processing utilities that
+extend the functionality of `scipy.signal` (and others) for specific GW data
+applications.
 
-These objects form the basic 1-D and 2-D arrays with metadata from which
-we can build specific data representations like the `TimeSeries`.
+See the sub-modules for more details.
 """
 
-
-from .array import Array
-from .array2d import Array2D
-from .index import Index
-from .series import Series
-
-from . import io
-
-__author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__all__ = ['Array', 'Series', 'Array2D', 'Index']
+__author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
```

### Comparing `pydischarge-0.0.1/pdpy/types/array.py` & `pydischarge-0.0.2/pydischarge/types/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module provides the `Array`.
 
 The `Array` structure provides the core array-with-metadata environment
 with the standard array methods wrapped to return instances of itself.
 
 Each sub-class of `Array` should override the `Array._metadata_slots`
@@ -57,22 +57,22 @@
     ----------
     value : array-like
         input data array
 
     unit : `~astropy.units.Unit`, optional
         physical unit of these data
 
-    epoch : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+    epoch : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
         GPS epoch associated with these data,
-        any input parsable by `~pdpy.time.to_gps` is fine
+        any input parsable by `~pydischarge.time.to_gps` is fine
 
     name : `str`, optional
         descriptive title for this array
 
-    channel : `~pdpy.detector.Channel`, `str`, optional
+    channel : `~pydischarge.detector.Channel`, `str`, optional
         source data stream for these data
 
     dtype : `~numpy.dtype`, optional
         input data type
 
     copy : `bool`, optional, default: `False`
         choose to copy the input data to new memory
@@ -331,15 +331,15 @@
             pass
 
     # channel
     @property
     def channel(self):
         """Instrumental channel associated with these data
 
-        :type: `~pdpy.detector.Channel`
+        :type: `~pydischarge.detector.Channel`
         """
         try:
             return self._channel
         except AttributeError:
             self._channel = None
             return self._channel
```

### Comparing `pydischarge-0.0.1/pdpy/types/array2d.py` & `pydischarge-0.0.2/pydischarge/types/array2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """The `Series` is a one-dimensional array with metadata
 """
 
 from warnings import warn
 
 
@@ -68,22 +68,22 @@
         takes precedence over `y0` and `dy` so should be
         given in place of these if relevant, not alongside
 
     yunit : `~astropy.units.Unit`, optional
         the unit of the y-axis coordinates. If not given explicitly, it will be
         taken from any of `dy`, `y0`, or `yindex`, or set to a boring default
 
-    epoch : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+    epoch : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
         GPS epoch associated with these data,
-        any input parsable by `~pdpy.time.to_gps` is fine
+        any input parsable by `~pydischarge.time.to_gps` is fine
 
     name : `str`, optional
         descriptive title for this array
 
-    channel : `~pdpy.detector.Channel`, `str`, optional
+    channel : `~pydischarge.detector.Channel`, `str`, optional
         source data stream for these data
 
     dtype : `~numpy.dtype`, optional
         input data type
 
     copy : `bool`, optional, default: `False`
         choose to copy the input data to new memory
@@ -279,15 +279,15 @@
         except AttributeError:
             pass
 
     @property
     def yspan(self):
         """Y-axis [low, high) segment encompassed by these data
 
-        :type: `~pdpy.segments.Segment`
+        :type: `~pydischarge.segments.Segment`
         """
         return self._index_span("y")
 
     @property
     def T(self):
         trans = self.value.T.view(type(self))
         trans.__array_finalize__(self)
@@ -301,17 +301,17 @@
         else:
             trans.x0 = self.y0
             trans.dx = self.dy
         return trans
 
     # -- Array2D methods ------------------------
 
-    def _is_compatible_pdpy(self, other):
+    def _is_compatible_pydischarge(self, other):
         self._compare_index(other, "y")
-        return super()._is_compatible_pdpy(other)
+        return super()._is_compatible_pydischarge(other)
 
     def value_at(self, x, y):
         """Return the value of this `Series` at the given `(x, y)` coordinates
 
         Parameters
         ----------
         x : `float`, `~astropy.units.Quantity`
```

### Comparing `pydischarge-0.0.1/pdpy/types/index.py` & `pydischarge-0.0.2/pydischarge/types/index.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Quantity array for indexing a Series
 """
 
 import numpy
 
 from astropy.units import Quantity
```

### Comparing `pydischarge-0.0.1/pdpy/types/io/ascii.py` & `pydischarge-0.0.2/pydischarge/types/io/ascii.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read a `Series` from AN ASCII file
 
 These files should be in two-column x,y format
 """
 
 from numpy import (savetxt, loadtxt, column_stack)
@@ -50,15 +50,15 @@
 # -- write --------------------------------------------------------------------
 
 def write_ascii_series(series, output, **kwargs):
     """Write a `Series` to a file in ASCII format
 
     Parameters
     ----------
-    series : :class:`~pdpy.data.Series`
+    series : :class:`~pydischarge.data.Series`
         data series to write
 
     output : `str`, `file`
         file to write to
 
     See also
     --------
```

### Comparing `pydischarge-0.0.1/pdpy/types/io/hdf5.py` & `pydischarge-0.0.2/pydischarge/types/io/hdf5.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Basic HDF5 I/O methods for Array and sub-classes
 """
 
 import pickle
 from decimal import Decimal
 from operator import attrgetter
@@ -134,15 +134,15 @@
 def write_hdf5_array(array, h5g, path=None, attrs=None,
                      append=False, overwrite=False,
                      compression='gzip', **kwargs):
     """Write the ``array`` to an `h5py.Dataset`
 
     Parameters
     ----------
-    array : `pdpy.types.Array`
+    array : `pydischarge.types.Array`
         the data object to write
 
     h5g : `str`, `h5py.Group`
         a file path to write to, or an `h5py.Group` in which to create
         a new dataset
 
     path : `str`, optional
```

### Comparing `pydischarge-0.0.1/pdpy/types/io/ligolw.py` & `pydischarge-0.0.2/pydischarge/types/io/ligolw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Read/write series in LIGO_LW-XML
 """
 
 from .. import Series
 from ...io.ligolw import read_ligolw
 from ...time import to_gps
@@ -179,15 +179,15 @@
 
     **params
         other ``<Param>`` ``(name, value)`` pairs to use in matching
         the parent correct ``<LIGO_LW>`` element to read
 
     Returns
     -------
-    series : `~pdpy.types.Series`
+    series : `~pydischarge.types.Series`
         a series with metadata read from the ``<Array>``
     """
     from ligo.lw.ligolw import Dim
 
     # read document and find relevant <Array> element
     xmldoc = read_ligolw(
         source,
```

### Comparing `pydischarge-0.0.1/pdpy/types/series.py` & `pydischarge-0.0.2/pydischarge/types/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """The `Series` is a one-dimensional array with metadata
 """
 
 from warnings import warn
 from math import floor
 
@@ -62,22 +62,22 @@
         takes precedence over `x0` and `dx` so should be
         given in place of these if relevant, not alongside
 
     xunit : `~astropy.units.Unit`, optional
         the unit of the x-axis index. If not given explicitly, it will be
         taken from any of `dx`, `x0`, or `xindex`, or set to a boring default
 
-    epoch : `~pdpy.time.LIGOTimeGPS`, `float`, `str`, optional
+    epoch : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`, optional
         GPS epoch associated with these data,
-        any input parsable by `~pdpy.time.to_gps` is fine
+        any input parsable by `~pydischarge.time.to_gps` is fine
 
     name : `str`, optional
         descriptive title for this array
 
-    channel : `~pdpy.detector.Channel`, `str`, optional
+    channel : `~pydischarge.detector.Channel`, `str`, optional
         source data stream for these data
 
     dtype : `~numpy.dtype`, optional
         input data type
 
     copy : `bool`, optional, default: `False`
         choose to copy the input data to new memory
@@ -363,15 +363,15 @@
             self.dx = self.dx.to(unit)
             self.x0 = self.x0.to(unit)
 
     @property
     def xspan(self):
         """X-axis [low, high) segment encompassed by these data
 
-        :type: `~pdpy.segments.Segment`
+        :type: `~pydischarge.segments.Segment`
         """
         return self._index_span("x")
 
     # -- series i/o -----------------------------
 
     @classmethod
     def read(cls, source, *args, **kwargs):
@@ -494,15 +494,15 @@
         ----------
         delta : `float`, `~astropy.units.Quantity`, `str`
             The amount by which to shift (in x-axis units if `float`), give
             a negative value to shift backwards in time
 
         Examples
         --------
-        >>> from pdpy.types import Series
+        >>> from pydischarge.types import Series
         >>> a = Series([1, 2, 3, 4, 5], x0=0, dx=1, xunit='m')
         >>> print(a.x0)
         0.0 m
         >>> a.shift(5)
         >>> print(a.x0)
         5.0 m
         >>> a.shift('-1 km')
@@ -655,15 +655,15 @@
     def is_compatible(self, other):
         """Check whether this series and other have compatible metadata
 
         This method tests that the `sample size <Series.dx>`, and the
         `~Series.unit` match.
         """
         if isinstance(other, type(self)):
-            return self._is_compatible_pdpy(other)
+            return self._is_compatible_pydischarge(other)
         return self._is_compatible_numpy(other)
 
     def _compatibility_error(self, other, attr, name):
         return ValueError(
             "{} {} do not match: {} vs {}".format(
                 type(self).__name__,
                 name,
@@ -702,15 +702,15 @@
             ):
                 raise self._compatibility_error(
                     other,
                     _index,
                     "{}-axis indexes".format(axis),
                 )
 
-    def _is_compatible_pdpy(self, other):
+    def _is_compatible_pydischarge(self, other):
         """Check whether this series and another series are compatible
         """
         self._compare_index(other, axis="x")
 
         # check units
         if not (
             self.unit == other.unit
@@ -1096,15 +1096,15 @@
 
         If `self.xindex` is an array of timestamps, and if `other.xspan` is
         not a subset of `self.xspan`, then `other` will be cropped before
         being adding to `self`.
 
         Users who wish to taper or window their `Series` should do so before
         passing it to this method. See :meth:`TimeSeries.taper` and
-        :func:`~pdpy.signal.window.planck` for more information.
+        :func:`~pydischarge.signal.window.planck` for more information.
         """
         # check Series compatibility
         self.is_compatible(other)
         if (self.xunit == second) and (other.xspan[0] < self.xspan[0]):
             other = other.crop(start=self.xspan[0])
         if (self.xunit == second) and (other.xspan[1] > self.xspan[1]):
             other = other.crop(end=self.xspan[1])
```

### Comparing `pydischarge-0.0.1/pdpy/types/sliceutils.py` & `pydischarge-0.0.2/pydischarge/types/sliceutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utilities for the core types
 
 These methods are designed for internal use only.
 """
 
 from numbers import Integral
```

### Comparing `pydischarge-0.0.1/pdpy/types/tests/test_array.py` & `pydischarge-0.0.2/pydischarge/types/tests/test_array.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit test for pdpy.types classes
+"""Unit test for pydischarge.types classes
 """
 
 import pickle
 import warnings
 from unittest import mock
 
 import pytest
@@ -44,15 +44,15 @@
 GPS_EPOCH = 12345
 TIME_EPOCH = Time(12345, format='gps', scale='utc')
 CHANNEL_NAME = 'G1:TEST-CHANNEL'
 CHANNEL = Channel(CHANNEL_NAME)
 
 
 class TestArray(object):
-    """Test `pdpy.types.Array`
+    """Test `pydischarge.types.Array`
     """
     TEST_CLASS = Array
     DTYPE = None
 
     # -- setup ----------------------------------
 
     @classmethod
@@ -117,15 +117,15 @@
 
         # test unit gets passed properly
         array = self.create(unit='m')
         assert array.unit is units.m
 
         # test unrecognised units
         with mock.patch.dict(
-                'pdpy.detector.units.UNRECOGNIZED_UNITS', clear=True), \
+                'pydischarge.detector.units.UNRECOGNIZED_UNITS', clear=True), \
                 pytest.warns(units.UnitsWarning):
             array = self.create(unit='blah')
         assert isinstance(array.unit, units.IrreducibleUnit)
         assert str(array.unit) == 'blah'
 
         # test setting unit doesn't work
         with pytest.raises(AttributeError):
@@ -252,15 +252,15 @@
         # check basic override works
         array.override_unit('m')
         assert array.unit is units.meter
 
         # check parse_strict works for each of 'raise' (default), 'warn',
         # and 'silent'
         with mock.patch.dict(
-                'pdpy.detector.units.UNRECOGNIZED_UNITS', clear=True):
+                'pydischarge.detector.units.UNRECOGNIZED_UNITS', clear=True):
             with pytest.raises(ValueError):
                 array.override_unit('blah', parse_strict='raise')
             with pytest.warns(units.UnitsWarning):
                 array.override_unit('blah', parse_strict='warn')
             array.override_unit('blah', parse_strict='silent')
         assert isinstance(array.unit, units.IrreducibleUnit)
         assert str(array.unit) == 'blah'
```

### Comparing `pydischarge-0.0.1/pdpy/types/tests/test_array2d.py` & `pydischarge-0.0.2/pydischarge/types/tests/test_array2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.types.array2d`
+"""Unit tests for :mod:`pydischarge.types.array2d`
 """
 
 import pytest
 
 import numpy
 
 from astropy import units
@@ -194,15 +194,15 @@
         )
 
     def test_single_column_slice(self):
         """Check that we can slice an `Array2D` into a single column.
 
         But still represent the output as an `Array2D` with `Index` arrays.
 
-        This tests regression of https://github.com/pdpy-github/pdpy/issues/1504.
+        This tests regression of https://github.com/pydischarge-github/pydischarge/issues/1504.
         """
         # create an array with indices
         a = self.create()
         a.xindex
         a.yindex
 
         # select a slice of width 1 (as opposed to indexing a single column)
```

### Comparing `pydischarge-0.0.1/pdpy/types/tests/test_index.py` & `pydischarge-0.0.2/pydischarge/types/tests/test_index.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for :mod:`pdpy.types.index`
+"""Unit tests for :mod:`pydischarge.types.index`
 """
 
 from astropy import units
 
 from .. import Index
 
 
 class TestIndex(object):
     TEST_CLASS = Index
 
     def test_define_regular(self):
-        """Check for regression against pdpy/pdpy#1596.
+        """Check for regression against pydischarge/pydischarge#1596.
         """
         ind_len = 1000
         a = self.TEST_CLASS.define(
             1262936373.4853957,
             0.051,
             ind_len
         )
         assert len(a) == ind_len
 
     def test_define_index_length(self):
-        """Check for regression against pdpy/pdpy#1506.
+        """Check for regression against pydischarge/pydischarge#1506.
         """
         a = self.TEST_CLASS.define(
             units.Quantity(1000000000),
             units.Quantity(0.01),
             500,
         )
         assert a.is_regular()
```

### Comparing `pydischarge-0.0.1/pdpy/types/tests/test_series.py` & `pydischarge-0.0.2/pydischarge/types/tests/test_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for pdpy.types.series
+"""Unit tests for pydischarge.types.series
 """
 
 import warnings
 
 import numpy
 
 import pytest
```

### Comparing `pydischarge-0.0.1/pdpy/utils/__init__.py` & `pydischarge-0.0.2/pydischarge/timeseries/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Miscellaneous utilties for PDpy
+"""Create, manipulate, read, and write time-series data
 """
 
-from sys import stdout
+from .core import (TimeSeriesBase, TimeSeriesBaseDict, TimeSeriesBaseList)
+from .timeseries import (TimeSeries, TimeSeriesDict, TimeSeriesList)
+from .statevector import (StateVector, StateVectorDict, StateVectorList,
+                          StateTimeSeries, StateTimeSeriesDict, Bits)
 
-from .misc import (
-    gprint,
-    if_not_none,
-    null_context,
-    round_to_power,
-    unique,
-)
+from . import io
 
-__author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
+__author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
```

### Comparing `pydischarge-0.0.1/pdpy/utils/decorators.py` & `pydischarge-0.0.2/pydischarge/utils/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Decorators for PDpy
+"""Decorators for pyDischarge
 """
 
 import warnings
 from functools import wraps
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
```

### Comparing `pydischarge-0.0.1/pdpy/utils/enum.py` & `pydischarge-0.0.2/pydischarge/utils/enum.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2019-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utilties for enumerations
 """
 
 from enum import Enum
 
 import numpy
```

### Comparing `pydischarge-0.0.1/pdpy/utils/env.py` & `pydischarge-0.0.2/pydischarge/utils/env.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Environment utilities for PDpy
+"""Environment utilities for pyDischarge
 """
 
 import os
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 TRUE = (
@@ -57,15 +57,15 @@
         if the environment variable matches as 'yes' or similar
     False
         otherwise
 
     Examples
     --------
     >>> import os
-    >>> from pdpy.utils.env import bool_env
+    >>> from pydischarge.utils.env import bool_env
     >>> os.environ['GWPY_VALUE'] = 'yes'
     >>> print(bool_env('GWPY_VALUE'))
     True
     >>> os.environ['GWPY_VALUE'] = 'something else'
     >>> print(bool_env('GWPY_VALUE'))
     False
     >>> print(bool_env('GWPY_VALUE2'))
```

### Comparing `pydischarge-0.0.1/pdpy/utils/lal.py` & `pydischarge-0.0.2/pydischarge/utils/lal.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utilies for interacting with the LIGO Algorithm Library.
 
 This module requires lal >= 6.14.0
 """
 
 import operator
@@ -30,16 +30,16 @@
 import numpy
 
 from astropy import units
 
 import lal
 
 from ..time import to_gps
-# import pdpy.detector.units to register other units now
-from ..detector import units as pdpy_units  # noqa: F401
+# import pydischarge.detector.units to register other units now
+from ..detector import units as pydischarge_units  # noqa: F401
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 # -- type matching ------------------------------------------------------------
 
 # LAL type enum
 LAL_TYPE_STR = {
@@ -80,15 +80,15 @@
 def to_lal_type_str(pytype):
     """Convert the input python type to a LAL type string
 
     Examples
     --------
     To convert a python type:
 
-    >>> from pdpy.utils.lal import to_lal_type_str
+    >>> from pydischarge.utils.lal import to_lal_type_str
     >>> to_lal_type_str(float)
     'REAL8'
 
     To convert a `numpy.dtype`:
 
     >>> import numpy
     >>> to_lal_type_str(numpy.dtype('uint32'))
@@ -137,15 +137,15 @@
     Raises
     ------
     AttributeError
         if the function is not found
 
     Examples
     --------
-    >>> from pdpy.utils.lal import find_typed_function
+    >>> from pydischarge.utils.lal import find_typed_function
     >>> find_typed_function(float, 'Create', 'Sequence')
     <built-in function CreateREAL8Sequence>
     """
     laltype = to_lal_type_str(pytype)
     return getattr(module, '{0}{1}{2}'.format(prefix, laltype, suffix))
 
 
@@ -298,16 +298,16 @@
 
 
 def to_lal_ligotimegps(gps):
     """Convert the given GPS time to a `lal.LIGOTimeGPS` object
 
     Parameters
     ----------
-    gps : `~pdpy.time.LIGOTimeGPS`, `float`, `str`
-        input GPS time, can be anything parsable by :meth:`~pdpy.time.to_gps`
+    gps : `~pydischarge.time.LIGOTimeGPS`, `float`, `str`
+        input GPS time, can be anything parsable by :meth:`~pydischarge.time.to_gps`
 
     Returns
     -------
     ligotimegps : `lal.LIGOTimeGPS`
         a SWIG-LAL `~lal.LIGOTimeGPS` representation of the given GPS time
     """
     gps = to_gps(gps)
```

### Comparing `pydischarge-0.0.1/pdpy/utils/misc.py` & `pydischarge-0.0.2/pydischarge/utils/misc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Miscellaneous utilties for PDpy
+"""Miscellaneous utilties for pyDischarge
 """
 
 import sys
 import math
 import warnings
 from collections import OrderedDict
 from contextlib import nullcontext
@@ -39,28 +39,28 @@
 gprint.__doc__ = print.__doc__
 
 
 def null_context():
     """Null context manager
     """
     warnings.warn(
-        "pdpy.utils.null_context is deprecated and will be removed in "
-        "PDpy 3.1.0, please update your code to use "
+        "pydischarge.utils.null_context is deprecated and will be removed in "
+        "pyDischarge 3.1.0, please update your code to use "
         "contextlib.nullcontext from the Python standard library (>=3.7)",
         DeprecationWarning,
     )
     return nullcontext()
 
 
 def if_not_none(func, value):
     """Apply func to value if value is not None
 
     Examples
     --------
-    >>> from pdpy.utils.misc import if_not_none
+    >>> from pydischarge.utils.misc import if_not_none
     >>> if_not_none(int, '1')
     1
     >>> if_not_none(int, None)
     None
     """
     if value is None:
         return
@@ -89,15 +89,15 @@
 
     Notes
     -----
     The object returned will be of the same type as `base`.
 
     Examples
     --------
-    >>> from pdpy.utils.misc import round_to_power
+    >>> from pydischarge.utils.misc import round_to_power
     >>> round_to_power(2)
     2
     >>> round_to_power(9, base=10)
     10
     >>> round_to_power(5, which='lower')
     4
     """
@@ -115,12 +115,12 @@
 
 def unique(list_):
     """Return a version of the input list with unique elements,
     preserving order
 
     Examples
     --------
-    >>> from pdpy.utils.misc import unique
+    >>> from pydischarge.utils.misc import unique
     >>> unique(['b', 'c', 'a', 'a', 'd', 'e', 'd', 'a'])
     ['b', 'c', 'a', 'd', 'e']
     """
     return list(OrderedDict.fromkeys(list_).keys())
```

### Comparing `pydischarge-0.0.1/pdpy/utils/mp.py` & `pydischarge-0.0.2/pydischarge/utils/mp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utilities for multi-processing
 """
 
 import warnings
 from multiprocessing import (Queue, Process)
 from operator import itemgetter
```

### Comparing `pydischarge-0.0.1/pdpy/utils/progress.py` & `pydischarge-0.0.2/pydischarge/utils/progress.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2017-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utilities for multi-processing
 """
 
 import sys
 
 from tqdm import tqdm
```

### Comparing `pydischarge-0.0.1/pdpy/utils/shell.py` & `pydischarge-0.0.2/pydischarge/utils/shell.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utilities for calling out to the shell
 """
 
 import warnings
 from distutils.spawn import find_executable
 from subprocess import (Popen, PIPE, CalledProcessError)
@@ -26,15 +26,15 @@
 from .decorators import deprecated_function
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 
 @deprecated_function(
     message=(
-        "pdpy.utils.shell.which is deprecated in favour of shutil.which from "
+        "pydischarge.utils.shell.which is deprecated in favour of shutil.which from "
         "the Python standard library, and will be removed in a future release"
     ),
 )
 def which(program):
     """Find full path of executable program
 
     Parameters
@@ -56,15 +56,15 @@
     if exe is None:
         raise ValueError("No executable '%s' found in PATH" % program)
     return exe
 
 
 @deprecated_function(
     message=(
-        "pdpy.utils.shell.call is deprecated in favour of subprocess.call "
+        "pydischarge.utils.shell.call is deprecated in favour of subprocess.call "
         "from the Python standard library, and will be removed in a "
         "future release."
     ),
 )
 def call(cmd, stdout=PIPE, stderr=PIPE, on_error='raise', **kwargs):
     """Call out to the shell using `subprocess.Popen`
```

### Comparing `pydischarge-0.0.1/pdpy/utils/sphinx/epydoc.py` & `pydischarge-0.0.2/pydischarge/utils/sphinx/epydoc.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.1/pdpy/utils/sphinx/ex2rst.py` & `pydischarge-0.0.2/pydischarge/utils/sphinx/ex2rst.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Louisiana State University (2014-2017)
 #               Cardiff University (2017-2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Convert PDpy example python files into rst files for sphinx documentation
+"""Convert pyDischarge example python files into rst files for sphinx documentation
 """
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org'
 
 import argparse
 import sys
 from pathlib import Path
@@ -55,15 +55,15 @@
         the fully rendered RST text block
     """
     infile = Path(infile)
     lines = infile.read_text().splitlines()
     ref = '-'.join((infile.parent.name, infile.with_suffix("").name))
 
     output = []
-    header = ['.. _pdpy-example-%s:\n' % ref]
+    header = ['.. _pydischarge-example-%s:\n' % ref]
 
     indoc = False
     incode = False
     code = []
     context = "reset"
 
     for i, line in enumerate(lines):
```

### Comparing `pydischarge-0.0.1/pdpy/utils/sphinx/zenodo.py` & `pydischarge-0.0.2/pydischarge/utils/sphinx/zenodo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 import argparse
 import requests
 import sys
 
 
 def parse_command_line():
```

### Comparing `pydischarge-0.0.1/pdpy/utils/tests/test_decorators.py` & `pydischarge-0.0.2/pydischarge/utils/tests/test_decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.utils.decorators`
+"""Tests for :mod:`pydischarge.utils.decorators`
 """
 
 import pytest
 
 from .. import decorators
 
 
 def test_return_as():
-    """Test `pdpy.utils.decorators.return_as` works
+    """Test `pydischarge.utils.decorators.return_as` works
     """
     @decorators.return_as(float)
     def myfunc(value):
         return int(value)
 
     result = myfunc(1.5)
 
     # check type was cast
     assert isinstance(result, float)
     # check result is still the same
     assert result == 1.0
 
 
 def test_return_as_error():
-    """Test that `pdpy.utils.decorators.return_as` error handling works
+    """Test that `pydischarge.utils.decorators.return_as` error handling works
     """
     @decorators.return_as(int)
     def myfunc(value):
         return str(value)
 
     with pytest.raises(
         ValueError,
```

### Comparing `pydischarge-0.0.1/pdpy/utils/tests/test_enum.py` & `pydischarge-0.0.2/pydischarge/utils/tests/test_enum.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2019-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.utils.enum`
+"""Tests for :mod:`pydischarge.utils.enum`
 """
 
 import pytest
 
 import numpy
 
-from .. import enum as pdpy_enum
+from .. import enum as pydischarge_enum
 
 
-class _MyEnum(pdpy_enum.NumpyTypeEnum):
+class _MyEnum(pydischarge_enum.NumpyTypeEnum):
     INT16 = 100
     FLOAT32 = 200
 
 
 class TestNumpyTypeEnum(object):
     TEST_CLASS = _MyEnum
```

### Comparing `pydischarge-0.0.1/pdpy/utils/tests/test_env.py` & `pydischarge-0.0.2/pydischarge/utils/tests/test_env.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2018-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.utils.env`
+"""Tests for :mod:`pydischarge.utils.env`
 """
 
 from unittest import mock
 
 import pytest
 
 from .. import env as utils_env
@@ -52,21 +52,21 @@
 @mock.patch.dict('os.environ', values=BOOL_ENV)
 @pytest.mark.parametrize(
     'env, result',
     [(k, True) for k in sorted(BOOL_TRUE)]
     + [(k, False) for k in sorted(BOOL_FALSE)],
 )
 def test_bool_env(env, result):
-    """Test :meth:`pdpy.utils.env.bool_env` _without_ the `default` keyword
+    """Test :meth:`pydischarge.utils.env.bool_env` _without_ the `default` keyword
     """
     assert utils_env.bool_env(env) is result
 
 
 @mock.patch.dict('os.environ', values=BOOL_TRUE)
 @pytest.mark.parametrize('env, default, result', [
     ('TEST_YES', False, True),
     ('TEST_MISSING', True, True),
 ])
 def test_bool_env_default(env, default, result):
-    """Test :meth:`pdpy.utils.env.bool_env` _with_ the `default` keyword
+    """Test :meth:`pydischarge.utils.env.bool_env` _with_ the `default` keyword
     """
     assert utils_env.bool_env(env, default=default) is result
```

### Comparing `pydischarge-0.0.1/pdpy/utils/tests/test_lal.py` & `pydischarge-0.0.2/pydischarge/utils/tests/test_lal.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Unit test for utils module
 """
 
 import pytest
 
 import numpy
 
 from astropy import units
 
 # import necessary modules
 lal = pytest.importorskip('lal')
-utils_lal = pytest.importorskip('pdpy.utils.lal')
+utils_lal = pytest.importorskip('pydischarge.utils.lal')
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 
 def test_to_lal_type_str():
     assert utils_lal.to_lal_type_str(float) == 'REAL8'
     assert utils_lal.to_lal_type_str(
```

### Comparing `pydischarge-0.0.1/pdpy/utils/tests/test_misc.py` & `pydischarge-0.0.2/pydischarge/utils/tests/test_misc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,90 +1,90 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.utils.misc`
+"""Tests for :mod:`pydischarge.utils.misc`
 """
 
 import sys
 
 import pytest
 
 from .. import misc as utils_misc
 
 
 def test_gprint(capsys):
-    """Test for :func:`pdpy.utils.misc.gprint`
+    """Test for :func:`pydischarge.utils.misc.gprint`
     """
     utils_misc.gprint('test')
     assert capsys.readouterr().out == 'test\n'
     utils_misc.gprint('test', end=' ')
     assert capsys.readouterr().out == 'test '
     utils_misc.gprint('test', end='x', file=sys.stderr)
     cap = capsys.readouterr()
     assert not cap.out
     assert cap.err == 'testx'
 
 
 def test_null_context():
-    """Test for :func:`pdpy.utils.misc.null_context`
+    """Test for :func:`pydischarge.utils.misc.null_context`
     """
     with pytest.warns(DeprecationWarning):
         ctx = utils_misc.null_context()
     with ctx:
         print('this should work')
 
 
 def test_round_to_power():
-    """Test for :func:`pdpy.utils.misc.round_to_power`
+    """Test for :func:`pydischarge.utils.misc.round_to_power`
     """
     # test basic features
     assert utils_misc.round_to_power(2) == 2
     assert utils_misc.round_to_power(9, base=10) == 10
     assert utils_misc.round_to_power(5, which='lower') == 4
     assert utils_misc.round_to_power(5, which='upper') == 8
     # test output
     base = 10.
     rounded = utils_misc.round_to_power(9, base=base)
     assert base == rounded
     assert type(base) == type(rounded)
 
 
 def test_round_to_power_error():
-    """Test for an errored use case of :func:`pdpy.utils.misc.round_to_power`
+    """Test for an errored use case of :func:`pydischarge.utils.misc.round_to_power`
     """
     with pytest.raises(
         ValueError,
         match="^'which' argument must be one of 'lower', 'upper', or None$",
     ):
         utils_misc.round_to_power(7, which='')
 
 
 def test_unique():
-    """Test for :func:`pdpy.utils.misc.unique`
+    """Test for :func:`pydischarge.utils.misc.unique`
     """
     a = [1, 2, 4, 3, 5, 4, 5, 3]
     assert utils_misc.unique(a) == [1, 2, 4, 3, 5]
 
 
 @pytest.mark.parametrize('func, value, out', [
     (str, None, None),
     (str, 1, '1'),
 ])
 def test_if_not_none(func, value, out):
-    """Test for :func:`pdpy.utils.misc.if_not_none`
+    """Test for :func:`pydischarge.utils.misc.if_not_none`
     """
     assert utils_misc.if_not_none(func, value) == out
```

### Comparing `pydischarge-0.0.1/pdpy/utils/tests/test_mp.py` & `pydischarge-0.0.2/pydischarge/utils/tests/test_mp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Unit test for utils module
 """
 
 from math import sqrt
 
 import pytest
```

### Comparing `pydischarge-0.0.1/pdpy/utils/tests/test_shell.py` & `pydischarge-0.0.2/pydischarge/utils/tests/test_shell.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Duncan Macleod (2014-2020)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
 """Unit test for utils module
 """
 
 import platform
 import subprocess
 import sys
@@ -70,8 +70,8 @@
     assert rec[1].category is UserWarning
 
 
 def test_which():
     with pytest.warns(DeprecationWarning):
         assert shell.which('python') == find_executable('python')
     with pytest.raises(ValueError), pytest.warns(DeprecationWarning):
-        shell.which('pdpy-no-executable')
+        shell.which('pydischarge-no-executable')
```

### Comparing `pydischarge-0.0.1/pdpy/utils/tests/test_sphinx_ex2rst.py` & `pydischarge-0.0.2/pydischarge/utils/tests/test_sphinx_ex2rst.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Cardiff University (2021)
 #
-# This file is part of PDpy.
+# This file is part of pyDischarge.
 #
-# PDpy is free software: you can redistribute it and/or modify
+# pyDischarge is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PDpy is distributed in the hope that it will be useful,
+# pyDischarge is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PDpy.  If not, see <http://www.gnu.org/licenses/>.
+# along with pyDischarge.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`pdpy.utils.sphinx.ex2rst`
+"""Tests for :mod:`pydischarge.utils.sphinx.ex2rst`
 """
 
 import pytest
 
 from ..sphinx import ex2rst
 
 EXAMPLE = """
@@ -29,50 +29,50 @@
 \"\"\"Example example
 
 Something something something
 \"\"\"
 
 __author__ = "Duncan Macleod"
 __credits__ = "Someone else"  # ignored
-__currentmodule__ = "pdpy.timeseries"
+__currentmodule__ = "pydischarge.timeseries"
 
 # This is an example:
-from pdpy.timeseries import TimeSeries
+from pydischarge.timeseries import TimeSeries
 
 # and then we do this:
 a = TimeSeries(12345)
 plot = a.plot()
 plot.show()
 
 # and then something else
 b = TimeSeries(67890)
 
 # tada!
 """
 
 EXAMPLE_OUTPUT = """
-.. _pdpy-example-test_ex2rst0-example:
+.. _pydischarge-example-test_ex2rst0-example:
 
 .. sectionauthor:: Duncan Macleod
 
-.. currentmodule:: pdpy.timeseries
+.. currentmodule:: pydischarge.timeseries
 
 Example example
 ###############
 
 Something something something
 
 This is an example:
 
 .. plot::
    :context: reset
    :nofigs:
    :include-source:
 
-   from pdpy.timeseries import TimeSeries
+   from pydischarge.timeseries import TimeSeries
 
 and then we do this:
 
 .. plot::
    :context:
    :include-source:
```

### Comparing `pydischarge-0.0.1/pydischarge.egg-info/requires.txt` & `pydischarge-0.0.2/pydischarge.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.1/pyproject.toml` & `pydischarge-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -102,43 +102,43 @@
 conda = [
   "python-framel >=8.40.1",
   "python-ldas-tools-framecpp ; sys_platform != 'win32'",
   "python-nds2-client",
 ]
 
 [project.scripts]
-pdpy-plot = "pdpy.cli.pdpy_plot:main"
+pydischarge-plot = "pydischarge.cli.pydischarge_plot:main"
 
 [project.urls]
-"Bug Tracker" = "https://github.com/pdpy-github/pdpy/issues"
-"Discussion Forum" = "https://pdpy.slack.com"
-"Documentation" = "https://pdpy.github.io/docs/"
-"Source Code" = "https://github.com/pdpy-github/pdpy"
+"Bug Tracker" = "https://github.com/pydischarge-github/pydischarge/issues"
+"Discussion Forum" = "https://pydischarge.slack.com"
+"Documentation" = "https://pydischarge.github.io/docs/"
+"Source Code" = "https://github.com/pydischarge-github/pydischarge"
 
 [tool.setuptools]
 license-files = [ "LICENSE" ]
 
 [tool.setuptools.packages.find]
 # note: this is only required in CI, which otherwise fails because
 #       GHA is creating a temporary directory that setuptools
 #       discovers as another top-level package
 include = [
-  "pdpy*",
+  "pydischarge*",
 ]
 
 [tool.setuptools_scm]
-write_to = "pdpy/_version.py"
+write_to = "pydischarge/_version.py"
 
 # -- coverage.py
 
 [tool.coverage.run]
-source = [ "pdpy" ]
+source = [ "pydischarge" ]
 omit = [
   # ignore vendored sphinx extension
-  "pdpy/utils/sphinx/epydoc.py",
+  "pydischarge/utils/sphinx/epydoc.py",
   # don't report coverage for _version.py
   # (generated automatically by setuptools-scm)
   "*/_version.py",
 ]
 
 [tool.coverage.report]
 # print report with one decimal point
```
