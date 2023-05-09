# Comparing `tmp/clophfit-0.5.2.tar.gz` & `tmp/clophfit-0.5.3.tar.gz`

## Comparing `clophfit-0.5.2.tar` & `clophfit-0.5.3.tar`

### file list

```diff
@@ -1,233 +1,232 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.5.2/.codespellrc
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.5.2/.darglint
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 clophfit-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clophfit-0.5.2/.python-version
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 clophfit-0.5.2/.readthedocs.yml
--rw-r--r--   0        0        0    13863 2020-02-02 00:00:00.000000 clophfit-0.5.2/CHANGELOG.md
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 clophfit-0.5.2/CONTRIBUTING.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.5.2/bandit.yml
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.5.2/cz_customize_info.txt
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.5.2/.github/dependabot.yml
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 clophfit-0.5.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 clophfit-0.5.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.5.2/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.5.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/Makefile
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/conf.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/.gitkeep
--rw-r--r--   0        0        0    49846 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/bs_pd_f1.png
--rw-r--r--   0        0        0    55458 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/bs_pd_f2.png
--rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/bs_pd_f3.png
--rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/bs_pd_f4.png
--rw-r--r--   0        0        0    16293 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/bs_pd_f5.png
--rw-r--r--   0        0        0    23529 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/bs_pd_f6.png
--rw-r--r--   0        0        0    41234 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/bs_pd_f7.png
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/csvtable.png
--rw-r--r--   0        0        0    20158 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/emcee-01.png
--rw-r--r--   0        0        0   109446 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/emcee-02.png
--rw-r--r--   0        0        0    18582 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/emcee-11.png
--rw-r--r--   0        0        0   420822 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/emcee-12.png
--rw-r--r--   0        0        0    14293 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/f01.png
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/file.png
--rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/gR_fit1.png
--rw-r--r--   0        0        0    32629 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/gR_fit2.png
--rw-r--r--   0        0        0   117478 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/gR_fit3.png
--rw-r--r--   0        0        0    42999 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/gR_fit4.png
--rw-r--r--   0        0        0    83505 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/gR_fit5.png
--rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/gR_fit6.png
--rw-r--r--   0        0        0    14823 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/gR_fit7.png
--rw-r--r--   0        0        0    18894 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/glmfit0.png
--rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/glmfit1.png
--rw-r--r--   0        0        0    33541 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/glmfit2.png
--rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/glmfit3.png
--rw-r--r--   0        0        0    34747 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/glmfit_np.r_.png
--rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmfit1.png
--rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmfit2.png
--rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmfit3.png
--rw-r--r--   0        0        0    48655 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmfit4.png
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmfit5.png
--rw-r--r--   0        0        0    21693 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmodel1.png
--rw-r--r--   0        0        0    28428 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmodel2.png
--rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmodel3.png
--rw-r--r--   0        0        0    29389 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmodel4.png
--rw-r--r--   0        0        0    23708 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmodel5.png
--rw-r--r--   0        0        0   187683 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmodel6.png
--rw-r--r--   0        0        0    24709 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/lmodel_H04.png
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/note_file.png
--rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/r_bs.png
--rw-r--r--   0        0        0    24754 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/ratio2P-lmodel1.png
--rw-r--r--   0        0        0    63411 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/ratio2P-lmodel2.png
--rw-r--r--   0        0        0    31838 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/ratio2P_R1.png
--rw-r--r--   0        0        0   114443 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/ratio2P_R2.png
--rw-r--r--   0        0        0    43555 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/ratio2P_R3.png
--rw-r--r--   0        0        0    94094 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/ratio2P_R4.png
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/ratio2P_R5.png
--rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/ratio2P_R6.png
--rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/_static/rpy_bs.png
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/api/api.rst
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/api/prtecan.uml.rst
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/misc/CHANGELOG.md -> ../../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/misc/CONTRIBUTING.md -> ../../CONTRIBUTING.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/misc/license.rst
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/misc/misc.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/references/cli.rst
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/references/description.rst
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/references/older.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/references/references.rst
--rw-r--r--   0        0        0  1541128 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/tutorials/prenspire.ipynb
--rw-r--r--   0        0        0  1966192 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/tutorials/prtecan.ipynb
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/tutorials/tutorials.rst
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/tutorials/usage.org
--rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/tutorials/usage.rst
--rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/tutorials/usage2.org
--rw-r--r--   0        0        0    58554 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/tutorials/usage2.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/__init__.py
--rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/py.typed
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/binding/__init__.py
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/binding/fitting.py
--rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/dil_buffer.py
--rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/dil_correction.py
--rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/fit_rpy.py
--rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/fit_titration.py
--rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/fit_titration_global.py
--rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/merge.py
--rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/plot_tecan.py
--rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/fit.tecan
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/fit.tecan.cl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/new_sort_K.sh
--rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/sum_all
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/sum_e2
--rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/sum_lib
--rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/sum_lib2
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/sum_s202n
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/sum_v224q
--rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/old/bash/w_ave.sh
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/prenspire/__init__.py
--rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/prenspire/prenspire.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/prtecan/__init__.py
--rw-r--r--   0        0        0    51583 2020-02-02 00:00:00.000000 clophfit-0.5.2/src/clophfit/prtecan/prtecan.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/conftest.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/test_binding.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/test_cli.py
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/test_oldscripts.py
--rw-r--r--   0        0        0     9059 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/test_prenspire.py
--rw-r--r--   0        0        0    26589 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/test_prtecan.py
--rw-r--r--   0        0        0    34305 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/24well_clop0_95.csv
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/M1-A6-G12-nota
--rw-r--r--   0        0        0    13407 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/M1-A6-G12.csv
--rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/M1-A6-G12_11columns.csv
--rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/M1-A6-G12_missing_emptyline_fin.csv
--rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/M1-A6-G12_missing_emptyline_ini.csv
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/S202N-E2_pHs-nota
--rw-r--r--   0        0        0   832084 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/S202N-E2_pHs.csv
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/S202N-E2_pHs_nota
--rw-r--r--   0        0        0   103231 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/e2-T-without_sample_column.csv
--rw-r--r--   0        0        0   103682 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/e2dan-emwavelength.csv
--rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/e2dan-exwavelength.csv
--rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/e2dan-exwavelength2.csv
--rw-r--r--   0        0        0   104939 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/e2dan-exwavelengthstrange.csv
--rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/e2dan-with_sample_column.csv
--rw-r--r--   0        0        0   373788 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/h148g-spettroC-Efin.csv
--rw-r--r--   0        0        0   344763 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/h148g-spettroC-idx0.csv
--rw-r--r--   0        0        0   373857 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/h148g-spettroC-idx2.csv
--rw-r--r--   0        0        0   344941 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/h148g-spettroC-incomplete.csv
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/h148g-spettroC-nota
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/h148g-spettroC-nota-Err
--rw-r--r--   0        0        0   373790 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/h148g-spettroC.csv
--rw-r--r--   0        0        0    98464 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/data/NTT_37C_pKa.csv
--rw-r--r--   0        0        0    17235 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/data/output/NTT_37C_pKa_A.csv
--rw-r--r--   0        0        0    68449 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/data/output/NTT_37C_pKa_A.png
--rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/data/output/NTT_37C_pKa_B.csv
--rw-r--r--   0        0        0    53309 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/EnSpire/data/output/NTT_37C_pKa_B.png
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_100.xls
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_150.xls
--rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_20.xls
--rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_5.78.xls
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_50.xls
--rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_6.38.xls
--rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_6.83.xls
--rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_7.24.xls
--rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_7.67.xls
--rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_8.23.xls
--rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_8.82.xls
--rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290212_9.31.xls
--rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290513_5.5.xls
--rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290513_5.5_bad.xls
--rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290513_7.2.xls
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/290513_8.8.xls
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/list.cl
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/list.cl20
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/list.pH
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/list.pH2
--rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/200214 pH data.ods
--rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/NaCl1_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/NaCl2_200214.xls
--rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/NaCl3_200214.xls
--rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/NaCl4_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/NaCl5_200214.xls
--rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/NaCl6_200214.xls
--rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/NaCl7_200214.xls
--rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/NaCl8_200214.xls
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/additions.cl
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/additions.pH
--rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/fit0-1.csv
--rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/fit0.csv
--rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/fit1-1.csv
--rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/fit1.csv
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/list.cl
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/list.pH
--rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/pH5.0_200214.xls
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/pH5.8_200214.xls
--rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/pH6.5_200214.xls
--rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/pH7.1_200214.xls
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/pH7.6_200214.xls
--rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/pH8.3_200214.xls
--rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/pH9.1_200214.xls
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/scheme.txt
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/140220/scheme0.txt
--rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
--rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
--rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/exceptions/84wells_290212_20.xlsx
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/Tecan/exceptions/88wells_290212_20.xlsx
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/A01-20140311a.dat
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/A01.dat
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/A11.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/B01.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/H04.dat
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/NTT-A04-Cl_note
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/copyIP.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/ratio2P.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/w.txt
--rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_A.csv
--rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_A.png
--rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_B.csv
--rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_B.png
--rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_C.csv
--rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_C.png
--rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_D.csv
--rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_D.png
--rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_E.csv
--rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_E.png
--rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_F.csv
--rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/Meas/A04 Cl_F.png
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/global/Cl/A11-failed.dat
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/global/Cl/B05-20130628-cor.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/global/pH/B01-failed.dat
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/global/pH/D05.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/global/pH/H04-with_nan.dat
--rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/k/D05.dat-bs.png
--rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/k/D05.dat.png
--rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/output/global/Cl/B05-20130628-cor.dat.png
--rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.5.2/tests/data/output/global/pH/D05.dat.png
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 clophfit-0.5.2/.gitignore
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.5.2/LICENSE.txt
--rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 clophfit-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 clophfit-0.5.2/docs/README.md
--rw-r--r--   0        0        0     8822 2020-02-02 00:00:00.000000 clophfit-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.5.3/.codespellrc
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.5.3/.darglint
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 clophfit-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clophfit-0.5.3/.python-version
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 clophfit-0.5.3/.readthedocs.yml
+-rw-r--r--   0        0        0    13919 2020-02-02 00:00:00.000000 clophfit-0.5.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 clophfit-0.5.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.5.3/bandit.yml
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.5.3/cz_customize_info.txt
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.5.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 clophfit-0.5.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.5.3/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.5.3/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/Makefile
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/conf.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/.gitkeep
+-rw-r--r--   0        0        0    49846 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/bs_pd_f1.png
+-rw-r--r--   0        0        0    55458 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/bs_pd_f2.png
+-rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/bs_pd_f3.png
+-rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/bs_pd_f4.png
+-rw-r--r--   0        0        0    16293 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/bs_pd_f5.png
+-rw-r--r--   0        0        0    23529 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/bs_pd_f6.png
+-rw-r--r--   0        0        0    41234 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/bs_pd_f7.png
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/csvtable.png
+-rw-r--r--   0        0        0    20158 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/emcee-01.png
+-rw-r--r--   0        0        0   109446 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/emcee-02.png
+-rw-r--r--   0        0        0    18582 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/emcee-11.png
+-rw-r--r--   0        0        0   420822 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/emcee-12.png
+-rw-r--r--   0        0        0    14293 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/f01.png
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/file.png
+-rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/gR_fit1.png
+-rw-r--r--   0        0        0    32629 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/gR_fit2.png
+-rw-r--r--   0        0        0   117478 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/gR_fit3.png
+-rw-r--r--   0        0        0    42999 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/gR_fit4.png
+-rw-r--r--   0        0        0    83505 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/gR_fit5.png
+-rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/gR_fit6.png
+-rw-r--r--   0        0        0    14823 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/gR_fit7.png
+-rw-r--r--   0        0        0    18894 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/glmfit0.png
+-rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/glmfit1.png
+-rw-r--r--   0        0        0    33541 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/glmfit2.png
+-rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/glmfit3.png
+-rw-r--r--   0        0        0    34747 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/glmfit_np.r_.png
+-rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/lmfit1.png
+-rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/lmfit2.png
+-rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/lmfit3.png
+-rw-r--r--   0        0        0    48655 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/lmfit4.png
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/lmfit5.png
+-rw-r--r--   0        0        0    21693 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/lmodel1.png
+-rw-r--r--   0        0        0    28428 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/lmodel2.png
+-rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/lmodel3.png
+-rw-r--r--   0        0        0    29389 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/lmodel4.png
+-rw-r--r--   0        0        0    23708 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/lmodel5.png
+-rw-r--r--   0        0        0   187683 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/lmodel6.png
+-rw-r--r--   0        0        0    24709 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/lmodel_H04.png
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/note_file.png
+-rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/r_bs.png
+-rw-r--r--   0        0        0    24754 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/ratio2P-lmodel1.png
+-rw-r--r--   0        0        0    63411 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/ratio2P-lmodel2.png
+-rw-r--r--   0        0        0    31838 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/ratio2P_R1.png
+-rw-r--r--   0        0        0   114443 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/ratio2P_R2.png
+-rw-r--r--   0        0        0    43555 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/ratio2P_R3.png
+-rw-r--r--   0        0        0    94094 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/ratio2P_R4.png
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/ratio2P_R5.png
+-rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/ratio2P_R6.png
+-rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/_static/rpy_bs.png
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/api/api.rst
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/api/prtecan.uml.rst
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/misc/CHANGELOG.md -> ../../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/misc/CONTRIBUTING.md -> ../../CONTRIBUTING.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/misc/license.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/misc/misc.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/references/cli.rst
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/references/description.rst
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/references/older.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/references/references.rst
+-rw-r--r--   0        0        0  1541128 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/tutorials/prenspire.ipynb
+-rw-r--r--   0        0        0  1966192 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/tutorials/prtecan.ipynb
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/tutorials/tutorials.rst
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/tutorials/usage.org
+-rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/tutorials/usage.rst
+-rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/tutorials/usage2.org
+-rw-r--r--   0        0        0    58554 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/tutorials/usage2.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/__init__.py
+-rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/py.typed
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/binding/__init__.py
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/binding/fitting.py
+-rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/dil_buffer.py
+-rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/dil_correction.py
+-rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/fit_rpy.py
+-rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/fit_titration.py
+-rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/fit_titration_global.py
+-rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/merge.py
+-rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/plot_tecan.py
+-rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/bash/fit.tecan
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/bash/fit.tecan.cl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/bash/new_sort_K.sh
+-rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/bash/sum_all
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/bash/sum_e2
+-rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/bash/sum_lib
+-rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/bash/sum_lib2
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/bash/sum_s202n
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/bash/sum_v224q
+-rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/old/bash/w_ave.sh
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/prenspire/__init__.py
+-rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/prenspire/prenspire.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/prtecan/__init__.py
+-rw-r--r--   0        0        0    51583 2020-02-02 00:00:00.000000 clophfit-0.5.3/src/clophfit/prtecan/prtecan.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/conftest.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/test_binding.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/test_cli.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/test_oldscripts.py
+-rw-r--r--   0        0        0     9059 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/test_prenspire.py
+-rw-r--r--   0        0        0    26589 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/test_prtecan.py
+-rw-r--r--   0        0        0    34305 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/24well_clop0_95.csv
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/M1-A6-G12-nota
+-rw-r--r--   0        0        0    13407 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/M1-A6-G12.csv
+-rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/M1-A6-G12_11columns.csv
+-rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/M1-A6-G12_missing_emptyline_fin.csv
+-rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/M1-A6-G12_missing_emptyline_ini.csv
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/S202N-E2_pHs-nota
+-rw-r--r--   0        0        0   832084 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/S202N-E2_pHs.csv
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/S202N-E2_pHs_nota
+-rw-r--r--   0        0        0   103231 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/e2-T-without_sample_column.csv
+-rw-r--r--   0        0        0   103682 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/e2dan-emwavelength.csv
+-rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/e2dan-exwavelength.csv
+-rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/e2dan-exwavelength2.csv
+-rw-r--r--   0        0        0   104939 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/e2dan-exwavelengthstrange.csv
+-rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/e2dan-with_sample_column.csv
+-rw-r--r--   0        0        0   373788 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/h148g-spettroC-Efin.csv
+-rw-r--r--   0        0        0   344763 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/h148g-spettroC-idx0.csv
+-rw-r--r--   0        0        0   373857 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/h148g-spettroC-idx2.csv
+-rw-r--r--   0        0        0   344941 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/h148g-spettroC-incomplete.csv
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/h148g-spettroC-nota
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/h148g-spettroC-nota-Err
+-rw-r--r--   0        0        0   373790 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/h148g-spettroC.csv
+-rw-r--r--   0        0        0    98464 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/data/NTT_37C_pKa.csv
+-rw-r--r--   0        0        0    17235 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/data/output/NTT_37C_pKa_A.csv
+-rw-r--r--   0        0        0    68449 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/data/output/NTT_37C_pKa_A.png
+-rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/data/output/NTT_37C_pKa_B.csv
+-rw-r--r--   0        0        0    53309 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/EnSpire/data/output/NTT_37C_pKa_B.png
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/290212_100.xls
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/290212_150.xls
+-rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/290212_20.xls
+-rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/290212_5.78.xls
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/290212_50.xls
+-rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/290212_6.38.xls
+-rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/290212_6.83.xls
+-rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/290212_7.24.xls
+-rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/290212_7.67.xls
+-rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/290212_8.23.xls
+-rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/290212_8.82.xls
+-rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/290212_9.31.xls
+-rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/290513_5.5.xls
+-rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/290513_5.5_bad.xls
+-rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/290513_7.2.xls
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/290513_8.8.xls
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/list.cl
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/list.cl20
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/list.pH
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/list.pH2
+-rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/200214 pH data.ods
+-rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/NaCl1_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/NaCl2_200214.xls
+-rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/NaCl3_200214.xls
+-rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/NaCl4_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/NaCl5_200214.xls
+-rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/NaCl6_200214.xls
+-rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/NaCl7_200214.xls
+-rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/NaCl8_200214.xls
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/additions.cl
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/additions.pH
+-rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/fit0-1.csv
+-rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/fit0.csv
+-rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/fit1-1.csv
+-rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/fit1.csv
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/list.cl
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/list.pH
+-rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/pH5.0_200214.xls
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/pH5.8_200214.xls
+-rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/pH6.5_200214.xls
+-rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/pH7.1_200214.xls
+-rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/pH7.6_200214.xls
+-rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/pH8.3_200214.xls
+-rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/pH9.1_200214.xls
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/scheme.txt
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/140220/scheme0.txt
+-rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
+-rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
+-rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/exceptions/84wells_290212_20.xlsx
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/Tecan/exceptions/88wells_290212_20.xlsx
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/A01-20140311a.dat
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/A01.dat
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/A11.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/B01.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/H04.dat
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/NTT-A04-Cl_note
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/copyIP.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/ratio2P.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/w.txt
+-rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/Meas/A04 Cl_A.csv
+-rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/Meas/A04 Cl_A.png
+-rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/Meas/A04 Cl_B.csv
+-rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/Meas/A04 Cl_B.png
+-rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/Meas/A04 Cl_C.csv
+-rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/Meas/A04 Cl_C.png
+-rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/Meas/A04 Cl_D.csv
+-rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/Meas/A04 Cl_D.png
+-rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/Meas/A04 Cl_E.csv
+-rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/Meas/A04 Cl_E.png
+-rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/Meas/A04 Cl_F.csv
+-rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/Meas/A04 Cl_F.png
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/global/Cl/A11-failed.dat
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/global/Cl/B05-20130628-cor.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/global/pH/B01-failed.dat
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/global/pH/D05.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/global/pH/H04-with_nan.dat
+-rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/k/D05.dat-bs.png
+-rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/k/D05.dat.png
+-rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/output/global/Cl/B05-20130628-cor.dat.png
+-rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.5.3/tests/data/output/global/pH/D05.dat.png
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 clophfit-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.5.3/LICENSE.txt
+-rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 clophfit-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     6018 2020-02-02 00:00:00.000000 clophfit-0.5.3/docs/README.md
+-rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 clophfit-0.5.3/PKG-INFO
```

### Comparing `clophfit-0.5.2/.pre-commit-config.yaml` & `clophfit-0.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/CHANGELOG.md` & `clophfit-0.5.3/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,23 @@
+<!-- markdownlint-disable MD024 -->
+<!-- vale write-good.TooWordy = NO -->
+
 # Changelog
 
+## v0.5.3 (2023-05-09)
+
+### Docs
+
+- updated docs/README.md
+
 ## v0.5.2 (2023-05-09)
 
-### Fix
+### CI/CD
 
-- **CI/CD**: release to PyPI
+- Unify CI/CD into a single workflow
 
 ## v0.5.1 (2023-05-09)
 
 ### Fix
 
 - **CI/CD**: release to PyPI
 
@@ -406,15 +415,15 @@
 
 ### Fix
 
 - `clop prtecan` Install from pipx.
 
 ### Refactor
 
-- Path and str are mixing yet it is fixed.
+- Path and str are mixing.
 - tests do not use os.chdir() anymore.
 
 ## 0.3.6 (2022-09-21)
 
 ### Feat
 
 - [docs] Add click-sphinx.
@@ -452,15 +461,15 @@
 ### Added
 
 - Tecan file parser.
 - usage.org (exported to .rst) serves as tutorial in docs and includes:
   - liaisan-data
   - new-bootstrap
   - lmfit global
-  - emcee (very slow)
+  - emcee (extremely slow)
 - command `clop`.
 - <https://pypi.org/project/readme-renderer/> in lint.
 
 ### Changed
 
 - Update to python 3.9 and 3.10.
 - Update dependencies:
@@ -487,33 +496,34 @@
 
 ## 0.2.0 (2021-11-14)
 
 - Reference for running older scripts; reproducibility thanks to
   [Poetry](https://python-poetry.org) and
   [Pyenv](https://github.com/pyenv/pyenv):
 
-      LDFLAGS=-L/usr/lib/openssl-1.0/ CFLAGS=-I/usr/include/openssl-1.0/ pyenv install 3.4.10
+      LDFLAGS=-L/usr/lib/openssl-1.0/ CFLAGS=-I/usr/include/openssl-1.0/ \
+        pyenv install 3.4.10
       ++CONFIGURE_OPTS="--without-ensurepip" pyenv install 3.5.8++
       CC=clang pyenv install 3.5.10
       poetry env use 3.5
       poetry install
-      ../../src/clophfit/fit_titration.py Meas/A04\ Cl_A.csv NTT-A04-Cl_note -t cl -d output-enspire
-      ../../src/clophfit/fit_titration_global.py D05.dat output-D05 --boot 99
-      ../../src/clophfit/fit_titration_global.py -t cl --boot 999 B05-20130628-cor.dat output-B05
+      .. fit_titration.py Meas/A04\ Cl_A.csv NTT-A04-Cl_note -t cl -d output-enspire
+      .. fit_titration_global.py D05.dat output-D05 --boot 99
+      .. fit_titration_global.py -t cl --boot 999 B05-20130628-cor.dat output-B05
 
 - Note that `fit_rpy.py` did never work (indeed did not use #!/usr/bin/env
   python).
 
 - Tested dependencies for `fit_titration` (without warnings):
 
       cycler          0.10.0 Composable style cycles
       lmfit           0.8.3  Least-Squares Minimization with Bounds and Constraints
       matplotlib      1.5.3  Python plotting package
-      numpy           1.10.4 NumPy: array processing for numbers, strings, records, and objects.
-      pandas          0.18.1 Powerful data structures for data analysis, time series,and statistics
+      numpy           1.10.4 NumPy: array processing for numbers, strings, …
+      pandas          0.18.1 Powerful data structures for data analysis, …
       pyparsing       2.4.7  Python parsing module
       python-dateutil 2.8.1  Extensions to the standard Python datetime module
       pytz            2021.3 World timezone definitions, modern and historical
       rpy2            2.3.10 Python interface to the R language (embedded R)
       scipy           0.18.1 SciPy: Scientific Library for Python
       seaborn         0.7.1  Seaborn: statistical data visualization
       six             1.16.0 Python 2 and 3 compatibility utilities
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `clophfit-0.5.2/CONTRIBUTING.md` & `clophfit-0.5.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/cz_customize_info.txt` & `clophfit-0.5.3/cz_customize_info.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/.github/workflows/cd.yml` & `clophfit-0.5.3/.github/workflows/docs.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,66 @@
-# Release to GitHub and PyPI after testing TestPyPI
-name: CD
+# Deploy static content to GitHub Pages
+name: Docs
+
 on:
   push:
-  # workflow_run:
-  #   workflows: ["CI"]
-  #   types:
-  #     - completed
+  workflow_dispatch:
+
+# Allow one concurrent deployment
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 env:
-  STABLE_PYTHON_VERSION: "3.10"
+  STABLE_PYTHON_VERSION: "3.11"
 
 jobs:
-  testpypi:
+  build:
     runs-on: ubuntu-latest
-    if: "startsWith(github.event.head_commit.message, 'bump:')"
-    outputs:
-      version: ${{ steps.version.outputs.ver }}
     steps:
-      - name: Check out the repository
+      - name: Checkout
         uses: actions/checkout@v3
       - name: Set up Python ${{ env.STABLE_PYTHON_VERSION }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ env.STABLE_PYTHON_VERSION }}
-      - name: Get version
-        id: version
+      - name: Install binaries for docs
         run: |
-          echo ${{ github.event.head_commit.message }}
-          ver=`echo ${{ github.event.head_commit.message }} | awk '{ print $NF }'`
-          echo "ver=${ver}" >> $GITHUB_OUTPUT
-          echo "ver=${ver}" >> $GITHUB_ENV
-      - name: Run clop
+          sudo apt-get update
+          sudo apt-get install -y pandoc
+          sudo apt-get install -y plantuml
+      - name: Install pip and hatch
         run: |
-          python -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple/ clophfit==${{ env.ver }}
-          clop --version
-          clop prtecan tests/Tecan/list.pH
-          cat out2/metadata-labels.txt
-
-  release:
-    name: Release to github
-    needs: testpypi
-    runs-on: ubuntu-latest
-    steps:
-      - name: Check out the repository
-        uses: actions/checkout@v3
-      - name: Create Release
-        uses: ncipollo/release-action@v1
+          python -m pip install --constraint=.github/workflows/constraints.txt pip
+          pip install --constraint=.github/workflows/constraints.txt hatch
+          pip --version
+          hatch --version
+      - name: Run hatch
+        run: |
+          hatch run docs:build
+      - name: Upload artifact
+        uses: actions/upload-pages-artifact@v1
         with:
-          # bodyFile: "release.md"
-          tag: v${{ needs.testpypi.outputs.version }}
+          path: "./docs/_build"
 
-  publish:
-    name: Publish to PyPI
-    needs: release
+  deploy:
     runs-on: ubuntu-latest
+    if: ${{ github.ref == 'refs/heads/main' }}
+    needs: build
+    environment:
+      name: github-pages
+      url: ${{ steps.deployment.outputs.page_url }}
+    # Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
+    permissions:
+      contents: read
+      pages: write
+      id-token: write
     steps:
-      - name: Check out the repository
-        uses: actions/checkout@v3
-      - run: |
-          pipx run hatch build
-          pipx run hatch publish --user=__token__ --auth=${{ secrets.PYPI_TOKEN }}
+      - name: Download artifact
+        uses: actions/download-artifact@v3
+        with:
+          name: github-pages
+      - name: Setup Pages
+        uses: actions/configure-pages@v2
+      - name: Deploy to GitHub Pages
+        id: deployment
+        uses: actions/deploy-pages@v2
```

### Comparing `clophfit-0.5.2/.github/workflows/ci.yml` & `clophfit-0.5.3/.github/workflows/ci.yml`

 * *Files 22% similar despite different names*

```diff
@@ -139,7 +139,63 @@
       - name: Create coverage report
         run: |
           hatch run coverage:combine
           hatch run coverage:report
           hatch run coverage:xml
       - name: Upload coverage report
         uses: codecov/codecov-action@v3.1.3
+
+  testpypi:
+    needs: [pre-commit, typeguard, checks, tests, coverage]
+    runs-on: ubuntu-latest
+    if: "startsWith(github.event.head_commit.message, 'bump:')"
+    outputs:
+      version: ${{ steps.version.outputs.ver }}
+    steps:
+      - name: Check out the repository
+        uses: actions/checkout@v3
+      - name: Set up Python ${{ env.STABLE_PYTHON_VERSION }}
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ env.STABLE_PYTHON_VERSION }}
+      - name: Get version
+        id: version
+        run: |
+          echo ${{ github.event.head_commit.message }}
+          ver=`echo ${{ github.event.head_commit.message }} | awk '{ print $NF }'`
+          echo "ver=${ver}" >> $GITHUB_OUTPUT
+          echo "ver=${ver}" >> $GITHUB_ENV
+      - name: Run clop
+        run: |
+          python -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple/ clophfit==${{ env.ver }}
+          clop --version
+          clop prtecan tests/Tecan/list.pH
+          cat out2/metadata-labels.txt
+
+  release:
+    name: Release to github
+    needs: testpypi
+    runs-on: ubuntu-latest
+    steps:
+      - name: Check out the repository
+        uses: actions/checkout@v3
+      - name: Create Release
+        uses: ncipollo/release-action@v1
+        with:
+          # bodyFile: "release.md"
+          tag: v${{ needs.testpypi.outputs.version }}
+
+  publish:
+    name: Publish to PyPI
+    needs: testpypi
+    runs-on: ubuntu-latest
+    steps:
+      - name: Check out the repository
+        uses: actions/checkout@v3
+      - name: Set up Python ${{ env.STABLE_PYTHON_VERSION }}
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ env.STABLE_PYTHON_VERSION }}
+      - name: Build and publish
+        run: |
+          pipx run hatch build
+          pipx run hatch publish --user=__token__ --auth=${{ secrets.PYPI_TOKEN }}
```

### Comparing `clophfit-0.5.2/docs/Makefile` & `clophfit-0.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/conf.py` & `clophfit-0.5.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "ClopHfit"
 copyright = "2021, Daniele Arosio"  # noqa: A001
 author = "Daniele Arosio"
 
 # The full version, including alpha/beta/rc tags
-release = "0.5.2"
+release = "0.5.3"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `clophfit-0.5.2/docs/make.bat` & `clophfit-0.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/bs_pd_f1.png` & `clophfit-0.5.3/docs/_static/bs_pd_f1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/bs_pd_f2.png` & `clophfit-0.5.3/docs/_static/bs_pd_f2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/bs_pd_f3.png` & `clophfit-0.5.3/docs/_static/bs_pd_f3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/bs_pd_f4.png` & `clophfit-0.5.3/docs/_static/bs_pd_f4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/bs_pd_f5.png` & `clophfit-0.5.3/docs/_static/bs_pd_f5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/bs_pd_f6.png` & `clophfit-0.5.3/docs/_static/bs_pd_f6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/bs_pd_f7.png` & `clophfit-0.5.3/docs/_static/bs_pd_f7.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/csvtable.png` & `clophfit-0.5.3/docs/_static/csvtable.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/emcee-01.png` & `clophfit-0.5.3/docs/_static/emcee-01.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/emcee-02.png` & `clophfit-0.5.3/docs/_static/emcee-02.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/emcee-11.png` & `clophfit-0.5.3/docs/_static/emcee-11.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/emcee-12.png` & `clophfit-0.5.3/docs/_static/emcee-12.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/f01.png` & `clophfit-0.5.3/docs/_static/f01.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/file.png` & `clophfit-0.5.3/docs/_static/file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/gR_fit1.png` & `clophfit-0.5.3/docs/_static/gR_fit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/gR_fit2.png` & `clophfit-0.5.3/docs/_static/gR_fit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/gR_fit3.png` & `clophfit-0.5.3/docs/_static/gR_fit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/gR_fit4.png` & `clophfit-0.5.3/docs/_static/gR_fit4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/gR_fit5.png` & `clophfit-0.5.3/docs/_static/gR_fit5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/gR_fit6.png` & `clophfit-0.5.3/docs/_static/gR_fit6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/gR_fit7.png` & `clophfit-0.5.3/docs/_static/gR_fit7.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/glmfit0.png` & `clophfit-0.5.3/docs/_static/glmfit0.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/glmfit1.png` & `clophfit-0.5.3/docs/_static/glmfit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/glmfit2.png` & `clophfit-0.5.3/docs/_static/glmfit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/glmfit3.png` & `clophfit-0.5.3/docs/_static/glmfit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/glmfit_np.r_.png` & `clophfit-0.5.3/docs/_static/glmfit_np.r_.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/lmfit1.png` & `clophfit-0.5.3/docs/_static/lmfit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/lmfit2.png` & `clophfit-0.5.3/docs/_static/lmfit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/lmfit3.png` & `clophfit-0.5.3/docs/_static/lmfit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/lmfit4.png` & `clophfit-0.5.3/docs/_static/lmfit4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/lmfit5.png` & `clophfit-0.5.3/docs/_static/lmfit5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/lmodel1.png` & `clophfit-0.5.3/docs/_static/lmodel1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/lmodel2.png` & `clophfit-0.5.3/docs/_static/lmodel2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/lmodel3.png` & `clophfit-0.5.3/docs/_static/lmodel3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/lmodel4.png` & `clophfit-0.5.3/docs/_static/lmodel4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/lmodel5.png` & `clophfit-0.5.3/docs/_static/lmodel5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/lmodel6.png` & `clophfit-0.5.3/docs/_static/lmodel6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/lmodel_H04.png` & `clophfit-0.5.3/docs/_static/lmodel_H04.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/note_file.png` & `clophfit-0.5.3/docs/_static/note_file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/r_bs.png` & `clophfit-0.5.3/docs/_static/r_bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/ratio2P-lmodel1.png` & `clophfit-0.5.3/docs/_static/ratio2P-lmodel1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/ratio2P-lmodel2.png` & `clophfit-0.5.3/docs/_static/ratio2P-lmodel2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/ratio2P_R1.png` & `clophfit-0.5.3/docs/_static/ratio2P_R1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/ratio2P_R2.png` & `clophfit-0.5.3/docs/_static/ratio2P_R2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/ratio2P_R3.png` & `clophfit-0.5.3/docs/_static/ratio2P_R3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/ratio2P_R4.png` & `clophfit-0.5.3/docs/_static/ratio2P_R4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/ratio2P_R5.png` & `clophfit-0.5.3/docs/_static/ratio2P_R5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/ratio2P_R6.png` & `clophfit-0.5.3/docs/_static/ratio2P_R6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/_static/rpy_bs.png` & `clophfit-0.5.3/docs/_static/rpy_bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/api/api.rst` & `clophfit-0.5.3/docs/api/api.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/api/prtecan.uml.rst` & `clophfit-0.5.3/docs/api/prtecan.uml.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/references/description.rst` & `clophfit-0.5.3/docs/references/description.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/references/older.rst` & `clophfit-0.5.3/docs/references/older.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/tutorials/prenspire.ipynb` & `clophfit-0.5.3/docs/tutorials/prenspire.ipynb`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/tutorials/prtecan.ipynb` & `clophfit-0.5.3/docs/tutorials/prtecan.ipynb`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/tutorials/usage.org` & `clophfit-0.5.3/docs/tutorials/usage.org`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/tutorials/usage.rst` & `clophfit-0.5.3/docs/tutorials/usage.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/tutorials/usage2.org` & `clophfit-0.5.3/docs/tutorials/usage2.org`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/docs/tutorials/usage2.rst` & `clophfit-0.5.3/docs/tutorials/usage2.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/src/clophfit/__main__.py` & `clophfit-0.5.3/src/clophfit/__main__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/src/clophfit/binding/fitting.py` & `clophfit-0.5.3/src/clophfit/binding/fitting.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/src/clophfit/old/dil_buffer.py` & `clophfit-0.5.3/src/clophfit/old/dil_buffer.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/src/clophfit/old/dil_correction.py` & `clophfit-0.5.3/src/clophfit/old/dil_correction.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/src/clophfit/old/fit_rpy.py` & `clophfit-0.5.3/src/clophfit/old/fit_rpy.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/src/clophfit/old/fit_titration.py` & `clophfit-0.5.3/src/clophfit/old/fit_titration.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/src/clophfit/old/fit_titration_global.py` & `clophfit-0.5.3/src/clophfit/old/fit_titration_global.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/src/clophfit/old/merge.py` & `clophfit-0.5.3/src/clophfit/old/merge.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/src/clophfit/old/plot_tecan.py` & `clophfit-0.5.3/src/clophfit/old/plot_tecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/src/clophfit/old/bash/w_ave.sh` & `clophfit-0.5.3/src/clophfit/old/bash/w_ave.sh`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/src/clophfit/prenspire/__init__.py` & `clophfit-0.5.3/src/clophfit/prenspire/__init__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/src/clophfit/prenspire/prenspire.py` & `clophfit-0.5.3/src/clophfit/prenspire/prenspire.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/src/clophfit/prtecan/__init__.py` & `clophfit-0.5.3/src/clophfit/prtecan/__init__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/src/clophfit/prtecan/prtecan.py` & `clophfit-0.5.3/src/clophfit/prtecan/prtecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/test_binding.py` & `clophfit-0.5.3/tests/test_binding.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/test_cli.py` & `clophfit-0.5.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/test_oldscripts.py` & `clophfit-0.5.3/tests/test_oldscripts.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/test_prenspire.py` & `clophfit-0.5.3/tests/test_prenspire.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/test_prtecan.py` & `clophfit-0.5.3/tests/test_prtecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/24well_clop0_95.csv` & `clophfit-0.5.3/tests/EnSpire/24well_clop0_95.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/M1-A6-G12.csv` & `clophfit-0.5.3/tests/EnSpire/M1-A6-G12.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/M1-A6-G12_11columns.csv` & `clophfit-0.5.3/tests/EnSpire/M1-A6-G12_11columns.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/M1-A6-G12_missing_emptyline_fin.csv` & `clophfit-0.5.3/tests/EnSpire/M1-A6-G12_missing_emptyline_fin.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/M1-A6-G12_missing_emptyline_ini.csv` & `clophfit-0.5.3/tests/EnSpire/M1-A6-G12_missing_emptyline_ini.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/S202N-E2_pHs.csv` & `clophfit-0.5.3/tests/EnSpire/S202N-E2_pHs.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/S202N-E2_pHs_nota` & `clophfit-0.5.3/tests/EnSpire/S202N-E2_pHs_nota`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/e2-T-without_sample_column.csv` & `clophfit-0.5.3/tests/EnSpire/e2-T-without_sample_column.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/e2dan-emwavelength.csv` & `clophfit-0.5.3/tests/EnSpire/e2dan-emwavelength.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/e2dan-exwavelength.csv` & `clophfit-0.5.3/tests/EnSpire/e2dan-exwavelength.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/e2dan-exwavelength2.csv` & `clophfit-0.5.3/tests/EnSpire/e2dan-exwavelength2.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/e2dan-exwavelengthstrange.csv` & `clophfit-0.5.3/tests/EnSpire/e2dan-exwavelengthstrange.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/e2dan-with_sample_column.csv` & `clophfit-0.5.3/tests/EnSpire/e2dan-with_sample_column.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/h148g-spettroC-Efin.csv` & `clophfit-0.5.3/tests/EnSpire/h148g-spettroC-Efin.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/h148g-spettroC-idx0.csv` & `clophfit-0.5.3/tests/EnSpire/h148g-spettroC-idx0.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/h148g-spettroC-idx2.csv` & `clophfit-0.5.3/tests/EnSpire/h148g-spettroC-idx2.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/h148g-spettroC-incomplete.csv` & `clophfit-0.5.3/tests/EnSpire/h148g-spettroC-incomplete.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/h148g-spettroC-nota` & `clophfit-0.5.3/tests/EnSpire/h148g-spettroC-nota`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/h148g-spettroC-nota-Err` & `clophfit-0.5.3/tests/EnSpire/h148g-spettroC-nota-Err`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/h148g-spettroC.csv` & `clophfit-0.5.3/tests/EnSpire/h148g-spettroC.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/data/NTT_37C_pKa.csv` & `clophfit-0.5.3/tests/EnSpire/data/NTT_37C_pKa.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/data/output/NTT_37C_pKa_A.csv` & `clophfit-0.5.3/tests/EnSpire/data/output/NTT_37C_pKa_A.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/data/output/NTT_37C_pKa_A.png` & `clophfit-0.5.3/tests/EnSpire/data/output/NTT_37C_pKa_A.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/data/output/NTT_37C_pKa_B.csv` & `clophfit-0.5.3/tests/EnSpire/data/output/NTT_37C_pKa_B.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/EnSpire/data/output/NTT_37C_pKa_B.png` & `clophfit-0.5.3/tests/EnSpire/data/output/NTT_37C_pKa_B.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/290212_100.xls` & `clophfit-0.5.3/tests/Tecan/290212_100.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/290212_150.xls` & `clophfit-0.5.3/tests/Tecan/290212_150.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/290212_20.xls` & `clophfit-0.5.3/tests/Tecan/290212_20.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/290212_5.78.xls` & `clophfit-0.5.3/tests/Tecan/290212_5.78.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/290212_50.xls` & `clophfit-0.5.3/tests/Tecan/290212_50.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/290212_6.38.xls` & `clophfit-0.5.3/tests/Tecan/290212_6.38.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/290212_6.83.xls` & `clophfit-0.5.3/tests/Tecan/290212_6.83.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/290212_7.24.xls` & `clophfit-0.5.3/tests/Tecan/290212_7.24.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/290212_7.67.xls` & `clophfit-0.5.3/tests/Tecan/290212_7.67.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/290212_8.23.xls` & `clophfit-0.5.3/tests/Tecan/290212_8.23.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/290212_8.82.xls` & `clophfit-0.5.3/tests/Tecan/290212_8.82.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/290212_9.31.xls` & `clophfit-0.5.3/tests/Tecan/290212_9.31.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/290513_5.5.xls` & `clophfit-0.5.3/tests/Tecan/290513_5.5.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/290513_5.5_bad.xls` & `clophfit-0.5.3/tests/Tecan/290513_5.5_bad.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/290513_7.2.xls` & `clophfit-0.5.3/tests/Tecan/290513_7.2.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/290513_8.8.xls` & `clophfit-0.5.3/tests/Tecan/290513_8.8.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/200214 pH data.ods` & `clophfit-0.5.3/tests/Tecan/140220/200214 pH data.ods`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/NaCl1_200214.xls` & `clophfit-0.5.3/tests/Tecan/140220/NaCl1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/NaCl2_200214.xls` & `clophfit-0.5.3/tests/Tecan/140220/NaCl2_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/NaCl3_200214.xls` & `clophfit-0.5.3/tests/Tecan/140220/NaCl3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/NaCl4_200214.xls` & `clophfit-0.5.3/tests/Tecan/140220/NaCl4_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/NaCl5_200214.xls` & `clophfit-0.5.3/tests/Tecan/140220/NaCl5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/NaCl6_200214.xls` & `clophfit-0.5.3/tests/Tecan/140220/NaCl6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/NaCl7_200214.xls` & `clophfit-0.5.3/tests/Tecan/140220/NaCl7_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/NaCl8_200214.xls` & `clophfit-0.5.3/tests/Tecan/140220/NaCl8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/fit0-1.csv` & `clophfit-0.5.3/tests/Tecan/140220/fit0-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/fit0.csv` & `clophfit-0.5.3/tests/Tecan/140220/fit0.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/fit1-1.csv` & `clophfit-0.5.3/tests/Tecan/140220/fit1-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/fit1.csv` & `clophfit-0.5.3/tests/Tecan/140220/fit1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/pH5.0_200214.xls` & `clophfit-0.5.3/tests/Tecan/140220/pH5.0_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/pH5.8_200214.xls` & `clophfit-0.5.3/tests/Tecan/140220/pH5.8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/pH6.5_200214.xls` & `clophfit-0.5.3/tests/Tecan/140220/pH6.5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/pH7.1_200214.xls` & `clophfit-0.5.3/tests/Tecan/140220/pH7.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/pH7.6_200214.xls` & `clophfit-0.5.3/tests/Tecan/140220/pH7.6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/pH8.3_200214.xls` & `clophfit-0.5.3/tests/Tecan/140220/pH8.3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/140220/pH9.1_200214.xls` & `clophfit-0.5.3/tests/Tecan/140220/pH9.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx` & `clophfit-0.5.3/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls` & `clophfit-0.5.3/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/exceptions/84wells_290212_20.xlsx` & `clophfit-0.5.3/tests/Tecan/exceptions/84wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/Tecan/exceptions/88wells_290212_20.xlsx` & `clophfit-0.5.3/tests/Tecan/exceptions/88wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/A01-20140311a.dat` & `clophfit-0.5.3/tests/data/A01-20140311a.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/A01.dat` & `clophfit-0.5.3/tests/data/A01.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/NTT-A04-Cl_note` & `clophfit-0.5.3/tests/data/NTT-A04-Cl_note`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/Meas/A04 Cl_A.csv` & `clophfit-0.5.3/tests/data/Meas/A04 Cl_A.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/Meas/A04 Cl_A.png` & `clophfit-0.5.3/tests/data/Meas/A04 Cl_A.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/Meas/A04 Cl_B.csv` & `clophfit-0.5.3/tests/data/Meas/A04 Cl_B.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/Meas/A04 Cl_B.png` & `clophfit-0.5.3/tests/data/Meas/A04 Cl_B.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/Meas/A04 Cl_C.csv` & `clophfit-0.5.3/tests/data/Meas/A04 Cl_C.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/Meas/A04 Cl_C.png` & `clophfit-0.5.3/tests/data/Meas/A04 Cl_C.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/Meas/A04 Cl_D.csv` & `clophfit-0.5.3/tests/data/Meas/A04 Cl_D.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/Meas/A04 Cl_D.png` & `clophfit-0.5.3/tests/data/Meas/A04 Cl_D.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/Meas/A04 Cl_E.csv` & `clophfit-0.5.3/tests/data/Meas/A04 Cl_E.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/Meas/A04 Cl_E.png` & `clophfit-0.5.3/tests/data/Meas/A04 Cl_E.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/Meas/A04 Cl_F.csv` & `clophfit-0.5.3/tests/data/Meas/A04 Cl_F.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/Meas/A04 Cl_F.png` & `clophfit-0.5.3/tests/data/Meas/A04 Cl_F.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/k/D05.dat-bs.png` & `clophfit-0.5.3/tests/data/k/D05.dat-bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/k/D05.dat.png` & `clophfit-0.5.3/tests/data/k/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.5.3/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.5.3/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.5.3/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.5.3/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/output/global/Cl/B05-20130628-cor.dat.png` & `clophfit-0.5.3/tests/data/output/global/Cl/B05-20130628-cor.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/tests/data/output/global/pH/D05.dat.png` & `clophfit-0.5.3/tests/data/output/global/pH/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/.gitignore` & `clophfit-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/LICENSE.txt` & `clophfit-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.2/pyproject.toml` & `clophfit-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
   "macromolecule binding"
 ]
 license = "BSD-3-Clause"
 license-files = {paths = ["LICENSE.txt"]}
 name = "clophfit"
 readme = "docs/README.md"
 requires-python = ">=3.8, <3.12"
-version = "0.5.2"
+version = "0.5.3"
 
 [project.optional-dependencies]
 dev = [
   "commitizen < 3.2.2",
   "ipykernel",
   "jupyter",
   "ruff == 0.0.265",
@@ -106,15 +106,15 @@
 '''
 line-length = 88
 skip-string-normalization = false
 
 [tool.commitizen]
 name = "cz_customize"
 tag_format = "v$version"
-version = "0.5.2"
+version = "0.5.3"
 version_files = [
   "pyproject.toml:version",
   "docs/conf.py:release",
   "docs/README.md:Version"
 ]
 
 [tool.commitizen.customize]
```

### Comparing `clophfit-0.5.2/docs/README.md` & `clophfit-0.5.3/docs/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![codecov](https://codecov.io/gh/darosio/ClopHfit/branch/main/graph/badge.svg?token=OU6F9VFUQ6)](https://codecov.io/gh/darosio/ClopHfit)
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.6354112.svg)](https://doi.org/10.5281/zenodo.6354112)
 
 Cli for fitting macromolecule pH titration or binding assay data, e.g.
 fluorescence spectra.
 
-- Version: "0.5.2"
+- Version: "0.5.3"
 
 ## Features
 
 - Plate Reader data Parser.
 - Perform non-linear least square fitting.
 - Extract and fit pH and chloride titrations of GFP libraries.
   - For 2 labelblocks (e.g. 400, 485 nm) fit data separately and globally.
@@ -180,16 +180,17 @@
 Manually updated pinned dependencies for CI/CD:
 
 - .github/workflows/constraints.txt (testing dependabot)
 
 Configuration files:
 
 - pre-commit configured in .pre-commit-config.yaml;
-- flake8 (for rst-docstrings and bandit) configured in .flake8 (pinned in
-  pre-commit);
+- bandit (sys) configured in bandit.yml;
+- pylint (sys) configured in pyproject.toml;
+- isort (sys) configured in pyproject.toml;
 - black configured in pyproject.toml (pinned in pre-commit);
 - ruff configured in pyproject.toml (pinned in pre-commit);
 - darglint configured in .darglint (pinned in pre-commit);
 - codespell configured in .codespellrc (pinned in pre-commit);
 - coverage configured in pyproject.toml (tests deps);
 - mypy configured in pyproject.toml (tests deps);
 - commitizen in pyproject.toml (dev deps and pinned in pre-commit).
```

### Comparing `clophfit-0.5.2/PKG-INFO` & `clophfit-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clophfit
-Version: 0.5.2
+Version: 0.5.3
 Summary: Cli for fitting macromolecule pH titration or binding assays data e.g. fluorescence spectra.
 Project-URL: Bug Tracker, https://github.com/darosio/ClopHfit/issues
 Project-URL: Changelog, https://darosio.github.io/ClopHfit/misc/CHANGELOG.html
 Project-URL: Discussions, https://github.com/darosio/ClopHfit/discussions
 Project-URL: Documentation, https://clophfit.readthedocs.io
 Project-URL: Github releases, https://github.com/darosio/ClopHfit/releases
 Project-URL: Homepage, https://github.com/darosio/ClopHfit
@@ -71,15 +71,15 @@
 [![codecov](https://codecov.io/gh/darosio/ClopHfit/branch/main/graph/badge.svg?token=OU6F9VFUQ6)](https://codecov.io/gh/darosio/ClopHfit)
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.6354112.svg)](https://doi.org/10.5281/zenodo.6354112)
 
 Cli for fitting macromolecule pH titration or binding assay data, e.g.
 fluorescence spectra.
 
-- Version: "0.5.2"
+- Version: "0.5.3"
 
 ## Features
 
 - Plate Reader data Parser.
 - Perform non-linear least square fitting.
 - Extract and fit pH and chloride titrations of GFP libraries.
   - For 2 labelblocks (e.g. 400, 485 nm) fit data separately and globally.
@@ -246,16 +246,17 @@
 Manually updated pinned dependencies for CI/CD:
 
 - .github/workflows/constraints.txt (testing dependabot)
 
 Configuration files:
 
 - pre-commit configured in .pre-commit-config.yaml;
-- flake8 (for rst-docstrings and bandit) configured in .flake8 (pinned in
-  pre-commit);
+- bandit (sys) configured in bandit.yml;
+- pylint (sys) configured in pyproject.toml;
+- isort (sys) configured in pyproject.toml;
 - black configured in pyproject.toml (pinned in pre-commit);
 - ruff configured in pyproject.toml (pinned in pre-commit);
 - darglint configured in .darglint (pinned in pre-commit);
 - codespell configured in .codespellrc (pinned in pre-commit);
 - coverage configured in pyproject.toml (tests deps);
 - mypy configured in pyproject.toml (tests deps);
 - commitizen in pyproject.toml (dev deps and pinned in pre-commit).
```

