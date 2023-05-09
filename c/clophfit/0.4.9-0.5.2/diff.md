# Comparing `tmp/clophfit-0.4.9.tar.gz` & `tmp/clophfit-0.5.2.tar.gz`

## Comparing `clophfit-0.4.9.tar` & `clophfit-0.5.2.tar`

### file list

```diff
@@ -1,200 +1,233 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.4.9/.codespellrc
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.4.9/.darglint
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 clophfit-0.4.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clophfit-0.4.9/.python-version
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 clophfit-0.4.9/.readthedocs.yml
--rw-r--r--   0        0        0    13365 2020-02-02 00:00:00.000000 clophfit-0.4.9/CHANGELOG.md
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 clophfit-0.4.9/CONTRIBUTING.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.4.9/bandit.yml
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.4.9/cz_customize_info.txt
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.4.9/.github/dependabot.yml
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 clophfit-0.4.9/.github/workflows/cd.yml
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 clophfit-0.4.9/.github/workflows/ci.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.4.9/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.4.9/.github/workflows/docs.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/Makefile
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/conf.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/.gitkeep
--rw-r--r--   0        0        0    49846 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/bs_pd_f1.png
--rw-r--r--   0        0        0    55458 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/bs_pd_f2.png
--rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/bs_pd_f3.png
--rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/bs_pd_f4.png
--rw-r--r--   0        0        0    16293 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/bs_pd_f5.png
--rw-r--r--   0        0        0    23529 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/bs_pd_f6.png
--rw-r--r--   0        0        0    41234 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/bs_pd_f7.png
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/csvtable.png
--rw-r--r--   0        0        0    20158 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/emcee-01.png
--rw-r--r--   0        0        0   109446 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/emcee-02.png
--rw-r--r--   0        0        0    18582 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/emcee-11.png
--rw-r--r--   0        0        0   420822 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/emcee-12.png
--rw-r--r--   0        0        0    14293 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/f01.png
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/file.png
--rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/gR_fit1.png
--rw-r--r--   0        0        0    32629 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/gR_fit2.png
--rw-r--r--   0        0        0   117478 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/gR_fit3.png
--rw-r--r--   0        0        0    42999 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/gR_fit4.png
--rw-r--r--   0        0        0    83505 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/gR_fit5.png
--rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/gR_fit6.png
--rw-r--r--   0        0        0    14823 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/gR_fit7.png
--rw-r--r--   0        0        0    18894 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/glmfit0.png
--rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/glmfit1.png
--rw-r--r--   0        0        0    33541 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/glmfit2.png
--rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/glmfit3.png
--rw-r--r--   0        0        0    34747 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/glmfit_np.r_.png
--rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmfit1.png
--rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmfit2.png
--rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmfit3.png
--rw-r--r--   0        0        0    48655 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmfit4.png
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmfit5.png
--rw-r--r--   0        0        0    21693 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmodel1.png
--rw-r--r--   0        0        0    28428 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmodel2.png
--rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmodel3.png
--rw-r--r--   0        0        0    29389 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmodel4.png
--rw-r--r--   0        0        0    23708 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmodel5.png
--rw-r--r--   0        0        0   187683 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmodel6.png
--rw-r--r--   0        0        0    24709 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmodel_H04.png
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/note_file.png
--rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/r_bs.png
--rw-r--r--   0        0        0    24754 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/ratio2P-lmodel1.png
--rw-r--r--   0        0        0    63411 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/ratio2P-lmodel2.png
--rw-r--r--   0        0        0    31838 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/ratio2P_R1.png
--rw-r--r--   0        0        0   114443 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/ratio2P_R2.png
--rw-r--r--   0        0        0    43555 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/ratio2P_R3.png
--rw-r--r--   0        0        0    94094 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/ratio2P_R4.png
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/ratio2P_R5.png
--rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/ratio2P_R6.png
--rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/rpy_bs.png
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/api/api.rst
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/api/prtecan.uml.rst
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/misc/CHANGELOG.md -> ../../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/misc/CONTRIBUTING.md -> ../../CONTRIBUTING.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/misc/license.rst
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/misc/misc.rst
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/references/description.rst
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/references/references.rst
--rw-r--r--   0        0        0  1966192 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/tutorials/prtecan.ipynb
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/tutorials/tutorials.rst
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/tutorials/usage.org
--rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/tutorials/usage.rst
--rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/tutorials/usage2.org
--rw-r--r--   0        0        0    58554 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/tutorials/usage2.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/__init__.py
--rw-r--r--   0        0        0     7325 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/py.typed
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/binding/__init__.py
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/binding/fitting.py
--rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/dil_buffer.py
--rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/dil_correction.py
--rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/fit_rpy.py
--rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/fit_titration.py
--rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/fit_titration_global.py
--rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/merge.py
--rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/plot_tecan.py
--rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/fit.tecan
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/fit.tecan.cl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/new_sort_K.sh
--rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/sum_all
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/sum_e2
--rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/sum_lib
--rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/sum_lib2
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/sum_s202n
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/sum_v224q
--rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/w_ave.sh
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/prtecan/__init__.py
--rw-r--r--   0        0        0    51839 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/prtecan/prtecan.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/conftest.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/test_binding.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/test_cli.py
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/test_oldscripts.py
--rw-r--r--   0        0        0    26589 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/test_prtecan.py
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_100.xls
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_150.xls
--rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_20.xls
--rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_5.78.xls
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_50.xls
--rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_6.38.xls
--rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_6.83.xls
--rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_7.24.xls
--rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_7.67.xls
--rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_8.23.xls
--rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_8.82.xls
--rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_9.31.xls
--rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290513_5.5.xls
--rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290513_5.5_bad.xls
--rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290513_7.2.xls
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290513_8.8.xls
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/list.cl
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/list.cl20
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/list.pH
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/list.pH2
--rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/200214 pH data.ods
--rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/NaCl1_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/NaCl2_200214.xls
--rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/NaCl3_200214.xls
--rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/NaCl4_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/NaCl5_200214.xls
--rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/NaCl6_200214.xls
--rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/NaCl7_200214.xls
--rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/NaCl8_200214.xls
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/additions.cl
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/additions.pH
--rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/fit0-1.csv
--rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/fit0.csv
--rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/fit1-1.csv
--rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/fit1.csv
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/list.cl
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/list.pH
--rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/pH5.0_200214.xls
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/pH5.8_200214.xls
--rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/pH6.5_200214.xls
--rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/pH7.1_200214.xls
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/pH7.6_200214.xls
--rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/pH8.3_200214.xls
--rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/pH9.1_200214.xls
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/scheme.txt
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/scheme0.txt
--rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
--rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
--rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/exceptions/84wells_290212_20.xlsx
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/exceptions/88wells_290212_20.xlsx
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/A01-20140311a.dat
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/A01.dat
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/A11.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/B01.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/H04.dat
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/NTT-A04-Cl_note
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/copyIP.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/ratio2P.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/w.txt
--rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_A.csv
--rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_A.png
--rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_B.csv
--rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_B.png
--rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_C.csv
--rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_C.png
--rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_D.csv
--rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_D.png
--rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_E.csv
--rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_E.png
--rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_F.csv
--rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_F.png
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/global/Cl/A11-failed.dat
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/global/Cl/B05-20130628-cor.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/global/pH/B01-failed.dat
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/global/pH/D05.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/global/pH/H04-with_nan.dat
--rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/k/D05.dat-bs.png
--rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/k/D05.dat.png
--rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/output/global/Cl/B05-20130628-cor.dat.png
--rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/output/global/pH/D05.dat.png
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 clophfit-0.4.9/.gitignore
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.4.9/LICENSE.txt
--rw-r--r--   0        0        0    11373 2020-02-02 00:00:00.000000 clophfit-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/README.md
--rw-r--r--   0        0        0     8470 2020-02-02 00:00:00.000000 clophfit-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.5.2/.codespellrc
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.5.2/.darglint
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 clophfit-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clophfit-0.5.2/.python-version
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 clophfit-0.5.2/.readthedocs.yml
+-rw-r--r--   0        0        0    13863 2020-02-02 00:00:00.000000 clophfit-0.5.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 clophfit-0.5.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.5.2/bandit.yml
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.5.2/cz_customize_info.txt
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.5.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 clophfit-0.5.2/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 clophfit-0.5.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.5.2/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.5.2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/Makefile
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/conf.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/.gitkeep
+-rw-r--r--   0        0        0    49846 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/bs_pd_f1.png
+-rw-r--r--   0        0        0    55458 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/bs_pd_f2.png
+-rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/bs_pd_f3.png
+-rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/bs_pd_f4.png
+-rw-r--r--   0        0        0    16293 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/bs_pd_f5.png
+-rw-r--r--   0        0        0    23529 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/bs_pd_f6.png
+-rw-r--r--   0        0        0    41234 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/bs_pd_f7.png
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/csvtable.png
+-rw-r--r--   0        0        0    20158 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/emcee-01.png
+-rw-r--r--   0        0        0   109446 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/emcee-02.png
+-rw-r--r--   0        0        0    18582 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/emcee-11.png
+-rw-r--r--   0        0        0   420822 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/emcee-12.png
+-rw-r--r--   0        0        0    14293 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/f01.png
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/file.png
+-rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/gR_fit1.png
+-rw-r--r--   0        0        0    32629 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/gR_fit2.png
+-rw-r--r--   0        0        0   117478 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/gR_fit3.png
+-rw-r--r--   0        0        0    42999 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/gR_fit4.png
+-rw-r--r--   0        0        0    83505 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/gR_fit5.png
+-rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/gR_fit6.png
+-rw-r--r--   0        0        0    14823 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/gR_fit7.png
+-rw-r--r--   0        0        0    18894 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/glmfit0.png
+-rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/glmfit1.png
+-rw-r--r--   0        0        0    33541 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/glmfit2.png
+-rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/glmfit3.png
+-rw-r--r--   0        0        0    34747 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/glmfit_np.r_.png
+-rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmfit1.png
+-rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmfit2.png
+-rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmfit3.png
+-rw-r--r--   0        0        0    48655 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmfit4.png
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmfit5.png
+-rw-r--r--   0        0        0    21693 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmodel1.png
+-rw-r--r--   0        0        0    28428 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmodel2.png
+-rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmodel3.png
+-rw-r--r--   0        0        0    29389 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmodel4.png
+-rw-r--r--   0        0        0    23708 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmodel5.png
+-rw-r--r--   0        0        0   187683 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmodel6.png
+-rw-r--r--   0        0        0    24709 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmodel_H04.png
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/note_file.png
+-rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/r_bs.png
+-rw-r--r--   0        0        0    24754 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/ratio2P-lmodel1.png
+-rw-r--r--   0        0        0    63411 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/ratio2P-lmodel2.png
+-rw-r--r--   0        0        0    31838 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/ratio2P_R1.png
+-rw-r--r--   0        0        0   114443 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/ratio2P_R2.png
+-rw-r--r--   0        0        0    43555 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/ratio2P_R3.png
+-rw-r--r--   0        0        0    94094 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/ratio2P_R4.png
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/ratio2P_R5.png
+-rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/ratio2P_R6.png
+-rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/rpy_bs.png
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/api/api.rst
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/api/prtecan.uml.rst
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/misc/CHANGELOG.md -> ../../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/misc/CONTRIBUTING.md -> ../../CONTRIBUTING.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/misc/license.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/misc/misc.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/references/cli.rst
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/references/description.rst
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/references/older.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/references/references.rst
+-rw-r--r--   0        0        0  1541128 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/tutorials/prenspire.ipynb
+-rw-r--r--   0        0        0  1966192 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/tutorials/prtecan.ipynb
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/tutorials/tutorials.rst
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/tutorials/usage.org
+-rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/tutorials/usage.rst
+-rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/tutorials/usage2.org
+-rw-r--r--   0        0        0    58554 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/tutorials/usage2.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/__init__.py
+-rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/py.typed
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/binding/__init__.py
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/binding/fitting.py
+-rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/dil_buffer.py
+-rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/dil_correction.py
+-rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/fit_rpy.py
+-rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/fit_titration.py
+-rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/fit_titration_global.py
+-rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/merge.py
+-rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/plot_tecan.py
+-rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/fit.tecan
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/fit.tecan.cl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/new_sort_K.sh
+-rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/sum_all
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/sum_e2
+-rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/sum_lib
+-rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/sum_lib2
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/sum_s202n
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/sum_v224q
+-rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/w_ave.sh
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/prenspire/__init__.py
+-rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/prenspire/prenspire.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/prtecan/__init__.py
+-rw-r--r--   0        0        0    51583 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/prtecan/prtecan.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/conftest.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/test_binding.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/test_cli.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/test_oldscripts.py
+-rw-r--r--   0        0        0     9059 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/test_prenspire.py
+-rw-r--r--   0        0        0    26589 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/test_prtecan.py
+-rw-r--r--   0        0        0    34305 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/24well_clop0_95.csv
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/M1-A6-G12-nota
+-rw-r--r--   0        0        0    13407 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/M1-A6-G12.csv
+-rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/M1-A6-G12_11columns.csv
+-rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/M1-A6-G12_missing_emptyline_fin.csv
+-rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/M1-A6-G12_missing_emptyline_ini.csv
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/S202N-E2_pHs-nota
+-rw-r--r--   0        0        0   832084 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/S202N-E2_pHs.csv
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/S202N-E2_pHs_nota
+-rw-r--r--   0        0        0   103231 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/e2-T-without_sample_column.csv
+-rw-r--r--   0        0        0   103682 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/e2dan-emwavelength.csv
+-rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/e2dan-exwavelength.csv
+-rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/e2dan-exwavelength2.csv
+-rw-r--r--   0        0        0   104939 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/e2dan-exwavelengthstrange.csv
+-rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/e2dan-with_sample_column.csv
+-rw-r--r--   0        0        0   373788 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/h148g-spettroC-Efin.csv
+-rw-r--r--   0        0        0   344763 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/h148g-spettroC-idx0.csv
+-rw-r--r--   0        0        0   373857 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/h148g-spettroC-idx2.csv
+-rw-r--r--   0        0        0   344941 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/h148g-spettroC-incomplete.csv
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/h148g-spettroC-nota
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/h148g-spettroC-nota-Err
+-rw-r--r--   0        0        0   373790 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/h148g-spettroC.csv
+-rw-r--r--   0        0        0    98464 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/data/NTT_37C_pKa.csv
+-rw-r--r--   0        0        0    17235 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/data/output/NTT_37C_pKa_A.csv
+-rw-r--r--   0        0        0    68449 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/data/output/NTT_37C_pKa_A.png
+-rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/data/output/NTT_37C_pKa_B.csv
+-rw-r--r--   0        0        0    53309 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/data/output/NTT_37C_pKa_B.png
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_100.xls
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_150.xls
+-rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_20.xls
+-rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_5.78.xls
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_50.xls
+-rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_6.38.xls
+-rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_6.83.xls
+-rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_7.24.xls
+-rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_7.67.xls
+-rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_8.23.xls
+-rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_8.82.xls
+-rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_9.31.xls
+-rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290513_5.5.xls
+-rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290513_5.5_bad.xls
+-rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290513_7.2.xls
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290513_8.8.xls
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/list.cl
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/list.cl20
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/list.pH
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/list.pH2
+-rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/200214 pH data.ods
+-rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/NaCl1_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/NaCl2_200214.xls
+-rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/NaCl3_200214.xls
+-rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/NaCl4_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/NaCl5_200214.xls
+-rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/NaCl6_200214.xls
+-rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/NaCl7_200214.xls
+-rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/NaCl8_200214.xls
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/additions.cl
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/additions.pH
+-rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/fit0-1.csv
+-rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/fit0.csv
+-rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/fit1-1.csv
+-rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/fit1.csv
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/list.cl
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/list.pH
+-rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/pH5.0_200214.xls
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/pH5.8_200214.xls
+-rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/pH6.5_200214.xls
+-rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/pH7.1_200214.xls
+-rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/pH7.6_200214.xls
+-rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/pH8.3_200214.xls
+-rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/pH9.1_200214.xls
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/scheme.txt
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/scheme0.txt
+-rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
+-rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
+-rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/exceptions/84wells_290212_20.xlsx
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/exceptions/88wells_290212_20.xlsx
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/A01-20140311a.dat
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/A01.dat
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/A11.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/B01.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/H04.dat
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/NTT-A04-Cl_note
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/copyIP.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/ratio2P.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/w.txt
+-rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_A.csv
+-rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_A.png
+-rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_B.csv
+-rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_B.png
+-rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_C.csv
+-rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_C.png
+-rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_D.csv
+-rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_D.png
+-rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_E.csv
+-rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_E.png
+-rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_F.csv
+-rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_F.png
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/global/Cl/A11-failed.dat
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/global/Cl/B05-20130628-cor.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/global/pH/B01-failed.dat
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/global/pH/D05.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/global/pH/H04-with_nan.dat
+-rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/k/D05.dat-bs.png
+-rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/k/D05.dat.png
+-rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/output/global/Cl/B05-20130628-cor.dat.png
+-rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/output/global/pH/D05.dat.png
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 clophfit-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.5.2/LICENSE.txt
+-rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 clophfit-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/README.md
+-rw-r--r--   0        0        0     8822 2020-02-02 00:00:00.000000 clophfit-0.5.2/PKG-INFO
```

### Comparing `clophfit-0.4.9/.pre-commit-config.yaml` & `clophfit-0.5.2/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -4,44 +4,49 @@
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-added-large-files # hyper
+        exclude: "^tests/EnSpire/"
       - id: check-case-conflict
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-shebang-scripts-are-executable
       - id: check-merge-conflict
       - id: check-symlinks
       - id: destroyed-symlinks
       - id: check-yaml # hyper
       - id: check-toml # hyper
       - id: debug-statements
       - id: end-of-file-fixer # hyper
+        exclude: "^tests/EnSpire/"
       - id: mixed-line-ending
+        exclude: "^tests/EnSpire/"
       - id: name-tests-test
         args: [--pytest-test-first]
       - id: requirements-txt-fixer
       - id: detect-private-key
       - id: trailing-whitespace # hyper
+        exclude: "^tests/EnSpire/"
 
   - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
     rev: v2.8.0
     hooks:
       - id: pretty-format-ini
         args: [--autofix]
       - id: pretty-format-toml
         args: [--autofix]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.263
+    rev: v0.0.265
     hooks:
       - id: ruff
+        # args: [--exclude, "src/clophfit/prenspire/*"]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black-jupyter
       - id: black
         require_serial: true
@@ -92,12 +97,12 @@
   - repo: https://github.com/shellcheck-py/shellcheck-py
     rev: v0.9.0.2
     hooks:
       - id: shellcheck
         args: [-x]
 
   - repo: https://github.com/commitizen-tools/commitizen
-    rev: 3.2.0
+    rev: 3.2.1
     hooks:
       - id: commitizen
       - id: commitizen-branch
         stages: [push]
```

### Comparing `clophfit-0.4.9/CHANGELOG.md` & `clophfit-0.5.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,44 @@
 # Changelog
 
+## v0.5.2 (2023-05-09)
+
+### Fix
+
+- **CI/CD**: release to PyPI
+
+## v0.5.1 (2023-05-09)
+
+### Fix
+
+- **CI/CD**: release to PyPI
+
+## v0.5.0 (2023-05-09)
+
+### Feat
+
+- Add prenspire to parse PerkinElmer files
+
+### Build
+
+- bump ruff from 0.0.264 to 0.0.265 (#246)
+- bump typeguard from 4.0.0rc5 to 4.0.0rc6 (#245)
+- update commitizen requirement from <3.2.1 to <3.2.2 (#244)
+
+### chore
+
+- update pre-commit hooks (#247)
+- default to python 3.11
+
+## v0.4.10 (2023-05-03)
+
+### Refactor
+
+- Labelblock KEYS
+
 ## v0.4.9 (2023-05-03)
 
 ### Build
 
 - bump sphinx from 6.2.1 to 7.0.0 (#236)
 - bump ruff from 0.0.263 to 0.0.264 (#243)
 - bump autodocsumm from 0.2.10 to 0.2.11 (#242)
```

### Comparing `clophfit-0.4.9/CONTRIBUTING.md` & `clophfit-0.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/cz_customize_info.txt` & `clophfit-0.5.2/cz_customize_info.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/.github/workflows/cd.yml` & `clophfit-0.5.2/.github/workflows/cd.yml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 on:
   push:
   # workflow_run:
   #   workflows: ["CI"]
   #   types:
   #     - completed
 env:
-  STABLE_PYTHON_VERSION: "3.11"
+  STABLE_PYTHON_VERSION: "3.10"
 
 jobs:
   testpypi:
     runs-on: ubuntu-latest
     if: "startsWith(github.event.head_commit.message, 'bump:')"
     outputs:
       version: ${{ steps.version.outputs.ver }}
```

### Comparing `clophfit-0.4.9/.github/workflows/ci.yml` & `clophfit-0.5.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/.github/workflows/docs.yml` & `clophfit-0.5.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/Makefile` & `clophfit-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/conf.py` & `clophfit-0.5.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "ClopHfit"
 copyright = "2021, Daniele Arosio"  # noqa: A001
 author = "Daniele Arosio"
 
 # The full version, including alpha/beta/rc tags
-release = "0.4.9"
+release = "0.5.2"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `clophfit-0.4.9/docs/make.bat` & `clophfit-0.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/bs_pd_f1.png` & `clophfit-0.5.2/docs/_static/bs_pd_f1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/bs_pd_f2.png` & `clophfit-0.5.2/docs/_static/bs_pd_f2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/bs_pd_f3.png` & `clophfit-0.5.2/docs/_static/bs_pd_f3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/bs_pd_f4.png` & `clophfit-0.5.2/docs/_static/bs_pd_f4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/bs_pd_f5.png` & `clophfit-0.5.2/docs/_static/bs_pd_f5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/bs_pd_f6.png` & `clophfit-0.5.2/docs/_static/bs_pd_f6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/bs_pd_f7.png` & `clophfit-0.5.2/docs/_static/bs_pd_f7.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/csvtable.png` & `clophfit-0.5.2/docs/_static/csvtable.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/emcee-01.png` & `clophfit-0.5.2/docs/_static/emcee-01.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/emcee-02.png` & `clophfit-0.5.2/docs/_static/emcee-02.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/emcee-11.png` & `clophfit-0.5.2/docs/_static/emcee-11.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/emcee-12.png` & `clophfit-0.5.2/docs/_static/emcee-12.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/f01.png` & `clophfit-0.5.2/docs/_static/f01.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/file.png` & `clophfit-0.5.2/docs/_static/file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/gR_fit1.png` & `clophfit-0.5.2/docs/_static/gR_fit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/gR_fit2.png` & `clophfit-0.5.2/docs/_static/gR_fit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/gR_fit3.png` & `clophfit-0.5.2/docs/_static/gR_fit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/gR_fit4.png` & `clophfit-0.5.2/docs/_static/gR_fit4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/gR_fit5.png` & `clophfit-0.5.2/docs/_static/gR_fit5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/gR_fit6.png` & `clophfit-0.5.2/docs/_static/gR_fit6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/gR_fit7.png` & `clophfit-0.5.2/docs/_static/gR_fit7.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/glmfit0.png` & `clophfit-0.5.2/docs/_static/glmfit0.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/glmfit1.png` & `clophfit-0.5.2/docs/_static/glmfit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/glmfit2.png` & `clophfit-0.5.2/docs/_static/glmfit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/glmfit3.png` & `clophfit-0.5.2/docs/_static/glmfit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/glmfit_np.r_.png` & `clophfit-0.5.2/docs/_static/glmfit_np.r_.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/lmfit1.png` & `clophfit-0.5.2/docs/_static/lmfit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/lmfit2.png` & `clophfit-0.5.2/docs/_static/lmfit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/lmfit3.png` & `clophfit-0.5.2/docs/_static/lmfit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/lmfit4.png` & `clophfit-0.5.2/docs/_static/lmfit4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/lmfit5.png` & `clophfit-0.5.2/docs/_static/lmfit5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/lmodel1.png` & `clophfit-0.5.2/docs/_static/lmodel1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/lmodel2.png` & `clophfit-0.5.2/docs/_static/lmodel2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/lmodel3.png` & `clophfit-0.5.2/docs/_static/lmodel3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/lmodel4.png` & `clophfit-0.5.2/docs/_static/lmodel4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/lmodel5.png` & `clophfit-0.5.2/docs/_static/lmodel5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/lmodel6.png` & `clophfit-0.5.2/docs/_static/lmodel6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/lmodel_H04.png` & `clophfit-0.5.2/docs/_static/lmodel_H04.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/note_file.png` & `clophfit-0.5.2/docs/_static/note_file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/r_bs.png` & `clophfit-0.5.2/docs/_static/r_bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/ratio2P-lmodel1.png` & `clophfit-0.5.2/docs/_static/ratio2P-lmodel1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/ratio2P-lmodel2.png` & `clophfit-0.5.2/docs/_static/ratio2P-lmodel2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/ratio2P_R1.png` & `clophfit-0.5.2/docs/_static/ratio2P_R1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/ratio2P_R2.png` & `clophfit-0.5.2/docs/_static/ratio2P_R2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/ratio2P_R3.png` & `clophfit-0.5.2/docs/_static/ratio2P_R3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/ratio2P_R4.png` & `clophfit-0.5.2/docs/_static/ratio2P_R4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/ratio2P_R5.png` & `clophfit-0.5.2/docs/_static/ratio2P_R5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/ratio2P_R6.png` & `clophfit-0.5.2/docs/_static/ratio2P_R6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/_static/rpy_bs.png` & `clophfit-0.5.2/docs/_static/rpy_bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/api/prtecan.uml.rst` & `clophfit-0.5.2/docs/api/prtecan.uml.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/references/description.rst` & `clophfit-0.5.2/docs/references/description.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/tutorials/prtecan.ipynb` & `clophfit-0.5.2/docs/tutorials/prtecan.ipynb`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/tutorials/usage.org` & `clophfit-0.5.2/docs/tutorials/usage.org`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/tutorials/usage.rst` & `clophfit-0.5.2/docs/tutorials/usage.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/tutorials/usage2.org` & `clophfit-0.5.2/docs/tutorials/usage2.org`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/docs/tutorials/usage2.rst` & `clophfit-0.5.2/docs/tutorials/usage2.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/src/clophfit/__main__.py` & `clophfit-0.5.2/src/clophfit/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import warnings
 from pathlib import Path
 
 import click
 
 from clophfit import binding
 from clophfit import prtecan
+from clophfit.prenspire.prenspire import EnspireFile
 
 
 def fit_routine(  # noqa: PLR0913
     titan: prtecan.TitrationAnalysis,
     kind: str,
     weight: bool,
     confint: float,
@@ -259,7 +260,24 @@
                 verbose,
                 out,
                 klim,
                 title,
                 sel,
                 pdf,
             )
+
+
+@clop.command("prenspire")
+@click.argument("csv", type=click.Path(path_type=Path))
+@click.option(
+    "--out",
+    type=click.Path(path_type=Path),
+    default="Meas",
+    help="Path to output results.",
+    show_default=True,
+)
+@click.option("--verbose", "-v", count=True, help="Verbosity of messages.")
+def enspire(csv, out, verbose):  # type: ignore
+    """Save spectra as csv tables from EnSpire xls file."""
+    ef = EnspireFile(csv, verbose=verbose)
+    ef.extract_measurements(verbose=verbose)
+    ef.export_measurements(out)
```

### Comparing `clophfit-0.4.9/src/clophfit/binding/fitting.py` & `clophfit-0.5.2/src/clophfit/binding/fitting.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/src/clophfit/old/dil_buffer.py` & `clophfit-0.5.2/src/clophfit/old/dil_buffer.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/src/clophfit/old/dil_correction.py` & `clophfit-0.5.2/src/clophfit/old/dil_correction.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/src/clophfit/old/fit_rpy.py` & `clophfit-0.5.2/src/clophfit/old/fit_rpy.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/src/clophfit/old/fit_titration.py` & `clophfit-0.5.2/src/clophfit/old/fit_titration.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/src/clophfit/old/fit_titration_global.py` & `clophfit-0.5.2/src/clophfit/old/fit_titration_global.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/src/clophfit/old/merge.py` & `clophfit-0.5.2/src/clophfit/old/merge.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/src/clophfit/old/plot_tecan.py` & `clophfit-0.5.2/src/clophfit/old/plot_tecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/src/clophfit/old/bash/w_ave.sh` & `clophfit-0.5.2/src/clophfit/old/bash/w_ave.sh`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/src/clophfit/prtecan/__init__.py` & `clophfit-0.5.2/src/clophfit/prtecan/__init__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/src/clophfit/prtecan/prtecan.py` & `clophfit-0.5.2/src/clophfit/prtecan/prtecan.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import warnings
 from contextlib import suppress
 from dataclasses import InitVar
 from dataclasses import dataclass
 from dataclasses import field
 from pathlib import Path
 from typing import Callable
+from typing import ClassVar
 from typing import Sequence
 
 import matplotlib.pyplot as plt  # type: ignore
 import numpy as np
 import pandas as pd
 import seaborn as sb  # type: ignore  # noqa: ICN001
 from matplotlib.backends.backend_pdf import PdfPages  # type: ignore
@@ -289,14 +290,24 @@
     _data_buffersubtracted: dict[str, float] | None = None
     _data_buffersubtracted_norm: dict[str, float] | None = None
     _buffer_wells: list[str] | None = None
     _buffer: float | None = None
     _buffer_norm: float | None = None
     _sd_buffer: float | None = None
     _sd_buffer_norm: float | None = None
+    _KEYS: ClassVar[list[str]] = [
+        "Emission Bandwidth",
+        "Emission Wavelength",
+        "Excitation Bandwidth",
+        "Excitation Wavelength",
+        "Mode",
+        "Integration Time",
+        "Number of Flashes",
+    ]
+    _NORM_KEYS: ClassVar[list[str]] = ["Integration Time", "Number of Flashes", "Gain"]
 
     def __post_init__(self, lines: list[list[str | int | float]]) -> None:
         """Generate metadata and data for this labelblock."""
         if lines[14][0] == "<>" and lines[23] == lines[24] == [""] * 13:
             stripped = strip_lines(lines)
             stripped[14:23] = []
             self.metadata = extract_metadata(stripped)
@@ -349,40 +360,23 @@
                             stacklevel=2,
                         )
         except AssertionError as exc:
             msg = "Cannot extract data in Labelblock: not 96 wells?"
             raise ValueError(msg) from exc
         return data
 
-    _KEYS = [  # noqa: RUF008 "False positive for ClassVar"
-        "Emission Bandwidth",
-        "Emission Wavelength",
-        "Excitation Bandwidth",
-        "Excitation Wavelength",
-        "Mode",
-        "Integration Time",
-        "Number of Flashes",
-    ]
-
     @property
     def data_norm(self) -> dict[str, float]:
         """Normalize data by number of flashes, integration time and gain."""
         if self._data_norm is None:
-            if (
-                isinstance(self.metadata["Gain"].value, (float, int))
-                and isinstance(self.metadata["Number of Flashes"].value, (float, int))
-                and isinstance(self.metadata["Integration Time"].value, (float, int))
-            ):
-                norm = (
-                    1000.0
-                    / self.metadata["Gain"].value
-                    / self.metadata["Number of Flashes"].value
-                    / self.metadata["Integration Time"].value
-                )
-            else:
+            try:
+                norm = 1000.0
+                for k in Labelblock._NORM_KEYS:
+                    norm /= self.metadata[k].value  # type: ignore
+            except TypeError:
                 warnings.warn(
                     "Could not normalize for non numerical Gain, Number of Flashes or Integration time.",
                     stacklevel=2,
                 )  # pragma: no cover
             self._data_norm = {k: v * norm for k, v in self.data.items()}
         return self._data_norm
```

### Comparing `clophfit-0.4.9/tests/test_binding.py` & `clophfit-0.5.2/tests/test_binding.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/test_oldscripts.py` & `clophfit-0.5.2/tests/test_oldscripts.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/test_prtecan.py` & `clophfit-0.5.2/tests/test_prtecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/290212_100.xls` & `clophfit-0.5.2/tests/Tecan/290212_100.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/290212_150.xls` & `clophfit-0.5.2/tests/Tecan/290212_150.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/290212_20.xls` & `clophfit-0.5.2/tests/Tecan/290212_20.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/290212_5.78.xls` & `clophfit-0.5.2/tests/Tecan/290212_5.78.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/290212_50.xls` & `clophfit-0.5.2/tests/Tecan/290212_50.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/290212_6.38.xls` & `clophfit-0.5.2/tests/Tecan/290212_6.38.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/290212_6.83.xls` & `clophfit-0.5.2/tests/Tecan/290212_6.83.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/290212_7.24.xls` & `clophfit-0.5.2/tests/Tecan/290212_7.24.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/290212_7.67.xls` & `clophfit-0.5.2/tests/Tecan/290212_7.67.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/290212_8.23.xls` & `clophfit-0.5.2/tests/Tecan/290212_8.23.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/290212_8.82.xls` & `clophfit-0.5.2/tests/Tecan/290212_8.82.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/290212_9.31.xls` & `clophfit-0.5.2/tests/Tecan/290212_9.31.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/290513_5.5.xls` & `clophfit-0.5.2/tests/Tecan/290513_5.5.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/290513_5.5_bad.xls` & `clophfit-0.5.2/tests/Tecan/290513_5.5_bad.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/290513_7.2.xls` & `clophfit-0.5.2/tests/Tecan/290513_7.2.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/290513_8.8.xls` & `clophfit-0.5.2/tests/Tecan/290513_8.8.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/200214 pH data.ods` & `clophfit-0.5.2/tests/Tecan/140220/200214 pH data.ods`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/NaCl1_200214.xls` & `clophfit-0.5.2/tests/Tecan/140220/NaCl1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/NaCl2_200214.xls` & `clophfit-0.5.2/tests/Tecan/140220/NaCl2_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/NaCl3_200214.xls` & `clophfit-0.5.2/tests/Tecan/140220/NaCl3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/NaCl4_200214.xls` & `clophfit-0.5.2/tests/Tecan/140220/NaCl4_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/NaCl5_200214.xls` & `clophfit-0.5.2/tests/Tecan/140220/NaCl5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/NaCl6_200214.xls` & `clophfit-0.5.2/tests/Tecan/140220/NaCl6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/NaCl7_200214.xls` & `clophfit-0.5.2/tests/Tecan/140220/NaCl7_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/NaCl8_200214.xls` & `clophfit-0.5.2/tests/Tecan/140220/NaCl8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/fit0-1.csv` & `clophfit-0.5.2/tests/Tecan/140220/fit0-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/fit0.csv` & `clophfit-0.5.2/tests/Tecan/140220/fit0.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/fit1-1.csv` & `clophfit-0.5.2/tests/Tecan/140220/fit1-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/fit1.csv` & `clophfit-0.5.2/tests/Tecan/140220/fit1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/pH5.0_200214.xls` & `clophfit-0.5.2/tests/Tecan/140220/pH5.0_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/pH5.8_200214.xls` & `clophfit-0.5.2/tests/Tecan/140220/pH5.8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/pH6.5_200214.xls` & `clophfit-0.5.2/tests/Tecan/140220/pH6.5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/pH7.1_200214.xls` & `clophfit-0.5.2/tests/Tecan/140220/pH7.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/pH7.6_200214.xls` & `clophfit-0.5.2/tests/Tecan/140220/pH7.6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/pH8.3_200214.xls` & `clophfit-0.5.2/tests/Tecan/140220/pH8.3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/140220/pH9.1_200214.xls` & `clophfit-0.5.2/tests/Tecan/140220/pH9.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx` & `clophfit-0.5.2/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls` & `clophfit-0.5.2/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/exceptions/84wells_290212_20.xlsx` & `clophfit-0.5.2/tests/Tecan/exceptions/84wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/Tecan/exceptions/88wells_290212_20.xlsx` & `clophfit-0.5.2/tests/Tecan/exceptions/88wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/A01-20140311a.dat` & `clophfit-0.5.2/tests/data/A01-20140311a.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/A01.dat` & `clophfit-0.5.2/tests/data/A01.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/NTT-A04-Cl_note` & `clophfit-0.5.2/tests/data/NTT-A04-Cl_note`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/Meas/A04 Cl_A.csv` & `clophfit-0.5.2/tests/data/Meas/A04 Cl_A.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/Meas/A04 Cl_A.png` & `clophfit-0.5.2/tests/data/Meas/A04 Cl_A.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/Meas/A04 Cl_B.csv` & `clophfit-0.5.2/tests/data/Meas/A04 Cl_B.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/Meas/A04 Cl_B.png` & `clophfit-0.5.2/tests/data/Meas/A04 Cl_B.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/Meas/A04 Cl_C.csv` & `clophfit-0.5.2/tests/data/Meas/A04 Cl_C.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/Meas/A04 Cl_C.png` & `clophfit-0.5.2/tests/data/Meas/A04 Cl_C.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/Meas/A04 Cl_D.csv` & `clophfit-0.5.2/tests/data/Meas/A04 Cl_D.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/Meas/A04 Cl_D.png` & `clophfit-0.5.2/tests/data/Meas/A04 Cl_D.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/Meas/A04 Cl_E.csv` & `clophfit-0.5.2/tests/data/Meas/A04 Cl_E.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/Meas/A04 Cl_E.png` & `clophfit-0.5.2/tests/data/Meas/A04 Cl_E.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/Meas/A04 Cl_F.csv` & `clophfit-0.5.2/tests/data/Meas/A04 Cl_F.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/Meas/A04 Cl_F.png` & `clophfit-0.5.2/tests/data/Meas/A04 Cl_F.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/k/D05.dat-bs.png` & `clophfit-0.5.2/tests/data/k/D05.dat-bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/k/D05.dat.png` & `clophfit-0.5.2/tests/data/k/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.5.2/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.5.2/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.5.2/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.5.2/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/output/global/Cl/B05-20130628-cor.dat.png` & `clophfit-0.5.2/tests/data/output/global/Cl/B05-20130628-cor.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/tests/data/output/global/pH/D05.dat.png` & `clophfit-0.5.2/tests/data/output/global/pH/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/.gitignore` & `clophfit-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/LICENSE.txt` & `clophfit-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.9/pyproject.toml` & `clophfit-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -44,22 +44,22 @@
   "macromolecule binding"
 ]
 license = "BSD-3-Clause"
 license-files = {paths = ["LICENSE.txt"]}
 name = "clophfit"
 readme = "docs/README.md"
 requires-python = ">=3.8, <3.12"
-version = "0.4.9"
+version = "0.5.2"
 
 [project.optional-dependencies]
 dev = [
-  "commitizen < 3.2.1",
+  "commitizen < 3.2.2",
   "ipykernel",
   "jupyter",
-  "ruff == 0.0.264",
+  "ruff == 0.0.265",
   "pylsp-mypy",
   "python-lsp-ruff"
 ]
 docs = [
   "autodocsumm == 0.2.11",
   "myst-parser == 1.0.0",
   "nbsphinx == 0.9.1",
@@ -71,15 +71,15 @@
 ]
 tests = [
   "coverage[toml] < 7.2.6",
   "mypy < 1.3",
   "pandas-stubs == 2.0.1.230501",
   "Pygments < 2.15.2",
   "pytest < 7.3.2",
-  "typeguard == 4.0.0rc5",
+  "typeguard == 4.0.0rc6",
   "xdoctest < 1.1.2"
 ]
 
 [project.scripts]
 "clop" = "clophfit.__main__:clop"
 
 [project.urls]
@@ -106,15 +106,15 @@
 '''
 line-length = 88
 skip-string-normalization = false
 
 [tool.commitizen]
 name = "cz_customize"
 tag_format = "v$version"
-version = "0.4.9"
+version = "0.5.2"
 version_files = [
   "pyproject.toml:version",
   "docs/conf.py:release",
   "docs/README.md:Version"
 ]
 
 [tool.commitizen.customize]
@@ -192,16 +192,14 @@
 combine = "coverage combine {args}"
 report = "coverage report"
 xml = "coverage xml"
 
 [tool.hatch.envs.default]
 # type = "pip-deepfreeze"  # pipx runpip hatch install hatch-pip-deepfreeze
 features = ["dev", "tests", "docs"]
-# extra-dependencies = []
-python = "3.10"
 
 [tool.hatch.envs.default.scripts]
 bump = [
   "cz bump --major-version-zero -ch {args}",  # e.g. "--increment PATCH"
   "hatch build",
   "hatch publish -r test"
 ]
@@ -268,27 +266,26 @@
 [tool.mypy]
 # enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 enable_error_code = ["redundant-expr", "truthy-bool"]
 exclude = "src/clophfit/old"
 files = ["src", "tests", "docs/conf.py"]
 plugins = "numpy.typing.mypy_plugin"
 pretty = true
-python_version = "3.10"
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 strict = true
 warn_unreachable = true
 warn_unused_configs = true
 
 [tool.pylint]
 
 [tool.pylint.master]
 ignore-paths = ["src/clophfit/_version.py", "src/clophfit/old"]
-py-version = "3.10"
+py-version = "3.11"
 
 [tool.pylint.messages_control]
 disable = [
   "invalid-name",
   "design",
   "line-too-long",
   "too-many-lines",
```

### Comparing `clophfit-0.4.9/docs/README.md` & `clophfit-0.5.2/docs/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![codecov](https://codecov.io/gh/darosio/ClopHfit/branch/main/graph/badge.svg?token=OU6F9VFUQ6)](https://codecov.io/gh/darosio/ClopHfit)
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.6354112.svg)](https://doi.org/10.5281/zenodo.6354112)
 
 Cli for fitting macromolecule pH titration or binding assay data, e.g.
 fluorescence spectra.
 
-- Version: "0.4.9"
+- Version: "0.5.2"
 
 ## Features
 
 - Plate Reader data Parser.
 - Perform non-linear least square fitting.
 - Extract and fit pH and chloride titrations of GFP libraries.
   - For 2 labelblocks (e.g. 400, 485 nm) fit data separately and globally.
@@ -40,17 +40,26 @@
         clop prtecan list.pH -k ph --scheme ../scheme.txt --no-bg --no-weight \
             --out 4old --Klim 6.8,8.4 --sel 7.6,20
 
 - Predict chloride dissociation constant `K_d` at given pH:
 
         clop eq1 --help
 
+- Parser for EnSpire (PerkinElmer) file:
+
+        clop prenspire file.csv -out folder
+
+  Destination folder (default: "./Meas") will contain for each _Measurement_:
+
+  - a table (csv) in wide tabular form e.g. <lambda, A01, ..., H12>;
+  - corresponding graphical (png) representation of spectra from all wells.
+
 To use clophfit in your python:
 
-    from clophfit import prtecan, binding
+    from clophfit import prenspire, prtecan, binding
 
 ## Installation
 
     pipx install clophfit
 
 You can get the library directly from
 [PyPI](https://pypi.org/project/ClopHfit/):
@@ -67,30 +76,31 @@
   [pip-deepfreeze](https://pypi.org/project/pip-deepfreeze/). You can run
   `hatch env show` to list available environments and scripts.
 
         hatch run init  # init repo with pre-commit hooks
         hatch run sync  # sync venv with deepfreeze
 
         hatch run lint:run
-        hatch run tests.py3.10:all
+        hatch run tests.py3.11:all
 
   Hatch handles everything for you, including setting up an temporary virtual
   environment for each run.
 
 - `pre-commit` for all style and consistency checking. While you can run it with
   nox, this is such an important tool that it deserves to be installed on its
   own. If pre-commit fails during pushing upstream then stage changes, Commit
   Extend (into previous commit), and repeat pushing.
 
 `pip`, `pip-deepfreeze` and `hatch` are pinned in
 .github/workflows/constraints.txt for consistency with CI/CD.
 
     pipx install pre-commit
-    pipx install hatch
-    pipx runpip hatch install hatch-pip-deepfreeze
+    pipx install pip-deepfreeze
+
+    pacman -S python-hatch python-hyperlink python-httpx
 
 ### Setting up a development with direnv
 
     echo "layout hatch" > .envrc
     hatch run init
 
 ### Setting up a development environment manually
@@ -143,14 +153,15 @@
 ### Bump and releasing
 
 To bump version and upload build to test.pypi using:
 
     hatch run bump
     hatch run bump "--increment PATCH" "--files-only" \
         ["--no-verify" to bypass pre-commit and commit-msg hooks]
+    git push
 
 while to update only the CHANGELOG.md file:
 
     hatch run ch
 
 Release will automatically occur after pushing.
```

### Comparing `clophfit-0.4.9/PKG-INFO` & `clophfit-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clophfit
-Version: 0.4.9
+Version: 0.5.2
 Summary: Cli for fitting macromolecule pH titration or binding assays data e.g. fluorescence spectra.
 Project-URL: Bug Tracker, https://github.com/darosio/ClopHfit/issues
 Project-URL: Changelog, https://darosio.github.io/ClopHfit/misc/CHANGELOG.html
 Project-URL: Discussions, https://github.com/darosio/ClopHfit/discussions
 Project-URL: Documentation, https://clophfit.readthedocs.io
 Project-URL: Github releases, https://github.com/darosio/ClopHfit/releases
 Project-URL: Homepage, https://github.com/darosio/ClopHfit
@@ -35,20 +35,20 @@
 Requires-Dist: rpy2<3.5.12
 Requires-Dist: scipy<1.10.2
 Requires-Dist: seaborn<0.12.3
 Requires-Dist: sympy<1.11.2
 Requires-Dist: tqdm<4.65.1
 Requires-Dist: xlrd<2.0.2
 Provides-Extra: dev
-Requires-Dist: commitizen<3.2.1; extra == 'dev'
+Requires-Dist: commitizen<3.2.2; extra == 'dev'
 Requires-Dist: ipykernel; extra == 'dev'
 Requires-Dist: jupyter; extra == 'dev'
 Requires-Dist: pylsp-mypy; extra == 'dev'
 Requires-Dist: python-lsp-ruff; extra == 'dev'
-Requires-Dist: ruff==0.0.264; extra == 'dev'
+Requires-Dist: ruff==0.0.265; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: autodocsumm==0.2.11; extra == 'docs'
 Requires-Dist: myst-parser==1.0.0; extra == 'docs'
 Requires-Dist: nbsphinx==0.9.1; extra == 'docs'
 Requires-Dist: pydata-sphinx-theme==0.13.3; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints==1.23.0; extra == 'docs'
 Requires-Dist: sphinx-click==4.4.0; extra == 'docs'
@@ -56,30 +56,30 @@
 Requires-Dist: sphinxcontrib-plantuml==0.25; extra == 'docs'
 Provides-Extra: tests
 Requires-Dist: coverage[toml]<7.2.6; extra == 'tests'
 Requires-Dist: mypy<1.3; extra == 'tests'
 Requires-Dist: pandas-stubs==2.0.1.230501; extra == 'tests'
 Requires-Dist: pygments<2.15.2; extra == 'tests'
 Requires-Dist: pytest<7.3.2; extra == 'tests'
-Requires-Dist: typeguard==4.0.0rc5; extra == 'tests'
+Requires-Dist: typeguard==4.0.0rc6; extra == 'tests'
 Requires-Dist: xdoctest<1.1.2; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # ClopHfit
 
 [![PyPI](https://img.shields.io/pypi/v/ClopHfit.svg)](https://pypi.org/project/ClopHfit/)
 [![CI](https://github.com/darosio/ClopHfit/actions/workflows/ci.yml/badge.svg)](https://github.com/darosio/ClopHfit/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/darosio/ClopHfit/branch/main/graph/badge.svg?token=OU6F9VFUQ6)](https://codecov.io/gh/darosio/ClopHfit)
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.6354112.svg)](https://doi.org/10.5281/zenodo.6354112)
 
 Cli for fitting macromolecule pH titration or binding assay data, e.g.
 fluorescence spectra.
 
-- Version: "0.4.9"
+- Version: "0.5.2"
 
 ## Features
 
 - Plate Reader data Parser.
 - Perform non-linear least square fitting.
 - Extract and fit pH and chloride titrations of GFP libraries.
   - For 2 labelblocks (e.g. 400, 485 nm) fit data separately and globally.
@@ -106,17 +106,26 @@
         clop prtecan list.pH -k ph --scheme ../scheme.txt --no-bg --no-weight \
             --out 4old --Klim 6.8,8.4 --sel 7.6,20
 
 - Predict chloride dissociation constant `K_d` at given pH:
 
         clop eq1 --help
 
+- Parser for EnSpire (PerkinElmer) file:
+
+        clop prenspire file.csv -out folder
+
+  Destination folder (default: "./Meas") will contain for each _Measurement_:
+
+  - a table (csv) in wide tabular form e.g. <lambda, A01, ..., H12>;
+  - corresponding graphical (png) representation of spectra from all wells.
+
 To use clophfit in your python:
 
-    from clophfit import prtecan, binding
+    from clophfit import prenspire, prtecan, binding
 
 ## Installation
 
     pipx install clophfit
 
 You can get the library directly from
 [PyPI](https://pypi.org/project/ClopHfit/):
@@ -133,30 +142,31 @@
   [pip-deepfreeze](https://pypi.org/project/pip-deepfreeze/). You can run
   `hatch env show` to list available environments and scripts.
 
         hatch run init  # init repo with pre-commit hooks
         hatch run sync  # sync venv with deepfreeze
 
         hatch run lint:run
-        hatch run tests.py3.10:all
+        hatch run tests.py3.11:all
 
   Hatch handles everything for you, including setting up an temporary virtual
   environment for each run.
 
 - `pre-commit` for all style and consistency checking. While you can run it with
   nox, this is such an important tool that it deserves to be installed on its
   own. If pre-commit fails during pushing upstream then stage changes, Commit
   Extend (into previous commit), and repeat pushing.
 
 `pip`, `pip-deepfreeze` and `hatch` are pinned in
 .github/workflows/constraints.txt for consistency with CI/CD.
 
     pipx install pre-commit
-    pipx install hatch
-    pipx runpip hatch install hatch-pip-deepfreeze
+    pipx install pip-deepfreeze
+
+    pacman -S python-hatch python-hyperlink python-httpx
 
 ### Setting up a development with direnv
 
     echo "layout hatch" > .envrc
     hatch run init
 
 ### Setting up a development environment manually
@@ -209,14 +219,15 @@
 ### Bump and releasing
 
 To bump version and upload build to test.pypi using:
 
     hatch run bump
     hatch run bump "--increment PATCH" "--files-only" \
         ["--no-verify" to bypass pre-commit and commit-msg hooks]
+    git push
 
 while to update only the CHANGELOG.md file:
 
     hatch run ch
 
 Release will automatically occur after pushing.
```

