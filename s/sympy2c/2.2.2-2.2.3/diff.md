# Comparing `tmp/sympy2c-2.2.2.tar.gz` & `tmp/sympy2c-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sympy2c-2.2.2.tar", last modified: Mon Dec 19 13:37:32 2022, max compression
+gzip compressed data, was "sympy2c-2.2.3.tar", last modified: Tue May  9 18:46:39 2023, max compression
```

## Comparing `sympy2c-2.2.2.tar` & `sympy2c-2.2.3.tar`

### file list

```diff
@@ -1,405 +1,419 @@
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-12-19 13:37:32.977119 sympy2c-2.2.2/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      452 2022-08-16 09:56:27.000000 sympy2c-2.2.2/AUTHORS.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      741 2022-08-16 09:56:27.000000 sympy2c-2.2.2/CONTRIBUTING.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9800 2022-12-19 13:15:17.000000 sympy2c-2.2.2/HISTORY.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      758 2022-08-16 09:56:27.000000 sympy2c-2.2.2/LICENSE.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10696 2022-12-19 13:37:32.977236 sympy2c-2.2.2/PKG-INFO
--rw-r--r--   0 uweschmitt   (501) staff       (20)       87 2022-10-25 11:20:39.000000 sympy2c-2.2.2/README.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      733 2022-12-13 12:59:39.000000 sympy2c-2.2.2/pyproject.toml
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1210 2022-12-19 13:37:32.977665 sympy2c-2.2.2/setup.cfg
--rw-r--r--   0 uweschmitt   (501) staff       (20)      293 2022-12-07 15:40:45.000000 sympy2c-2.2.2/setup.py
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-12-19 13:37:32.882146 sympy2c-2.2.2/src/
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-12-19 13:37:32.887555 sympy2c-2.2.2/src/sympy2c/
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2098 2022-12-16 15:27:28.000000 sympy2c-2.2.2/src/sympy2c/__init__.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1487 2022-12-07 15:42:34.000000 sympy2c-2.2.2/src/sympy2c/build_f2c.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2957 2022-12-16 13:38:02.000000 sympy2c-2.2.2/src/sympy2c/build_gsl.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1840 2022-11-22 12:52:11.000000 sympy2c-2.2.2/src/sympy2c/build_lsoda.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2592 2022-12-16 15:30:23.000000 sympy2c-2.2.2/src/sympy2c/build_lsoda_fast.py
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-12-19 13:37:32.888723 sympy2c-2.2.2/src/sympy2c/c_code/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      872 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/c_code/__init__.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    89712 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/c_code/lsoda.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    13137 2022-12-19 09:30:27.000000 sympy2c-2.2.2/src/sympy2c/compiler.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3031 2022-10-18 09:16:57.000000 sympy2c-2.2.2/src/sympy2c/create_curry_class.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2154 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/expressions.py
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-12-19 13:37:32.927852 sympy2c-2.2.2/src/sympy2c/f2c_files/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      304 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/abort_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      194 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/arith.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1328 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/backspac.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      272 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/c_abs.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      354 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/c_cos.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      936 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/c_div.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      349 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/c_exp.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      384 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/c_log.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      350 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/c_sin.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      605 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/c_sqrt.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      494 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/cabs.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1393 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/close.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)       44 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/ctype.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      218 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_abs.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_acos.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_asin.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_atan.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      271 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_atn2.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      255 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_cnjg.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      241 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_cos.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_cosh.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      232 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_dim.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      241 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_exp.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      201 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_imag.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      269 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_int.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      291 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_lg10.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      241 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_log.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      688 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_mod.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      281 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_nint.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      207 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_prod.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      266 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_sign.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      241 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_sin.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_sinh.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_sqrt.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      241 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_tan.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/d_tanh.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      239 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/derf_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      253 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/derfc_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2624 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/dfe.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      471 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/dolio.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      972 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/dtime_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1624 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/due.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      521 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/ef1asc_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      427 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/ef1cmc_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2838 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/endfile.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      270 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/erf_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      275 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/erfc_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6442 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/err.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      839 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/etime_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      543 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/exit_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4688 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/f2c.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1139 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/f2c_ctype.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)      684 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/f77_aloc.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4933 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/f77vers.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2939 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/fio.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8566 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/fmt.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2006 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/fmt.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)      865 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/fmtlib.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      665 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/fp.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)      917 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/ftell64_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      900 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/ftell_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      592 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/getarg_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1223 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/getenv_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      218 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/h_abs.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      230 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/h_dim.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      294 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/h_dnnt.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      442 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/h_indx.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      205 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/h_len.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      207 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/h_mod.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      281 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/h_nint.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      266 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/h_sign.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      346 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/hl_ge.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      345 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/hl_gt.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      346 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/hl_le.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      345 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/hl_lt.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    18128 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/i77vers.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      214 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/i_abs.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      225 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/i_dim.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      291 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/i_dnnt.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      430 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/i_indx.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      203 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/i_len.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      211 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/i_mod.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      278 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/i_nint.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      260 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/i_sign.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      196 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/iargc_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2639 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/iio.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1125 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/ilnw.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2732 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/inquire.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      334 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/l_ge.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      333 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/l_gt.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      334 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/l_le.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      333 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/l_lt.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1097 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/lbitbits.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      258 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/lbitshft.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1564 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/lio.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)    14743 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/lread.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4616 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/lwrite.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2249 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/main.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     5701 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/open.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      412 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/pow_ci.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      276 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/pow_dd.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      448 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/pow_di.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      489 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/pow_hh.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      488 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/pow_ii.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      516 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/pow_qq.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      436 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/pow_ri.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      851 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/pow_zi.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      549 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/pow_zz.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1151 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/qbitbits.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      258 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/qbitshft.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      206 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_abs.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      233 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_acos.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      233 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_asin.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      233 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_atan.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      253 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_atn2.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      235 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_cnjg.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      229 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_cos.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      233 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_cosh.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      214 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_dim.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      229 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_exp.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      189 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_imag.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      257 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_int.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      279 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_lg10.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      229 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_log.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      678 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_mod.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      269 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_nint.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      248 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_sign.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      229 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_sin.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      233 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_sinh.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      233 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_sqrt.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      229 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_tan.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      233 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/r_tanh.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      718 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/rawio.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8929 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/rdfmt.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      475 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/rewind.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1492 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/rsfe.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1785 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/rsli.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    11585 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/rsne.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1458 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/s_cat.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      722 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/s_cmp.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1024 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/s_copy.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1617 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/s_paus.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      759 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/s_rnge.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      762 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/s_stop.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      828 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/sfe.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      689 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/sig_die.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      842 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/signal1.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)      299 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/signal_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      330 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/signbit.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1865 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/sue.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1252 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/sysdep1.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)      652 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/system_.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      386 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/typesize.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1619 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/uio.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     7584 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/uninit.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      972 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/util.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4751 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/wref.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     7506 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/wrtfmt.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1280 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/wsfe.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      697 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/wsle.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      479 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/wsne.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1174 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/xwsne.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      268 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/z_abs.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      363 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/z_cos.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      913 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/z_div.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      357 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/z_exp.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2729 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/z_log.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      359 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/z_sin.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      581 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/f2c_files/z_sqrt.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    22285 2022-12-13 15:34:22.000000 sympy2c-2.2.2/src/sympy2c/function.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4024 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/globals.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6039 2022-12-16 14:02:42.000000 sympy2c-2.2.2/src/sympy2c/integral.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9886 2022-10-18 09:16:57.000000 sympy2c-2.2.2/src/sympy2c/interpolation.py
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-12-19 13:37:32.976890 sympy2c-2.2.2/src/sympy2c/lsoda_modified/
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2014 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/blkdta000.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1251 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/blkdta000.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2185 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/bnorm.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1187 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/bnorm.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     5331 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/cfode.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4252 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/cfode.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)      961 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/d1mach.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4040 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dasum.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2960 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dasum.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4500 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/daxpy.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3493 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/daxpy.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2176 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dcabs1.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1397 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dcabs1.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4294 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dcopy.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3283 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dcopy.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4409 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ddot.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3411 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ddot.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12081 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dgbmv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10532 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dgbmv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12789 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dgemm.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    11119 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dgemm.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9805 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dgemv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8763 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dgemv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6778 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dger.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     5693 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dger.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3991 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dnrm2.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3073 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dnrm2.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4258 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/drot.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3168 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/drot.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3364 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/drotg.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2288 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/drotg.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6291 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/drotm.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     5268 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/drotm.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6604 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/drotmg.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6360 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/drotmg.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12244 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsbmv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    11151 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsbmv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4026 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dscal.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2996 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dscal.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     5466 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsdot.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4203 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsdot.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9921 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dspmv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9466 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dspmv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     7981 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dspr.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     7298 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dspr.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9153 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dspr2.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8614 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dspr2.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4416 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dswap.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3461 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dswap.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12961 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsymm.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    11181 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsymm.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10228 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsymv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9397 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsymv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8248 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsyr.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     7269 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsyr.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9503 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsyr2.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8594 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsyr2.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    13968 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsyr2k.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12494 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsyr2k.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12148 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsyrk.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10798 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsyrk.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    13612 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtbmv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12567 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtbmv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    13711 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtbsv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12651 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtbsv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10626 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtpmv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10659 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtpmv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10721 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtpsv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10741 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtpsv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    13967 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtrmm.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12807 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtrmm.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10696 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtrmv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10128 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtrmv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    14773 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtrsm.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    13788 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtrsm.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10679 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtrsv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10124 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtrsv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3629 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dzasum.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2619 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dzasum.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4341 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dznrm2.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3380 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/dznrm2.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2087 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ewset.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1088 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ewset.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4688 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/f2c.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3671 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/icamax.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2780 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/icamax.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3720 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/idamax.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2787 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/idamax.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     5025 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/intdy.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3190 2022-12-16 15:22:07.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/intdy.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3670 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/isamax.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2732 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/isamax.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3700 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/izamax.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2804 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/izamax.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3897 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/lsame.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3137 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/lsame.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    97145 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/lsoda.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    79164 2022-12-16 15:22:08.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/lsoda.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10818 2022-12-16 15:22:10.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/prja.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     7857 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/prja.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4036 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sasum.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2933 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sasum.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4423 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/saxpy.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3407 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/saxpy.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2120 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/scabs1.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1346 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/scabs1.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3804 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/scasum.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2609 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/scasum.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4308 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/scnrm2.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3323 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/scnrm2.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4246 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/scopy.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3235 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/scopy.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4337 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sdot.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3327 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sdot.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8649 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sdsdot.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     7144 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sdsdot.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    11967 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sgbmv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10398 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sgbmv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12682 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sgemm.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10985 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sgemm.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9693 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sgemv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8629 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sgemv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6676 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sger.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     5572 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sger.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3945 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/snrm2.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2990 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/snrm2.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4622 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/solsy.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3243 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/solsy.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3214 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/srcma.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1834 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/srcma.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4151 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/srot.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3055 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/srot.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3265 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/srotg.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2173 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/srotg.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6218 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/srotm.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     5206 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/srotm.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6441 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/srotmg.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6214 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/srotmg.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12134 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssbmv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    11017 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssbmv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3964 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sscal.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2924 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sscal.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9811 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sspmv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9332 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sspmv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     7901 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sspr.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     7189 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sspr.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9057 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sspr2.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8493 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sspr2.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4362 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sswap.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3401 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/sswap.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12847 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssymm.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    11047 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssymm.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10118 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssymv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9263 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssymv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8166 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssyr.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     7160 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssyr.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9409 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssyr2.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8473 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssyr2.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    13883 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssyr2k.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12360 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssyr2k.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12063 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssyrk.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10676 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssyrk.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    13562 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/stbmv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12495 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/stbmv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    13661 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/stbsv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12579 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/stbsv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    35457 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/stoda.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    27916 2022-11-03 15:17:14.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/stoda.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10576 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/stpmv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10587 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/stpmv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10671 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/stpsv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10669 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/stpsv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    13891 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/strmm.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12697 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/strmm.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10646 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/strmv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10056 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/strmv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    14706 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/strsm.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    13679 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/strsm.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10743 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/strsv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10137 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/strsv.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1505 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/vmnorm.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      688 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/vmnorm.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3709 2022-12-16 15:22:11.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/xerbla.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2319 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/xerbla.f
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8039 2022-11-17 13:00:43.000000 sympy2c-2.2.2/src/sympy2c/lsoda_modified/xerrwv.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)    35609 2022-12-07 15:41:03.000000 sympy2c-2.2.2/src/sympy2c/lu_generator.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    41096 2022-12-16 15:31:56.000000 sympy2c-2.2.2/src/sympy2c/module.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10796 2022-12-16 15:30:23.000000 sympy2c-2.2.2/src/sympy2c/ode.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4759 2022-12-07 16:38:28.000000 sympy2c-2.2.2/src/sympy2c/ode_combined.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4695 2022-12-19 09:21:01.000000 sympy2c-2.2.2/src/sympy2c/ode_combined_cython_template.pyx
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8056 2022-12-16 15:30:23.000000 sympy2c-2.2.2/src/sympy2c/ode_fast.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     7031 2022-12-07 16:39:26.000000 sympy2c-2.2.2/src/sympy2c/ode_fast_cython_template.pyx
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2160 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/python_function.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2380 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/rec_inv.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1339 2022-08-16 09:56:27.000000 sympy2c-2.2.2/src/sympy2c/speedup.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2901 2022-10-18 09:16:57.000000 sympy2c-2.2.2/src/sympy2c/symbol.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3954 2022-12-16 15:30:23.000000 sympy2c-2.2.2/src/sympy2c/utils.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     5927 2022-10-18 09:16:57.000000 sympy2c-2.2.2/src/sympy2c/vector.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9379 2022-09-15 12:26:27.000000 sympy2c-2.2.2/src/sympy2c/visitor.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1179 2022-12-16 13:19:28.000000 sympy2c-2.2.2/src/sympy2c/wrapper.py
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-12-19 13:37:32.888491 sympy2c-2.2.2/src/sympy2c.egg-info/
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10696 2022-12-19 13:37:32.000000 sympy2c-2.2.2/src/sympy2c.egg-info/PKG-INFO
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12714 2022-12-19 13:37:32.000000 sympy2c-2.2.2/src/sympy2c.egg-info/SOURCES.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2022-12-19 13:37:32.000000 sympy2c-2.2.2/src/sympy2c.egg-info/dependency_links.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2021-12-09 14:43:13.000000 sympy2c-2.2.2/src/sympy2c.egg-info/not-zip-safe
--rw-r--r--   0 uweschmitt   (501) staff       (20)      259 2022-12-19 13:37:32.000000 sympy2c-2.2.2/src/sympy2c.egg-info/requires.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)        8 2022-12-19 13:37:32.000000 sympy2c-2.2.2/src/sympy2c.egg-info/top_level.txt
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-05-09 18:46:39.191800 sympy2c-2.2.3/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      452 2022-08-16 09:56:27.000000 sympy2c-2.2.3/AUTHORS.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      741 2022-08-16 09:56:27.000000 sympy2c-2.2.3/CONTRIBUTING.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9930 2023-05-09 18:46:20.000000 sympy2c-2.2.3/HISTORY.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      758 2022-08-16 09:56:27.000000 sympy2c-2.2.3/LICENSE.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10826 2023-05-09 18:46:39.191912 sympy2c-2.2.3/PKG-INFO
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       87 2022-10-25 11:20:39.000000 sympy2c-2.2.3/README.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      733 2022-12-13 12:59:39.000000 sympy2c-2.2.3/pyproject.toml
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1210 2023-05-09 18:46:39.192319 sympy2c-2.2.3/setup.cfg
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      293 2022-12-07 15:40:45.000000 sympy2c-2.2.3/setup.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-05-09 18:46:39.112444 sympy2c-2.2.3/src/
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-05-09 18:46:39.117745 sympy2c-2.2.3/src/sympy2c/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2098 2022-12-16 15:27:28.000000 sympy2c-2.2.3/src/sympy2c/__init__.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1487 2022-12-07 15:42:34.000000 sympy2c-2.2.3/src/sympy2c/build_f2c.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2957 2022-12-16 13:38:02.000000 sympy2c-2.2.3/src/sympy2c/build_gsl.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1840 2022-11-22 12:52:11.000000 sympy2c-2.2.3/src/sympy2c/build_lsoda.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2592 2022-12-16 15:30:23.000000 sympy2c-2.2.3/src/sympy2c/build_lsoda_fast.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-05-09 18:46:39.118817 sympy2c-2.2.3/src/sympy2c/c_code/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      872 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/c_code/__init__.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    89476 2023-05-09 12:34:47.000000 sympy2c-2.2.3/src/sympy2c/c_code/lsoda.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    13166 2023-05-09 14:55:41.000000 sympy2c-2.2.3/src/sympy2c/compiler.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3031 2022-10-18 09:16:57.000000 sympy2c-2.2.3/src/sympy2c/create_curry_class.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2154 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/expressions.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-05-09 18:46:39.148644 sympy2c-2.2.3/src/sympy2c/f2c_files/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      304 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/abort_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      194 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/arith.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1328 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/backspac.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      272 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/c_abs.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      354 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/c_cos.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      936 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/c_div.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      349 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/c_exp.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      384 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/c_log.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      350 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/c_sin.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      605 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/c_sqrt.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      494 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/cabs.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1393 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/close.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       44 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/ctype.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      218 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_abs.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_acos.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_asin.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_atan.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      271 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_atn2.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      255 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_cnjg.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      241 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_cos.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_cosh.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      232 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_dim.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      241 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_exp.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      201 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_imag.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      269 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_int.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      291 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_lg10.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      241 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_log.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      688 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_mod.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      281 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_nint.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      207 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_prod.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      266 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_sign.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      241 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_sin.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_sinh.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_sqrt.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      241 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_tan.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/d_tanh.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      239 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/derf_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      253 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/derfc_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2624 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/dfe.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      471 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/dolio.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      972 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/dtime_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1624 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/due.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      521 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/ef1asc_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      427 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/ef1cmc_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2838 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/endfile.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      270 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/erf_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      275 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/erfc_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6442 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/err.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      839 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/etime_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      543 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/exit_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4688 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/f2c.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1139 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/f2c_ctype.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      684 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/f77_aloc.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4933 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/f77vers.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2939 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/fio.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8566 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/fmt.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2006 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/fmt.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      865 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/fmtlib.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      665 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/fp.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      917 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/ftell64_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      900 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/ftell_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      592 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/getarg_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1223 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/getenv_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      218 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/h_abs.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      230 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/h_dim.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      294 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/h_dnnt.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      442 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/h_indx.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      205 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/h_len.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      207 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/h_mod.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      281 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/h_nint.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      266 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/h_sign.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      346 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/hl_ge.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      345 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/hl_gt.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      346 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/hl_le.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      345 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/hl_lt.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    18128 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/i77vers.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      214 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/i_abs.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      225 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/i_dim.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      291 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/i_dnnt.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      430 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/i_indx.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      203 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/i_len.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      211 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/i_mod.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      278 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/i_nint.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      260 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/i_sign.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      196 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/iargc_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2639 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/iio.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1125 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/ilnw.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2732 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/inquire.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      334 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/l_ge.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      333 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/l_gt.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      334 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/l_le.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      333 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/l_lt.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1097 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/lbitbits.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      258 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/lbitshft.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1564 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/lio.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    14743 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/lread.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4616 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/lwrite.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2249 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/main.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     5701 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/open.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      412 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/pow_ci.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      276 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/pow_dd.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      448 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/pow_di.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      489 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/pow_hh.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      488 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/pow_ii.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      516 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/pow_qq.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      436 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/pow_ri.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      851 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/pow_zi.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      549 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/pow_zz.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1151 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/qbitbits.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      258 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/qbitshft.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      206 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_abs.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      233 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_acos.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      233 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_asin.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      233 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_atan.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      253 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_atn2.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      235 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_cnjg.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      229 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_cos.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      233 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_cosh.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      214 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_dim.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      229 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_exp.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      189 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_imag.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      257 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_int.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      279 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_lg10.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      229 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_log.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      678 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_mod.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      269 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_nint.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      248 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_sign.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      229 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_sin.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      233 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_sinh.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      233 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_sqrt.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      229 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_tan.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      233 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/r_tanh.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      718 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/rawio.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8929 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/rdfmt.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      475 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/rewind.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1492 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/rsfe.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1785 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/rsli.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    11585 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/rsne.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1458 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/s_cat.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      722 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/s_cmp.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1024 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/s_copy.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1617 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/s_paus.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      759 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/s_rnge.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      762 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/s_stop.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      828 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/sfe.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      689 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/sig_die.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      842 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/signal1.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      299 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/signal_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      330 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/signbit.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1865 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/sue.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1252 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/sysdep1.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      652 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/system_.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      386 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/typesize.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1619 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/uio.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     7584 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/uninit.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      972 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/util.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4751 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/wref.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     7506 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/wrtfmt.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1280 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/wsfe.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      697 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/wsle.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      479 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/wsne.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1174 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/xwsne.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      268 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/z_abs.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      363 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/z_cos.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      913 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/z_div.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      357 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/z_exp.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2729 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/z_log.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      359 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/z_sin.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      581 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/f2c_files/z_sqrt.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    22285 2022-12-13 15:34:22.000000 sympy2c-2.2.3/src/sympy2c/function.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4024 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/globals.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6039 2022-12-16 14:02:42.000000 sympy2c-2.2.3/src/sympy2c/integral.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9886 2022-10-18 09:16:57.000000 sympy2c-2.2.3/src/sympy2c/interpolation.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-05-09 18:46:39.189846 sympy2c-2.2.3/src/sympy2c/lsoda_modified/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2014 2023-04-27 13:14:52.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/blkdta000.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1251 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/blkdta000.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2185 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/bnorm.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1187 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/bnorm.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     5331 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/cfode.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4252 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/cfode.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      981 2023-04-27 13:57:37.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/d1mach.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4040 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dasum.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2960 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dasum.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4500 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/daxpy.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3493 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/daxpy.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2176 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dcabs1.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1397 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dcabs1.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4294 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dcopy.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3283 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dcopy.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4409 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ddot.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3411 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ddot.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12081 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dgbmv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10532 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dgbmv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12789 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dgemm.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    11119 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dgemm.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9805 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dgemv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8763 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dgemv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6778 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dger.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     5693 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dger.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3991 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dnrm2.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3073 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dnrm2.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4258 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/drot.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3168 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/drot.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3364 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/drotg.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2288 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/drotg.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6291 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/drotm.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     5268 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/drotm.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6604 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/drotmg.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6360 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/drotmg.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12244 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsbmv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    11151 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsbmv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4026 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dscal.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2996 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dscal.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     5466 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsdot.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4203 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsdot.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9921 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dspmv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9466 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dspmv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     7981 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dspr.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     7298 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dspr.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9153 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dspr2.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8614 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dspr2.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4416 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dswap.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3461 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dswap.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12961 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsymm.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    11181 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsymm.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10228 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsymv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9397 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsymv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8248 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsyr.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     7269 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsyr.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9503 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsyr2.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8594 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsyr2.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    13968 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsyr2k.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12494 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsyr2k.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12148 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsyrk.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10798 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsyrk.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    13612 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtbmv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12567 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtbmv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    13711 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtbsv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12651 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtbsv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10626 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtpmv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10659 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtpmv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10721 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtpsv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10741 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtpsv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    13967 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtrmm.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12807 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtrmm.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10696 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtrmv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10128 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtrmv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    14773 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtrsm.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    13788 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtrsm.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10679 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtrsv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10124 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtrsv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3629 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dzasum.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2619 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dzasum.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4341 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dznrm2.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3380 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/dznrm2.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2087 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ewset.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1088 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ewset.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4688 2023-04-27 13:15:16.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/f2c.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3671 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/icamax.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2780 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/icamax.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3720 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/idamax.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2787 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/idamax.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     5025 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/intdy.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3190 2022-12-16 15:22:07.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/intdy.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3670 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/isamax.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2732 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/isamax.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3700 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/izamax.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2804 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/izamax.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3897 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/lsame.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3137 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/lsame.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    97145 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/lsoda.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    79164 2022-12-16 15:22:08.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/lsoda.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10818 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/prja.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     7857 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/prja.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4036 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sasum.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2933 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sasum.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4423 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/saxpy.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3407 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/saxpy.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2120 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/scabs1.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1346 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/scabs1.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3804 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/scasum.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2609 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/scasum.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4308 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/scnrm2.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3323 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/scnrm2.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4246 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/scopy.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3235 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/scopy.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4337 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sdot.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3327 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sdot.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8649 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sdsdot.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     7144 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sdsdot.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    11967 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sgbmv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10398 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sgbmv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12682 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sgemm.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10985 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sgemm.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9693 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sgemv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8629 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sgemv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6676 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sger.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     5572 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sger.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3945 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/snrm2.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2990 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/snrm2.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4622 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/solsy.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3243 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/solsy.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3214 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/srcma.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1834 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/srcma.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4151 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/srot.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3055 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/srot.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3265 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/srotg.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2173 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/srotg.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6218 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/srotm.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     5206 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/srotm.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6441 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/srotmg.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6214 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/srotmg.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12134 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssbmv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    11017 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssbmv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3964 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sscal.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2924 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sscal.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9811 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sspmv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9332 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sspmv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     7901 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sspr.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     7189 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sspr.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9057 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sspr2.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8493 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sspr2.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4362 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sswap.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3401 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/sswap.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12847 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssymm.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    11047 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssymm.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10118 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssymv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9263 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssymv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8166 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssyr.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     7160 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssyr.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9409 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssyr2.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8473 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssyr2.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    13883 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssyr2k.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12360 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssyr2k.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12063 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssyrk.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10676 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssyrk.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    13562 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/stbmv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12495 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/stbmv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    13661 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/stbsv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12579 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/stbsv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    35457 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/stoda.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    27916 2022-11-03 15:17:14.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/stoda.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10576 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/stpmv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10587 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/stpmv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10671 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/stpsv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10669 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/stpsv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    13891 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/strmm.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12697 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/strmm.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10646 2023-04-27 13:14:53.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/strmv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10056 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/strmv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    14706 2023-04-27 13:14:54.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/strsm.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    13679 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/strsm.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10743 2023-04-27 13:14:54.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/strsv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10137 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/strsv.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1505 2023-04-27 13:14:54.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/vmnorm.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      688 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/vmnorm.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3709 2023-04-27 13:14:54.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/xerbla.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2319 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/xerbla.f
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8039 2023-04-27 13:15:16.000000 sympy2c-2.2.3/src/sympy2c/lsoda_modified/xerrwv.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    35609 2022-12-07 15:41:03.000000 sympy2c-2.2.3/src/sympy2c/lu_generator.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    41096 2022-12-16 15:31:56.000000 sympy2c-2.2.3/src/sympy2c/module.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10796 2022-12-16 15:30:23.000000 sympy2c-2.2.3/src/sympy2c/ode.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4759 2022-12-07 16:38:28.000000 sympy2c-2.2.3/src/sympy2c/ode_combined.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4695 2022-12-19 09:21:01.000000 sympy2c-2.2.3/src/sympy2c/ode_combined_cython_template.pyx
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8056 2022-12-16 15:30:23.000000 sympy2c-2.2.3/src/sympy2c/ode_fast.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     7031 2022-12-07 16:39:26.000000 sympy2c-2.2.3/src/sympy2c/ode_fast_cython_template.pyx
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2160 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/python_function.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2380 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/rec_inv.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1339 2022-08-16 09:56:27.000000 sympy2c-2.2.3/src/sympy2c/speedup.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2901 2022-10-18 09:16:57.000000 sympy2c-2.2.3/src/sympy2c/symbol.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3954 2022-12-16 15:30:23.000000 sympy2c-2.2.3/src/sympy2c/utils.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     5927 2022-10-18 09:16:57.000000 sympy2c-2.2.3/src/sympy2c/vector.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9379 2022-09-15 12:26:27.000000 sympy2c-2.2.3/src/sympy2c/visitor.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1179 2022-12-16 13:19:28.000000 sympy2c-2.2.3/src/sympy2c/wrapper.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-05-09 18:46:39.118557 sympy2c-2.2.3/src/sympy2c.egg-info/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10826 2023-05-09 18:46:39.000000 sympy2c-2.2.3/src/sympy2c.egg-info/PKG-INFO
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    13023 2023-05-09 18:46:39.000000 sympy2c-2.2.3/src/sympy2c.egg-info/SOURCES.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2023-05-09 18:46:39.000000 sympy2c-2.2.3/src/sympy2c.egg-info/dependency_links.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2021-12-09 14:43:13.000000 sympy2c-2.2.3/src/sympy2c.egg-info/not-zip-safe
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      259 2023-05-09 18:46:39.000000 sympy2c-2.2.3/src/sympy2c.egg-info/requires.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        8 2023-05-09 18:46:39.000000 sympy2c-2.2.3/src/sympy2c.egg-info/top_level.txt
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-05-09 18:46:39.191673 sympy2c-2.2.3/tests/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8375 2022-12-16 15:30:23.000000 sympy2c-2.2.3/tests/test_basic.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1963 2022-08-16 09:56:27.000000 sympy2c-2.2.3/tests/test_expressions.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      917 2022-08-16 09:56:27.000000 sympy2c-2.2.3/tests/test_import.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3307 2022-12-16 15:30:23.000000 sympy2c-2.2.3/tests/test_module.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      485 2022-10-18 09:16:57.000000 sympy2c-2.2.3/tests/test_numba.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     7297 2022-08-16 09:56:27.000000 sympy2c-2.2.3/tests/test_ode.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    15645 2022-12-16 15:30:24.000000 sympy2c-2.2.3/tests/test_ode_fast.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8153 2022-12-13 13:49:33.000000 sympy2c-2.2.3/tests/test_ode_fast_combined.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4140 2022-12-16 15:30:23.000000 sympy2c-2.2.3/tests/test_pickling.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1100 2022-08-16 09:56:27.000000 sympy2c-2.2.3/tests/test_python_function.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1668 2022-08-16 09:56:27.000000 sympy2c-2.2.3/tests/test_rec_inv.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2041 2022-08-16 09:56:27.000000 sympy2c-2.2.3/tests/test_special_functions.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1489 2022-10-18 09:16:57.000000 sympy2c-2.2.3/tests/test_ufuncs.py
```

### Comparing `sympy2c-2.2.2/CONTRIBUTING.rst` & `sympy2c-2.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/HISTORY.rst` & `sympy2c-2.2.3/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+2.2.3 (2023-05-09)
+------------------
+* updated code to be compatible with latest numba and clang
+* also tested with Python 3.11
+
 2.2.2 (2022-12-19)
 ------------------
 * changed wrapper injection into fast solvers
 
 2.2.1 (2022-12-13)
 ------------------
 * fix broken downward compatibility of version 2.2.0
```

### Comparing `sympy2c-2.2.2/LICENSE.rst` & `sympy2c-2.2.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/PKG-INFO` & `sympy2c-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sympy2c
-Version: 2.2.2
+Version: 2.2.3
 Summary: sympy2c is a sympy to c compiler including solving odes at c level.
 Author: Uwe Schmitt
 Author-email: uwe.schmitt@id.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/sympy2c
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -29,14 +29,19 @@
 
 
 
 =======
 History
 =======
 
+2.2.3 (2023-05-09)
+------------------
+* updated code to be compatible with latest numba and clang
+* also tested with Python 3.11
+
 2.2.2 (2022-12-19)
 ------------------
 * changed wrapper injection into fast solvers
 
 2.2.1 (2022-12-13)
 ------------------
 * fix broken downward compatibility of version 2.2.0
```

### Comparing `sympy2c-2.2.2/pyproject.toml` & `sympy2c-2.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/setup.cfg` & `sympy2c-2.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sympy2c
-version = 2.2.2
+version = 2.2.3
 license = MIT License
 description = sympy2c is a sympy to c compiler including solving odes at c level.
 author = Uwe Schmitt
 author_email = uwe.schmitt@id.ethz.ch
 classifiers = 
 	Intended Audience :: Science/Research
 	Intended Audience :: Developers
```

### Comparing `sympy2c-2.2.2/src/sympy2c/__init__.py` & `sympy2c-2.2.3/src/sympy2c/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/build_f2c.py` & `sympy2c-2.2.3/src/sympy2c/build_f2c.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/build_gsl.py` & `sympy2c-2.2.3/src/sympy2c/build_gsl.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/build_lsoda.py` & `sympy2c-2.2.3/src/sympy2c/build_lsoda.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/build_lsoda_fast.py` & `sympy2c-2.2.3/src/sympy2c/build_lsoda_fast.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/c_code/__init__.py` & `sympy2c-2.2.3/src/sympy2c/c_code/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/c_code/lsoda.c` & `sympy2c-2.2.3/src/sympy2c/c_code/lsoda.c`

 * *Files 1% similar despite different names*

```diff
@@ -49,19 +49,15 @@
 /************
  * idamax.c *
  ************/
 
 #include <math.h>
 #include <stdio.h>
 
-static int 
-idamax(n, dx, incx)
-    double         *dx;
-    int             n, incx;
-
+static int idamax(int n, double *dx, int incx)
 /* Purpose : Find largest component of double vector dx
 
 
    --- Input ---
 
    n    : number of elements in input vector
    dx   : double vector with n+1 elements, dx[0] is not used
@@ -118,18 +114,15 @@
 
 }
 
 /***********
  * dscal.c *
  ***********/
 
-void 
-dscal(n, da, dx, incx)
-    double          da, *dx;
-    int             n, incx;
+void dscal(int n, double da, double * dx, int incx)
 
 /* Purpose : scalar vector multiplication
 
    dx = da * dx
 
 
    --- Input ---
@@ -185,19 +178,16 @@
 
 }
 
 /**********
  * ddot.c *
  **********/
 
-static double 
-ddot(n, dx, incx, dy, incy)
-    double         *dx, *dy;
-    int             n, incx, incy;
-
+static double
+ddot(int n, double *dx, int incx, double *dy, int incy)
 /*
    Purpose : Inner product dx . dy
 
 
    --- Input ---
 
    n    : number of elements in input vector(s)
@@ -277,19 +267,16 @@
 From tam@dragonfly.wri.com Wed Apr 24 15:48:31 1991
 Return-Path: <tam>
 Date: Wed, 24 Apr 91 17:48:43 CDT
 From: tam@dragonfly.wri.com
 To: whitbeck@sanjuan.wrc.unr.edu
 */
 
-static void 
-daxpy(n, da, dx, incx, dy, incy)
-    double          da, *dx, *dy;
-    int             n, incx, incy;
-
+static void
+daxpy(int n, double da, double *dx, int incx, double *dy, int incy)
 /*
    Purpose : To compute
 
    dy = da * dx + dy
 
 
    --- Input ---
@@ -364,19 +351,16 @@
 
 }
 
 /***********
  * dgesl.c *
  ***********/
 
-static void 
-dgesl(a, n, ipvt, b, job)
-    double        **a, *b;
-    int             n, *ipvt, job;
-
+static void
+dgesl(double **a, int n, int *ipvt, double* b, int job)
 /*
    Purpose : dgesl solves the linear system
    a * x = b or Transpose(a) * x = b
    using the factors computed by dgeco or degfa.
 
 
    On Entry :
@@ -465,18 +449,15 @@
 
 }
 
 /***********
  * dgefa.c *
  ***********/
 
-void 
-dgefa(a, n, ipvt, info)
-    double        **a;
-    int             n, *ipvt, *info;
+void dgefa(double **a, int n, int * ipvt, int * info)
 
 /*
    Purpose : dgefa factors a double matrix by Gaussian elimination.
 
    dgefa is usually called by dgeco, but it can be called directly
    with a saving in time if rcond is not needed.
    (Time for dgeco) = (1+9/n)*(time for dgefa).
@@ -843,15 +824,15 @@
 */
 
 void lsoda(_lsoda_f f, _lsoda_jac jac, int neq, double *y, double *t, double tout, int itol, double *rtol, double *atol,
            int itask, int *istate, int iopt, int jt,
            int iwork1, int iwork2, int iwork5, int iwork6, int iwork7, int iwork8, int iwork9,
            double rwork1, double rwork5, double rwork6, double rwork7, void *_data)
 /*
-void 
+void
 lsoda(f, neq, y, t, tout, itol, rtol, atol, itask, istate,
       iopt, jt, iwork1, iwork2, iwork5, iwork6, iwork7, iwork8,
       iwork9, rwork1, rwork5, rwork6, rwork7, _data)
     _lsoda_f        f;
     void           *_data;
 
     int             neq, itol, itask, *istate, iopt, jt;
@@ -986,15 +967,15 @@
             if (*istate == 1) {
                 h0 = 0.;
                 mxordn = mord[1];
                 mxords = mord[2];
             }
         }
         /* end if ( iopt == 0 )   */
-         /* Optional inputs.   */ 
+         /* Optional inputs.   */
         else {        /* if ( iopt = 1 )  */
             ixpr = iwork5;
             if (ixpr < 0 || ixpr > 1) {
                 fprintf(stderr, "[lsoda] ixpr = %d is illegal\n", ixpr);
                 terminate(istate);
                 return;
             }
@@ -1051,15 +1032,15 @@
                 terminate(istate);
                 return;
             }
         }        /* end else   *//* end iopt = 1   */
     }            /* end if ( *istate == 1 || *istate == 3 )   */
     /*
        If *istate = 1, meth is initialized to 1.
-    
+
        Also allocate memory for yh, wm, ewt, savf, acor, ipvt.
     */
     if (*istate == 1) {
 /*
    If memory were not freed, *istate = 3 need not reallocate memory.
    Hence this section is not executed by *istate = 3.
 */
@@ -1387,17 +1368,17 @@
             break;
         }        /* end switch   */
     }            /* end if ( *istate == 2 || *istate == 3 )   */
     /*
        Block e.
        The next block is normally executed for all calls and contains
        the call to the one-step core integrator stoda.
-    
+
        This is a looping point for the integration steps.
-    
+
        First check for too many steps being taken, update ewt ( if not at
        start of problem).  Check for too much accuracy being requested, and
        check for h below the roundoff level in *t.
     */
     while (1) {
         if (*istate != 1 || nst != 0) {
             if ((nst - nslast) >= mxstep) {
@@ -1848,15 +1829,15 @@
         /* end if ( dsm <= 1. )   */
         /*
            The error test failed.  kflag keeps track of multiple failures.
            Restore tn and the yh array to their previous values, and prepare
            to try the step again.  Compute the optimum step size for this or
            one lower.  After 2 or more failures, h is forced to decrease
            by a factor of 0.2 or less.
-         */ 
+         */
         else {
             kflag--;
             tn = told;
             for (j = nq; j >= 1; j--)
                 for (i1 = j; i1 <= nq; i1++) {
                     yp1 = yh[i1];
                     yp2 = yh[i1 + 1];
@@ -1891,15 +1872,15 @@
                Control reaches this section if 3 or more failures have occurred.
                If 10 failures have occurred, exit with kflag = -1.
                It is assumed that the derivatives that have accumulated in the
                yh array have errors of the wrong order.  Hence the first
                derivative is recomputed, and the order is set to 1.  Then
                h is reduced by a factor of 10, and the step is retried,
                until it succeeds or h reaches hmin.
-             */ 
+             */
             else {
                 if (kflag == -10) {
                     kflag = -1;
                     hold = h;
                     jstart = 1;
                     break;
                 } else {
@@ -2229,15 +2210,15 @@
             for (i = 1; i <= n; i++)
                 wm[i][j] = (acor[i] - savf[i]) * fac;
             y[j] = yj;
         }
         nfe += n;
     } else {
         (*jac)(tn, y + 1, jac_matrix, _data);
-        for (j = 1; j <= n; j++) 
+        for (j = 1; j <= n; j++)
             for (i = 1; i <= n; i++)
                 wm[i][j] = -hl0 * jac_matrix[(i - 1) + n * (j - 1)];
         nfe += n;
     }
 /*
    Compute norm of Jacobian.
 */
@@ -2370,15 +2351,15 @@
             }
         }
         /* end functional iteration   */
         /*
            In the case of the chord method, compute the corrector error,
            and solve the linear system with that as right-hand side and
            P as coefficient matrix.
-         */ 
+         */
         else {
             yp1 = yh[2];
             for (i = 1; i <= n; i++)
                 y[i] = h * savf[i] - (yp1[i] + acor[i]);
             solsy(y);
             *del = vmnorm(n, y, ewt);
             yp1 = yh[1];
```

### Comparing `sympy2c-2.2.2/src/sympy2c/compiler.py` & `sympy2c-2.2.3/src/sympy2c/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,17 +237,17 @@
             f"{arg}" + (".ctypes" if is_vector else "")
             for (is_vector, arg) in zip(vector_flags, args)
         ]
         + ["__result.ctypes"]
     )
     arg_decl = ", ".join(args)
     numba_decorator = (
-        f"@numba.njit([{numba_signature}])"
+        f"@numba.jit([{numba_signature}], nopython=True)"
         if not vector_flags or any(vector_flags)
-        else f"@numba.vectorize([{numba_signature}])"
+        else f"@numba.vectorize([{numba_signature}], nopython=True)"
     )
     code = align(
         f"""
     |import numpy as np
     |{numba_decorator}
     |def {name}({arg_decl}):
     |    __result = np.zeros({res_shape if res_shape is not None else (1,)})
```

### Comparing `sympy2c-2.2.2/src/sympy2c/create_curry_class.py` & `sympy2c-2.2.3/src/sympy2c/create_curry_class.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/expressions.py` & `sympy2c-2.2.3/src/sympy2c/expressions.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/backspac.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/backspac.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/c_div.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/c_div.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/c_sqrt.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/c_sqrt.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/close.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/close.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/d_mod.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/d_mod.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/dfe.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/dfe.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/dtime_.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/dtime_.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/due.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/due.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/ef1asc_.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/ef1asc_.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/endfile.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/endfile.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/err.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/err.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/etime_.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/etime_.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/exit_.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/exit_.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/f2c.h` & `sympy2c-2.2.3/src/sympy2c/f2c_files/f2c.h`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/f2c_ctype.h` & `sympy2c-2.2.3/src/sympy2c/f2c_files/f2c_ctype.h`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/f77_aloc.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/f77_aloc.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/f77vers.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/f77vers.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/fio.h` & `sympy2c-2.2.3/src/sympy2c/f2c_files/fio.h`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/fmt.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/fmt.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/fmt.h` & `sympy2c-2.2.3/src/sympy2c/f2c_files/fmt.h`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/fmtlib.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/fmtlib.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/fp.h` & `sympy2c-2.2.3/src/sympy2c/f2c_files/fp.h`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/ftell64_.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/ftell64_.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/ftell_.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/ftell_.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/getarg_.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/getarg_.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/getenv_.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/getenv_.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/i77vers.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/i77vers.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/iio.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/iio.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/ilnw.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/ilnw.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/inquire.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/inquire.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/lbitbits.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/lbitbits.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/lio.h` & `sympy2c-2.2.3/src/sympy2c/f2c_files/lio.h`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/lread.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/lread.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/lwrite.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/lwrite.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/main.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/main.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/open.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/open.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/pow_qq.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/pow_qq.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/pow_zi.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/pow_zi.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/pow_zz.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/pow_zz.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/qbitbits.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/qbitbits.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/r_mod.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/r_mod.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/rawio.h` & `sympy2c-2.2.3/src/sympy2c/f2c_files/rawio.h`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/rdfmt.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/rdfmt.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/rsfe.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/rsfe.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/rsli.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/rsli.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/rsne.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/rsne.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/s_cat.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/s_cat.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/s_cmp.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/s_cmp.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/s_copy.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/s_copy.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/s_paus.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/s_paus.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/s_rnge.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/s_rnge.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/s_stop.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/s_stop.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/sfe.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/sfe.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/sig_die.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/sig_die.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/signal1.h` & `sympy2c-2.2.3/src/sympy2c/f2c_files/signal1.h`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/sue.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/sue.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/sysdep1.h` & `sympy2c-2.2.3/src/sympy2c/f2c_files/sysdep1.h`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/system_.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/system_.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/uio.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/uio.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/uninit.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/uninit.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/util.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/util.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/wref.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/wref.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/wrtfmt.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/wrtfmt.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/wsfe.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/wsfe.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/wsle.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/wsle.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/xwsne.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/xwsne.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/z_div.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/z_div.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/z_log.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/z_log.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/f2c_files/z_sqrt.c` & `sympy2c-2.2.3/src/sympy2c/f2c_files/z_sqrt.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/function.py` & `sympy2c-2.2.3/src/sympy2c/function.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/globals.py` & `sympy2c-2.2.3/src/sympy2c/globals.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/integral.py` & `sympy2c-2.2.3/src/sympy2c/integral.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/interpolation.py` & `sympy2c-2.2.3/src/sympy2c/interpolation.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/blkdta000.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/blkdta000.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/blkdta000.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/blkdta000.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/bnorm.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/bnorm.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/bnorm.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/bnorm.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/cfode.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/cfode.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/cfode.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/cfode.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/d1mach.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/d1mach.c`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 	-- in that order, at the end of the command line, as in
 		cc *.o -lf2c -lm
 	Source for libf2c is in /netlib/f2c/libf2c.zip, e.g.,
 
 		http://www.netlib.org/f2c/libf2c.zip
 /+ Standard C source for D1MACH -- remove the * in column 1 +/ */
 #include <stdio.h>
+#include <stdlib.h>
 #include <float.h>
 #include <math.h>
 double d1mach_(long *i)
 {
   switch(*i){
       case 1: return DBL_MIN;
       case 2: return DBL_MAX;
```

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dasum.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dasum.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dasum.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dasum.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/daxpy.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/daxpy.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/daxpy.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/daxpy.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dcabs1.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dcabs1.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dcabs1.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dcabs1.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dcopy.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dcopy.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dcopy.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dcopy.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ddot.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ddot.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ddot.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ddot.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dgbmv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dgbmv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dgbmv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dgbmv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dgemm.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dgemm.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dgemm.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dgemm.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dgemv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dgemv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dgemv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dgemv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dger.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dger.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dger.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dger.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dnrm2.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dnrm2.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dnrm2.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dnrm2.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/drot.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/drot.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/drot.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/drot.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/drotg.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/drotg.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/drotg.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/drotg.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/drotm.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/drotm.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/drotm.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/drotm.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/drotmg.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/drotmg.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/drotmg.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/drotmg.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsbmv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsbmv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsbmv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsbmv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dscal.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dscal.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dscal.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dscal.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsdot.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsdot.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsdot.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsdot.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dspmv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dspmv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dspmv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dspmv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dspr.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dspr.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dspr.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dspr.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dspr2.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dspr2.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dspr2.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dspr2.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dswap.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dswap.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dswap.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dswap.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsymm.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsymm.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsymm.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsymm.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsymv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsymv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsymv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsymv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsyr.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsyr.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsyr.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsyr.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsyr2.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsyr2.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsyr2.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsyr2.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsyr2k.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsyr2k.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsyr2k.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsyr2k.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsyrk.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsyrk.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dsyrk.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dsyrk.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtbmv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtbmv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtbmv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtbmv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtbsv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtbsv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtbsv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtbsv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtpmv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtpmv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtpmv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtpmv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtpsv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtpsv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtpsv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtpsv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtrmm.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtrmm.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtrmm.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtrmm.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtrmv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtrmv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtrmv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtrmv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtrsm.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtrsm.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtrsm.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtrsm.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtrsv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtrsv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dtrsv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dtrsv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dzasum.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dzasum.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dzasum.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dzasum.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dznrm2.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dznrm2.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/dznrm2.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/dznrm2.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ewset.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ewset.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ewset.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ewset.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/f2c.h` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/f2c.h`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/icamax.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/icamax.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/icamax.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/icamax.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/idamax.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/idamax.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/idamax.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/idamax.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/intdy.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/intdy.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/intdy.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/intdy.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/isamax.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/isamax.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/isamax.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/isamax.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/izamax.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/izamax.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/izamax.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/izamax.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/lsame.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/lsame.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/lsame.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/lsame.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/lsoda.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/lsoda.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/lsoda.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/lsoda.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/prja.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/prja.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/prja.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/prja.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sasum.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sasum.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sasum.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sasum.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/saxpy.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/saxpy.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/saxpy.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/saxpy.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/scabs1.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/scabs1.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/scabs1.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/scabs1.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/scasum.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/scasum.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/scasum.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/scasum.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/scnrm2.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/scnrm2.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/scnrm2.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/scnrm2.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/scopy.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/scopy.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/scopy.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/scopy.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sdot.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sdot.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sdot.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sdot.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sdsdot.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sdsdot.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sdsdot.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sdsdot.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sgbmv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sgbmv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sgbmv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sgbmv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sgemm.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sgemm.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sgemm.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sgemm.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sgemv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sgemv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sgemv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sgemv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sger.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sger.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sger.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sger.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/snrm2.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/snrm2.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/snrm2.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/snrm2.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/solsy.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/solsy.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/solsy.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/solsy.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/srcma.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/srcma.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/srcma.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/srcma.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/srot.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/srot.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/srot.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/srot.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/srotg.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/srotg.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/srotg.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/srotg.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/srotm.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/srotm.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/srotm.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/srotm.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/srotmg.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/srotmg.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/srotmg.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/srotmg.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssbmv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssbmv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssbmv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssbmv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sscal.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sscal.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sscal.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sscal.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sspmv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sspmv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sspmv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sspmv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sspr.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sspr.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sspr.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sspr.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sspr2.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sspr2.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sspr2.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sspr2.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sswap.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sswap.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/sswap.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/sswap.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssymm.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssymm.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssymm.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssymm.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssymv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssymv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssymv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssymv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssyr.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssyr.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssyr.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssyr.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssyr2.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssyr2.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssyr2.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssyr2.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssyr2k.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssyr2k.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssyr2k.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssyr2k.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssyrk.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssyrk.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/ssyrk.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/ssyrk.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/stbmv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/stbmv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/stbmv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/stbmv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/stbsv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/stbsv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/stbsv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/stbsv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/stoda.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/stoda.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/stoda.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/stoda.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/stpmv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/stpmv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/stpmv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/stpmv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/stpsv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/stpsv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/stpsv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/stpsv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/strmm.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/strmm.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/strmm.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/strmm.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/strmv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/strmv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/strmv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/strmv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/strsm.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/strsm.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/strsm.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/strsm.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/strsv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/strsv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/strsv.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/strsv.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/vmnorm.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/vmnorm.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/vmnorm.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/vmnorm.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/xerbla.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/xerbla.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/xerbla.f` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/xerbla.f`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lsoda_modified/xerrwv.c` & `sympy2c-2.2.3/src/sympy2c/lsoda_modified/xerrwv.c`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/lu_generator.py` & `sympy2c-2.2.3/src/sympy2c/lu_generator.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/module.py` & `sympy2c-2.2.3/src/sympy2c/module.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/ode.py` & `sympy2c-2.2.3/src/sympy2c/ode.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/ode_combined.py` & `sympy2c-2.2.3/src/sympy2c/ode_combined.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/ode_combined_cython_template.pyx` & `sympy2c-2.2.3/src/sympy2c/ode_combined_cython_template.pyx`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/ode_fast.py` & `sympy2c-2.2.3/src/sympy2c/ode_fast.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/ode_fast_cython_template.pyx` & `sympy2c-2.2.3/src/sympy2c/ode_fast_cython_template.pyx`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/python_function.py` & `sympy2c-2.2.3/src/sympy2c/python_function.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/rec_inv.py` & `sympy2c-2.2.3/src/sympy2c/rec_inv.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/speedup.py` & `sympy2c-2.2.3/src/sympy2c/speedup.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/symbol.py` & `sympy2c-2.2.3/src/sympy2c/symbol.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/utils.py` & `sympy2c-2.2.3/src/sympy2c/utils.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/vector.py` & `sympy2c-2.2.3/src/sympy2c/vector.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/visitor.py` & `sympy2c-2.2.3/src/sympy2c/visitor.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c/wrapper.py` & `sympy2c-2.2.3/src/sympy2c/wrapper.py`

 * *Files identical despite different names*

### Comparing `sympy2c-2.2.2/src/sympy2c.egg-info/PKG-INFO` & `sympy2c-2.2.3/src/sympy2c.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sympy2c
-Version: 2.2.2
+Version: 2.2.3
 Summary: sympy2c is a sympy to c compiler including solving odes at c level.
 Author: Uwe Schmitt
 Author-email: uwe.schmitt@id.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/sympy2c
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -29,14 +29,19 @@
 
 
 
 =======
 History
 =======
 
+2.2.3 (2023-05-09)
+------------------
+* updated code to be compatible with latest numba and clang
+* also tested with Python 3.11
+
 2.2.2 (2022-12-19)
 ------------------
 * changed wrapper injection into fast solvers
 
 2.2.1 (2022-12-13)
 ------------------
 * fix broken downward compatibility of version 2.2.0
```

### Comparing `sympy2c-2.2.2/src/sympy2c.egg-info/SOURCES.txt` & `sympy2c-2.2.3/src/sympy2c.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -390,8 +390,21 @@
 src/sympy2c/lsoda_modified/strsm.f
 src/sympy2c/lsoda_modified/strsv.c
 src/sympy2c/lsoda_modified/strsv.f
 src/sympy2c/lsoda_modified/vmnorm.c
 src/sympy2c/lsoda_modified/vmnorm.f
 src/sympy2c/lsoda_modified/xerbla.c
 src/sympy2c/lsoda_modified/xerbla.f
-src/sympy2c/lsoda_modified/xerrwv.c
+src/sympy2c/lsoda_modified/xerrwv.c
+tests/test_basic.py
+tests/test_expressions.py
+tests/test_import.py
+tests/test_module.py
+tests/test_numba.py
+tests/test_ode.py
+tests/test_ode_fast.py
+tests/test_ode_fast_combined.py
+tests/test_pickling.py
+tests/test_python_function.py
+tests/test_rec_inv.py
+tests/test_special_functions.py
+tests/test_ufuncs.py
```

