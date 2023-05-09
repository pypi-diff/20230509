# Comparing `tmp/pyopencl-2022.3.1.tar.gz` & `tmp/pyopencl-2023.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopencl-2022.3.1.tar", last modified: Tue Jan  3 22:37:15 2023, max compression
+gzip compressed data, was "pyopencl-2023.1.tar", last modified: Tue May  9 13:32:55 2023, max compression
```

## Comparing `pyopencl-2022.3.1.tar` & `pyopencl-2023.1.tar`

### file list

```diff
@@ -1,141 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 22:37:15.835850 pyopencl-2022.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-01-03 22:37:15.835850 pyopencl-2022.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/README_SETUP.txt
--rw-r--r--   0 runner    (1001) docker     (123)    31984 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/aksetup_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 22:37:15.815849 pyopencl-2022.3.1/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 22:37:15.815849 pyopencl-2022.3.1/contrib/fortran-to-opencl/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/contrib/fortran-to-opencl/README
--rw-r--r--   0 runner    (1001) docker     (123)    43661 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/contrib/fortran-to-opencl/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/contrib/pyopencl.vim
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 22:37:15.819849 pyopencl-2022.3.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/algorithm.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/array.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/howto.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/make_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    29441 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/misc.rst
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/runtime.rst
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/runtime_const.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/runtime_gl.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16401 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/runtime_memory.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/runtime_platform.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/runtime_program.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/runtime_queue.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/subst.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/doc/types.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 22:37:15.823850 pyopencl-2022.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/black-hole-accretion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/demo-struct-reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/demo_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/demo_array_svm.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/demo_elementwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/demo_elementwise_complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/demo_mandelbrot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/demo_meta_codepy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/demo_meta_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/dump-performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/dump-properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/gl_interop_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/gl_particle_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/ipython-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/median-filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32112 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/n-body.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/narray.py
--rw-r--r--   0 runner    (1001) docker     (123)    66806 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/noisyImage.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35441 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/pi-monte-carlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/svm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/examples/transpose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 22:37:15.827849 pyopencl-2022.3.1/pyopencl/
--rw-r--r--   0 runner    (1001) docker     (123)    79915 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/_cluda.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/_mymako.py
--rw-r--r--   0 runner    (1001) docker     (123)    51175 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)   108602 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/bitonic_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/bitonic_sort_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    15633 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/capture_call.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 22:37:15.827849 pyopencl-2022.3.1/pyopencl/characterize/
--rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/characterize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/characterize/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 22:37:15.827849 pyopencl-2022.3.1/pyopencl/cl/
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/cl/pyopencl-airy.cl
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/cl/pyopencl-bessel-j-complex.cl
--rw-r--r--   0 runner    (1001) docker     (123)    23274 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/cl/pyopencl-bessel-j.cl
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/cl/pyopencl-bessel-y.cl
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/cl/pyopencl-complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/cl/pyopencl-eval-tbl.cl
--rw-r--r--   0 runner    (1001) docker     (123)    31561 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/cl/pyopencl-hankel-complex.cl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 22:37:15.827849 pyopencl-2022.3.1/pyopencl/cl/pyopencl-random123/
--rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/cl/pyopencl-random123/array.h
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/cl/pyopencl-random123/openclfeatures.h
--rw-r--r--   0 runner    (1001) docker     (123)    21740 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/cl/pyopencl-random123/philox.cl
--rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/cl/pyopencl-random123/threefry.cl
--rw-r--r--   0 runner    (1001) docker     (123)    38528 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/cl/pyopencl-ranluxcl.cl
--rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/clmath.py
--rw-r--r--   0 runner    (1001) docker     (123)    25553 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/clrandom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/cltypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 22:37:15.831850 pyopencl-2022.3.1/pyopencl/compyte/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 22:37:14.000000 pyopencl-2022.3.1/pyopencl/compyte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-01-03 22:37:14.000000 pyopencl-2022.3.1/pyopencl/compyte/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     9809 2023-01-03 22:37:14.000000 pyopencl-2022.3.1/pyopencl/compyte/dtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 22:37:15.831850 pyopencl-2022.3.1/pyopencl/compyte/ndarray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 22:37:14.000000 pyopencl-2022.3.1/pyopencl/compyte/ndarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76836 2023-01-03 22:37:14.000000 pyopencl-2022.3.1/pyopencl/compyte/ndarray/gen_elemwise.py
--rw-r--r--   0 runner    (1001) docker     (123)    56332 2023-01-03 22:37:14.000000 pyopencl-2022.3.1/pyopencl/compyte/ndarray/gen_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-01-03 22:37:14.000000 pyopencl-2022.3.1/pyopencl/compyte/ndarray/setup_opencl.py
--rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-01-03 22:37:14.000000 pyopencl-2022.3.1/pyopencl/compyte/ndarray/test_gpu_elemwise.py
--rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-01-03 22:37:14.000000 pyopencl-2022.3.1/pyopencl/compyte/ndarray/test_gpu_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    38528 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/elementwise.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/invoker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/ipython_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    25547 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    65217 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    45689 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyopencl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 22:37:15.827849 pyopencl-2022.3.1/pyopencl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-01-03 22:37:15.000000 pyopencl-2022.3.1/pyopencl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-01-03 22:37:15.000000 pyopencl-2022.3.1/pyopencl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 22:37:15.000000 pyopencl-2022.3.1/pyopencl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 22:37:15.000000 pyopencl-2022.3.1/pyopencl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-01-03 22:37:15.000000 pyopencl-2022.3.1/pyopencl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-03 22:37:15.000000 pyopencl-2022.3.1/pyopencl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-01-03 22:37:15.835850 pyopencl-2022.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 22:37:15.831850 pyopencl-2022.3.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/src/bitlog.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/src/bitlog.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/src/clinfo_ext.h
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/src/mempool.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/src/pyopencl_ext.h
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/src/tools.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/src/wrap_cl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   161960 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/src/wrap_cl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/src/wrap_cl_part_1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20925 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/src/wrap_cl_part_2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    38115 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/src/wrap_constants.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/src/wrap_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    18767 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/src/wrap_mempool.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 22:37:15.835850 pyopencl-2022.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/test/add-vectors-32.spv
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/test/add-vectors-64.spv
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/test/empty-header.h
--rw-r--r--   0 runner    (1001) docker     (123)    35362 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/test/test_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    61367 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/test/test_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/test/test_arrays_in_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/test/test_clmath.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/test/test_clrandom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/test/test_enqueue_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    43703 2023-01-03 22:36:50.000000 pyopencl-2022.3.1/test/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.666548 pyopencl-2023.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-09 13:32:28.000000 pyopencl-2023.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-09 13:32:28.000000 pyopencl-2023.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-09 13:32:28.000000 pyopencl-2023.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-09 13:32:28.000000 pyopencl-2023.1/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-09 13:32:55.666548 pyopencl-2023.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-09 13:32:28.000000 pyopencl-2023.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-09 13:32:28.000000 pyopencl-2023.1/README_SETUP.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31984 2023-05-09 13:32:28.000000 pyopencl-2023.1/aksetup_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-05-09 13:32:28.000000 pyopencl-2023.1/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.642547 pyopencl-2023.1/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-09 13:32:28.000000 pyopencl-2023.1/contrib/cldis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.642547 pyopencl-2023.1/contrib/fortran-to-opencl/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-09 13:32:28.000000 pyopencl-2023.1/contrib/fortran-to-opencl/README
+-rw-r--r--   0 runner    (1001) docker     (123)    43661 2023-05-09 13:32:28.000000 pyopencl-2023.1/contrib/fortran-to-opencl/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-09 13:32:28.000000 pyopencl-2023.1/contrib/pyopencl.vim
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.646547 pyopencl-2023.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/algorithm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/array.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/howto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/make_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29441 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/runtime.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/runtime_const.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/runtime_gl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16401 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/runtime_memory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/runtime_platform.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/runtime_program.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/runtime_queue.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/subst.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-09 13:32:28.000000 pyopencl-2023.1/doc/types.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.654548 pyopencl-2023.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/black-hole-accretion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo-struct-reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo_array_svm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo_elementwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo_elementwise_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo_mandelbrot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo_meta_codepy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/demo_meta_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/dump-performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/dump-properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/gl_interop_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/gl_particle_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/ipython-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/median-filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32112 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/n-body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/narray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66806 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/noisyImage.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35441 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/pi-monte-carlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/svm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-05-09 13:32:28.000000 pyopencl-2023.1/examples/transpose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.658548 pyopencl-2023.1/pyopencl/
+-rw-r--r--   0 runner    (1001) docker     (123)    80080 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/_cluda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/_mymako.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51198 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111678 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/bitonic_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/bitonic_sort_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/capture_call.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.658548 pyopencl-2023.1/pyopencl/characterize/
+-rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/characterize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/characterize/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.658548 pyopencl-2023.1/pyopencl/cl/
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-airy.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-bessel-j-complex.cl
+-rw-r--r--   0 runner    (1001) docker     (123)    23274 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-bessel-j.cl
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-bessel-y.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-eval-tbl.cl
+-rw-r--r--   0 runner    (1001) docker     (123)    31561 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-hankel-complex.cl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.662548 pyopencl-2023.1/pyopencl/cl/pyopencl-random123/
+-rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-random123/array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-random123/openclfeatures.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21740 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-random123/philox.cl
+-rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-random123/threefry.cl
+-rw-r--r--   0 runner    (1001) docker     (123)    38528 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cl/pyopencl-ranluxcl.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/clmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25553 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/clrandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/cltypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.662548 pyopencl-2023.1/pyopencl/compyte/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9809 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/dtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.662548 pyopencl-2023.1/pyopencl/compyte/ndarray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/ndarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76836 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/ndarray/gen_elemwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56332 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/ndarray/gen_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/ndarray/setup_opencl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/ndarray/test_gpu_elemwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-05-09 13:32:54.000000 pyopencl-2023.1/pyopencl/compyte/ndarray/test_gpu_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38637 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/elementwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13721 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/invoker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/ipython_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25547 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65279 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45549 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyopencl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.658548 pyopencl-2023.1/pyopencl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-09 13:32:55.000000 pyopencl-2023.1/pyopencl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-09 13:32:55.000000 pyopencl-2023.1/pyopencl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:32:55.000000 pyopencl-2023.1/pyopencl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:32:55.000000 pyopencl-2023.1/pyopencl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-09 13:32:55.000000 pyopencl-2023.1/pyopencl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 13:32:55.000000 pyopencl-2023.1/pyopencl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-09 13:32:28.000000 pyopencl-2023.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-09 13:32:28.000000 pyopencl-2023.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-09 13:32:55.666548 pyopencl-2023.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-05-09 13:32:28.000000 pyopencl-2023.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.666548 pyopencl-2023.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/bitlog.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/bitlog.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/clinfo_ext.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/mempool.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/pyopencl_ext.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/tools.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/wrap_cl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   161960 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/wrap_cl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/wrap_cl_part_1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20925 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/wrap_cl_part_2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    38115 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/wrap_constants.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/wrap_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18767 2023-05-09 13:32:28.000000 pyopencl-2023.1/src/wrap_mempool.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:32:55.666548 pyopencl-2023.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/add-vectors-32.spv
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/add-vectors-64.spv
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/empty-header.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35358 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/test_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63301 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/test_arrays_in_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/test_clmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/test_clrandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/test_enqueue_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43703 2023-05-09 13:32:28.000000 pyopencl-2023.1/test/test_wrapper.py
```

### Comparing `pyopencl-2022.3.1/CITATION.cff` & `pyopencl-2023.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/LICENSE` & `pyopencl-2023.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/MANIFEST.in` & `pyopencl-2023.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/PKG-INFO` & `pyopencl-2023.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencl
-Version: 2022.3.1
+Version: 2023.1
 Summary: Python wrapper for OpenCL
 Home-page: http://mathema.tician.de/software/pyopencl
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
 Classifier: Environment :: Console
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyopencl-2022.3.1/README.rst` & `pyopencl-2023.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/README_SETUP.txt` & `pyopencl-2023.1/README_SETUP.txt`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/aksetup_helper.py` & `pyopencl-2023.1/aksetup_helper.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/contrib/fortran-to-opencl/README` & `pyopencl-2023.1/contrib/fortran-to-opencl/README`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/contrib/fortran-to-opencl/translate.py` & `pyopencl-2023.1/contrib/fortran-to-opencl/translate.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/contrib/pyopencl.vim` & `pyopencl-2023.1/contrib/pyopencl.vim`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/doc/Makefile` & `pyopencl-2023.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/doc/algorithm.rst` & `pyopencl-2023.1/doc/algorithm.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/doc/array.rst` & `pyopencl-2023.1/doc/array.rst`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,21 @@
 Conditionals
 ^^^^^^^^^^^^
 
 .. autofunction:: if_positive
 .. autofunction:: maximum
 .. autofunction:: minimum
 
+Logical Operations
+^^^^^^^^^^^^^^^^^^
+
+.. autofunction:: logical_and
+.. autofunction:: logical_or
+.. autofunction:: logical_not
+
 .. _reductions:
 
 Reductions
 ^^^^^^^^^^
 
 .. autofunction:: sum
 .. autofunction:: all
```

### Comparing `pyopencl-2022.3.1/doc/howto.rst` & `pyopencl-2023.1/doc/howto.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/doc/index.rst` & `pyopencl-2023.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/doc/make_constants.py` & `pyopencl-2023.1/doc/make_constants.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/doc/misc.rst` & `pyopencl-2023.1/doc/misc.rst`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 It is important to note that OpenCL is not restricted to GPUs. In fact, no special
 hardware is required to use OpenCL for computation--your existing CPU is enough.
 On Linux or macOS, type::
 
     conda install pocl
 
 to install a CPU-based OpenCL driver.
-On macOS, pocl can offer a marked robustness (and, sometimes, performance)
+On macOS, PoCL can offer a marked robustness (and, sometimes, performance)
 improvement over the OpenCL drivers built into the operating system.
 
 On Linux and Windows, you can use Intel's CPU OpenCL runtime::
 
     conda install intel-opencl-rt
 
 On Linux Intel Broadwell or newer processors with an Intel graphics card, you
@@ -159,15 +159,15 @@
     pip install pyopencl
 
 
 You can also install the following CPU based OpenCL implementation using pip
 shipped as binary wheels. Note that pyopencl has to be installed using a wheel
 for pyopencl to recognize these wheels.
 
-To install pyopencl with pocl, a CPU based implementation do::
+To install pyopencl with PoCL, a CPU based implementation do::
 
     pip install pyopencl[pocl]
 
 To install pyopencl with oclgrind, an OpenCL debugger do::
 
     pip install pyopencl[oclgrind]
 
@@ -399,15 +399,15 @@
   * complex*complex
   * real+complex
 
   *look* like they may do the right thing, but silently do the wrong thing.
 * Rewrite of the wrapper layer to be based on CFFI
 * Pypy compatibility
 * Faster kernel invocation through Python launcher code generation
-* POCL compatibility
+* PoCL compatibility
 
 Version 2015.1
 --------------
 
 * Support for new-style buffer protocol
 * Numerous fixes
```

### Comparing `pyopencl-2022.3.1/doc/runtime.rst` & `pyopencl-2023.1/doc/runtime.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/doc/runtime_const.rst` & `pyopencl-2023.1/doc/runtime_const.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/doc/runtime_gl.rst` & `pyopencl-2023.1/doc/runtime_gl.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/doc/runtime_memory.rst` & `pyopencl-2023.1/doc/runtime_memory.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/doc/runtime_platform.rst` & `pyopencl-2023.1/doc/runtime_platform.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/doc/runtime_program.rst` & `pyopencl-2023.1/doc/runtime_program.rst`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         Only available with CL 1.2.
 
         .. versionadded:: 2011.2
 
     .. attribute:: kernel_name
 
         You may use ``program.kernel_name`` to obtain a :class:`Kernel`
-        objects from a program. Note that every lookup of this type
+        object from a program. Note that every lookup of this type
         produces a new kernel object, so that this **won't** work::
 
             prg.sum.set_args(a_g, b_g, res_g)
             ev = cl.enqueue_nd_range_kernel(queue, prg.sum, a_np.shape, None)
 
         Instead, either use the (recommended, stateless) calling interface::
```

### Comparing `pyopencl-2022.3.1/doc/runtime_queue.rst` & `pyopencl-2023.1/doc/runtime_queue.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/doc/subst.rst` & `pyopencl-2023.1/doc/subst.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/doc/types.rst` & `pyopencl-2023.1/doc/types.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/black-hole-accretion.py` & `pyopencl-2023.1/examples/black-hole-accretion.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/demo-struct-reduce.py` & `pyopencl-2023.1/examples/demo-struct-reduce.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/demo.py` & `pyopencl-2023.1/examples/demo.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/demo_array.py` & `pyopencl-2023.1/examples/demo_array.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/demo_array_svm.py` & `pyopencl-2023.1/examples/demo_array_svm.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/demo_elementwise.py` & `pyopencl-2023.1/examples/demo_elementwise.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/demo_elementwise_complex.py` & `pyopencl-2023.1/examples/demo_elementwise_complex.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/demo_mandelbrot.py` & `pyopencl-2023.1/examples/demo_mandelbrot.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/demo_meta_codepy.py` & `pyopencl-2023.1/examples/demo_meta_codepy.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/demo_meta_template.py` & `pyopencl-2023.1/examples/demo_meta_template.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/dump-performance.py` & `pyopencl-2023.1/examples/dump-performance.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/dump-properties.py` & `pyopencl-2023.1/examples/dump-properties.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/gl_interop_demo.py` & `pyopencl-2023.1/examples/gl_interop_demo.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/gl_particle_animation.py` & `pyopencl-2023.1/examples/gl_particle_animation.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/ipython-demo.ipynb` & `pyopencl-2023.1/examples/ipython-demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/median-filter.py` & `pyopencl-2023.1/examples/median-filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-import pyopencl as cl
 import numpy as np
 from imageio import imread, imsave
 
+import pyopencl as cl
+
 # Read in image
 img = imread("noisyImage.jpg").astype(np.float32)
 print(img.shape)
+
 img = np.mean(img, axis=2)
 print(img.shape)
 
 ctx = cl.create_some_context()
 queue = cl.CommandQueue(ctx)
 
 mf = cl.mem_flags
@@ -89,8 +91,8 @@
 )
 # Call Kernel. Automatically takes care of block/grid distribution
 prg.medianFilter(queue, img.shape, None, img_g, result_g, width_g, height_g)
 result = np.empty_like(img)
 cl.enqueue_copy(queue, result, result_g)
 
 # Show the blurred image
-imsave("medianFilter-OpenCL.jpg", result)
+imsave("medianFilter-OpenCL.jpg", result, mode="RGB")
```

### Comparing `pyopencl-2022.3.1/examples/n-body.py` & `pyopencl-2023.1/examples/n-body.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/narray.py` & `pyopencl-2023.1/examples/narray.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/noisyImage.jpg` & `pyopencl-2023.1/examples/noisyImage.jpg`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/pi-monte-carlo.py` & `pyopencl-2023.1/examples/pi-monte-carlo.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/svm.py` & `pyopencl-2023.1/examples/svm.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/examples/transpose.py` & `pyopencl-2023.1/examples/transpose.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/__init__.py` & `pyopencl-2023.1/pyopencl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,16 +40,18 @@
 os.environ["PYOPENCL_HOME"] = os.path.dirname(os.path.abspath(__file__))
 
 try:
     import pyopencl._cl as _cl
 except ImportError:
     from os.path import dirname, join, realpath
     if realpath(join(os.getcwd(), "pyopencl")) == realpath(dirname(__file__)):
-        warn("It looks like you are importing PyOpenCL from "
-                "its source directory. This likely won't work.")
+        warn(
+            "It looks like you are importing PyOpenCL from "
+            "its source directory. This likely won't work.",
+            stacklevel=2)
     raise
 
 import numpy as np
 
 import sys
 
 _PYPY = "__pypy__" in sys.builtin_module_names
@@ -261,19 +263,19 @@
 
 class CommandQueueUsedAfterExit(UserWarning):
     pass
 
 
 def compiler_output(text):
     if int(os.environ.get("PYOPENCL_COMPILER_OUTPUT", "0")):
-        warn(text, CompilerWarning)
+        warn(text, CompilerWarning, stacklevel=3)
     else:
         warn("Non-empty compiler output encountered. Set the "
                 "environment variable PYOPENCL_COMPILER_OUTPUT=1 "
-                "to see more.", CompilerWarning)
+                "to see more.", CompilerWarning, stacklevel=3)
 
 # }}}
 
 
 # {{{ find pyopencl shipped source code
 
 def _find_pyopencl_include_path():
@@ -382,16 +384,16 @@
         platform = platform_or_context
 
     if "AMD Accelerated" in platform.name:
         _PLAT_BUILD_OPTIONS.setdefault(platform.name, []).extend(
                 ["-g", "-O0"])
         os.environ["CPU_MAX_COMPUTE_UNITS"] = "1"
     else:
-        warn("do not know how to enable debugging on '%s'"
-                % platform.name)
+        warn(f"Do not know how to enable debugging on '{platform.name}'",
+             stacklevel=2)
 
 
 class Program:
     def __init__(self, arg1, arg2=None, arg3=None):
         if arg2 is None:
             # 1-argument form: program
             self._prg = arg1
@@ -963,15 +965,16 @@
             raise Error("'shape' must be passed if 'hostbuf' is not given")
 
         if shape is None and hostbuf is not None:
             shape = hostbuf.shape
 
         if hostbuf is not None and not \
                 (flags & (mem_flags.USE_HOST_PTR | mem_flags.COPY_HOST_PTR)):
-            warn("'hostbuf' was passed, but no memory flags to make use of it.")
+            warn("'hostbuf' was passed, but no memory flags to make use of it.",
+                 stacklevel=2)
 
         if hostbuf is None and pitches is not None:
             raise Error("'pitches' may only be given if 'hostbuf' is given")
 
         if context._get_cl_version() >= (1, 2) and get_cl_header_version() >= (1, 2):
             if buffer is not None and is_array:
                 raise ValueError(
@@ -1035,16 +1038,17 @@
                 raise TypeError("'buffer' argument is not supported for CL < 1.2")
 
             image_old_init(self, context, flags, format, shape,
                     pitches, hostbuf)
 
     class _ImageInfoGetter:
         def __init__(self, event):
-            warn("Image.image.attr is deprecated and will go away in 2021. "
-                    "Use Image.attr directly, instead.")
+            warn(
+                "Image.image.attr is deprecated and will go away in 2021. "
+                "Use Image.attr directly, instead.", stacklevel=2)
 
             self.event = event
 
         def __getattr__(self, name):
             try:
                 inf_attr = getattr(_cl.image_info, name.upper())
             except AttributeError:
@@ -2167,16 +2171,18 @@
         if wait_for:
             _cl._enqueue_wait_for_events(queue, wait_for)
         return _cl._enqueue_marker(queue)
 
 
 def enqueue_fill_buffer(queue, mem, pattern, offset, size, wait_for=None):
     if not (queue._get_cl_version() >= (1, 2) and get_cl_header_version() >= (1, 2)):
-        warn("The context for this queue does not declare OpenCL 1.2 support, so "
-                "the next thing you might see is a crash")
+        warn(
+            "The context for this queue does not declare OpenCL 1.2 support, so "
+            "the next thing you might see is a crash",
+            stacklevel=2)
 
     if _PYPY and isinstance(pattern, np.generic):
         pattern = np.asarray(pattern)
 
     return _cl._enqueue_fill_buffer(queue, mem, pattern, offset, size, wait_for)
 
 # }}}
```

### Comparing `pyopencl-2022.3.1/pyopencl/_cluda.py` & `pyopencl-2023.1/pyopencl/_cluda.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/_mymako.py` & `pyopencl-2023.1/pyopencl/_mymako.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/algorithm.py` & `pyopencl-2023.1/pyopencl/algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -483,25 +483,25 @@
             boundary_mnr = known_bits + "1" + (self.bits-len(known_bits)-1)*"0"
 
             return ("((mnr < {}) ? {} : {})".format(
                 int(boundary_mnr, 2),
                 get_count_branch(known_bits+"0"),
                 get_count_branch(known_bits+"1")))
 
-        codegen_args = dict(
-                bits=self.bits,
-                key_ctype=dtype_to_ctype(self.key_dtype),
-                key_expr=key_expr,
-                index_ctype=dtype_to_ctype(self.index_dtype),
-                index_type_max=np.iinfo(self.index_dtype).max,
-                padded_bin=_padded_bin,
-                scan_ctype=scan_ctype,
-                sort_arg_names=sort_arg_names,
-                get_count_branch=get_count_branch,
-                )
+        codegen_args = {
+                "bits": self.bits,
+                "key_ctype": dtype_to_ctype(self.key_dtype),
+                "key_expr": key_expr,
+                "index_ctype": dtype_to_ctype(self.index_dtype),
+                "index_type_max": np.iinfo(self.index_dtype).max,
+                "padded_bin": _padded_bin,
+                "scan_ctype": scan_ctype,
+                "sort_arg_names": sort_arg_names,
+                "get_count_branch": get_count_branch,
+                }
 
         preamble = scan_t_cdecl+RADIX_SORT_PREAMBLE_TPL.render(**codegen_args)
         scan_preamble = preamble \
                 + RADIX_SORT_SCAN_PREAMBLE_TPL.render(**codegen_args)
 
         self.scan_kernel = scan_kernel(
                 context, scan_dtype,
```

### Comparing `pyopencl-2022.3.1/pyopencl/array.py` & `pyopencl-2023.1/pyopencl/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 
 # {{{ VecLookupWarner
 
 class VecLookupWarner:
     def __getattr__(self, name):
         warn("pyopencl.array.vec is deprecated. "
              "Please use pyopencl.cltypes for OpenCL vector and scalar types",
-             DeprecationWarning, 2)
+             DeprecationWarning, stacklevel=2)
 
         if name == "types":
             name = "vec_types"
         elif name == "type_to_scalar_and_count":
             name = "vec_type_to_scalar_and_count"
 
         return getattr(cltypes, name)
@@ -299,15 +299,15 @@
 
 
 class DefaultAllocator(cl.tools.DeferredAllocator):
     def __init__(self, *args, **kwargs):
         warn("pyopencl.array.DefaultAllocator is deprecated. "
                 "It will be continue to exist throughout the 2013.x "
                 "versions of PyOpenCL.",
-                DeprecationWarning, 2)
+                DeprecationWarning, stacklevel=2)
         cl.tools.DeferredAllocator.__init__(self, *args, **kwargs)
 
 # }}}
 
 
 # {{{ array class
 
@@ -912,15 +912,15 @@
             spelling.
         """
 
         if async_:
             warn("calling pyopencl.Array.get with 'async_=True' is deprecated. "
                     "Please use pyopencl.Array.get_async for asynchronous "
                     "device-to-host transfers",
-                    DeprecationWarning, 2)
+                    DeprecationWarning, stacklevel=2)
 
         ary, event1 = self._get(queue=queue, ary=ary, async_=async_, **kwargs)
 
         return ary
 
     def get_async(self, queue=None, ary=None, **kwargs):
         """
@@ -979,16 +979,18 @@
             return (f"<cl.{type(self).__name__} {self.shape} of {self.dtype} "
                     f"at {id(self):x} without queue, call with_queue()>")
 
         result = repr(self.get())
         if result[:5] == "array":
             result = f"cl.{type(self).__name__}" + result[5:]
         else:
-            warn(f"{type(result).__name__}.__repr__ was expected to return a "
-                     f"string starting with 'array', got '{result[:10]!r}'")
+            warn(
+                f"{type(result).__name__}.__repr__ was expected to return a "
+                f"string starting with 'array', got '{result[:10]!r}'",
+                stacklevel=2)
 
         return result
 
     def safely_stringify_for_pudb(self):
         return f"cl.{type(self).__name__} {self.dtype} {self.shape}"
 
     def __hash__(self):
@@ -2667,17 +2669,17 @@
                     cl.kernel_work_group_info.WORK_GROUP_SIZE,
                     queue.device))
 
         wait_for_this = (dest_indices.events + src_indices.events
             + builtins.sum((i.events for i in arrays[chunk_slice]), [])
             + builtins.sum((o.events for o in out[chunk_slice]), []))
         evt = knl(queue, gs, ls,
-                *([o for o in out[chunk_slice]]
+                *(list(out[chunk_slice])
                     + [dest_indices, src_indices]
-                    + [i for i in arrays[chunk_slice]]
+                    + list(arrays[chunk_slice])
                     + src_offsets_list[chunk_slice]
                     + [src_indices.size]), wait_for=wait_for_this)
         for o in out[chunk_slice]:
             o.add_event(evt)
 
     return out
 
@@ -2745,17 +2747,17 @@
                     queue.device))
 
         wait_for_this = (wait_for
             + builtins.sum([i.events for i in arrays[chunk_slice]], [])
             + builtins.sum([o.events for o in out[chunk_slice]], []))
         evt = knl(queue, gs, ls,
                 *(
-                    [o for o in out[chunk_slice]]
+                    list(out[chunk_slice])
                     + [dest_indices]
-                    + [i for i in arrays[chunk_slice]]
+                    + list(arrays[chunk_slice])
                     + [use_fill_cla, array_lengths_cla, dest_indices.size]),
                 wait_for=wait_for_this)
 
         for o in out[chunk_slice]:
             o.add_event(evt)
 
     return out
@@ -3125,14 +3127,110 @@
     out.add_event(_minimum_maximum_backend(out,  a, b, queue=queue, minmax="min"))
 
     return out
 
 # }}}
 
 
+# {{{ logical ops
+
+def _logical_op(x1, x2, out, operator, queue=None):
+    # NOTE: Copied from pycuda.gpuarray
+    assert operator in ["&&", "||"]
+
+    if np.isscalar(x1) and np.isscalar(x2):
+        if out is None:
+            out = empty(queue, shape=(), dtype=np.int8)
+
+        if operator == "&&":
+            out[:] = np.logical_and(x1, x2)
+        else:
+            out[:] = np.logical_or(x1, x2)
+    elif np.isscalar(x1) or np.isscalar(x2):
+        scalar_arg, = [x for x in (x1, x2) if np.isscalar(x)]
+        ary_arg, = [x for x in (x1, x2) if not np.isscalar(x)]
+        queue = queue or ary_arg.queue
+        allocator = ary_arg.allocator
+
+        if not isinstance(ary_arg, Array):
+            raise ValueError("logical_and can take either scalar or Array"
+                             " as inputs")
+
+        out = out or ary_arg._new_like_me(dtype=np.int8)
+
+        assert out.shape == ary_arg.shape and out.dtype == np.int8
+
+        knl = elementwise.get_array_scalar_binop_kernel(
+            queue.context,
+            operator,
+            out.dtype,
+            ary_arg.dtype,
+            np.dtype(type(scalar_arg))
+        )
+        elwise_kernel_runner(lambda *args, **kwargs: knl)(out, ary_arg, scalar_arg)
+    else:
+        if not (isinstance(x1, Array) and isinstance(x2, Array)):
+            raise ValueError("logical_or/logical_and can take either scalar"
+                             " or Arrays as inputs")
+        if x1.shape != x2.shape:
+            raise NotImplementedError("Broadcasting not supported")
+
+        queue = queue or x1.queue or x2.queue
+        allocator = x1.allocator or x2.allocator
+
+        if out is None:
+            out = empty(queue, allocator=allocator,
+                        shape=x1.shape, dtype=np.int8)
+
+        assert out.shape == x1.shape and out.dtype == np.int8
+
+        knl = elementwise.get_array_binop_kernel(
+            queue.context,
+            operator,
+            out.dtype,
+            x1.dtype, x2.dtype)
+        elwise_kernel_runner(lambda *args, **kwargs: knl)(out, x1, x2)
+
+    return out
+
+
+def logical_and(x1, x2, /, out=None, queue=None):
+    """
+    Returns the element-wise logical AND of *x1* and *x2*.
+    """
+    return _logical_op(x1, x2, out, "&&", queue=queue)
+
+
+def logical_or(x1, x2, /, out=None, queue=None):
+    """
+    Returns the element-wise logical OR of *x1* and *x2*.
+    """
+    return _logical_op(x1, x2, out, "||", queue=queue)
+
+
+def logical_not(x, /, out=None, queue=None):
+    """
+    Returns the element-wise logical NOT of *x*.
+    """
+    if np.isscalar(x):
+        out = out or empty(queue, shape=(), dtype=np.int8)
+        out[:] = np.logical_not(x)
+    else:
+        queue = queue or x.queue
+        out = out or empty(queue, shape=x.shape, dtype=np.int8,
+                           allocator=x.allocator)
+        knl = elementwise.get_logical_not_kernel(queue.context,
+                                                 x.dtype)
+        elwise_kernel_runner(lambda *args, **kwargs: knl)(out, x)
+
+    return out
+
+# }}}
+
+
 # {{{ reductions
 
 def sum(a, dtype=None, queue=None, slice=None, initial=np._NoValue):
     """
     .. versionadded:: 2011.1
     """
     if initial is not np._NoValue and not isinstance(initial, SCALAR_CLASSES):
```

### Comparing `pyopencl-2022.3.1/pyopencl/bitonic_sort.py` & `pyopencl-2023.1/pyopencl/bitonic_sort.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/bitonic_sort_templates.py` & `pyopencl-2023.1/pyopencl/bitonic_sort_templates.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/cache.py` & `pyopencl-2023.1/pyopencl/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,16 +107,17 @@
                 from time import sleep
                 sleep(wait_time_seconds)
 
                 attempts += 1
 
                 if attempts % warn_attempts == 0:
                     from warnings import warn
-                    warn("could not obtain cache lock--delete '%s' if necessary"
-                            % self.lock_file)
+                    warn(
+                        f"Could not obtain cache lock--delete '{self.lock_file}' "
+                        "if necessary", stacklevel=2)
 
                 if attempts > exit_attempts:
                     raise RuntimeError("waited more than one minute "
                             "on the lock file '%s'"
                             "--something is wrong" % self.lock_file)
 
             cleanup_m.register(self)
@@ -205,15 +206,15 @@
                     break  # stop searching the include path
 
             if not found:
                 pass
 
     _inner(src)
 
-    result = list((name,) + vals for name, vals in result.items())
+    result = [(name,) + vals for name, vals in result.items()]
     result.sort()
 
     return result
 
 
 def get_file_md5sum(fname):
     checksum = new_hash()
@@ -296,16 +297,17 @@
                         raise _InvalidInfoFile()
                 finally:
                     info_file.close()
 
             except _InvalidInfoFile:
                 mod_cache_dir_m.reset()
                 from warnings import warn
-                warn("PyOpenCL encountered an invalid info file for cache key %s"
-                        % cache_key)
+                warn(
+                    "PyOpenCL encountered an invalid info file for "
+                    f"cache key '{cache_key}'", stacklevel=2)
                 return None
 
             # }}}
 
             # {{{ load binary
 
             binary_file = open(binary_path, "rb")
@@ -509,17 +511,18 @@
         # build from source instead, otherwise report the failure.
         if build_program_failure and not was_cached:
             raise
 
         if not build_program_failure:
             from warnings import warn
             from traceback import format_exc
-            warn("PyOpenCL compiler caching failed with an exception:\n"
-                    "[begin exception]\n%s[end exception]"
-                    % format_exc())
+            warn(
+                "PyOpenCL compiler caching failed with an exception:\n"
+                f"[begin exception]\n{format_exc()}[end exception]",
+                stacklevel=2)
 
         prg = _cl._Program(ctx, src)
         was_cached = False
         already_built = False
 
     if not already_built:
         prg.build(options_bytes, devices)
```

### Comparing `pyopencl-2022.3.1/pyopencl/capture_call.py` & `pyopencl-2023.1/pyopencl/capture_call.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/characterize/__init__.py` & `pyopencl-2023.1/pyopencl/characterize/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,33 +108,33 @@
 
     if nv_compute_cap is not None:
         if nv_compute_cap < (2, 0):
             return 16
         else:
             if nv_compute_cap >= (3, 0):
                 from warnings import warn
-                warn("wildly guessing conflicting local access size on '%s'"
-                        % dev,
-                        CLCharacterizationWarning)
+                warn(
+                    f"Wildly guessing conflicting local access size on '{dev}'",
+                    CLCharacterizationWarning, stacklevel=2)
 
             return 32
 
     if dev.type & cl.device_type.GPU:
         from warnings import warn
-        warn("wildly guessing conflicting local access size on '%s'"
-                % dev,
-                CLCharacterizationWarning)
+        warn(
+            f"Wildly guessing conflicting local access size on '{dev}'",
+            CLCharacterizationWarning, stacklevel=2)
         return 16
     elif dev.type & cl.device_type.CPU:
         return 1
     else:
         from warnings import warn
-        warn("wildly guessing conflicting local access size on '%s'"
-                % dev,
-                CLCharacterizationWarning)
+        warn(
+            f"Wildly guessing conflicting local access size on '{dev}'",
+            CLCharacterizationWarning, stacklevel=2)
         return 16
 
 
 def local_memory_access_granularity(dev):
     """Return the number of bytes per bank in local memory."""
     return 4
 
@@ -146,35 +146,35 @@
 
     if nv_compute_cap is not None:
         if nv_compute_cap < (2, 0):
             return 16
         else:
             if nv_compute_cap >= (3, 0):
                 from warnings import warn
-                warn("wildly guessing local memory bank count on '%s'"
-                        % dev,
-                        CLCharacterizationWarning)
+                warn(
+                    f"Wildly guessing local memory bank count on '{dev}'",
+                    CLCharacterizationWarning, stacklevel=2)
 
             return 32
 
     if dev.type & cl.device_type.GPU:
         from warnings import warn
-        warn("wildly guessing local memory bank count on '%s'"
-                % dev,
-                CLCharacterizationWarning)
+        warn(
+            f"Wildly guessing local memory bank count on '{dev}'",
+            CLCharacterizationWarning, stacklevel=2)
         return 16
     elif dev.type & cl.device_type.CPU:
         if dev.local_mem_type == cl.device_local_mem_type.GLOBAL:
             raise RuntimeError("asking for a bank count is "
                     "meaningless for cache-based lmem")
 
     from warnings import warn
-    warn("wildly guessing conflicting local access size on '%s'"
-            % dev,
-            CLCharacterizationWarning)
+    warn(
+        f"Wildly guessing conflicting local access size on '{dev}'",
+        CLCharacterizationWarning, stacklevel=2)
     return 16
 
 
 def why_not_local_access_conflict_free(dev, itemsize,
         array_shape, array_stored_shape=None):
     """
     :param itemsize: size of accessed data in bytes
@@ -194,17 +194,17 @@
 
     array_shape = array_shape[::-1]
     array_stored_shape = array_stored_shape[::-1]
 
     gran = local_memory_access_granularity(dev)
     if itemsize != gran:
         from warnings import warn
-        warn("local conflict info might be inaccurate "
-                "for itemsize != %d" % gran,
-                CLCharacterizationWarning)
+        warn(
+            f"Local conflict info might be inaccurate for itemsize != {gran}",
+            CLCharacterizationWarning, stacklevel=2)
 
     sim_wi = simultaneous_work_items_on_local_access(dev)
     bank_count = local_memory_bank_count(dev)
 
     conflicts = []
 
     for work_item_axis in range(rank):
@@ -328,17 +328,17 @@
 
     import re
     version = platform.version
     ver_match = re.match(
             r"^OpenCL [0-9.]+ [Pp]o[Cc][Ll] ([0-9]+)\.([0-9]+)", version)
 
     if ver_match is None:
-        msg = f"pocl version number did not have expected format: '{version}'"
         from warnings import warn
-        warn(msg)
+        warn(f"PoCL version number did not have expected format: '{version}'",
+             stacklevel=2)
         return fallback_value
     else:
         return (int(ver_match.group(1)), int(ver_match.group(2)))
 
 
 _CHECK_FOR_POCL_ARG_COUNT_BUG_CACHE: Dict[cl.Device, bool] = {}
```

### Comparing `pyopencl-2022.3.1/pyopencl/characterize/performance.py` & `pyopencl-2023.1/pyopencl/characterize/performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,14 @@
 
     rates = []
     num_dips = 0
 
     while True:
         elapsed = _get_time(queue, f, timer_factory=timer_factory)
         rate = global_size/elapsed
-        print(global_size, rate, num_dips)
 
         keep_trying = not rates
 
         if rates and rate > 1.05*max(rates):  # big improvement
             keep_trying = True
             num_dips = 0
 
@@ -227,11 +226,11 @@
                 val += val; val += val; val += val; val += val; val += val;
 
                 val += val; val += val; val += val; val += val; val += val;
                 val += val; val += val; val += val; val += val; val += val;
             }
             tgt[get_local_id(0)] = val;
         }
-        """ % dict(op_t=type), ())
+        """ % {"op_t": type}, ())
 
 
 # vim: foldmethod=marker:filetype=pyopencl
```

### Comparing `pyopencl-2022.3.1/pyopencl/cl/pyopencl-airy.cl` & `pyopencl-2023.1/pyopencl/cl/pyopencl-airy.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/cl/pyopencl-bessel-j-complex.cl` & `pyopencl-2023.1/pyopencl/cl/pyopencl-bessel-j-complex.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/cl/pyopencl-bessel-j.cl` & `pyopencl-2023.1/pyopencl/cl/pyopencl-bessel-j.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/cl/pyopencl-bessel-y.cl` & `pyopencl-2023.1/pyopencl/cl/pyopencl-bessel-y.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/cl/pyopencl-complex.h` & `pyopencl-2023.1/pyopencl/cl/pyopencl-complex.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/cl/pyopencl-eval-tbl.cl` & `pyopencl-2023.1/pyopencl/cl/pyopencl-eval-tbl.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/cl/pyopencl-hankel-complex.cl` & `pyopencl-2023.1/pyopencl/cl/pyopencl-hankel-complex.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/cl/pyopencl-random123/array.h` & `pyopencl-2023.1/pyopencl/cl/pyopencl-random123/array.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/cl/pyopencl-random123/openclfeatures.h` & `pyopencl-2023.1/pyopencl/cl/pyopencl-random123/openclfeatures.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/cl/pyopencl-random123/philox.cl` & `pyopencl-2023.1/pyopencl/cl/pyopencl-random123/philox.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/cl/pyopencl-random123/threefry.cl` & `pyopencl-2023.1/pyopencl/cl/pyopencl-random123/threefry.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/cl/pyopencl-ranluxcl.cl` & `pyopencl-2023.1/pyopencl/cl/pyopencl-ranluxcl.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/clmath.py` & `pyopencl-2023.1/pyopencl/clmath.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/clrandom.py` & `pyopencl-2023.1/pyopencl/clrandom.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/cltypes.py` & `pyopencl-2023.1/pyopencl/cltypes.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 """
 
 import numpy as np
 from pyopencl.tools import get_or_register_dtype
 import warnings
 
 if __file__.endswith("array.py"):
-    warnings.warn("pyopencl.array.vec is deprecated. Please use pyopencl.cltypes")
+    warnings.warn(
+        "pyopencl.array.vec is deprecated. Please use pyopencl.cltypes.",
+        stacklevel=2)
 
 """
 This file provides a type mapping from OpenCl type names to their numpy equivalents
 """
 
 char = np.int8
 uchar = np.uint8
@@ -73,18 +75,18 @@
             while len(names) < padded_count:
                 names.append("padding%d" % (len(names) - count))
 
             if len(titles) < len(names):
                 titles.extend((len(names) - len(titles)) * [None])
 
             try:
-                dtype = np.dtype(dict(
-                    names=names,
-                    formats=[base_type] * padded_count,
-                    titles=titles))
+                dtype = np.dtype({
+                    "names": names,
+                    "formats": [base_type] * padded_count,
+                    "titles": titles})
             except NotImplementedError:
                 try:
                     dtype = np.dtype([((n, title), base_type)
                                       for (n, title) in zip(names, titles)])
                 except TypeError:
                     dtype = np.dtype([(n, base_type) for (n, title)
                                       in zip(names, titles)])
@@ -94,27 +96,30 @@
             set_global(name, dtype)
 
             def create_array(dtype, count, padded_count, *args, **kwargs):
                 if len(args) < count:
                     from warnings import warn
                     warn("default values for make_xxx are deprecated;"
                          " instead specify all parameters or use"
-                         " cltypes.zeros_xxx", DeprecationWarning)
+                         " cltypes.zeros_xxx",
+                         DeprecationWarning, stacklevel=4)
+
                 padded_args = tuple(list(args) + [0] * (padded_count - len(args)))
                 array = eval("array(padded_args, dtype=dtype)",
-                             dict(array=np.array, padded_args=padded_args,
-                                  dtype=dtype))
+                             {"array": np.array,
+                              "padded_args": padded_args,
+                              "dtype": dtype})
                 for key, val in list(kwargs.items()):
                     array[key] = val
                 return array
 
             set_global("make_" + name, eval(
                 "lambda *args, **kwargs: create_array(dtype, %i, %i, "
                 "*args, **kwargs)" % (count, padded_count),
-                dict(create_array=create_array, dtype=dtype)))
+                {"create_array": create_array, "dtype": dtype}))
             set_global("filled_" + name, eval(
                 "lambda val: make_%s(*[val]*%i)" % (name, count)))
             set_global("zeros_" + name, eval("lambda: filled_%s(0)" % (name)))
             set_global("ones_" + name, eval("lambda: filled_%s(1)" % (name)))
 
             vec_types[np.dtype(base_type), count] = dtype
             vec_type_to_scalar_and_count[dtype] = np.dtype(base_type), count
```

### Comparing `pyopencl-2022.3.1/pyopencl/compyte/array.py` & `pyopencl-2023.1/pyopencl/compyte/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,21 +188,19 @@
             if strides is not None and shape is not None \
                     and product(shape) == product(x.shape) \
                     and x.flags.forc:
                 # Workaround: If we're being asked to do what amounts to a
                 # contiguous reshape, at least do that.
 
                 if strides == f_contiguous_strides(x.dtype.itemsize, shape):
-                    # **dict is a workaround for Python 2.5 syntax.
-                    result = x.reshape(-1).reshape(*shape, **dict(order="F"))
+                    result = x.reshape(-1).reshape(*shape, order="F")
                     assert result.strides == strides
                     return result
                 elif strides == c_contiguous_strides(x.dtype.itemsize, shape):
-                    # **dict is a workaround for Python 2.5 syntax.
-                    result = x.reshape(-1).reshape(*shape, **dict(order="C"))
+                    result = x.reshape(-1).reshape(*shape, order="C")
                     assert result.strides == strides
                     return result
 
             raise NotImplementedError(
                     "as_strided won't work on non-builtin arrays for now. "
                     "See https://github.com/numpy/numpy/issues/2466")
```

### Comparing `pyopencl-2022.3.1/pyopencl/compyte/dtypes.py` & `pyopencl-2023.1/pyopencl/compyte/dtypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 def fill_registry_with_c_types(reg, respect_windows, include_bool=True):
     from sys import platform
     import struct
 
     if include_bool:
         # bool is of unspecified size in the OpenCL spec and may in fact be
         # 4-byte.
-        reg.get_or_register_dtype("bool", np.bool8)
+        reg.get_or_register_dtype("bool", np.bool_)
 
     reg.get_or_register_dtype(["signed char", "char"], np.int8)
     reg.get_or_register_dtype("unsigned char", np.uint8)
     reg.get_or_register_dtype(["short", "signed short",
         "signed short int", "short signed int"], np.int16)
     reg.get_or_register_dtype(["unsigned short",
         "unsigned short int", "short unsigned int"], np.uint16)
@@ -177,15 +177,15 @@
     reg.get_or_register_dtype(["uintptr_t"], np.uintp)
 
     reg.get_or_register_dtype("float", np.float32)
     reg.get_or_register_dtype("double", np.float64)
 
 
 def fill_registry_with_c99_stdint_types(reg):
-    reg.get_or_register_dtype("bool", np.bool8)
+    reg.get_or_register_dtype("bool", np.bool_)
 
     reg.get_or_register_dtype("int8_t", np.int8)
     reg.get_or_register_dtype("uint8_t", np.uint8)
     reg.get_or_register_dtype("int16_t", np.int16)
     reg.get_or_register_dtype("uint16_t", np.uint16)
     reg.get_or_register_dtype("int32_t", np.int32)
     reg.get_or_register_dtype("uint32_t", np.uint32)
```

### Comparing `pyopencl-2022.3.1/pyopencl/compyte/ndarray/gen_elemwise.py` & `pyopencl-2023.1/pyopencl/compyte/ndarray/gen_elemwise.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/compyte/ndarray/gen_reduction.py` & `pyopencl-2023.1/pyopencl/compyte/ndarray/gen_reduction.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/compyte/ndarray/setup_opencl.py` & `pyopencl-2023.1/pyopencl/compyte/ndarray/setup_opencl.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/compyte/ndarray/test_gpu_elemwise.py` & `pyopencl-2023.1/pyopencl/compyte/ndarray/test_gpu_elemwise.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/compyte/ndarray/test_gpu_ndarray.py` & `pyopencl-2023.1/pyopencl/compyte/ndarray/test_gpu_ndarray.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/elementwise.py` & `pyopencl-2023.1/pyopencl/elementwise.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,38 +86,31 @@
     if return_match is not None:
         from warnings import warn
         warn("Using a 'return' statement in an element-wise operation will "
                 "likely lead to incorrect results. Use "
                 "PYOPENCL_ELWISE_CONTINUE instead.",
                 stacklevel=3)
 
-    source = ("""//CL//
+    source = (f"""//CL//
         {preamble}
 
         #define PYOPENCL_ELWISE_CONTINUE continue
 
-        __kernel void {name}({arguments})
+        __kernel void {name}({", ".join(arg.declarator() for arg in arguments)})
         {{
           int lid = get_local_id(0);
           int gsize = get_global_size(0);
           int work_group_start = get_local_size(0)*get_group_id(0);
           long i;
 
           {loop_prep};
-          {body}
+          {body % {"operation": operation}}
           {after_loop};
         }}
-        """.format(
-            arguments=", ".join(arg.declarator() for arg in arguments),
-            name=name,
-            preamble=preamble,
-            loop_prep=loop_prep,
-            after_loop=after_loop,
-            body=body % dict(operation=operation),
-            ))
+        """)
 
     return cl.Program(context, source).build(options)
 
 
 def get_elwise_kernel_and_types(
         context: cl.Context,
         arguments: Union[str, List[DtypedArgument]],
@@ -252,15 +245,15 @@
             if isinstance(arg, VectorArg) and not arg.with_offset:
                 from warnings import warn
                 warn(
                         f"ElementwiseKernel '{self.name}' used with VectorArgs "
                         "that do not have offset support enabled. This usage is "
                         "deprecated. Just pass with_offset=True to VectorArg, "
                         "everything should sort itself out automatically.",
-                        DeprecationWarning)
+                        DeprecationWarning, stacklevel=2)
 
         if not any(isinstance(arg, VectorArg) for arg in arg_descrs):
             raise RuntimeError(
                 "ElementwiseKernel can only be used with functions that have "
                 "at least one vector argument")
 
         return knl, arg_descrs
@@ -1154,10 +1147,20 @@
             VectorArg(then_else_dtype, "result", with_offset=True),
             VectorArg(crit_dtype, "crit", with_offset=True),
             then_arg, else_arg,
             ],
             f"result[i] = crit[i] > 0 ? {then_} : {else_}",
             name="if_positive")
 
+
+@context_dependent_memoize
+def get_logical_not_kernel(context, in_dtype):
+    return get_elwise_kernel(context, [
+        VectorArg(np.int8, "z", with_offset=True),
+        VectorArg(in_dtype, "y", with_offset=True),
+        ],
+        "z[i] = (y[i] == 0)",
+        name="logical_not_kernel")
+
 # }}}
 
 # vim: fdm=marker
```

### Comparing `pyopencl-2022.3.1/pyopencl/invoker.py` & `pyopencl-2023.1/pyopencl/invoker.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,16 +150,16 @@
             cl_arg_idx += 1
 
         elif arg_dtype.kind == "c":
             if warn_about_arg_count_bug:
                 warn("{knl_name}: arguments include complex numbers, and "
                         "some (but not all) of the target devices mishandle "
                         "struct kernel arguments (hence the workaround is "
-                        "disabled".format(
-                            knl_name=function_name), stacklevel=2)
+                        "disabled".format(knl_name=function_name),
+                        stacklevel=2)
 
             if arg_dtype == np.complex64:
                 arg_char = "f"
             elif arg_dtype == np.complex128:
                 arg_char = "d"
             else:
                 raise TypeError("unexpected complex type: %s" % arg_dtype)
@@ -305,21 +305,21 @@
                 name=f"<pyopencl invoker for '{function_name}'>"),
             enqueue_name)
 
 
 # {{{ Helper functions related to argument sizes and device limits
 
 def _get_max_parameter_size(dev):
-    """Return the device's maximum parameter size adjusted for pocl."""
+    """Return the device's maximum parameter size adjusted for PoCL."""
     from pyopencl.characterize import get_pocl_version
 
     dev_limit = dev.max_parameter_size
     pocl_version = get_pocl_version(dev.platform, fallback_value=(1, 8))
     if pocl_version is not None and pocl_version < (3, 0):
-        # Current pocl versions (as of 04/2022) have an incorrect parameter
+        # Current PoCL versions (as of 04/2022) have an incorrect parameter
         # size limit of 1024; see e.g. https://github.com/pocl/pocl/pull/1046
         if dev_limit == 1024:
             if dev.type & cl.device_type.CPU:
                 return 1024*1024
             if dev.type & cl.device_type.GPU:
                 # All modern Nvidia GPUs (starting from Compute Capability 2)
                 # have this limit
@@ -354,23 +354,25 @@
             total_arg_size = dev_ptr_size * num_cl_args
 
         if total_arg_size > dev_limit:
             from warnings import warn
             warn(f"Kernel '{function_name}' has {num_cl_args} arguments with "
                 f"a total size of {total_arg_size} bytes, which is higher than "
                 f"the limit of {dev_limit} bytes on {dev}. This might "
-                "lead to compilation errors, especially on GPU devices.")
+                "lead to compilation errors, especially on GPU devices.",
+                stacklevel=3)
         elif is_estimate and total_arg_size >= dev_limit * 0.75:
             # Since total_arg_size is just an estimate, also warn in case we are
             # just below the actual limit.
             from warnings import warn
             warn(f"Kernel '{function_name}' has {num_cl_args} arguments with "
                 f"a total size of {total_arg_size} bytes, which approaches "
                 f"the limit of {dev_limit} bytes on {dev}. This might "
-                "lead to compilation errors, especially on GPU devices.")
+                "lead to compilation errors, especially on GPU devices.",
+                stacklevel=3)
 
 # }}}
 
 
 invoker_cache = WriteOncePersistentDict(
         "pyopencl-invoker-cache-v41",
         key_builder=_NumpyTypesKeyBuilder())
```

### Comparing `pyopencl-2022.3.1/pyopencl/ipython_ext.py` & `pyopencl-2023.1/pyopencl/ipython_ext.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/reduction.py` & `pyopencl-2023.1/pyopencl/reduction.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/pyopencl/scan.py` & `pyopencl-2023.1/pyopencl/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -861,15 +861,16 @@
         else:
             leftovers.add(word)
             return word
 
     s = re.sub(r"\b([a-zA-Z0-9_]+)\b", replace_id, s)
     if leftovers:
         from warnings import warn
-        warn("leftover words in identifier prefixing: " + " ".join(leftovers))
+        warn("Leftover words in identifier prefixing: " + " ".join(leftovers),
+             stacklevel=3)
 
     return mako.template.Template(s, strict_undefined=True)     # type: ignore
 
 
 @dataclass(frozen=True)
 class _GeneratedScanKernelInfo:
     scan_src: str
@@ -1081,30 +1082,30 @@
 
         self.name_prefix = name_prefix
 
         # {{{ set up shared code dict
 
         from pyopencl.characterize import has_double_support
 
-        self.code_variables = dict(
-            np=np,
-            dtype_to_ctype=dtype_to_ctype,
-            preamble=preamble,
-            name_prefix=name_prefix,
-            index_dtype=self.index_dtype,
-            scan_dtype=dtype,
-            is_segmented=self.is_segmented,
-            arg_dtypes=arg_dtypes,
-            arg_ctypes=arg_ctypes,
-            scan_expr=_process_code_for_macro(scan_expr),
-            neutral=_process_code_for_macro(neutral),
-            is_gpu=bool(self.devices[0].type & cl.device_type.GPU),
-            double_support=all(
+        self.code_variables = {
+            "np": np,
+            "dtype_to_ctype": dtype_to_ctype,
+            "preamble": preamble,
+            "name_prefix": name_prefix,
+            "index_dtype": self.index_dtype,
+            "scan_dtype": dtype,
+            "is_segmented": self.is_segmented,
+            "arg_dtypes": arg_dtypes,
+            "arg_ctypes": arg_ctypes,
+            "scan_expr": _process_code_for_macro(scan_expr),
+            "neutral": _process_code_for_macro(neutral),
+            "is_gpu": bool(self.devices[0].type & cl.device_type.GPU),
+            "double_support": all(
                 has_double_support(dev) for dev in devices),
-            )
+            }
 
         index_typename = dtype_to_ctype(self.index_dtype)
         scan_typename = dtype_to_ctype(dtype)
 
         # This key is meant to uniquely identify the non-device parameters for
         # the scan kernel.
         self.kernel_key = (
```

### Comparing `pyopencl-2022.3.1/pyopencl/tools.py` & `pyopencl-2023.1/pyopencl/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -659,17 +659,17 @@
     arg_names = []
     for arg in supported_arg_names:
         if arg not in metafunc.fixturenames:
             continue
 
         if arg == "ctx_getter":
             from warnings import warn
-            warn("The 'ctx_getter' arg is deprecated in "
-                    "favor of 'ctx_factory'.",
-                    DeprecationWarning)
+            warn(
+                "The 'ctx_getter' arg is deprecated in favor of 'ctx_factory'.",
+                DeprecationWarning, stacklevel=2)
 
         arg_names.append(arg)
 
     return arg_names
 
 
 def get_pyopencl_fixture_arg_values():
@@ -899,17 +899,17 @@
     result = []
 
     for arg_type in arg_types:
         if isinstance(arg_type, VectorArg) and arg_type.with_offset:
             result.append("__global %(type)s *%(name)s = "
                     "(__global %(type)s *) "
                     "((__global char *) %(name)s__base + %(name)s__offset);"
-                    % dict(
-                        type=dtype_to_ctype(arg_type.dtype),
-                        name=arg_type.name))
+                    % {
+                        "type": dtype_to_ctype(arg_type.dtype),
+                        "name": arg_type.name})
 
     return "\n".join(result)
 
 # }}}
 
 
 def get_gl_sharing_context_properties():
@@ -1093,34 +1093,30 @@
 
     pre_decls = cdl.get_declarations()
 
     offset_code = "\n".join(
             "result[%d] = pycl_offsetof(%s, %s);" % (i+1, name, field_name)
             for i, (field_name, _) in enumerate(fields))
 
-    src = r"""
+    src = rf"""
         #define pycl_offsetof(st, m) \
                  ((uint) ((__local char *) &(dummy.m) \
                  - (__local char *)&dummy ))
 
-        %(pre_decls)s
+        {pre_decls}
 
-        %(my_decl)s
+        {c_decl}
 
         __kernel void get_size_and_offsets(__global uint *result)
-        {
-            result[0] = sizeof(%(my_type)s);
-            __local %(my_type)s dummy;
-            %(offset_code)s
-        }
-    """ % dict(
-            pre_decls=pre_decls,
-            my_decl=c_decl,
-            my_type=name,
-            offset_code=offset_code)
+        {{
+            result[0] = sizeof({name});
+            __local {name} dummy;
+            {offset_code}
+        }}
+    """
 
     if context is None:
         context = cl.Context([device])
 
     queue = cl.CommandQueue(context)
 
     prg = cl.Program(context, src)
```

### Comparing `pyopencl-2022.3.1/pyopencl.egg-info/PKG-INFO` & `pyopencl-2023.1/pyopencl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencl
-Version: 2022.3.1
+Version: 2023.1
 Summary: Python wrapper for OpenCL
 Home-page: http://mathema.tician.de/software/pyopencl
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
 Classifier: Environment :: Console
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyopencl-2022.3.1/pyopencl.egg-info/SOURCES.txt` & `pyopencl-2023.1/pyopencl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 README_SETUP.txt
 aksetup_helper.py
 configure.py
 pyproject.toml
 pytest.ini
 setup.cfg
 setup.py
+contrib/cldis.py
 contrib/pyopencl.vim
 contrib/fortran-to-opencl/README
 contrib/fortran-to-opencl/translate.py
 doc/Makefile
 doc/algorithm.rst
 doc/array.rst
 doc/conf.py
```

### Comparing `pyopencl-2022.3.1/pyproject.toml` & `pyopencl-2023.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/setup.cfg` & `pyopencl-2023.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/setup.py` & `pyopencl-2023.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/src/bitlog.cpp` & `pyopencl-2023.1/src/bitlog.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/src/bitlog.hpp` & `pyopencl-2023.1/src/bitlog.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/src/clinfo_ext.h` & `pyopencl-2023.1/src/clinfo_ext.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/src/mempool.hpp` & `pyopencl-2023.1/src/mempool.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/src/pyopencl_ext.h` & `pyopencl-2023.1/src/pyopencl_ext.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/src/tools.hpp` & `pyopencl-2023.1/src/tools.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/src/wrap_cl.cpp` & `pyopencl-2023.1/src/wrap_cl.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/src/wrap_cl.hpp` & `pyopencl-2023.1/src/wrap_cl.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/src/wrap_cl_part_1.cpp` & `pyopencl-2023.1/src/wrap_cl_part_1.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/src/wrap_cl_part_2.cpp` & `pyopencl-2023.1/src/wrap_cl_part_2.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/src/wrap_constants.cpp` & `pyopencl-2023.1/src/wrap_constants.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/src/wrap_helpers.hpp` & `pyopencl-2023.1/src/wrap_helpers.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/src/wrap_mempool.cpp` & `pyopencl-2023.1/src/wrap_mempool.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/test/add-vectors-32.spv` & `pyopencl-2023.1/test/add-vectors-32.spv`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/test/add-vectors-64.spv` & `pyopencl-2023.1/test/add-vectors-64.spv`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/test/test_algorithm.py` & `pyopencl-2023.1/test/test_algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1028,15 +1028,15 @@
     from pyopencl.algorithm import KeyValueSorter
     kvs = KeyValueSorter(context)
     starts, lists, evt = kvs(queue, keys, values, nkeys, starts_dtype=np.int32)
 
     starts = starts.get()
     lists = lists.get()
 
-    mydict = dict()
+    mydict = {}
     for k, v in zip(keys.get(), values.get()):
         mydict.setdefault(k, []).append(v)
 
     for i in range(nkeys):
         start, end = starts[i:i+2]
         assert sorted(mydict[i]) == sorted(lists[start:end])
 
@@ -1063,15 +1063,15 @@
     dev = ctx.devices[0]
     if (dev.platform.name == "Apple" and dev.type & cl.device_type.CPU):
         pytest.xfail("Bitonic sort won't work on Apple CPU: no workgroup "
             "parallelism")
     if (dev.platform.name == "Portable Computing Language"
             and dtype == np.float64
             and get_pocl_version(dev.platform) < (1, 0)):
-        pytest.xfail("Double precision bitonic sort doesn't work on POCL < 1.0")
+        pytest.xfail("Double precision bitonic sort doesn't work on PoCL < 1.0")
 
     if dtype == np.float64 and not has_double_support(dev):
         from pytest import skip
         skip("double precision not supported on %s" % dev)
     # Requires https://github.com/intel/llvm/releases/tag/2022-WW50 or newer to pass
     # on Intel CL.
 
@@ -1113,30 +1113,30 @@
 
     ctx = cl.create_some_context()
     queue = cl.CommandQueue(ctx)
 
     device = queue.device
     if device.platform.vendor == "The pocl project" \
             and device.type & cl.device_type.GPU:
-        pytest.xfail("bitonic argsort fails on POCL + Nvidia,"
-                "at least the K40, as of pocl 1.6, 2021-01-20")
+        pytest.xfail("bitonic argsort fails on PoCL + Nvidia,"
+                "at least the K40, as of PoCL 1.6, 2021-01-20")
     # Requires https://github.com/intel/llvm/releases/tag/2022-WW50 or newer to pass
     # on Intel CL.
 
     dev = ctx.devices[0]
     if (dev.platform.name == "Portable Computing Language"
             and sys.platform == "darwin"):
-        pytest.xfail("Bitonic sort crashes on Apple POCL")
+        pytest.xfail("Bitonic sort crashes on Apple PoCL")
     if (dev.platform.name == "Apple" and dev.type & cl.device_type.CPU):
         pytest.xfail("Bitonic sort won't work on Apple CPU: no workgroup "
             "parallelism")
     if (dev.platform.name == "Portable Computing Language"
             and dtype == np.float64
             and get_pocl_version(dev.platform) < (1, 0)):
-        pytest.xfail("Double precision bitonic sort doesn't work on POCL < 1.0")
+        pytest.xfail("Double precision bitonic sort doesn't work on PoCL < 1.0")
     if (dev.platform.name == "Intel(R) OpenCL" and size == 0):
         pytest.xfail("size-0 arange fails on Intel CL")
 
     if dtype == np.float64 and not has_double_support(dev):
         from pytest import skip
         skip("double precision not supported on %s" % dev)
 
@@ -1145,15 +1145,15 @@
 
     index = cl.array.arange(queue, 0, size, 1, dtype=np.int32)
     m = clrandom.rand(queue, (size,), dtype, luxury=None, a=0, b=239432234)
 
     sorterm = BitonicSort(ctx)
 
     ms = m.copy()
-    # enqueue_marker crashes under CL 1.1 pocl if there is anything to wait for
+    # enqueue_marker crashes under CL 1.1 PoCL if there is anything to wait for
     # (no clEnqueueWaitForEvents) https://github.com/inducer/pyopencl/pull/237
     if (dev.platform.name == "Portable Computing Language"
             and cl.get_cl_header_version() < (1, 2)):
         ms.finish()
         index.finish()
     ms, evt = sorterm(ms, idx=index, axis=0)
```

### Comparing `pyopencl-2022.3.1/test/test_array.py` & `pyopencl-2023.1/test/test_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -834,16 +834,16 @@
     context = ctx_factory()
     queue = cl.CommandQueue(context)
 
     device = queue.device
     if device.platform.vendor == "The pocl project" \
             and device.type & cl.device_type.GPU \
             and rng_class is RanluxGenerator:
-        pytest.xfail("ranlux test fails on POCL + Nvidia,"
-                "at least the Titan V, as of pocl 1.6, 2021-01-20")
+        pytest.xfail("ranlux test fails on PoCL + Nvidia,"
+                "at least the Titan V, as of PoCL 1.6, 2021-01-20")
 
     if device.platform.vendor == "Intel(R) Corporation" \
             and rng_class is RanluxGenerator:
         pytest.xfail("compiling ranlux kernel causes a segfault on "
                 "Intel CPU runtime as of 2022-02-13")
 
     if has_double_support(context.devices[0]):
@@ -901,16 +901,16 @@
 def test_random_int_in_range(ctx_factory, rng_class, dtype, plot_hist=False):
     context = ctx_factory()
     queue = cl.CommandQueue(context)
 
     if queue.device.platform.vendor == "The pocl project" \
             and queue.device.type & cl.device_type.GPU \
             and rng_class is RanluxGenerator:
-        pytest.xfail("ranlux test fails on POCL + Nvidia,"
-                "at least the Titan V, as of pocl 1.6, 2021-01-20")
+        pytest.xfail("ranlux test fails on PoCL + Nvidia,"
+                "at least the Titan V, as of PoCL 1.6, 2021-01-20")
 
     if rng_class is RanluxGenerator:
         gen = rng_class(queue, 5120)
     else:
         gen = rng_class(context)
 
     # if (dtype == np.int64
@@ -1635,16 +1635,16 @@
 def test_get_async(ctx_factory):
     context = ctx_factory()
     queue = cl.CommandQueue(context)
 
     device = queue.device
     if device.platform.vendor == "The pocl project" \
             and device.type & cl.device_type.GPU:
-        pytest.xfail("the async get test fails on POCL + Nvidia,"
-                "at least the K40, as of pocl 1.6, 2021-01-20")
+        pytest.xfail("the async get test fails on PoCL + Nvidia,"
+                "at least the K40, as of PoCL 1.6, 2021-01-20")
 
     rng = np.random.default_rng(seed=42)
     a = rng.random(10**6, dtype=np.float32)
     a_gpu = cl_array.to_device(queue, a)
     b = a + a**5 + 1
     b_gpu = a_gpu + a_gpu**5 + 1
 
@@ -2292,14 +2292,68 @@
 
         # safe to let this proceed to deallocation, since we're not
         # operating on the memory
 
 # }}}
 
 
+def test_logical_and_or(ctx_factory):
+    # NOTE: Copied over from pycuda/test/test_gpuarray.py
+    rng = np.random.default_rng(seed=0)
+    ctx = ctx_factory()
+    cq = cl.CommandQueue(ctx)
+
+    for op in ["logical_and", "logical_or"]:
+        x_np = rng.random((10, 4))
+        y_np = rng.random((10, 4))
+        zeros_np = np.zeros((10, 4))
+        ones_np = np.ones((10, 4))
+
+        x_cl = cl_array.to_device(cq, x_np)
+        y_cl = cl_array.to_device(cq, y_np)
+        zeros_cl = cl_array.zeros(cq, (10, 4), np.float64)
+        ones_cl = cl_array.zeros(cq, (10, 4), np.float64) + 1
+
+        np.testing.assert_array_equal(
+            getattr(cl_array, op)(x_cl, y_cl).get(),
+            getattr(np, op)(x_np, y_np))
+        np.testing.assert_array_equal(
+            getattr(cl_array, op)(x_cl, ones_cl).get(),
+            getattr(np, op)(x_np, ones_np))
+        np.testing.assert_array_equal(
+            getattr(cl_array, op)(x_cl, zeros_cl).get(),
+            getattr(np, op)(x_np, zeros_np))
+        np.testing.assert_array_equal(
+            getattr(cl_array, op)(x_cl, 1.0).get(),
+            getattr(np, op)(x_np, ones_np))
+        np.testing.assert_array_equal(
+            getattr(cl_array, op)(x_cl, 0.0).get(),
+            getattr(np, op)(x_np, 0.0))
+
+
+def test_logical_not(ctx_factory):
+    # NOTE: Copied over from pycuda/test/test_gpuarray.py
+    ctx = ctx_factory()
+    cq = cl.CommandQueue(ctx)
+
+    rng = np.random.default_rng(seed=0)
+    x_np = rng.random((10, 4))
+    x_cl = cl_array.to_device(cq, x_np)
+
+    np.testing.assert_array_equal(
+        cl_array.logical_not(x_cl).get(),
+        np.logical_not(x_np))
+    np.testing.assert_array_equal(
+        cl_array.logical_not(cl_array.zeros(cq, 10, np.float64)).get(),
+        np.logical_not(np.zeros(10)))
+    np.testing.assert_array_equal(
+        cl_array.logical_not((cl_array.zeros(cq, 10, np.float64) + 1)).get(),
+        np.logical_not(np.ones(10)))
+
+
 if __name__ == "__main__":
     if len(sys.argv) > 1:
         exec(sys.argv[1])
     else:
         from pytest import main
         main([__file__])
```

### Comparing `pyopencl-2022.3.1/test/test_arrays_in_structs.py` & `pyopencl-2023.1/test/test_arrays_in_structs.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2022.3.1/test/test_clmath.py` & `pyopencl-2023.1/test/test_clmath.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,20 +160,16 @@
     queue = cl.CommandQueue(context)
 
     for s in sizes:
         a = cl_array.arange(queue, s, dtype=np.float32)/10
         a2 = cl_array.arange(queue, s, dtype=np.float32)/45.2 + 0.1
         b = clmath.fmod(a, a2)
 
-        a = a.get()
-        a2 = a2.get()
-        b = b.get()
-
-        for i in range(s):
-            assert math.fmod(a[i], a2[i]) == b[i]
+        # https://salsa.debian.org/opencl-team/python-pyopencl/-/merge_requests/3#note_383761
+        assert np.max(np.abs((np.fmod(a.get(), a2.get()) - b.get()))) < 1e-4
 
 
 def test_ldexp(ctx_factory):
     context = ctx_factory()
     queue = cl.CommandQueue(context)
 
     for s in sizes:
```

### Comparing `pyopencl-2022.3.1/test/test_clrandom.py` & `pyopencl-2023.1/test/test_clrandom.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
     size = 10
 
     with cl.CommandQueue(cl_ctx) as queue:
         device = queue.device
         if device.platform.vendor == "The pocl project" \
                 and device.type & cl.device_type.GPU \
                 and rng_class is make_ranlux_generator:
-            pytest.xfail("ranlux test fails on POCL + Nvidia,"
-                    "at least the K40, as of pocl 1.6, 2021-01-20")
+            pytest.xfail("ranlux test fails on PoCL + Nvidia,"
+                    "at least the K40, as of PoCL 1.6, 2021-01-20")
 
         rng.uniform(queue, size, dtype)
 
         if dtype not in (np.int32, np.int64):
             rng.normal(queue, size, dtype)
```

### Comparing `pyopencl-2022.3.1/test/test_enqueue_copy.py` & `pyopencl-2023.1/test/test_enqueue_copy.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,21 +42,21 @@
     ctx = ctx_factory()
     queue = cl.CommandQueue(ctx)
 
     if (honor_skip
             and ctx.devices[0].platform.name == "Portable Computing Language"
             and get_pocl_version(ctx.devices[0].platform) <= (0, 13)):
         # https://github.com/pocl/pocl/issues/353
-        pytest.skip("POCL's rectangular copies crash")
+        pytest.skip("PoCL's rectangular copies crash")
 
     device = queue.device
     if device.platform.vendor == "The pocl project" \
             and device.type & cl.device_type.GPU:
-        pytest.xfail("rect copies fail on POCL + Nvidia,"
-                "at least the K40, as of pocl 1.6, 2021-01-20")
+        pytest.xfail("rect copies fail on PoCL + Nvidia,"
+                "at least the K40, as of PoCL 1.6, 2021-01-20")
 
     if honor_skip and queue.device.platform.name == "Apple":
         pytest.xfail("Apple's CL implementation crashes on this.")
 
     ary_in_shp = 256, 128  # Entire array shape from which sub-array copied to device
     sub_ary_shp = 128, 96  # Sub-array shape to be copied to device
     ary_in_origin = 20, 13  # Sub-array origin
@@ -131,21 +131,21 @@
     ctx = ctx_factory()
     queue = cl.CommandQueue(ctx)
 
     if (honor_skip
             and ctx.devices[0].platform.name == "Portable Computing Language"
             and get_pocl_version(ctx.devices[0].platform) <= (0, 13)):
         # https://github.com/pocl/pocl/issues/353
-        pytest.skip("POCL's rectangular copies crash")
+        pytest.skip("PoCL's rectangular copies crash")
 
     device = queue.device
     if device.platform.vendor == "The pocl project" \
             and device.type & cl.device_type.GPU:
-        pytest.xfail("rect copies fail on POCL + Nvidia,"
-                "at least the K40, as of pocl 1.6, 2021-01-20")
+        pytest.xfail("rect copies fail on PoCL + Nvidia,"
+                "at least the K40, as of PoCL 1.6, 2021-01-20")
 
     if honor_skip and queue.device.platform.name == "Apple":
         pytest.skip("Apple's CL implementation crashes on this.")
 
     ary_in_shp = 256, 128, 31  # array shape from which sub-array copied to device
     sub_ary_shp = 128, 96, 20  # Sub-array shape to be copied to device
     ary_in_origin = 20, 13, 7  # Sub-array origin
```

### Comparing `pyopencl-2022.3.1/test/test_wrapper.py` & `pyopencl-2023.1/test/test_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,25 +30,25 @@
 import pyopencl.clrandom
 from pyopencl.tools import (  # noqa: F401
         pytest_generate_tests_for_pyopencl as pytest_generate_tests,
         ImmediateAllocator, DeferredAllocator)
 from pyopencl.characterize import get_pocl_version
 
 
-def _xfail_if_pocl(plat, up_to_version, msg="unsupported by pocl"):
+def _xfail_if_pocl(plat, up_to_version, msg="unsupported by PoCL"):
     if plat.vendor == "The pocl project":
         if up_to_version is None or get_pocl_version(plat) <= up_to_version:
             pytest.xfail(msg)
 
 
 def _xfail_if_pocl_gpu(device, what):
     if device.platform.vendor == "The pocl project" \
             and device.type & cl.device_type.GPU:
-        pytest.xfail(f"POCL's {what} support don't work right on Nvidia GPUs, "
-                "at least the Titan V, as of pocl 1.6, 2021-01-20")
+        pytest.xfail(f"PoCL's {what} support don't work right on Nvidia GPUs, "
+                "at least the Titan V, as of PoCL 1.6, 2021-01-20")
 
 
 # {{{ test_get_info
 
 def test_get_info(ctx_factory):
     ctx = ctx_factory()
     device, = ctx.devices
@@ -406,15 +406,15 @@
     if not device.image_support:
         from pytest import skip
         skip("images not supported on %s" % device)
 
     if "Intel" in device.vendor and "31360.31426" in device.version:
         from pytest import skip
         skip("images crashy on %s" % device)
-    _xfail_if_pocl(device.platform, None, "pocl does not support CL_ADDRESS_CLAMP")
+    _xfail_if_pocl(device.platform, None, "PoCL does not support CL_ADDRESS_CLAMP")
 
     prg = cl.Program(context, """
         __kernel void copy_image(
           __global float *dest,
           __read_only image2d_t src,
           sampler_t samp,
           int stride0)
@@ -484,15 +484,15 @@
     if not device.image_support:
         from pytest import skip
         skip("images not supported on %s" % device)
 
     if device.platform.vendor == "Intel(R) Corporation":
         from pytest import skip
         skip("images crashy on %s" % device)
-    _xfail_if_pocl(device.platform, None, "pocl does not support CL_ADDRESS_CLAMP")
+    _xfail_if_pocl(device.platform, None, "PoCL does not support CL_ADDRESS_CLAMP")
 
     prg = cl.Program(context, """
         __kernel void copy_image_plane(
           __global float2 *dest,
           __read_only image3d_t src,
           sampler_t samp,
           int stride0,
@@ -750,17 +750,17 @@
 # }}}
 
 
 # {{{ test_enqueue_barrier_marker
 
 def test_enqueue_barrier_marker(ctx_factory):
     ctx = ctx_factory()
-    # Still relevant on pocl 1.0RC1.
+    # Still relevant on PoCL 1.0RC1.
     _xfail_if_pocl(
-            ctx.devices[0].platform, (1, 0), "pocl crashes on enqueue_barrier")
+            ctx.devices[0].platform, (1, 0), "PoCL crashes on enqueue_barrier")
 
     queue = cl.CommandQueue(ctx)
 
     if queue._get_cl_version() >= (1, 2) and cl.get_cl_header_version() <= (1, 1):
         pytest.skip("CL impl version >= 1.2, header version <= 1.1--cannot be sure "
                 "that clEnqueueWaitForEvents is implemented")
 
@@ -787,15 +787,15 @@
 # {{{ test_unload_compiler
 
 def test_unload_compiler(platform):
     if (platform._get_cl_version() < (1, 2)
             or cl.get_cl_header_version() < (1, 2)):
         from pytest import skip
         skip("clUnloadPlatformCompiler is only available in OpenCL 1.2")
-    _xfail_if_pocl(platform, (0, 13), "pocl does not support unloading compiler")
+    _xfail_if_pocl(platform, (0, 13), "PoCL does not support unloading compiler")
     if platform.vendor == "Intel(R) Corporation":
         from pytest import skip
         skip("Intel proprietary driver does not support unloading compiler")
     cl.unload_platform_compiler(platform)
 
 # }}}
 
@@ -837,15 +837,15 @@
     if (ctx._get_cl_version() < (1, 1)
             and cl.get_cl_header_version() < (1, 1)):
         from pytest import skip
         skip("UserEvent is only available in OpenCL 1.1")
 
     # https://github.com/pocl/pocl/issues/201
     _xfail_if_pocl(ctx.devices[0].platform, (0, 13),
-            "pocl's user events don't work right")
+            "PoCL's user events don't work right")
 
     status = {}
 
     def event_waiter1(e, key):
         e.wait()
         status[key] = True
 
@@ -1134,15 +1134,15 @@
         pytest.xfail("AMD CPU doesn't do coarse-grain SVM")
     if ("AMD" in dev.platform.name
             and dev.type & cl.device_type.GPU):
         pytest.xfail("AMD GPU crashes on SVM unmap")
     if (dev.platform.vendor == "The pocl project"
             and dev.type & cl.device_type.GPU
             and "k40" in dev.name.lower()):
-        pytest.xfail("Crashes on K40s via POCL-CUDA")
+        pytest.xfail("Crashes on K40s via PoCL-CUDA")
 
     dtype = np.dtype(np.float32)
     n = 3000
     if use_opaque_style:
         svm_ary = cl.SVMAllocation(ctx, n*dtype.itemsize, alignment=64,
                                    flags=cl.svm_mem_flags.READ_WRITE)
     else:
```

