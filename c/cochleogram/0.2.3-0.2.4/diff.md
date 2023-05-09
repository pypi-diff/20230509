# Comparing `tmp/cochleogram-0.2.3.tar.gz` & `tmp/cochleogram-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cochleogram-0.2.3.tar", last modified: Thu Apr 27 22:30:52 2023, max compression
+gzip compressed data, was "cochleogram-0.2.4.tar", last modified: Tue May  9 20:47:45 2023, max compression
```

## Comparing `cochleogram-0.2.3.tar` & `cochleogram-0.2.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:30:52.510623 cochleogram-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:30:52.502623 cochleogram-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:30:52.506623 cochleogram-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-27 22:30:41.000000 cochleogram-0.2.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-27 22:30:41.000000 cochleogram-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-27 22:30:52.510623 cochleogram-0.2.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:30:52.506623 cochleogram-0.2.3/cochleogram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/gui.enaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:30:52.510623 cochleogram-0.2.3/cochleogram/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/icons/cells.png
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/icons/exclude.png
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/icons/main-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/icons/make_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/icons/spiral.png
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/icons/tile.png
--rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    20794 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    26607 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/presenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 22:30:52.000000 cochleogram-0.2.3/cochleogram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:30:52.506623 cochleogram-0.2.3/cochleogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-27 22:30:52.000000 cochleogram-0.2.3/cochleogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-27 22:30:52.000000 cochleogram-0.2.3/cochleogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 22:30:52.000000 cochleogram-0.2.3/cochleogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-27 22:30:52.000000 cochleogram-0.2.3/cochleogram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-27 22:30:52.000000 cochleogram-0.2.3/cochleogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 22:30:52.000000 cochleogram-0.2.3/cochleogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 22:30:41.000000 cochleogram-0.2.3/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-27 22:30:41.000000 cochleogram-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-27 22:30:41.000000 cochleogram-0.2.3/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 22:30:52.510623 cochleogram-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:47:45.228226 cochleogram-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:47:45.224225 cochleogram-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:47:45.224225 cochleogram-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-09 20:47:35.000000 cochleogram-0.2.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-09 20:47:35.000000 cochleogram-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-09 20:47:45.228226 cochleogram-0.2.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:47:45.224225 cochleogram-0.2.4/cochleogram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/gui.enaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:47:45.228226 cochleogram-0.2.4/cochleogram/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/icons/cells.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/icons/exclude.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/icons/main-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/icons/make_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/icons/spiral.png
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/icons/tile.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26608 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/presenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 20:47:45.000000 cochleogram-0.2.4/cochleogram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:47:45.228226 cochleogram-0.2.4/cochleogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-09 20:47:45.000000 cochleogram-0.2.4/cochleogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-09 20:47:45.000000 cochleogram-0.2.4/cochleogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:47:45.000000 cochleogram-0.2.4/cochleogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-09 20:47:45.000000 cochleogram-0.2.4/cochleogram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-09 20:47:45.000000 cochleogram-0.2.4/cochleogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 20:47:45.000000 cochleogram-0.2.4/cochleogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-09 20:47:35.000000 cochleogram-0.2.4/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-09 20:47:35.000000 cochleogram-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-09 20:47:35.000000 cochleogram-0.2.4/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 20:47:45.228226 cochleogram-0.2.4/setup.cfg
```

### Comparing `cochleogram-0.2.3/.github/workflows/publish-to-pypi.yml` & `cochleogram-0.2.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.3/.gitignore` & `cochleogram-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.3/PKG-INFO` & `cochleogram-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.2.3
+Version: 0.2.4
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.2.3/cochleogram/gui.enaml` & `cochleogram-0.2.4/cochleogram/gui.enaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
                                HGroup, Html, Label, MainWindow, Menu, MenuBar,
                                MPLCanvas, ObjectCombo, ProgressBar, PushButton,
                                Slider, Window)
 
 from cochleogram import plot, util
 from cochleogram.model import Cochlea
 from cochleogram.presenter import Presenter
-from cochleogram import reader
+from cochleogram import readers
 
 
 def load_icon(name):
     data = resources.files('cochleogram.icons').joinpath(f'{name}.png').read_bytes()
     img = Image(data=data)
     icg = IconImage(image=img)
     return Icon(images=[icg])
@@ -44,41 +44,42 @@
         q = 'There are unsaved changes. Your current analysis will be lost. Are you sure?'
         button = question(None, 'Confirm action', q)
         if button is None or button.text == 'No':
             return
 
     path = FileDialogEx.get_existing_directory(window, current_path=window.current_path)
     if path:
-        load_processed_dataset(path, window, reader.ProcessedReader)
+        load_processed_dataset(path, window, readers.ProcessedReader)
 
 
 def open_20x_lif_file(window):
     # Check for unsaved changes
     if any(p.unsaved_changes for p in window.presenters):
         q = 'There are unsaved changes. Your current analysis will be lost. Are you sure?'
         button = question(None, 'Confirm action', q)
         if button is None or button.text == 'No':
             return
 
     path = FileDialogEx.get_open_file_name(window, current_path=window.current_path)
     if path:
-        load_processed_dataset(path, window, reader.LIFReader)
+        load_processed_dataset(path, window, readers.LIFReader)
 
 
 def load_processed_dataset(path, window, reader_class):
     workspace = window.find('dock_area')
     # Remove existing cochlea
     for p in window.presenters:
         remove_dock_item(workspace, p)
 
-    iface = reader_class(path)
+    reader = reader_class(path)
     # Now, load new cochlea
     window.current_path = path
-    window.cochlea = iface.load_cochlea()
-    window.presenters = [Presenter(p, iface) for p in window.cochlea.pieces]
+    window.cochlea = reader.load_cochlea()
+    window.reader = reader
+    window.presenters = [Presenter(p, reader) for p in window.cochlea.pieces]
     target = 'help'
     for p in window.presenters:
         try:
             p.load_state()
         except IOError:
             pass
         target = add_dock_item(workspace, p, target)
@@ -414,14 +415,15 @@
                 window.close()
 
 
 enamldef CompositeWindow(Window):
 
     modality = 'application_modal'
     title = 'Generate Composite'
+    attr reader
     attr cochlea
     attr channels = cochlea.channel_names
 
     Container:
         CheckBox: include_freq_map:
             text = 'Include frequency map?'
             visible << cochlea.ihc_spiral_complete()
@@ -443,29 +445,32 @@
                         channels.remove(loop_item)
 
         PushButton:
             text = 'Generate'
             enabled << len(channels) != 0
             clicked ::
                 try:
-                    fig = plot.plot_composite(cochlea, include_freq_map=include_freq_map.checked)
-                    fig.suptitle(cochlea.name)
-                    fig.savefig(cochlea.path / f'{cochlea.name}_frequency_map.pdf')
+                    fig = plot.plot_composite(cochlea,
+                                              include_freq_map=include_freq_map.checked,
+                                              channels=channels)
+                    fig.suptitle(reader.get_name())
+                    reader.save_figure(fig, 'frequency_map')
                     information(self, 'Composite', 'Composite has been generated.')
                 except Exception as e:
                     log.exception(e)
                     critical(self, 'Composite', str(e))
 
 
 enamldef CochleagramWindow(MainWindow): window:
 
     initial_size = (900, 900)
     title = 'Cochelogram'
     icon = load_icon('main-icon')
 
+    attr reader
     attr cochlea
     attr presenters = []
     attr current_path = ''
 
     MenuBar:
         Menu:
             title = '&File'
@@ -515,15 +520,15 @@
             Action:
                 separator = True
 
             Action:
                 text = 'Generate composite (frequency map)\tCtrl+F'
                 enabled << cochlea is not None
                 triggered ::
-                    window = CompositeWindow(cochlea=cochlea)
+                    window = CompositeWindow(cochlea=cochlea, reader=reader)
                     window.show()
 
     initialized ::
         for presenter in presenters:
             deferred_call(add_dock_item, workspace, presenter)
 
     closing ::
```

### Comparing `cochleogram-0.2.3/cochleogram/icons/cells.png` & `cochleogram-0.2.4/cochleogram/icons/cells.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.3/cochleogram/icons/exclude.png` & `cochleogram-0.2.4/cochleogram/icons/exclude.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.3/cochleogram/icons/main-icon.png` & `cochleogram-0.2.4/cochleogram/icons/main-icon.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.3/cochleogram/icons/make_icons.py` & `cochleogram-0.2.4/cochleogram/icons/make_icons.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.3/cochleogram/icons/spiral.png` & `cochleogram-0.2.4/cochleogram/icons/spiral.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.3/cochleogram/icons/tile.png` & `cochleogram-0.2.4/cochleogram/icons/tile.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.3/cochleogram/instructions.html` & `cochleogram-0.2.4/cochleogram/instructions.html`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.3/cochleogram/main.py` & `cochleogram-0.2.4/cochleogram/main.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.3/cochleogram/model.py` & `cochleogram-0.2.4/cochleogram/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,18 @@
         xv, yv, zv = self.info['voxel_size'][:3]
         xub = xlb + xpx * xv
         yub = ylb + ypx * yv
         zub = zlb + zpx * zv
         self.extent = [xlb, xub, ylb, yub, zlb, zub]
         self.n_channels = self.image.shape[-1]
 
+    @property
+    def channel_names(self):
+        return [c['name'] for c in self.info['channels']]
+
     def contains(self, x, y):
         contains_x = self.extent[0] <= x <= self.extent[1]
         contains_y = self.extent[2] <= y <= self.extent[3]
         return contains_x and contains_y
 
     def to_coords(self, x, y, z=None):
         lower = self.info["lower"]
@@ -346,32 +350,40 @@
         extent = self.get_image_extent()
         center = np.array(extent).reshape((2, 2)).mean(axis=1)
         return tuple(center)
 
     def get_rotation(self):
         return self.info.get('rotation', 0)
 
-    def get_image(self, channel=None, z_slice=None, axis='z',
+    def get_image(self, channels=None, z_slice=None, axis='z',
                   norm_percentile=99):
         if z_slice is None:
             data = self.image.max(axis='xyz'.index(axis))
         else:
             data = self.image[:, :, z_slice, :]
 
+        if channels is None or channels == 'All':
+            channels = self.channel_names
+        elif isinstance(channels, int):
+            raise ValueError('Must provide name for channel')
+        elif isinstance(channels, str):
+            channels = [channels]
+        elif len(channels) == 0:
+            raise ValueError('Cannot generate image with zero channels')
+        for c in channels:
+            if c not in self.channel_names:
+                raise ValueError(f'Channel {c} does not exist')
+
         x, y = data.shape[:2]
         image = []
         for c, c_info in enumerate(self.info['channels']):
-            if isinstance(channel, int):
-                raise ValueError('Must provide name for channel')
-            if channel is None or channel == 'All' or c_info['name'] == channel:
+            if c_info['name'] in channels:
                 color = CHANNEL_CONFIG[c_info['name']]['display_color']
                 rgb = colors.to_rgba(color)[:3]
                 image.append(data[..., c][..., np.newaxis] * rgb)
-        if len(image) == 0:
-            raise ValueError(f'Channel {channel} does not exist')
         image = np.concatenate([i[np.newaxis] for i in image]).max(axis=0)
         image_max =  np.percentile(image, norm_percentile, axis=(0, 1), keepdims=True)
         image_mask = image_max != 0
         return np.divide(image, image_max, where=image_mask).clip(0, 1)
 
     def get_state(self):
         return {"extent": self.extent}
@@ -426,15 +438,15 @@
         keys = 'IHC', 'OHC1', 'OHC2', 'OHC3', 'Extra'
         self.spirals = {k: Points() for k in keys}
         self.cells = {k: Points() for k in keys}
 
     @property
     def channel_names(self):
         # We assume that each tile has the same set of channels
-        return [c['name'] for c in self.tiles[0].info['channels']]
+        return self.tiles[0].channel_names
 
     def get_image_extent(self):
         extents = np.vstack([tile.get_image_extent() for tile in self.tiles])
         xmin = extents[:, 0].min()
         xmax = extents[:, 1].max()
         ymin = extents[:, 2].min()
         ymax = extents[:, 3].max()
```

### Comparing `cochleogram-0.2.3/cochleogram/plot.py` & `cochleogram-0.2.4/cochleogram/plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from matplotlib import pyplot as plt
 from matplotlib import patheffects as path_effects
 from matplotlib import transforms
+import numpy as np
 
 
-def _plot_piece(ax, piece, xo, yo, xmax, ymax, freq_map=None):
+def _plot_piece(ax, piece, xo, yo, xmax, ymax, freq_map=None, cells=None,
+                channels=None):
     tile = piece.merge_tiles()
-    img = tile.get_image()
+    img = tile.get_image(channels=channels)
     extent = tile.get_image_extent()
     xr = extent[0] - xo
     yr = extent[2] - yo
     xe = extent[1] - extent[0]
     ye = extent[3] - extent[2]
     extent = (xo, xo+xe, yo, yo+ye)
     t = tile.get_image_transform() + ax.transData
@@ -28,31 +30,40 @@
             ax.plot(x-xr, y-yr, 'ko', mec='w', mew=2)
             t = ax.annotate(f, (x-xr, y-yr), (5, 5), color='white', textcoords='offset points')
             t.set_path_effects([
                 path_effects.Stroke(linewidth=3, foreground='black'),
                 path_effects.Normal(),
             ])
 
+    if cells is not None:
+        for cell in cells:
+            x, y = piece.cells[cell].get_nodes()
+            x = np.subtract(x, xr)
+            y = np.subtract(y, yr)
+            ax.plot(x, y, 'w.')
+
     return xo, yo, xmax, ymax
 
 
-def plot_composite(cochlea, include_freq_map=True):
+def plot_composite(cochlea, include_freq_map=True, cells=None, channels=None):
     figure, ax = plt.subplots(1, 1, figsize=(11, 8.5))
     if include_freq_map:
         freq_map = cochlea.make_frequency_map()
     else:
         freq_map = None
 
     xo, yo = 0, 0
     xmax, ymax = 0, 0
     for piece in cochlea.pieces[:3]:
-        xo, yo, xmax, ymax = _plot_piece(ax, piece, xo, yo, xmax, ymax, freq_map)
+        xo, yo, xmax, ymax = _plot_piece(ax, piece, xo, yo, xmax, ymax,
+                                         freq_map, cells, channels)
     xo, yo = 0, ymax
     for piece in cochlea.pieces[3:]:
-        xo, yo, xmax, ymax = _plot_piece(ax, piece, xo, yo, xmax, ymax, freq_map)
+        xo, yo, xmax, ymax = _plot_piece(ax, piece, xo, yo, xmax, ymax,
+                                         freq_map, cells, channels)
     ax.set_facecolor('k')
     ax.axis([0, xmax, 0, ymax])
     ax.set_xticks([])
     ax.set_yticks([])
 
     figure.subplots_adjust(left=0.025, right=0.975, top=0.95, bottom=0.025)
     return figure
```

### Comparing `cochleogram-0.2.3/cochleogram/presenter.py` & `cochleogram-0.2.4/cochleogram/presenter.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
     def redraw_if_needed(self):
         if self.needs_redraw:
             self.redraw()
             self.needs_redraw = False
 
     def redraw(self, event=None):
         z_slice = None if self.display_mode == 'projection' else self.z_slice
-        image = self.tile.get_image(channel=self.display_channel,
+        image = self.tile.get_image(channels=self.display_channel,
                                     z_slice=z_slice).swapaxes(0, 1)
         self.artist.set_data(image)
         xlb, xub, ylb, yub = extent = self.tile.get_image_extent()[:4]
         self.artist.set_extent(extent)
         self.rectangle.set_bounds(xlb, ylb, xub-xlb, yub-ylb)
 
         t = self.tile.get_image_transform()
```

### Comparing `cochleogram-0.2.3/cochleogram/reader.py` & `cochleogram-0.2.4/cochleogram/readers.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     def load_cochlea(self):
         raise NotImplementedError
 
     def save_analysis(self, state, piece):
         raise NotImplementedError
 
-    def load_analysis(self, piece):
+    def load_analysis(self, cochlea):
         raise NotImplementedError
 
     def state_filename(self, piece):
         raise NotImplementedError
 
     def load_state(self, piece):
         state_filename = self.state_filename(piece)
@@ -35,14 +35,21 @@
         return json.loads(state_filename.read_text())
 
     def save_state(self, piece, state):
         state_filename = self.state_filename(piece)
         state_filename.parent.mkdir(exist_ok=True)
         state_filename.write_text(json.dumps(state, indent=4))
 
+    def get_name(self):
+        return self.path.stem
+
+    def save_figure(self, fig, suffix):
+        filename = self.save_path() / f'{self.get_name()}_{suffix}.pdf'
+        fig.savefig(filename)
+
 
 class LIFReader(Reader):
 
     def __init__(self, path):
         from readlif.reader import LifFile
         super().__init__(path)
         self.fh = LifFile(path)
@@ -89,17 +96,19 @@
 
         return model.Piece(tiles, piece)
 
     def load_cochlea(self):
         pieces = [self.load_piece(p, sn) for p, sn in self.list_pieces().items()]
         return model.Cochlea(pieces)
 
+    def save_path(self):
+        return self.path.parent / self.path.stem
+
     def state_filename(self, piece):
-        return self.path.parent / self.path.stem /  \
-            f'{self.path.stem}_piece_{piece.piece}_analysis.json'
+        return self.save_path() / f'{self.path.stem}_piece_{piece.piece}_analysis.json'
 
 
 class ProcessedReader(Reader):
 
     def list_pieces(self):
         p_piece = re.compile('.*piece_(\d+)\w?')
         pieces = []
@@ -145,7 +154,13 @@
 
     def load_cochlea(self):
         pieces = [self.load_piece(p) for p in self.list_pieces()]
         return model.Cochlea(pieces)
 
     def state_filename(self, piece):
         return self.path /  f'{self.path.stem}_piece_{piece.piece}_analysis.json'
+
+    def save_path(self):
+        return self.path
+
+    def state_filename(self, piece):
+        return self.save_path() / f'{self.path.stem}_piece_{piece.piece}_analysis.json'
```

### Comparing `cochleogram-0.2.3/cochleogram/util.py` & `cochleogram-0.2.4/cochleogram/util.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.3/cochleogram.egg-info/PKG-INFO` & `cochleogram-0.2.4/cochleogram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.2.3
+Version: 0.2.4
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.2.3/cochleogram.egg-info/SOURCES.txt` & `cochleogram-0.2.4/cochleogram.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 cochleogram/__init__.py
 cochleogram/gui.enaml
 cochleogram/instructions.html
 cochleogram/main.py
 cochleogram/model.py
 cochleogram/plot.py
 cochleogram/presenter.py
-cochleogram/reader.py
+cochleogram/readers.py
 cochleogram/util.py
 cochleogram/version.py
 cochleogram.egg-info/PKG-INFO
 cochleogram.egg-info/SOURCES.txt
 cochleogram.egg-info/dependency_links.txt
 cochleogram.egg-info/entry_points.txt
 cochleogram.egg-info/requires.txt
```

### Comparing `cochleogram-0.2.3/pyproject.toml` & `cochleogram-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.3/readme.rst` & `cochleogram-0.2.4/readme.rst`

 * *Files identical despite different names*

