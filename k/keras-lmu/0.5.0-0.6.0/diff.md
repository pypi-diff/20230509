# Comparing `tmp/keras-lmu-0.5.0.tar.gz` & `tmp/keras-lmu-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-lmu-0.5.0.tar", last modified: Fri Jan 27 00:11:34 2023, max compression
+gzip compressed data, was "keras-lmu-0.6.0.tar", last modified: Tue May  9 15:13:55 2023, max compression
```

## Comparing `keras-lmu-0.5.0.tar` & `keras-lmu-0.6.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:11:34.795879 keras-lmu-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/.nengobones.yml
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/CONTRIBUTORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-01-27 00:11:34.795879 keras-lmu-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:11:34.791879 keras-lmu-0.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:11:34.791879 keras-lmu-0.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/docs/api-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/docs/basic-usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:11:34.795879 keras-lmu-0.5.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/docs/examples/psMNIST-training.png
--rw-r--r--   0 runner    (1001) docker     (123)  1252848 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/docs/examples/psMNIST-weights.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/docs/examples/psMNIST.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/docs/project.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:11:34.795879 keras-lmu-0.5.0/keras_lmu/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/keras_lmu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41170 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/keras_lmu/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:11:34.795879 keras-lmu-0.5.0/keras_lmu/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/keras_lmu/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/keras_lmu/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/keras_lmu/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)    23455 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/keras_lmu/tests/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/keras_lmu/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:11:34.795879 keras-lmu-0.5.0/keras_lmu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-01-27 00:11:34.000000 keras-lmu-0.5.0/keras_lmu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-01-27 00:11:34.000000 keras-lmu-0.5.0/keras_lmu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 00:11:34.000000 keras-lmu-0.5.0/keras_lmu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 00:10:37.000000 keras-lmu-0.5.0/keras_lmu.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-01-27 00:11:34.000000 keras-lmu-0.5.0/keras_lmu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-27 00:11:34.000000 keras-lmu-0.5.0/keras_lmu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-01-27 00:11:34.811879 keras-lmu-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-01-27 00:09:49.000000 keras-lmu-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:13:55.288609 keras-lmu-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/.nengobones.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/CONTRIBUTORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-05-09 15:13:55.288609 keras-lmu-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:13:55.284609 keras-lmu-0.6.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:13:55.284609 keras-lmu-0.6.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/api-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/basic-usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:13:55.284609 keras-lmu-0.6.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/examples/psMNIST-training.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1252848 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/examples/psMNIST-weights.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    14224 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/examples/psMNIST.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/project.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:13:55.284609 keras-lmu-0.6.0/keras_lmu/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/keras_lmu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42115 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/keras_lmu/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:13:55.288609 keras-lmu-0.6.0/keras_lmu/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/keras_lmu/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/keras_lmu/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/keras_lmu/tests/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24043 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/keras_lmu/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/keras_lmu/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:13:55.284609 keras-lmu-0.6.0/keras_lmu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-05-09 15:13:55.000000 keras-lmu-0.6.0/keras_lmu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-09 15:13:55.000000 keras-lmu-0.6.0/keras_lmu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:13:55.000000 keras-lmu-0.6.0/keras_lmu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:12:45.000000 keras-lmu-0.6.0/keras_lmu.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-09 15:13:55.000000 keras-lmu-0.6.0/keras_lmu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 15:13:55.000000 keras-lmu-0.6.0/keras_lmu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-09 15:13:55.288609 keras-lmu-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/setup.py
```

### Comparing `keras-lmu-0.5.0/.nengobones.yml` & `keras-lmu-0.6.0/.nengobones.yml`

 * *Files 8% similar despite different names*

```diff
@@ -77,37 +77,37 @@
     azure_name: nengo-dl
     azure_group: nengo-ci
     coverage: true
     remote_vars:
       TF_FORCE_GPU_ALLOW_GROWTH: "true"
       TF_VERSION: $TF_VERSION
     remote_setup:
-      - micromamba install -y "$TF_VERSION"
+      - micromamba install -y "$TF_VERSION" cudnn=8.4
   - template: remote-script
     remote_script: docs
     output_name: remote-docs
     host: azure-docs
     azure_name: nengo-dl-docs
     azure_group: nengo-ci
     remote_setup:
-      - micromamba install -y "$TF_VERSION"
+      - micromamba install -y "$TF_VERSION" cudnn=8.4
   - template: remote-script
     remote_script: examples
     output_name: remote-examples
     host: azure-examples
     azure_name: nengo-dl-examples
     azure_group: nengo-ci
     remote_setup:
-      - micromamba install -y "$TF_VERSION"
+      - micromamba install -y "$TF_VERSION" cudnn=8.4
   - template: deploy
     wheel: true
 
 pre_commit_config_yaml: {}
 
 pyproject_toml: {}
 
 version_py:
   type: semver
   major: 0
-  minor: 5
+  minor: 6
   patch: 0
-  release: true
+  release: True
```

### Comparing `keras-lmu-0.5.0/CHANGES.rst` & `keras-lmu-0.6.0/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,35 @@
 
    - Added
    - Changed
    - Deprecated
    - Removed
    - Fixed
 
+0.6.0 (May 5, 2023)
+===================
+
+*Compatible with TensorFlow 2.4 - 2.11*
+
+**Changed**
+
+- ``LMUFeedforward`` can now be used with unknown sequence lengths, and ``LMU`` will
+  use ``LMUFeedforward`` for unknown sequence lengths (as long as the other conditions
+  are met, as before). (`#52`_)
+- Allow ``input_to_hidden=True`` with ``hidden_cell=None``. This will act as a skip
+  connection. (`#52`_)
+- Changed order of LMU states so that the LMU memory state always comes first, and
+  any states from the hidden cell come afterwards. (`#52`_)
+
+**Fixed**
+
+- Fixed errors when setting non-default dtype on LMU layers. (`#52`_)
+
+.. _#52: https://github.com/nengo/keras-lmu/pull/52
+
 0.5.0 (January 26, 2023)
 ========================
 
 *Compatible with TensorFlow 2.4 - 2.11*
 
 **Added**
```

### Comparing `keras-lmu-0.5.0/CONTRIBUTING.rst` & `keras-lmu-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.5.0/LICENSE.rst` & `keras-lmu-0.6.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.5.0/MANIFEST.in` & `keras-lmu-0.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.5.0/PKG-INFO` & `keras-lmu-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-lmu
-Version: 0.5.0
+Version: 0.6.0
 Summary: Keras implementation of Legendre Memory Units
 Home-page: https://www.nengo.ai/keras-lmu
 Author: Applied Brain Research
 Author-email: info@appliedbrainresearch.com
 License: Free for non-commercial use
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -114,14 +114,35 @@
 
    - Added
    - Changed
    - Deprecated
    - Removed
    - Fixed
 
+0.6.0 (May 5, 2023)
+===================
+
+*Compatible with TensorFlow 2.4 - 2.11*
+
+**Changed**
+
+- ``LMUFeedforward`` can now be used with unknown sequence lengths, and ``LMU`` will
+  use ``LMUFeedforward`` for unknown sequence lengths (as long as the other conditions
+  are met, as before). (`#52`_)
+- Allow ``input_to_hidden=True`` with ``hidden_cell=None``. This will act as a skip
+  connection. (`#52`_)
+- Changed order of LMU states so that the LMU memory state always comes first, and
+  any states from the hidden cell come afterwards. (`#52`_)
+
+**Fixed**
+
+- Fixed errors when setting non-default dtype on LMU layers. (`#52`_)
+
+.. _#52: https://github.com/nengo/keras-lmu/pull/52
+
 0.5.0 (January 26, 2023)
 ========================
 
 *Compatible with TensorFlow 2.4 - 2.11*
 
 **Added**
```

### Comparing `keras-lmu-0.5.0/README.rst` & `keras-lmu-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.5.0/docs/_static/favicon.ico` & `keras-lmu-0.6.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.5.0/docs/basic-usage.rst` & `keras-lmu-0.6.0/docs/basic-usage.rst`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.5.0/docs/citation.rst` & `keras-lmu-0.6.0/docs/citation.rst`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.5.0/docs/examples/psMNIST-training.png` & `keras-lmu-0.6.0/docs/examples/psMNIST-training.png`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.5.0/docs/examples/psMNIST-weights.hdf5` & `keras-lmu-0.6.0/docs/examples/psMNIST-weights.hdf5`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.5.0/docs/examples/psMNIST.ipynb` & `keras-lmu-0.6.0/docs/examples/psMNIST.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999787414965986%*

 * *Differences: {"'cells'": "{21: {'source': {insert: [(11, 'result = None\\n')]}}}"}*

```diff
@@ -319,14 +319,15 @@
                 "saved_weights_fname = \"./psMNIST-weights.hdf5\"\n",
                 "callbacks = [\n",
                 "    tf.keras.callbacks.ModelCheckpoint(\n",
                 "        filepath=saved_weights_fname, monitor=\"val_loss\", verbose=1, save_best_only=True\n",
                 "    ),\n",
                 "]\n",
                 "\n",
+                "result = None\n",
                 "if do_training:\n",
                 "    result = model.fit(\n",
                 "        X_train,\n",
                 "        Y_train,\n",
                 "        epochs=epochs,\n",
                 "        batch_size=batch_size,\n",
                 "        validation_data=(X_valid, Y_valid),\n",
```

### Comparing `keras-lmu-0.5.0/docs/examples.rst` & `keras-lmu-0.6.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.5.0/docs/getting-started.rst` & `keras-lmu-0.6.0/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.5.0/keras_lmu/layers.py` & `keras-lmu-0.6.0/keras_lmu/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Core classes for the KerasLMU package."""
 
+import warnings
+
 import numpy as np
 import tensorflow as tf
 from packaging import version
 
 # pylint: disable=ungrouped-imports
 if version.parse(tf.__version__) < version.parse("2.6.0rc0"):
     from tensorflow.python.keras.layers.recurrent import DropoutRNNCellMixin
@@ -150,31 +152,32 @@
 
         if self.discretizer not in ("zoh", "euler"):
             raise ValueError(
                 f"discretizer must be 'zoh' or 'euler' (got '{self.discretizer}')"
             )
 
         if self.hidden_cell is None:
-            for conn in ("hidden_to_memory", "input_to_hidden"):
-                if getattr(self, conn):
-                    raise ValueError(f"{conn} must be False if hidden_cell is None")
+            if self.hidden_to_memory:
+                raise ValueError(
+                    "hidden_to_memory must be False if hidden_cell is None"
+                )
 
             self.hidden_output_size = self.memory_d * self.order
             self.hidden_state_size = []
         elif hasattr(self.hidden_cell, "state_size"):
             self.hidden_output_size = self.hidden_cell.output_size
             self.hidden_state_size = self.hidden_cell.state_size
         else:
             # TODO: support layers that don't have the `units` attribute
             self.hidden_output_size = self.hidden_cell.units
             self.hidden_state_size = [self.hidden_cell.units]
 
-        self.state_size = tf.nest.flatten(self.hidden_state_size) + [
-            self.memory_d * self.order
-        ]
+        self.state_size = [self.memory_d * self.order] + tf.nest.flatten(
+            self.hidden_state_size
+        )
         self.output_size = self.hidden_output_size
 
     @property
     def theta(self):
         """
         Value of the ``theta`` parameter.
 
@@ -224,15 +227,15 @@
 
         Note that this accepts and returns matrices that are transposed from the
         standard linear system implementation (as that makes it easier to use in
         `.call`).
         """
 
         # combine A/B and pad to make square matrix
-        em_upper = tf.concat([A, B], axis=0)
+        em_upper = tf.concat([A, B], axis=0)  # pylint: disable=no-value-for-parameter
         em = tf.pad(em_upper, [(0, 0), (0, B.shape[0])])
 
         # compute matrix exponential
         ms = tf.linalg.expm(em)
 
         # slice A/B back out of combined matrix
         discrt_A = ms[: A.shape[0], : A.shape[1]]
@@ -322,21 +325,25 @@
         """
 
         if training is None:
             training = tf.keras.backend.learning_phase()
 
         states = tf.nest.flatten(states)
 
-        # state for the hidden cell
-        h = states[:-1]
         # state for the LMU memory
-        m = states[-1]
+        m = states[0]
+        # state for the hidden cell
+        h = states[1:]
 
         # compute memory input
-        u = tf.concat((inputs, h[0]), axis=1) if self.hidden_to_memory else inputs
+        u = (
+            tf.concat((inputs, h[0]), axis=1)  # pylint: disable=no-value-for-parameter
+            if self.hidden_to_memory
+            else inputs
+        )
         if self.dropout > 0:
             u *= self.get_dropout_mask_for_cell(u, training)
         if self.kernel is not None:
             u = tf.matmul(u, self.kernel, name="kernel_matmul")
         if self.bias is not None:
             u = u + self.bias
 
@@ -377,26 +384,30 @@
         else:
             m = _m
 
         # re-combine memory/order dimensions
         m = tf.reshape(m, (-1, self.memory_d * self.order))
 
         # apply hidden cell
-        h_in = tf.concat((m, inputs), axis=1) if self.input_to_hidden else m
+        h_in = (
+            tf.concat((m, inputs), axis=1)  # pylint: disable=no-value-for-parameter
+            if self.input_to_hidden
+            else m
+        )
 
         if self.hidden_cell is None:
             o = h_in
             h = []
         elif hasattr(self.hidden_cell, "state_size"):
             o, h = self.hidden_cell(h_in, h, training=training)
         else:
             o = self.hidden_cell(h_in, training=training)
             h = [o]
 
-        return o, h + [m]
+        return o, [m] + h
 
     def reset_dropout_mask(self):
         """Reset dropout mask for memory and hidden components."""
         super().reset_dropout_mask()
         if isinstance(self.hidden_cell, DropoutRNNCellMixin):
             self.hidden_cell.reset_dropout_mask()
 
@@ -407,34 +418,34 @@
             self.hidden_cell.reset_recurrent_dropout_mask()
 
     def get_config(self):
         """Return config of layer (for serialization during model saving/loading)."""
 
         config = super().get_config()
         config.update(
-            dict(
-                memory_d=self.memory_d,
-                order=self.order,
-                theta=self._init_theta,
-                hidden_cell=tf.keras.layers.serialize(self.hidden_cell),
-                trainable_theta=self.trainable_theta,
-                hidden_to_memory=self.hidden_to_memory,
-                memory_to_memory=self.memory_to_memory,
-                input_to_hidden=self.input_to_hidden,
-                discretizer=self.discretizer,
-                kernel_initializer=self.kernel_initializer,
-                recurrent_initializer=self.recurrent_initializer,
-                kernel_regularizer=self.kernel_regularizer,
-                recurrent_regularizer=self.recurrent_regularizer,
-                use_bias=self.use_bias,
-                bias_initializer=self.bias_initializer,
-                bias_regularizer=self.bias_regularizer,
-                dropout=self.dropout,
-                recurrent_dropout=self.recurrent_dropout,
-            )
+            {
+                "memory_d": self.memory_d,
+                "order": self.order,
+                "theta": self._init_theta,
+                "hidden_cell": tf.keras.layers.serialize(self.hidden_cell),
+                "trainable_theta": self.trainable_theta,
+                "hidden_to_memory": self.hidden_to_memory,
+                "memory_to_memory": self.memory_to_memory,
+                "input_to_hidden": self.input_to_hidden,
+                "discretizer": self.discretizer,
+                "kernel_initializer": self.kernel_initializer,
+                "recurrent_initializer": self.recurrent_initializer,
+                "kernel_regularizer": self.kernel_regularizer,
+                "recurrent_regularizer": self.recurrent_regularizer,
+                "use_bias": self.use_bias,
+                "bias_initializer": self.bias_initializer,
+                "bias_regularizer": self.bias_regularizer,
+                "dropout": self.dropout,
+                "recurrent_dropout": self.recurrent_dropout,
+            }
         )
 
         return config
 
     @classmethod
     def from_config(cls, config):
         """Load model from serialized config."""
@@ -589,31 +600,30 @@
                 self.layer.theta
                 if isinstance(self.layer, LMUFeedforward)
                 else self.layer.cell.theta
             )
 
         return self._init_theta
 
-    def build(self, input_shapes):
+    def build(self, input_shape):
         """
         Builds the layer.
 
         Notes
         -----
         This method should not be called manually; rather, use the implicit layer
         callable behaviour (like ``my_layer(inputs)``), which will apply this method
         with some additional bookkeeping.
         """
 
-        super().build(input_shapes)
+        super().build(input_shape)
 
         if (
             not self.hidden_to_memory
             and not self.memory_to_memory
-            and input_shapes[1] is not None
             and not self.trainable_theta
         ):
             self.layer = LMUFeedforward(
                 memory_d=self.memory_d,
                 order=self.order,
                 theta=self._init_theta,
                 hidden_cell=self.hidden_cell,
@@ -622,14 +632,15 @@
                 kernel_initializer=self.kernel_initializer,
                 kernel_regularizer=self.kernel_regularizer,
                 use_bias=self.use_bias,
                 bias_initializer=self.bias_initializer,
                 bias_regularizer=self.bias_regularizer,
                 dropout=self.dropout,
                 return_sequences=self.return_sequences,
+                dtype=self.dtype,
             )
         else:
             self.layer = tf.keras.layers.RNN(
                 LMUCell(
                     memory_d=self.memory_d,
                     order=self.order,
                     theta=self._init_theta,
@@ -644,19 +655,21 @@
                     kernel_regularizer=self.kernel_regularizer,
                     recurrent_regularizer=self.recurrent_regularizer,
                     use_bias=self.use_bias,
                     bias_initializer=self.bias_initializer,
                     bias_regularizer=self.bias_regularizer,
                     dropout=self.dropout,
                     recurrent_dropout=self.recurrent_dropout,
+                    dtype=self.dtype,
                 ),
                 return_sequences=self.return_sequences,
+                dtype=self.dtype,
             )
 
-        self.layer.build(input_shapes)
+        self.layer.build(input_shape)
 
     def call(self, inputs, training=None):
         """
         Apply this layer to inputs.
 
         Notes
         -----
@@ -668,35 +681,35 @@
         return self.layer.call(inputs, training=training)
 
     def get_config(self):
         """Return config of layer (for serialization during model saving/loading)."""
 
         config = super().get_config()
         config.update(
-            dict(
-                memory_d=self.memory_d,
-                order=self.order,
-                theta=self._init_theta,
-                hidden_cell=tf.keras.layers.serialize(self.hidden_cell),
-                trainable_theta=self.trainable_theta,
-                hidden_to_memory=self.hidden_to_memory,
-                memory_to_memory=self.memory_to_memory,
-                input_to_hidden=self.input_to_hidden,
-                discretizer=self.discretizer,
-                kernel_initializer=self.kernel_initializer,
-                recurrent_initializer=self.recurrent_initializer,
-                kernel_regularizer=self.kernel_regularizer,
-                recurrent_regularizer=self.recurrent_regularizer,
-                use_bias=self.use_bias,
-                bias_initializer=self.bias_initializer,
-                bias_regularizer=self.bias_regularizer,
-                dropout=self.dropout,
-                recurrent_dropout=self.recurrent_dropout,
-                return_sequences=self.return_sequences,
-            )
+            {
+                "memory_d": self.memory_d,
+                "order": self.order,
+                "theta": self._init_theta,
+                "hidden_cell": tf.keras.layers.serialize(self.hidden_cell),
+                "trainable_theta": self.trainable_theta,
+                "hidden_to_memory": self.hidden_to_memory,
+                "memory_to_memory": self.memory_to_memory,
+                "input_to_hidden": self.input_to_hidden,
+                "discretizer": self.discretizer,
+                "kernel_initializer": self.kernel_initializer,
+                "recurrent_initializer": self.recurrent_initializer,
+                "kernel_regularizer": self.kernel_regularizer,
+                "recurrent_regularizer": self.recurrent_regularizer,
+                "use_bias": self.use_bias,
+                "bias_initializer": self.bias_initializer,
+                "bias_regularizer": self.bias_regularizer,
+                "dropout": self.dropout,
+                "recurrent_dropout": self.recurrent_dropout,
+                "return_sequences": self.return_sequences,
+            }
         )
 
         return config
 
     @classmethod
     def from_config(cls, config):
         """Load model from serialized config."""
@@ -786,17 +799,14 @@
         return_sequences=False,
         conv_mode="fft",
         truncate_ir=1e-4,
         **kwargs,
     ):
         super().__init__(**kwargs)
 
-        if input_to_hidden and hidden_cell is None:
-            raise ValueError("input_to_hidden must be False if hidden_cell is None")
-
         if conv_mode not in ("fft", "raw"):
             raise ValueError(f"Unrecognized conv mode '{conv_mode}'")
 
         self.memory_d = memory_d
         self.order = order
         self.theta = theta
         self.hidden_cell = hidden_cell
@@ -822,16 +832,18 @@
                 trainable_theta=False,
                 input_to_hidden=False,
                 hidden_to_memory=False,
                 memory_to_memory=False,
                 discretizer=discretizer,
                 kernel_initializer=None,
                 trainable=False,
+                dtype=self.dtype,
             ),
             return_sequences=True,
+            dtype=self.dtype,
         )
         self.impulse_response = None
         self.kernel = None
         self.bias = None
 
     def build(self, input_shape):
         """
@@ -842,39 +854,45 @@
         This method should not be called manually; rather, use the implicit layer
         callable behaviour (like ``my_layer(inputs)``), which will apply this method
         with some additional bookkeeping.
         """
 
         super().build(input_shape)
 
-        seq_len = input_shape[1]
         enc_d = input_shape[-1]
-
+        seq_len = input_shape[1]
         if seq_len is None:
-            # TODO: we could dynamically run the impulse response for longer if
-            #  needed using stateful=True
-            raise ValueError(
-                f"LMUFeedforward requires that the input shape's temporal axis be "
-                f"fully specified (got {seq_len})"
+            theta_factor = 5
+            warnings.warn(
+                f"Approximating unknown impulse length with {theta_factor}*theta; "
+                f"setting a fixed sequence length on inputs will remove the need for "
+                f"approximation"
             )
+            impulse_len = self.theta * theta_factor
+        else:
+            impulse_len = seq_len
 
-        impulse = tf.reshape(tf.eye(seq_len, 1), (1, -1, 1))
+        impulse = tf.reshape(tf.eye(impulse_len, 1), (1, -1, 1))
 
         self.impulse_response = tf.squeeze(
             self.delay_layer(impulse, training=False), axis=0
         )
 
         if self.conv_mode == "fft":
-            self.impulse_response = tf.signal.rfft(
-                tf.transpose(self.impulse_response),
-                fft_length=[2 * seq_len],
+            self.impulse_response_fft = (
+                None
+                if seq_len is None
+                else tf.signal.rfft(
+                    tf.transpose(self.impulse_response),
+                    fft_length=[2 * seq_len],
+                )
             )
         else:
             if self.truncate_ir is not None:
-                assert self.impulse_response.shape == (seq_len, self.order)
+                assert self.impulse_response.shape == (impulse_len, self.order)
 
                 cumsum = tf.math.cumsum(
                     tf.math.abs(self.impulse_response), axis=0, reverse=True
                 )
                 cumsum = cumsum / cumsum[0]
                 to_drop = tf.reduce_all(cumsum < self.truncate_ir, axis=-1)
                 if to_drop[-1]:
@@ -945,21 +963,27 @@
 
         if self.conv_mode == "fft":
             m = self._fft_convolution(u)
         elif self.conv_mode == "raw":
             m = self._raw_convolution(u)
 
         # apply hidden cell
-        h_in = tf.concat((m, inputs), axis=-1) if self.input_to_hidden else m
+        h_in = (
+            tf.concat((m, inputs), axis=-1)  # pylint: disable=no-value-for-parameter
+            if self.input_to_hidden
+            else m
+        )
 
         if self.hidden_cell is None:
             h = h_in if self.return_sequences else h_in[:, -1]
         elif hasattr(self.hidden_cell, "state_size"):
             h = tf.keras.layers.RNN(
-                self.hidden_cell, return_sequences=self.return_sequences
+                self.hidden_cell,
+                return_sequences=self.return_sequences,
+                dtype=self.dtype,
             )(h_in, training=training)
         else:
             if not self.return_sequences:
                 # no point applying the hidden cell to the whole sequence
                 h = self.hidden_cell(h_in[:, -1], training=training)
             else:
                 h = tf.keras.layers.TimeDistributed(self.hidden_cell)(
@@ -973,17 +997,25 @@
 
         # FFT requires shape (batch, memory_d, timesteps)
         u = tf.transpose(u, perm=[0, 2, 1])
 
         # Pad sequences to avoid circular convolution
         # Perform the FFT
         fft_input = tf.signal.rfft(u, fft_length=[2 * seq_len])
+        impulse_response = (
+            tf.signal.rfft(
+                tf.transpose(self.impulse_response[:seq_len]),
+                fft_length=[2 * seq_len],
+            )
+            if self.impulse_response_fft is None
+            else self.impulse_response_fft
+        )
 
         # Elementwise product of FFT (with broadcasting)
-        result = tf.expand_dims(fft_input, axis=-2) * self.impulse_response
+        result = tf.expand_dims(fft_input, axis=-2) * impulse_response
 
         # Inverse FFT
         m = tf.signal.irfft(result, fft_length=[2 * seq_len])[..., :seq_len]
 
         m = tf.reshape(m, (-1, self.order * self.memory_d, seq_len))
 
         return tf.transpose(m, perm=[0, 2, 1])
@@ -1004,31 +1036,31 @@
         return m
 
     def get_config(self):
         """Return config of layer (for serialization during model saving/loading)."""
 
         config = super().get_config()
         config.update(
-            dict(
-                memory_d=self.memory_d,
-                order=self.order,
-                theta=self.theta,
-                hidden_cell=tf.keras.layers.serialize(self.hidden_cell),
-                input_to_hidden=self.input_to_hidden,
-                discretizer=self.discretizer,
-                kernel_initializer=self.kernel_initializer,
-                kernel_regularizer=self.kernel_regularizer,
-                use_bias=self.use_bias,
-                bias_initializer=self.bias_initializer,
-                bias_regularizer=self.bias_regularizer,
-                dropout=self.dropout,
-                return_sequences=self.return_sequences,
-                conv_mode=self.conv_mode,
-                truncate_ir=self.truncate_ir,
-            )
+            {
+                "memory_d": self.memory_d,
+                "order": self.order,
+                "theta": self.theta,
+                "hidden_cell": tf.keras.layers.serialize(self.hidden_cell),
+                "input_to_hidden": self.input_to_hidden,
+                "discretizer": self.discretizer,
+                "kernel_initializer": self.kernel_initializer,
+                "kernel_regularizer": self.kernel_regularizer,
+                "use_bias": self.use_bias,
+                "bias_initializer": self.bias_initializer,
+                "bias_regularizer": self.bias_regularizer,
+                "dropout": self.dropout,
+                "return_sequences": self.return_sequences,
+                "conv_mode": self.conv_mode,
+                "truncate_ir": self.truncate_ir,
+            }
         )
 
         return config
 
     @classmethod
     def from_config(cls, config):
         """Load model from serialized config."""
```

### Comparing `keras-lmu-0.5.0/keras_lmu/tests/test_benchmarks.py` & `keras-lmu-0.6.0/keras_lmu/tests/test_benchmarks.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     # TensorFlow version: 2.6.0
 
     dims = 32
     seq_len = 512
     batch_size = 16
     odims = 2
 
-    kwargs = dict(memory_d=dims, order=256, theta=784, hidden_cell=None)
+    kwargs = {"memory_d": dims, "order": 256, "theta": 784, "hidden_cell": None}
     if mode == "rnn":
         lmu_layer = tf.keras.layers.RNN(
             layers.LMUCell(**kwargs),
             return_sequences=False,
         )
     elif mode in ("fft", "raw"):
         lmu_layer = layers.LMUFeedforward(
```

### Comparing `keras-lmu-0.5.0/keras_lmu/tests/test_layers.py` & `keras-lmu-0.6.0/keras_lmu/tests/test_layers.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,23 +70,23 @@
 
 @pytest.mark.parametrize("has_input_kernel", (True, False))
 @pytest.mark.parametrize("feedforward", (True, False))
 @pytest.mark.parametrize("discretizer", ("zoh", "euler"))
 def test_layer_vs_cell(rng, has_input_kernel, feedforward, discretizer):
     n_steps = 10
     input_d = 32
-    kwargs = dict(
-        memory_d=4 if has_input_kernel else input_d,
-        order=12,
-        theta=n_steps * (8 if discretizer == "euler" else 1),
-        discretizer=discretizer,
-        kernel_initializer="glorot_uniform" if has_input_kernel else None,
-        memory_to_memory=not feedforward,
-        use_bias=True,
-    )
+    kwargs = {
+        "memory_d": 4 if has_input_kernel else input_d,
+        "order": 12,
+        "theta": n_steps * (8 if discretizer == "euler" else 1),
+        "discretizer": discretizer,
+        "kernel_initializer": "glorot_uniform" if has_input_kernel else None,
+        "memory_to_memory": not feedforward,
+        "use_bias": True,
+    }
 
     def hidden_cell():
         return tf.keras.layers.SimpleRNNCell(units=64)
 
     inp = rng.uniform(-1, 1, size=(2, n_steps, input_d))
 
     lmu_cell = tf.keras.layers.RNN(
@@ -213,57 +213,69 @@
 
 
 @pytest.mark.parametrize("return_sequences", (True, False))
 @pytest.mark.parametrize(
     "hidden_cell",
     (
         lambda: None,
-        lambda: tf.keras.layers.Dense(4),
-        lambda: tf.keras.layers.SimpleRNNCell(4),
+        lambda: tf.keras.layers.Dense(4, dtype="float64"),
+        lambda: tf.keras.layers.SimpleRNNCell(4, dtype="float64"),
     ),
 )
-@pytest.mark.parametrize("memory_d", [1, 4])
 @pytest.mark.parametrize("discretizer", ("zoh", "euler"))
 @pytest.mark.parametrize("conv_mode", ["fft", "raw"])
+@pytest.mark.parametrize("seq_len", [10, 50])
 def test_feedforward(
-    return_sequences, hidden_cell, memory_d, discretizer, conv_mode, rng
+    return_sequences, hidden_cell, discretizer, conv_mode, seq_len, rng, seed
 ):
-    kwargs = dict(
-        memory_d=memory_d,
-        order=2,
-        theta=12,
-        hidden_cell=hidden_cell(),
-        discretizer=discretizer,
-    )
+    kwargs = {
+        "memory_d": 4,
+        "order": 2,
+        "theta": 5,
+        "hidden_cell": hidden_cell(),
+        "discretizer": discretizer,
+        "dtype": "float64",
+    }
 
-    x = rng.uniform(-1, 1, size=(2, 10, 32))
+    x = rng.uniform(-1, 1, size=(2, seq_len, 32))
 
     rnn_layer = tf.keras.layers.RNN(
         layers.LMUCell(**kwargs),
         return_sequences=return_sequences,
+        dtype="float64",
     )
     rnn_out = rnn_layer(x)
 
     ff_layer = layers.LMUFeedforward(
         return_sequences=return_sequences, conv_mode=conv_mode, **kwargs
     )
-    ff_layer.build(x.shape)
-    ff_layer.kernel.assign(rnn_layer.cell.kernel)
+    ff_layer.build((2, None, 32))  # testing with unknown sequence length
+    ff_layer.set_weights(rnn_layer.get_weights())
     ff_out = ff_layer(x, training=None)
 
-    assert np.allclose(rnn_out, ff_out, atol=2e-6)
+    assert ff_out.dtype == rnn_out.dtype == "float64"
+    assert np.allclose(
+        rnn_out,
+        ff_out,
+        # larger error for longer sequences, where the error accumulates more
+        atol=5e-8 if seq_len < 50 else 5e-4,
+    ), np.max(abs(rnn_out - ff_out))
 
 
 @pytest.mark.parametrize("truncate_ir", [None, 1e-5, 1e-4, 1e-3])
 def test_raw_truncation(truncate_ir, rng):
     seq_len = 64
     theta = 11.2
-    kwargs = dict(
-        memory_d=4, order=4, theta=theta, hidden_cell=None, kernel_initializer=None
-    )
+    kwargs = {
+        "memory_d": 4,
+        "order": 4,
+        "theta": theta,
+        "hidden_cell": None,
+        "kernel_initializer": None,
+    }
 
     x = rng.uniform(-1, 1, size=(2, seq_len, kwargs["memory_d"]))
 
     rnn_layer = tf.keras.layers.RNN(layers.LMUCell(**kwargs), return_sequences=True)
     rnn_out = rnn_layer(x)
 
     ff_layer = layers.LMUFeedforward(
@@ -276,74 +288,66 @@
     # only one seed in 50 failed with `atol=truncate_ir`, hence the 1.2 fudge factor
     atol = 2e-6 if truncate_ir is None else 1.2 * truncate_ir
     assert np.allclose(rnn_out, ff_out, atol=atol)
 
 
 def test_validation_errors():
     ff_layer = layers.LMUFeedforward(1, 2, 3, None)
-    with pytest.raises(ValueError, match="temporal axis be fully specified"):
+    with pytest.warns(UserWarning, match="unknown impulse length"):
         ff_layer(tf.keras.Input((None, 32)))
 
     with pytest.raises(ValueError, match="hidden_to_memory must be False"):
         layers.LMUCell(1, 2, 3, None, hidden_to_memory=True)
 
-    with pytest.raises(ValueError, match="input_to_hidden must be False"):
-        layers.LMUCell(1, 2, 3, None, input_to_hidden=True)
-
-    with pytest.raises(ValueError, match="input_to_hidden must be False"):
-        layers.LMUFeedforward(1, 2, 3, None, input_to_hidden=True)
-
     with pytest.raises(ValueError, match="Unrecognized conv mode"):
         layers.LMUFeedforward(1, 2, 3, None, conv_mode="raw_bad")
 
 
 @pytest.mark.parametrize(
-    "should_use_feedforward, hidden_to_memory, memory_to_memory, steps, "
-    "trainable_theta",
+    "should_use_feedforward, hidden_to_memory, memory_to_memory, trainable_theta",
     [
-        (True, False, False, 5, False),
-        (False, True, False, 5, False),
-        (False, False, True, 5, False),
-        (False, False, False, None, False),
-        (False, False, False, 5, True),
+        (True, False, False, False),
+        (False, True, False, False),
+        (False, False, True, False),
+        (False, False, False, True),
     ],
 )
 def test_feedforward_auto_swap(
-    should_use_feedforward, hidden_to_memory, memory_to_memory, steps, trainable_theta
+    should_use_feedforward, hidden_to_memory, memory_to_memory, trainable_theta
 ):
     lmu = layers.LMU(
         4,
         2,
         3,
         tf.keras.layers.Dense(5),
         hidden_to_memory=hidden_to_memory,
         memory_to_memory=memory_to_memory,
         trainable_theta=trainable_theta,
     )
-    lmu.build((32, steps, 8))
+    lmu.build((32, None, 8))
 
     assert isinstance(lmu.layer, layers.LMUFeedforward) == should_use_feedforward
 
 
 @pytest.mark.parametrize(
     "hidden_cell",
     (tf.keras.layers.SimpleRNNCell(units=10), tf.keras.layers.Dense(units=10), None),
 )
 @pytest.mark.parametrize("feedforward", (True, False))
 def test_hidden_types(hidden_cell, feedforward, rng):
     x = rng.uniform(-1, 1, size=(2, 5, 32))
 
-    lmu_params = dict(
-        memory_d=1,
-        order=3,
-        theta=4,
-        kernel_initializer=tf.keras.initializers.constant(
+    lmu_params = {
+        "memory_d": 1,
+        "order": 3,
+        "theta": 4,
+        "kernel_initializer": tf.keras.initializers.constant(
             rng.uniform(-1, 1, size=(32, 1))
         ),
-    )
+    }
 
     base_lmu = tf.keras.layers.RNN(
         layers.LMUCell(hidden_cell=None, **lmu_params),
         return_sequences=True,
     )
     base_output = base_lmu(x)
     if isinstance(hidden_cell, tf.keras.layers.SimpleRNNCell):
@@ -362,32 +366,32 @@
             layers.LMUCell(hidden_cell=hidden_cell, **lmu_params),
             return_sequences=True,
         )
     )
     lmu_output = lmu(x)
 
     assert np.allclose(
-        lmu_output, base_output, atol=2e-6 if feedforward else 1e-8
+        lmu_output, base_output, atol=3e-6 if feedforward else 1e-8
     ), np.max(np.abs(lmu_output - base_output))
 
 
 @pytest.mark.parametrize("feedforward", (True, False))
 @pytest.mark.parametrize("hidden_cell", (None, tf.keras.layers.Dense))
 def test_connection_params(feedforward, hidden_cell):
     input_shape = (32, 7 if feedforward else None, 6)
 
     x = tf.keras.Input(batch_shape=input_shape)
 
-    lmu_args = dict(
-        memory_d=1,
-        order=3,
-        theta=4,
-        hidden_cell=hidden_cell if hidden_cell is None else hidden_cell(units=5),
-        input_to_hidden=False,
-    )
+    lmu_args = {
+        "memory_d": 1,
+        "order": 3,
+        "theta": 4,
+        "hidden_cell": hidden_cell if hidden_cell is None else hidden_cell(units=5),
+        "input_to_hidden": False,
+    }
     if not feedforward:
         lmu_args["hidden_to_memory"] = False
         lmu_args["memory_to_memory"] = False
 
     lmu = (
         layers.LMUCell(**lmu_args)
         if not feedforward
@@ -448,15 +452,15 @@
 @pytest.mark.parametrize("feedforward", (True, False))
 def test_dropout(
     dropout, recurrent_dropout, hidden_dropout, hidden_recurrent_dropout, feedforward
 ):
     if feedforward:
         kwargs = {}
     else:
-        kwargs = dict(memory_to_memory=True, recurrent_dropout=recurrent_dropout)
+        kwargs = {"memory_to_memory": True, "recurrent_dropout": recurrent_dropout}
     lmu = layers.LMU(
         memory_d=1,
         order=3,
         theta=4,
         hidden_cell=tf.keras.layers.SimpleRNNCell(
             5, dropout=hidden_dropout, recurrent_dropout=hidden_recurrent_dropout
         ),
@@ -497,15 +501,15 @@
         hidden_to_memory=not feedforward,
         memory_to_memory=not feedforward,
         input_to_hidden=not feedforward,
         discretizer=discretizer,
         kernel_initializer="zeros",
     )
 
-    inputs = tf.keras.layers.Input((5 if feedforward else None, 10))
+    inputs = tf.keras.layers.Input((None, 10))
     lmu = lmu_layer(inputs)
     outputs = tf.keras.layers.Dense(2)(lmu)
 
     model = tf.keras.Model(inputs=inputs, outputs=outputs)
 
     x_train = tf.ones((5, 5, 10))
     x_test = tf.ones((5, 5, 10))
@@ -720,16 +724,34 @@
     assert np.isclose(regularization_loss, target)
 
 
 @pytest.mark.parametrize("cls", [layers.LMUCell, layers.LMU, layers.LMUFeedforward])
 def test_get_config(cls):
     """Test that all ``__init__`` arguments appear in the ``get_config`` dictionary."""
 
-    params = dict(memory_d=2, order=5, theta=3.2, hidden_cell=None)
-    obj = cls(**params)
+    obj = cls(memory_d=2, order=5, theta=3.2, hidden_cell=None)
 
     config = obj.get_config()
     sig = inspect.signature(cls.__init__)
 
     for key in sig.parameters:
         if key not in ("self", "kwargs"):
             assert key in config, key
+
+
+@pytest.mark.parametrize("feedforward", [True, False])
+@pytest.mark.parametrize("dtype", [None, "float32", "float64"])
+def test_dtype(feedforward, dtype):
+    x = np.ones((2, 10, 5))
+    layer = layers.LMU(
+        1,
+        2,
+        3,
+        tf.keras.layers.SimpleRNNCell(4, dtype=dtype),
+        trainable_theta=not feedforward,
+        dtype=dtype,
+    )
+    y = layer(x)
+    assert isinstance(
+        layer.layer, layers.LMUFeedforward if feedforward else tf.keras.layers.RNN
+    )
+    assert y.dtype == ("float32" if dtype is None else dtype)
```

### Comparing `keras-lmu-0.5.0/keras_lmu/version.py` & `keras-lmu-0.6.0/keras_lmu/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 We use semantic versioning (see http://semver.org/) and conform to PEP440 (see
 https://www.python.org/dev/peps/pep-0440/). '.dev0' will be added to the version
 unless the code base represents a release version. Release versions are git
 tagged with the version.
 """
 
-version_info = (0, 5, 0)
+version_info = (0, 6, 0)
 
 name = "keras-lmu"
 dev = None
 
 # use old string formatting, so that this can still run in Python <= 3.5
 # (since this file is parsed in setup.py, before python_requires is applied)
 version = ".".join(str(v) for v in version_info)
 if dev is not None:
-    version += ".dev%d" % dev
+    version += ".dev%d" % dev  # pragma: no cover
 
 copyright = "Copyright (c) 2019-2023 Applied Brain Research"
```

### Comparing `keras-lmu-0.5.0/keras_lmu.egg-info/PKG-INFO` & `keras-lmu-0.6.0/keras_lmu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-lmu
-Version: 0.5.0
+Version: 0.6.0
 Summary: Keras implementation of Legendre Memory Units
 Home-page: https://www.nengo.ai/keras-lmu
 Author: Applied Brain Research
 Author-email: info@appliedbrainresearch.com
 License: Free for non-commercial use
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -114,14 +114,35 @@
 
    - Added
    - Changed
    - Deprecated
    - Removed
    - Fixed
 
+0.6.0 (May 5, 2023)
+===================
+
+*Compatible with TensorFlow 2.4 - 2.11*
+
+**Changed**
+
+- ``LMUFeedforward`` can now be used with unknown sequence lengths, and ``LMU`` will
+  use ``LMUFeedforward`` for unknown sequence lengths (as long as the other conditions
+  are met, as before). (`#52`_)
+- Allow ``input_to_hidden=True`` with ``hidden_cell=None``. This will act as a skip
+  connection. (`#52`_)
+- Changed order of LMU states so that the LMU memory state always comes first, and
+  any states from the hidden cell come afterwards. (`#52`_)
+
+**Fixed**
+
+- Fixed errors when setting non-default dtype on LMU layers. (`#52`_)
+
+.. _#52: https://github.com/nengo/keras-lmu/pull/52
+
 0.5.0 (January 26, 2023)
 ========================
 
 *Compatible with TensorFlow 2.4 - 2.11*
 
 **Added**
```

### Comparing `keras-lmu-0.5.0/keras_lmu.egg-info/SOURCES.txt` & `keras-lmu-0.6.0/keras_lmu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.5.0/setup.cfg` & `keras-lmu-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.5.0/setup.py` & `keras-lmu-0.6.0/setup.py`

 * *Files identical despite different names*

