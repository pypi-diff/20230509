# Comparing `tmp/solidpython2-2.0.1.tar.gz` & `tmp/solidpython2-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidpython2-2.0.1.tar", max compression
+gzip compressed data, was "solidpython2-2.0.2.tar", max compression
```

## Comparing `solidpython2-2.0.1.tar` & `solidpython2-2.0.2.tar`

### file list

```diff
@@ -1,173 +1,253 @@
--rw-r--r--   0        0        0    22930 2023-03-15 13:23:46.110122 solidpython2-2.0.1/README.rst
--rw-r--r--   0        0        0     1116 2023-04-11 17:10:49.921489 solidpython2-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      108 2023-03-16 11:22:53.244444 solidpython2-2.0.1/solid2/__init__.py
--rw-r--r--   0        0        0     1687 2023-03-20 22:35:21.713279 solidpython2-2.0.1/solid2/config.py
--rw-r--r--   0        0        0      381 2023-03-15 13:33:52.945033 solidpython2-2.0.1/solid2/core/__init__.py
--rw-r--r--   0        0        0       53 2023-03-20 22:35:21.713279 solidpython2-2.0.1/solid2/core/builtins/__init__.py
--rw-r--r--   0        0        0     3633 2023-03-20 22:35:21.713279 solidpython2-2.0.1/solid2/core/builtins/convenience.py
--rw-r--r--   0        0        0     1040 2023-03-20 22:35:21.713279 solidpython2-2.0.1/solid2/core/builtins/implicit.primitives
--rw-r--r--   0        0        0      754 2023-03-20 22:35:21.713279 solidpython2-2.0.1/solid2/core/builtins/openscad.mutators
--rw-r--r--   0        0        0     1968 2023-03-20 22:35:21.713279 solidpython2-2.0.1/solid2/core/builtins/openscad.primitives
--rw-r--r--   0        0        0    25400 2023-03-20 22:35:21.713279 solidpython2-2.0.1/solid2/core/builtins/openscad_primitives.py
--rw-r--r--   0        0        0      367 2023-03-20 22:35:21.713279 solidpython2-2.0.1/solid2/core/builtins/primitives.py
--rw-r--r--   0        0        0      938 2022-09-03 20:01:15.234639 solidpython2-2.0.1/solid2/core/extension_manager.py
--rw-r--r--   0        0        0       32 2023-03-19 13:30:20.199884 solidpython2-2.0.1/solid2/core/object_base/__init__.py
--rw-r--r--   0        0        0     3522 2023-03-20 14:58:07.769013 solidpython2-2.0.1/solid2/core/object_base/access_syntax_mixin.py
--rw-r--r--   0        0        0     6839 2023-03-23 17:47:21.609266 solidpython2-2.0.1/solid2/core/object_base/object_base_impl.py
--rw-r--r--   0        0        0     2253 2023-03-20 14:58:07.769013 solidpython2-2.0.1/solid2/core/object_base/operator_mixin.py
--rw-r--r--   0        0        0     3994 2022-08-12 15:59:10.183877 solidpython2-2.0.1/solid2/core/object_factory.py
--rw-r--r--   0        0        0     3469 2023-03-21 17:35:24.083900 solidpython2-2.0.1/solid2/core/parse_scad.py
--rw-r--r--   0        0        0     5493 2023-03-19 13:30:20.199884 solidpython2-2.0.1/solid2/core/scad_import.py
--rw-r--r--   0        0        0     3049 2023-03-23 17:47:21.609266 solidpython2-2.0.1/solid2/core/scad_render.py
--rw-r--r--   0        0        0     2152 2022-08-12 15:59:10.183877 solidpython2-2.0.1/solid2/core/utils.py
--rwxr-xr-x   0        0        0      559 2023-03-15 22:53:12.381332 solidpython2-2.0.1/solid2/examples/01-basics.py
--rwxr-xr-x   0        0        0      846 2023-03-15 22:55:23.517187 solidpython2-2.0.1/solid2/examples/02-vars-and-operators.py
--rwxr-xr-x   0        0        0      647 2022-08-12 15:59:10.183877 solidpython2-2.0.1/solid2/examples/03-debug-background.py
--rwxr-xr-x   0        0        0     1272 2022-08-12 15:59:10.183877 solidpython2-2.0.1/solid2/examples/04-convenience.py
--rwxr-xr-x   0        0        0      934 2022-08-12 15:59:10.183877 solidpython2-2.0.1/solid2/examples/05-access-style-syntax.py
--rwxr-xr-x   0        0        0     1182 2023-03-15 22:58:40.236989 solidpython2-2.0.1/solid2/examples/06-functions.py
--rwxr-xr-x   0        0        0      527 2023-03-19 11:58:59.349891 solidpython2-2.0.1/solid2/examples/07-libs-bosl2-attachable.py
--rw-r--r--   0        0        0     3329 2023-04-11 09:39:25.912704 solidpython2-2.0.1/solid2/examples/07-libs-bosl2-logo.py
--rwxr-xr-x   0        0        0     1762 2023-03-20 14:58:07.769013 solidpython2-2.0.1/solid2/examples/07-libs-bosl2.py
--rwxr-xr-x   0        0        0      620 2022-08-12 15:59:10.183877 solidpython2-2.0.1/solid2/examples/07-libs.py
--rwxr-xr-x   0        0        0     2448 2023-03-20 14:58:07.769013 solidpython2-2.0.1/solid2/examples/08-extensions.py
--rwxr-xr-x   0        0        0     1675 2022-12-15 10:19:43.476714 solidpython2-2.0.1/solid2/examples/09-code-attach-extension.py
--rwxr-xr-x   0        0        0      889 2023-03-19 12:43:05.625475 solidpython2-2.0.1/solid2/examples/10-customizer.py
--rw-r--r--   0        0        0      158 2022-08-12 15:59:10.183877 solidpython2-2.0.1/solid2/examples/11-font/LICENSE_README
--rw-r--r--   0        0        0    47404 2022-08-12 15:59:10.187877 solidpython2-2.0.1/solid2/examples/11-font/RichEatin.otf
--rwxr-xr-x   0        0        0      192 2023-03-15 13:23:46.114122 solidpython2-2.0.1/solid2/examples/11-fonts.py
--rwxr-xr-x   0        0        0      335 2023-03-15 13:23:46.114122 solidpython2-2.0.1/solid2/examples/12-animation.py
--rwxr-xr-x   0        0        0     2032 2023-03-19 12:43:05.625475 solidpython2-2.0.1/solid2/examples/13-animated-bouncing-ball.py
--rwxr-xr-x   0        0        0     1381 2022-08-12 15:59:10.187877 solidpython2-2.0.1/solid2/examples/14-implicitCAD.py
--rwxr-xr-x   0        0        0     1794 2022-08-12 15:59:10.187877 solidpython2-2.0.1/solid2/examples/15-implicitCAD2.py
--rwxr-xr-x   0        0        0     1102 2022-08-12 15:59:10.187877 solidpython2-2.0.1/solid2/examples/16-mazebox-bosl2.py
--rwxr-xr-x   0        0        0     2243 2023-03-15 13:23:46.114122 solidpython2-2.0.1/solid2/examples/17-greedy-scad-interface.py
--rw-r--r--   0        0        0     1196 2022-08-12 15:59:10.187877 solidpython2-2.0.1/solid2/examples/maze7.png
--rwxr-xr-x   0        0        0      293 2022-08-12 15:59:10.187877 solidpython2-2.0.1/solid2/examples/run_all_examples.py
--rw-r--r--   0        0        0        1 2022-08-12 15:59:10.187877 solidpython2-2.0.1/solid2/extensions/__init__.py
--rw-r--r--   0        0        0      210 2023-04-11 09:14:35.909512 solidpython2-2.0.1/solid2/extensions/bosl2/__init__.py
--rw-r--r--   0        0        0     3320 2023-04-11 17:06:59.193743 solidpython2-2.0.1/solid2/extensions/bosl2/affine.py
--rw-r--r--   0        0        0    13304 2023-04-11 17:07:00.797742 solidpython2-2.0.1/solid2/extensions/bosl2/attachments.py
--rw-r--r--   0        0        0      880 2023-04-11 17:07:00.089742 solidpython2-2.0.1/solid2/extensions/bosl2/ball_bearings.py
--rw-r--r--   0        0        0     7575 2023-04-11 17:06:59.361743 solidpython2-2.0.1/solid2/extensions/bosl2/beziers.py
--rw-r--r--   0        0        0    17177 2023-04-11 17:07:38.985699 solidpython2-2.0.1/solid2/extensions/bosl2/bosl2_access_syntax_mixin.py
--rw-r--r--   0        0        0     1002 2023-04-11 09:15:15.373553 solidpython2-2.0.1/solid2/extensions/bosl2/bosl2_base.py
--rw-r--r--   0        0        0      611 2023-04-11 09:15:20.845559 solidpython2-2.0.1/solid2/extensions/bosl2/bosl2_patches.py
--rw-r--r--   0        0        0    10958 2023-04-11 17:06:59.285743 solidpython2-2.0.1/solid2/extensions/bosl2/bottlecaps.py
--rw-r--r--   0        0        0     1542 2023-04-11 17:06:59.617743 solidpython2-2.0.1/solid2/extensions/bosl2/color.py
--rw-r--r--   0        0        0     7216 2023-04-11 17:06:59.181743 solidpython2-2.0.1/solid2/extensions/bosl2/comparisons.py
--rw-r--r--   0        0        0     1140 2023-04-11 17:06:59.557743 solidpython2-2.0.1/solid2/extensions/bosl2/constants.py
--rw-r--r--   0        0        0     3012 2023-04-11 17:07:00.637742 solidpython2-2.0.1/solid2/extensions/bosl2/coords.py
--rw-r--r--   0        0        0     3619 2023-04-11 17:07:00.817741 solidpython2-2.0.1/solid2/extensions/bosl2/cubetruss.py
--rw-r--r--   0        0        0    10737 2023-04-11 17:07:41.925695 solidpython2-2.0.1/solid2/extensions/bosl2/distributors.py
--rw-r--r--   0        0        0     8138 2023-04-11 17:07:00.341742 solidpython2-2.0.1/solid2/extensions/bosl2/drawing.py
--rw-r--r--   0        0        0    12656 2023-04-11 17:06:59.321743 solidpython2-2.0.1/solid2/extensions/bosl2/fnliterals.py
--rw-r--r--   0        0        0    12640 2023-04-11 17:06:59.725743 solidpython2-2.0.1/solid2/extensions/bosl2/gears.py
--rw-r--r--   0        0        0    19280 2023-04-11 17:06:59.797742 solidpython2-2.0.1/solid2/extensions/bosl2/geometry.py
--rw-r--r--   0        0        0     5048 2023-04-11 17:07:00.869741 solidpython2-2.0.1/solid2/extensions/bosl2/hinges.py
--rw-r--r--   0        0        0     9521 2023-04-11 17:07:00.721742 solidpython2-2.0.1/solid2/extensions/bosl2/joiners.py
--rw-r--r--   0        0        0     5628 2023-04-11 17:06:59.581743 solidpython2-2.0.1/solid2/extensions/bosl2/linalg.py
--rw-r--r--   0        0        0     1831 2023-04-11 17:06:59.237743 solidpython2-2.0.1/solid2/extensions/bosl2/linear_bearings.py
--rw-r--r--   0        0        0     6948 2023-04-11 17:06:59.217743 solidpython2-2.0.1/solid2/extensions/bosl2/lists.py
--rw-r--r--   0        0        0     4347 2023-04-11 17:07:00.605742 solidpython2-2.0.1/solid2/extensions/bosl2/masks2d.py
--rw-r--r--   0        0        0     8167 2023-04-11 17:07:00.289742 solidpython2-2.0.1/solid2/extensions/bosl2/masks3d.py
--rw-r--r--   0        0        0    12664 2023-04-11 17:07:00.545742 solidpython2-2.0.1/solid2/extensions/bosl2/math.py
--rw-r--r--   0        0        0     3783 2023-04-11 17:07:00.853741 solidpython2-2.0.1/solid2/extensions/bosl2/metric_screws.py
--rw-r--r--   0        0        0     1359 2023-04-11 17:07:00.825741 solidpython2-2.0.1/solid2/extensions/bosl2/modular_hose.py
--rw-r--r--   0        0        0     2335 2023-04-11 17:07:00.505742 solidpython2-2.0.1/solid2/extensions/bosl2/mutators.py
--rw-r--r--   0        0        0     1189 2023-04-11 17:07:00.645742 solidpython2-2.0.1/solid2/extensions/bosl2/nema_steppers.py
--rw-r--r--   0        0        0     6047 2023-04-11 17:07:00.905741 solidpython2-2.0.1/solid2/extensions/bosl2/openscad.py
--rw-r--r--   0        0        0     4057 2023-04-11 17:06:59.233743 solidpython2-2.0.1/solid2/extensions/bosl2/partitions.py
--rw-r--r--   0        0        0     7789 2023-04-11 17:07:00.153742 solidpython2-2.0.1/solid2/extensions/bosl2/paths.py
--rw-r--r--   0        0        0     3389 2023-04-11 17:06:59.613743 solidpython2-2.0.1/solid2/extensions/bosl2/polyhedra.py
--rw-r--r--   0        0        0     7756 2023-04-11 17:07:00.905741 solidpython2-2.0.1/solid2/extensions/bosl2/regions.py
--rw-r--r--   0        0        0    20790 2023-04-11 17:06:59.905743 solidpython2-2.0.1/solid2/extensions/bosl2/rounding.py
--rw-r--r--   0        0        0     3054 2023-04-11 17:07:00.589742 solidpython2-2.0.1/solid2/extensions/bosl2/screw_drive.py
--rw-r--r--   0        0        0    14579 2023-04-11 17:06:59.557743 solidpython2-2.0.1/solid2/extensions/bosl2/screws.py
--rw-r--r--   0        0        0    14152 2023-04-11 17:06:59.681743 solidpython2-2.0.1/solid2/extensions/bosl2/shapes2d.py
--rw-r--r--   0        0        0    26883 2023-04-11 17:07:43.537693 solidpython2-2.0.1/solid2/extensions/bosl2/shapes3d.py
--rw-r--r--   0        0        0    17226 2023-04-11 17:07:44.613692 solidpython2-2.0.1/solid2/extensions/bosl2/skin.py
--rw-r--r--   0        0        0     1597 2023-04-11 17:07:00.577742 solidpython2-2.0.1/solid2/extensions/bosl2/sliders.py
--rw-r--r--   0        0        0      679 2023-04-11 17:06:58.953744 solidpython2-2.0.1/solid2/extensions/bosl2/std.py
--rw-r--r--   0        0        0     7258 2023-04-11 17:07:00.625742 solidpython2-2.0.1/solid2/extensions/bosl2/strings.py
--rw-r--r--   0        0        0     1722 2023-04-11 17:07:00.121742 solidpython2-2.0.1/solid2/extensions/bosl2/structs.py
--rw-r--r--   0        0        0    36862 2023-04-11 17:07:00.209742 solidpython2-2.0.1/solid2/extensions/bosl2/threading.py
--rw-r--r--   0        0        0     8561 2023-04-11 17:06:59.937742 solidpython2-2.0.1/solid2/extensions/bosl2/transforms.py
--rw-r--r--   0        0        0     4786 2023-04-11 17:06:59.909742 solidpython2-2.0.1/solid2/extensions/bosl2/trigonometry.py
--rw-r--r--   0        0        0      611 2023-04-11 17:07:00.569742 solidpython2-2.0.1/solid2/extensions/bosl2/tripod_mounts.py
--rw-r--r--   0        0        0     3060 2023-04-11 17:07:00.113742 solidpython2-2.0.1/solid2/extensions/bosl2/turtle3d.py
--rw-r--r--   0        0        0     7958 2023-04-11 17:07:00.561742 solidpython2-2.0.1/solid2/extensions/bosl2/utility.py
--rw-r--r--   0        0        0     4557 2023-04-11 17:06:59.301743 solidpython2-2.0.1/solid2/extensions/bosl2/vectors.py
--rw-r--r--   0        0        0     1772 2023-04-11 17:07:00.277742 solidpython2-2.0.1/solid2/extensions/bosl2/version.py
--rw-r--r--   0        0        0     9788 2023-04-11 17:07:00.273742 solidpython2-2.0.1/solid2/extensions/bosl2/vnf.py
--rw-r--r--   0        0        0     2165 2023-04-11 17:07:00.665742 solidpython2-2.0.1/solid2/extensions/bosl2/walls.py
--rw-r--r--   0        0        0     1045 2023-04-11 17:06:59.181743 solidpython2-2.0.1/solid2/extensions/bosl2/wiring.py
--rwxr-xr-x   0        0        0     3867 2023-04-11 09:39:25.920704 solidpython2-2.0.1/solid2/extensions/bosl2_generator.py
--rw-r--r--   0        0        0      264 2022-08-12 15:59:10.187877 solidpython2-2.0.1/solid2/extensions/greedy_scad_interface/__init__.py
--rw-r--r--   0        0        0     1647 2023-03-19 12:43:05.633475 solidpython2-2.0.1/solid2/extensions/greedy_scad_interface/customizer_widgets.py
--rw-r--r--   0        0        0      871 2023-03-15 13:23:46.114122 solidpython2-2.0.1/solid2/extensions/greedy_scad_interface/scad_interface.py
--rw-r--r--   0        0        0     1034 2023-03-19 03:02:37.644529 solidpython2-2.0.1/solid2/extensions/greedy_scad_interface/scad_variable.py
--rwxr-xr-x   0        0        0     3570 2023-03-22 15:09:19.365226 solidpython2-2.0.1/solid2/extensions/openscad_extension_generator.py
--rw-r--r--   0        0        0    18422 2023-04-11 17:10:49.921489 solidpython2-2.0.1/solid2/libs/BOSL2/affine.scad
--rw-r--r--   0        0        0   158011 2023-04-11 17:10:49.921489 solidpython2-2.0.1/solid2/libs/BOSL2/attachments.scad
--rw-r--r--   0        0        0    10326 2023-04-11 17:10:49.921489 solidpython2-2.0.1/solid2/libs/BOSL2/ball_bearings.scad
--rw-r--r--   0        0        0    76076 2023-04-11 17:10:49.925489 solidpython2-2.0.1/solid2/libs/BOSL2/beziers.scad
--rw-r--r--   0        0        0     3557 2023-04-11 17:10:49.925489 solidpython2-2.0.1/solid2/libs/BOSL2/bosl1compat.scad
--rw-r--r--   0        0        0    53194 2023-04-11 17:10:49.925489 solidpython2-2.0.1/solid2/libs/BOSL2/bottlecaps.scad
--rw-r--r--   0        0        0     1257 2023-04-11 17:10:49.925489 solidpython2-2.0.1/solid2/libs/BOSL2/builtins.scad
--rw-r--r--   0        0        0     8302 2023-04-11 17:10:49.925489 solidpython2-2.0.1/solid2/libs/BOSL2/color.scad
--rw-r--r--   0        0        0    40080 2023-04-11 17:10:49.925489 solidpython2-2.0.1/solid2/libs/BOSL2/comparisons.scad
--rw-r--r--   0        0        0     9779 2023-04-11 17:10:49.925489 solidpython2-2.0.1/solid2/libs/BOSL2/constants.scad
--rw-r--r--   0        0        0    18570 2023-04-11 17:10:49.925489 solidpython2-2.0.1/solid2/libs/BOSL2/coords.scad
--rw-r--r--   0        0        0    28607 2023-04-11 17:10:49.925489 solidpython2-2.0.1/solid2/libs/BOSL2/cubetruss.scad
--rw-r--r--   0        0        0    88642 2023-04-11 17:10:49.925489 solidpython2-2.0.1/solid2/libs/BOSL2/distributors.scad
--rw-r--r--   0        0        0    62214 2023-04-11 17:10:49.925489 solidpython2-2.0.1/solid2/libs/BOSL2/drawing.scad
--rw-r--r--   0        0        0    56985 2023-04-11 17:10:49.925489 solidpython2-2.0.1/solid2/libs/BOSL2/fnliterals.scad
--rw-r--r--   0        0        0    65959 2023-04-11 17:10:49.929489 solidpython2-2.0.1/solid2/libs/BOSL2/gears.scad
--rw-r--r--   0        0        0   125434 2023-04-11 17:10:49.929489 solidpython2-2.0.1/solid2/libs/BOSL2/geometry.scad
--rw-r--r--   0        0        0    31047 2023-04-11 17:10:49.929489 solidpython2-2.0.1/solid2/libs/BOSL2/hinges.scad
--rw-r--r--   0        0        0    58197 2023-04-11 17:10:49.929489 solidpython2-2.0.1/solid2/libs/BOSL2/joiners.scad
--rw-r--r--   0        0        0    31481 2023-04-11 17:10:49.929489 solidpython2-2.0.1/solid2/libs/BOSL2/linalg.scad
--rw-r--r--   0        0        0     8378 2023-04-11 17:10:49.929489 solidpython2-2.0.1/solid2/libs/BOSL2/linear_bearings.scad
--rw-r--r--   0        0        0    47932 2023-04-11 17:10:49.929489 solidpython2-2.0.1/solid2/libs/BOSL2/lists.scad
--rw-r--r--   0        0        0    24740 2023-04-11 17:10:49.929489 solidpython2-2.0.1/solid2/libs/BOSL2/masks2d.scad
--rw-r--r--   0        0        0    26185 2023-04-11 17:10:49.929489 solidpython2-2.0.1/solid2/libs/BOSL2/masks3d.scad
--rw-r--r--   0        0        0    54569 2023-04-11 17:10:49.929489 solidpython2-2.0.1/solid2/libs/BOSL2/math.scad
--rw-r--r--   0        0        0    23837 2023-04-11 17:10:49.933489 solidpython2-2.0.1/solid2/libs/BOSL2/metric_screws.scad
--rw-r--r--   0        0        0     9089 2023-04-11 17:10:49.933489 solidpython2-2.0.1/solid2/libs/BOSL2/modular_hose.scad
--rw-r--r--   0        0        0    21204 2023-04-11 17:10:49.933489 solidpython2-2.0.1/solid2/libs/BOSL2/mutators.scad
--rw-r--r--   0        0        0    10102 2023-04-11 17:10:49.933489 solidpython2-2.0.1/solid2/libs/BOSL2/nema_steppers.scad
--rw-r--r--   0        0        0    25544 2023-04-11 17:10:49.933489 solidpython2-2.0.1/solid2/libs/BOSL2/partitions.scad
--rw-r--r--   0        0        0    55148 2023-04-11 17:10:49.933489 solidpython2-2.0.1/solid2/libs/BOSL2/paths.scad
--rw-r--r--   0        0        0    44343 2023-04-11 17:10:49.933489 solidpython2-2.0.1/solid2/libs/BOSL2/polyhedra.scad
--rw-r--r--   0        0        0    62670 2023-04-11 17:10:49.933489 solidpython2-2.0.1/solid2/libs/BOSL2/regions.scad
--rw-r--r--   0        0        0   220660 2023-04-11 17:10:49.937489 solidpython2-2.0.1/solid2/libs/BOSL2/rounding.scad
--rw-r--r--   0        0        0    14301 2023-04-11 17:10:49.937489 solidpython2-2.0.1/solid2/libs/BOSL2/screw_drive.scad
--rw-r--r--   0        0        0   179010 2023-04-11 17:10:49.937489 solidpython2-2.0.1/solid2/libs/BOSL2/screws.scad
--rw-r--r--   0        0        0    91055 2023-04-11 17:10:49.937489 solidpython2-2.0.1/solid2/libs/BOSL2/shapes2d.scad
--rw-r--r--   0        0        0   181418 2023-04-11 17:10:49.937489 solidpython2-2.0.1/solid2/libs/BOSL2/shapes3d.scad
--rw-r--r--   0        0        0   238386 2023-04-11 17:10:49.941489 solidpython2-2.0.1/solid2/libs/BOSL2/skin.scad
--rw-r--r--   0        0        0     6786 2023-04-11 17:10:49.941489 solidpython2-2.0.1/solid2/libs/BOSL2/sliders.scad
--rw-r--r--   0        0        0     1071 2023-04-11 17:10:49.941489 solidpython2-2.0.1/solid2/libs/BOSL2/std.scad
--rw-r--r--   0        0        0    34155 2023-04-11 17:10:49.941489 solidpython2-2.0.1/solid2/libs/BOSL2/strings.scad
--rw-r--r--   0        0        0     5355 2023-04-11 17:10:49.941489 solidpython2-2.0.1/solid2/libs/BOSL2/structs.scad
--rw-r--r--   0        0        0   102085 2023-04-11 17:10:49.941489 solidpython2-2.0.1/solid2/libs/BOSL2/threading.scad
--rw-r--r--   0        0        0    63253 2023-04-11 17:10:49.941489 solidpython2-2.0.1/solid2/libs/BOSL2/transforms.scad
--rw-r--r--   0        0        0    15310 2023-04-11 17:10:49.941489 solidpython2-2.0.1/solid2/libs/BOSL2/trigonometry.scad
--rw-r--r--   0        0        0     4103 2023-04-11 17:10:49.941489 solidpython2-2.0.1/solid2/libs/BOSL2/tripod_mounts.scad
--rw-r--r--   0        0        0    48075 2023-04-11 17:10:49.941489 solidpython2-2.0.1/solid2/libs/BOSL2/turtle3d.scad
--rw-r--r--   0        0        0    37770 2023-04-11 17:10:49.945489 solidpython2-2.0.1/solid2/libs/BOSL2/utility.scad
--rw-r--r--   0        0        0    25847 2023-04-11 17:10:49.945489 solidpython2-2.0.1/solid2/libs/BOSL2/vectors.scad
--rw-r--r--   0        0        0     6572 2023-04-11 17:10:49.945489 solidpython2-2.0.1/solid2/libs/BOSL2/version.scad
--rw-r--r--   0        0        0    85308 2023-04-11 17:10:49.945489 solidpython2-2.0.1/solid2/libs/BOSL2/vnf.scad
--rw-r--r--   0        0        0    16411 2023-04-11 17:10:49.945489 solidpython2-2.0.1/solid2/libs/BOSL2/walls.scad
--rw-r--r--   0        0        0     3545 2023-04-11 17:10:49.945489 solidpython2-2.0.1/solid2/libs/BOSL2/wiring.scad
--rw-r--r--   0        0        0        0 2022-08-12 15:59:10.203877 solidpython2-2.0.1/solid2/libs/__init__.py
--rw-r--r--   0        0        0     7048 2022-08-12 15:59:10.203877 solidpython2-2.0.1/solid2/libs/py_scadparser/LICENSE
--rw-r--r--   0        0        0      640 2022-08-12 15:59:10.203877 solidpython2-2.0.1/solid2/libs/py_scadparser/README.md
--rw-r--r--   0        0        0    48312 2023-03-23 17:47:21.609266 solidpython2-2.0.1/solid2/libs/py_scadparser/parsetab.py
--rw-r--r--   0        0        0     1229 2023-03-23 17:47:21.609266 solidpython2-2.0.1/solid2/libs/py_scadparser/scad_ast.py
--rw-r--r--   0        0        0     8328 2023-03-23 17:47:21.609266 solidpython2-2.0.1/solid2/libs/py_scadparser/scad_parser.py
--rw-r--r--   0        0        0     2745 2023-03-21 16:32:26.613592 solidpython2-2.0.1/solid2/libs/py_scadparser/scad_tokens.py
--rw-r--r--   0        0        0    24503 1970-01-01 00:00:00.000000 solidpython2-2.0.1/setup.py
--rw-r--r--   0        0        0    24246 1970-01-01 00:00:00.000000 solidpython2-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    22930 2023-03-15 13:23:46.110122 solidpython2-2.0.2/README.rst
+-rw-r--r--   0        0        0     1116 2023-05-09 10:27:48.203458 solidpython2-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-04-24 23:08:31.053339 solidpython2-2.0.2/solid2/__init__.py
+-rw-r--r--   0        0        0     1681 2023-04-26 10:51:37.721722 solidpython2-2.0.2/solid2/config.py
+-rw-r--r--   0        0        0      381 2023-05-09 10:20:41.792164 solidpython2-2.0.2/solid2/core/__init__.py
+-rw-r--r--   0        0        0       53 2023-04-26 17:53:48.422660 solidpython2-2.0.2/solid2/core/builtins/__init__.py
+-rw-r--r--   0        0        0     3633 2023-04-21 22:55:04.234686 solidpython2-2.0.2/solid2/core/builtins/convenience.py
+-rw-r--r--   0        0        0     1040 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/core/builtins/implicit.primitives
+-rw-r--r--   0        0        0      754 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/core/builtins/openscad.mutators
+-rw-r--r--   0        0        0     1968 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/core/builtins/openscad.primitives
+-rw-r--r--   0        0        0    25400 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/core/builtins/openscad_primitives.py
+-rw-r--r--   0        0        0      367 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/core/builtins/primitives.py
+-rw-r--r--   0        0        0      938 2022-09-03 20:01:15.234639 solidpython2-2.0.2/solid2/core/extension_manager.py
+-rw-r--r--   0        0        0       32 2023-03-19 13:30:20.199884 solidpython2-2.0.2/solid2/core/object_base/__init__.py
+-rw-r--r--   0        0        0     3522 2023-03-20 14:58:07.769013 solidpython2-2.0.2/solid2/core/object_base/access_syntax_mixin.py
+-rw-r--r--   0        0        0     6866 2023-05-02 10:30:45.741949 solidpython2-2.0.2/solid2/core/object_base/object_base_impl.py
+-rw-r--r--   0        0        0     2253 2023-03-20 14:58:07.769013 solidpython2-2.0.2/solid2/core/object_base/operator_mixin.py
+-rw-r--r--   0        0        0     3994 2022-08-12 15:59:10.183877 solidpython2-2.0.2/solid2/core/object_factory.py
+-rw-r--r--   0        0        0     3428 2023-04-26 10:51:10.097683 solidpython2-2.0.2/solid2/core/parse_scad.py
+-rw-r--r--   0        0        0     5489 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/core/scad_import.py
+-rw-r--r--   0        0        0     3051 2023-05-02 10:30:37.857979 solidpython2-2.0.2/solid2/core/scad_render.py
+-rw-r--r--   0        0        0     2016 2023-04-24 10:34:26.227909 solidpython2-2.0.2/solid2/core/utils.py
+-rwxr-xr-x   0        0        0      559 2023-04-28 10:25:21.909011 solidpython2-2.0.2/solid2/examples/01-basics.py
+-rwxr-xr-x   0        0        0      846 2023-04-21 12:24:05.601732 solidpython2-2.0.2/solid2/examples/02-vars-and-operators.py
+-rwxr-xr-x   0        0        0      647 2022-08-12 15:59:10.183877 solidpython2-2.0.2/solid2/examples/03-debug-background.py
+-rwxr-xr-x   0        0        0     1272 2022-08-12 15:59:10.183877 solidpython2-2.0.2/solid2/examples/04-convenience.py
+-rwxr-xr-x   0        0        0      934 2022-08-12 15:59:10.183877 solidpython2-2.0.2/solid2/examples/05-access-style-syntax.py
+-rwxr-xr-x   0        0        0     1182 2023-03-15 22:58:40.236989 solidpython2-2.0.2/solid2/examples/06-functions.py
+-rwxr-xr-x   0        0        0      425 2023-04-24 18:27:22.516007 solidpython2-2.0.2/solid2/examples/07-libs-bosl2-attachable.py
+-rw-r--r--   0        0        0     3329 2023-04-11 09:39:25.912704 solidpython2-2.0.2/solid2/examples/07-libs-bosl2-logo.py
+-rwxr-xr-x   0        0        0     1762 2023-04-23 11:52:48.014465 solidpython2-2.0.2/solid2/examples/07-libs-bosl2.py
+-rwxr-xr-x   0        0        0      620 2023-04-21 23:01:13.315397 solidpython2-2.0.2/solid2/examples/07-libs.x.py
+-rwxr-xr-x   0        0        0     2448 2023-03-20 14:58:07.769013 solidpython2-2.0.2/solid2/examples/08-extensions.py
+-rwxr-xr-x   0        0        0     1656 2023-04-24 18:33:54.580435 solidpython2-2.0.2/solid2/examples/09-code-attach-extension.py
+-rwxr-xr-x   0        0        0      906 2023-04-21 22:55:04.234686 solidpython2-2.0.2/solid2/examples/10-customizer.py
+-rw-r--r--   0        0        0      158 2022-08-12 15:59:10.183877 solidpython2-2.0.2/solid2/examples/11-font/LICENSE_README
+-rw-r--r--   0        0        0    47404 2022-08-12 15:59:10.187877 solidpython2-2.0.2/solid2/examples/11-font/RichEatin.otf
+-rwxr-xr-x   0        0        0      192 2023-03-15 13:23:46.114122 solidpython2-2.0.2/solid2/examples/11-fonts.x.py
+-rwxr-xr-x   0        0        0      335 2023-03-15 13:23:46.114122 solidpython2-2.0.2/solid2/examples/12-animation.py
+-rwxr-xr-x   0        0        0     2032 2023-03-19 12:43:05.625475 solidpython2-2.0.2/solid2/examples/13-animated-bouncing-ball.py
+-rwxr-xr-x   0        0        0     1381 2023-04-21 23:01:13.315397 solidpython2-2.0.2/solid2/examples/14-implicitCAD.x.py
+-rwxr-xr-x   0        0        0     1794 2023-04-21 23:01:13.315397 solidpython2-2.0.2/solid2/examples/15-implicitCAD2.x.py
+-rwxr-xr-x   0        0        0     1102 2022-08-12 15:59:10.187877 solidpython2-2.0.2/solid2/examples/16-mazebox-bosl2.py
+-rwxr-xr-x   0        0        0     2243 2023-03-15 13:23:46.114122 solidpython2-2.0.2/solid2/examples/17-greedy-scad-interface.py
+-rw-r--r--   0        0        0     1196 2022-08-12 15:59:10.187877 solidpython2-2.0.2/solid2/examples/maze7.png
+-rw-r--r--   0        0        0        1 2023-04-24 16:33:55.353741 solidpython2-2.0.2/solid2/extensions/__init__.py
+-rw-r--r--   0        0        0       51 2023-04-21 22:55:14.018704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.git
+-rw-r--r--   0        0        0      522 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      655 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      318 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/check_for_tabs.json
+-rw-r--r--   0        0        0      307 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/openscad_docsgen.json
+-rw-r--r--   0        0        0     1214 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/workflows/gen_docs.yml
+-rw-r--r--   0        0        0     1448 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/workflows/gen_tutorials.yml
+-rw-r--r--   0        0        0     2823 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1253 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.gitignore
+-rw-r--r--   0        0        0     1197 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.openscad_docsgen_rc
+-rw-r--r--   0        0        0      132 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/.openscad_mdimggen_rc
+-rw-r--r--   0        0        0     2142 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1323 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/LICENSE
+-rw-r--r--   0        0        0     2926 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/README.md
+-rw-r--r--   0        0        0    37745 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/WRITING_DOCS.md
+-rw-r--r--   0        0        0    18422 2023-04-21 22:55:14.034704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/affine.scad
+-rw-r--r--   0        0        0   158011 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/attachments.scad
+-rw-r--r--   0        0        0    10326 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/ball_bearings.scad
+-rw-r--r--   0        0        0    76076 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/beziers.scad
+-rw-r--r--   0        0        0     3557 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/bosl1compat.scad
+-rw-r--r--   0        0        0    53194 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/bottlecaps.scad
+-rw-r--r--   0        0        0     1257 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/builtins.scad
+-rw-r--r--   0        0        0     8302 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/color.scad
+-rw-r--r--   0        0        0    40080 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/comparisons.scad
+-rw-r--r--   0        0        0     9779 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/constants.scad
+-rw-r--r--   0        0        0    18570 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/coords.scad
+-rw-r--r--   0        0        0    28607 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/cubetruss.scad
+-rw-r--r--   0        0        0    88642 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/distributors.scad
+-rw-r--r--   0        0        0    62214 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/drawing.scad
+-rw-r--r--   0        0        0     1389 2023-04-21 22:55:14.038704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/BOSL2logo.scad
+-rw-r--r--   0        0        0      559 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/attachments.scad
+-rw-r--r--   0        0        0     1344 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/boolean_geometry.scad
+-rw-r--r--   0        0        0      505 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/fractal_tree.scad
+-rw-r--r--   0        0        0     4168 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/lsystems.scad
+-rw-r--r--   0        0        0     2465 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/orientations.scad
+-rw-r--r--   0        0        0      704 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/examples/spherical_patch.scad
+-rw-r--r--   0        0        0    56985 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/fnliterals.scad
+-rw-r--r--   0        0        0    65959 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/gears.scad
+-rw-r--r--   0        0        0   125434 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/geometry.scad
+-rw-r--r--   0        0        0    31047 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/hinges.scad
+-rw-r--r--   0        0        0   117043 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/images/BOSL2logo.png
+-rw-r--r--   0        0        0    58197 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/joiners.scad
+-rw-r--r--   0        0        0    31481 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/linalg.scad
+-rw-r--r--   0        0        0     8378 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/linear_bearings.scad
+-rw-r--r--   0        0        0    47932 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/lists.scad
+-rw-r--r--   0        0        0    24740 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/masks2d.scad
+-rw-r--r--   0        0        0    26185 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/masks3d.scad
+-rw-r--r--   0        0        0    54569 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/math.scad
+-rw-r--r--   0        0        0    23837 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/metric_screws.scad
+-rw-r--r--   0        0        0     9089 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/modular_hose.scad
+-rw-r--r--   0        0        0    21204 2023-04-21 22:55:14.042704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/mutators.scad
+-rw-r--r--   0        0        0    10102 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/nema_steppers.scad
+-rw-r--r--   0        0        0    25544 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/partitions.scad
+-rw-r--r--   0        0        0    55148 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/paths.scad
+-rw-r--r--   0        0        0    44343 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/polyhedra.scad
+-rw-r--r--   0        0        0    62670 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/regions.scad
+-rw-r--r--   0        0        0   220660 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/rounding.scad
+-rw-r--r--   0        0        0    14301 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/screw_drive.scad
+-rw-r--r--   0        0        0   179010 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/screws.scad
+-rwxr-xr-x   0        0        0      115 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/check_for_tabs.sh
+-rwxr-xr-x   0        0        0      569 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/find_modular_asserts.sh
+-rwxr-xr-x   0        0        0     2784 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/func_coverage.py
+-rwxr-xr-x   0        0        0     2345 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/img2scad.py
+-rwxr-xr-x   0        0        0      545 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/increment_version.sh
+-rwxr-xr-x   0        0        0      511 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/linecount.sh
+-rwxr-xr-x   0        0        0      368 2023-04-21 22:55:14.046704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/purge_wiki_history.sh
+-rwxr-xr-x   0        0        0      790 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/scripts/run_tests.sh
+-rw-r--r--   0        0        0    91055 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/shapes2d.scad
+-rw-r--r--   0        0        0   181418 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/shapes3d.scad
+-rw-r--r--   0        0        0   238386 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/skin.scad
+-rw-r--r--   0        0        0     6786 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/sliders.scad
+-rw-r--r--   0        0        0     1071 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/std.scad
+-rw-r--r--   0        0        0    34155 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/strings.scad
+-rw-r--r--   0        0        0     5355 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/structs.scad
+-rw-r--r--   0        0        0      186 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/README.txt
+-rw-r--r--   0        0        0     1443 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/polyhedra.scad
+-rw-r--r--   0        0        0     4998 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_affine.scad
+-rw-r--r--   0        0        0      371 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_attachments.scad
+-rw-r--r--   0        0        0    16598 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_comparisons.scad
+-rw-r--r--   0        0        0    12026 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_coords.scad
+-rw-r--r--   0        0        0      393 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_cubetruss.scad
+-rw-r--r--   0        0        0      999 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_distributors.scad
+-rw-r--r--   0        0        0     5679 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_drawing.scad
+-rw-r--r--   0        0        0     9824 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_edges.scad
+-rw-r--r--   0        0        0    23237 2023-04-21 22:55:14.050704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_fnliterals.scad
+-rw-r--r--   0        0        0    62561 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_geometry.scad
+-rw-r--r--   0        0        0    11660 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_linalg.scad
+-rw-r--r--   0        0        0      425 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_linear_bearings.scad
+-rw-r--r--   0        0        0    13578 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_lists.scad
+-rw-r--r--   0        0        0     8961 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_masks2d.scad
+-rw-r--r--   0        0        0    26667 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_math.scad
+-rw-r--r--   0        0        0     1351 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_mutators.scad
+-rw-r--r--   0        0        0    12273 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_paths.scad
+-rw-r--r--   0        0        0     7958 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_regions.scad
+-rw-r--r--   0        0        0     8862 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_rounding.scad
+-rw-r--r--   0        0        0      700 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_screw_drive.scad
+-rw-r--r--   0        0        0    64080 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_shapes2d.scad
+-rw-r--r--   0        0        0    24086 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_shapes3d.scad
+-rw-r--r--   0        0        0      861 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_skin.scad
+-rw-r--r--   0        0        0    13469 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_strings.scad
+-rw-r--r--   0        0        0     2713 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_structs.scad
+-rw-r--r--   0        0        0    16142 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_transforms.scad
+-rw-r--r--   0        0        0     1777 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_trigonometry.scad
+-rw-r--r--   0        0        0    13375 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_utility.scad
+-rw-r--r--   0        0        0    10291 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_vectors.scad
+-rw-r--r--   0        0        0     3493 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_version.scad
+-rw-r--r--   0        0        0     3259 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tests/test_vnf.scad
+-rw-r--r--   0        0        0   102085 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/threading.scad
+-rw-r--r--   0        0        0    63253 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/transforms.scad
+-rw-r--r--   0        0        0    15310 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/trigonometry.scad
+-rw-r--r--   0        0        0     4103 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tripod_mounts.scad
+-rw-r--r--   0        0        0    48075 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/turtle3d.scad
+-rw-r--r--   0        0        0    49578 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Attachments.md
+-rw-r--r--   0        0        0     6344 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Distributors.md
+-rw-r--r--   0        0        0     3329 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/FractalTree.md
+-rw-r--r--   0        0        0     7580 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Mutators.md
+-rw-r--r--   0        0        0    14859 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Paths.md
+-rw-r--r--   0        0        0    20047 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Shapes2d.md
+-rw-r--r--   0        0        0     9378 2023-04-21 22:55:14.054704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Shapes3d.md
+-rw-r--r--   0        0        0     6553 2023-04-21 22:55:14.058704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/Transforms.md
+-rw-r--r--   0        0        0     7054 2023-04-21 22:55:14.058704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tutorials/VNF.md
+-rw-r--r--   0        0        0    37770 2023-04-21 22:55:14.058704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/utility.scad
+-rw-r--r--   0        0        0    25847 2023-04-21 22:55:14.058704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/vectors.scad
+-rw-r--r--   0        0        0     6572 2023-04-21 22:55:14.058704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/version.scad
+-rw-r--r--   0        0        0    85308 2023-04-21 22:55:14.058704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/vnf.scad
+-rw-r--r--   0        0        0    16411 2023-04-21 22:55:14.058704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/walls.scad
+-rw-r--r--   0        0        0     3545 2023-04-21 22:55:14.058704 solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/wiring.scad
+-rw-r--r--   0        0        0      210 2023-04-11 09:14:35.909512 solidpython2-2.0.2/solid2/extensions/bosl2/__init__.py
+-rw-r--r--   0        0        0     3318 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/affine.py
+-rw-r--r--   0        0        0    13302 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/attachments.py
+-rw-r--r--   0        0        0      878 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/ball_bearings.py
+-rw-r--r--   0        0        0     7573 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/beziers.py
+-rw-r--r--   0        0        0    15500 2023-04-26 17:41:35.972132 solidpython2-2.0.2/solid2/extensions/bosl2/bosl2_access_syntax_mixin.py
+-rw-r--r--   0        0        0     1002 2023-04-11 09:15:15.373553 solidpython2-2.0.2/solid2/extensions/bosl2/bosl2_base.py
+-rw-r--r--   0        0        0      611 2023-04-23 17:29:35.094413 solidpython2-2.0.2/solid2/extensions/bosl2/bosl2_patches.py
+-rw-r--r--   0        0        0    10956 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/bottlecaps.py
+-rw-r--r--   0        0        0     1540 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/color.py
+-rw-r--r--   0        0        0     7214 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/comparisons.py
+-rw-r--r--   0        0        0     1138 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/constants.py
+-rw-r--r--   0        0        0     3010 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/coords.py
+-rw-r--r--   0        0        0     3617 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/cubetruss.py
+-rw-r--r--   0        0        0    10735 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/distributors.py
+-rw-r--r--   0        0        0     8136 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/drawing.py
+-rw-r--r--   0        0        0    12654 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/fnliterals.py
+-rw-r--r--   0        0        0    12638 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/gears.py
+-rw-r--r--   0        0        0    19278 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/geometry.py
+-rw-r--r--   0        0        0     5046 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/hinges.py
+-rw-r--r--   0        0        0     9519 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/joiners.py
+-rw-r--r--   0        0        0     5626 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/linalg.py
+-rw-r--r--   0        0        0     1829 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/linear_bearings.py
+-rw-r--r--   0        0        0     6946 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/lists.py
+-rw-r--r--   0        0        0     4345 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/masks2d.py
+-rw-r--r--   0        0        0     8165 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/masks3d.py
+-rw-r--r--   0        0        0    12662 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/math.py
+-rw-r--r--   0        0        0     3781 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/metric_screws.py
+-rw-r--r--   0        0        0     1357 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/modular_hose.py
+-rw-r--r--   0        0        0     2333 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/mutators.py
+-rw-r--r--   0        0        0     1187 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/nema_steppers.py
+-rw-r--r--   0        0        0     6047 2023-04-26 17:41:37.688128 solidpython2-2.0.2/solid2/extensions/bosl2/openscad.py
+-rw-r--r--   0        0        0     4055 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/partitions.py
+-rw-r--r--   0        0        0     7787 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/paths.py
+-rw-r--r--   0        0        0     3387 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/polyhedra.py
+-rw-r--r--   0        0        0     7754 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/regions.py
+-rw-r--r--   0        0        0    20788 2023-05-02 09:54:08.391238 solidpython2-2.0.2/solid2/extensions/bosl2/rounding.py
+-rw-r--r--   0        0        0     3052 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/screw_drive.py
+-rw-r--r--   0        0        0    14577 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/screws.py
+-rw-r--r--   0        0        0    14150 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/shapes2d.py
+-rw-r--r--   0        0        0    26881 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/shapes3d.py
+-rw-r--r--   0        0        0    17224 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/skin.py
+-rw-r--r--   0        0        0     1595 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/sliders.py
+-rw-r--r--   0        0        0      679 2023-04-26 17:41:35.796132 solidpython2-2.0.2/solid2/extensions/bosl2/std.py
+-rw-r--r--   0        0        0     7256 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/strings.py
+-rw-r--r--   0        0        0     1720 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/structs.py
+-rw-r--r--   0        0        0    36860 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/threading.py
+-rw-r--r--   0        0        0     8559 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/transforms.py
+-rw-r--r--   0        0        0     4784 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/trigonometry.py
+-rw-r--r--   0        0        0      609 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/tripod_mounts.py
+-rw-r--r--   0        0        0     3058 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/turtle3d.py
+-rw-r--r--   0        0        0     7956 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/utility.py
+-rw-r--r--   0        0        0     4555 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/vectors.py
+-rw-r--r--   0        0        0     1770 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/version.py
+-rw-r--r--   0        0        0     9786 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/vnf.py
+-rw-r--r--   0        0        0     2163 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/walls.py
+-rw-r--r--   0        0        0     1043 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2/wiring.py
+-rwxr-xr-x   0        0        0     3575 2023-05-02 09:54:08.395238 solidpython2-2.0.2/solid2/extensions/bosl2_generator.py
+-rw-r--r--   0        0        0      264 2023-04-24 23:08:43.905363 solidpython2-2.0.2/solid2/extensions/greedy_scad_interface/__init__.py
+-rw-r--r--   0        0        0     1647 2023-03-19 12:43:05.633475 solidpython2-2.0.2/solid2/extensions/greedy_scad_interface/customizer_widgets.py
+-rw-r--r--   0        0        0      871 2023-03-15 13:23:46.114122 solidpython2-2.0.2/solid2/extensions/greedy_scad_interface/scad_interface.py
+-rw-r--r--   0        0        0     1034 2023-04-24 23:08:38.709354 solidpython2-2.0.2/solid2/extensions/greedy_scad_interface/scad_variable.py
+-rwxr-xr-x   0        0        0     3623 2023-04-24 16:39:42.154697 solidpython2-2.0.2/solid2/extensions/openscad_extension_generator.py
+-rwxr-xr-x   0        0        0     3650 2023-04-26 17:33:19.525225 solidpython2-2.0.2/solid2/extensions/scad2solid.py
+-rw-r--r--   0        0        0        0 2022-08-12 15:59:10.203877 solidpython2-2.0.2/solid2/libs/__init__.py
+-rw-r--r--   0        0        0       56 2023-04-21 22:55:14.022704 solidpython2-2.0.2/solid2/libs/py_scadparser/.git
+-rw-r--r--   0        0        0     1855 2023-04-21 22:55:14.070704 solidpython2-2.0.2/solid2/libs/py_scadparser/.gitignore
+-rw-r--r--   0        0        0     7048 2023-04-21 22:55:14.070704 solidpython2-2.0.2/solid2/libs/py_scadparser/LICENSE
+-rw-r--r--   0        0        0      722 2023-04-21 22:55:14.070704 solidpython2-2.0.2/solid2/libs/py_scadparser/README.md
+-rw-r--r--   0        0        0    44947 2023-04-23 20:12:18.566240 solidpython2-2.0.2/solid2/libs/py_scadparser/__pycache__/parsetab.cpython-310.pyc
+-rw-r--r--   0        0        0     2673 2023-04-23 20:09:17.734159 solidpython2-2.0.2/solid2/libs/py_scadparser/__pycache__/scad_ast.cpython-310.pyc
+-rw-r--r--   0        0        0    10330 2023-04-23 20:09:17.730159 solidpython2-2.0.2/solid2/libs/py_scadparser/__pycache__/scad_parser.cpython-310.pyc
+-rw-r--r--   0        0        0     2696 2023-04-23 20:09:17.738159 solidpython2-2.0.2/solid2/libs/py_scadparser/__pycache__/scad_tokens.cpython-310.pyc
+-rw-r--r--   0        0        0    48312 2023-04-23 20:09:17.922159 solidpython2-2.0.2/solid2/libs/py_scadparser/parsetab.py
+-rw-r--r--   0        0        0     1229 2023-04-21 22:55:14.070704 solidpython2-2.0.2/solid2/libs/py_scadparser/scad_ast.py
+-rw-r--r--   0        0        0     8328 2023-04-21 22:55:14.070704 solidpython2-2.0.2/solid2/libs/py_scadparser/scad_parser.py
+-rw-r--r--   0        0        0     2706 2023-04-21 22:55:14.070704 solidpython2-2.0.2/solid2/libs/py_scadparser/scad_tokens.py
+-rw-r--r--   0        0        0      280 2023-04-21 22:55:14.070704 solidpython2-2.0.2/solid2/libs/py_scadparser/test.scad
+-rw-r--r--   0        0        0    24920 1970-01-01 00:00:00.000000 solidpython2-2.0.2/setup.py
+-rw-r--r--   0        0        0    24246 1970-01-01 00:00:00.000000 solidpython2-2.0.2/PKG-INFO
```

### Comparing `solidpython2-2.0.1/README.rst` & `solidpython2-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/pyproject.toml` & `solidpython2-2.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solidpython2"
-version = "2.0.1"
+version = "2.0.2"
 description = "Python interface to the OpenSCAD declarative geometry language"
 authors = ["jeff"]
 homepage = "https://github.com/jeff-dh/SolidPython"
 repository = "https://github.com/jeff-dh/SolidPython"
 license = "LGPL-2.1"
 readme = "README.rst"
 keywords = [
```

### Comparing `solidpython2-2.0.1/solid2/config.py` & `solidpython2-2.0.2/solid2/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,16 +39,16 @@
             #sorry, but I've no clue what the paths are on other operating systems
             paths.append(Path("/usr/share/openscad/libraries"))
 
         return paths
 
     def get_pickle_cache_dir(self):
         default_paths = {
-            'Linux':   Path.home() / '.local/share/expSolidPython/pickle_cache',
-            'Darwin':  Path.home() / 'Documents/expSolidPython/pickle_cache',
-            'Windows': Path('My Documents/expSolidPython/pickle_cache')
+            'Linux':   Path.home() / '.local/share/SolidPython2/pickle_cache',
+            'Darwin':  Path.home() / 'Documents/SolidPython2/pickle_cache',
+            'Windows': Path('My Documents/SolidPython2/pickle_cache')
         }
         return default_paths[platform.system()]
 
 
 config = Config()
```

### Comparing `solidpython2-2.0.1/solid2/core/builtins/convenience.py` & `solidpython2-2.0.2/solid2/core/builtins/convenience.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,17 +42,17 @@
 def translateY(y) : return translate((0, y, 0))
 def translateZ(z) : return translate((0, 0, z))
 
 def rotateX(x): return rotate((x, 0, 0))
 def rotateY(y): return rotate((0, y, 0))
 def rotateZ(z): return rotate((0, 0, z))
 
-def scaleX(x): return scale((x, 0, 0))
-def scaleY(y): return scale((0, y, 0))
-def scaleZ(z): return scale((0, 0, z))
+def scaleX(x): return scale((x, 1, 1))
+def scaleY(y): return scale((1, y, 1))
+def scaleZ(z): return scale((1, 1, z))
 
 if not config.use_implicit_builtins:
     def resizeX(x): return resize((x, 0, 0))
     def resizeY(y): return resize((0, y, 0))
     def resizeZ(z): return resize((0, 0, z))
 
     def mirrorX(): return mirror((1, 0, 0))
```

### Comparing `solidpython2-2.0.1/solid2/core/builtins/implicit.primitives` & `solidpython2-2.0.2/solid2/core/builtins/implicit.primitives`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/core/builtins/openscad.mutators` & `solidpython2-2.0.2/solid2/core/builtins/openscad.mutators`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/core/builtins/openscad.primitives` & `solidpython2-2.0.2/solid2/core/builtins/openscad.primitives`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/core/builtins/openscad_primitives.py` & `solidpython2-2.0.2/solid2/core/builtins/openscad_primitives.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/core/extension_manager.py` & `solidpython2-2.0.2/solid2/core/extension_manager.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/core/object_base/access_syntax_mixin.py` & `solidpython2-2.0.2/solid2/core/object_base/access_syntax_mixin.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/core/object_base/object_base_impl.py` & `solidpython2-2.0.2/solid2/core/object_base/object_base_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         from ..scad_render import scad_render
         return scad_render(self)[:-1]
 
     def save_as_scad(self, filename='', outdir=''):
         from ..scad_render import scad_render_to_file
         return scad_render_to_file(self, filename, outdir)
 
-    def save_as_stl(self, filename='', outdir=''):
+    def save_as_stl(self, filename=None):
         from ..scad_render import render_to_stl_file
         return render_to_stl_file(self, filename)
 
 class ObjectBase(RenderMixin):
     def __init__(self):
         self._children = []
 
@@ -61,25 +61,21 @@
         """
             returns the scad code for a given node tuple consiting of name,
             params and children list.
 
             -> translate(v = [1, 2, 3]) {children[0]; children[1]; ...};\n
         """
         from ..utils import indent
-        s = self._generate_scad_head()
-
-        if self._children:
-            s += " {\n"
-            for child in self._children:
-                s += indent(child._render())
-            s += "}"
+        renderedChildsList = [indent(child._render()) for child in self._children]
+        if renderedChildsList:
+            renderedChilds = f" {{\n{''.join(renderedChildsList)}}}\n"
         else:
-            s += ";"
+            renderedChilds = ";\n"
 
-        return s + "\n"
+        return self._generate_scad_head() + renderedChilds
 
     def _generate_scad_head(self):
         """
             for a given function name and dict of params it returns:
                 {name}(p1=v1, p2=v2,...)
                 -> translate(v = [1, 2, 3])
         """
```

### Comparing `solidpython2-2.0.1/solid2/core/object_base/operator_mixin.py` & `solidpython2-2.0.2/solid2/core/object_base/operator_mixin.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/core/object_factory.py` & `solidpython2-2.0.2/solid2/core/object_factory.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/core/parse_scad.py` & `solidpython2-2.0.2/solid2/core/parse_scad.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 from ..config import config
 from .object_base import OpenSCADConstant
 from .utils import escape_openscad_identifier
 from .object_factory import create_openscad_wrapper_from_symbols
 
 callables_entry = namedtuple("callables_entry", ["name", "args", "kwargs"])
 
-# ===========
-# = Parsing =
-# ===========
+
 def get_pickle_filename(filename):
     md5 = hashlib.md5()
     md5.update(filename.as_posix().encode('utf-8'))
     filename_hash = md5.hexdigest()
 
     with open(filename, mode='rb') as f:
         d = hashlib.md5()
```

### Comparing `solidpython2-2.0.1/solid2/core/scad_import.py` & `solidpython2-2.0.2/solid2/core/scad_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,30 +32,30 @@
                                         [new_namespace_dict, use_not_include, skip_render]
 
 def load_scad_file_into_dict(resolved_scad, dest_namespace_dict, use_not_include, skip_render):
     #check the cache
     cached_dict = check_module_cache(resolved_scad, use_not_include)
     if cached_dict:
         dest_namespace_dict.update(cached_dict)
-        return dest_namespace_dict
+        return
 
     #otherwise parse the file
     new_namespace_dict = get_scad_file_as_dict(resolved_scad)
     dest_namespace_dict.update(new_namespace_dict)
 
     #and update the cache
     update_module_cache(resolved_scad, new_namespace_dict, use_not_include, skip_render)
 
 def load_scad_dir_into_dict(resolved_scad, dest_namespace_dict, use_not_include, skip_render):
     assert(resolved_scad.is_dir())
 
     #for each file in the dir
     for f in resolved_scad.iterdir():
         #skip non .scad files
-        if f.suffix != ".scad":
+        if f.is_file() and f.suffix != ".scad":
             continue
 
         #load it
         subspace = ExpSolidNamespace(f)
         load_scad_file_or_dir_into_dict(f, subspace.__dict__, use_not_include, skip_render)
 
         #and add it to the dest_namespace_dict
```

### Comparing `solidpython2-2.0.1/solid2/core/scad_render.py` & `solidpython2-2.0.2/solid2/core/scad_render.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 from pathlib import Path
 
 from .scad_import import module_cache_by_resolved_filename, extra_scad_includes
 from ..config import config
 
-# =========================================
-# = Rendering Python code to OpenSCAD code=
-# =========================================
+
+def get_default_filename(suffix):
+    #try to get the filename of the calling module
+    import __main__
+    if hasattr(__main__, "__file__"):
+        #not called from a terminal
+        calling_file = Path(__main__.__file__).absolute()
+        outfile = calling_file.with_suffix(suffix)
+    else:
+        outfile = "solid_out" + suffix
+
+    return outfile
+
 def render_to_stl_file(root, filename):
-    scad_render_to_file(root, Path(filename).with_suffix(".stl.scad"))
+    if not filename:
+        filename = get_default_filename(".stl")
+    scad_file = \
+        scad_render_to_file(root,
+                            Path(filename).with_suffix(".stl.scad"))
 
     import subprocess
-    args = ["openscad", "-o", filename, Path(filename).with_suffix(".stl.scad")]
-    cp = subprocess.run(args, stdout=subprocess.PIPE)
-
-    if cp.returncode == 0:
-        return Path(filename).absolute().as_posix()
+    args = ["openscad", "-o", filename, scad_file]
+    subprocess.check_call(args,
+                          stdout=subprocess.PIPE,
+                          stderr=subprocess.DEVNULL)
 
-    return None
+    return Path(filename).absolute().as_posix()
 
 def scad_render(root, file_header = ''):
     #get a list of all used and included files
     includes = get_include_string()
 
     #call extensions pre_render
     from .extension_manager import default_extension_manager
@@ -39,34 +52,26 @@
     return file_header + includes + extensions_header_str + scad_body \
                        + extensions_footer_str
 
 def scad_render_to_file(scad_object, filename=None, out_dir='', file_header=''):
 
     if out_dir == None:
         out_dir = ''
-    header = f"// Generated by ExpSolidPython\n" + "\n"
 
     rendered_string = scad_render(scad_object, file_header=file_header)
 
     return _write_to_file(rendered_string, filename, out_dir)
 
 def _write_to_file(out_string, filename=None, outdir=''):
     outfile = filename
 
     if not outfile:
         suffix = ".scad" if not config.use_implicit_builtins else ".escad"
+        outfile = get_default_filename(suffix)
 
-        #try to get the filename of the calling module
-        import __main__
-        if hasattr(__main__, "__file__"):
-            #not called from a terminal
-            calling_file = Path(__main__.__file__).absolute()
-            outfile = calling_file.with_suffix(suffix)
-        else:
-            outfile = "expsolid_out" + suffix
 
     outpath = Path(outdir)
     if not outpath.exists():
         outpath.mkdir()
 
     outfile_path = outpath / Path(outfile)
```

### Comparing `solidpython2-2.0.1/solid2/core/utils.py` & `solidpython2-2.0.2/solid2/core/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,21 +57,13 @@
     if type(o) == bool:
         return str(o).lower()
     if type(o) == float:
         return f"{o:.10f}"  # type: ignore
     if type(o) == str:
         return f'\"{o}\"'  # type: ignore
     if isinstance(o, ObjectBase):
-        #[:-1] removing traling ;\n
-        return o._render()[:-2]
+        return o._render()[:-2] #[:-1] removing traling ;\n
     if hasattr(o, "__iter__"):
-        s = "["
-        first = True
-        for i in o:  # type: ignore
-            if not first:
-                s += ", "
-            first = False
-            s += py2openscad(i)
-        s += "]"
-        return s
+        scadVals = [py2openscad(i) for i in o]
+        return f"[{', '.join(scadVals)}]"
     return str(o)
```

### Comparing `solidpython2-2.0.1/solid2/examples/01-basics.py` & `solidpython2-2.0.2/solid2/examples/01-basics.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/examples/02-vars-and-operators.py` & `solidpython2-2.0.2/solid2/examples/02-vars-and-operators.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/examples/03-debug-background.py` & `solidpython2-2.0.2/solid2/examples/03-debug-background.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/examples/04-convenience.py` & `solidpython2-2.0.2/solid2/examples/04-convenience.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/examples/05-access-style-syntax.py` & `solidpython2-2.0.2/solid2/examples/05-access-style-syntax.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/examples/06-functions.py` & `solidpython2-2.0.2/solid2/examples/06-functions.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/examples/07-libs-bosl2-logo.py` & `solidpython2-2.0.2/solid2/examples/07-libs-bosl2-logo.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/examples/07-libs-bosl2.py` & `solidpython2-2.0.2/solid2/examples/07-libs-bosl2.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/examples/07-libs.py` & `solidpython2-2.0.2/solid2/examples/07-libs.x.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/examples/08-extensions.py` & `solidpython2-2.0.2/solid2/examples/08-extensions.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/examples/09-code-attach-extension.py` & `solidpython2-2.0.2/solid2/examples/09-code-attach-extension.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,16 +36,14 @@
         code_str = code_str.replace("/*", "/_*")
         code_str = code_str.replace("*/", "*_/")
 
         # return the string to be appended to the *.scad file
         return f'/* Generated from the following ExpSolid code:\n\n' +\
                f'{code_str}*/'
 
-    assert(False)
-
 # register the post_render extension. This hooks it into the "_render" routine.
 # It will be called after the root gets rendered. It's return string will be
 # appended to the rendered string.
 from solid2.core.extension_manager import default_extension_manager
 default_extension_manager.register_post_render(attach_code_post_render)
 
 # =============
```

### Comparing `solidpython2-2.0.1/solid2/examples/10-customizer.py` & `solidpython2-2.0.2/solid2/examples/10-customizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 side = CustomizerSliderVariable("side", 4)
 cube_pos = CustomizerSliderVariable("cube_pos", [5, 5, 5])
 cube_size = CustomizerSliderVariable("cube_size", 5)
 customizedText = CustomizerDropdownVariable("text", "customize me!",
                                             ["customize me!", "Thank you!"])
 
 #use scad_inline to use them
-scene = scad_inline("""
+scene = union()
+scene += scad_inline("""
                     for (i = [1:objects]){
                         translate([2*i*side,0,0]){
                             cube(side);
                         }
                     }
                     """)
```

### Comparing `solidpython2-2.0.1/solid2/examples/11-font/RichEatin.otf` & `solidpython2-2.0.2/solid2/examples/11-font/RichEatin.otf`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/examples/13-animated-bouncing-ball.py` & `solidpython2-2.0.2/solid2/examples/13-animated-bouncing-ball.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/examples/14-implicitCAD.py` & `solidpython2-2.0.2/solid2/examples/14-implicitCAD.x.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/examples/15-implicitCAD2.py` & `solidpython2-2.0.2/solid2/examples/15-implicitCAD2.x.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/examples/16-mazebox-bosl2.py` & `solidpython2-2.0.2/solid2/examples/16-mazebox-bosl2.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/examples/17-greedy-scad-interface.py` & `solidpython2-2.0.2/solid2/examples/17-greedy-scad-interface.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/examples/maze7.png` & `solidpython2-2.0.2/solid2/examples/maze7.png`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/affine.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/affine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/affine.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/affine.scad'}", use_not_include=False)
 
 class affine2d_identity(_Bosl2Base):
     def __init__(self, **kwargs):
        super().__init__("affine2d_identity", {**kwargs})
 
 class affine2d_translate(_Bosl2Base):
     def __init__(self, v=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/attachments.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/attachments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/attachments.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/attachments.scad'}", use_not_include=False)
 
 _tags = _OpenSCADConstant('_tags')
 _tag = _OpenSCADConstant('_tag')
 _tag_prefix = _OpenSCADConstant('_tag_prefix')
 _overlap = _OpenSCADConstant('_overlap')
 _color = _OpenSCADConstant('_color')
 _save_color = _OpenSCADConstant('_save_color')
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/ball_bearings.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/ball_bearings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/ball_bearings.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/ball_bearings.scad'}", use_not_include=False)
 
 class ball_bearing_info(_Bosl2Base):
     def __init__(self, trade_size=None, **kwargs):
        super().__init__("ball_bearing_info", {"trade_size" : trade_size, **kwargs})
 
 class ball_bearing(_Bosl2Base):
     def __init__(self, trade_size=None, id=None, od=None, width=None, shield=None, anchor=None, spin=None, orient=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/beziers.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/beziers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/beziers.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/beziers.scad'}", use_not_include=False)
 
 _bezier_matrix_table = _OpenSCADConstant('_bezier_matrix_table')
 class bezier_points(_Bosl2Base):
     def __init__(self, curve=None, u=None, **kwargs):
        super().__init__("bezier_points", {"curve" : curve, "u" : u, **kwargs})
 
 class _signed_pascals_triangle(_Bosl2Base):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/bosl2_access_syntax_mixin.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/bosl2_access_syntax_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,16 @@
 
-class Bosl2AccessSyntaxMixin:
+from solid2.core.object_base import AccessSyntaxMixin as _AccessSyntaxMixin
+
+class Bosl2AccessSyntaxMixin(_AccessSyntaxMixin):
 
     def _get_std(self):
         from . import std
         return std
 
-    def translate(self, v=None, **kwargs):
-        return self._get_std().translate(v, **kwargs)(self)
-
-    def scale(self, v=None, **kwargs):
-        return self._get_std().scale(v, **kwargs)(self)
-
-    def rotate(self, a=None, v=None, **kwargs):
-        return self._get_std().rotate(a, v, **kwargs)(self)
-
-    def mirror(self, v=None, **kwargs):
-        return self._get_std().mirror(v, **kwargs)(self)
-
-    def resize(self, newsize=None, auto=None, **kwargs):
-        return self._get_std().resize(newsize, auto, **kwargs)(self)
-
-    def color(self, c=None, alpha=None, **kwargs):
-        return self._get_std().color(c, alpha, **kwargs)(self)
-
-    def minkowski(self, **kwargs):
-        return self._get_std().minkowski(**kwargs)(self)
-
-    def offset(self, r=None, delta=None, chamfer=None, _fn=None, **kwargs):
-        return self._get_std().offset(r, delta, chamfer, _fn, **kwargs)(self)
-
-    def hull(self, **kwargs):
-        return self._get_std().hull(**kwargs)(self)
-
-    def render(self, convexity=None, **kwargs):
-        return self._get_std().render(convexity, **kwargs)(self)
-
-    def linear_extrude(self, height=None, center=None, convexity=None, twist=None, slices=None, scale=None, **kwargs):
-        return self._get_std().linear_extrude(height, center, convexity, twist, slices, scale, **kwargs)(self)
-
-    def rotate_extrude(self, angle=None, convexity=None, _fn=None, **kwargs):
-        return self._get_std().rotate_extrude(angle, convexity, _fn, **kwargs)(self)
-
-    def projection(self, cut=None, **kwargs):
-        return self._get_std().projection(cut, **kwargs)(self)
-
-    def surface(self, file=None, center=None, convexity=None, invert=None, **kwargs):
-        return self._get_std().surface(file, center, convexity, invert, **kwargs)(self)
-
     def move(self, v=None, p=None, **kwargs):
         return self._get_std().move(v, p, **kwargs)(self)
 
     def left(self, x=None, p=None, **kwargs):
         return self._get_std().left(x, p, **kwargs)(self)
 
     def right(self, x=None, p=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/bosl2_base.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/bosl2_base.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/bosl2_patches.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/bosl2_patches.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/bottlecaps.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/bottlecaps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/bottlecaps.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/bottlecaps.scad'}", use_not_include=False)
 
 _sp_specs = _OpenSCADConstant('_sp_specs')
 _sp_twist = _OpenSCADConstant('_sp_twist')
 _sp_thread_width = _OpenSCADConstant('_sp_thread_width')
 class pco1810_neck(_Bosl2Base):
     def __init__(self, wall=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("pco1810_neck", {"wall" : wall, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/color.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/color.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/color.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/color.scad'}", use_not_include=False)
 
 class hsl(_Bosl2Base):
     def __init__(self, h=None, s=None, l=None, a=None, **kwargs):
        super().__init__("hsl", {"h" : h, "s" : s, "l" : l, "a" : a, **kwargs})
 
 class hsv(_Bosl2Base):
     def __init__(self, h=None, s=None, v=None, a=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/comparisons.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/comparisons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/comparisons.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/comparisons.scad'}", use_not_include=False)
 
 class approx(_Bosl2Base):
     def __init__(self, a=None, b=None, eps=None, **kwargs):
        super().__init__("approx", {"a" : a, "b" : b, "eps" : eps, **kwargs})
 
 class all_zero(_Bosl2Base):
     def __init__(self, x=None, eps=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/constants.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/constants.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/constants.scad'}", use_not_include=False)
 
 _UNDEF = _OpenSCADConstant('_UNDEF')
 INCH = _OpenSCADConstant('INCH')
 LEFT = _OpenSCADConstant('LEFT')
 RIGHT = _OpenSCADConstant('RIGHT')
 FRONT = _OpenSCADConstant('FRONT')
 FWD = _OpenSCADConstant('FWD')
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/coords.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/coords.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/coords.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/coords.scad'}", use_not_include=False)
 
 class point2d(_Bosl2Base):
     def __init__(self, p=None, fill=None, **kwargs):
        super().__init__("point2d", {"p" : p, "fill" : fill, **kwargs})
 
 class path2d(_Bosl2Base):
     def __init__(self, points=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/cubetruss.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/cubetruss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/cubetruss.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/cubetruss.scad'}", use_not_include=False)
 
 _cubetruss_size = _OpenSCADConstant('_cubetruss_size')
 _cubetruss_strut_size = _OpenSCADConstant('_cubetruss_strut_size')
 _cubetruss_bracing = _OpenSCADConstant('_cubetruss_bracing')
 _cubetruss_clip_thickness = _OpenSCADConstant('_cubetruss_clip_thickness')
 class cubetruss_dist(_Bosl2Base):
     def __init__(self, cubes=None, gaps=None, size=None, strut=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/distributors.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/distributors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/distributors.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/distributors.scad'}", use_not_include=False)
 
 class move_copies(_Bosl2Base):
     def __init__(self, a=None, p=None, **kwargs):
        super().__init__("move_copies", {"a" : a, "p" : p, **kwargs})
 
 class xcopies(_Bosl2Base):
     def __init__(self, spacing=None, n=None, l=None, sp=None, p=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/drawing.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/drawing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/drawing.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/drawing.scad'}", use_not_include=False)
 
 class stroke(_Bosl2Base):
     def __init__(self, path=None, width=None, closed=None, endcaps=None, endcap1=None, endcap2=None, joints=None, dots=None, endcap_width=None, endcap_width1=None, endcap_width2=None, joint_width=None, dots_width=None, endcap_length=None, endcap_length1=None, endcap_length2=None, joint_length=None, dots_length=None, endcap_extent=None, endcap_extent1=None, endcap_extent2=None, joint_extent=None, dots_extent=None, endcap_angle=None, endcap_angle1=None, endcap_angle2=None, joint_angle=None, dots_angle=None, endcap_color=None, endcap_color1=None, endcap_color2=None, joint_color=None, dots_color=None, color=None, trim=None, trim1=None, trim2=None, singleton_scale=None, convexity=None, **kwargs):
        super().__init__("stroke", {"path" : path, "width" : width, "closed" : closed, "endcaps" : endcaps, "endcap1" : endcap1, "endcap2" : endcap2, "joints" : joints, "dots" : dots, "endcap_width" : endcap_width, "endcap_width1" : endcap_width1, "endcap_width2" : endcap_width2, "joint_width" : joint_width, "dots_width" : dots_width, "endcap_length" : endcap_length, "endcap_length1" : endcap_length1, "endcap_length2" : endcap_length2, "joint_length" : joint_length, "dots_length" : dots_length, "endcap_extent" : endcap_extent, "endcap_extent1" : endcap_extent1, "endcap_extent2" : endcap_extent2, "joint_extent" : joint_extent, "dots_extent" : dots_extent, "endcap_angle" : endcap_angle, "endcap_angle1" : endcap_angle1, "endcap_angle2" : endcap_angle2, "joint_angle" : joint_angle, "dots_angle" : dots_angle, "endcap_color" : endcap_color, "endcap_color1" : endcap_color1, "endcap_color2" : endcap_color2, "joint_color" : joint_color, "dots_color" : dots_color, "color" : color, "trim" : trim, "trim1" : trim1, "trim2" : trim2, "singleton_scale" : singleton_scale, "convexity" : convexity, **kwargs})
 
 class dashed_stroke(_Bosl2Base):
     def __init__(self, path=None, dashpat=None, closed=None, fit=None, mindash=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/fnliterals.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/fnliterals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/fnliterals.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/fnliterals.scad'}", use_not_include=False)
 
 class map(_Bosl2Base):
     def __init__(self, func=None, list=None, **kwargs):
        super().__init__("map", {"func" : func, "list" : list, **kwargs})
 
 class filter(_Bosl2Base):
     def __init__(self, func=None, list=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/gears.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/gears.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/gears.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/gears.scad'}", use_not_include=False)
 
 class spur_gear(_Bosl2Base):
     def __init__(self, pitch=None, teeth=None, thickness=None, shaft_diam=None, hide=None, pressure_angle=None, clearance=None, backlash=None, helical=None, slices=None, interior=None, mod=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("spur_gear", {"pitch" : pitch, "teeth" : teeth, "thickness" : thickness, "shaft_diam" : shaft_diam, "hide" : hide, "pressure_angle" : pressure_angle, "clearance" : clearance, "backlash" : backlash, "helical" : helical, "slices" : slices, "interior" : interior, "mod" : mod, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
 class spur_gear2d(_Bosl2Base):
     def __init__(self, pitch=None, teeth=None, hide=None, pressure_angle=None, clearance=None, backlash=None, interior=None, mod=None, anchor=None, spin=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/geometry.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/geometry.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/geometry.scad'}", use_not_include=False)
 
 class is_point_on_line(_Bosl2Base):
     def __init__(self, point=None, line=None, bounded=None, eps=None, **kwargs):
        super().__init__("is_point_on_line", {"point" : point, "line" : line, "bounded" : bounded, "eps" : eps, **kwargs})
 
 class _is_point_on_line(_Bosl2Base):
     def __init__(self, point=None, line=None, bounded=None, eps=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/hinges.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/hinges.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/hinges.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/hinges.scad'}", use_not_include=False)
 
 class knuckle_hinge(_Bosl2Base):
     def __init__(self, length=None, segs=None, offset=None, inner=None, arm_height=None, arm_angle=None, gap=None, seg_ratio=None, knuckle_diam=None, pin_diam=None, fill=None, clear_top=None, round_bot=None, round_top=None, pin_fn=None, clearance=None, tap_depth=None, screw_head=None, screw_tolerance=None, anchor=None, orient=None, spin=None, **kwargs):
        super().__init__("knuckle_hinge", {"length" : length, "segs" : segs, "offset" : offset, "inner" : inner, "arm_height" : arm_height, "arm_angle" : arm_angle, "gap" : gap, "seg_ratio" : seg_ratio, "knuckle_diam" : knuckle_diam, "pin_diam" : pin_diam, "fill" : fill, "clear_top" : clear_top, "round_bot" : round_bot, "round_top" : round_top, "pin_fn" : pin_fn, "clearance" : clearance, "tap_depth" : tap_depth, "screw_head" : screw_head, "screw_tolerance" : screw_tolerance, "anchor" : anchor, "orient" : orient, "spin" : spin, **kwargs})
 
 class knuckle_hinge(_Bosl2Base):
     def __init__(self, length=None, segs=None, offset=None, inner=None, arm_height=None, arm_angle=None, gap=None, seg_ratio=None, knuckle_diam=None, pin_diam=None, fill=None, clear_top=None, round_bot=None, round_top=None, pin_fn=None, clearance=None, teardrop=None, tap_depth=None, screw_head=None, screw_tolerance=None, knuckle_clearance=None, anchor=None, orient=None, spin=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/joiners.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/joiners.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/joiners.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/joiners.scad'}", use_not_include=False)
 
 class half_joiner_clear(_Bosl2Base):
     def __init__(self, l=None, w=None, ang=None, clearance=None, overlap=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("half_joiner_clear", {"l" : l, "w" : w, "ang" : ang, "clearance" : clearance, "overlap" : overlap, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
 class half_joiner(_Bosl2Base):
     def __init__(self, l=None, w=None, base=None, ang=None, screwsize=None, anchor=None, spin=None, orient=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/linalg.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/linalg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/linalg.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/linalg.scad'}", use_not_include=False)
 
 class is_matrix(_Bosl2Base):
     def __init__(self, A=None, m=None, n=None, square=None, **kwargs):
        super().__init__("is_matrix", {"A" : A, "m" : m, "n" : n, "square" : square, **kwargs})
 
 class is_matrix_symmetric(_Bosl2Base):
     def __init__(self, A=None, eps=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/linear_bearings.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/linear_bearings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/linear_bearings.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/linear_bearings.scad'}", use_not_include=False)
 
 class lmXuu_info(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("lmXuu_info", {"size" : size, **kwargs})
 
 class linear_bearing_housing(_Bosl2Base):
     def __init__(self, d=None, l=None, tab=None, gap=None, wall=None, tabwall=None, screwsize=None, anchor=None, spin=None, orient=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/lists.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/lists.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/lists.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/lists.scad'}", use_not_include=False)
 
 class is_homogeneous(_Bosl2Base):
     def __init__(self, l=None, depth=None, **kwargs):
        super().__init__("is_homogeneous", {"l" : l, "depth" : depth, **kwargs})
 
 class is_homogenous(_Bosl2Base):
     def __init__(self, l=None, depth=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/masks2d.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/masks2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/masks2d.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/masks2d.scad'}", use_not_include=False)
 
 class mask2d_roundover(_Bosl2Base):
     def __init__(self, r=None, inset=None, excess=None, d=None, anchor=None, spin=None, **kwargs):
        super().__init__("mask2d_roundover", {"r" : r, "inset" : inset, "excess" : excess, "d" : d, "anchor" : anchor, "spin" : spin, **kwargs})
 
 class mask2d_cove(_Bosl2Base):
     def __init__(self, r=None, inset=None, excess=None, d=None, anchor=None, spin=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/masks3d.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/masks3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/masks3d.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/masks3d.scad'}", use_not_include=False)
 
 class chamfer_edge_mask(_Bosl2Base):
     def __init__(self, l=None, chamfer=None, excess=None, h=None, length=None, height=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("chamfer_edge_mask", {"l" : l, "chamfer" : chamfer, "excess" : excess, "h" : h, "length" : length, "height" : height, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
 class chamfer_corner_mask(_Bosl2Base):
     def __init__(self, chamfer=None, anchor=None, spin=None, orient=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/math.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/math.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/math.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/math.scad'}", use_not_include=False)
 
 PHI = _OpenSCADConstant('PHI')
 EPSILON = _OpenSCADConstant('EPSILON')
 INF = _OpenSCADConstant('INF')
 NAN = _OpenSCADConstant('NAN')
 class count(_Bosl2Base):
     def __init__(self, n=None, s=None, step=None, reverse=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/metric_screws.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/metric_screws.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/metric_screws.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/metric_screws.scad'}", use_not_include=False)
 
 class get_metric_bolt_head_size(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("get_metric_bolt_head_size", {"size" : size, **kwargs})
 
 class get_metric_bolt_head_height(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/modular_hose.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/modular_hose.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/modular_hose.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/modular_hose.scad'}", use_not_include=False)
 
 _small_end = _OpenSCADConstant('_small_end')
 _big_end = _OpenSCADConstant('_big_end')
 _hose_waist = _OpenSCADConstant('_hose_waist')
 class modular_hose(_Bosl2Base):
     def __init__(self, size=None, type=None, clearance=None, waist_len=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("modular_hose", {"size" : size, "type" : type, "clearance" : clearance, "waist_len" : waist_len, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/mutators.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/mutators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/mutators.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/mutators.scad'}", use_not_include=False)
 
 class bounding_box(_Bosl2Base):
     def __init__(self, excess=None, planar=None, **kwargs):
        super().__init__("bounding_box", {"excess" : excess, "planar" : planar, **kwargs})
 
 class chain_hull(_Bosl2Base):
     def __init__(self, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/nema_steppers.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/nema_steppers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/nema_steppers.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/nema_steppers.scad'}", use_not_include=False)
 
 class nema_motor_info(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("nema_motor_info", {"size" : size, **kwargs})
 
 class nema_stepper_motor(_Bosl2Base):
     def __init__(self, size=None, h=None, shaft_len=None, details=None, atype=None, anchor=None, spin=None, orient=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/openscad.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/openscad.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/partitions.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/partitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/partitions.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/partitions.scad'}", use_not_include=False)
 
 class half_of(_Bosl2Base):
     def __init__(self, p=None, v=None, cp=None, **kwargs):
        super().__init__("half_of", {"p" : p, "v" : v, "cp" : cp, **kwargs})
 
 class left_half(_Bosl2Base):
     def __init__(self, p=None, x=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/paths.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/paths.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/paths.scad'}", use_not_include=False)
 
 class is_path(_Bosl2Base):
     def __init__(self, list=None, dim=None, fast=None, **kwargs):
        super().__init__("is_path", {"list" : list, "dim" : dim, "fast" : fast, **kwargs})
 
 class is_1region(_Bosl2Base):
     def __init__(self, path=None, name=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/polyhedra.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/polyhedra.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/polyhedra.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/polyhedra.scad'}", use_not_include=False)
 
 _tribonacci = _OpenSCADConstant('_tribonacci')
 _polyhedra_ = _OpenSCADConstant('_polyhedra_')
 _stellated_polyhedra_ = _OpenSCADConstant('_stellated_polyhedra_')
 class _unique_groups(_Bosl2Base):
     def __init__(self, m=None, **kwargs):
        super().__init__("_unique_groups", {"m" : m, **kwargs})
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/regions.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/regions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/regions.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/regions.scad'}", use_not_include=False)
 
 class is_region(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("is_region", {"x" : x, **kwargs})
 
 class is_valid_region(_Bosl2Base):
     def __init__(self, region=None, eps=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/rounding.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/rounding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/rounding.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/rounding.scad'}", use_not_include=False)
 
 class round_corners(_Bosl2Base):
     def __init__(self, path=None, method=None, radius=None, r=None, cut=None, joint=None, width=None, k=None, closed=None, verbose=None, **kwargs):
        super().__init__("round_corners", {"path" : path, "method" : method, "radius" : radius, "r" : r, "cut" : cut, "joint" : joint, "width" : width, "k" : k, "closed" : closed, "verbose" : verbose, **kwargs})
 
 class _smooth_bez_fill(_Bosl2Base):
     def __init__(self, points=None, k=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/screw_drive.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/screw_drive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/screw_drive.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/screw_drive.scad'}", use_not_include=False)
 
 class _phillips_shaft(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("_phillips_shaft", {"x" : x, **kwargs})
 
 class _ph_bot_angle(_Bosl2Base):
     def __init__(self, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/screws.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/screws.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/screws.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/screws.scad'}", use_not_include=False)
 
 class _get_spec(_Bosl2Base):
     def __init__(self, spec=None, needtype=None, origin=None, thread=None, head=None, drive=None, drive_size=None, shape=None, thickness=None, **kwargs):
        super().__init__("_get_spec", {"spec" : spec, "needtype" : needtype, "origin" : origin, "thread" : thread, "head" : head, "drive" : drive, "drive_size" : drive_size, "shape" : shape, "thickness" : thickness, **kwargs})
 
 class _struct_reset(_Bosl2Base):
     def __init__(self, s=None, keyval=None, grow=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/shapes2d.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/shapes2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/shapes2d.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/shapes2d.scad'}", use_not_include=False)
 
 class square(_Bosl2Base):
     def __init__(self, size=None, center=None, anchor=None, spin=None, **kwargs):
        super().__init__("square", {"size" : size, "center" : center, "anchor" : anchor, "spin" : spin, **kwargs})
 
 class rect(_Bosl2Base):
     def __init__(self, size=None, rounding=None, chamfer=None, atype=None, anchor=None, spin=None, _return_override=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/shapes3d.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/shapes3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/shapes3d.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/shapes3d.scad'}", use_not_include=False)
 
 class cube(_Bosl2Base):
     def __init__(self, size=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("cube", {"size" : size, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
 class cuboid(_Bosl2Base):
     def __init__(self, size=None, p1=None, p2=None, chamfer=None, rounding=None, edges=None, except_edges=None, trimcorners=None, anchor=None, spin=None, orient=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/skin.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/skin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/skin.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/skin.scad'}", use_not_include=False)
 
 _leadin_ogive = _OpenSCADConstant('_leadin_ogive')
 _leadin_cut = _OpenSCADConstant('_leadin_cut')
 _leadin_sqrt = _OpenSCADConstant('_leadin_sqrt')
 _leadin_linear = _OpenSCADConstant('_leadin_linear')
 _lead_in_table = _OpenSCADConstant('_lead_in_table')
 _MAP_DIAG = _OpenSCADConstant('_MAP_DIAG')
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/sliders.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/sliders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/sliders.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/sliders.scad'}", use_not_include=False)
 
 class slider(_Bosl2Base):
     def __init__(self, l=None, w=None, h=None, base=None, wall=None, ang=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("slider", {"l" : l, "w" : w, "h" : h, "base" : base, "wall" : wall, "ang" : ang, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
 class rail(_Bosl2Base):
     def __init__(self, l=None, w=None, h=None, chamfer=None, ang=None, anchor=None, spin=None, orient=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/std.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/std.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/strings.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/strings.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/strings.scad'}", use_not_include=False)
 
 class substr(_Bosl2Base):
     def __init__(self, str=None, pos=None, len=None, **kwargs):
        super().__init__("substr", {"str" : str, "pos" : pos, "len" : len, **kwargs})
 
 class _substr(_Bosl2Base):
     def __init__(self, str=None, pos=None, len=None, substr=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/structs.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/structs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/structs.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/structs.scad'}", use_not_include=False)
 
 class struct_set(_Bosl2Base):
     def __init__(self, struct=None, key=None, value=None, grow=None, **kwargs):
        super().__init__("struct_set", {"struct" : struct, "key" : key, "value" : value, "grow" : grow, **kwargs})
 
 class _format_key(_Bosl2Base):
     def __init__(self, key=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/threading.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/threading.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/threading.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/threading.scad'}", use_not_include=False)
 
 class threaded_rod(_Bosl2Base):
     def __init__(self, d=None, l=None, pitch=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, starts=None, internal=None, d1=None, d2=None, length=None, h=None, height=None, blunt_start=None, blunt_start1=None, blunt_start2=None, lead_in=None, lead_in1=None, lead_in2=None, lead_in_ang=None, lead_in_ang1=None, lead_in_ang2=None, end_len=None, end_len1=None, end_len2=None, lead_in_shape=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("threaded_rod", {"d" : d, "l" : l, "pitch" : pitch, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "starts" : starts, "internal" : internal, "d1" : d1, "d2" : d2, "length" : length, "h" : h, "height" : height, "blunt_start" : blunt_start, "blunt_start1" : blunt_start1, "blunt_start2" : blunt_start2, "lead_in" : lead_in, "lead_in1" : lead_in1, "lead_in2" : lead_in2, "lead_in_ang" : lead_in_ang, "lead_in_ang1" : lead_in_ang1, "lead_in_ang2" : lead_in_ang2, "end_len" : end_len, "end_len1" : end_len1, "end_len2" : end_len2, "lead_in_shape" : lead_in_shape, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
 class threaded_nut(_Bosl2Base):
     def __init__(self, nutwidth=None, id=None, h=None, pitch=None, starts=None, shape=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, id1=None, id2=None, ibevel1=None, ibevel2=None, ibevel=None, bevang=None, thickness=None, height=None, length=None, l=None, blunt_start=None, blunt_start1=None, blunt_start2=None, lead_in=None, lead_in1=None, lead_in2=None, lead_in_ang=None, lead_in_ang1=None, lead_in_ang2=None, end_len=None, end_len1=None, end_len2=None, lead_in_shape=None, anchor=None, spin=None, orient=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/transforms.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/transforms.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/transforms.scad'}", use_not_include=False)
 
 _NO_ARG = _OpenSCADConstant('_NO_ARG')
 class move(_Bosl2Base):
     def __init__(self, v=None, p=None, **kwargs):
        super().__init__("move", {"v" : v, "p" : p, **kwargs})
 
 class translate(_Bosl2Base):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/trigonometry.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/trigonometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/trigonometry.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/trigonometry.scad'}", use_not_include=False)
 
 class law_of_cosines(_Bosl2Base):
     def __init__(self, a=None, b=None, c=None, C=None, **kwargs):
        super().__init__("law_of_cosines", {"a" : a, "b" : b, "c" : c, "C" : C, **kwargs})
 
 class law_of_sines(_Bosl2Base):
     def __init__(self, a=None, A=None, b=None, B=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/tripod_mounts.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/tripod_mounts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/tripod_mounts.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/tripod_mounts.scad'}", use_not_include=False)
 
 class manfrotto_rc2_plate(_Bosl2Base):
     def __init__(self, chamfer=None, anchor=None, orient=None, spin=None, **kwargs):
        super().__init__("manfrotto_rc2_plate", {"chamfer" : chamfer, "anchor" : anchor, "orient" : orient, "spin" : spin, **kwargs})
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/turtle3d.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/turtle3d.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/turtle3d.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/turtle3d.scad'}", use_not_include=False)
 
 class _transpart(_Bosl2Base):
     def __init__(self, T=None, **kwargs):
        super().__init__("_transpart", {"T" : T, **kwargs})
 
 class _rotpart(_Bosl2Base):
     def __init__(self, T=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/utility.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/utility.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/utility.scad'}", use_not_include=False)
 
 class typeof(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("typeof", {"x" : x, **kwargs})
 
 class is_type(_Bosl2Base):
     def __init__(self, x=None, types=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/vectors.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/vectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/vectors.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/vectors.scad'}", use_not_include=False)
 
 class is_vector(_Bosl2Base):
     def __init__(self, v=None, length=None, zero=None, all_nonzero=None, eps=None, **kwargs):
        super().__init__("is_vector", {"v" : v, "length" : length, "zero" : zero, "all_nonzero" : all_nonzero, "eps" : eps, **kwargs})
 
 class add_scalar(_Bosl2Base):
     def __init__(self, v=None, s=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/version.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/version.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/version.scad'}", use_not_include=False)
 
 BOSL_VERSION = _OpenSCADConstant('BOSL_VERSION')
 class bosl_version(_Bosl2Base):
     def __init__(self, **kwargs):
        super().__init__("bosl_version", {**kwargs})
 
 class bosl_version_num(_Bosl2Base):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/vnf.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/vnf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/vnf.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/vnf.scad'}", use_not_include=False)
 
 EMPTY_VNF = _OpenSCADConstant('EMPTY_VNF')
 _vnf_validate_errs = _OpenSCADConstant('_vnf_validate_errs')
 class vnf_vertex_array(_Bosl2Base):
     def __init__(self, points=None, caps=None, cap1=None, cap2=None, col_wrap=None, row_wrap=None, reverse=None, style=None, **kwargs):
        super().__init__("vnf_vertex_array", {"points" : points, "caps" : caps, "cap1" : cap1, "cap2" : cap2, "col_wrap" : col_wrap, "row_wrap" : row_wrap, "reverse" : reverse, "style" : style, **kwargs})
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/walls.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/walls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/walls.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/walls.scad'}", use_not_include=False)
 
 class sparse_wall(_Bosl2Base):
     def __init__(self, h=None, l=None, thick=None, maxang=None, strut=None, max_bridge=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("sparse_wall", {"h" : h, "l" : l, "thick" : thick, "maxang" : maxang, "strut" : strut, "max_bridge" : max_bridge, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
 class corrugated_wall(_Bosl2Base):
     def __init__(self, h=None, l=None, thick=None, strut=None, wall=None, anchor=None, spin=None, orient=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2/wiring.py` & `solidpython2-2.0.2/solid2/extensions/bosl2/wiring.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/wiring.scad'}", use_not_include=False)
+_extra_scad_include(f"{_Path(__file__).parent.parent / 'bosl2/BOSL2/wiring.scad'}", use_not_include=False)
 
 class _hex_offset_ring(_Bosl2Base):
     def __init__(self, d=None, lev=None, **kwargs):
        super().__init__("_hex_offset_ring", {"d" : d, "lev" : lev, **kwargs})
 
 class _hex_offsets(_Bosl2Base):
     def __init__(self, n=None, d=None, lev=None, arr=None, **kwargs):
```

### Comparing `solidpython2-2.0.1/solid2/extensions/bosl2_generator.py` & `solidpython2-2.0.2/solid2/extensions/bosl2_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,84 +10,75 @@
 headerTemplate = """\
 from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
 from solid2.core.scad_import import extra_scad_include as _extra_scad_include
 from pathlib import Path as _Path
 
 from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_extra_scad_include(f"{{_Path(__file__).parent.parent / '{scadFile}'}}", use_not_include={use_not_include})
+_extra_scad_include(f"{{_Path(__file__).parent.parent / '{scadFile}'}}", {use_not_include})
 
 """
 
 callableTemplate = """\
 class {name}(_Bosl2Base):
     def __init__({paramStr}):
        super().__init__({initStr})
 
 """
 
 mixinHeader = """
-class Bosl2AccessSyntaxMixin:
+from solid2.core.object_base import AccessSyntaxMixin as _AccessSyntaxMixin
+
+class Bosl2AccessSyntaxMixin(_AccessSyntaxMixin):
 
     def _get_std(self):
         from . import std
         return std
 """
 mixinTemplate = """
     def {name}(self, {paramListWithDefaults}**kwargs):
         return self._get_std().{name}({paramList}**kwargs)(self)
 """
 
-scad_builtins_mutators = \
-    Path(__file__).parent.parent / "core" / "builtins" / "openscad.mutators"
 scad_builtins_primitives = \
     Path(__file__).parent.parent / "core" / "builtins" / "openscad.primitives"
 
 def generateBosl2Std(bosl2_dir):
     stubFile = Path(__file__).absolute().parent / "bosl2" / "std.py"
 
     with open(stubFile, "w") as std_f:
         std_f.write("from .openscad import *\n")
-        stdlibs = []
         with open(bosl2_dir / "std.scad") as f:
             for l in f.readlines():
                 l = l.strip()
                 if not l.startswith("include <"):
                     continue
                 l = l.replace("include <", "").replace(">", "")
                 std_f.write(f"from .{Path(l).stem} import *\n")
-                stdlibs.append(l)
-
-            # for f in bosl2_dir.iterdir():
-            #     if not f.suffix == ".scad" or f.name in stdlibs:
-            #         continue
-            #     std_f.write(f"from . import {f.stem}\n")
-
 
 def generateBosl2AccessSyntaxMixin(bosl2_dir, outputDir):
     def generateCallable(c):
         name = escape(c.name)
         paramNames = [escape(p.name) for p in c.parameters]
+        paramNames = list(dict.fromkeys(paramNames))
 
         paramListWithDefaults = ", ".join([f"{p}=None" for p in paramNames])
         paramList = ", ".join([f'{p}' for p in paramNames])
 
         if paramListWithDefaults: paramListWithDefaults += ", "
         if paramList: paramList += ", "
 
         return mixinTemplate.format(name=name,
                                     paramListWithDefaults=paramListWithDefaults,
                                     paramList=paramList)
 
-    mixinFiles = [scad_builtins_mutators]
-
     mods = ["transforms", "attachments", "mutators",
             "distributors", "partitions", "color"]
-    for m in mods:
-        mixinFiles.append((bosl2_dir / m).with_suffix(".scad"))
+
+    mixinFiles = [(bosl2_dir / m).with_suffix(".scad") for m in mods]
 
     modules = []
     for f in mixinFiles:
         m, _, _ = scad_parser.parseFile(f)
         modules += m
 
 
@@ -95,15 +86,15 @@
         f.write(mixinHeader)
 
         for c in modules:
             if c.name.startswith("_"):
                 continue
             f.write(generateCallable(c))
 
-bosl2_dir = Path("../libs/BOSL2")
+bosl2_dir = Path("./bosl2/BOSL2")
 output_dir = Path(__file__).parent / "bosl2"
 
 makePackage(output_dir)
 generateBosl2Std(bosl2_dir)
 generateBosl2AccessSyntaxMixin(bosl2_dir, output_dir)
 
 for f in bosl2_dir.iterdir():
@@ -113,11 +104,11 @@
         continue
 
     generateStub(f, output_dir, False,
                  headerTemplate=headerTemplate,
                  callableTemplate=callableTemplate)
 
 generateStub(scad_builtins_primitives, output_dir, False,
-                headerTemplate=\
-                    "from .bosl2_base import Bosl2Base as _Bosl2Base\n\n",
-                callableTemplate=callableTemplate)
+             headerTemplate=\
+                 "from .bosl2_base import Bosl2Base as _Bosl2Base\n\n",
+             callableTemplate=callableTemplate)
```

### Comparing `solidpython2-2.0.1/solid2/extensions/greedy_scad_interface/customizer_widgets.py` & `solidpython2-2.0.2/solid2/extensions/greedy_scad_interface/customizer_widgets.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/extensions/greedy_scad_interface/scad_interface.py` & `solidpython2-2.0.2/solid2/extensions/greedy_scad_interface/scad_interface.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/extensions/greedy_scad_interface/scad_variable.py` & `solidpython2-2.0.2/solid2/extensions/greedy_scad_interface/scad_variable.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/extensions/openscad_extension_generator.py` & `solidpython2-2.0.2/solid2/extensions/openscad_extension_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
     def generateConstant(c):
         return constantTemplate.format(name=escape(c.name)) + "\n"
 
     def generateCallable(c):
         name = escape(c.name)
         paramNames = [escape(p.name) for p in c.parameters]
+        paramNames = list(dict.fromkeys(paramNames))
 
         paramStr = ", ".join(["self"] +
                              [f"{p}=None" for p in paramNames] +
                              ["**kwargs"])
         initList = [f'"{p}" : {p}' for p in paramNames]
         initList.append("**kwargs")
         initStr = f'"{name}", {{{", ".join(initList)}}}'
```

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/affine.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/affine.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/attachments.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/attachments.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/ball_bearings.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/ball_bearings.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/beziers.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/beziers.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/bosl1compat.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/bosl1compat.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/bottlecaps.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/bottlecaps.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/builtins.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/builtins.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/color.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/color.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/comparisons.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/comparisons.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/constants.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/constants.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/coords.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/coords.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/cubetruss.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/cubetruss.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/distributors.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/distributors.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/drawing.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/drawing.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/fnliterals.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/fnliterals.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/gears.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/gears.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/geometry.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/geometry.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/hinges.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/hinges.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/joiners.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/joiners.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/linalg.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/linalg.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/linear_bearings.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/linear_bearings.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/lists.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/lists.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/masks2d.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/masks2d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/masks3d.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/masks3d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/math.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/math.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/metric_screws.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/metric_screws.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/modular_hose.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/modular_hose.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/mutators.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/mutators.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/nema_steppers.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/nema_steppers.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/partitions.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/partitions.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/paths.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/paths.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/polyhedra.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/polyhedra.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/regions.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/regions.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/rounding.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/rounding.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/screw_drive.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/screw_drive.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/screws.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/screws.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/shapes2d.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/shapes2d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/shapes3d.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/shapes3d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/skin.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/skin.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/sliders.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/sliders.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/std.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/std.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/strings.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/strings.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/structs.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/structs.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/threading.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/threading.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/transforms.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/transforms.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/trigonometry.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/trigonometry.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/tripod_mounts.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/tripod_mounts.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/turtle3d.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/turtle3d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/utility.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/utility.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/vectors.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/vectors.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/version.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/version.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/vnf.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/vnf.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/walls.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/walls.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/BOSL2/wiring.scad` & `solidpython2-2.0.2/solid2/extensions/bosl2/BOSL2/wiring.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/py_scadparser/LICENSE` & `solidpython2-2.0.2/solid2/libs/py_scadparser/LICENSE`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/py_scadparser/README.md` & `solidpython2-2.0.2/solid2/libs/py_scadparser/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,6 +1,8 @@
 # py_scadparser
 A basic openscad parser written in python using ply.
 
-This parser is intended to be used within solidpython to import openscad code. For this purpose we only need to extract the global definitions of a openscad file. That's exactly what this package does. It parses a openscad file and extracts top level definitions. This includes "use"d and "include"d filenames, global variables, function and module definitions.
+This parser is intended to be used within solidpython to import openscad code. For this purpose we only need to extract the global definitions of a openscad file. That's exactly what this package does. It parses a openscad file and extracts top level definitions. This includes global variables, function and module definitions.
 
 Even though this parser actually parses (almost?) the entire openscad language (at least the portions used in my test libraries) 90% is dismissed and only the needed definitions are processed and extracted.
+
+For information on what this parser is capable of and how to use it, take a look at the bottom of scad_parser.py.
```

### Comparing `solidpython2-2.0.1/solid2/libs/py_scadparser/parsetab.py` & `solidpython2-2.0.2/solid2/libs/py_scadparser/parsetab.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/py_scadparser/scad_ast.py` & `solidpython2-2.0.2/solid2/libs/py_scadparser/scad_ast.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/py_scadparser/scad_parser.py` & `solidpython2-2.0.2/solid2/libs/py_scadparser/scad_parser.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.1/solid2/libs/py_scadparser/scad_tokens.py` & `solidpython2-2.0.2/solid2/libs/py_scadparser/scad_tokens.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,38 +41,34 @@
 #LICENSE: BSD
 simple_escape = r"""([a-wyzA-Z._~!=&\^\-\\?'"]|x(?![0-9a-fA-F]))"""
 decimal_escape = r"""(\d+)(?!\d)"""
 hex_escape = r"""(x[0-9a-fA-F]+)(?![0-9a-fA-F])"""
 bad_escape = r"""([\\][^a-zA-Z._~^!=&\^\-\\?'"x0-9])"""
 escape_sequence = r"""(\\("""+simple_escape+'|'+decimal_escape+'|'+hex_escape+'))'
 escape_sequence_start_in_string = r"""(\\[0-9a-zA-Z._~!=&\^\-\\?'"])"""
-string_char = r"""([^"\\] | """+escape_sequence_start_in_string+')'
+string_char = r"""([^"\\]|"""+escape_sequence_start_in_string+')'
 t_STRING = '"'+string_char+'*"' + " | " + "'" +string_char+ "*'"
 
 t_EQUAL = "=="
 t_GREATER_OR_EQUAL = ">="
 t_LESS_OR_EQUAL = "<="
 t_NOT_EQUAL = "!="
-t_AND = r"\&\&"
-t_OR = r"\|\|"
+t_AND = "\&\&"
+t_OR = "\|\|"
 
 t_FILENAME = r'<[a-zA-Z_0-9/\\\.-]*>'
 
-def t_eat_escaped_quotes(t):
-    r"\\\""
-    pass
-
 def t_comments1(t):
     r'(/\*(.|\n)*?\*/)'
     t.lexer.lineno += t.value.count("\n")
     pass
 
 def t_comments2(t):
-    r'//.*[\n\']?'
-    t.lexer.lineno += 1
+    r'//.*[\n]?'
+    t.lexer.lineno += t.value.count("\n")
     pass
 
 def t_whitespace(t):
     r'\s'
     t.lexer.lineno += t.value.count("\n")
 
 def t_ID(t):
```

### Comparing `solidpython2-2.0.1/setup.py` & `solidpython2-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,27 +5,37 @@
 ['solid2',
  'solid2.core',
  'solid2.core.builtins',
  'solid2.core.object_base',
  'solid2.examples',
  'solid2.extensions',
  'solid2.extensions.bosl2',
+ 'solid2.extensions.bosl2.BOSL2.scripts',
  'solid2.extensions.greedy_scad_interface',
  'solid2.libs',
  'solid2.libs.py_scadparser']
 
 package_data = \
-{'': ['*'], 'solid2.examples': ['11-font/*'], 'solid2.libs': ['BOSL2/*']}
+{'': ['*'],
+ 'solid2.examples': ['11-font/*'],
+ 'solid2.extensions.bosl2': ['BOSL2/*',
+                             'BOSL2/.github/*',
+                             'BOSL2/.github/ISSUE_TEMPLATE/*',
+                             'BOSL2/.github/workflows/*',
+                             'BOSL2/examples/*',
+                             'BOSL2/images/*',
+                             'BOSL2/tests/*',
+                             'BOSL2/tutorials/*']}
 
 install_requires = \
 ['ply>=3.11,<4.0', 'setuptools>=65.6.3']
 
 setup_kwargs = {
     'name': 'solidpython2',
-    'version': '2.0.1',
+    'version': '2.0.2',
     'description': 'Python interface to the OpenSCAD declarative geometry language',
     'long_description': '\n.. image:: https://readthedocs.org/projects/solidpython2/badge/?version=latest\n    :target: http://solidpython2.readthedocs.io/en/latest/?badge=latest\n    :alt: Documentation Status\n\n**If you switch from the regular SolidPython:master branch to this branch, have a\nlook at** `Version 2.x.x`_.\n\nSolidPython\n===========\n\n.. contents::\n   \nOpenSCAD for Python\n-------------------\n\nSolidPython is a generalization of Phillip Tiefenbacher\'s openscad\nmodule, found on `Thingiverse <http://www.thingiverse.com/thing:1481>`__. It\ngenerates valid OpenSCAD code from Python code with minimal overhead. Here\'s a\nsimple example:\n\nThis Python code:\n\n.. code:: python\n\n    from solid2 import *\n    d = difference()(\n        cube(10),\n        sphere(15)\n    )\n    d.as_scad()\n\nGenerates this OpenSCAD code:\n\n.. code:: python\n\n    difference(){\n        cube(10);\n        sphere(15);\n    }\n\nThat doesn\'t seem like such a savings, but the following SolidPython code is a\nlot shorter (and I think clearer) than the SCAD code it compiles to:\n\n.. code:: python\n\n    from solid2 import *\n    d = cube(5) + right(5)(sphere(5)) - cylinder(r=2, h=6)\n\nGenerates this OpenSCAD code:\n\n.. code::\n\n    difference(){\n        union(){\n            cube(5);\n            translate( [5, 0,0]){\n                sphere(5);\n            }\n        }\n        cylinder(r=2, h=6);\n    }\n\nAdvantages\n----------\n\nIn contrast to OpenSCAD -- which is a constrained domain specific language --\nPython is a full blown modern programming language and as such supports\npretty much all modern programming features. Furthermore a huge number of\nlibraries is available.\n\nSolidPython lets you use all these fancy python features to generate your\nconstructive solid geometry models.\n\nOn the one hand it makes the generation of your models a lot easier, because\nyou don\'t need to learn another domain specific language and you can use all\nthe programming technique you\'re already familiar with. On the other hand it\ngives you a lot more power, because you can use all the comprehensive python\nlibraries to generate your models.\n\nI would almost say this enables you to do what ever you want with ease.\nAs (maybe little uncommon) example, you could write a program that:\n\n  - looks up the mail adress of your actuall president (based on your ip address)\n  - writes a mail to him or her and asks for a portrait\n  - waits for a reply\n  - generates a heightmap from the picture you received and maps it onto a vase\n\nThis should be pretty straight forward with SolidPython but is impossible with\npure OpenSCAD.\n\nFurhtermore SolidPython 2.x.x is designed to be extendible. As such you can extend SolidPython itself using python. Actually parts of SolidPython itself are implemented as extensions (everything but the core one-to-one mapping of OpenScad to Python), these include operators, access style syntax, convenience functions, scad_interface and bosl2 support. Furthermore some of the SolidPython 1.x.x solid.utils features are also implemented as extensions (bill of material & part-hole).\n\nInstalling SolidPython\n----------------------\n\n-  Install latest release via\n   `PyPI <https://pypi.python.org/pypi/solidpython2>`__:\n\n   .. code:: bash\n\n       pip install solidpython2\n\n   (You may need to use ``sudo pip install solidpython2``, depending on\n   your environment. This is commonly discouraged though. You\'ll be happiest \n   working in a `virtual environment <https://docs.python.org/3/tutorial/venv.html>`__ \n   where you can easily control dependencies for a given project)\n\n- Install current master straight from Github:\n\n  .. code:: bash\n\n      pip install git+https://github.com/jeff-dh/SolidPython\n\nUsing SolidPython\n-----------------\n\n-  Include SolidPython at the top of your Python file:\n\n   .. code:: python\n\n       from solid2 import *\n\n   (See `this issue <https://github.com/SolidCode/SolidPython/issues/114>`__ for \n   a discussion of other import styles)\n\n-  OpenSCAD uses curly-brace blocks ({}) to create its tree. SolidPython\n   uses parentheses with comma-delimited lists. \n   \n   **OpenSCAD:**\n\n   .. code::\n\n       difference(){\n           cube(10);\n           sphere(15);\n       }\n\n   **SolidPython:**\n\n   .. code::\n\n       d = difference()(\n           cube(10),  # Note the comma between each element!\n           sphere(15)\n       )\n\n-  Call ``py_scad_obj.as_scad()`` to generate SCAD code. This returns\n   a string of valid OpenSCAD code.\n-  *or*: call ``py_scad_obj.save_as_scad("filepath.scad")`` to store\n   that code in a file.\n-  If ``filepath.scad`` is open in the OpenSCAD IDE and Design => \'Automatic\n   Reload and Compile\' is checked in the OpenSCAD IDE, running\n   ``py_scad_obj.save_as_scad()`` from Python will load the object in the\n   IDE.\n-  Alternately, you could call OpenSCAD\'s command line and render\n   straight to STL.\n\nImporting OpenSCAD code\n-----------------------\n\n- Use ``solid2.import_scad(path)`` to import OpenSCAD code. Relative paths will check the current location designated in `OpenSCAD library directories <https://en.wikibooks.org/wiki/OpenSCAD_User_Manual/Libraries>`__.\n\n**Ex:** \n\n``scadfile.scad``\n\n.. code::\n\n    module box(w,h,d){\n        cube([w,h,d]);\n    }\n\n``your_file.py``\n\n.. code:: python\n\n    from solid2 import *\n\n    scadfile = import_scad(\'/path/to/scadfile.scad\') \n    b = scadfile.box(2,4,6)\n    b.save_as_scad(\'out_file.scad\')\n\n- Recursively import OpenSCAD code by calling ``import_scad()`` with a directory argument.\n\n.. code:: python\n\n    from solid2 import *\n\n    # MCAD is OpenSCAD\'s most common utility library: https://github.com/openscad/MCAD\n    # If it\'s installed for OpenSCAD (on MacOS, at: ``$HOME/Documents/OpenSCAD/libraries``)\n    mcad = import_scad(\'MCAD\')\n\n    # MCAD contains about 15 separate packages, each included as its own namespace\n    print(dir(mcad)) # => [\'bearing\', \'bitmap\', \'boxes\', etc...]\n    mount = mcad.motors.stepper_motor_mount(nema_standard=17)\n    mount.save_as_scad(\'motor_mount_file.scad\')\n\n- OpenSCAD has the ``use()`` and ``include()`` statements for importing SCAD code, and SolidPython has them, too. They pollute the global namespace, though, and you may have better luck with ``import_scad()``,\n\n**Ex:**\n\n``scadfile.scad``\n\n.. code::\n\n    module box(w,h,d){\n        cube([w,h,d]);\n    }\n\n``your_file.py``\n\n.. code:: python\n\n    from solid2 import *\n\n    # use() puts the module `box()` into the global namespace\n    use(\'/path/to/scadfile.scad\') \n    b = box(2,4,6)\n    scad_render_to_file(b, \'out_file.scad\')\n\n\nExample Code\n------------\n\nThe best way to learn how SolidPython works is to look at the included\nexample code. If you\'ve installed SolidPython, the following line of\nPython will print (the location of) the examples directory:\n\n.. code:: python\n\n    import os, solid2; print(os.path.dirname(solid2.__file__) + \'/examples\')\n        \n\nOr browse the example code on Github\n`here <https://github.com/jeff-dh/SolidPython/tree/exp_solid/solid2/examples>`__\n\nExtra syntactic sugar\n=====================\n\nBasic operators\n---------------\n\nSolidPython overrides the basic operators + and | (union), - (difference), \\*\nand & (intersection) and ~ (debug). So\n\n.. code:: python\n\n    c = cylinder(r=10, h=5) + cylinder(r=2, h=30)\n\nis the same as:\n\n.. code:: python\n\n    c = union()(\n        cylinder(r=10, h=5),\n        cylinder(r=2, h=30)\n    )\n\nLikewise:\n\n.. code:: python\n\n    c = cylinder(r=10, h=5)\n    c -= cylinder(r=2, h=30)\n\nis the same as:\n\n.. code:: python\n\n    c = difference()(\n        cylinder(r=10, h=5),\n        cylinder(r=2, h=30)\n    )\n\nAccess Style Syntax\n-------------------\n\nSince at least some people (including me) don\'t like the OpenSCAD Syntax, SolidPython 2.x.x introduces the support for the so called "Access-Style-Syntax". This enables you to call some of the SolidPython / OpenSCAD functions as member functions of any OpenSCADObject instead of wrapping it in an instance of it.\n\nIn other words, e.g. code:\n\n.. code:: python\n\n  up(10)(cube(1))\n  #is equal to\n  cube(1).up(10)\n\nThe available member functions are the following:\n\n.. code:: python\n\n  union, difference, intersection, translate, scale, rotate, mirror, resize,\n  color, offset, hull, render, projection, surface, linear_extrude,\n  rotate_extrude, debug, background, root and disable\n\nAlso the convenience functions are available:\n\n.. code:: python\n\n  up, down, left, right, forward, fwd, back, translateX, translateY, translateZ,\n  rotateX, rotateY, rotateZ, mirrorX, mirrorY, mirrorZ, scaleX, scaleY, scaleZ,\n  resizeX, resizeY, resizeZ\n\nFurthermore you can chain these functions, because they all return the transformed OpenSCADObject, e.g.:\n\n.. code:: python\n\n  cube(1).up(10).back(20).rotate(10, 0, 5).mirror(1, 0, 0).color("green").root()\n\nConvenience functions\n---------------------\n\nSolidPython includes a number of convenience functions. Currently these\ninclude:\n\nDirections for arranging things:\n\n.. code:: python\n\n  up, down, left, right, forward, fwd, back\n\nTransformations per dimension:\n\n.. code:: python\n\n  translateX, translateY, translateZ, rotateX, rotateY, rotateZ, mirrorX,\n  mirrorY, mirrorZ, resizeX, resizeY, resizeZ, scaleX, scaleY, scaleZ\n\nFurthermore the operations `translate, scale, resize, mirror, rotate, cube and square` are overwritten in a way that they accept single integer or float values as first parameter. (`translate(1, 2, 3)` equals `translate([1, 2, 3])`)\n\n.. code:: python\n\n    cylinder().rotateY(90).up(10)\n\nseems a lot clearer to me than:\n\n.. code:: python\n\n    translate([0,0,10])(\n        rotate([0, 90, 0])(\n          cylinder()\n    ))\n\nFeatures\n========\n\nBOSL2\n-----\n\nSolidPython supports -- at least -- quite a lot of the **bosl2** library. You can use it by importing the ``solid2.extensions.bosl2``. Take a look at `bosl2 example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/07-libs-bosl2.py>`_ and `mazebox example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/16-mazebox-bosl2.py>`_ to get an idea how to use it and what\'s possible.\n\nI would suggest to use it as kind of a standard library for SolidPython.\nTake a look at their `Wiki <https://github.com/revarbat/BOSL2/wiki>`_ to get an idea about it\'s features.\n\n\nAnimation, Customizer, custom Fonts, ImplicitCad, Extensions\n------------------------------------------------------------\n\nSolidPython supports the following features\n\n* native **OpenSCAD customizer** support `customizer example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/10-customizer.py>`_ `greedy scad interface example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/17-greedy-scad-interface.py>`_\n* native **OpenSCAD animation** support `animation example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/12-animation.py>`_ and `animation example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/13-animated-bouncing-ball.py>`_\n* **custom fonts** `fonts example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/11-fonts.py>`_\n* supports **ImplicitCAD** `implicitCAD example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/14-implicitCAD.py>`_ `implicitCAD example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/15-implicitCAD2.py>`_\n* SolidPython is extendible `extensions example 1 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/08-extensions.py>`_  `extension example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/09-code-attach-extension.py>`_\n\nJupyter Renderer\n================\n\nSolidPython can be rendered inside a Jupyter Notebook using ViewScad. Unfortunately the pypi version of ``viewscad`` seems to be not compatible with ``solid2``. @jreiberkyle created `this viewscad fork <https://github.com/jreiberkyle/ViewSCAD>`__ and made it work with `solid2` (`#7 <https://github.com/jeff-dh/SolidPython/issues/7>`__)\n\nVersion 2.x.x\n=============\n\nSolidPython 2.x.x is a refactored version of SolidPython 1.x.x.\nThe refactoring process was based on the following proposal:\nhttps://github.com/SolidCode/SolidPython/issues/169\n\nThe goal was to\n\n* extract the "core" from SolidPython\n* make a solid package that only contains the fundamentals (+ a few convenience features) \n* make it extendible\n* try to get complex libraries working properly (mcad, bosl, bosl2)\n* **KISS**: ``from solid2 import *`` -> imports only ~1000 lines of source code and has (almost?) all the feautres SolidPython 1.x.x has\n* be a drop in replacement for SolidPython 1.x.x -- as far as possible, see Backwards Compatibility Section\n* get all kinds of nice features working (see Features section)\n\nThe result is a refactored and in some parts rewritten version of SolidPython we would like to release as SolidPython 2.x.x. The major improvement is a code base that should be better maintainable and extendible.\n\nBesides these benefits SolidPython 2.x.x implemented quite a few nice new features (cf. Features section).\n\nFeatures\n--------\n\nSolidPython 2.x.x has support for the following new features:\n\n* **bosl2** - SolidPython is now able to handle bosl2 pretty well (don\'t know whether everything works, but quite a lot). `bosl2 example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/07-libs-bosl2.py>`_ and `mazebox example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/16-mazebox-bosl2.py>`_\n* native **OpenSCAD customizer** support `customizer example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/10-customizer.py>`_ and `greedy scad interface example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/17-greedy-scad-interface.py>`_\n* native **OpenSCAD animation** support `animation example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/12-animation.py>`_ and `animation example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/13-animated-bouncing-ball.py>`_\n* **custom fonts** `fonts example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/11-fonts.py>`_\n* supports **ImplicitCAD** `implicitCAD example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/14-implicitCAD.py>`_ and `implicitCAD example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/15-implicitCAD2.py>`_\n\nFurthermore it has several minor improvements, like these which are based on ideas from *posts* from the SolidPython universe:\n\n* use invert operator (~) as # in OpenSCAD `#167 <https://github.com/SolidCode/SolidPython/pull/167>`_\n* convenience function including to pass sizes as integer parameters (``translate(10, 20, 30)``) `#63 <https://github.com/SolidCode/SolidPython/pull/63#issuecomment-688171416>`_\n* *access-style* syntax: ``cube(1).up(5).rotate(45, 0, 0)`` `#66 <https://github.com/SolidCode/SolidPython/pull/66>`_ This is additional! The OpenSCAD / SolidPython style syntax is still fully supported.\n\nAnother nice little feature especially to play around and debug it is that the ``__repr__`` operator of each "OpenSCADObject" now calls ``scad_render``. With this the python shell becomes pretty good in debuging and playing around with solid code and the library itself:\n\n.. code:: python\n\n  >>> from solid2 import *\n  >>> c = cube(5)\n  >>> c.up(5)\n  translate(v = [0, 0, 5]) {\n          cube(size = 5);\n  };\n  >>> c.up(5).save_as_scad()\n  \'/home/xxx/xxx/xxx/SolidPython/expsolid_out.scad\'\n  >>>\n\nBackwards compatibility\n-----------------------\n\nSolidPython 2.x.x should be a complete and mostly backwards compatible drop in\nreplacement for SolidPython 1.x.x.\nThe backwards compatibility is not 100% as depicted by the version number.\nSomethings (and even interfaces) changed. We tried to stay as backward\ncompatible as possible.  The package should behave 98% the same as SolidPython\nunless you do some "deep access" -- that\'s by 99% chance not backwards\ncompatible (like modifying OpenSCADObjects or import internal modules).\n\nAs long as you stick to:\n\n.. code:: python\n\n  from solid2 import *\n\nyou shoul be fine.\n\n**solid.utils**\n\n``solid.utils`` consisted of convenience functions and "modelling extensions" (kind of a small third party library like `mcad, bosl, bosl2`).\nThe convenience functions are now -- or the missing ones are supposed to be -- part of `solid2.extensions.convenience` and are automatically importet with the main package.\n\nConcerning the "modelling extensions" I would actually like to get rid of them as part of the SolidPython 2.x.x package. The resons are the following:\n\n* these modelling extensions (like `extrude_along_path, splines, screw_threads, part_hole,...`) don\'t align with the (core) purpose of SolidPython as I understand it (I think SolidPython is supposed to be a python "wrapper" / interface for OpenSCAD)\n* these modelling extensions are "yet another implementation" of common modelling task that need to be maintained. I would prefere a SolidPython design where these features are outsourced into a third party library\n* SolidPython 2.x.x has a pretty good **bosl2** support and bosl2 has all (?) the features provided by `solid.utils`:\n\n  * extrude_along_path: https://github.com/revarbat/BOSL2/wiki/mutators.scad#module-path_extrude\n  * First-class Negative Space (Holes): https://github.com/revarbat/BOSL2/wiki/attachments.scad#module-diff\n  * Splines / Bezier: https://github.com/revarbat/BOSL2/wiki/beziers.scad\n  * Screw threads: https://github.com/revarbat/BOSL2/wiki/screws.scad https://github.com/revarbat/BOSL2/wiki/metric_screws.scad https://github.com/revarbat/BOSL2/wiki/threading.scad\n  * distributors: https://github.com/revarbat/BOSL2/wiki/distributors.scad\n  * bouding boxes: https://github.com/revarbat/BOSL2/wiki/mutators.scad#module-bounding_box\n  * arcs, pie slices, tubes, ...: https://github.com/revarbat/BOSL2/wiki/shapes3d.scad https://github.com/revarbat/BOSL2/wiki/drawing.scad\n  * cut models in "half" / by a plane: https://github.com/revarbat/BOSL2/wiki/mutators.scad#functionmodule-half_of\n  * attachments: https://github.com/revarbat/BOSL2/wiki/attachments.scad\n\nAnd a looooot more.....\n\nI don\'t see why SolidPython should implement and maintain its own set of these features. Furthermore I assume a third party library (like `bosl2`) is probably able to provide more sophisticated implementations than we will ever be able to provide.\n\nPlease take a look at the `bosl2` implementations. I did some very basic tests in ``examples/07-libs-bosl2.py`` and -- at least -- was able to create basic examples for the core `solid.utils` features using bosl2.\n\nI would also be fine with a python third party library that implements these features, but I would like to seperate it from SolidPython itself. The reason is to achieve a SolidPython module which is independent from it (development, bugs, maintainance) with the goal to get an as solid and stable as possible SolidPython (core) package.\n\nBUT, since I assume quite a few people out there are using `solid.utils` up until now and simply getting rid of it might cause some brouhaha, my suggestion for a compromise is the `solid_legay` extension.\n\n**solid2_legacy**\n\nThe `solid2_legacy` extension is basicly everything that used to be `solid.utils`. Furhtermore it tries to "mimic" the SolidPython 1.x.x interface. This is the effort to become as backward compatible as possible. This might for example be useful when trying to get existing SolidPython 1.x.x code running.\n\nThe `solid2_legacy` extension got extracted into a seperate repo (and pip package). You should be able to just import the package if it is installed or somewhere in your import path.\n\nIf you want to use those features import the extension and take a look at it.\n\n.. code:: python\n\n  from solid2_legacy import *\n\nAnyway SolidPython 1.x.x `imports` do not work with SolidPython 2.x.x! (see Interface changes - imoprt paths have changed)\n\nI was able to get the SolidPython 1.x.x examples running just by changing the imports and they all (except for the splines example which seems to have an internal issue) worked "out of the box".\n\n\n**Interface changes**\n\n* OpenSCAD identifier escaping:\n        * all *illegal* python idetifiers are escape with a single prepending underscore\n        * special variables ``$fn -> _fn`` (*note*: ``segments`` still works)\n        * identifier starting with a digit ``module 12ptStar() -> _12ptStar()`` (*note*: ``__12ptStar`` still works)\n        * python keywords ``module import() -> _import()`` (*note*: ``import\\_``  still works)\n\n* import paths have changed (a lot)\n    * as long as you only import the root package it should be fine, otherwise probably not\n    \n    .. code:: python\n    \n            from solid2 import * #fine\n            from solid2 import objects #crash\n            from solid2 import solidpython #crash\n            from solid2 import splines #crash\n            from solid2 import utils #crash\n\n* all extensions have been moved:\n    * solid.utils has been moved to ``solid2_legacy``. If you want to use them import that extension\n    * there are some example implementations of the part / hole feature and\n      bill of materials in ``solid2_legacy``. They seem to work but are\n      not tested extensively. Take a look at ``examples/xx_legacy*``.\n    * please take a look at the bosl2 example. BOSL2 provides many features which\n      might be alternatives.\n\n* OpenSCADObject internally changed a lot\n    If you access it directly\n    (e.g. mycube.set_modifier) this might not work. But if you import\n    ``solid2_legacy`` some dummy methods will be monkey patched onto\n    OpenSCADObject so you might be able to at least run the code, but it\n    might render not correctly.\n\n* maybe some more things I can\'t remember. Some function signatures changed\n  slightly. But as long as as you stick to the regular public interface\n  everything should be fine.\n\n\nContact\n=======\n\nEnjoy!\n\nIf you have any questions or bug reports please report them to the SolidPython\n`GitHub page <https://github.com/jeff-dh/SolidPython>`__!\n\n\n\nCheers!\n\nLicense\n=======\n\nThis library is free software; you can redistribute it and/or modify it\nunder the terms of the GNU Lesser General Public License as published by\nthe Free Software Foundation; either version 2.1 of the License, or (at\nyour option) any later version.\n\nThis library is distributed in the hope that it will be useful, but\nWITHOUT ANY WARRANTY; without even the implied warranty of\nMERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\nGeneral Public License for more details.\n\n`Full text of the\nlicense <http://www.gnu.org/licenses/old-licenses/lgpl-2.1.txt>`__.\n\nSome class docstrings are derived from the `OpenSCAD User Manual\n<https://en.wikibooks.org/wiki/OpenSCAD_User_Manual>`__, so \nare available under the `Creative Commons Attribution-ShareAlike License\n<https://creativecommons.org/licenses/by-sa/3.0/>`__. \n\n',
     'author': 'jeff',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jeff-dh/SolidPython',
```

### Comparing `solidpython2-2.0.1/PKG-INFO` & `solidpython2-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidpython2
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python interface to the OpenSCAD declarative geometry language
 Home-page: https://github.com/jeff-dh/SolidPython
 License: LGPL-2.1
 Keywords: 3D,CAD,CSG,constructive solid geometry,geometry,modeling,OpenSCAD
 Author: jeff
 Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
```

