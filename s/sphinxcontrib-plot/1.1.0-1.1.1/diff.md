# Comparing `tmp/sphinxcontrib-plot-1.1.0.tar.gz` & `tmp/sphinxcontrib-plot-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-plot-1.1.0.tar", last modified: Thu Apr 27 07:30:13 2023, max compression
+gzip compressed data, was "sphinxcontrib-plot-1.1.1.tar", last modified: Tue May  9 03:18:26 2023, max compression
```

## Comparing `sphinxcontrib-plot-1.1.0.tar` & `sphinxcontrib-plot-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-04-27 07:30:13.898770 sphinxcontrib-plot-1.1.0/
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)     1418 2021-07-29 23:39:29.000000 sphinxcontrib-plot-1.1.0/LICENSE
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       51 2021-07-29 23:39:29.000000 sphinxcontrib-plot-1.1.0/MANIFEST.in
--rw-rw-r--   0 ypguo    (19391612) Domain Users (1049089)    10498 2023-04-27 07:30:13.899777 sphinxcontrib-plot-1.1.0/PKG-INFO
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    10171 2023-04-27 07:18:45.000000 sphinxcontrib-plot-1.1.0/README.rst
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       76 2023-04-27 07:30:13.900776 sphinxcontrib-plot-1.1.0/setup.cfg
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      625 2023-04-27 07:18:07.000000 sphinxcontrib-plot-1.1.0/setup.py
-drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-04-27 07:30:13.876563 sphinxcontrib-plot-1.1.0/sphinxcontrib/
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      269 2021-07-29 23:39:29.000000 sphinxcontrib-plot-1.1.0/sphinxcontrib/__init__.py
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    17855 2023-04-27 07:16:01.000000 sphinxcontrib-plot-1.1.0/sphinxcontrib/plot.py
-drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-04-27 07:30:13.883588 sphinxcontrib-plot-1.1.0/sphinxcontrib_plot.egg-info/
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    10498 2023-04-27 07:30:13.000000 sphinxcontrib-plot-1.1.0/sphinxcontrib_plot.egg-info/PKG-INFO
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      357 2023-04-27 07:30:13.000000 sphinxcontrib-plot-1.1.0/sphinxcontrib_plot.egg-info/SOURCES.txt
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)        1 2023-04-27 07:30:13.000000 sphinxcontrib-plot-1.1.0/sphinxcontrib_plot.egg-info/dependency_links.txt
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       14 2023-04-27 07:30:13.000000 sphinxcontrib-plot-1.1.0/sphinxcontrib_plot.egg-info/namespace_packages.txt
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       12 2023-04-27 07:30:13.000000 sphinxcontrib-plot-1.1.0/sphinxcontrib_plot.egg-info/requires.txt
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       14 2023-04-27 07:30:13.000000 sphinxcontrib-plot-1.1.0/sphinxcontrib_plot.egg-info/top_level.txt
+drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-05-09 03:18:26.921362 sphinxcontrib-plot-1.1.1/
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)     1418 2021-07-29 23:39:29.000000 sphinxcontrib-plot-1.1.1/LICENSE
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       51 2021-07-29 23:39:29.000000 sphinxcontrib-plot-1.1.1/MANIFEST.in
+-rw-rw-r--   0 ypguo    (19391612) Domain Users (1049089)    13533 2023-05-09 03:18:26.921362 sphinxcontrib-plot-1.1.1/PKG-INFO
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    13206 2023-05-09 03:17:41.000000 sphinxcontrib-plot-1.1.1/README.rst
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       76 2023-05-09 03:18:26.921362 sphinxcontrib-plot-1.1.1/setup.cfg
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      625 2023-05-09 03:18:13.000000 sphinxcontrib-plot-1.1.1/setup.py
+drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-05-09 03:18:26.911982 sphinxcontrib-plot-1.1.1/sphinxcontrib/
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      269 2021-07-29 23:39:29.000000 sphinxcontrib-plot-1.1.1/sphinxcontrib/__init__.py
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    17949 2023-05-09 02:51:34.000000 sphinxcontrib-plot-1.1.1/sphinxcontrib/plot.py
+drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-05-09 03:18:26.921362 sphinxcontrib-plot-1.1.1/sphinxcontrib_plot.egg-info/
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    13533 2023-05-09 03:18:26.000000 sphinxcontrib-plot-1.1.1/sphinxcontrib_plot.egg-info/PKG-INFO
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      357 2023-05-09 03:18:26.000000 sphinxcontrib-plot-1.1.1/sphinxcontrib_plot.egg-info/SOURCES.txt
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)        1 2023-05-09 03:18:26.000000 sphinxcontrib-plot-1.1.1/sphinxcontrib_plot.egg-info/dependency_links.txt
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       14 2023-05-09 03:18:26.000000 sphinxcontrib-plot-1.1.1/sphinxcontrib_plot.egg-info/namespace_packages.txt
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       12 2023-05-09 03:18:26.000000 sphinxcontrib-plot-1.1.1/sphinxcontrib_plot.egg-info/requires.txt
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       14 2023-05-09 03:18:26.000000 sphinxcontrib-plot-1.1.1/sphinxcontrib_plot.egg-info/top_level.txt
```

### Comparing `sphinxcontrib-plot-1.1.0/LICENSE` & `sphinxcontrib-plot-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-plot-1.1.0/PKG-INFO` & `sphinxcontrib-plot-1.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-plot
-Version: 1.1.0
+Version: 1.1.1
 Summary: Embed gnuplot, ditaa, pyplot, DOT, etc. diagrams in your Sphinx-based documentation.
 Home-page: https://github.com/stathissideris/sphinxcontrib-plot
 Author: Yongping Guo
 Author-email: guoyoooping@163.com
 License: GPLv3
 Platform: any
 License-File: LICENSE
 
 sphinxcontrib-plot
 *********************
 
-A sphinx extension to plot all kind of graph such as ditaa/gnuplot/pyplot, etc. within .rst file.
+A sphinx extension to plot all kinds of graph such as ditaa, gnuplot, pyplot,
+dot, convert, blockdiag, seqdiag, actdiag, nwdiag.
 
 .. image:: http://gnuplot.sourceforge.net/demo_5.2/transparent.2.png
 
 Usage: Inline diagram, show as svg::
 
     .. plot:: gnuplot
         :caption: figure 3. illustration for gnuplot
@@ -219,16 +220,123 @@
         -fill blue  -draw "path 'M 68,65 L 85.1,18.0 A 50,50 0 0,1  118,65   Z'"
         -fill gold  -draw "path 'M 60,70 L  110,70   A 50,50 0 1,1   60,20   Z'"
         -fill black -stroke none  -pointsize 10
         -draw "text 57,19 '10' text 70,20 '10' text 90,19 '70' text 113,78 '270'"
 
 .. image:: https://legacy.imagemagick.org/Usage/draw/piechart.jpg
 
-2.6 Other applications
-----------------------
+2.6 blockdiag, seqdiag, actdiag, nwdiag.
+------------------------------------------
+
+demo for blockdiag::
+
+    .. plot:: blockdiag
+        :caption: demo for blockdiag
+        :name: demo for blockdiag
+
+        blockdiag {
+          // Set stacked to nodes.
+          stacked [stacked];
+          diamond [shape = "diamond", stacked];
+          database [shape = "flowchart.database", stacked];
+
+          stacked -> diamond -> database;
+        }
+
+This will generate the follong image on your .htm/.pdf document generated from
+sphinx:
+
+.. image:: http://blockdiag.com/en/_images/blockdiag-56cb174d92d602f8cc9013006e661c4806e1d5ab.png
+
+demo for seqdiag::
+
+    .. plot:: blockdiag
+        :caption: demo for seqdiag
+        :name: demo for seqdiag
+
+    seqdiag {
+      // Set edge metrix.
+      edge_length = 300;  // default value is 192
+      span_height = 80;  // default value is 40
+
+      // Set fontsize.
+      default_fontsize = 16;  // default value is 11
+
+      // Do not show activity line
+      activation = none;
+
+      // Numbering edges automaticaly
+      autonumber = True;
+
+      // Change note color
+      default_note_color = lightblue;
+
+      browser  -> webserver [label = "GET \n/index.html"];
+      browser <-- webserver [note = "Apache works!"];
+    }
+
+This will generate the follong image on your .htm/.pdf document generated from
+sphinx:
+
+.. image:: http://blockdiag.com/en/_images/seqdiag-9d43a794bd1f63fc9418595e4451c5fb9c52ad39.png
+
+demo for actdiag::
+
+    .. plot:: actdiag
+        :caption: demo for actdiag
+        :name: demo for actdiag
+
+    actdiag {
+      write -> convert -> image
+
+      lane user {
+         label = "User"
+         write [label = "Writing reST"];
+         image [label = "Get diagram IMAGE"];
+      }
+      lane actdiag {
+         convert [label = "Convert reST to Image"];
+      }
+    }
+
+This will generate the follong image on your .htm/.pdf document generated from
+sphinx:
+
+.. image:: http://blockdiag.com/en/_images/actdiag-27aec367951ef70f7b5badceebbcc0c2bc687752.png
+
+demo for nwdiag::
+
+    .. plot:: nwdiag
+        :caption: demo for actdiag
+        :name: demo for actdiag
+
+    nwdiag {
+      network dmz {
+          address = "210.x.x.x/24"
+
+          web01 [address = "210.x.x.1"];
+          web02 [address = "210.x.x.2"];
+      }
+      network internal {
+          address = "172.x.x.x/24";
+
+          web01 [address = "172.x.x.1"];
+          web02 [address = "172.x.x.2"];
+          db01;
+          db02;
+      }
+    }
+
+This will generate the follong image on your .htm/.pdf document generated from
+sphinx:
+
+.. image:: http://blockdiag.com/en/_images/nwdiag-be3d31eeeacd641176a6f63703748e33d278419a.png
+
+2.7 Other applications
+-------------------------
 
 In theory, All the command which could generate graph could be used after the
 directive "..plot::". Please report it when you found anyone which works or
 doesn't work.
 
 3 Options
 ===========
@@ -312,7 +420,17 @@
 | 1.0.8 Bug fix: When there is no :size: in gnuplot plot, it might crash.
 | 1.0.10 Bug fix: fix the issue that convert doesn't work.
 | 1.0.13 Support magick script
 | 1.0.17 bug fix: convert can has no body.
 | 1.0.18 New feature: 1) Support montage command; 2) Support including .gif image into html and pdf. If it's html, play the .gif, or else if it's pdf, convert the .gif to a list of frame.
 | 1.0.19 Support lines starting with # in the convert/montage body.
 | 1.1.0 Bug fix: It doesn't work for ditaa with convert parameters.
+| 1.1.1 Support the following plot command: blockdiag, seqdiag, actdiag, nwdiag.
+
+Refenreces
+==========
+
+#. blockdiag, http://blockdiag.com/en/blockdiag/index.html
+#. seqdiag , http://blockdiag.com/en/seqdiag/index.html
+#. actdiag , http://blockdiag.com/en/nwdiag/actdiag.html
+#. nwdiag , http://blockdiag.com/en/nwdiag/index.html
+
```

### Comparing `sphinxcontrib-plot-1.1.0/setup.py` & `sphinxcontrib-plot-1.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 requires = ['Sphinx>=0.6',
         ]
 
 setup(
     name='sphinxcontrib-plot',
-    version='1.1.0',
+    version='1.1.1',
     url='https://github.com/stathissideris/sphinxcontrib-plot',
     license='GPLv3',
     author='Yongping Guo',
     author_email='guoyoooping@163.com',
     description='Embed gnuplot, ditaa, pyplot, DOT, etc. diagrams in your Sphinx-based documentation.',
     long_description=open('README.rst').read(),
     platforms='any',
```

### Comparing `sphinxcontrib-plot-1.1.0/sphinxcontrib/plot.py` & `sphinxcontrib-plot-1.1.1/sphinxcontrib/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,16 +202,17 @@
     #print("cmd: %s" %(cmd))
     if "ditaa" in cmd:
         if (not options.get("convert", None)):
             args.insert(1, "--svg") #to support Chinese, draw it always with --svg.
         args.extend([infname, outfname])
         # Ditaa must work on the target directory.
         os.chdir(os.path.dirname(out["outfullfn"]))
-    elif "seqdiag" in cmd:
-        #seqdiag only support svg, convert it to pdf automatically.
+    elif "seqdiag" in cmd or "blockdiag" in cmd \
+            or "actdiag" in cmd or "nwdiag" in cmd:
+        #seqdiag ... etc, only support svg, convert it to pdf automatically.
         if (plot_format in ["svg", "pdf"]) and ("-Tsvg" not in cmd):
             #ditaa support vector image by --svg parameter.
             args.insert(1, "-Tsvg")
             os.chdir(os.path.dirname(out["outfullfn"]))
         args.extend([infname, '-o', outfname])
     elif args[0] == "dot":
         # dot -Tpng in_file -o out_file
@@ -321,15 +322,15 @@
             os.system("mv %s %s" %(conver_outfile, out["outfullfn"]))
         #if options.get("background", None):
         #    # Add a background
         #    print("convert %s -background %s -flatten %s"
         #            %(out["outfullfn"], options["background"], out["outfullfn"]))
         #    os.system("convert %s -background %s -flatten %s"
         #            %(out["outfullfn"], options["background"], out["outfullfn"]))
-    elif (args[0] == "ditaa" or args[0] == "dot" or args[0] == "seqdiag") \
+    elif (args[0] in ["ditaa", "dot", "seqdiag", "blockdiag", "actdiag", "nwdiag"]) \
             and (plot_format in ['pdf']):
         # In fact ditaa don't support pdf, we convert the .svg to .pdf inkscape
         if (args[0] == "dot"):
             print("mv %s %s-%s.svg" %(out["outfullfn"], args[0], hashkey))
             os.system("mv %s %s-%s.svg" %(out["outfullfn"], args[0], hashkey))
         else:
             print("mv %s %s-%s.svg" %(outfname, args[0], hashkey))
```

### Comparing `sphinxcontrib-plot-1.1.0/sphinxcontrib_plot.egg-info/PKG-INFO` & `sphinxcontrib-plot-1.1.1/sphinxcontrib_plot.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-plot
-Version: 1.1.0
+Version: 1.1.1
 Summary: Embed gnuplot, ditaa, pyplot, DOT, etc. diagrams in your Sphinx-based documentation.
 Home-page: https://github.com/stathissideris/sphinxcontrib-plot
 Author: Yongping Guo
 Author-email: guoyoooping@163.com
 License: GPLv3
 Platform: any
 License-File: LICENSE
 
 sphinxcontrib-plot
 *********************
 
-A sphinx extension to plot all kind of graph such as ditaa/gnuplot/pyplot, etc. within .rst file.
+A sphinx extension to plot all kinds of graph such as ditaa, gnuplot, pyplot,
+dot, convert, blockdiag, seqdiag, actdiag, nwdiag.
 
 .. image:: http://gnuplot.sourceforge.net/demo_5.2/transparent.2.png
 
 Usage: Inline diagram, show as svg::
 
     .. plot:: gnuplot
         :caption: figure 3. illustration for gnuplot
@@ -219,16 +220,123 @@
         -fill blue  -draw "path 'M 68,65 L 85.1,18.0 A 50,50 0 0,1  118,65   Z'"
         -fill gold  -draw "path 'M 60,70 L  110,70   A 50,50 0 1,1   60,20   Z'"
         -fill black -stroke none  -pointsize 10
         -draw "text 57,19 '10' text 70,20 '10' text 90,19 '70' text 113,78 '270'"
 
 .. image:: https://legacy.imagemagick.org/Usage/draw/piechart.jpg
 
-2.6 Other applications
-----------------------
+2.6 blockdiag, seqdiag, actdiag, nwdiag.
+------------------------------------------
+
+demo for blockdiag::
+
+    .. plot:: blockdiag
+        :caption: demo for blockdiag
+        :name: demo for blockdiag
+
+        blockdiag {
+          // Set stacked to nodes.
+          stacked [stacked];
+          diamond [shape = "diamond", stacked];
+          database [shape = "flowchart.database", stacked];
+
+          stacked -> diamond -> database;
+        }
+
+This will generate the follong image on your .htm/.pdf document generated from
+sphinx:
+
+.. image:: http://blockdiag.com/en/_images/blockdiag-56cb174d92d602f8cc9013006e661c4806e1d5ab.png
+
+demo for seqdiag::
+
+    .. plot:: blockdiag
+        :caption: demo for seqdiag
+        :name: demo for seqdiag
+
+    seqdiag {
+      // Set edge metrix.
+      edge_length = 300;  // default value is 192
+      span_height = 80;  // default value is 40
+
+      // Set fontsize.
+      default_fontsize = 16;  // default value is 11
+
+      // Do not show activity line
+      activation = none;
+
+      // Numbering edges automaticaly
+      autonumber = True;
+
+      // Change note color
+      default_note_color = lightblue;
+
+      browser  -> webserver [label = "GET \n/index.html"];
+      browser <-- webserver [note = "Apache works!"];
+    }
+
+This will generate the follong image on your .htm/.pdf document generated from
+sphinx:
+
+.. image:: http://blockdiag.com/en/_images/seqdiag-9d43a794bd1f63fc9418595e4451c5fb9c52ad39.png
+
+demo for actdiag::
+
+    .. plot:: actdiag
+        :caption: demo for actdiag
+        :name: demo for actdiag
+
+    actdiag {
+      write -> convert -> image
+
+      lane user {
+         label = "User"
+         write [label = "Writing reST"];
+         image [label = "Get diagram IMAGE"];
+      }
+      lane actdiag {
+         convert [label = "Convert reST to Image"];
+      }
+    }
+
+This will generate the follong image on your .htm/.pdf document generated from
+sphinx:
+
+.. image:: http://blockdiag.com/en/_images/actdiag-27aec367951ef70f7b5badceebbcc0c2bc687752.png
+
+demo for nwdiag::
+
+    .. plot:: nwdiag
+        :caption: demo for actdiag
+        :name: demo for actdiag
+
+    nwdiag {
+      network dmz {
+          address = "210.x.x.x/24"
+
+          web01 [address = "210.x.x.1"];
+          web02 [address = "210.x.x.2"];
+      }
+      network internal {
+          address = "172.x.x.x/24";
+
+          web01 [address = "172.x.x.1"];
+          web02 [address = "172.x.x.2"];
+          db01;
+          db02;
+      }
+    }
+
+This will generate the follong image on your .htm/.pdf document generated from
+sphinx:
+
+.. image:: http://blockdiag.com/en/_images/nwdiag-be3d31eeeacd641176a6f63703748e33d278419a.png
+
+2.7 Other applications
+-------------------------
 
 In theory, All the command which could generate graph could be used after the
 directive "..plot::". Please report it when you found anyone which works or
 doesn't work.
 
 3 Options
 ===========
@@ -312,7 +420,17 @@
 | 1.0.8 Bug fix: When there is no :size: in gnuplot plot, it might crash.
 | 1.0.10 Bug fix: fix the issue that convert doesn't work.
 | 1.0.13 Support magick script
 | 1.0.17 bug fix: convert can has no body.
 | 1.0.18 New feature: 1) Support montage command; 2) Support including .gif image into html and pdf. If it's html, play the .gif, or else if it's pdf, convert the .gif to a list of frame.
 | 1.0.19 Support lines starting with # in the convert/montage body.
 | 1.1.0 Bug fix: It doesn't work for ditaa with convert parameters.
+| 1.1.1 Support the following plot command: blockdiag, seqdiag, actdiag, nwdiag.
+
+Refenreces
+==========
+
+#. blockdiag, http://blockdiag.com/en/blockdiag/index.html
+#. seqdiag , http://blockdiag.com/en/seqdiag/index.html
+#. actdiag , http://blockdiag.com/en/nwdiag/actdiag.html
+#. nwdiag , http://blockdiag.com/en/nwdiag/index.html
+
```

