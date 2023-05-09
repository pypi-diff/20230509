# Comparing `tmp/sleepeeg-0.0.1.tar.gz` & `tmp/sleepeeg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepeeg-0.0.1.tar", last modified: Sun Apr 16 16:15:43 2023, max compression
+gzip compressed data, was "sleepeeg-0.1.1.tar", last modified: Tue May  9 13:32:46 2023, max compression
```

## Comparing `sleepeeg-0.0.1.tar` & `sleepeeg-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 16:15:43.194537 sleepeeg-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-03-20 20:54:05.000000 sleepeeg-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1575 2023-04-16 16:15:43.194537 sleepeeg-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2023-04-16 16:10:40.000000 sleepeeg-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 16:15:43.170600 sleepeeg-0.0.1/docs/
--rw-rw-rw-   0        0        0     1302 2023-03-20 20:54:05.000000 sleepeeg-0.0.1/docs/conf.py
--rw-rw-rw-   0        0        0      621 2023-04-16 16:10:28.000000 sleepeeg-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 16:15:43.195536 sleepeeg-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      241 2023-03-26 21:13:28.000000 sleepeeg-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:15:43.175586 sleepeeg-0.0.1/sleepeeg/
--rw-rw-rw-   0        0        0    29483 2023-04-10 11:29:46.000000 sleepeeg-0.0.1/sleepeeg/base.py
--rw-rw-rw-   0        0        0    20748 2023-04-16 15:46:09.000000 sleepeeg-0.0.1/sleepeeg/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:15:43.192542 sleepeeg-0.0.1/sleepeeg.egg-info/
--rw-rw-rw-   0        0        0     1575 2023-04-16 16:15:43.000000 sleepeeg-0.0.1/sleepeeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-04-16 16:15:43.000000 sleepeeg-0.0.1/sleepeeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 16:15:43.000000 sleepeeg-0.0.1/sleepeeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-16 16:15:43.000000 sleepeeg-0.0.1/sleepeeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-16 16:15:43.000000 sleepeeg-0.0.1/sleepeeg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 13:32:46.368809 sleepeeg-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2023-03-20 20:54:05.000000 sleepeeg-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1966 2023-05-09 13:32:46.367812 sleepeeg-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1696 2023-05-09 11:39:44.000000 sleepeeg-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 13:32:46.339886 sleepeeg-0.1.1/docs/
+-rw-rw-rw-   0        0        0     1302 2023-03-20 20:54:05.000000 sleepeeg-0.1.1/docs/conf.py
+-rw-rw-rw-   0        0        0      660 2023-05-09 13:32:29.000000 sleepeeg-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 13:32:46.368809 sleepeeg-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      241 2023-03-26 21:13:28.000000 sleepeeg-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:32:46.343876 sleepeeg-0.1.1/sleepeeg/
+-rw-rw-rw-   0        0        0    49799 2023-05-09 13:10:00.000000 sleepeeg-0.1.1/sleepeeg/base.py
+-rw-rw-rw-   0        0        0    23551 2023-05-09 13:20:03.000000 sleepeeg-0.1.1/sleepeeg/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:32:46.366814 sleepeeg-0.1.1/sleepeeg.egg-info/
+-rw-rw-rw-   0        0        0     1966 2023-05-09 13:32:46.000000 sleepeeg-0.1.1/sleepeeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-05-09 13:32:46.000000 sleepeeg-0.1.1/sleepeeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 13:32:46.000000 sleepeeg-0.1.1/sleepeeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2023-05-09 13:32:46.000000 sleepeeg-0.1.1/sleepeeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-09 13:32:46.000000 sleepeeg-0.1.1/sleepeeg.egg-info/top_level.txt
```

### Comparing `sleepeeg-0.0.1/LICENSE` & `sleepeeg-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.0.1/PKG-INFO` & `sleepeeg-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: sleepeeg
-Version: 0.0.1
+Version: 0.1.1
 Summary: Sleep EEG preprocessing and analysis
 Author-email: Gennadiy Belonosov <gennadiyb@mail.tau.ac.il>
 License: MIT
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sleep-eeg-processing
 **sleepeeg** is a high-level API built on top of [mne-python](https://mne.tools/stable/index.html) for preprocessing and analysis of sleep EEG data.
 ## Installation
 0. Make sure you have [Python](https://www.python.org/downloads/) installed.
     - The script was tested with the version 3.10.9
     - Python 3.11.x currently isn't supported because of the yasa's dependency on the numba library.
-1. Create a python environment
+1. Create a Python virtual environment, for more info you can refer to python [venv](https://docs.python.org/3/tutorial/venv.html), [virtualenv](https://virtualenv.pypa.io/en/latest/user_guide.html) or [conda](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).
 2. Activate the environment
 3. 
     ```
     pip install sleepeeg
     ```
 4. (Optional, but recommended) [Download](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/NirLab-TAU/sleep-eeg-processing/tree/main/notebooks) notebooks.
-5. (Optional, but recommended) Prepare [GPU acceleration](https://mne.tools/stable/install/advanced.html#gpu-acceleration-with-cuda) by installing [CUDA](https://developer.nvidia.com/cuda-downloads) and [CuPy](https://cupy.dev/).
+5. (Optional, but recommended) Prepare [GPU acceleration](https://mne.tools/stable/install/advanced.html#gpu-acceleration-with-cuda) by installing [CUDA](https://developer.nvidia.com/cuda-downloads) and [CuPy](https://cupy.dev/). After installation, to permanently enable CUDA use, do: 
+    ```
+    mne.utils.set_config('MNE_USE_CUDA', 'true')
+    ```
 6. (Optional) For OpenGL acceleration of [MNE plot](https://mne.tools/stable/generated/mne.io.Raw.html#mne.io.Raw.plot) install [pyopengl](https://pyopengl.sourceforge.net/documentation/installation.html) and use `plot(use_opengl=True)`.
 
 ## Quickstart
 1. Open any of the downloaded notebooks using the created environment.
 2. Follow the notebook's instructions.
```

### Comparing `sleepeeg-0.0.1/README.md` & `sleepeeg-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # sleep-eeg-processing
 **sleepeeg** is a high-level API built on top of [mne-python](https://mne.tools/stable/index.html) for preprocessing and analysis of sleep EEG data.
 ## Installation
 0. Make sure you have [Python](https://www.python.org/downloads/) installed.
     - The script was tested with the version 3.10.9
     - Python 3.11.x currently isn't supported because of the yasa's dependency on the numba library.
-1. Create a python environment
+1. Create a Python virtual environment, for more info you can refer to python [venv](https://docs.python.org/3/tutorial/venv.html), [virtualenv](https://virtualenv.pypa.io/en/latest/user_guide.html) or [conda](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).
 2. Activate the environment
 3. 
     ```
     pip install sleepeeg
     ```
 4. (Optional, but recommended) [Download](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/NirLab-TAU/sleep-eeg-processing/tree/main/notebooks) notebooks.
-5. (Optional, but recommended) Prepare [GPU acceleration](https://mne.tools/stable/install/advanced.html#gpu-acceleration-with-cuda) by installing [CUDA](https://developer.nvidia.com/cuda-downloads) and [CuPy](https://cupy.dev/).
+5. (Optional, but recommended) Prepare [GPU acceleration](https://mne.tools/stable/install/advanced.html#gpu-acceleration-with-cuda) by installing [CUDA](https://developer.nvidia.com/cuda-downloads) and [CuPy](https://cupy.dev/). After installation, to permanently enable CUDA use, do: 
+    ```
+    mne.utils.set_config('MNE_USE_CUDA', 'true')
+    ```
 6. (Optional) For OpenGL acceleration of [MNE plot](https://mne.tools/stable/generated/mne.io.Raw.html#mne.io.Raw.plot) install [pyopengl](https://pyopengl.sourceforge.net/documentation/installation.html) and use `plot(use_opengl=True)`.
 
 ## Quickstart
 1. Open any of the downloaded notebooks using the created environment.
 2. Follow the notebook's instructions.
```

### Comparing `sleepeeg-0.0.1/docs/conf.py` & `sleepeeg-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.0.1/pyproject.toml` & `sleepeeg-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 exclude = ["notebooks"]  # empty by default
 
 [project]
 name = "sleepeeg"
-version = "0.0.1"
+version = "0.1.1"
 authors = [
     {name = "Gennadiy Belonosov", email = "gennadiyb@mail.tau.ac.il"},
 ]
 description = "Sleep EEG preprocessing and analysis"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 license = {text = "MIT"}
 dependencies = [
     "attrs",
     "mne",
     "mne-qt-browser",
     "pyqt5",
     "yasa==0.6.3",
     "lspopt",
     "ipympl",
     "numpy",
     "pandas",
     "scipy",
     "fooof",
+    "natsort",
+    "more-itertools"
 ]
```

### Comparing `sleepeeg-0.0.1/sleepeeg/base.py` & `sleepeeg-0.1.1/sleepeeg/pipeline.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,792 +1,626 @@
-import os
-import errno
+"""This module contains and describes pipe elements for sleep eeg analysis.
+"""
 
-from abc import ABC, abstractmethod
-from collections.abc import Iterable
-from pathlib import Path
-
-from typing import TypeVar, Type
 from attrs import define, field
-
+from pathlib import Path
 import matplotlib.pyplot as plt
 import numpy as np
-import mne
-from tqdm import tqdm
+import mne.io
 
-# For type annotation of pipe elements.
-BasePipeType = TypeVar("BasePipeType", bound="BasePipe")
 
+from collections.abc import Iterable
 
-@define(kw_only=True, slots=False)
-class BasePipe(ABC):
-    """A template class for the pipeline segments."""
-
-    prec_pipe: Type[BasePipeType] = field(default=None, metadata={"my_metadata": 1})
-    """Preceding pipe that hands over mne_raw attr."""
+from sleepeeg.base import BasePipe, BaseHypnoPipe, BaseEventPipe, BaseSpectrum
 
-    path_to_eeg: Path = field(converter=Path)
-    """Can be any file type supported by 
-    `mne.io.read_raw() <https://mne.tools/stable/generated/
-    mne.io.Raw.html#mne.io.Raw.save>`_.
-    """
-
-    @path_to_eeg.default
-    def _set_path_to_eeg(self):
-        if self.prec_pipe:
-            return "/"
-        raise TypeError('Provide either "pipe" or "path_to_eeg" arguments')
-
-    @path_to_eeg.validator
-    def _validate_path_to_eeg(self, attr, value):
-        if not value.exists():
-            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), value)
-
-    output_dir: Path = field(converter=Path)
-    """Path to the directory where the output will be saved."""
-
-    @output_dir.default
-    def _set_output_dir(self):
-        return (
-            self.prec_pipe.output_dir if self.prec_pipe else self.path_to_eeg.parents[0]
-        )
 
-    @output_dir.validator
-    def _validate_output_dir(self, attr, value):
-        self.output_dir.mkdir(exist_ok=True)
+@define(kw_only=True)
+class CleaningPipe(BasePipe):
+    """The cleaning pipeline element.
 
-    mne_raw: mne.io.Raw = field(init=False)
-    """An instanse of  
-    `mne.io.Raw <https://mne.tools/stable/generated/
-    mne.io.Raw.html#mne-io-raw>`_.
+    Contains resampling function, band and notch filters,
+    browser for manual selection of bad channels
+    and bad data spans.
     """
 
-    @mne_raw.default
-    def _read_mne_raw(self):
-        from mne.io import read_raw
+    def resample(
+        self,
+        save: bool = False,
+        mne_resample_args: dict = None,
+    ):
+        """A wrapper for
+        `mne.io.Raw.resample <https://mne.tools/stable/generated/mne.io.Raw.html#mne.io.Raw.resample>`_
+        with an additional option to save the resampled data.
 
-        try:
-            return (
-                self.prec_pipe.mne_raw if self.prec_pipe else read_raw(self.path_to_eeg)
+        Args:
+            save: Whether to save a resampled data to a fif file. Defaults to False.
+            mne_resample_args: Arguments passed to `mne.io.Raw.resample <https://mne.tools/stable/
+                generated/mne.io.Raw.html#mne.io.Raw.resample>`_. Defaults to None.
+        """
+        mne_resample_args = mne_resample_args or dict()
+        mne_resample_args.setdefault("sfreq", 250)
+        self.mne_raw.resample(**mne_resample_args)
+        if save:
+            self.save_raw(
+                "_".join(
+                    filter(
+                        None,
+                        [
+                            "resampled",
+                            str(mne_resample_args["sfreq"]) + "hz",
+                            "raw.fif",
+                        ],
+                    )
+                )
             )
-        except Exception as err:
-            print(f"Unexpected {err=}, {type(err)=}")
-            raise
 
-    @property
-    def sf(self):
+    def filter(
+        self,
+        mne_filter_args: dict = None,
+    ):
         """A wrapper for
-        `mne.Info["sfreq"] <https://mne.tools/stable/generated/
-        mne.Info.html#mne-info>`_.
+        `mne.io.Raw.filter <https://mne.tools/stable/generated/mne.io.Raw.html#mne.io.Raw.filter>`_.
 
-        Returns:
-            float: sampling frequency
+        Args:
+            mne_filter_args: Arguments passed to `mne.io.Raw.filter <https://mne.tools/stable/generated/mne.io.Raw.html#mne.io.Raw.filter>`_.
         """
-        return self.mne_raw.info["sfreq"]
+        mne_filter_args = mne_filter_args or dict()
+        mne_filter_args.setdefault("l_freq", 0.3)
+        self.mne_raw.load_data()
+        self.mne_raw.filter(**mne_filter_args)
 
-    def plot(
+    def notch(
         self,
-        butterfly: bool = False,
-        save_annotations: bool = False,
-        save_bad_channels: bool = False,
-        scalings: str | dict = "auto",
-        use_opengl: bool = False,
-        overwrite: bool = False,
+        mne_notch_args: dict = None,
     ):
-        """A wrapper for `mne.io.Raw.plot() <https://mne.tools/stable/
-        generated/mne.io.Raw.html#mne.io.Raw.plot>`_.
+        """A wrapper for
+        `mne.io.Raw.notch_filter <https://mne.tools/stable/generated/mne.io.Raw.html#mne.io.Raw.notch_filter>`_.
+
+        Args:
+            freqs: Frequencies to filter out from data,
+                e.g. np.arange(50, 251, 50) for sampling freq 250 Hz.
+                Defaults to None.
+            picks: Channels to filter, if None - all channels will be filtered.
+                Defaults to "eeg".
+            n_jobs: The number of jobs to run in parallel or CUDA. Defaults to "cuda".
+        """
+        mne_notch_args = mne_notch_args or dict()
+        mne_notch_args.setdefault("freqs", np.arange(50, int(self.sf / 2), 50))
+        self.mne_raw.notch_filter(**mne_notch_args)
+
+    def read_bad_channels(self, path=None):
+        """Imports bad channels from file to mne raw object.
 
         Args:
-            butterfly: Whether to start in butterfly mode. Defaults to False.
-            save_annotations: Whether to save annotations as txt. Defaults to False.
-            save_bad_channels: Whether to save bad channels as txt. Defaults to False.
-            scalings: Scale for amplitude per channel type. Defaults to 'auto'.
-            use_opengl: Whether to use OpenGL acceleration. Defaults to None.
-            overwrite: Whether to overwrite annotations and bad_channels files if exist.
-                Defaults to False.
-        """
-        from mne import pick_types
-
-        order = pick_types(self.mne_raw.info, eeg=True) if butterfly else None
-        self.mne_raw.plot(
-            theme="dark",
-            block=True,
-            scalings=scalings,
-            bad_color="r",
-            proj=False,
-            order=order,
-            butterfly=butterfly,
-            use_opengl=use_opengl,
+            path: Path to the txt file with bad channel name per row. Defaults to None.
+        """
+        p = (
+            Path(path)
+            if path
+            else self.output_dir / self.__class__.__name__ / "bad_channels.txt"
         )
-        if save_annotations:
-            self.mne_raw.annotations.save(
-                self.output_dir / "annotations.txt", overwrite=overwrite
-            )
-        if save_bad_channels:
-            with open(
-                self.output_dir / "bad_channels.txt", "w" if overwrite else "x"
-            ) as f:
-                for bad in self.mne_raw.info["bads"]:
-                    f.write(f"{bad}\n")
-
-    def save_raw(self, fname: str):
-        """A wrapper for `mne.io.Raw.save <https://mne.tools/stable/
-        generated/mne.io.Raw.html#mne.io.Raw.save>`_.
+        with open(p, "r") as f:
+            self.mne_raw.info["bads"] = list(filter(None, f.read().split("\n")))
+
+    def read_annotations(self, path=None):
+        """Imports annotations from file to mne raw object
 
         Args:
-            fname: filename for the fif file being saved.
+            path: Path to txt file with mne-style annotations. Defaults to None.
         """
-        path_to_resampled = self.output_dir / "saved_raw"
-        path_to_resampled.mkdir(exist_ok=True)
-        self.mne_raw.save(path_to_resampled / fname)
+        from mne import read_annotations
+
+        p = (
+            Path(path)
+            if path
+            else self.output_dir / self.__class__.__name__ / "annotations.txt"
+        )
+        self.mne_raw.set_annotations(read_annotations(p))
 
 
-@define(kw_only=True, slots=False)
-class BaseHypnoPipe(BasePipe, ABC):
-    """A template class for the sleep stage analysis pipeline segments."""
+@define(kw_only=True)
+class ICAPipe(BasePipe):
+    """The ICA pipeline element.
 
-    path_to_hypno: Path = field(converter=Path)
-    """Path to hypnogram. Must be text file with every 
-    row being int representing sleep stage for the epoch.
+    Contains ica fitting, plotting multiple ica plots,
+    selecting ica exclusion components and
+    its application to the raw data.
+    More at `mne.preprocessing.ICA <https://mne.tools/stable/
+    generated/mne.preprocessing.ICA.html#mne-preprocessing-ica>`_.
     """
 
-    @path_to_hypno.default
-    def _set_path_to_hypno(self):
-        return "/"
-
-    @path_to_hypno.validator
-    def _validate_path_to_hypno(self, attr, value):
-        if not value.exists():
-            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), value)
+    n_components: int | float | None = field(default=30)
+    """Number of principal components (from the pre-whitening PCA step) 
+    that are passed to the ICA algorithm during fitting.
+    """
 
-    hypno_freq: float = field(converter=float)
-    """Sampling rate of the hypnogram in Hz.
+    method: str = field(default="fastica")
+    """The ICA method to use in the fit method. 
 
-    E.g., 1/30 means 1 sample per 30 secs epoch,
-    250 means 1 sample per 1/250 sec epoch.
+    Can be 'fastica', 'infomax' or 'picard'
+    Use the fit_params argument to set additional parameters.
     """
-
-    @hypno_freq.default
-    def _get_hypno_freq(self):
-        if self.prec_pipe and isinstance(self.prec_pipe, BaseHypnoPipe):
-            return self.prec_pipe.hypno_freq
-        return 1
-
-    hypno: np.ndarray = field()
-    """ Hypnogram with sampling frequency hypno_freq
-    with int representing sleep stage.
+    fit_params: dict = field(default=None)
+    """Additional parameters passed to the ICA estimator as specified by method. 
+    Allowed entries are determined by the various algorithm implementations: 
+    see `FastICA <https://scikit-learn.org/stable/modules/generated/sklearn.
+    decomposition.FastICA.html#sklearn.decomposition.FastICA>`_, 
+    `picard <https://pierreablin.github.io/picard/generated/picard.picard.html#picard.picard>`_ and
+    `infomax <https://mne.tools/stable/generated/mne.preprocessing.infomax.html#mne.preprocessing.infomax>`_.
     """
 
-    @hypno.default
-    def _import_hypno(self):
-        if self.prec_pipe and isinstance(self.prec_pipe, BaseHypnoPipe):
-            return self.prec_pipe.hypno
-        if self.path_to_hypno == Path("/"):
-            return np.empty(0)
-        try:
-            return np.loadtxt(self.path_to_hypno)
-        except Exception as err:
-            print(f"Unexpected {err=}, {type(err)=}")
-            raise
+    path_to_ica: Path = field(converter=Path, default="/")
 
-    hypno_up: np.array = field()
-    """ Hypnogram upsampled to the sampling frequency of the raw data.
+    mne_ica: mne.preprocessing.ICA = field()
+    """Instance of 
+    `mne.preprocessing.ICA <https://mne.tools/stable/
+    generated/mne.preprocessing.ICA.html#mne-preprocessing-ica>`_.
     """
 
-    @hypno_up.default
-    def _set_hypno_up(self):
-        return self.hypno
+    @mne_ica.default
+    def _set_mne_ica(self):
+        if self.path_to_ica == Path("/"):
+            return mne.preprocessing.ICA(
+                n_components=self.n_components,
+                method=self.method,
+                fit_params=self.fit_params,
+            )
+        return mne.preprocessing.read_ica(self.path_to_ica)
 
     def __attrs_post_init__(self):
-        if self.hypno.any():
-            self.__upsample_hypno()
+        self.mne_raw.load_data()
 
-    def __upsample_hypno(self):
-        from yasa import hypno_upsample_to_data
+    def fit(self, filter_args=None, ica_fit_args=None):
+        """Highpass-filters (1Hz) a copy of the mne_raw object
+        and then runs `mne.preprocessing.ICA.fit <https://mne.tools/stable/
+        generated/mne.preprocessing.ICA.html#mne.preprocessing.ICA.fit>`_.
+        """
+        filter_args = filter_args or dict()
+        ica_fit_args = ica_fit_args or dict()
+        filter_args.setdefault("l_freq", 1.0)
+        if self.mne_raw.info["highpass"] < 1.0:
+            filtered_raw = self.mne_raw.copy()
+            filtered_raw.filter(**filter_args)
+        else:
+            filtered_raw = self.mne_raw
+        self.mne_ica.fit(filtered_raw, **ica_fit_args)
 
-        self.hypno_up = hypno_upsample_to_data(
-            self.hypno, self.hypno_freq, self.mne_raw, verbose=False
-        )
+    def plot_sources(self, **kwargs):
+        """A wrapper for `mne.preprocessing.ICA.plot_sources <https://mne.tools/stable/
+        generated/mne.preprocessing.ICA.html#mne.preprocessing.ICA.plot_sources>`_.
+        """
+        self.mne_ica.plot_sources(self.mne_raw, block=True, **kwargs)
 
-    def predict_hypno(
-        self,
-        eeg_name: str = "E183",
-        eog_name: str = "E252",
-        emg_name: str = "E247",
-        ref_name: str = "E26",
-        save=True,
-    ):
-        from yasa import SleepStaging, hypno_str_to_int
+    def plot_components(self, **kwargs):
+        """A wrapper for `mne.preprocessing.ICA.plot_components <https://mne.tools/stable/
+        generated/mne.preprocessing.ICA.html#mne.preprocessing.ICA.plot_components>`_.
+        """
+        self.mne_ica.plot_components(inst=self.mne_raw, **kwargs)
 
-        sls = SleepStaging(
-            self.mne_raw.copy().load_data().set_eeg_reference(ref_channels=[ref_name]),
-            eeg_name=eeg_name,
-            eog_name=eog_name,
-            emg_name=emg_name,
+    def plot_overlay(self, exclude=None, picks=None, start=10, stop=20, **kwargs):
+        """A wrapper for `mne.preprocessing.ICA.plot_overlay <https://mne.tools/stable/
+        generated/mne.preprocessing.ICA.html#mne.preprocessing.ICA.plot_overlay>`_.
+        """
+        self.mne_ica.plot_overlay(
+            self.mne_raw, exclude=exclude, picks=picks, start=start, stop=stop, **kwargs
         )
-        hypno = sls.predict()
-        self.hypno = hypno_str_to_int(hypno)
-        self.hypno_freq = 1 / 30
-        self.__upsample_hypno()
-        sls.plot_predict_proba()
-        if save:
-            np.savetxt(self.output_dir / "predicted_hypno.txt", self.hypno, fmt="%d")
-            plt.savefig(self.output_dir / "predicted_hypno_probabilities.png")
-
-    def sleep_stats(self, save: bool = False):
-        """A wrapper for
-        `yasa.sleep_statistics <https://raphaelvallat.com/yasa/build/html/generated/yasa.sleep_statistics.html#yasa-sleep-statistics>`_.
 
-        Args:
-            save: Whether to save the stats to csv. Defaults to False.
+    def plot_properties(self, picks=None, **kwargs):
+        """A wrapper for `mne.preprocessing.ICA.plot_properties <https://mne.tools/stable/
+        generated/mne.preprocessing.ICA.html#mne.preprocessing.ICA.plot_properties>`_.
         """
+        self.mne_ica.plot_properties(self.mne_raw, picks=picks, **kwargs)
 
-        from yasa import sleep_statistics
-        from csv import DictWriter
+    def apply(self, exclude=None, **kwargs):
+        """Remove selected components from the signal.
 
-        assert self.hypno.any(), "There is no hypnogram to get stats from."
-        stats = sleep_statistics(self.hypno, self.hypno_freq)
-        if save:
-            with open(self.output_dir / "sleep_stats.csv", "w", newline="") as csv_file:
-                w = DictWriter(csv_file, stats.keys())
-                w.writeheader()
-                w.writerow(stats)
-            return
-        return stats
-
-
-@define(kw_only=True, slots=False)
-class BaseEventPipe(BaseHypnoPipe, ABC):
-    """A template class for event detection."""
-
-    results = field(init=False)
-    """Event detection results as returned by YASA's event detection methods. 
-    Depending on the child class can be instance of either 
-    SpindlesResults, SWResults or REMResults classes. 
-    """
-
-    tfrs: dict = field(init=False)
-    """Instances of mne.time_frequency.AverageTFR per sleep stage.
-    """
-
-    @abstractmethod
-    def detect():
-        pass
-
-    def _save_to_csv(self):
-        self.results.summary().to_csv(
-            self.output_dir / f"{self.__class__.__name__[:-4].lower()}.csv", index=False
-        )
-
-    def _save_avg_fig(self):
-        plt.savefig(self.output_dir / f"{self.__class__.__name__[:-4].lower()}_avg.png")
+        A wrapper for `mne.preprocessing.ICA.apply <https://mne.tools/stable/
+        generated/mne.preprocessing.ICA.html#mne.preprocessing.ICA.apply>`_.
+        """
+        self.mne_ica.apply(self.mne_raw, exclude=exclude, **kwargs)
 
-    def plot_average(self, hue: str = "Stage", save: bool = False, **kwargs):
-        """Average of YASA's detected event.
+    def save_ica(self, fname="data-ica.fif", overwrite=False):
+        """A wrapper for `mne.preprocessing.ICA.save <https://mne.tools/stable/
+        generated/mne.preprocessing.ICA.html#mne.preprocessing.ICA.save>`_.
 
         Args:
-            hue: Grouping variable that will produce lines with different colors.
-                Can be either "Channel" or "Stage". Defaults to "Stage".
-            save: Whether to save the figure to file. Defaults to False.
-            **kwargs: Optional arguments passed to YASA's plot_average() method.
+            fname: filename for the ica file being saved. Defaults to "data-ica.fif".
+            overwrite: Whether to overwrite the file. Defaults to False.
         """
-        self.results.plot_average(hue=hue, **kwargs)
-        if save:
-            self._save_avg_fig()
+        fif_folder = self.output_dir / self.__class__.__name__ / "saved_ica"
+        fif_folder.mkdir(exist_ok=True)
+        self.mne_ica.save(fif_folder / fname, overwrite=overwrite)
 
-    def plot_topomap_per_stage(
-        self,
-        prop: str,
-        stage: str = "N2",
-        aggfunc: str = "mean",
-        sleep_stages: dict = {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4},
-        axis: plt.axis = None,
-        cmap: str = "plasma",
-        save: bool = False,
-    ):
-        """Plots topomap for a sleep stage and some property of detected events.
 
-        Args:
-            prop: Any event property returned by self.results.summary().
-            stage: One of the sleep_stages keys. Defaults to "N2".
-            aggfunc: Averaging function, "mean" or "median". Defaults to "mean".
-            sleep_stages: Mapping between sleep stages names and their integer representations.
-                Defaults to {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4}.
-            axis: Instance of `matplotlib.pyplot.axis <https://matplotlib.org/
-                stable/api/_as_gen/matplotlib.pyplot.axis.html#matplotlib-pyplot-axis>`_.
-                Defaults to None.
-            cmap: Matplotlib `colormap <https://matplotlib.org/stable/tutorials/colors/colormaps.html>`_.
-                Defaults to "plasma".
-            save: Whether to save the figure. Defaults to False.
-        """
-        from natsort import natsort_keygen
-        from more_itertools import collapse
+@define(kw_only=True)
+class SpectralPipe(BaseHypnoPipe, BaseSpectrum):
+    """The spectral analyses pipeline element.
 
-        grouped_summary = (
-            self.results.summary(grp_chan=True, grp_stage=True, aggfunc=aggfunc)
-            .sort_values("Channel", key=natsort_keygen())
-            .reset_index()
-        )
-        assert np.isin(
-            sleep_stages[stage], grouped_summary["Stage"].unique()
-        ).all(), "No such stage in the detected events, was it included in the detect method?"
-
-        is_new_axis = False
-        if not axis:
-            fig, axis = plt.subplots()
-            is_new_axis = True
-
-        per_stage = grouped_summary.loc[
-            grouped_summary["Stage"].isin(collapse([sleep_stages[stage]]))
-        ].groupby("Channel")
-        per_stage = per_stage.mean() if aggfunc == "mean" else per_stage.median()
-        per_stage = per_stage.sort_values("Channel", key=natsort_keygen()).reset_index()
-
-        info = self.mne_raw.copy().pick(list(per_stage["Channel"].unique())).info
-        data = per_stage[prop]
-        im, cn = mne.viz.plot_topomap(
-            data, info, axes=axis, cmap=cmap, show=False, vlim=(data.min(), data.max())
-        )
-        plt.colorbar(
-            im,
-            ax=axis,
-            orientation="vertical",
-            shrink=0.6,
-            label=prop,
-        )
-        if is_new_axis:
-            fig.suptitle(f"{stage} {self.__class__.__name__[:-4]} ({prop})")
-        if save and is_new_axis:
-            fig.savefig(
-                self.output_dir
-                / f"topomap_{self.__class__.__name__[:-4].lower()}_{prop.lower()}.png"
-            )
+    Contains methods for computing and plotting PSD,
+    spectrogram and topomaps, per sleep stage.
+    """
 
-    def plot_topomap_collage(
+    def plot_hypnospectrogram(
         self,
-        props: Iterable[str],
-        aggfunc: str = "mean",
-        stages_to_plot: tuple = "all",
-        sleep_stages: dict = {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4},
-        cmap: str = "plasma",
+        picks: str | Iterable[str] = ("E101",),
+        sec_per_seg: float = 4.096,
+        freq_range: tuple = (0, 40),
+        cmap: str = "inferno",
+        overlap: bool = False,
         save: bool = False,
     ):
-        """Plots topomap collage for multiple sleep stages and event properties.
+        """Plots hypnogram and spectrogram.
 
         Args:
-            props: Properties from the self.results.summary() to generate topomaps for.
-            aggfunc: Averaging function, "mean" or "median". Defaults to "mean".
-            stages_to_plot: stages_to_plot: Tuple of strings representing names from sleep_stages,
-                e.g., ("REM", "N1"). If set to "all" plots every stage provided in sleep_stages.
-                Defaults to "all".
-            sleep_stages: Mapping between sleep stages names and their integer representations.
-                Defaults to {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4}.
-            cmap: Matplotlib `colormap <https://matplotlib.org/stable/tutorials/colors/colormaps.html>`_.
-                Defaults to "plasma".
+            picks: Channels to calculate spectrogram on, more info at
+                `mne.io.Raw.get_data <https://mne.tools/stable/generated/
+                mne.io.Raw.html#mne.io.Raw.get_data>`_.
+                Defaults to ("E101",).
+            sec_per_seg: Segment length in seconds. Defaults to 4.096.
+            freq_range: Range of x axis on spectrogram plot. Defaults to (0, 40).
+            cmap: Matplotlib `colormap <https://matplotlib.org/stable/tutorials/colors/colormaps.html>`_. Defaults to "inferno".
+            overlap: Whether to plot hypnogram over the spectrogram or on top of it. Defaults to False.
             save: Whether to save the figure. Defaults to False.
         """
-        if stages_to_plot == "all":
-            stages_to_plot = {
-                k: v
-                for k, v in sleep_stages.items()
-                if v in self.results.summary()["Stage"].unique()
-            }
-        n_rows = len(stages_to_plot)
-        n_cols = len(props)
-
-        fig = plt.figure(figsize=(n_cols * 4, n_rows * 4), layout="constrained")
-        subfigs = fig.subfigures(n_rows, 1)
-
-        for row_index, stage in enumerate(tqdm(stages_to_plot)):
-            axes = subfigs[row_index].subplots(1, n_cols)
-
-            for col_index, prop in enumerate(tqdm(props, leave=False)):
-                self.plot_topomap_per_stage(
-                    stage=stage,
-                    prop=prop,
-                    aggfunc=aggfunc,
-                    sleep_stages=sleep_stages,
-                    axis=axes[col_index],
-                    cmap=cmap,
-                )
-                axes[col_index].set_title(f"{prop}")
-
-            subfigs[row_index].suptitle(f"{stage}", fontsize="xx-large")
-        fig.suptitle(f"{self.__class__.__name__[:-4]}", fontsize="xx-large")
+        # Import data from the raw mne file.
+        data = self.mne_raw.get_data(picks, units="uV", reject_by_annotation="NaN")[0]
+        # Create a plot figure
+        fig = self.__plot_hypnospectrogram(
+            data,
+            self.sf,
+            self.hypno_up,
+            win_sec=sec_per_seg,
+            fmin=freq_range[0],
+            fmax=freq_range[1],
+            trimperc=0,
+            cmap=cmap,
+            overlap=overlap,
+        )
+        # Save the figure if 'save' set to True
         if save:
             fig.savefig(
-                self.output_dir
-                / f"topomap_{self.__class__.__name__[:-4].lower()}_collage.png"
+                self.output_dir / self.__class__.__name__ / f"spectrogram.png",
+                bbox_inches="tight",
             )
 
-    def apply_tfr(
-        self,
-        freqs,
-        n_freqs,
-        time_before,
-        time_after,
-        n_jobs=-1,
-        method="morlet",
-        **kwargs,
+    def _compute_psd_per_stage(
+        self, picks, sleep_stages, avg_ref, dB, method_args=None
     ):
-        assert self.results, "Run detect method first"
-        assert (
-            method == "morlet" or method == "multitaper"
-        ), "method should be 'morlet' or 'multitaper'"
-        from natsort import natsorted
-
-        sleep_stages = {
-            -2: "Unscored",
-            -1: "Art",
-            0: "Wake",
-            1: "N1",
-            2: "N2",
-            3: "N3",
-            4: "REM",
-        }
-        freqs = np.linspace(freqs[0], freqs[1], n_freqs)
-        df_raw = self.results.get_sync_events(
-            time_before=time_before, time_after=time_after
-        )[["Event", "Amplitude", "Channel", "Stage"]]
-
-        self.tfrs = {}
-
-        for stage in df_raw["Stage"].unique():
-            df = df_raw[df_raw["Stage"] == stage]
-            # Group amplitudes by channel and events
-            df = df.groupby(["Channel", "Event"], group_keys=True).apply(
-                lambda x: x["Amplitude"]
-            )
+        from collections import defaultdict
+        from scipy import signal, ndimage
 
-            # Create dict for every channel and values with array of shape (n_events, 1, n_event_times)
-            for_tfrs = {
-                channel: np.expand_dims(
-                    np.array(
-                        events_df.groupby(level=1)
-                        .apply(lambda x: x.to_numpy())
-                        .tolist()
-                    ),
-                    axis=1,
-                )
-                for channel, events_df in df.groupby(level=0)
-            }
+        assert (
+            self.hypno.any()
+        ), f"Hypnogram hasn't been provided, can't compute PSD per stage"
 
-            # Calculate tfrs
-            if method == "morlet":
-                tfrs = {
-                    channel: mne.time_frequency.tfr_array_morlet(
-                        v,
-                        self.sf,
-                        freqs,
-                        n_jobs=n_jobs,
-                        output="avg_power",
-                        verbose="error",
-                        **kwargs,
-                    )
-                    for channel, v in tqdm(for_tfrs.items())
-                }
-            elif method == "multitaper":
-                tfrs = {
-                    channel: mne.time_frequency.tfr_array_multitaper(
-                        v,
-                        self.sf,
-                        freqs,
-                        n_jobs=n_jobs,
-                        output="avg_power",
-                        verbose="error",
-                        **kwargs,
-                    )
-                    for channel, v in tqdm(for_tfrs.items())
-                }
-            # Sort and combine
-            data = np.squeeze(
-                np.array([tfr for channel, tfr in natsorted(tfrs.items())])
+        method_args = method_args or dict()
+        method_args["axis"] = 1
+        if "nperseg" not in method_args:
+            method_args["nperseg"] = self.sf * 4.096
+        # Import data from the raw mne file.
+        self.mne_raw.load_data()
+        if avg_ref:
+            data = (
+                self.mne_raw.copy()
+                .set_eeg_reference()
+                .get_data(picks=picks, units="uV", reject_by_annotation="NaN")
             )
-            if data.ndim == 2:
-                data = np.expand_dims(data, axis=0)
-            self.tfrs[sleep_stages[stage]] = mne.time_frequency.AverageTFR(
-                info=self.mne_raw.copy().pick(list(tfrs.keys())).info,
-                data=data,
-                times=np.linspace(
-                    -time_before,
-                    time_after,
-                    int((time_before + time_after) * self.sf + 1),
-                ),
-                freqs=freqs,
-                nave=np.mean([arr.shape[0] for arr in for_tfrs.values()], dtype=int),
+        else:
+            data = self.mne_raw.get_data(
+                picks=picks, units="uV", reject_by_annotation="NaN"
             )
+        data = np.ma.array(data, mask=np.isnan(data))
+        n_samples_total = np.ma.compress_cols(data).shape[1]
+        psds = defaultdict(list)
+        psd_per_stage = {}
+        for stage, index in sleep_stages.items():
+            weights = []
+            n_samples = 0
+            try:
+                regions = ndimage.find_objects(
+                    ndimage.label(
+                        np.logical_or.reduce([self.hypno_up == i for i in index])
+                    )[0]
+                )
+            except TypeError:
+                regions = ndimage.find_objects(ndimage.label(self.hypno_up == index)[0])
+            for region in regions:
+                compressed = np.ma.compress_cols(data[:, region[0]])
+                if compressed.size > method_args["nperseg"]:
+                    weights.append(compressed.shape[1])
+                    freqs, psd = signal.welch(
+                        compressed,
+                        fs=self.sf,
+                        **method_args,
+                    )
+                    psds[stage].append(psd)
+                    n_samples += compressed.shape[1]
+            avg = np.average(np.array(psds[stage]), weights=weights, axis=0)
+            psd_per_stage[stage] = [
+                freqs,
+                10 * np.log10(avg) if dB else avg,
+                round(n_samples / n_samples_total * 100, 2),
+            ]
+        return psd_per_stage
 
+    def __plot_hypnospectrogram(
+        self, data, sf, hypno, win_sec, fmin, fmax, trimperc, cmap, overlap
+    ):
+        """
+        ?
+        """
+        # Increase font size while preserving original
+        old_fontsize = plt.rcParams["font.size"]
+        plt.rcParams.update({"font.size": 18})
+
+        if overlap or not hypno.any():
+            fig, ax = plt.subplots(nrows=1, figsize=(12, 4))
+            im = self.__plot_spectrogram(
+                data, sf, win_sec, fmin, fmax, trimperc, cmap, ax
+            )
+            if hypno.any():
+                ax_hypno = ax.twinx()
+                self.__plot_hypnogram(sf, hypno, ax_hypno)
+            # Add colorbar
+            cbar = fig.colorbar(
+                im, ax=ax, shrink=0.95, fraction=0.1, aspect=25, pad=0.1
+            )
+            cbar.ax.set_ylabel("Log Power (dB / Hz)", rotation=90, labelpad=20)
+            # Revert font-size
+            plt.rcParams.update({"font.size": old_fontsize})
+            return fig
+
+        fig, (ax0, ax1) = plt.subplots(
+            nrows=2, figsize=(12, 6), gridspec_kw={"height_ratios": [1, 2]}
+        )
+        plt.subplots_adjust(hspace=0.1)
+
+        # Hypnogram (top axis)
+        self.__plot_hypnogram(sf, hypno, ax0)
+        # Spectrogram (bottom axis)
+        self.__plot_spectrogram(data, sf, win_sec, fmin, fmax, trimperc, cmap, ax1)
+        # Revert font-size
+        plt.rcParams.update({"font.size": old_fontsize})
+        return fig
+
+    @staticmethod
+    def __plot_hypnogram(sf, hypno, ax0):
+        from pandas import Series
+
+        hypno = np.asarray(hypno).astype(int)
+        t_hyp = np.arange(hypno.size) / (sf * 3600)
+        # Make sure that REM is displayed after Wake
+        hypno = Series(hypno).map({-2: -2, -1: -1, 0: 0, 1: 2, 2: 3, 3: 4, 4: 1}).values
+        # Hypnogram (top axis)
+        ax0.step(t_hyp, -1 * hypno, color="k")
+        if -2 in hypno and -1 in hypno:
+            # Both Unscored and Artefacts are present
+            ax0.set_yticks([2, 1, 0, -1, -2, -3, -4])
+            ax0.set_yticklabels(["Uns", "Art", "W", "R", "N1", "N2", "N3"])
+            ax0.set_ylim(-4.5, 2.5)
+        elif -2 in hypno and -1 not in hypno:
+            # Only Unscored are present
+            ax0.set_yticks([2, 0, -1, -2, -3, -4])
+            ax0.set_yticklabels(["Uns", "W", "R", "N1", "N2", "N3"])
+            ax0.set_ylim(-4.5, 2.5)
+
+        elif -2 not in hypno and -1 in hypno:
+            # Only Artefacts are present
+            ax0.set_yticks([1, 0, -1, -2, -3, -4])
+            ax0.set_yticklabels(["Art", "W", "R", "N1", "N2", "N3"])
+            ax0.set_ylim(-4.5, 1.5)
+        else:
+            # No artefacts or Unscored
+            ax0.set_yticks([0, -1, -2, -3, -4])
+            ax0.set_yticklabels(["W", "R", "N1", "N2", "N3"])
+            ax0.set_ylim(-4.5, 0.5)
+        ax0.set_xlim(0, t_hyp.max())
+        ax0.set_ylabel("Stage")
+        ax0.xaxis.set_visible(False)
+        ax0.spines["right"].set_visible(False)
+        ax0.spines["top"].set_visible(False)
+        return ax0
+
+    @staticmethod
+    def __plot_spectrogram(data, sf, win_sec, fmin, fmax, trimperc, cmap, ax):
+        from matplotlib.colors import Normalize
+        from lspopt import spectrogram_lspopt
+        import numpy as np
+
+        # Calculate multi-taper spectrogram
+        nperseg = int(win_sec * sf)
+        f, t, Sxx = spectrogram_lspopt(data, sf, nperseg=nperseg, noverlap=0)
+        Sxx = 10 * np.log10(
+            Sxx, out=np.full(Sxx.shape, np.nan), where=(Sxx != 0)
+        )  # Convert uV^2 / Hz --> dB / Hz
+
+        # Select only relevant frequencies (up to 30 Hz)
+        good_freqs = np.logical_and(f >= fmin, f <= fmax)
+        Sxx = Sxx[good_freqs, :]
+        f = f[good_freqs]
+        t /= 3600  # Convert t to hours
+
+        # Normalization
+        vmin, vmax = np.nanpercentile(Sxx, [0 + trimperc, 100 - trimperc])
+        norm = Normalize(vmin=vmin, vmax=vmax)
+        im = ax.pcolormesh(
+            t, f, Sxx, norm=norm, cmap=cmap, antialiased=True, shading="auto"
+        )
+        ax.set_xlim(0, t.max())
+        ax.set_ylabel("Frequency [Hz]")
+        ax.set_xlabel("Time [hrs]")
+        return im
+
+
+@define(kw_only=True)
+class SpindlesPipe(BaseEventPipe):
+    """Spindles detection."""
 
-@define(kw_only=True, slots=False)
-class BaseSpectrum(ABC):
-    """A template class for the spectral analysis."""
-
-    psd_per_stage: dict = field(init=False)
-    """ Dictionary of the form sleep_stage:[freqs array with shape (n_freqs), 
-    psd array with shape (n_electrodes, n_freqs), 
-    sleep_stage percent from the whole unrejected data]
-    """
-
-    def plot_psd_per_stage(
+    def detect(
         self,
-        picks: str | Iterable[str] = ("E101",),
-        sec_per_seg: float = 4.096,
-        psd_range: tuple = (-40, 60),
-        freq_range: tuple = (0, 40),
-        xscale: str = "linear",
-        sleep_stages: dict = {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4},
-        axis: plt.axis = None,
+        picks: str | Iterable[str] = ("eeg"),
+        include: Iterable[int] = (1, 2, 3),
+        freq_sp: Iterable[float] = (12, 15),
+        freq_broad: Iterable[float] = (1, 30),
+        duration: Iterable[float] = (0.5, 2),
+        min_distance: int = 500,
+        thresh: dict = {"corr": 0.65, "rel_pow": 0.2, "rms": 1.5},
+        multi_only: bool = False,
+        remove_outliers: bool = False,
+        verbose: bool = False,
         save: bool = False,
     ):
-        """Plot PSD per sleep stage.
-
-        Args:
-            picks: Channels to calculate PSD on, more info at
-                `mne.io.Raw.get_data <https://mne.tools/stable/generated/
-                mne.io.Raw.html#mne.io.Raw.get_data>`_.
-                Defaults to ("E101",).
-            sec_per_seg: Welch segment length in seconds. Defaults to 4.096.
-            psd_range: Range of y axis on PSD plot. Defaults to (-40, 60).
-            freq_range: Range of x axis on PSD plot. Defaults to (0, 40).
-            xscale: Scale of the X axis, check available values at
-                `matplotlib.axes.Axes.set_xscale <https://mne.tools/stable/
-                generated/mne.io.Raw.html#mne.io.Raw.get_data>`_.
-                Defaults to "linear".
-            sleep_stages: Mapping between sleep stages names and their integer representations.
-                Defaults to {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4}.
-            axis: Instance of `matplotlib.pyplot.axis <https://matplotlib.org/
-                stable/api/_as_gen/matplotlib.pyplot.axis.html#matplotlib-pyplot-axis>`_.
-                Defaults to None.
-            save: Whether to save the figure. Defaults to False.
+        """Wrapper around YASA's `spindles_detect <https://raphaelvallat.com/
+        yasa/build/html/generated/yasa.spindles_detect.html>`_.
         """
+        from yasa import spindles_detect
 
-        is_new_axis = False
-
-        if not axis:
-            fig, axis = plt.subplots()
-            is_new_axis = True
-
-        psd_per_stage = self._compute_psd_per_stage(
-            picks=picks,
-            sleep_stages=sleep_stages,
-            sec_per_seg=sec_per_seg,
-            avg_ref=False,
-            dB=True,
+        self.results = spindles_detect(
+            data=self.mne_raw.copy().load_data().set_eeg_reference().pick(picks),
+            hypno=self.hypno_up,
+            verbose=verbose,
+            include=include,
+            freq_sp=freq_sp,
+            freq_broad=freq_broad,
+            duration=duration,
+            min_distance=min_distance,
+            thresh=thresh,
+            multi_only=multi_only,
+            remove_outliers=remove_outliers,
         )
+        if save:
+            self._save_to_csv()
 
-        for stage in sleep_stages:
-            axis.plot(
-                psd_per_stage[stage][0],
-                psd_per_stage[stage][1][0],
-                label=f"{stage} ({psd_per_stage[stage][2]}%)",
-            )
 
-        axis.set_xlim(freq_range)
-        axis.set_ylim(psd_range)
-        axis.set_xscale(xscale)
-        axis.set_title("Welch's PSD")
-        axis.set_ylabel("PSD [dB/Hz]")
-        axis.set_xlabel(f"{xscale} frequency [Hz]".capitalize())
-        axis.legend()
-        # Save the figure if 'save' set to True and no axis has been passed.
-        if save and is_new_axis:
-            fig.savefig(self.output_dir / f"psd.png")
+@define(kw_only=True)
+class SlowWavesPipe(BaseEventPipe):
+    """Slow waves detection."""
 
-    def plot_topomap_per_stage(
+    def detect(
         self,
-        stage: str = "REM",
-        band: dict = {"Delta": (0, 4)},
-        sec_per_seg: float = 4.096,
-        dB: bool = False,
-        sleep_stages: dict = {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4},
-        axis: plt.axis = None,
-        fooof: bool = False,
-        cmap: str = "plasma",
+        picks: str | Iterable[str] = ("eeg"),
+        include: Iterable[int] = (1, 2, 3),
+        freq_sw: Iterable[float] = (0.3, 1.5),
+        dur_neg: Iterable[float] = (0.3, 1.5),
+        dur_pos: Iterable[float] = (0.1, 1),
+        amp_neg: Iterable[float] = (40, 200),
+        amp_pos: Iterable[float] = (10, 150),
+        amp_ptp: Iterable[float] = (75, 350),
+        coupling: bool = False,
+        coupling_params: dict = {"freq_sp": (12, 16), "p": 0.05, "time": 1},
+        remove_outliers: bool = False,
         save: bool = False,
     ):
-        """Plots topomap for a sleep stage and a frequency band.
-
-        Args:
-            stage: One of the sleep_stages keys. Defaults to "REM".
-            band: Name-value pair - with name=arbitrary name
-                and value=(l_freq, h_freq).
-                Defaults to {"Delta": (0, 4)}.
-            sec_per_seg: Welch segment length in seconds. Defaults to 4.096.
-            dB: Whether transform PSD to dB. Defaults to False.
-            sleep_stages: Mapping between sleep stages names and their integer representations.
-                Defaults to {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4}.
-            axis: Instance of `matplotlib.pyplot.axis <https://matplotlib.org/
-                stable/api/_as_gen/matplotlib.pyplot.axis.html#matplotlib-pyplot-axis>`_.
-                Defaults to None.
-            fooof: Whether to plot parametrised spectra.
-                More at `fooof <https://fooof-tools.github.io/fooof/auto_examples/analyses/
-                plot_mne_example.html#sphx-glr-auto-examples-analyses-plot-mne-example-py>`_.
-                Defaults to False.
-            cmap: Matplotlib `colormap <https://matplotlib.org/stable/tutorials/colors/colormaps.html>`_.
-                Defaults to "plasma".
-            save: Whether to save the figure. Defaults to False.
+        """Wrapper around YASA's `sw_detect <https://raphaelvallat.com/yasa/
+        build/html/generated/yasa.sw_detect.html>`_.
         """
-        from mne.viz import plot_topomap
+        from yasa import sw_detect
 
-        if not hasattr(self, "psd_per_stage") or stage not in self.psd_per_stage.keys():
-            assert (
-                stage in sleep_stages.keys()
-            ), f"sleep_stages should contain provided stage"
-
-        is_new_axis = False
-
-        if axis is None:
-            fig, axis = plt.subplots()
-            is_new_axis = True
-
-        if not hasattr(self, "psd_per_stage") or stage not in self.psd_per_stage.keys():
-            self.psd_per_stage = self._compute_psd_per_stage(
-                picks=["eeg"],
-                sleep_stages=sleep_stages,
-                sec_per_seg=sec_per_seg,
-                avg_ref=True,
-                dB=dB,
-            )
+        self.results = sw_detect(
+            data=self.mne_raw.copy().load_data().set_eeg_reference().pick(picks),
+            hypno=self.hypno_up,
+            verbose=False,
+            include=include,
+            freq_sw=freq_sw,
+            dur_neg=dur_neg,
+            dur_pos=dur_pos,
+            amp_neg=amp_neg,
+            amp_pos=amp_pos,
+            amp_ptp=amp_ptp,
+            coupling=coupling,
+            coupling_params=coupling_params,
+            remove_outliers=remove_outliers,
+        )
+        if save:
+            self._save_to_csv()
 
-        [(k, b)] = band.items()
 
-        if fooof:
-            from fooof import FOOOFGroup
-            from fooof.bands import Bands
-            from fooof.analysis import get_band_peak_fg
-
-            # Initialize a FOOOFGroup object, with desired settings
-            fg = FOOOFGroup(
-                peak_width_limits=[1, 6],
-                min_peak_height=0.15,
-                peak_threshold=2.0,
-                max_n_peaks=6,
-                verbose=False,
-            )
+@define(kw_only=True)
+class REMsPipe(BaseEventPipe):
+    """Rapid eye movements detection."""
 
-            # Define the frequency range to fit
-            freq_range = [1, 45]
+    def detect(
+        self,
+        loc_chname: str = "E46",
+        roc_chname: str = "E238",
+        include: int | Iterable[int] = 4,
+        freq_rem: Iterable[float] = (0.5, 5),
+        duration: Iterable[float] = (0.3, 1.2),
+        amplitude: Iterable[float] = (50, 325),
+        remove_outliers: bool = False,
+        save: bool = False,
+    ):
+        """Wrapper around YASA's `rem_detect <https://raphaelvallat.com/yasa/
+        build/html/generated/yasa.rem_detect.html>`_.
+        """
+        from yasa import rem_detect
 
-            fg.fit(
-                self.psd_per_stage[stage][0],
-                self.psd_per_stage[stage][1],
-                freq_range=freq_range,
-            )
+        referenced = self.mne_raw.copy().load_data().set_eeg_reference()
+        loc = referenced.get_data([loc_chname], units="uV", reject_by_annotation="NaN")
+        roc = referenced.get_data([roc_chname], units="uV", reject_by_annotation="NaN")
+        self.results = rem_detect(
+            loc=loc,
+            roc=roc,
+            sf=self.sf,
+            hypno=self.hypno_up,
+            verbose=False,
+            include=include,
+            freq_rem=freq_rem,
+            duration=duration,
+            amplitude=amplitude,
+            remove_outliers=remove_outliers,
+        )
+        if save:
+            self._save_to_csv()
 
-            # Define frequency bands of interest
-            bands = Bands(band)
+    def plot_average(self, save=False, yasa_args=None):
+        yasa_args = yasa_args or dict()
+        self.results.plot_average(**yasa_args)
+        if save:
+            self._save_avg_fig()
 
-            # Extract peaks
-            peaks = get_band_peak_fg(fg, bands[list(band)[0]])
+    def plot_topomap(self):
+        raise AttributeError("'REMsPipe' object has no attribute 'plot_topomap'")
 
-            peaks[np.where(np.isnan(peaks))] = 0
-            # Extract the power values from the detected peaks
-            psds = peaks[:, 1]
+    def plot_topomap_collage(self):
+        raise AttributeError("'REMsPipe' object has no attribute 'plot_topomap'")
 
-        else:
-            psds = np.take(
-                self.psd_per_stage[stage][1],
-                np.where(
-                    np.logical_and(
-                        self.psd_per_stage[stage][0] >= b[0],
-                        self.psd_per_stage[stage][0] <= b[1],
-                    )
-                )[0],
-                axis=1,
-            ).sum(axis=1)
 
-        im, cn = plot_topomap(
-            psds, self.mne_raw.info, size=5, cmap=cmap, axes=axis, show=False
-        )
+@define(kw_only=True)
+class CombinedPipe(BaseSpectrum):
+    """The pipeline element combining results from multiple subjects.
 
-        # divider = make_axes_locatable(axis)
-        # cax = divider.append_axes('right', size='5%', pad=0.05)
-        plt.colorbar(
-            im,
-            ax=axis,
-            orientation="vertical",
-            shrink=0.6,
-            label="dB/Hz" if dB else r"$\mu V^{2}/Hz$",
-        )
+    Contains methods for computing and plotting combined PSD,
+    spectrogram and topomaps, per sleep stage.
+    """
 
-        if is_new_axis:
-            fig.suptitle(f"{stage} ({b[0]}-{b[1]} Hz)")
-        if save and is_new_axis:
-            fig.savefig(self.output_dir / f"topomap_{list(band)[0]}.png")
+    pipes: Iterable[BaseHypnoPipe] = field()
+    """Stores pipeline elements for multiple subjects.
+    """
 
-    def plot_topomap_collage(
-        self,
-        stages_to_plot: tuple = "all",
-        bands: dict = {
-            "Delta": (0, 3.99),
-            "Theta": (4, 7.99),
-            "Alpha": (8, 12.49),
-            "SMR": (12.5, 15),
-            "Beta": (12.5, 29.99),
-            "Gamma": (30, 60),
-        },
-        sec_per_seg: float = 4.096,
-        dB: bool = False,
-        sleep_stages: dict = {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4},
-        fooof: bool = False,
-        cmap: str = "plasma",
-        save: bool = False,
-    ):
-        """Plots topomap collage for multiple sleep stages and bands.
+    mne_raw: mne.io.Raw = field(init=False)
 
-        Args:
-            stages_to_plot: Tuple of strings representing names from sleep_stages,
-                e.g., ("REM", "N1").
-                If set to "all" plots every stage provided in sleep_stages.
-                Defaults to "all".
-            bands: Dict of name-value pairs - with name=arbitrary name
-                and value=(l_freq, h_freq).
-                Defaults to { "Delta": (0, 3.99), "Theta": (4, 7.99), "Alpha": (8, 12.49),
-                "SMR": (12.5, 15), "Beta": (12.5, 29.99), "Gamma": (30, 60), }.
-            sec_per_seg: Welch segment length in seconds.. Defaults to 4.096.
-            dB: Whether transform PSD to dB. Defaults to False.
-            sleep_stages: Mapping between sleep stages names and their integer representations.
-                Defaults to {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4}.
-            fooof: Whether to plot parametrised spectra.
-                More at `fooof <https://fooof-tools.github.io/fooof/auto_examples/analyses/
-                plot_mne_example.html#sphx-glr-auto-examples-analyses-plot-mne-example-py>`_.
-                Defaults to False. Defaults to False.
-            cmap: Matplotlib `colormap <https://matplotlib.org/stable/tutorials/colors/colormaps.html>`_.
-                Defaults to "plasma".
-            save: Whether to save the figure. Defaults to False.
-        """
-        if stages_to_plot == "all":
-            stages_to_plot = sleep_stages.keys()
-        n_rows = len(stages_to_plot)
-        n_cols = len(bands)
-
-        fig = plt.figure(figsize=(n_cols * 4, n_rows * 4), layout="constrained")
-        subfigs = fig.subfigures(n_rows, 1)
-
-        for row_index, stage in enumerate(stages_to_plot):
-            axes = subfigs[row_index].subplots(1, n_cols)
-
-            for col_index, band_key in enumerate(bands):
-                self.plot_topomap_per_stage(
-                    stage=stage,
-                    band={band_key: bands[band_key]},
+    @mne_raw.default
+    def _get_mne_raw_from_pipe(self):
+        return self.pipes[0].mne_raw
+
+    def _compute_psd_per_stage(self, picks, sleep_stages, sec_per_seg, avg_ref, dB):
+        psd_per_stage = {}
+        psds = []
+        for pipe in self.pipes:
+            psds.append(
+                pipe._compute_psd_per_stage(
+                    picks=picks,
+                    sleep_stages=sleep_stages,
                     sec_per_seg=sec_per_seg,
+                    avg_ref=avg_ref,
                     dB=dB,
-                    sleep_stages=sleep_stages,
-                    axis=axes[col_index],
-                    cmap=cmap,
-                    fooof=fooof,
-                )
-                axes[col_index].set_title(
-                    f"{band_key} ({bands[band_key][0]}-{bands[band_key][1]} Hz)"
                 )
-
-            subfigs[row_index].suptitle(
-                f"{stage} ({self.psd_per_stage[stage][2]}%)", fontsize="xx-large"
             )
 
-        if save:
-            fig.savefig(self.output_dir / f"topomap_collage.png")
-
-    @abstractmethod
-    def _compute_psd_per_stage(self):
-        pass
+        for stage in sleep_stages:
+            psd_per_stage[stage] = [
+                psds[0][stage][0],
+                np.sum([psd[stage][1] for psd in psds], axis=0) / len(self.pipes),
+                round(sum([psd[stage][2] for psd in psds]) / len(self.pipes), 2),
+            ]
+        return psd_per_stage
```

### Comparing `sleepeeg-0.0.1/sleepeeg.egg-info/PKG-INFO` & `sleepeeg-0.1.1/sleepeeg.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: sleepeeg
-Version: 0.0.1
+Version: 0.1.1
 Summary: Sleep EEG preprocessing and analysis
 Author-email: Gennadiy Belonosov <gennadiyb@mail.tau.ac.il>
 License: MIT
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sleep-eeg-processing
 **sleepeeg** is a high-level API built on top of [mne-python](https://mne.tools/stable/index.html) for preprocessing and analysis of sleep EEG data.
 ## Installation
 0. Make sure you have [Python](https://www.python.org/downloads/) installed.
     - The script was tested with the version 3.10.9
     - Python 3.11.x currently isn't supported because of the yasa's dependency on the numba library.
-1. Create a python environment
+1. Create a Python virtual environment, for more info you can refer to python [venv](https://docs.python.org/3/tutorial/venv.html), [virtualenv](https://virtualenv.pypa.io/en/latest/user_guide.html) or [conda](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).
 2. Activate the environment
 3. 
     ```
     pip install sleepeeg
     ```
 4. (Optional, but recommended) [Download](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/NirLab-TAU/sleep-eeg-processing/tree/main/notebooks) notebooks.
-5. (Optional, but recommended) Prepare [GPU acceleration](https://mne.tools/stable/install/advanced.html#gpu-acceleration-with-cuda) by installing [CUDA](https://developer.nvidia.com/cuda-downloads) and [CuPy](https://cupy.dev/).
+5. (Optional, but recommended) Prepare [GPU acceleration](https://mne.tools/stable/install/advanced.html#gpu-acceleration-with-cuda) by installing [CUDA](https://developer.nvidia.com/cuda-downloads) and [CuPy](https://cupy.dev/). After installation, to permanently enable CUDA use, do: 
+    ```
+    mne.utils.set_config('MNE_USE_CUDA', 'true')
+    ```
 6. (Optional) For OpenGL acceleration of [MNE plot](https://mne.tools/stable/generated/mne.io.Raw.html#mne.io.Raw.plot) install [pyopengl](https://pyopengl.sourceforge.net/documentation/installation.html) and use `plot(use_opengl=True)`.
 
 ## Quickstart
 1. Open any of the downloaded notebooks using the created environment.
 2. Follow the notebook's instructions.
```

