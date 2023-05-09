# Comparing `tmp/jaxip-0.5.7.tar.gz` & `tmp/jaxip-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxip-0.5.7.tar", last modified: Mon May  8 16:52:51 2023, max compression
+gzip compressed data, was "jaxip-0.5.8.tar", last modified: Tue May  9 21:10:40 2023, max compression
```

## Comparing `jaxip-0.5.7.tar` & `jaxip-0.5.8.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.187937 jaxip-0.5.7/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.5.7/AUTHORS.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.5.7/CONTRIBUTING.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)      569 2023-03-02 17:04:49.000000 jaxip-0.5.7/HISTORY.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.5.7/LICENSE
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.5.7/MANIFEST.in
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5342 2023-05-08 16:52:51.187937 jaxip-0.5.7/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4755 2023-05-08 16:51:03.000000 jaxip-0.5.7/README.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.163937 jaxip-0.5.7/docs/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.5.7/docs/Makefile
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.155937 jaxip-0.5.7/docs/_build/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.155937 jaxip-0.5.7/docs/_build/doctrees/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.163937 jaxip-0.5.7/docs/_build/doctrees/nbsphinx/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    15512 2023-05-08 16:43:13.000000 jaxip-0.5.7/docs/_build/doctrees/nbsphinx/notebooks_potential_training_29_21.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-08 16:43:14.000000 jaxip-0.5.7/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-08 16:43:14.000000 jaxip-0.5.7/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-08 16:43:14.000000 jaxip-0.5.7/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.155937 jaxip-0.5.7/docs/_build/html/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.167937 jaxip-0.5.7/docs/_build/html/_images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    15512 2023-05-08 16:43:13.000000 jaxip-0.5.7/docs/_build/html/_images/notebooks_potential_training_29_21.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-08 16:43:14.000000 jaxip-0.5.7/docs/_build/html/_images/notebooks_tutorials_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-08 16:43:14.000000 jaxip-0.5.7/docs/_build/html/_images/notebooks_tutorials_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-08 16:43:14.000000 jaxip-0.5.7/docs/_build/html/_images/notebooks_tutorials_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.167937 jaxip-0.5.7/docs/_build/html/_static/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.5.7/docs/_build/html/_static/file.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.7/docs/_build/html/_static/minus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.7/docs/_build/html/_static/plus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.5.7/docs/authors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6406 2023-05-01 12:49:56.000000 jaxip-0.5.7/docs/conf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.5.7/docs/contributing.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       81 2023-05-01 12:51:50.000000 jaxip-0.5.7/docs/examples.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.5.7/docs/history.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.167937 jaxip-0.5.7/docs/images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.5.7/docs/images/flowchart.drawio.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.5.7/docs/images/water.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      315 2023-05-06 13:11:44.000000 jaxip-0.5.7/docs/index.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.5.7/docs/installation.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-05-08 16:43:07.000000 jaxip-0.5.7/docs/jaxip.atoms.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      507 2023-05-08 16:51:03.000000 jaxip-0.5.7/docs/jaxip.datasets.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-05-08 16:43:07.000000 jaxip-0.5.7/docs/jaxip.descriptors.acsf.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      595 2023-05-08 16:43:07.000000 jaxip-0.5.7/docs/jaxip.descriptors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-05-08 16:51:03.000000 jaxip-0.5.7/docs/jaxip.models.nn.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      234 2023-05-08 16:51:03.000000 jaxip-0.5.7/docs/jaxip.models.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1129 2023-05-08 16:43:07.000000 jaxip-0.5.7/docs/jaxip.potentials.nnp.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      464 2023-05-08 16:51:03.000000 jaxip-0.5.7/docs/jaxip.potentials.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      935 2023-05-08 16:43:07.000000 jaxip-0.5.7/docs/jaxip.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-05-08 16:43:07.000000 jaxip-0.5.7/docs/jaxip.utils.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.5.7/docs/make.bat
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-05-08 16:43:07.000000 jaxip-0.5.7/docs/modules.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.5.7/docs/readme.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-06 13:11:44.000000 jaxip-0.5.7/docs/theory.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.5.7/docs/usage.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.171937 jaxip-0.5.7/jaxip/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      575 2023-05-06 13:11:44.000000 jaxip-0.5.7/jaxip/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/_version.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.175937 jaxip-0.5.7/jaxip/atoms/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      174 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/atoms/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      355 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/atoms/_box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      779 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/atoms/_neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1342 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/atoms/_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3593 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/atoms/box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5034 2023-05-01 06:50:37.000000 jaxip-0.5.7/jaxip/atoms/element.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2865 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/atoms/neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    16306 2023-05-06 13:11:44.000000 jaxip-0.5.7/jaxip/atoms/structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2589 2023-02-08 21:09:37.000000 jaxip-0.5.7/jaxip/base.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1131 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/config.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.175937 jaxip-0.5.7/jaxip/datasets/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      154 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/datasets/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6668 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/datasets/runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1021 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/datasets/transformer.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.175937 jaxip-0.5.7/jaxip/descriptors/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/descriptors/__init__.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.175937 jaxip-0.5.7/jaxip/descriptors/acsf/
--rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.5.7/jaxip/descriptors/acsf/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5275 2023-05-06 13:11:44.000000 jaxip-0.5.7/jaxip/descriptors/acsf/_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7581 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/descriptors/acsf/acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2226 2023-03-23 20:22:06.000000 jaxip-0.5.7/jaxip/descriptors/acsf/angular.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2874 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/descriptors/acsf/cutoff.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1352 2023-03-23 20:22:06.000000 jaxip-0.5.7/jaxip/descriptors/acsf/radial.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1011 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/descriptors/acsf/symmetry.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      765 2023-05-01 09:07:44.000000 jaxip-0.5.7/jaxip/descriptors/base.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7476 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/descriptors/scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/logger.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.175937 jaxip-0.5.7/jaxip/models/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       88 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/models/__init__.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.179937 jaxip-0.5.7/jaxip/models/nn/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      181 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/models/nn/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/models/nn/activation.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/models/nn/initializer.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2849 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/models/nn/network.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.179937 jaxip-0.5.7/jaxip/potentials/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      196 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/potentials/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1949 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/potentials/_energy.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/potentials/_force.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1807 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/potentials/atomic_potential.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.179937 jaxip-0.5.7/jaxip/potentials/nnp/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      196 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/potentials/nnp/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9589 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/potentials/nnp/gradient_descent.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9747 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/potentials/nnp/kalman_filter.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/potentials/nnp/metrics.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    19255 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/potentials/nnp/potential.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11326 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/potentials/nnp/settings.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      643 2023-05-07 09:13:07.000000 jaxip-0.5.7/jaxip/types.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)      200 2023-01-05 20:40:22.000000 jaxip-0.5.7/jaxip/units.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.183937 jaxip-0.5.7/jaxip/utils/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/utils/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1427 2023-02-18 20:52:11.000000 jaxip-0.5.7/jaxip/utils/attribute.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/utils/batch.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2008 2023-03-23 20:22:06.000000 jaxip-0.5.7/jaxip/utils/compare.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/utils/profiler.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.5.7/jaxip/utils/tokenize.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.171937 jaxip-0.5.7/jaxip.egg-info/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5342 2023-05-08 16:52:51.000000 jaxip-0.5.7/jaxip.egg-info/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3140 2023-05-08 16:52:51.000000 jaxip-0.5.7/jaxip.egg-info/SOURCES.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-08 16:52:51.000000 jaxip-0.5.7/jaxip.egg-info/dependency_links.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-05-08 16:52:51.000000 jaxip-0.5.7/jaxip.egg-info/entry_points.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-08 16:52:51.000000 jaxip-0.5.7/jaxip.egg-info/not-zip-safe
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-05-08 16:52:51.000000 jaxip-0.5.7/jaxip.egg-info/requires.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-05-08 16:52:51.000000 jaxip-0.5.7/jaxip.egg-info/top_level.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-05-08 16:52:51.187937 jaxip-0.5.7/setup.cfg
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.5.7/setup.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.183937 jaxip-0.5.7/tests/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.183937 jaxip-0.5.7/tests/.ipynb_checkpoints/
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.7/tests/.ipynb_checkpoints/h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.5.7/tests/.ipynb_checkpoints/h2o-checkpoint.json
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.5.7/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.5.7/tests/.ipynb_checkpoints/test-checkpoint.ipynb
--rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.5.7/tests/__init__.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.7/tests/h2o.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.5.7/tests/h2o.json
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-05-08 16:42:40.000000 jaxip-0.5.7/tests/scaling.001.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-05-08 16:42:40.000000 jaxip-0.5.7/tests/scaling.008.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5117 2023-05-07 11:23:30.000000 jaxip-0.5.7/tests/test_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4116 2023-05-08 16:51:03.000000 jaxip-0.5.7/tests/test_nn.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3420 2023-05-01 12:41:07.000000 jaxip-0.5.7/tests/test_nnp.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4816 2023-05-01 12:41:07.000000 jaxip-0.5.7/tests/test_runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2859 2023-05-01 12:41:07.000000 jaxip-0.5.7/tests/test_scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4937 2023-04-24 20:54:27.000000 jaxip-0.5.7/tests/test_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-05-08 16:42:40.000000 jaxip-0.5.7/tests/weights.001.pkl
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-05-08 16:42:40.000000 jaxip-0.5.7/tests/weights.008.pkl
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.267821 jaxip-0.5.8/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.5.8/AUTHORS.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.5.8/CONTRIBUTING.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      569 2023-03-02 17:04:49.000000 jaxip-0.5.8/HISTORY.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.5.8/LICENSE
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.5.8/MANIFEST.in
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5342 2023-05-09 21:10:40.267821 jaxip-0.5.8/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4755 2023-05-08 16:51:03.000000 jaxip-0.5.8/README.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.247821 jaxip-0.5.8/docs/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.5.8/docs/Makefile
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.239821 jaxip-0.5.8/docs/_build/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.239821 jaxip-0.5.8/docs/_build/doctrees/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.247821 jaxip-0.5.8/docs/_build/doctrees/nbsphinx/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    15512 2023-05-09 20:59:51.000000 jaxip-0.5.8/docs/_build/doctrees/nbsphinx/notebooks_potential_training_30_21.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-09 20:59:52.000000 jaxip-0.5.8/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-09 20:59:52.000000 jaxip-0.5.8/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-09 20:59:52.000000 jaxip-0.5.8/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.239821 jaxip-0.5.8/docs/_build/html/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.247821 jaxip-0.5.8/docs/_build/html/_images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    15512 2023-05-09 20:58:04.000000 jaxip-0.5.8/docs/_build/html/_images/notebooks_potential_training_30_21.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-09 20:58:05.000000 jaxip-0.5.8/docs/_build/html/_images/notebooks_tutorials_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-09 20:58:05.000000 jaxip-0.5.8/docs/_build/html/_images/notebooks_tutorials_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-09 20:58:05.000000 jaxip-0.5.8/docs/_build/html/_images/notebooks_tutorials_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.251821 jaxip-0.5.8/docs/_build/html/_static/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.5.8/docs/_build/html/_static/file.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.8/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.8/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.5.8/docs/authors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6406 2023-05-01 12:49:56.000000 jaxip-0.5.8/docs/conf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.5.8/docs/contributing.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       81 2023-05-01 12:51:50.000000 jaxip-0.5.8/docs/examples.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.5.8/docs/history.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.251821 jaxip-0.5.8/docs/images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.5.8/docs/images/flowchart.drawio.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.5.8/docs/images/water.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      315 2023-05-06 13:11:44.000000 jaxip-0.5.8/docs/index.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.5.8/docs/installation.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.atoms.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      507 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.datasets.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.descriptors.acsf.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      595 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.descriptors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.models.nn.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      234 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.models.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1129 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.potentials.nnp.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      464 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.potentials.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      941 2023-05-09 21:10:18.000000 jaxip-0.5.8/docs/jaxip.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.utils.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.5.8/docs/make.bat
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/modules.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.5.8/docs/readme.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-06 13:11:44.000000 jaxip-0.5.8/docs/theory.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.5.8/docs/usage.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.251821 jaxip-0.5.8/jaxip/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      575 2023-05-06 13:11:44.000000 jaxip-0.5.8/jaxip/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/_version.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.255821 jaxip-0.5.8/jaxip/atoms/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      174 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/atoms/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      355 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/atoms/_box.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      779 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/atoms/_neighbor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1342 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/atoms/_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3724 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/atoms/box.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5034 2023-05-01 06:50:37.000000 jaxip-0.5.8/jaxip/atoms/element.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3015 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/atoms/neighbor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    16818 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/atoms/structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1131 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/config.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.255821 jaxip-0.5.8/jaxip/datasets/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      154 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/datasets/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6668 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/datasets/runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1021 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/datasets/transformer.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.259822 jaxip-0.5.8/jaxip/descriptors/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/descriptors/__init__.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.259822 jaxip-0.5.8/jaxip/descriptors/acsf/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.5.8/jaxip/descriptors/acsf/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5275 2023-05-06 13:11:44.000000 jaxip-0.5.8/jaxip/descriptors/acsf/_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7583 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/descriptors/acsf/acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2228 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/descriptors/acsf/angular.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2644 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/descriptors/acsf/cutoff.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1354 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/descriptors/acsf/radial.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1011 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/descriptors/acsf/symmetry.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      765 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/descriptors/base.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7476 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/descriptors/scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/logger.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.259822 jaxip-0.5.8/jaxip/models/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       88 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/models/__init__.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.259822 jaxip-0.5.8/jaxip/models/nn/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      181 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/models/nn/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/models/nn/activation.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/models/nn/initializer.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2849 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/models/nn/network.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.259822 jaxip-0.5.8/jaxip/potentials/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      196 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/potentials/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1949 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/potentials/_energy.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/potentials/_force.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1807 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/potentials/atomic_potential.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.263821 jaxip-0.5.8/jaxip/potentials/nnp/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      196 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/potentials/nnp/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9589 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/potentials/nnp/gradient_descent.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9747 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/potentials/nnp/kalman_filter.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/potentials/nnp/metrics.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    19255 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/potentials/nnp/potential.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11326 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/potentials/nnp/settings.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3555 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/pytree.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      643 2023-05-07 09:13:07.000000 jaxip-0.5.8/jaxip/types.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      200 2023-01-05 20:40:22.000000 jaxip-0.5.8/jaxip/units.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.263821 jaxip-0.5.8/jaxip/utils/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/utils/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1427 2023-02-18 20:52:11.000000 jaxip-0.5.8/jaxip/utils/attribute.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/utils/batch.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2008 2023-03-23 20:22:06.000000 jaxip-0.5.8/jaxip/utils/compare.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/utils/profiler.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.5.8/jaxip/utils/tokenize.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.255821 jaxip-0.5.8/jaxip.egg-info/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5342 2023-05-09 21:10:40.000000 jaxip-0.5.8/jaxip.egg-info/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3142 2023-05-09 21:10:40.000000 jaxip-0.5.8/jaxip.egg-info/SOURCES.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-09 21:10:40.000000 jaxip-0.5.8/jaxip.egg-info/dependency_links.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-05-09 21:10:40.000000 jaxip-0.5.8/jaxip.egg-info/entry_points.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-09 21:10:40.000000 jaxip-0.5.8/jaxip.egg-info/not-zip-safe
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-05-09 21:10:40.000000 jaxip-0.5.8/jaxip.egg-info/requires.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-05-09 21:10:40.000000 jaxip-0.5.8/jaxip.egg-info/top_level.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-05-09 21:10:40.267821 jaxip-0.5.8/setup.cfg
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.5.8/setup.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.267821 jaxip-0.5.8/tests/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.267821 jaxip-0.5.8/tests/.ipynb_checkpoints/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.8/tests/.ipynb_checkpoints/h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.5.8/tests/.ipynb_checkpoints/h2o-checkpoint.json
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.5.8/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.5.8/tests/.ipynb_checkpoints/test-checkpoint.ipynb
+-rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.5.8/tests/__init__.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.8/tests/h2o.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.5.8/tests/h2o.json
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-05-09 21:01:28.000000 jaxip-0.5.8/tests/scaling.001.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-05-09 21:01:28.000000 jaxip-0.5.8/tests/scaling.008.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5117 2023-05-07 11:23:30.000000 jaxip-0.5.8/tests/test_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4116 2023-05-08 16:51:03.000000 jaxip-0.5.8/tests/test_nn.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3420 2023-05-01 12:41:07.000000 jaxip-0.5.8/tests/test_nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4816 2023-05-01 12:41:07.000000 jaxip-0.5.8/tests/test_runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2859 2023-05-01 12:41:07.000000 jaxip-0.5.8/tests/test_scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4937 2023-04-24 20:54:27.000000 jaxip-0.5.8/tests/test_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-05-09 21:01:28.000000 jaxip-0.5.8/tests/weights.001.pkl
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-05-09 21:01:28.000000 jaxip-0.5.8/tests/weights.008.pkl
```

### Comparing `jaxip-0.5.7/CONTRIBUTING.rst` & `jaxip-0.5.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/HISTORY.rst` & `jaxip-0.5.8/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/LICENSE` & `jaxip-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/PKG-INFO` & `jaxip-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxip
-Version: 0.5.7
+Version: 0.5.8
 Summary: JAX-based Interatomic Potential
 Home-page: https://github.com/hghcomphys/jaxip
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: jaxip
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `jaxip-0.5.7/README.rst` & `jaxip-0.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/Makefile` & `jaxip-0.5.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/_build/doctrees/nbsphinx/notebooks_potential_training_29_21.png` & `jaxip-0.5.8/docs/_build/doctrees/nbsphinx/notebooks_potential_training_30_21.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png` & `jaxip-0.5.8/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png` & `jaxip-0.5.8/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png` & `jaxip-0.5.8/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/_build/html/_images/notebooks_potential_training_29_21.png` & `jaxip-0.5.8/docs/_build/html/_images/notebooks_potential_training_30_21.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/_build/html/_images/notebooks_tutorials_38_0.png` & `jaxip-0.5.8/docs/_build/html/_images/notebooks_tutorials_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/_build/html/_images/notebooks_tutorials_45_0.png` & `jaxip-0.5.8/docs/_build/html/_images/notebooks_tutorials_45_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/_build/html/_images/notebooks_tutorials_51_0.png` & `jaxip-0.5.8/docs/_build/html/_images/notebooks_tutorials_51_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/conf.py` & `jaxip-0.5.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/images/flowchart.drawio.png` & `jaxip-0.5.8/docs/images/flowchart.drawio.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/images/water.png` & `jaxip-0.5.8/docs/images/water.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/installation.rst` & `jaxip-0.5.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/jaxip.atoms.rst` & `jaxip-0.5.8/docs/jaxip.atoms.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/jaxip.descriptors.acsf.rst` & `jaxip-0.5.8/docs/jaxip.descriptors.acsf.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/jaxip.descriptors.rst` & `jaxip-0.5.8/docs/jaxip.descriptors.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/jaxip.models.nn.rst` & `jaxip-0.5.8/docs/jaxip.models.nn.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/jaxip.potentials.nnp.rst` & `jaxip-0.5.8/docs/jaxip.potentials.nnp.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/jaxip.rst` & `jaxip-0.5.8/docs/jaxip.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,34 +13,34 @@
    jaxip.models
    jaxip.potentials
    jaxip.utils
 
 Submodules
 ----------
 
-jaxip.base module
------------------
+jaxip.config module
+-------------------
 
-.. automodule:: jaxip.base
+.. automodule:: jaxip.config
    :members:
    :undoc-members:
    :show-inheritance:
 
-jaxip.config module
+jaxip.logger module
 -------------------
 
-.. automodule:: jaxip.config
+.. automodule:: jaxip.logger
    :members:
    :undoc-members:
    :show-inheritance:
 
-jaxip.logger module
+jaxip.pytree module
 -------------------
 
-.. automodule:: jaxip.logger
+.. automodule:: jaxip.pytree
    :members:
    :undoc-members:
    :show-inheritance:
 
 jaxip.types module
 ------------------
```

### Comparing `jaxip-0.5.7/docs/jaxip.utils.rst` & `jaxip-0.5.8/docs/jaxip.utils.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/make.bat` & `jaxip-0.5.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/theory.rst` & `jaxip-0.5.8/docs/theory.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/docs/usage.rst` & `jaxip-0.5.8/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/__init__.py` & `jaxip-0.5.8/jaxip/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/atoms/_neighbor.py` & `jaxip-0.5.8/jaxip/atoms/_neighbor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/atoms/_structure.py` & `jaxip-0.5.8/jaxip/atoms/_structure.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/atoms/box.py` & `jaxip-0.5.8/jaxip/atoms/box.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from dataclasses import dataclass
 from typing import Optional
 
 import jax
 import jax.numpy as jnp
 
 from jaxip.atoms._box import _apply_pbc
-from jaxip.base import _BaseJaxPytreeDataClass, register_jax_pytree_node
 from jaxip.logger import logger
+from jaxip.pytree import BaseJaxPytreeDataClass, register_jax_pytree_node
 from jaxip.types import Array, Dtype
 from jaxip.types import dtype as _dtype
 
 
 @dataclass
-class Box(_BaseJaxPytreeDataClass):
+class Box(BaseJaxPytreeDataClass):
     """
     Simulation box which is responsible for applying PBCs
     when there are available lattice info.
 
     .. warning::
         Current implementation works only for orthogonal cells.
         No support for triclinic cells yet.
@@ -39,14 +39,16 @@
             except ValueError:
                 logger.error(
                     "Unexpected lattice matrix type or dimension",
                     exception=ValueError,  # type:ignore
                 )
 
         logger.debug(f"Initializing {self}")
+        self._assert_jit_dynamic_attributes(expected=("lattice",))
+        self._assert_jit_static_attributes(expected=("dtype",))
 
     def __hash__(self) -> int:
         """Enforce to use the parent class's hash method (JIT)."""
         return super().__hash__()
 
     def __bool__(self) -> bool:
         """Check whether the box instance with lattice info makes sense."""
```

### Comparing `jaxip-0.5.7/jaxip/atoms/element.py` & `jaxip-0.5.8/jaxip/atoms/element.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/atoms/neighbor.py` & `jaxip-0.5.8/jaxip/atoms/neighbor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from dataclasses import dataclass, field
 from typing import Optional
 
 import jax.numpy as jnp
 
 from jaxip.atoms._neighbor import _calculate_cutoff_mask
-from jaxip.base import _BaseJaxPytreeDataClass, register_jax_pytree_node
 from jaxip.logger import logger
+from jaxip.pytree import BaseJaxPytreeDataClass, register_jax_pytree_node
 from jaxip.types import Array
 
 
 @dataclass
-class Neighbor(_BaseJaxPytreeDataClass):
+class Neighbor(BaseJaxPytreeDataClass):
     """
     Create a neighbor list of atoms for an input structure
     and it is by design independent of `Structure`.
 
     .. note::
         For MD simulations, re-neighboring the list is required every few steps.
         This is usually implemented together with defining a skin radius.
@@ -23,14 +23,16 @@
     mask: Optional[Array] = None
     r_cutoff: Optional[float] = None
     r_cutoff_updated: bool = field(init=False, default=False)
 
     def __post_init__(self) -> None:
         """Post initialize the neighbor list."""
         logger.debug(f"Initializing {self}")
+        self._assert_jit_dynamic_attributes(expected=("mask",))
+        self._assert_jit_static_attributes(expected=('r_cutoff', 'r_cutoff_updated'))
 
     def __hash__(self) -> int:
         """Enforce to use the parent class's hash method (JIT)."""
         return super().__hash__()
 
     def set_cutoff_radius(self, r_cutoff: float) -> None:
         """
```

### Comparing `jaxip-0.5.7/jaxip/atoms/structure.py` & `jaxip-0.5.8/jaxip/atoms/structure.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from ase import Atoms as AseAtoms
 from jax import tree_util
 
 from jaxip.atoms._structure import _calculate_distance
 from jaxip.atoms.box import Box
 from jaxip.atoms.element import ElementMap
 from jaxip.atoms.neighbor import Neighbor
-from jaxip.base import _BaseJaxPytreeDataClass, register_jax_pytree_node
 from jaxip.logger import logger
+from jaxip.pytree import BaseJaxPytreeDataClass, register_jax_pytree_node
 from jaxip.types import Array, Dtype, Element
 from jaxip.types import dtype as _dtype
 from jaxip.units import units
 
 
 class Inputs(NamedTuple):
     """
@@ -31,15 +31,15 @@
     position: Array
     atype: Array
     lattice: Array
     emap: Dict[Element, Array]
 
 
 @dataclass
-class Structure(_BaseJaxPytreeDataClass):
+class Structure(BaseJaxPytreeDataClass):
     """
     A structure contains arrays of atomic attributes
     for a collection of atoms in the simulation box.
 
     Atomic attributes:
 
     * `position`: per-atom position x, y, and z
@@ -220,14 +220,33 @@
         """Get atom attributes which are basically array values."""
         return cls._get_jit_dynamic_attributes()
 
     def __post_init__(self) -> None:
         """Post initializations."""
         self.position = self.box.shift_inside_box(self.position)
         logger.debug(f"Initializing {self.__class__.__name__}()")
+        self._assert_jit_dynamic_attributes(
+            expected=(
+                "position", 
+                "force", 
+                "energy", 
+                "total_energy", 
+                "charge", 
+                "total_charge",
+                "atom_type"
+            )
+        )
+        self._assert_jit_static_attributes(
+            expected=(
+                'box', 
+                'element_map',
+                'neighbor',
+                'requires_neighbor_update',
+            )
+        )
 
     def __hash__(self) -> int:
         """Enforce to use the parent class's hash method (JIT)."""
         return super().__hash__()
 
     # --------------------------------------------------------------------------------------
```

### Comparing `jaxip-0.5.7/jaxip/config.py` & `jaxip-0.5.8/jaxip/config.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/datasets/runner.py` & `jaxip-0.5.8/jaxip/datasets/runner.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/datasets/transformer.py` & `jaxip-0.5.8/jaxip/datasets/transformer.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/descriptors/acsf/_acsf.py` & `jaxip-0.5.8/jaxip/descriptors/acsf/_acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/descriptors/acsf/acsf.py` & `jaxip-0.5.8/jaxip/descriptors/acsf/acsf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import itertools
 from dataclasses import dataclass
 from typing import Optional, Tuple
 
 import jax.numpy as jnp
 
 from jaxip.atoms.structure import Structure
-from jaxip.base import register_jax_pytree_node
 from jaxip.descriptors.acsf._acsf import (
     _calculate_descriptor,
     _calculate_grad_descriptor_per_atom,
 )
 from jaxip.descriptors.acsf.angular import AngularSymmetryFunction
 from jaxip.descriptors.acsf.radial import RadialSymmetryFunction
 from jaxip.descriptors.acsf.symmetry import EnvironmentElements, SymmetryFunction
 from jaxip.descriptors.base import Descriptor
 from jaxip.logger import logger
+from jaxip.pytree import register_jax_pytree_node
 from jaxip.types import Array, Element
 
 
 @dataclass
 class ACSF(Descriptor):
     """
     Atom-centered Symmetry Function (`ACSF`_) descriptor.
```

### Comparing `jaxip-0.5.7/jaxip/descriptors/acsf/angular.py` & `jaxip-0.5.8/jaxip/descriptors/acsf/angular.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 
 import jax
 import jax.numpy as jnp
 
-from jaxip.base import register_jax_pytree_node
 from jaxip.descriptors.acsf.cutoff import CutoffFunction
 from jaxip.descriptors.acsf.symmetry import SymmetryFunction
+from jaxip.pytree import register_jax_pytree_node
 from jaxip.types import Array
 
 
 class AngularSymmetryFunction(SymmetryFunction, metaclass=ABCMeta):
     """A base class for `three body` (angular) symmetry functions."""
 
     def __hash__(self) -> int:
```

### Comparing `jaxip-0.5.7/jaxip/descriptors/acsf/cutoff.py` & `jaxip-0.5.8/jaxip/descriptors/acsf/cutoff.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import math
 from dataclasses import dataclass
 from typing import Callable, Optional
 
 import jax
 import jax.numpy as jnp
 
-from jaxip.base import _BaseJaxPytreeDataClass, register_jax_pytree_node
 from jaxip.logger import logger
+from jaxip.pytree import BaseJaxPytreeDataClass, register_jax_pytree_node
 from jaxip.types import Array
 
 _TANH_PRE: float = ((math.e + 1 / math.e) / (math.e - 1 / math.e)) ** 3
 
 
 @dataclass
-class CutoffFunction(_BaseJaxPytreeDataClass):
+class CutoffFunction(BaseJaxPytreeDataClass):
     """Cutoff function for ACSF descriptor.
 
     See `cutoff function`_ and `cutoff type`_ for more details.
 
     .. _`cutoff function`: https://compphysvienna.github.io/n2p2/api/cutoff_functions.html?highlight=cutoff#
     .. _`cutoff type`: https://compphysvienna.github.io/n2p2/topics/keywords.html?highlight=cutoff_type
     """
@@ -33,23 +33,17 @@
             try:
                 self.cutoff_function = getattr(self, f"{self.cutoff_type}")
             except AttributeError:
                 logger.error(
                     f"'{self.__class__.__name__}' has no cutoff function '{self.cutoff_type}'",
                     exception=NotImplementedError,
                 )
-        self._check_jit_attributes()
-
-    @classmethod
-    def _check_jit_attributes(cls) -> None:
-        """An optional check to ensure jit static and dynamics attributes are correctly identified."""
-        assert cls._get_jit_dynamic_attributes() == tuple()
-        assert (
-            cls._get_jit_static_attributes() == \
-            ('r_cutoff', 'cutoff_type', 'cutoff_function')
+        self._assert_jit_dynamic_attributes()
+        self._assert_jit_static_attributes(
+            expected=('r_cutoff', 'cutoff_type', 'cutoff_function')
         )
 
     def __hash__(self) -> int:
         """Enforce to use the parent class's hash method (JIT)."""
         return super().__hash__()
 
     @jax.jit
```

### Comparing `jaxip-0.5.7/jaxip/descriptors/acsf/radial.py` & `jaxip-0.5.8/jaxip/descriptors/acsf/radial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 
 import jax
 import jax.numpy as jnp
 
-from jaxip.base import register_jax_pytree_node
 from jaxip.descriptors.acsf.cutoff import CutoffFunction
 from jaxip.descriptors.acsf.symmetry import SymmetryFunction
+from jaxip.pytree import register_jax_pytree_node
 from jaxip.types import Array
 
 
 class RadialSymmetryFunction(SymmetryFunction, metaclass=ABCMeta):
     """A base class for `two body` (radial) symmetry functions."""
 
     @abstractmethod
```

### Comparing `jaxip-0.5.7/jaxip/descriptors/acsf/symmetry.py` & `jaxip-0.5.8/jaxip/descriptors/acsf/symmetry.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from abc import ABCMeta, abstractmethod
 from typing import NamedTuple, Optional
 
-from jaxip.base import _BaseJaxPytreeDataClass
 from jaxip.descriptors.acsf.cutoff import CutoffFunction
 from jaxip.logger import logger
+from jaxip.pytree import BaseJaxPytreeDataClass
 from jaxip.types import Array, Element
 
 
-class SymmetryFunction(_BaseJaxPytreeDataClass, metaclass=ABCMeta):
+class SymmetryFunction(BaseJaxPytreeDataClass, metaclass=ABCMeta):
     """
     A base class for symmetry functions.
     All symmetry functions (i.e. radial and angular) must derive from this base class.
     """
 
     def __init__(self, cfn: CutoffFunction) -> None:
         self.cfn: CutoffFunction = cfn
```

### Comparing `jaxip-0.5.7/jaxip/descriptors/base.py` & `jaxip-0.5.8/jaxip/descriptors/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABCMeta, abstractmethod
 
-from jaxip.base import _BaseJaxPytreeDataClass
+from jaxip.pytree import BaseJaxPytreeDataClass
 from jaxip.types import Array
 
 
-class Descriptor(_BaseJaxPytreeDataClass, metaclass=ABCMeta):
+class Descriptor(BaseJaxPytreeDataClass, metaclass=ABCMeta):
     """A base class for atomic environment descriptors."""
 
     @abstractmethod
     def add(self, *args, **kwargs) -> None:
         ...
 
     @abstractmethod
```

### Comparing `jaxip-0.5.7/jaxip/descriptors/scaler.py` & `jaxip-0.5.8/jaxip/descriptors/scaler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/logger.py` & `jaxip-0.5.8/jaxip/logger.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/models/nn/activation.py` & `jaxip-0.5.8/jaxip/models/nn/activation.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/models/nn/initializer.py` & `jaxip-0.5.8/jaxip/models/nn/initializer.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/models/nn/network.py` & `jaxip-0.5.8/jaxip/models/nn/network.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/potentials/_energy.py` & `jaxip-0.5.8/jaxip/potentials/_energy.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/potentials/_force.py` & `jaxip-0.5.8/jaxip/potentials/_force.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/potentials/atomic_potential.py` & `jaxip-0.5.8/jaxip/potentials/atomic_potential.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/potentials/nnp/gradient_descent.py` & `jaxip-0.5.8/jaxip/potentials/nnp/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/potentials/nnp/kalman_filter.py` & `jaxip-0.5.8/jaxip/potentials/nnp/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/potentials/nnp/metrics.py` & `jaxip-0.5.8/jaxip/potentials/nnp/metrics.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/potentials/nnp/potential.py` & `jaxip-0.5.8/jaxip/potentials/nnp/potential.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/potentials/nnp/settings.py` & `jaxip-0.5.8/jaxip/potentials/nnp/settings.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/types.py` & `jaxip-0.5.8/jaxip/types.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/utils/attribute.py` & `jaxip-0.5.8/jaxip/utils/attribute.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/utils/batch.py` & `jaxip-0.5.8/jaxip/utils/batch.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/utils/compare.py` & `jaxip-0.5.8/jaxip/utils/compare.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/utils/profiler.py` & `jaxip-0.5.8/jaxip/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip/utils/tokenize.py` & `jaxip-0.5.8/jaxip/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/jaxip.egg-info/PKG-INFO` & `jaxip-0.5.8/jaxip.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxip
-Version: 0.5.7
+Version: 0.5.8
 Summary: JAX-based Interatomic Potential
 Home-page: https://github.com/hghcomphys/jaxip
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: jaxip
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `jaxip-0.5.7/jaxip.egg-info/SOURCES.txt` & `jaxip-0.5.8/jaxip.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -25,32 +25,32 @@
 docs/jaxip.rst
 docs/jaxip.utils.rst
 docs/make.bat
 docs/modules.rst
 docs/readme.rst
 docs/theory.rst
 docs/usage.rst
-docs/_build/doctrees/nbsphinx/notebooks_potential_training_29_21.png
+docs/_build/doctrees/nbsphinx/notebooks_potential_training_30_21.png
 docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
 docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
 docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
-docs/_build/html/_images/notebooks_potential_training_29_21.png
+docs/_build/html/_images/notebooks_potential_training_30_21.png
 docs/_build/html/_images/notebooks_tutorials_38_0.png
 docs/_build/html/_images/notebooks_tutorials_45_0.png
 docs/_build/html/_images/notebooks_tutorials_51_0.png
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
 docs/images/flowchart.drawio.png
 docs/images/water.png
 jaxip/__init__.py
 jaxip/_version.py
-jaxip/base.py
 jaxip/config.py
 jaxip/logger.py
+jaxip/pytree.py
 jaxip/types.py
 jaxip/units.py
 jaxip.egg-info/PKG-INFO
 jaxip.egg-info/SOURCES.txt
 jaxip.egg-info/dependency_links.txt
 jaxip.egg-info/entry_points.txt
 jaxip.egg-info/not-zip-safe
```

### Comparing `jaxip-0.5.7/setup.py` & `jaxip-0.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/tests/.ipynb_checkpoints/h2o-checkpoint.data` & `jaxip-0.5.8/tests/.ipynb_checkpoints/h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/tests/.ipynb_checkpoints/h2o-checkpoint.json` & `jaxip-0.5.8/tests/.ipynb_checkpoints/h2o-checkpoint.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/tests/.ipynb_checkpoints/input.h2o-checkpoint.data` & `jaxip-0.5.8/tests/.ipynb_checkpoints/input.h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/tests/.ipynb_checkpoints/test-checkpoint.ipynb` & `jaxip-0.5.8/tests/.ipynb_checkpoints/test-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/tests/h2o.data` & `jaxip-0.5.8/tests/h2o.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/tests/h2o.json` & `jaxip-0.5.8/tests/h2o.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/tests/test_acsf.py` & `jaxip-0.5.8/tests/test_acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/tests/test_nn.py` & `jaxip-0.5.8/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/tests/test_nnp.py` & `jaxip-0.5.8/tests/test_nnp.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/tests/test_runner.py` & `jaxip-0.5.8/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/tests/test_scaler.py` & `jaxip-0.5.8/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/tests/test_structure.py` & `jaxip-0.5.8/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/tests/weights.001.pkl` & `jaxip-0.5.8/tests/weights.001.pkl`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.7/tests/weights.008.pkl` & `jaxip-0.5.8/tests/weights.008.pkl`

 * *Files identical despite different names*

