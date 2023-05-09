# Comparing `tmp/particlespy-0.6.0.tar.gz` & `tmp/particlespy-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "particlespy-0.6.0.tar", last modified: Tue Jul 13 08:03:20 2021, max compression
+gzip compressed data, was "particlespy-0.6.2.tar", last modified: Tue May  9 09:42:11 2023, max compression
```

## Comparing `particlespy-0.6.0.tar` & `particlespy-0.6.2.tar`

### file list

```diff
@@ -1,29 +1,36 @@
-drwxrwxrwx   0        0        0        0 2021-07-13 08:03:20.869411 particlespy-0.6.0/
--rw-rw-rw-   0        0        0    35825 2020-03-16 10:41:46.000000 particlespy-0.6.0/LICENSE
--rw-rw-rw-   0        0        0     1328 2021-07-13 08:03:20.868409 particlespy-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      811 2021-07-13 07:52:01.000000 particlespy-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2021-07-13 08:03:20.841048 particlespy-0.6.0/particlespy/
--rw-rw-rw-   0        0        0       20 2021-07-13 07:52:01.000000 particlespy-0.6.0/particlespy/__init__.py
--rw-rw-rw-   0        0        0     2453 2021-07-13 07:52:08.000000 particlespy-0.6.0/particlespy/api.py
--rw-rw-rw-   0        0        0     1496 2021-07-13 07:52:08.000000 particlespy-0.6.0/particlespy/custom_kernels.py
--rw-rw-rw-   0        0        0     6684 2021-07-13 07:52:04.000000 particlespy-0.6.0/particlespy/find_zoneaxis.py
-drwxrwxrwx   0        0        0        0 2021-07-13 08:03:20.865323 particlespy-0.6.0/particlespy/parameters/
--rw-rw-rw-   0        0        0   786560 2021-07-13 07:52:04.000000 particlespy-0.6.0/particlespy/parameters/manual_mask.npy
--rw-rw-rw-   0        0        0     8720 2021-07-13 07:52:04.000000 particlespy-0.6.0/particlespy/parameters/parameters_current.hdf5
--rw-rw-rw-   0        0        0     8720 2021-07-13 07:52:04.000000 particlespy-0.6.0/particlespy/parameters/parameters_previous.hdf5
--rw-rw-rw-   0        0        0    19341 2021-07-13 07:52:04.000000 particlespy-0.6.0/particlespy/particle_analysis.py
--rw-rw-rw-   0        0        0     1076 2021-07-13 07:52:04.000000 particlespy-0.6.0/particlespy/particle_load.py
--rw-rw-rw-   0        0        0      836 2021-07-13 07:52:04.000000 particlespy-0.6.0/particlespy/particle_save.py
--rw-rw-rw-   0        0        0    12234 2021-07-13 07:52:04.000000 particlespy-0.6.0/particlespy/ptcl_class.py
--rw-rw-rw-   0        0        0     4589 2021-07-13 07:52:04.000000 particlespy-0.6.0/particlespy/radial_profile.py
--rw-rw-rw-   0        0        0    32031 2021-07-13 07:52:04.000000 particlespy-0.6.0/particlespy/seg_ui.py
--rw-rw-rw-   0        0        0    11531 2021-07-13 07:52:03.000000 particlespy-0.6.0/particlespy/segimgs.py
--rw-rw-rw-   0        0        0     4743 2021-07-13 07:52:03.000000 particlespy-0.6.0/particlespy/segptcls.py
-drwxrwxrwx   0        0        0        0 2021-07-13 08:03:20.856219 particlespy-0.6.0/particlespy.egg-info/
--rw-rw-rw-   0        0        0     1328 2021-07-13 08:03:20.000000 particlespy-0.6.0/particlespy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      652 2021-07-13 08:03:20.000000 particlespy-0.6.0/particlespy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-13 08:03:20.000000 particlespy-0.6.0/particlespy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2021-07-13 08:03:20.000000 particlespy-0.6.0/particlespy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-07-13 08:03:20.000000 particlespy-0.6.0/particlespy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-07-13 08:03:20.869411 particlespy-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1080 2021-07-13 07:52:03.000000 particlespy-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:42:11.063649 particlespy-0.6.2/
+-rw-rw-rw-   0        0        0    35825 2023-04-27 09:22:55.000000 particlespy-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0     1272 2023-05-09 09:42:11.062650 particlespy-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0      796 2023-05-09 09:41:37.000000 particlespy-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 09:42:11.004683 particlespy-0.6.2/particlespy/
+-rw-rw-rw-   0        0        0       20 2023-04-27 09:22:55.000000 particlespy-0.6.2/particlespy/__init__.py
+-rw-rw-rw-   0        0        0     2485 2023-05-09 09:41:37.000000 particlespy-0.6.2/particlespy/api.py
+-rw-rw-rw-   0        0        0     1496 2023-04-27 09:22:55.000000 particlespy-0.6.2/particlespy/custom_kernels.py
+-rw-rw-rw-   0        0        0     6684 2023-04-27 09:22:56.000000 particlespy-0.6.2/particlespy/find_zoneaxis.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:42:11.040062 particlespy-0.6.2/particlespy/parameters/
+-rw-rw-rw-   0        0        0   786560 2023-05-09 09:37:19.000000 particlespy-0.6.2/particlespy/parameters/manual_mask.npy
+-rw-rw-rw-   0        0        0     8720 2023-05-09 09:37:19.000000 particlespy-0.6.2/particlespy/parameters/parameters_current.hdf5
+-rw-rw-rw-   0        0        0     8720 2023-05-09 09:37:19.000000 particlespy-0.6.2/particlespy/parameters/parameters_previous.hdf5
+-rw-rw-rw-   0        0        0    19340 2023-05-09 09:41:37.000000 particlespy-0.6.2/particlespy/particle_analysis.py
+-rw-rw-rw-   0        0        0     1076 2023-04-27 09:22:56.000000 particlespy-0.6.2/particlespy/particle_load.py
+-rw-rw-rw-   0        0        0      836 2023-04-27 09:22:56.000000 particlespy-0.6.2/particlespy/particle_save.py
+-rw-rw-rw-   0        0        0    12234 2023-04-27 09:22:56.000000 particlespy-0.6.2/particlespy/ptcl_class.py
+-rw-rw-rw-   0        0        0     4609 2023-04-27 09:23:49.000000 particlespy-0.6.2/particlespy/radial_profile.py
+-rw-rw-rw-   0        0        0    32185 2023-04-27 09:23:49.000000 particlespy-0.6.2/particlespy/seg_ui.py
+-rw-rw-rw-   0        0        0    11531 2023-04-27 09:22:56.000000 particlespy-0.6.2/particlespy/segimgs.py
+-rw-rw-rw-   0        0        0     4820 2023-05-09 09:41:37.000000 particlespy-0.6.2/particlespy/segptcls.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:42:11.061655 particlespy-0.6.2/particlespy/tests/
+-rw-rw-rw-   0        0        0       20 2023-05-09 09:41:37.000000 particlespy-0.6.2/particlespy/tests/__init__.py
+-rw-rw-rw-   0        0        0     2380 2023-05-09 09:41:37.000000 particlespy-0.6.2/particlespy/tests/generate_test_data.py
+-rw-rw-rw-   0        0        0     6208 2023-05-09 09:41:37.000000 particlespy-0.6.2/particlespy/tests/test_particle_analysis.py
+-rw-rw-rw-   0        0        0     3380 2023-05-09 09:41:37.000000 particlespy-0.6.2/particlespy/tests/test_particle_clustering.py
+-rw-rw-rw-   0        0        0      742 2023-05-09 09:41:37.000000 particlespy-0.6.2/particlespy/tests/test_particle_io.py
+-rw-rw-rw-   0        0        0      558 2023-04-27 09:22:56.000000 particlespy-0.6.2/particlespy/tests/test_plotting.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:42:11.040062 particlespy-0.6.2/particlespy.egg-info/
+-rw-rw-rw-   0        0        0     1272 2023-05-09 09:42:10.000000 particlespy-0.6.2/particlespy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      885 2023-05-09 09:42:10.000000 particlespy-0.6.2/particlespy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 09:42:10.000000 particlespy-0.6.2/particlespy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-05-09 09:42:10.000000 particlespy-0.6.2/particlespy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-09 09:42:10.000000 particlespy-0.6.2/particlespy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 09:42:11.063649 particlespy-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1085 2023-05-09 09:41:37.000000 particlespy-0.6.2/setup.py
```

### Comparing `particlespy-0.6.0/LICENSE` & `particlespy-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `particlespy-0.6.0/PKG-INFO` & `particlespy-0.6.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: particlespy
-Version: 0.6.0
+Version: 0.6.2
 Summary: A package to perform particle segmentation and analysis
 Home-page: https://github.com/ePSIC-DLS/particlespy
 Author: Thomas Slater
 Author-email: tjaslater@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![Build Status](https://travis-ci.com/ePSIC-DLS/ParticleSpy.svg?branch=master)](https://travis-ci.com/ePSIC-DLS/ParticleSpy)
+![Build Status](https://github.com/ePSIC-DLS/particlespy/actions/workflows/python-package-conda.yml/badge.svg)
 [![codecov](https://codecov.io/gh/ePSIC-DLS/ParticleSpy/branch/master/graph/badge.svg)](https://codecov.io/gh/ePSIC-DLS/ParticleSpy)
 [![PyPI version](https://badge.fury.io/py/particlespy.svg)](https://badge.fury.io/py/particlespy)
 [![DOI](https://zenodo.org/badge/154111577.svg)](https://zenodo.org/badge/latestdoi/154111577)
 
 # ParticleSpy
 Package for analysing particles in electron microscopy data sets.
 
 The package can be installed from PyPI using pip install ParticleSpy.
 
 Documentation can be found at https://epsic-dls.github.io/particlespy/index.html.
-
-
```

### Comparing `particlespy-0.6.0/README.md` & `particlespy-0.6.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![Build Status](https://travis-ci.com/ePSIC-DLS/ParticleSpy.svg?branch=master)](https://travis-ci.com/ePSIC-DLS/ParticleSpy)
+![Build Status](https://github.com/ePSIC-DLS/particlespy/actions/workflows/python-package-conda.yml/badge.svg)
 [![codecov](https://codecov.io/gh/ePSIC-DLS/ParticleSpy/branch/master/graph/badge.svg)](https://codecov.io/gh/ePSIC-DLS/ParticleSpy)
 [![PyPI version](https://badge.fury.io/py/particlespy.svg)](https://badge.fury.io/py/particlespy)
 [![DOI](https://zenodo.org/badge/154111577.svg)](https://zenodo.org/badge/latestdoi/154111577)
 
 # ParticleSpy
 Package for analysing particles in electron microscopy data sets.
```

### Comparing `particlespy-0.6.0/particlespy/api.py` & `particlespy-0.6.2/particlespy/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,7 +64,10 @@
                 elif len(prop_list) == 3:
                     p._plot_three_properties(prop_list,ax,**kwargs)
                 else:
                     print("Can only plot one or two properties, please change the length of the property list.")
                     break
         
         plt.show()
+
+def test():
+    print('Test')
```

### Comparing `particlespy-0.6.0/particlespy/custom_kernels.py` & `particlespy-0.6.2/particlespy/custom_kernels.py`

 * *Files identical despite different names*

### Comparing `particlespy-0.6.0/particlespy/find_zoneaxis.py` & `particlespy-0.6.2/particlespy/find_zoneaxis.py`

 * *Files identical despite different names*

### Comparing `particlespy-0.6.0/particlespy/parameters/manual_mask.npy` & `particlespy-0.6.2/particlespy/parameters/manual_mask.npy`

 * *Files identical despite different names*

### Comparing `particlespy-0.6.0/particlespy/parameters/parameters_current.hdf5` & `particlespy-0.6.2/particlespy/parameters/parameters_current.hdf5`

 * *Files identical despite different names*

### Comparing `particlespy-0.6.0/particlespy/parameters/parameters_previous.hdf5` & `particlespy-0.6.2/particlespy/parameters/parameters_previous.hdf5`

 * *Files identical despite different names*

### Comparing `particlespy-0.6.0/particlespy/particle_analysis.py` & `particlespy-0.6.2/particlespy/particle_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         p.set_property("y",region.centroid[1]*image.axes_manager[1].scale,image.axes_manager[1].units)
         
         cal_axes_lengths = (region.major_axis_length*image.axes_manager[0].scale,region.minor_axis_length*image.axes_manager[0].scale)
         #Note: the above only works for square pixels
         p.set_axes_lengths(cal_axes_lengths,diam_units)
         
         #Set shape measures
-        peri = image.axes_manager[0].scale*perimeter(maskp,neighbourhood=4)
+        peri = image.axes_manager[0].scale*perimeter(maskp,neighborhood=4)
         circularity = 4*3.14159265*p.properties['area']['value']/(peri**2)
         p.set_circularity(circularity)
         eccentricity = region.eccentricity
         p.set_eccentricity(eccentricity)
         p.set_property("solidity",region.solidity,None)
         
         #Set total image intensity
```

### Comparing `particlespy-0.6.0/particlespy/particle_load.py` & `particlespy-0.6.2/particlespy/particle_load.py`

 * *Files identical despite different names*

### Comparing `particlespy-0.6.0/particlespy/particle_save.py` & `particlespy-0.6.2/particlespy/particle_save.py`

 * *Files identical despite different names*

### Comparing `particlespy-0.6.0/particlespy/ptcl_class.py` & `particlespy-0.6.2/particlespy/ptcl_class.py`

 * *Files identical despite different names*

### Comparing `particlespy-0.6.0/particlespy/radial_profile.py` & `particlespy-0.6.2/particlespy/radial_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,20 +114,21 @@
         If true, mark the particle radius on the profile plot.
     radius : float
     save : bool
     dir_save : str
         Default : None
     """
         
+    plt.figure()
     plt.xlabel('Distance from particle centre ('+units+')')
     plt.ylabel('Normalised intensity (counts)')
     
     for sig, count_and_dist in dist_count_dic.items():
         if sig=='Image':
             sig = 'ADF'
         plt.plot(np.array(count_and_dist[0])*scale, count_and_dist[1],label=sig)
         if mark_radius==True:
             plt.axvline(x=radius,color='k',linestyle='--')
     plt.legend()
     
     if save==True:
-        plt.savefig(dir_save,bbox_inches='tight',dpi=600)
+        plt.savefig(dir_save,bbox_inches='tight',dpi=600)
```

### Comparing `particlespy-0.6.0/particlespy/seg_ui.py` & `particlespy-0.6.2/particlespy/seg_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,15 @@
         self.getim(im_hs)
         self.getparams()
         
         self.prev_params = parameters()
         self.prev_params.generate()
         
         offset = 50
-        self.canvas_size = height
-        
+        self.canvas_size = [height,int(self.image.shape[1]/self.image.shape[0]*height)]
         self.layout = QHBoxLayout(self)
         
         # Initialize tab screen
         self.tabs = QTabWidget()
         self.tab1 = QWidget()
         self.tab2 = QWidget()
         self.tab3 = QWidget()
@@ -66,15 +65,15 @@
         rightlay = QVBoxLayout()
         self.tab1.setLayout(lay)
 
         #tab 1
         self.label = QLabel(self)
         qi = QImage(self.image.data, self.image.shape[1], self.image.shape[0], self.image.shape[1], QImage.Format_Grayscale8)
         pixmap = QPixmap(qi)
-        self.pixmap2 = pixmap.scaled(self.canvas_size, self.canvas_size, Qt.KeepAspectRatio)
+        self.pixmap2 = pixmap.scaled(self.canvas_size[1], self.canvas_size[0], Qt.KeepAspectRatio)
         self.label.setPixmap(self.pixmap2)
         self.label.setGeometry(10,10,self.pixmap2.width(),self.pixmap2.height())
         
         height = max((self.pixmap2.height()+50,300 + offset)) #300 +50
         
         self.resize(self.pixmap2.width()+130, height)
         
@@ -213,15 +212,15 @@
         tab2layout.addWidget(self.getarrayb)
         tab2layout.addStretch(1)
         self.tab2.setLayout(tab2layout)
 
         #Tab 3
       
 
-        self.mask = np.zeros([self.canvas_size,self.canvas_size,3])
+        self.mask = np.zeros([self.canvas_size[0],self.canvas_size[1],3])
         self.classifier = GaussianNB()
         self.tsparams = trainable_parameters()
         self.filter_kernels = ['Gaussian','Diff. Gaussians','Median','Minimum','Maximum','Sobel','Hessian','Laplacian','M-Sum','M-Mean','M-Standard Deviation','M-Median','M-Minimum','M-Maximum']
 
         lay3 = QHBoxLayout()
         im_lay = QVBoxLayout()
                
@@ -446,15 +445,15 @@
                 qi = QImage(invert(b).data, b.shape[1], b.shape[0], b.shape[1], QImage.Format_Indexed8)
             else:
                 qi = QImage(b.data, b.shape[1], b.shape[0], b.shape[1], QImage.Format_Indexed8)
         if self.imflag=="Labels":
             qi = QImage(labels.data, labels.shape[1], labels.shape[0], labels.shape[1], QImage.Format_Indexed8)
         #qi = QImage(imchoice.data, imchoice.shape[1], imchoice.shape[0], imchoice.shape[1], QImage.Format_Indexed8)
         pixmap = QPixmap(qi)
-        pixmap2 = pixmap.scaled(self.canvas_size, self.canvas_size, Qt.KeepAspectRatio)
+        pixmap2 = pixmap.scaled(self.canvas_size[1], self.canvas_size[0], Qt.KeepAspectRatio)
         self.label.setPixmap(pixmap2)
         
         self.prev_params.load()
         self.prev_params.save(filename=os.path.dirname(inspect.getfile(process))+'/parameters/parameters_previous.hdf5')
         self.params.save()
         
     def undo(self):
@@ -609,15 +608,15 @@
         self.colors =['#80A30015', '#806DA34D', '#8051E5FF', '#80BD2D87', '#80F5E663']
         self.color_index = 0
 
         self.pen_color = QColor(self.colors[0])
         self.penType = self.brush_tools[0]
         self.lineCount = 0
 
-        self.array = np.zeros((self.canvas_size,self.canvas_size,3),dtype=np.uint8)
+        self.array = np.zeros((self.canvas_size[0],self.canvas_size[1],3),dtype=np.uint8)
 
     def set_pen_color(self, c):
         self.color_index = c
         self.pen_color = QColor(self.colors[self.color_index])
 
     def changePen(self, brush):
         self.last_click = None
@@ -627,21 +626,21 @@
     def clearCanvas(self):
 
         self.last_click = None
         self.first_click = None
         self.lineCount = 0
 
         painter = QPainter(self.pixmap())
-        painter.eraseRect(0,0,self.canvas_size,self.canvas_size)
+        painter.eraseRect(0,0,self.canvas_size[0],self.canvas_size[1])
         painter.drawPixmap(0,0,self.OGpixmap)
         painter.end()
         self.update()
 
     def clearLabels(self):
-        self.array = np.zeros((self.canvas_size,self.canvas_size,3), dtype=np.uint8)
+        self.array = np.zeros((self.canvas_size[0],self.canvas_size[1],3), dtype=np.uint8)
 
     def redrawLabels(self):
         array = toggle_channels(self.array)
         self.drawLabels(array)
 
     def drawLabels(self, thin_labels):
 
@@ -651,15 +650,15 @@
         thicc_labels[:,:,1:] = toggle_channels(thin_labels)
         thicc_labels[:,:,0] = (thin_labels > 0)*255
 
         thicc_labels = np.flip(thicc_labels, axis=2).copy()
         qi = QImage(thicc_labels.data, thicc_labels.shape[1], thicc_labels.shape[0], 4*thicc_labels.shape[1], QImage.Format_ARGB32_Premultiplied)
         
         pixmap = QPixmap(qi)
-        pixmap = pixmap.scaled(self.canvas_size, self.canvas_size, Qt.KeepAspectRatio)
+        pixmap = pixmap.scaled(self.canvas_size[1], self.canvas_size[0], Qt.KeepAspectRatio)
         painter = QPainter(self.pixmap())
         painter.setOpacity(0.5)
         painter.drawPixmap(0,0,pixmap)
         painter.end()
         self.update()
 
     def lineDraw(self,pos1,pos2):
@@ -708,21 +707,24 @@
                 self.lineDraw(self.last_click, e.pos())
                 self.last_click = QPoint(e.x(),e.y())
                 self.lineCount += 1
     
     def flood(self, e):
         image = self.pixmap().toImage()
         b = image.bits()
-        b.setsize(self.canvas_size * self.canvas_size * 4)
-        arr = np.frombuffer(b, np.uint8).reshape((self.canvas_size, self.canvas_size, 4))
-        
+        b.setsize(self.canvas_size[0] * self.canvas_size[1] * 4)
+        arr = np.frombuffer(b, np.uint8)
+        arr = arr.reshape((self.canvas_size[0], self.canvas_size[1], 4)).copy()
+
         OGimage = self.OGpixmap.toImage()
-        b = OGimage.bits()
-        b.setsize(self.canvas_size * self.canvas_size * 4)
-        OGim = np.frombuffer(b, np.uint8).reshape((self.canvas_size, self.canvas_size, 4))
+        c = OGimage.bits()
+        c.setsize(self.canvas_size[0] * self.canvas_size[1] * 4)
+        
+        c = np.frombuffer(c, np.uint8).copy()
+        OGim = np.reshape(c, (self.canvas_size[0], self.canvas_size[1], 4))
         OGim = np.flip(OGim, axis=2)
 
         arr = arr.astype(np.int32)
         arr = np.flip(arr, axis=2)
 
         arr_test = np.zeros_like(arr)
         arr_test[arr != OGim] = arr[arr != OGim]
@@ -740,15 +742,14 @@
         #fills wil pen colour
         
         #BGRA
         paint_arr = np.flip(paint_arr, axis=2).copy()
         
         qi = QImage(paint_arr.data, paint_arr.shape[1], paint_arr.shape[0], 4*paint_arr.shape[1], QImage.Format_ARGB32_Premultiplied)
         pixmap = QPixmap(qi)
-        
         painter = QPainter(self.pixmap())
         painter.setOpacity(0.5)
         painter.drawPixmap(0,0,pixmap)
         painter.end()
         self.update()
         
         #self.array saves RGB values
```

### Comparing `particlespy-0.6.0/particlespy/segimgs.py` & `particlespy-0.6.2/particlespy/segimgs.py`

 * *Files identical despite different names*

### Comparing `particlespy-0.6.0/particlespy/segptcls.py` & `particlespy-0.6.2/particlespy/segptcls.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     
     if param.segment["watershed"]!=False:
         labels = p_watershed(labels,param.segment["watershed_size"],param.segment["watershed_erosion"])
         
     labels = clear_border(labels)
 
     if param.segment["min_size"]!=0:
-        remove_small_objects(labels,param.segment["min_size"],in_place=True)
+        labels = remove_small_objects(labels,param.segment["min_size"])
         
     return(labels)
     
 def threshold(data, process_param):
     if process_param["threshold"] == "otsu":
         thresh = threshold_otsu(data)
     if process_param["threshold"] == "mean":
@@ -117,19 +117,22 @@
         eroded_image=binary_erosion(thresh_image)
         for i in range(erosion-1):
             eroded_image=binary_erosion(eroded_image)
     else:
         eroded_image=thresh_image
     
     distance = ndi.distance_transform_edt(eroded_image)
-    local_maxi = peak_local_max(distance, indices=False, footprint=np.ones((min_size, min_size)),
-                            labels=thresh_image)
-    markers = ndi.label(local_maxi)[0]
+    coords = peak_local_max(distance, footprint=np.ones((min_size, min_size)), labels=thresh_image)
+    mask = np.zeros(distance.shape, dtype=bool)
+    mask[tuple(coords.T)] = True
+    markers, _ = ndi.label(mask)
+    #markers = ndi.label(local_maxi)[0]
     labels = watershed(-distance, markers, mask=thresh_image)
     return(labels)
     
 def rolling_ball(img,kernelsize=0):
     if kernelsize == 0:
         new_img = img
     else:
-        new_img = white_tophat(rescale_intensity(img, out_range = (-1,1)),selem=square(kernelsize))
+        new_img = img - white_tophat(rescale_intensity(img, out_range = (-1,1)),footprint=square(kernelsize))
     return (new_img)
+
```

### Comparing `particlespy-0.6.0/particlespy.egg-info/PKG-INFO` & `particlespy-0.6.2/particlespy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: particlespy
-Version: 0.6.0
+Version: 0.6.2
 Summary: A package to perform particle segmentation and analysis
 Home-page: https://github.com/ePSIC-DLS/particlespy
 Author: Thomas Slater
 Author-email: tjaslater@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![Build Status](https://travis-ci.com/ePSIC-DLS/ParticleSpy.svg?branch=master)](https://travis-ci.com/ePSIC-DLS/ParticleSpy)
+![Build Status](https://github.com/ePSIC-DLS/particlespy/actions/workflows/python-package-conda.yml/badge.svg)
 [![codecov](https://codecov.io/gh/ePSIC-DLS/ParticleSpy/branch/master/graph/badge.svg)](https://codecov.io/gh/ePSIC-DLS/ParticleSpy)
 [![PyPI version](https://badge.fury.io/py/particlespy.svg)](https://badge.fury.io/py/particlespy)
 [![DOI](https://zenodo.org/badge/154111577.svg)](https://zenodo.org/badge/latestdoi/154111577)
 
 # ParticleSpy
 Package for analysing particles in electron microscopy data sets.
 
 The package can be installed from PyPI using pip install ParticleSpy.
 
 Documentation can be found at https://epsic-dls.github.io/particlespy/index.html.
-
-
```

### Comparing `particlespy-0.6.0/particlespy.egg-info/SOURCES.txt` & `particlespy-0.6.2/particlespy.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -16,8 +16,14 @@
 particlespy.egg-info/PKG-INFO
 particlespy.egg-info/SOURCES.txt
 particlespy.egg-info/dependency_links.txt
 particlespy.egg-info/requires.txt
 particlespy.egg-info/top_level.txt
 particlespy/parameters/manual_mask.npy
 particlespy/parameters/parameters_current.hdf5
-particlespy/parameters/parameters_previous.hdf5
+particlespy/parameters/parameters_previous.hdf5
+particlespy/tests/__init__.py
+particlespy/tests/generate_test_data.py
+particlespy/tests/test_particle_analysis.py
+particlespy/tests/test_particle_clustering.py
+particlespy/tests/test_particle_io.py
+particlespy/tests/test_plotting.py
```

### Comparing `particlespy-0.6.0/setup.py` & `particlespy-0.6.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-install_requires=["hyperspy",
+install_requires=["hyperspy>=1.7",
                   "scikit-image>=0.17.1",
                   "scikit-learn>=0.21",
 				  "trackpy",
                   "numpy>=1.16.5",
 				  "PyQt5>=5.14.0"]
 
 setuptools.setup(
     name="particlespy",
     package_dir={'particlespy':'particlespy'},
-    version="0.6.0",
+    version="0.6.2",
     author="Thomas Slater",
     author_email="tjaslater@gmail.com",
     description="A package to perform particle segmentation and analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ePSIC-DLS/particlespy",
     packages=setuptools.find_packages(),
```

