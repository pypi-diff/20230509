# Comparing `tmp/rembg-2.0.35.tar.gz` & `tmp/rembg-2.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rembg-2.0.35.tar", last modified: Thu Apr 27 23:06:49 2023, max compression
+gzip compressed data, was "rembg-2.0.36.tar", last modified: Tue May  9 04:22:46 2023, max compression
```

## Comparing `rembg-2.0.35.tar` & `rembg-2.0.36.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:06:49.645459 rembg-2.0.35/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 23:06:34.000000 rembg-2.0.35/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-27 23:06:34.000000 rembg-2.0.35/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-04-27 23:06:49.645459 rembg-2.0.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-27 23:06:34.000000 rembg-2.0.35/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-27 23:06:34.000000 rembg-2.0.35/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:06:49.645459 rembg-2.0.35/rembg/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-27 23:06:49.645459 rembg-2.0.35/rembg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/bg.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:06:49.645459 rembg-2.0.35/rembg/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/commands/i_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/commands/p_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/commands/s_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/session_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:06:49.645459 rembg-2.0.35/rembg/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/sessions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/sessions/dis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/sessions/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/sessions/silueta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/sessions/u2net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/sessions/u2net_cloth_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/sessions/u2net_human_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-27 23:06:34.000000 rembg-2.0.35/rembg/sessions/u2netp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:06:49.641459 rembg-2.0.35/rembg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-04-27 23:06:49.000000 rembg-2.0.35/rembg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-27 23:06:49.000000 rembg-2.0.35/rembg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:06:49.000000 rembg-2.0.35/rembg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 23:06:49.000000 rembg-2.0.35/rembg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-27 23:06:49.000000 rembg-2.0.35/rembg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 23:06:49.000000 rembg-2.0.35/rembg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 23:06:34.000000 rembg-2.0.35/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-27 23:06:34.000000 rembg-2.0.35/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-27 23:06:49.645459 rembg-2.0.35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-27 23:06:34.000000 rembg-2.0.35/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-27 23:06:34.000000 rembg-2.0.35/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:22:46.167957 rembg-2.0.36/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 04:22:33.000000 rembg-2.0.36/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-09 04:22:33.000000 rembg-2.0.36/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-05-09 04:22:46.167957 rembg-2.0.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-05-09 04:22:33.000000 rembg-2.0.36/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-09 04:22:33.000000 rembg-2.0.36/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:22:46.167957 rembg-2.0.36/rembg/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 04:22:46.167957 rembg-2.0.36/rembg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/bg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:22:46.167957 rembg-2.0.36/rembg/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/commands/b_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/commands/i_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/commands/p_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/commands/s_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/session_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:22:46.167957 rembg-2.0.36/rembg/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/dis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/silueta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/u2net_cloth_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/u2net_human_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/u2netp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:22:46.167957 rembg-2.0.36/rembg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-05-09 04:22:46.000000 rembg-2.0.36/rembg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-09 04:22:46.000000 rembg-2.0.36/rembg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:22:46.000000 rembg-2.0.36/rembg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-09 04:22:46.000000 rembg-2.0.36/rembg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-09 04:22:46.000000 rembg-2.0.36/rembg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 04:22:46.000000 rembg-2.0.36/rembg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-09 04:22:33.000000 rembg-2.0.36/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-09 04:22:33.000000 rembg-2.0.36/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-09 04:22:46.167957 rembg-2.0.36/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-09 04:22:33.000000 rembg-2.0.36/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-09 04:22:33.000000 rembg-2.0.36/versioneer.py
```

### Comparing `rembg-2.0.35/LICENSE.txt` & `rembg-2.0.36/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.35/PKG-INFO` & `rembg-2.0.36/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.35
+Version: 2.0.36
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 License: UNKNOWN
 Keywords: remove,background,u2net
 Platform: UNKNOWN
@@ -117,18 +117,19 @@
 pip install rembg[gpu]
 ```
 
 ## Usage as a cli
 
 After the installation step you can use rembg just typing `rembg` in your terminal window.
 
-The `rembg` command has 3 subcommands, one for each input type:
+The `rembg` command has 4 subcommands, one for each input type:
 - `i` for files
 - `p` for folders
 - `s` for http server
+- `b` for RGB24 pixel binary stream
 
 You can get help about the main command using:
 
 ```
 rembg --help
 ```
 
@@ -209,14 +210,37 @@
 
 Remove the background from an uploaded image
 
 ```
 curl -s -F file=@/path/to/input.jpg "http://localhost:5000"  -o output.png
 ```
 
+### rembg `b`
+
+Process a sequence of RGB24 images from stdin. This is intended to be used with another program, such as FFMPEG, that outputs RGB24 pixel data to stdout, which is piped into the stdin of this program, although nothing prevents you from manually typing in images at stdin.
+
+```
+rembg b image_width image_height -o output_specifier
+```
+
+Arguments:
+
+- image_width : width of input image(s)
+- image_height : height of input image(s)
+- output_specifier: printf-style specifier for output filenames, for example if `output-%03u.png`, then output files will be named `output-000.png`, `output-001.png`, `output-002.png`, etc. Output files will be saved in PNG format regardless of the extension specified. You can omit it to write results to stdout.
+
+Example usage with FFMPEG:
+
+```
+ffmpeg -i input.mp4 -ss 10 -an -f rawvideo -pix_fmt rgb24 pipe:1 | rembg b 1280 720 -o folder/output-%03u.png
+```
+
+The width and height values must match the dimension of output images from FFMPEG. Note for FFMPEG, the "`-an -f rawvideo -pix_fmt rgb24 pipe:1`" part is required for the whole thing to work.
+
+
 ## Usage as a library
 
 Input and output as bytes
 
 ```python
 from rembg import remove
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rembg Version: 2.0.35 Summary: Remove image
+Metadata-Version: 2.1 Name: rembg Version: 2.0.36 Summary: Remove image
 background Home-page: https://github.com/danielgatis/rembg Author: Daniel Gatis
 Author-email: danielgatis@gmail.com License: UNKNOWN Keywords:
 remove,background,u2net Platform: UNKNOWN Classifier: License :: OSI Approved
 :: MIT License Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
@@ -51,78 +51,92 @@
 ```bash pip install rembg ``` GPU support: First of all, you need to check if
 your system supports the `onnxruntime-gpu`. Go to https://onnxruntime.ai and
 check the installation matrix.
 [https://raw.githubusercontent.com/danielgatis/rembg/master/onnxruntime-
 installation-matrix.png]
 If yes, just run: ```bash pip install rembg[gpu] ``` ## Usage as a cli After
 the installation step you can use rembg just typing `rembg` in your terminal
-window. The `rembg` command has 3 subcommands, one for each input type: - `i`
-for files - `p` for folders - `s` for http server You can get help about the
-main command using: ``` rembg --help ``` As well, about all the subcommands
-using: ``` rembg  --help ``` ### rembg `i` Used when input and output are
-files. Remove the background from a remote image ``` curl -s http://input.png |
-rembg i > output.png ``` Remove the background from a local file ``` rembg i
-path/to/input.png path/to/output.png ``` Remove the background specifying a
-model ``` rembg i -m u2netp path/to/input.png path/to/output.png ``` Remove the
-background returning only the mask ``` rembg i -om path/to/input.png path/to/
-output.png ``` Remove the background applying an alpha matting ``` rembg i -
-a path/to/input.png path/to/output.png ``` Passing extras parameters ``` rembg
-i -m sam -x '{"input_labels": [1], "input_points": [[100,100]]}' path/to/
-input.png path/to/output.png ``` ### rembg `p` Used when input and output are
-folders. Remove the background from all images in a folder ``` rembg p path/to/
-input path/to/output ``` Same as before, but watching for new/changed files to
-process ``` rembg p -w path/to/input path/to/output ``` ### rembg `s` Used to
-start http server. To see the complete endpoints documentation, go to: `http://
-localhost:5000/docs`. Remove the background from an image url ``` curl -
-s "http://localhost:5000/?url=http://input.png" -o output.png ``` Remove the
-background from an uploaded image ``` curl -s -F file=@/path/to/input.jpg
-"http://localhost:5000" -o output.png ``` ## Usage as a library Input and
-output as bytes ```python from rembg import remove input_path = 'input.png'
-output_path = 'output.png' with open(input_path, 'rb') as i: with open
-(output_path, 'wb') as o: input = i.read() output = remove(input) o.write
-(output) ``` Input and output as a PIL image ```python from rembg import remove
-from PIL import Image input_path = 'input.png' output_path = 'output.png' input
-= Image.open(input_path) output = remove(input) output.save(output_path) ```
-Input and output as a numpy array ```python from rembg import remove import cv2
-input_path = 'input.png' output_path = 'output.png' input = cv2.imread
-(input_path) output = remove(input) cv2.imwrite(output_path, output) ``` How to
-iterate over files in a performatic way ```python from pathlib import Path from
-rembg import remove, new_session session = new_session() for file in Path
-('path/to/folder').glob('*.png'): input_path = str(file) output_path = str
-(file.parent / (file.stem + ".out.png")) with open(input_path, 'rb') as i: with
-open(output_path, 'wb') as o: input = i.read() output = remove(input,
-session=session) o.write(output) ``` To see a full list of examples on how to
-use rembg, go to the [examples](USAGE.md) page. ## Usage as a docker Just
-replace the `rembg` command for `docker run danielgatis/rembg`. Try this: ```
-docker run danielgatis/rembg i path/to/input.png path/to/output.png ``` ##
-Models All models are downloaded and saved in the user home folder in the
-`.u2net` directory. The available models are: - u2net ([download](https://
-github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source]
-(https://github.com/xuebinqin/U-2-Net)): A pre-trained model for general use
-cases. - u2netp ([download](https://github.com/danielgatis/rembg/releases/
-download/v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)):
-A lightweight version of u2net model. - u2net_human_seg ([download](https://
-github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx),
-[source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for human
-segmentation. - u2net_cloth_seg ([download](https://github.com/danielgatis/
-rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx), [source](https://
-github.com/levindabhi/cloth-segmentation)): A pre-trained model for Cloths
-Parsing from human portrait. Here clothes are parsed into 3 category: Upper
-body, Lower body and Full body. - silueta ([download](https://github.com/
-danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://
-github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is
-reduced to 43Mb. - isnet-general-use ([download](https://github.com/
-danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source]
-(https://github.com/xuebinqin/DIS)): A new pre-trained model for general use
-cases. - sam ([download encoder](https://github.com/danielgatis/rembg/releases/
-download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://
-github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-
-quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A
-pre-trained model for any use cases. ### Some differences between the models
-result
+window. The `rembg` command has 4 subcommands, one for each input type: - `i`
+for files - `p` for folders - `s` for http server - `b` for RGB24 pixel binary
+stream You can get help about the main command using: ``` rembg --help ``` As
+well, about all the subcommands using: ``` rembg  --help ``` ### rembg `i` Used
+when input and output are files. Remove the background from a remote image ```
+curl -s http://input.png | rembg i > output.png ``` Remove the background from
+a local file ``` rembg i path/to/input.png path/to/output.png ``` Remove the
+background specifying a model ``` rembg i -m u2netp path/to/input.png path/to/
+output.png ``` Remove the background returning only the mask ``` rembg i -om
+path/to/input.png path/to/output.png ``` Remove the background applying an
+alpha matting ``` rembg i -a path/to/input.png path/to/output.png ``` Passing
+extras parameters ``` rembg i -m sam -x '{"input_labels": [1], "input_points":
+[[100,100]]}' path/to/input.png path/to/output.png ``` ### rembg `p` Used when
+input and output are folders. Remove the background from all images in a folder
+``` rembg p path/to/input path/to/output ``` Same as before, but watching for
+new/changed files to process ``` rembg p -w path/to/input path/to/output ```
+### rembg `s` Used to start http server. To see the complete endpoints
+documentation, go to: `http://localhost:5000/docs`. Remove the background from
+an image url ``` curl -s "http://localhost:5000/?url=http://input.png" -
+o output.png ``` Remove the background from an uploaded image ``` curl -s -
+F file=@/path/to/input.jpg "http://localhost:5000" -o output.png ``` ### rembg
+`b` Process a sequence of RGB24 images from stdin. This is intended to be used
+with another program, such as FFMPEG, that outputs RGB24 pixel data to stdout,
+which is piped into the stdin of this program, although nothing prevents you
+from manually typing in images at stdin. ``` rembg b image_width image_height -
+o output_specifier ``` Arguments: - image_width : width of input image(s) -
+image_height : height of input image(s) - output_specifier: printf-style
+specifier for output filenames, for example if `output-%03u.png`, then output
+files will be named `output-000.png`, `output-001.png`, `output-002.png`, etc.
+Output files will be saved in PNG format regardless of the extension specified.
+You can omit it to write results to stdout. Example usage with FFMPEG: ```
+ffmpeg -i input.mp4 -ss 10 -an -f rawvideo -pix_fmt rgb24 pipe:1 | rembg b 1280
+720 -o folder/output-%03u.png ``` The width and height values must match the
+dimension of output images from FFMPEG. Note for FFMPEG, the "`-an -f rawvideo
+-pix_fmt rgb24 pipe:1`" part is required for the whole thing to work. ## Usage
+as a library Input and output as bytes ```python from rembg import remove
+input_path = 'input.png' output_path = 'output.png' with open(input_path, 'rb')
+as i: with open(output_path, 'wb') as o: input = i.read() output = remove
+(input) o.write(output) ``` Input and output as a PIL image ```python from
+rembg import remove from PIL import Image input_path = 'input.png' output_path
+= 'output.png' input = Image.open(input_path) output = remove(input)
+output.save(output_path) ``` Input and output as a numpy array ```python from
+rembg import remove import cv2 input_path = 'input.png' output_path =
+'output.png' input = cv2.imread(input_path) output = remove(input) cv2.imwrite
+(output_path, output) ``` How to iterate over files in a performatic way
+```python from pathlib import Path from rembg import remove, new_session
+session = new_session() for file in Path('path/to/folder').glob('*.png'):
+input_path = str(file) output_path = str(file.parent / (file.stem +
+".out.png")) with open(input_path, 'rb') as i: with open(output_path, 'wb') as
+o: input = i.read() output = remove(input, session=session) o.write(output) ```
+To see a full list of examples on how to use rembg, go to the [examples]
+(USAGE.md) page. ## Usage as a docker Just replace the `rembg` command for
+`docker run danielgatis/rembg`. Try this: ``` docker run danielgatis/rembg i
+path/to/input.png path/to/output.png ``` ## Models All models are downloaded
+and saved in the user home folder in the `.u2net` directory. The available
+models are: - u2net ([download](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/u2net.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A
+pre-trained model for general use cases. - u2netp ([download](https://
+github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx), [source]
+(https://github.com/xuebinqin/U-2-Net)): A lightweight version of u2net model.
+- u2net_human_seg ([download](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/u2net_human_seg.onnx), [source](https://github.com/xuebinqin/U-
+2-Net)): A pre-trained model for human segmentation. - u2net_cloth_seg (
+[download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/
+u2net_cloth_seg.onnx), [source](https://github.com/levindabhi/cloth-
+segmentation)): A pre-trained model for Cloths Parsing from human portrait.
+Here clothes are parsed into 3 category: Upper body, Lower body and Full body.
+- silueta ([download](https://github.com/danielgatis/rembg/releases/download/
+v0.0.0/silueta.onnx), [source](https://github.com/xuebinqin/U-2-Net/issues/
+295)): Same as u2net but the size is reduced to 43Mb. - isnet-general-use (
+[download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-
+general-use.onnx), [source](https://github.com/xuebinqin/DIS)): A new pre-
+trained model for general use cases. - sam ([download encoder](https://
+github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-
+quant.onnx), [download decoder](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/vit_b-decoder-quant.onnx), [source](https://github.com/
+facebookresearch/segment-anything)): A pre-trained model for any use cases. ###
+Some differences between the models result
 original                   u2net                      u2netp                     u2net_human_seg            u2net_cloth_seg            silueta                    isnet-general-use          sam
 [https://                  [https://                  [https://                  [https://                  [https://                  [https://                  [https://                  [https://
 raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/
 danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/
 tests/fixtures/car-1.jpg]  tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-1.isnet- tests/results/car-
                            1.u2net.png]               1.u2netp.png]              1.u2net_human_seg.png]     1.u2net_cloth_seg.png]     1.silueta.png]             general-use.png]           1.sam.png]
 ### How to train your own model If You need more fine tunned models try this:
```

### Comparing `rembg-2.0.35/README.md` & `rembg-2.0.36/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -90,18 +90,19 @@
 pip install rembg[gpu]
 ```
 
 ## Usage as a cli
 
 After the installation step you can use rembg just typing `rembg` in your terminal window.
 
-The `rembg` command has 3 subcommands, one for each input type:
+The `rembg` command has 4 subcommands, one for each input type:
 - `i` for files
 - `p` for folders
 - `s` for http server
+- `b` for RGB24 pixel binary stream
 
 You can get help about the main command using:
 
 ```
 rembg --help
 ```
 
@@ -182,14 +183,37 @@
 
 Remove the background from an uploaded image
 
 ```
 curl -s -F file=@/path/to/input.jpg "http://localhost:5000"  -o output.png
 ```
 
+### rembg `b`
+
+Process a sequence of RGB24 images from stdin. This is intended to be used with another program, such as FFMPEG, that outputs RGB24 pixel data to stdout, which is piped into the stdin of this program, although nothing prevents you from manually typing in images at stdin.
+
+```
+rembg b image_width image_height -o output_specifier
+```
+
+Arguments:
+
+- image_width : width of input image(s)
+- image_height : height of input image(s)
+- output_specifier: printf-style specifier for output filenames, for example if `output-%03u.png`, then output files will be named `output-000.png`, `output-001.png`, `output-002.png`, etc. Output files will be saved in PNG format regardless of the extension specified. You can omit it to write results to stdout.
+
+Example usage with FFMPEG:
+
+```
+ffmpeg -i input.mp4 -ss 10 -an -f rawvideo -pix_fmt rgb24 pipe:1 | rembg b 1280 720 -o folder/output-%03u.png
+```
+
+The width and height values must match the dimension of output images from FFMPEG. Note for FFMPEG, the "`-an -f rawvideo -pix_fmt rgb24 pipe:1`" part is required for the whole thing to work.
+
+
 ## Usage as a library
 
 Input and output as bytes
 
 ```python
 from rembg import remove
```

#### html2text {}

```diff
@@ -37,78 +37,92 @@
 ```bash pip install rembg ``` GPU support: First of all, you need to check if
 your system supports the `onnxruntime-gpu`. Go to https://onnxruntime.ai and
 check the installation matrix.
 [https://raw.githubusercontent.com/danielgatis/rembg/master/onnxruntime-
 installation-matrix.png]
 If yes, just run: ```bash pip install rembg[gpu] ``` ## Usage as a cli After
 the installation step you can use rembg just typing `rembg` in your terminal
-window. The `rembg` command has 3 subcommands, one for each input type: - `i`
-for files - `p` for folders - `s` for http server You can get help about the
-main command using: ``` rembg --help ``` As well, about all the subcommands
-using: ``` rembg  --help ``` ### rembg `i` Used when input and output are
-files. Remove the background from a remote image ``` curl -s http://input.png |
-rembg i > output.png ``` Remove the background from a local file ``` rembg i
-path/to/input.png path/to/output.png ``` Remove the background specifying a
-model ``` rembg i -m u2netp path/to/input.png path/to/output.png ``` Remove the
-background returning only the mask ``` rembg i -om path/to/input.png path/to/
-output.png ``` Remove the background applying an alpha matting ``` rembg i -
-a path/to/input.png path/to/output.png ``` Passing extras parameters ``` rembg
-i -m sam -x '{"input_labels": [1], "input_points": [[100,100]]}' path/to/
-input.png path/to/output.png ``` ### rembg `p` Used when input and output are
-folders. Remove the background from all images in a folder ``` rembg p path/to/
-input path/to/output ``` Same as before, but watching for new/changed files to
-process ``` rembg p -w path/to/input path/to/output ``` ### rembg `s` Used to
-start http server. To see the complete endpoints documentation, go to: `http://
-localhost:5000/docs`. Remove the background from an image url ``` curl -
-s "http://localhost:5000/?url=http://input.png" -o output.png ``` Remove the
-background from an uploaded image ``` curl -s -F file=@/path/to/input.jpg
-"http://localhost:5000" -o output.png ``` ## Usage as a library Input and
-output as bytes ```python from rembg import remove input_path = 'input.png'
-output_path = 'output.png' with open(input_path, 'rb') as i: with open
-(output_path, 'wb') as o: input = i.read() output = remove(input) o.write
-(output) ``` Input and output as a PIL image ```python from rembg import remove
-from PIL import Image input_path = 'input.png' output_path = 'output.png' input
-= Image.open(input_path) output = remove(input) output.save(output_path) ```
-Input and output as a numpy array ```python from rembg import remove import cv2
-input_path = 'input.png' output_path = 'output.png' input = cv2.imread
-(input_path) output = remove(input) cv2.imwrite(output_path, output) ``` How to
-iterate over files in a performatic way ```python from pathlib import Path from
-rembg import remove, new_session session = new_session() for file in Path
-('path/to/folder').glob('*.png'): input_path = str(file) output_path = str
-(file.parent / (file.stem + ".out.png")) with open(input_path, 'rb') as i: with
-open(output_path, 'wb') as o: input = i.read() output = remove(input,
-session=session) o.write(output) ``` To see a full list of examples on how to
-use rembg, go to the [examples](USAGE.md) page. ## Usage as a docker Just
-replace the `rembg` command for `docker run danielgatis/rembg`. Try this: ```
-docker run danielgatis/rembg i path/to/input.png path/to/output.png ``` ##
-Models All models are downloaded and saved in the user home folder in the
-`.u2net` directory. The available models are: - u2net ([download](https://
-github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source]
-(https://github.com/xuebinqin/U-2-Net)): A pre-trained model for general use
-cases. - u2netp ([download](https://github.com/danielgatis/rembg/releases/
-download/v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)):
-A lightweight version of u2net model. - u2net_human_seg ([download](https://
-github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx),
-[source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for human
-segmentation. - u2net_cloth_seg ([download](https://github.com/danielgatis/
-rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx), [source](https://
-github.com/levindabhi/cloth-segmentation)): A pre-trained model for Cloths
-Parsing from human portrait. Here clothes are parsed into 3 category: Upper
-body, Lower body and Full body. - silueta ([download](https://github.com/
-danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://
-github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is
-reduced to 43Mb. - isnet-general-use ([download](https://github.com/
-danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source]
-(https://github.com/xuebinqin/DIS)): A new pre-trained model for general use
-cases. - sam ([download encoder](https://github.com/danielgatis/rembg/releases/
-download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://
-github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-
-quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A
-pre-trained model for any use cases. ### Some differences between the models
-result
+window. The `rembg` command has 4 subcommands, one for each input type: - `i`
+for files - `p` for folders - `s` for http server - `b` for RGB24 pixel binary
+stream You can get help about the main command using: ``` rembg --help ``` As
+well, about all the subcommands using: ``` rembg  --help ``` ### rembg `i` Used
+when input and output are files. Remove the background from a remote image ```
+curl -s http://input.png | rembg i > output.png ``` Remove the background from
+a local file ``` rembg i path/to/input.png path/to/output.png ``` Remove the
+background specifying a model ``` rembg i -m u2netp path/to/input.png path/to/
+output.png ``` Remove the background returning only the mask ``` rembg i -om
+path/to/input.png path/to/output.png ``` Remove the background applying an
+alpha matting ``` rembg i -a path/to/input.png path/to/output.png ``` Passing
+extras parameters ``` rembg i -m sam -x '{"input_labels": [1], "input_points":
+[[100,100]]}' path/to/input.png path/to/output.png ``` ### rembg `p` Used when
+input and output are folders. Remove the background from all images in a folder
+``` rembg p path/to/input path/to/output ``` Same as before, but watching for
+new/changed files to process ``` rembg p -w path/to/input path/to/output ```
+### rembg `s` Used to start http server. To see the complete endpoints
+documentation, go to: `http://localhost:5000/docs`. Remove the background from
+an image url ``` curl -s "http://localhost:5000/?url=http://input.png" -
+o output.png ``` Remove the background from an uploaded image ``` curl -s -
+F file=@/path/to/input.jpg "http://localhost:5000" -o output.png ``` ### rembg
+`b` Process a sequence of RGB24 images from stdin. This is intended to be used
+with another program, such as FFMPEG, that outputs RGB24 pixel data to stdout,
+which is piped into the stdin of this program, although nothing prevents you
+from manually typing in images at stdin. ``` rembg b image_width image_height -
+o output_specifier ``` Arguments: - image_width : width of input image(s) -
+image_height : height of input image(s) - output_specifier: printf-style
+specifier for output filenames, for example if `output-%03u.png`, then output
+files will be named `output-000.png`, `output-001.png`, `output-002.png`, etc.
+Output files will be saved in PNG format regardless of the extension specified.
+You can omit it to write results to stdout. Example usage with FFMPEG: ```
+ffmpeg -i input.mp4 -ss 10 -an -f rawvideo -pix_fmt rgb24 pipe:1 | rembg b 1280
+720 -o folder/output-%03u.png ``` The width and height values must match the
+dimension of output images from FFMPEG. Note for FFMPEG, the "`-an -f rawvideo
+-pix_fmt rgb24 pipe:1`" part is required for the whole thing to work. ## Usage
+as a library Input and output as bytes ```python from rembg import remove
+input_path = 'input.png' output_path = 'output.png' with open(input_path, 'rb')
+as i: with open(output_path, 'wb') as o: input = i.read() output = remove
+(input) o.write(output) ``` Input and output as a PIL image ```python from
+rembg import remove from PIL import Image input_path = 'input.png' output_path
+= 'output.png' input = Image.open(input_path) output = remove(input)
+output.save(output_path) ``` Input and output as a numpy array ```python from
+rembg import remove import cv2 input_path = 'input.png' output_path =
+'output.png' input = cv2.imread(input_path) output = remove(input) cv2.imwrite
+(output_path, output) ``` How to iterate over files in a performatic way
+```python from pathlib import Path from rembg import remove, new_session
+session = new_session() for file in Path('path/to/folder').glob('*.png'):
+input_path = str(file) output_path = str(file.parent / (file.stem +
+".out.png")) with open(input_path, 'rb') as i: with open(output_path, 'wb') as
+o: input = i.read() output = remove(input, session=session) o.write(output) ```
+To see a full list of examples on how to use rembg, go to the [examples]
+(USAGE.md) page. ## Usage as a docker Just replace the `rembg` command for
+`docker run danielgatis/rembg`. Try this: ``` docker run danielgatis/rembg i
+path/to/input.png path/to/output.png ``` ## Models All models are downloaded
+and saved in the user home folder in the `.u2net` directory. The available
+models are: - u2net ([download](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/u2net.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A
+pre-trained model for general use cases. - u2netp ([download](https://
+github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx), [source]
+(https://github.com/xuebinqin/U-2-Net)): A lightweight version of u2net model.
+- u2net_human_seg ([download](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/u2net_human_seg.onnx), [source](https://github.com/xuebinqin/U-
+2-Net)): A pre-trained model for human segmentation. - u2net_cloth_seg (
+[download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/
+u2net_cloth_seg.onnx), [source](https://github.com/levindabhi/cloth-
+segmentation)): A pre-trained model for Cloths Parsing from human portrait.
+Here clothes are parsed into 3 category: Upper body, Lower body and Full body.
+- silueta ([download](https://github.com/danielgatis/rembg/releases/download/
+v0.0.0/silueta.onnx), [source](https://github.com/xuebinqin/U-2-Net/issues/
+295)): Same as u2net but the size is reduced to 43Mb. - isnet-general-use (
+[download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-
+general-use.onnx), [source](https://github.com/xuebinqin/DIS)): A new pre-
+trained model for general use cases. - sam ([download encoder](https://
+github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-
+quant.onnx), [download decoder](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/vit_b-decoder-quant.onnx), [source](https://github.com/
+facebookresearch/segment-anything)): A pre-trained model for any use cases. ###
+Some differences between the models result
 original                   u2net                      u2netp                     u2net_human_seg            u2net_cloth_seg            silueta                    isnet-general-use          sam
 [https://                  [https://                  [https://                  [https://                  [https://                  [https://                  [https://                  [https://
 raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/
 danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/
 tests/fixtures/car-1.jpg]  tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-1.isnet- tests/results/car-
                            1.u2net.png]               1.u2netp.png]              1.u2net_human_seg.png]     1.u2net_cloth_seg.png]     1.silueta.png]             general-use.png]           1.sam.png]
 ### How to train your own model If You need more fine tunned models try this:
```

### Comparing `rembg-2.0.35/rembg/bg.py` & `rembg-2.0.36/rembg/bg.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     BORDER_DEFAULT,
     MORPH_ELLIPSE,
     MORPH_OPEN,
     GaussianBlur,
     getStructuringElement,
     morphologyEx,
 )
-from PIL import Image
+from PIL import Image, ImageOps
 from PIL.Image import Image as PILImage
 from pymatting.alpha.estimate_alpha_cf import estimate_alpha_cf
 from pymatting.foreground.estimate_foreground_ml import estimate_foreground_ml
 from pymatting.util.util import stack_images
 from scipy.ndimage import binary_erosion
 
 from .session_factory import new_session
@@ -109,14 +109,18 @@
     r, g, b, a = color
     colored_image = Image.new("RGBA", img.size, (r, g, b, a))
     colored_image.paste(img, mask=img)
 
     return colored_image
 
 
+def fix_image_orientation(img: PILImage) -> PILImage:
+    return ImageOps.exif_transpose(img)
+
+
 def remove(
     data: Union[bytes, PILImage, np.ndarray],
     alpha_matting: bool = False,
     alpha_matting_foreground_threshold: int = 240,
     alpha_matting_background_threshold: int = 10,
     alpha_matting_erode_size: int = 10,
     session: Optional[BaseSession] = None,
@@ -134,14 +138,17 @@
         img = Image.open(io.BytesIO(data))
     elif isinstance(data, np.ndarray):
         return_type = ReturnType.NDARRAY
         img = Image.fromarray(data)
     else:
         raise ValueError("Input type {} is not supported.".format(type(data)))
 
+    # Fix image orientation
+    img = fix_image_orientation(img)
+
     if session is None:
         session = new_session("u2net", *args, **kwargs)
 
     masks = session.predict(img, *args, **kwargs)
     cutouts = []
 
     for mask in masks:
```

### Comparing `rembg-2.0.35/rembg/commands/i_command.py` & `rembg-2.0.36/rembg/commands/i_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.35/rembg/commands/p_command.py` & `rembg-2.0.36/rembg/commands/p_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.35/rembg/commands/s_command.py` & `rembg-2.0.36/rembg/commands/s_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.35/rembg/session_factory.py` & `rembg-2.0.36/rembg/session_factory.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.35/rembg/sessions/__init__.py` & `rembg-2.0.36/rembg/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.35/rembg/sessions/base.py` & `rembg-2.0.36/rembg/sessions/base.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.35/rembg/sessions/dis.py` & `rembg-2.0.36/rembg/sessions/dis.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.35/rembg/sessions/sam.py` & `rembg-2.0.36/rembg/sessions/sam.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.35/rembg/sessions/silueta.py` & `rembg-2.0.36/rembg/sessions/silueta.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.35/rembg/sessions/u2net.py` & `rembg-2.0.36/rembg/sessions/u2net.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.35/rembg/sessions/u2net_cloth_seg.py` & `rembg-2.0.36/rembg/sessions/u2net_cloth_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.35/rembg/sessions/u2net_human_seg.py` & `rembg-2.0.36/rembg/sessions/u2net_human_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.35/rembg/sessions/u2netp.py` & `rembg-2.0.36/rembg/sessions/u2netp.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.35/rembg.egg-info/PKG-INFO` & `rembg-2.0.36/rembg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.35
+Version: 2.0.36
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 License: UNKNOWN
 Keywords: remove,background,u2net
 Platform: UNKNOWN
@@ -117,18 +117,19 @@
 pip install rembg[gpu]
 ```
 
 ## Usage as a cli
 
 After the installation step you can use rembg just typing `rembg` in your terminal window.
 
-The `rembg` command has 3 subcommands, one for each input type:
+The `rembg` command has 4 subcommands, one for each input type:
 - `i` for files
 - `p` for folders
 - `s` for http server
+- `b` for RGB24 pixel binary stream
 
 You can get help about the main command using:
 
 ```
 rembg --help
 ```
 
@@ -209,14 +210,37 @@
 
 Remove the background from an uploaded image
 
 ```
 curl -s -F file=@/path/to/input.jpg "http://localhost:5000"  -o output.png
 ```
 
+### rembg `b`
+
+Process a sequence of RGB24 images from stdin. This is intended to be used with another program, such as FFMPEG, that outputs RGB24 pixel data to stdout, which is piped into the stdin of this program, although nothing prevents you from manually typing in images at stdin.
+
+```
+rembg b image_width image_height -o output_specifier
+```
+
+Arguments:
+
+- image_width : width of input image(s)
+- image_height : height of input image(s)
+- output_specifier: printf-style specifier for output filenames, for example if `output-%03u.png`, then output files will be named `output-000.png`, `output-001.png`, `output-002.png`, etc. Output files will be saved in PNG format regardless of the extension specified. You can omit it to write results to stdout.
+
+Example usage with FFMPEG:
+
+```
+ffmpeg -i input.mp4 -ss 10 -an -f rawvideo -pix_fmt rgb24 pipe:1 | rembg b 1280 720 -o folder/output-%03u.png
+```
+
+The width and height values must match the dimension of output images from FFMPEG. Note for FFMPEG, the "`-an -f rawvideo -pix_fmt rgb24 pipe:1`" part is required for the whole thing to work.
+
+
 ## Usage as a library
 
 Input and output as bytes
 
 ```python
 from rembg import remove
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rembg Version: 2.0.35 Summary: Remove image
+Metadata-Version: 2.1 Name: rembg Version: 2.0.36 Summary: Remove image
 background Home-page: https://github.com/danielgatis/rembg Author: Daniel Gatis
 Author-email: danielgatis@gmail.com License: UNKNOWN Keywords:
 remove,background,u2net Platform: UNKNOWN Classifier: License :: OSI Approved
 :: MIT License Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
@@ -51,78 +51,92 @@
 ```bash pip install rembg ``` GPU support: First of all, you need to check if
 your system supports the `onnxruntime-gpu`. Go to https://onnxruntime.ai and
 check the installation matrix.
 [https://raw.githubusercontent.com/danielgatis/rembg/master/onnxruntime-
 installation-matrix.png]
 If yes, just run: ```bash pip install rembg[gpu] ``` ## Usage as a cli After
 the installation step you can use rembg just typing `rembg` in your terminal
-window. The `rembg` command has 3 subcommands, one for each input type: - `i`
-for files - `p` for folders - `s` for http server You can get help about the
-main command using: ``` rembg --help ``` As well, about all the subcommands
-using: ``` rembg  --help ``` ### rembg `i` Used when input and output are
-files. Remove the background from a remote image ``` curl -s http://input.png |
-rembg i > output.png ``` Remove the background from a local file ``` rembg i
-path/to/input.png path/to/output.png ``` Remove the background specifying a
-model ``` rembg i -m u2netp path/to/input.png path/to/output.png ``` Remove the
-background returning only the mask ``` rembg i -om path/to/input.png path/to/
-output.png ``` Remove the background applying an alpha matting ``` rembg i -
-a path/to/input.png path/to/output.png ``` Passing extras parameters ``` rembg
-i -m sam -x '{"input_labels": [1], "input_points": [[100,100]]}' path/to/
-input.png path/to/output.png ``` ### rembg `p` Used when input and output are
-folders. Remove the background from all images in a folder ``` rembg p path/to/
-input path/to/output ``` Same as before, but watching for new/changed files to
-process ``` rembg p -w path/to/input path/to/output ``` ### rembg `s` Used to
-start http server. To see the complete endpoints documentation, go to: `http://
-localhost:5000/docs`. Remove the background from an image url ``` curl -
-s "http://localhost:5000/?url=http://input.png" -o output.png ``` Remove the
-background from an uploaded image ``` curl -s -F file=@/path/to/input.jpg
-"http://localhost:5000" -o output.png ``` ## Usage as a library Input and
-output as bytes ```python from rembg import remove input_path = 'input.png'
-output_path = 'output.png' with open(input_path, 'rb') as i: with open
-(output_path, 'wb') as o: input = i.read() output = remove(input) o.write
-(output) ``` Input and output as a PIL image ```python from rembg import remove
-from PIL import Image input_path = 'input.png' output_path = 'output.png' input
-= Image.open(input_path) output = remove(input) output.save(output_path) ```
-Input and output as a numpy array ```python from rembg import remove import cv2
-input_path = 'input.png' output_path = 'output.png' input = cv2.imread
-(input_path) output = remove(input) cv2.imwrite(output_path, output) ``` How to
-iterate over files in a performatic way ```python from pathlib import Path from
-rembg import remove, new_session session = new_session() for file in Path
-('path/to/folder').glob('*.png'): input_path = str(file) output_path = str
-(file.parent / (file.stem + ".out.png")) with open(input_path, 'rb') as i: with
-open(output_path, 'wb') as o: input = i.read() output = remove(input,
-session=session) o.write(output) ``` To see a full list of examples on how to
-use rembg, go to the [examples](USAGE.md) page. ## Usage as a docker Just
-replace the `rembg` command for `docker run danielgatis/rembg`. Try this: ```
-docker run danielgatis/rembg i path/to/input.png path/to/output.png ``` ##
-Models All models are downloaded and saved in the user home folder in the
-`.u2net` directory. The available models are: - u2net ([download](https://
-github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source]
-(https://github.com/xuebinqin/U-2-Net)): A pre-trained model for general use
-cases. - u2netp ([download](https://github.com/danielgatis/rembg/releases/
-download/v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)):
-A lightweight version of u2net model. - u2net_human_seg ([download](https://
-github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx),
-[source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for human
-segmentation. - u2net_cloth_seg ([download](https://github.com/danielgatis/
-rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx), [source](https://
-github.com/levindabhi/cloth-segmentation)): A pre-trained model for Cloths
-Parsing from human portrait. Here clothes are parsed into 3 category: Upper
-body, Lower body and Full body. - silueta ([download](https://github.com/
-danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://
-github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is
-reduced to 43Mb. - isnet-general-use ([download](https://github.com/
-danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source]
-(https://github.com/xuebinqin/DIS)): A new pre-trained model for general use
-cases. - sam ([download encoder](https://github.com/danielgatis/rembg/releases/
-download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://
-github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-
-quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A
-pre-trained model for any use cases. ### Some differences between the models
-result
+window. The `rembg` command has 4 subcommands, one for each input type: - `i`
+for files - `p` for folders - `s` for http server - `b` for RGB24 pixel binary
+stream You can get help about the main command using: ``` rembg --help ``` As
+well, about all the subcommands using: ``` rembg  --help ``` ### rembg `i` Used
+when input and output are files. Remove the background from a remote image ```
+curl -s http://input.png | rembg i > output.png ``` Remove the background from
+a local file ``` rembg i path/to/input.png path/to/output.png ``` Remove the
+background specifying a model ``` rembg i -m u2netp path/to/input.png path/to/
+output.png ``` Remove the background returning only the mask ``` rembg i -om
+path/to/input.png path/to/output.png ``` Remove the background applying an
+alpha matting ``` rembg i -a path/to/input.png path/to/output.png ``` Passing
+extras parameters ``` rembg i -m sam -x '{"input_labels": [1], "input_points":
+[[100,100]]}' path/to/input.png path/to/output.png ``` ### rembg `p` Used when
+input and output are folders. Remove the background from all images in a folder
+``` rembg p path/to/input path/to/output ``` Same as before, but watching for
+new/changed files to process ``` rembg p -w path/to/input path/to/output ```
+### rembg `s` Used to start http server. To see the complete endpoints
+documentation, go to: `http://localhost:5000/docs`. Remove the background from
+an image url ``` curl -s "http://localhost:5000/?url=http://input.png" -
+o output.png ``` Remove the background from an uploaded image ``` curl -s -
+F file=@/path/to/input.jpg "http://localhost:5000" -o output.png ``` ### rembg
+`b` Process a sequence of RGB24 images from stdin. This is intended to be used
+with another program, such as FFMPEG, that outputs RGB24 pixel data to stdout,
+which is piped into the stdin of this program, although nothing prevents you
+from manually typing in images at stdin. ``` rembg b image_width image_height -
+o output_specifier ``` Arguments: - image_width : width of input image(s) -
+image_height : height of input image(s) - output_specifier: printf-style
+specifier for output filenames, for example if `output-%03u.png`, then output
+files will be named `output-000.png`, `output-001.png`, `output-002.png`, etc.
+Output files will be saved in PNG format regardless of the extension specified.
+You can omit it to write results to stdout. Example usage with FFMPEG: ```
+ffmpeg -i input.mp4 -ss 10 -an -f rawvideo -pix_fmt rgb24 pipe:1 | rembg b 1280
+720 -o folder/output-%03u.png ``` The width and height values must match the
+dimension of output images from FFMPEG. Note for FFMPEG, the "`-an -f rawvideo
+-pix_fmt rgb24 pipe:1`" part is required for the whole thing to work. ## Usage
+as a library Input and output as bytes ```python from rembg import remove
+input_path = 'input.png' output_path = 'output.png' with open(input_path, 'rb')
+as i: with open(output_path, 'wb') as o: input = i.read() output = remove
+(input) o.write(output) ``` Input and output as a PIL image ```python from
+rembg import remove from PIL import Image input_path = 'input.png' output_path
+= 'output.png' input = Image.open(input_path) output = remove(input)
+output.save(output_path) ``` Input and output as a numpy array ```python from
+rembg import remove import cv2 input_path = 'input.png' output_path =
+'output.png' input = cv2.imread(input_path) output = remove(input) cv2.imwrite
+(output_path, output) ``` How to iterate over files in a performatic way
+```python from pathlib import Path from rembg import remove, new_session
+session = new_session() for file in Path('path/to/folder').glob('*.png'):
+input_path = str(file) output_path = str(file.parent / (file.stem +
+".out.png")) with open(input_path, 'rb') as i: with open(output_path, 'wb') as
+o: input = i.read() output = remove(input, session=session) o.write(output) ```
+To see a full list of examples on how to use rembg, go to the [examples]
+(USAGE.md) page. ## Usage as a docker Just replace the `rembg` command for
+`docker run danielgatis/rembg`. Try this: ``` docker run danielgatis/rembg i
+path/to/input.png path/to/output.png ``` ## Models All models are downloaded
+and saved in the user home folder in the `.u2net` directory. The available
+models are: - u2net ([download](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/u2net.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A
+pre-trained model for general use cases. - u2netp ([download](https://
+github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx), [source]
+(https://github.com/xuebinqin/U-2-Net)): A lightweight version of u2net model.
+- u2net_human_seg ([download](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/u2net_human_seg.onnx), [source](https://github.com/xuebinqin/U-
+2-Net)): A pre-trained model for human segmentation. - u2net_cloth_seg (
+[download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/
+u2net_cloth_seg.onnx), [source](https://github.com/levindabhi/cloth-
+segmentation)): A pre-trained model for Cloths Parsing from human portrait.
+Here clothes are parsed into 3 category: Upper body, Lower body and Full body.
+- silueta ([download](https://github.com/danielgatis/rembg/releases/download/
+v0.0.0/silueta.onnx), [source](https://github.com/xuebinqin/U-2-Net/issues/
+295)): Same as u2net but the size is reduced to 43Mb. - isnet-general-use (
+[download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-
+general-use.onnx), [source](https://github.com/xuebinqin/DIS)): A new pre-
+trained model for general use cases. - sam ([download encoder](https://
+github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-
+quant.onnx), [download decoder](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/vit_b-decoder-quant.onnx), [source](https://github.com/
+facebookresearch/segment-anything)): A pre-trained model for any use cases. ###
+Some differences between the models result
 original                   u2net                      u2netp                     u2net_human_seg            u2net_cloth_seg            silueta                    isnet-general-use          sam
 [https://                  [https://                  [https://                  [https://                  [https://                  [https://                  [https://                  [https://
 raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/ raw.githubusercontent.com/
 danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/  danielgatis/rembg/master/
 tests/fixtures/car-1.jpg]  tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-         tests/results/car-1.isnet- tests/results/car-
                            1.u2net.png]               1.u2netp.png]              1.u2net_human_seg.png]     1.u2net_cloth_seg.png]     1.silueta.png]             general-use.png]           1.sam.png]
 ### How to train your own model If You need more fine tunned models try this:
```

### Comparing `rembg-2.0.35/rembg.egg-info/SOURCES.txt` & `rembg-2.0.36/rembg.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 rembg.egg-info/PKG-INFO
 rembg.egg-info/SOURCES.txt
 rembg.egg-info/dependency_links.txt
 rembg.egg-info/entry_points.txt
 rembg.egg-info/requires.txt
 rembg.egg-info/top_level.txt
 rembg/commands/__init__.py
+rembg/commands/b_command.py
 rembg/commands/i_command.py
 rembg/commands/p_command.py
 rembg/commands/s_command.py
 rembg/sessions/__init__.py
 rembg/sessions/base.py
 rembg/sessions/dis.py
 rembg/sessions/sam.py
```

### Comparing `rembg-2.0.35/setup.py` & `rembg-2.0.36/setup.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.35/versioneer.py` & `rembg-2.0.36/versioneer.py`

 * *Files identical despite different names*

