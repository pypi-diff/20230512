# Comparing `tmp/clophfit-0.5.4.tar.gz` & `tmp/clophfit-0.6.0.tar.gz`

## Comparing `clophfit-0.5.4.tar` & `clophfit-0.6.0.tar`

### file list

```diff
@@ -1,230 +1,620 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.5.4/.codespellrc
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.5.4/.darglint
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 clophfit-0.5.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clophfit-0.5.4/.python-version
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 clophfit-0.5.4/.readthedocs.yml
--rw-r--r--   0        0        0    14107 2020-02-02 00:00:00.000000 clophfit-0.5.4/CHANGELOG.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.5.4/bandit.yml
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.5.4/cz_customize_info.txt
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.5.4/.github/dependabot.yml
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 clophfit-0.5.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.5.4/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.5.4/.github/workflows/docs.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/Makefile
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/click.rst
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/conf.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/.gitkeep
--rw-r--r--   0        0        0    49846 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/bs_pd_f1.png
--rw-r--r--   0        0        0    55458 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/bs_pd_f2.png
--rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/bs_pd_f3.png
--rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/bs_pd_f4.png
--rw-r--r--   0        0        0    16293 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/bs_pd_f5.png
--rw-r--r--   0        0        0    23529 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/bs_pd_f6.png
--rw-r--r--   0        0        0    41234 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/bs_pd_f7.png
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/csvtable.png
--rw-r--r--   0        0        0    20158 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/emcee-01.png
--rw-r--r--   0        0        0   109446 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/emcee-02.png
--rw-r--r--   0        0        0    18582 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/emcee-11.png
--rw-r--r--   0        0        0   420822 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/emcee-12.png
--rw-r--r--   0        0        0    14293 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/f01.png
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/file.png
--rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/gR_fit1.png
--rw-r--r--   0        0        0    32629 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/gR_fit2.png
--rw-r--r--   0        0        0   117478 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/gR_fit3.png
--rw-r--r--   0        0        0    42999 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/gR_fit4.png
--rw-r--r--   0        0        0    83505 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/gR_fit5.png
--rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/gR_fit6.png
--rw-r--r--   0        0        0    14823 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/gR_fit7.png
--rw-r--r--   0        0        0    18894 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/glmfit0.png
--rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/glmfit1.png
--rw-r--r--   0        0        0    33541 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/glmfit2.png
--rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/glmfit3.png
--rw-r--r--   0        0        0    34747 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/glmfit_np.r_.png
--rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/lmfit1.png
--rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/lmfit2.png
--rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/lmfit3.png
--rw-r--r--   0        0        0    48655 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/lmfit4.png
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/lmfit5.png
--rw-r--r--   0        0        0    21693 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/lmodel1.png
--rw-r--r--   0        0        0    28428 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/lmodel2.png
--rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/lmodel3.png
--rw-r--r--   0        0        0    29389 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/lmodel4.png
--rw-r--r--   0        0        0    23708 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/lmodel5.png
--rw-r--r--   0        0        0   187683 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/lmodel6.png
--rw-r--r--   0        0        0    24709 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/lmodel_H04.png
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/note_file.png
--rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/r_bs.png
--rw-r--r--   0        0        0    24754 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/ratio2P-lmodel1.png
--rw-r--r--   0        0        0    63411 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/ratio2P-lmodel2.png
--rw-r--r--   0        0        0    31838 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/ratio2P_R1.png
--rw-r--r--   0        0        0   114443 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/ratio2P_R2.png
--rw-r--r--   0        0        0    43555 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/ratio2P_R3.png
--rw-r--r--   0        0        0    94094 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/ratio2P_R4.png
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/ratio2P_R5.png
--rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/ratio2P_R6.png
--rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/_static/rpy_bs.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/api/api.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/api/binding.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/api/prenspire.rst
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/api/prtecan.rst
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/references/contributing.rst
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/references/description.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/references/development.rst
--rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/references/older.rst
--rw-r--r--   0        0        0  1541128 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/tutorials/prenspire.ipynb
--rw-r--r--   0        0        0  1966192 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/tutorials/prtecan.ipynb
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/tutorials/tutorials.rst
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/tutorials/usage.org
--rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/tutorials/usage.rst
--rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/tutorials/usage2.org
--rw-r--r--   0        0        0    58554 2020-02-02 00:00:00.000000 clophfit-0.5.4/docs/tutorials/usage2.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/__init__.py
--rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/py.typed
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/binding/__init__.py
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/binding/fitting.py
--rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/dil_buffer.py
--rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/dil_correction.py
--rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/fit_rpy.py
--rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/fit_titration.py
--rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/fit_titration_global.py
--rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/merge.py
--rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/plot_tecan.py
--rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/bash/fit.tecan
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/bash/fit.tecan.cl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/bash/new_sort_K.sh
--rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/bash/sum_all
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/bash/sum_e2
--rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/bash/sum_lib
--rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/bash/sum_lib2
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/bash/sum_s202n
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/bash/sum_v224q
--rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/old/bash/w_ave.sh
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/prenspire/__init__.py
--rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/prenspire/prenspire.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/prtecan/__init__.py
--rw-r--r--   0        0        0    51583 2020-02-02 00:00:00.000000 clophfit-0.5.4/src/clophfit/prtecan/prtecan.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/conftest.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/test_binding.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/test_cli.py
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/test_oldscripts.py
--rw-r--r--   0        0        0     9059 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/test_prenspire.py
--rw-r--r--   0        0        0    26589 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/test_prtecan.py
--rw-r--r--   0        0        0    34305 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/24well_clop0_95.csv
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/M1-A6-G12-nota
--rw-r--r--   0        0        0    13407 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/M1-A6-G12.csv
--rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/M1-A6-G12_11columns.csv
--rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/M1-A6-G12_missing_emptyline_fin.csv
--rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/M1-A6-G12_missing_emptyline_ini.csv
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/S202N-E2_pHs-nota
--rw-r--r--   0        0        0   832084 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/S202N-E2_pHs.csv
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/S202N-E2_pHs_nota
--rw-r--r--   0        0        0   103231 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/e2-T-without_sample_column.csv
--rw-r--r--   0        0        0   103682 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/e2dan-emwavelength.csv
--rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/e2dan-exwavelength.csv
--rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/e2dan-exwavelength2.csv
--rw-r--r--   0        0        0   104939 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/e2dan-exwavelengthstrange.csv
--rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/e2dan-with_sample_column.csv
--rw-r--r--   0        0        0   373788 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/h148g-spettroC-Efin.csv
--rw-r--r--   0        0        0   344763 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/h148g-spettroC-idx0.csv
--rw-r--r--   0        0        0   373857 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/h148g-spettroC-idx2.csv
--rw-r--r--   0        0        0   344941 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/h148g-spettroC-incomplete.csv
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/h148g-spettroC-nota
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/h148g-spettroC-nota-Err
--rw-r--r--   0        0        0   373790 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/h148g-spettroC.csv
--rw-r--r--   0        0        0    98464 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/data/NTT_37C_pKa.csv
--rw-r--r--   0        0        0    17235 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/data/output/NTT_37C_pKa_A.csv
--rw-r--r--   0        0        0    68449 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/data/output/NTT_37C_pKa_A.png
--rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/data/output/NTT_37C_pKa_B.csv
--rw-r--r--   0        0        0    53309 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/EnSpire/data/output/NTT_37C_pKa_B.png
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/290212_100.xls
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/290212_150.xls
--rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/290212_20.xls
--rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/290212_5.78.xls
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/290212_50.xls
--rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/290212_6.38.xls
--rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/290212_6.83.xls
--rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/290212_7.24.xls
--rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/290212_7.67.xls
--rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/290212_8.23.xls
--rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/290212_8.82.xls
--rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/290212_9.31.xls
--rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/290513_5.5.xls
--rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/290513_5.5_bad.xls
--rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/290513_7.2.xls
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/290513_8.8.xls
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/list.cl
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/list.cl20
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/list.pH
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/list.pH2
--rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/200214 pH data.ods
--rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/NaCl1_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/NaCl2_200214.xls
--rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/NaCl3_200214.xls
--rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/NaCl4_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/NaCl5_200214.xls
--rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/NaCl6_200214.xls
--rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/NaCl7_200214.xls
--rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/NaCl8_200214.xls
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/additions.cl
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/additions.pH
--rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/fit0-1.csv
--rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/fit0.csv
--rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/fit1-1.csv
--rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/fit1.csv
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/list.cl
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/list.pH
--rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/pH5.0_200214.xls
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/pH5.8_200214.xls
--rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/pH6.5_200214.xls
--rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/pH7.1_200214.xls
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/pH7.6_200214.xls
--rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/pH8.3_200214.xls
--rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/pH9.1_200214.xls
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/scheme.txt
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/140220/scheme0.txt
--rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
--rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
--rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/exceptions/84wells_290212_20.xlsx
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/Tecan/exceptions/88wells_290212_20.xlsx
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/A01-20140311a.dat
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/A01.dat
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/A11.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/B01.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/H04.dat
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/NTT-A04-Cl_note
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/copyIP.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/ratio2P.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/w.txt
--rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/Meas/A04 Cl_A.csv
--rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/Meas/A04 Cl_A.png
--rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/Meas/A04 Cl_B.csv
--rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/Meas/A04 Cl_B.png
--rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/Meas/A04 Cl_C.csv
--rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/Meas/A04 Cl_C.png
--rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/Meas/A04 Cl_D.csv
--rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/Meas/A04 Cl_D.png
--rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/Meas/A04 Cl_E.csv
--rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/Meas/A04 Cl_E.png
--rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/Meas/A04 Cl_F.csv
--rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/Meas/A04 Cl_F.png
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/global/Cl/A11-failed.dat
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/global/Cl/B05-20130628-cor.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/global/pH/B01-failed.dat
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/global/pH/D05.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/global/pH/H04-with_nan.dat
--rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/k/D05.dat-bs.png
--rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/k/D05.dat.png
--rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/output/global/Cl/B05-20130628-cor.dat.png
--rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.5.4/tests/data/output/global/pH/D05.dat.png
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 clophfit-0.5.4/.gitignore
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.5.4/LICENSE.txt
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 clophfit-0.5.4/README.md
--rw-r--r--   0        0        0    11299 2020-02-02 00:00:00.000000 clophfit-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 clophfit-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.6.0/.codespellrc
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.6.0/.darglint
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 clophfit-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clophfit-0.6.0/.python-version
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 clophfit-0.6.0/.readthedocs.yml
+-rw-r--r--   0        0        0    14265 2020-02-02 00:00:00.000000 clophfit-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.6.0/bandit.yml
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.6.0/cz_customize_info.txt
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 clophfit-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.6.0/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.6.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 clophfit-0.6.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 clophfit-0.6.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 clophfit-0.6.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 clophfit-0.6.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 clophfit-0.6.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 clophfit-0.6.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/11b3d3ca6e421927
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/130214ef2e6098ef
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/131670e6ccfc6715
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/137c2a14e5640dbb
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/13c057b08bc4105d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/143f69763afbd89e
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/14ef6006fe7bf2
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/153da7b0739ef260
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/15b32ca8d00f1cae
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/19aed2f50aa71c97
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/1aa8b36c402defae
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/1b15865e53162b51
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/1b65e8fbfea9c2b0
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/1c537de80aa9a708
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/1e13e710a4100651
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/1e14494c6d9d503a
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/1e530d9e2164e716
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/1e929a3c51165a4b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/1f8035ed966e729d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/209c6f89b36027d7
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/20b76a076858757c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/21478a18e28ccf0
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/21479ce58ce9b1ea
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/222a002bd0ddacdc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/2270925982073307
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/25a483a75768569b
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/25b137203afc4eb2
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/271b2778e14aec7c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/2754c3a7f152706e
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/27a21f19f32ca7ac
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/2a740dd58f392409
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/2ad457ba8563157e
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/2b75656d53abbd39
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/2bbc3ffa616f0573
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/2c35970ecaa134ff
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/2c749e556f40375e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/2c784bc662ec7472
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/2eab477da6f4caa3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/2ecb294a7d3dac76
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/2f3b5f40ae7a6145
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/2fd2b5d35c1f42f7
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/307391559bab72ed
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/30e34ca43d50547d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/31028f8eb74adbc3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/327e6f70f6a2adba
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/33292ba14e01959
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/3512497cc934b4d9
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/3514fa6e59a399a1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/3525fc7d95417df3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/35f7638cab67947e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/36690335720b4e54
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/36a808c910f29527
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/37881d82f8551c4b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/37ccf0453e74a308
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/3801732ee0426f64
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/392432e9cd90f4a2
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/39283f94c534550f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/393edb290b87ba84
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/395dc11fdf646271
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/3aebde1df74a4162
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/3bd8fb5ce7870cf8
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/3c439aef9cc78e7a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/3d1fb52780af5912
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/3daf0949a0c6e976
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/3de15ed99048c046
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/3e59a142e657b36e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/3f89549c6095afbe
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/3fae15c33f502105
+-rw-r--r--   0        0        0     8559 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/4003b7e84cad1ef3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/42975af07cb0b54d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/42e17ec0588d5df6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/42f7b0b2da7eb16f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/43be53ee4e8632c4
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/44014a485c6b8130
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/44813919a467ea5f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/44d983eb3dc20824
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/459e8e58c9b208d0
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/45fb94c37d016648
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/461f5051457515d5
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/4629cf2ae795e8ff
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/46367eaa30649063
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/4730b7ff76691413
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/47e296c4efed2f38
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/4803dd9f8aa15091
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/481422142d03d2f7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/49e4ad9927c24f2a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/4a3cc286f1b03761
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/4af493c2b7ade6bf
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/4b0423a14ffff5dc
+-rw-r--r--   0        0        0    13616 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/4b3bb844175d5460
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/4d19dbce21de5cf0
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/4d4cb0f6213adb84
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/500a1618a670eb7c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/51a7c43be5f53423
+-rw-r--r--   0        0        0    12624 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/51b41aedd47b6e08
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/5235e55280f4458
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/531231c3d64e1691
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/5335261105fc494b
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/53415e850c3a506a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/538e3d82e14b125f
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/5436d7c7197735d0
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/54a646ccdc2ee666
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/54ceb06db033fffa
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/55ef5155d524c09d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/5a3c5e8ad9b78e6f
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/5a6c44708775c3af
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/5ac0281fd7b83f4
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/5bef27648655f0c9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/5cc91c90311eae6
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/5d1b7c5f37cead12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/5deaedeefed45e0a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/5df2cee35d5aa1db
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/5e863c3703479ee9
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/5eef25476fe4366b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/5f2ea04c66b7611a
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/6021544524daaa0c
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/60a96e75f35f1b46
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/617ed545639cfaaf
+-rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/63fe04ba5f55e235
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/65684b1fd0b6aae
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/665e1527c2a9fa85
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/67115cad3a1210ac
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/67e9cfffdbe4fb50
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/68435c8794147e9d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/69ff6844eae5316e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/6a69ce0900abde7c
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/6b1363350734d33f
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/6bf7fa57745161e6
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/6c04f6a663156434
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/6cfe654778c585b9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/6d252a6765c5dc8d
+-rw-r--r--   0        0        0    13616 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/6da5273ca70e2622
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/6dba13e38320e650
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/6e043c4229b7e3d2
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/6eb67c268fc5676c
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/6ec43c4849d56e69
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/6f211d4481af07c7
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/6f64485acc5b8065
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/6f6ee8020b31272b
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/6f967e0a5dbc539b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/70022523c41801a4
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/70152a1cb521bcd4
+-rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/7044bef236a632e3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/713dda5357dafce6
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/71a28e7fc5ed25ca
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/72eb6973a92754c1
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/73739f583025bbc8
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/74833aba9e291eef
+-rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/74c9b373f03aa37a
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/74dfe3322695196f
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/753d311efc734b73
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/7617855238fb32c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/77c4adcd861129fe
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/78285987930f256d
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/78dd26fe5c04f14d
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/7934eb3ed90a9717
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/7a2d6bcf40c5f5aa
+-rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/7b2a33e13a492605
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/7b68dc476acb0d2a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/7c267407b373967
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/7cc45d6e32117dc7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/7ce043e47c9208c7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/7d520cc6250b9a21
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/7d94bdaa76989cf2
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/7df502cf0bac47d2
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/7f9d4f56fabc36f4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/7fb24e1e44fe4c49
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/7fdd4e34c4b4030
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/803bfc8b3954658c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/8067cd6e45034896
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/8161b42e883164f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/81abf497eebf13c7
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/81f603ddae43ecd3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/826d81a75395ea3b
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/82cb17f0768cc8c2
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/8348543ee757f8b7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/84a94e78fe0ddcf1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/85195458f2b5783f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/8522c88bd048378a
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/85aed5c15dea21b8
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/85dce79d20ca3c9e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/8621ef81a84bdb9f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/887f28db0bea4da4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/896ae4973f9ed291
+-rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/8987dcc79e36dd43
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/89cc13da6eacbdd4
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/8a772e48de0bf95b
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/8aa1cf97f5eabf3c
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/8bcfb3c0347fdc8
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/8cb9c5345b7f577b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/8dc46fcdd3f4f16e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/8e484178dc21ea24
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/8f33fabc18a2e686
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/8fb4c96d67962a72
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/90b4bfee6abed850
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9112e3a72fe0d305
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9180fd56ae9b7e83
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/92279322365ba61d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/92a237b33c733180
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/93e4c7b749ef954e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9422b75ca7a94f29
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/942fef8a265a580e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/951c574da1a1709a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/951d34e2b1158fcc
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/96e8fd2559c8d7d3
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/971f21e0b5d8ac62
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/98bedec99ea4ae8a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/98ecab6d4659eb5b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/98ffa21ad1ea86e1
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9a5dd5c8327daaef
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9bf7af0a33b2a57b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9c7f2bd324909d8f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9ca7f16fbe5202fc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9cf6ed2e4b8b6dee
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9d174a5c223fee10
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9d5512b6597ed9ad
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9d9952141f197de0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9de2e860d1012813
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9de77b58f1ad38ed
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9e3dc8a322e2fac5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9e4ce9d8a07275d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9e920afba46b29b7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9ec9bb87e2904db8
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9f3996baa500c32b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/9fc1e55b16eec9b5
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a048e2bbab0cbdc0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a0ad535f3ab6ef7f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a10f4d6ce7ce5ecc
+-rw-r--r--   0        0        0    12624 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a118d72cad78a66b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a1294f06e2aa1b53
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a15f87dbab73ce41
+-rw-r--r--   0        0        0    12624 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a16b26fa0bbef734
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a34a5a8a53ef5ca5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a49c9f13b22bea4e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a4a98250e312ec07
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a540537c9bdd004
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a55f267990e8ed96
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a5f767f692a29945
+-rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a6f15bb7aba11471
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a7d81c8c93906f77
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a915f0b1845620bc
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a925cda11c8d5e3a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/a957135b53c988e9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/aa7606b6a9aa8e0a
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/aaa29bca5c8ccdb7
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/aabea21e415ec0cf
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/ab2c992a23418552
+-rw-r--r--   0        0        0    12624 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/ab7294a22443b388
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/acc36669f7806de3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/ad7795bda77461e2
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/ae961bc4c4054ed2
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/aeaf25f6a57f4f42
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/aecab2f76c518138
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/aef45a3102e8dd67
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/afa32a76a440b9c7
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/b2c9ba4958d8305b
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/b30442c27e9cd5c6
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/b32eacae6df7fa74
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/b390876f875e08b0
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/b3b894737047f924
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/b50e32c4da5c1b7a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/b5f613f8b69c799a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/b77edbf8b955007d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/b7cdd11e55b2b35
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/b7f17be293b86f6b
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/b7f9b4880c2479a6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/b8ae5df5df6dab22
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/b8dbbcdba5c6c68c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/b96e7826dfe4edcf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/b985b088692fcfec
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/ba71db08f00f2f67
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/ba81fd86c27e9939
+-rw-r--r--   0        0        0    12944 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/bae2d034d964fa6f
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/bb9905cd39de626c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/bba81bb0af5f55c6
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/bc077d46ab832ce8
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/bc4592ac524c5162
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/be5760086bd0fef1
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/be8802b8695dbfd7
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/bf0476c9d8be27ad
+-rw-r--r--   0        0        0     8559 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/bf7afb751176790c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/bff14ce620508265
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/c04cfeb09b898c1f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/c068e219b99fa17c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/c094cba02b9b45df
+-rw-r--r--   0        0        0    12624 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/c12a43fb62ce2242
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/c15252c3ec90c89e
+-rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/c18d4a93b15f2660
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/c1ad91be159dc7e5
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/c2bc75b2f7dcd0d4
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/c376373a0f7fb2f4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/c3ca0f51c4a1d7b
+-rw-r--r--   0        0        0    13616 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/c4f0b0a3426699a6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/c694f9853a96633c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/c735667725016809
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/c858743ba430a1b1
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/c8c96accc4165887
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/ca22c1fbd7b6913b
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/ca30380461635e99
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/cac1a8fecd2e2b3d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/cb26749f1ac73c3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/cbeb9ad7ddc68a5f
+-rw-r--r--   0        0        0     7856 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/cd1b84fa2821fca
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/cd2b8bf3a054a800
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/ce26256dfc313ced
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/ce5212a974176f3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/ce7f1cffe58861f0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/cf3437786acbe8c5
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/cfcf3517cbb01bb0
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d034a4ec56d6875c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d0fb710933e7b90f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d1216ff8812b5551
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d16561c2cc6ff744
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d1d6ab75a58ca904
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d2039852d770db3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d2b7c592c25ee6e8
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d2dc9c42a166bb79
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d30eddcb8c705b2e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d5185aed04facb22
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d5687334e6215a7a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d56f60e77a0ca690
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d5b8ed34733ca2a8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d60ee86baf67823f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d61e3e4cb925b7b3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d7144e7cc8e8802e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d75eef610061b468
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d8e8bad368de549d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d91b54c17fce3fb5
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/d96d412141a8bbf6
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/dac39ca9321b3485
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/dae61ab7fc1bc75a
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/db2a39ee586e3c4c
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/dc357362fd22c47e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/dc7cf6cce9191030
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/dc8ef4dcdac055ad
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/de296cc597fbd464
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/de30cf9005fd51c3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/df195c4b211392de
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/df920fcd24b1ee37
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e020dd0b3cc13ae6
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e06ae0138e22b2c1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e06b8226444b724e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e225610c3255f6b8
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e279cb08a63ede23
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e34da9ab23a6bc7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e371f0650ef0c79d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e3a63e25d2d68803
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e3d63854c68fd936
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e444b52b1d832954
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e5554d584755400e
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e604e19eccb601d1
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e7de86fdb1afc0ed
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e8a2de36bc34038b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e94b09047f59633d
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e9681bb0ab0a27a2
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/e9e39580379696b1
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/ea91e9036d85968e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/eb86a77a8b27077d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/ebc290b374c8ab35
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/ee424a918cdb6c12
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/ee7ac5b5b8eb90e2
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/efa86958d966ce51
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/efca47dd8b8859ed
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/efcc16996278efd2
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/f16edf8c80fd2598
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/f19fedd607f25db9
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/f30ce1ceafcfcd05
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/f3d4a45c0820986f
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/f4248e2517e6300d
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/f4b4300bed46563a
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/f5343f64aac24573
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/f8d33e61e9bf1410
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/f905f1309b71386a
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/f90d7e9495ddc2f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/f978d9cc997fa941
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/fa7d254dd91fdae2
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/fa7f65c55980a709
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/fabad0e916c7c59f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/fb1f8a23ee1f7fd9
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/fbbe0407d2238444
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/fc3ba0f09f49a662
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/fd0acfb4f1dfd655
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/fd580933d2a85868
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/fe02efdcd64657a4
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/fe454712e21b220f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/fe5dcad7195d857f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/fe9fdaf16352660d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/febe03f07d6c5ef9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 clophfit-0.6.0/.ruff_cache/content/ff9d6a9d2c3d7081
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/Makefile
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/click.rst
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/conf.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/.gitkeep
+-rw-r--r--   0        0        0    49846 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/bs_pd_f1.png
+-rw-r--r--   0        0        0    55458 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/bs_pd_f2.png
+-rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/bs_pd_f3.png
+-rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/bs_pd_f4.png
+-rw-r--r--   0        0        0    16293 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/bs_pd_f5.png
+-rw-r--r--   0        0        0    23529 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/bs_pd_f6.png
+-rw-r--r--   0        0        0    41234 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/bs_pd_f7.png
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/csvtable.png
+-rw-r--r--   0        0        0    20158 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/emcee-01.png
+-rw-r--r--   0        0        0   109446 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/emcee-02.png
+-rw-r--r--   0        0        0    18582 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/emcee-11.png
+-rw-r--r--   0        0        0   420822 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/emcee-12.png
+-rw-r--r--   0        0        0    14293 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/f01.png
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/file.png
+-rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/gR_fit1.png
+-rw-r--r--   0        0        0    32629 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/gR_fit2.png
+-rw-r--r--   0        0        0   117478 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/gR_fit3.png
+-rw-r--r--   0        0        0    42999 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/gR_fit4.png
+-rw-r--r--   0        0        0    83505 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/gR_fit5.png
+-rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/gR_fit6.png
+-rw-r--r--   0        0        0    14823 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/gR_fit7.png
+-rw-r--r--   0        0        0    18894 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/glmfit0.png
+-rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/glmfit1.png
+-rw-r--r--   0        0        0    33541 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/glmfit2.png
+-rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/glmfit3.png
+-rw-r--r--   0        0        0    34747 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/glmfit_np.r_.png
+-rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/lmfit1.png
+-rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/lmfit2.png
+-rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/lmfit3.png
+-rw-r--r--   0        0        0    48655 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/lmfit4.png
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/lmfit5.png
+-rw-r--r--   0        0        0    21693 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/lmodel1.png
+-rw-r--r--   0        0        0    28428 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/lmodel2.png
+-rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/lmodel3.png
+-rw-r--r--   0        0        0    29389 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/lmodel4.png
+-rw-r--r--   0        0        0    23708 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/lmodel5.png
+-rw-r--r--   0        0        0   187683 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/lmodel6.png
+-rw-r--r--   0        0        0    24709 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/lmodel_H04.png
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/note_file.png
+-rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/r_bs.png
+-rw-r--r--   0        0        0    24754 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/ratio2P-lmodel1.png
+-rw-r--r--   0        0        0    63411 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/ratio2P-lmodel2.png
+-rw-r--r--   0        0        0    31838 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/ratio2P_R1.png
+-rw-r--r--   0        0        0   114443 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/ratio2P_R2.png
+-rw-r--r--   0        0        0    43555 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/ratio2P_R3.png
+-rw-r--r--   0        0        0    94094 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/ratio2P_R4.png
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/ratio2P_R5.png
+-rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/ratio2P_R6.png
+-rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/_static/rpy_bs.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/api/api.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/api/binding.rst
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/api/prenspire.rst
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/api/prtecan.rst
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/references/contributing.rst
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/references/description.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/references/development.rst
+-rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/references/older.rst
+-rw-r--r--   0        0        0   174462 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/tutorials/prenspire.ipynb
+-rw-r--r--   0        0        0  1966192 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/tutorials/prtecan.ipynb
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/tutorials/tutorials.rst
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/tutorials/usage.org
+-rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/tutorials/usage.rst
+-rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/tutorials/usage2.org
+-rw-r--r--   0        0        0    58554 2020-02-02 00:00:00.000000 clophfit-0.6.0/docs/tutorials/usage2.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/__init__.py
+-rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/py.typed
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/binding/__init__.py
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/binding/fitting.py
+-rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/dil_buffer.py
+-rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/dil_correction.py
+-rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/fit_rpy.py
+-rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/fit_titration.py
+-rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/fit_titration_global.py
+-rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/merge.py
+-rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/plot_tecan.py
+-rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/bash/fit.tecan
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/bash/fit.tecan.cl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/bash/new_sort_K.sh
+-rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/bash/sum_all
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/bash/sum_e2
+-rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/bash/sum_lib
+-rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/bash/sum_lib2
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/bash/sum_s202n
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/bash/sum_v224q
+-rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/old/bash/w_ave.sh
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/prenspire/__init__.py
+-rw-r--r--   0        0        0    17662 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/prenspire/prenspire.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/prtecan/__init__.py
+-rw-r--r--   0        0        0    51583 2020-02-02 00:00:00.000000 clophfit-0.6.0/src/clophfit/prtecan/prtecan.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/test_binding.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/test_cli.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/test_oldscripts.py
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/test_prenspire.py
+-rw-r--r--   0        0        0    26589 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/test_prtecan.py
+-rw-r--r--   0        0        0    34305 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/24well_clop0_95.csv
+-rw-r--r--   0        0        0   103231 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/e2-T-without_sample_column.csv
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/h148g-spettroC-nota
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/h148g-spettroC-nota-Err
+-rw-r--r--   0        0        0   373790 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/h148g-spettroC.csv
+-rw-r--r--   0        0        0    98464 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/cli/NTT_37C_pKa.csv
+-rw-r--r--   0        0        0    17235 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv
+-rw-r--r--   0        0        0    68449 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.png
+-rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv
+-rw-r--r--   0        0        0    53309 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.png
+-rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv
+-rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv
+-rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv
+-rw-r--r--   0        0        0   103682 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/exceptions/e2dan-emwavelength.csv
+-rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/exceptions/e2dan-exwavelength.csv
+-rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/exceptions/e2dan-exwavelength2.csv
+-rw-r--r--   0        0        0   104939 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv
+-rw-r--r--   0        0        0   344763 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv
+-rw-r--r--   0        0        0   373857 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv
+-rw-r--r--   0        0        0   344941 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/290212_100.xls
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/290212_150.xls
+-rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/290212_20.xls
+-rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/290212_5.78.xls
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/290212_50.xls
+-rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/290212_6.38.xls
+-rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/290212_6.83.xls
+-rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/290212_7.24.xls
+-rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/290212_7.67.xls
+-rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/290212_8.23.xls
+-rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/290212_8.82.xls
+-rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/290212_9.31.xls
+-rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/290513_5.5.xls
+-rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/290513_5.5_bad.xls
+-rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/290513_7.2.xls
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/290513_8.8.xls
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/list.cl
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/list.cl20
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/list.pH
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/list.pH2
+-rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/200214 pH data.ods
+-rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/NaCl1_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/NaCl2_200214.xls
+-rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/NaCl3_200214.xls
+-rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/NaCl4_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/NaCl5_200214.xls
+-rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/NaCl6_200214.xls
+-rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/NaCl7_200214.xls
+-rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/NaCl8_200214.xls
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/additions.cl
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/additions.pH
+-rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/fit0-1.csv
+-rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/fit0.csv
+-rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/fit1-1.csv
+-rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/fit1.csv
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/list.cl
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/list.pH
+-rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/pH5.0_200214.xls
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/pH5.8_200214.xls
+-rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/pH6.5_200214.xls
+-rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/pH7.1_200214.xls
+-rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/pH7.6_200214.xls
+-rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/pH8.3_200214.xls
+-rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/pH9.1_200214.xls
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/scheme.txt
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/140220/scheme0.txt
+-rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
+-rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
+-rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/exceptions/84wells_290212_20.xlsx
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/Tecan/exceptions/88wells_290212_20.xlsx
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/A01-20140311a.dat
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/A01.dat
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/A11.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/B01.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/H04.dat
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/NTT-A04-Cl_note
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/copyIP.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/ratio2P.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/w.txt
+-rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/Meas/A04 Cl_A.csv
+-rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/Meas/A04 Cl_A.png
+-rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/Meas/A04 Cl_B.csv
+-rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/Meas/A04 Cl_B.png
+-rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/Meas/A04 Cl_C.csv
+-rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/Meas/A04 Cl_C.png
+-rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/Meas/A04 Cl_D.csv
+-rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/Meas/A04 Cl_D.png
+-rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/Meas/A04 Cl_E.csv
+-rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/Meas/A04 Cl_E.png
+-rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/Meas/A04 Cl_F.csv
+-rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/Meas/A04 Cl_F.png
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/global/Cl/A11-failed.dat
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/global/Cl/B05-20130628-cor.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/global/pH/B01-failed.dat
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/global/pH/D05.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/global/pH/H04-with_nan.dat
+-rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/k/D05.dat-bs.png
+-rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/k/D05.dat.png
+-rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/output/global/Cl/B05-20130628-cor.dat.png
+-rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.6.0/tests/data/output/global/pH/D05.dat.png
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 clophfit-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 clophfit-0.6.0/README.md
+-rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 clophfit-0.6.0/PKG-INFO
```

### Comparing `clophfit-0.5.4/.pre-commit-config.yaml` & `clophfit-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/CHANGELOG.md` & `clophfit-0.6.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 <!-- markdownlint-disable MD024 -->
 <!-- vale write-good.TooWordy = NO -->
 
 # Changelog
 
+## v0.6.0 (2023-05-12)
+
+### Feat
+
+- **prenspire**: Read platemap othen than 96-well
+
+### Build
+
+- update commitizen requirement from <3.2.2 to <3.2.3 (#256)
+
 ## v0.5.4 (2023-05-11)
 
 ### Docs
 
 - Reorganize readme sphinx etc.
 
 ### Build
```

### Comparing `clophfit-0.5.4/cz_customize_info.txt` & `clophfit-0.6.0/cz_customize_info.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/.github/workflows/ci.yml` & `clophfit-0.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/.github/workflows/docs.yml` & `clophfit-0.6.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/Makefile` & `clophfit-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/conf.py` & `clophfit-0.6.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 # -- Project information -----------------------------------------------------
 
 project = "ClopHfit"
 copyright = "2023, Daniele Arosio"  # noqa: A001
 author = "Daniele Arosio"
-release = "0.5.4"
+release = "0.6.0"
 html_title = "ClopHfit"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `clophfit-0.5.4/docs/index.rst` & `clophfit-0.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/make.bat` & `clophfit-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/bs_pd_f1.png` & `clophfit-0.6.0/docs/_static/bs_pd_f1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/bs_pd_f2.png` & `clophfit-0.6.0/docs/_static/bs_pd_f2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/bs_pd_f3.png` & `clophfit-0.6.0/docs/_static/bs_pd_f3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/bs_pd_f4.png` & `clophfit-0.6.0/docs/_static/bs_pd_f4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/bs_pd_f5.png` & `clophfit-0.6.0/docs/_static/bs_pd_f5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/bs_pd_f6.png` & `clophfit-0.6.0/docs/_static/bs_pd_f6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/bs_pd_f7.png` & `clophfit-0.6.0/docs/_static/bs_pd_f7.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/csvtable.png` & `clophfit-0.6.0/docs/_static/csvtable.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/emcee-01.png` & `clophfit-0.6.0/docs/_static/emcee-01.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/emcee-02.png` & `clophfit-0.6.0/docs/_static/emcee-02.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/emcee-11.png` & `clophfit-0.6.0/docs/_static/emcee-11.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/emcee-12.png` & `clophfit-0.6.0/docs/_static/emcee-12.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/f01.png` & `clophfit-0.6.0/docs/_static/f01.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/file.png` & `clophfit-0.6.0/docs/_static/file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/gR_fit1.png` & `clophfit-0.6.0/docs/_static/gR_fit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/gR_fit2.png` & `clophfit-0.6.0/docs/_static/gR_fit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/gR_fit3.png` & `clophfit-0.6.0/docs/_static/gR_fit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/gR_fit4.png` & `clophfit-0.6.0/docs/_static/gR_fit4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/gR_fit5.png` & `clophfit-0.6.0/docs/_static/gR_fit5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/gR_fit6.png` & `clophfit-0.6.0/docs/_static/gR_fit6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/gR_fit7.png` & `clophfit-0.6.0/docs/_static/gR_fit7.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/glmfit0.png` & `clophfit-0.6.0/docs/_static/glmfit0.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/glmfit1.png` & `clophfit-0.6.0/docs/_static/glmfit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/glmfit2.png` & `clophfit-0.6.0/docs/_static/glmfit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/glmfit3.png` & `clophfit-0.6.0/docs/_static/glmfit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/glmfit_np.r_.png` & `clophfit-0.6.0/docs/_static/glmfit_np.r_.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/lmfit1.png` & `clophfit-0.6.0/docs/_static/lmfit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/lmfit2.png` & `clophfit-0.6.0/docs/_static/lmfit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/lmfit3.png` & `clophfit-0.6.0/docs/_static/lmfit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/lmfit4.png` & `clophfit-0.6.0/docs/_static/lmfit4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/lmfit5.png` & `clophfit-0.6.0/docs/_static/lmfit5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/lmodel1.png` & `clophfit-0.6.0/docs/_static/lmodel1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/lmodel2.png` & `clophfit-0.6.0/docs/_static/lmodel2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/lmodel3.png` & `clophfit-0.6.0/docs/_static/lmodel3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/lmodel4.png` & `clophfit-0.6.0/docs/_static/lmodel4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/lmodel5.png` & `clophfit-0.6.0/docs/_static/lmodel5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/lmodel6.png` & `clophfit-0.6.0/docs/_static/lmodel6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/lmodel_H04.png` & `clophfit-0.6.0/docs/_static/lmodel_H04.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/note_file.png` & `clophfit-0.6.0/docs/_static/note_file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/r_bs.png` & `clophfit-0.6.0/docs/_static/r_bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/ratio2P-lmodel1.png` & `clophfit-0.6.0/docs/_static/ratio2P-lmodel1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/ratio2P-lmodel2.png` & `clophfit-0.6.0/docs/_static/ratio2P-lmodel2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/ratio2P_R1.png` & `clophfit-0.6.0/docs/_static/ratio2P_R1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/ratio2P_R2.png` & `clophfit-0.6.0/docs/_static/ratio2P_R2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/ratio2P_R3.png` & `clophfit-0.6.0/docs/_static/ratio2P_R3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/ratio2P_R4.png` & `clophfit-0.6.0/docs/_static/ratio2P_R4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/ratio2P_R5.png` & `clophfit-0.6.0/docs/_static/ratio2P_R5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/ratio2P_R6.png` & `clophfit-0.6.0/docs/_static/ratio2P_R6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/_static/rpy_bs.png` & `clophfit-0.6.0/docs/_static/rpy_bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/references/contributing.rst` & `clophfit-0.6.0/docs/references/contributing.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/references/description.rst` & `clophfit-0.6.0/docs/references/description.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/references/older.rst` & `clophfit-0.6.0/docs/references/older.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/tutorials/prtecan.ipynb` & `clophfit-0.6.0/docs/tutorials/prtecan.ipynb`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/tutorials/usage.org` & `clophfit-0.6.0/docs/tutorials/usage.org`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/tutorials/usage.rst` & `clophfit-0.6.0/docs/tutorials/usage.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/tutorials/usage2.org` & `clophfit-0.6.0/docs/tutorials/usage2.org`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/docs/tutorials/usage2.rst` & `clophfit-0.6.0/docs/tutorials/usage2.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/src/clophfit/__main__.py` & `clophfit-0.6.0/src/clophfit/__main__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/src/clophfit/binding/fitting.py` & `clophfit-0.6.0/src/clophfit/binding/fitting.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/src/clophfit/old/dil_buffer.py` & `clophfit-0.6.0/src/clophfit/old/dil_buffer.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/src/clophfit/old/dil_correction.py` & `clophfit-0.6.0/src/clophfit/old/dil_correction.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/src/clophfit/old/fit_rpy.py` & `clophfit-0.6.0/src/clophfit/old/fit_rpy.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/src/clophfit/old/fit_titration.py` & `clophfit-0.6.0/src/clophfit/old/fit_titration.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/src/clophfit/old/fit_titration_global.py` & `clophfit-0.6.0/src/clophfit/old/fit_titration_global.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/src/clophfit/old/merge.py` & `clophfit-0.6.0/src/clophfit/old/merge.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/src/clophfit/old/plot_tecan.py` & `clophfit-0.6.0/src/clophfit/old/plot_tecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/src/clophfit/old/bash/w_ave.sh` & `clophfit-0.6.0/src/clophfit/old/bash/w_ave.sh`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/src/clophfit/prenspire/__init__.py` & `clophfit-0.6.0/src/clophfit/prenspire/__init__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/src/clophfit/prenspire/prenspire.py` & `clophfit-0.6.0/src/clophfit/prenspire/prenspire.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,71 +113,58 @@
             -------
             int
 
             """
             min_line_length = 2  # for key: value
             count = 0
             for i, line in enumerate(lines):
-                # XXX: Sometime "Sample" is absent. if line[0:1] == ["Well"]:
-                if len(line) >= min_line_length and line[:2] == ["Well", "Sample"]:
+                if len(line) >= min_line_length and line[:1] == ["Well"]:
                     count += 1
                     idx = i
             if count == 0:
-                msg = f"No line starting with ['Well', 'Sample',...] found in {lines}"
+                msg = (
+                    f"No line starting with ['Well', 'Sample',...] found in {lines[:9]}"
+                )
                 raise CsvLineError(msg)
             elif count == 1:
                 return idx
             else:  # count > 1
-                msg = f"Multiple lines starting with ['Well', 'Sample',...] in {lines}"
+                msg = f"Multiple lines starting with ['Well', 'Sample',...] in {lines[:9]}"
                 raise CsvLineError(msg)
 
         def get_list_from_platemap() -> tuple[list[str], list[list[str]]]:
-            """Get well_list from Platemap contained in metadata_post.
+            """Extract well list and Platemap from _metadata_post.
 
             Returns
             -------
-                also Platemap, at this time.
+            tuple[list[str], list[list[str]]]
+                A tuple containing:
+                - A list of well IDs in the format "A01", "A02", etc.
+                - A list of lists representing the Platemap.
 
             Raises
             ------
             CsvLineError
-                If the number of plate columns is not equal to 12.
+                If the column '01' is not present 3 lines below ['Platemap:'].
 
             """
-            lines = self._metadata_post
-            idx = line_index(lines, ["Platemap:"])
-            # XXX: 24
-            if lines[idx + 3] != [
-                "",
-                "01",
-                "02",
-                "03",
-                "04",
-                "05",
-                "06",
-                "07",
-                "08",
-                "09",
-                "10",
-                "11",
-                "12",
-                "",
-            ]:
+            lines: list[list[str]] = self._metadata_post
+            idx: int = line_index(lines, ["Platemap:"])
+            if "01" not in lines[idx + 3]:
                 msg = "stop: Platemap format unexpected"
                 raise CsvLineError(msg)
-            # XXX:
-            plate = lines[idx + 4 : idx + 12]
-            p = []
-            for r in plate:
-                letter = r[0]
-                for c in range(1, len(r)):
-                    # strip out white spaces;fix "no background info available"
-                    if r[c].strip():
-                        p.append(f"{letter}{c:02}")
-            return p, plate
+            plate: list[list[str]] = []
+            for i in range(idx + 4, len(lines)):
+                if not lines[i]:
+                    break
+                plate.append(lines[i])
+            well_list: list[str] = [
+                f"{r[0]}{c:02}" for r in plate for c in range(1, len(r)) if r[c].strip()
+            ]
+            return well_list, plate
 
         def create_metadata() -> None:
             """Create metadata dictionary."""
             self.metadata: dict[str, str | list[str]] = {}
             self.metadata[pre[1][3]] = pre[2][3]
             self.metadata[pre[1][4]] = pre[2][4]
             self.metadata[pre[1][5]] = pre[2][5]
@@ -215,15 +202,14 @@
         verboseprint("checked csv format around ini and fin")  # type: ignore
         pre = csvl[0 : self._ini - 2]  # -3
         verboseprint("saved metadata_pre attribute")  # type: ignore
         self._data_list = csvl[self._ini - 1 : self._fin]
         verboseprint("saved _data_list attribute")  # type: ignore
         self._metadata_post = csvl[self._fin + 1 :]
         verboseprint("saved metadata_post attribute")  # type: ignore
-        # XXX: 24
         self._well_list_platemap, self._platemap = get_list_from_platemap()
         verboseprint("saved _well_list_platemap attribute")  # type: ignore
         create_metadata()
         self._filename = str(file)
 
     def extract_measurements(self, verbose: int = 0) -> None:  # noqa: PLR0915
         """Extract the measurements dictionary.
@@ -332,20 +318,16 @@
                     "well_list from data_list and platemap differ. It might be you did not exported data for all acquired wells",
                     stacklevel=2,
                 )
             return True
 
         columns = [r.replace(":", "") for r in headerdata]
         dfdata = pd.DataFrame(self._data_list[1:], columns=columns)
-        # XXX: Sometime "Sample" is absent. w = df.drop_duplicates(["Well"])
-        w = dfdata.drop_duplicates(["Well", "Sample"])
+        w = dfdata.drop_duplicates(["Well"])
         self.wells = w.Well.tolist()
-        # XXX: Sometime "Sample" is absent.
-        self.samples = w.Sample.tolist()
-        # XXX: 24
         check_lists()
         # Monochromator is expected to be either Exc or Ems
         for k, v in self.measurements.items():
             label = f"Meas{k}"
             heading = namedtuple("heading", "ex em res")
             head = heading(
                 f"{label}WavelengthExc", f"{label}WavelengthEms", f"{label}Result"
```

### Comparing `clophfit-0.5.4/src/clophfit/prtecan/__init__.py` & `clophfit-0.6.0/src/clophfit/prtecan/__init__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/src/clophfit/prtecan/prtecan.py` & `clophfit-0.6.0/src/clophfit/prtecan/prtecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/test_binding.py` & `clophfit-0.6.0/tests/test_binding.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/test_cli.py` & `clophfit-0.6.0/tests/test_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,62 +7,59 @@
 import pytest
 from click.testing import CliRunner
 from matplotlib.testing.compare import compare_images  # type: ignore
 from matplotlib.testing.exceptions import ImageComparisonFailure  # type: ignore
 
 from clophfit.__main__ import clop
 
+# tests path
+tpath = Path(__file__).parent
+
 
 def test_eq1() -> None:
     """It runs XXX pr.tecan and generates correct results and graphs."""
     runner = CliRunner()
     result = runner.invoke(clop, ["eq1", "2", "2", "2"])
     assert result.exit_code == 0
     assert "4." in result.output
 
 
 def test_prenspire(tmp_path: Path) -> None:
-    """Run cli with actual data."""
-    expected = Path(__file__).parent / "EnSpire" / "data" / "output"
+    """Test prenspire command with actual data and validate output."""
+    expected = tpath / "EnSpire" / "cli" / "output"
+    input_csv = tpath / "EnSpire" / "cli" / "NTT_37C_pKa.csv"
     out = tmp_path / "E"
     out.mkdir()
     runner = CliRunner()
     result = runner.invoke(
         clop,
-        ["prenspire", "tests/EnSpire/data/NTT_37C_pKa.csv", "--out", str(out)],
+        ["prenspire", str(input_csv), "--out", str(out)],
     )
     assert result.exit_code == 0
     # validate output files
     assert (out / "NTT_37C_pKa_A.csv").exists()
     assert (out / "NTT_37C_pKa_B.csv").exists()
     assert (out / "NTT_37C_pKa_A.png").exists()
     assert (out / "NTT_37C_pKa_B.png").exists()
     # validate output file contents
     assert filecmp.cmp(out / "NTT_37C_pKa_A.csv", expected / "NTT_37C_pKa_A.csv")
     assert filecmp.cmp(out / "NTT_37C_pKa_B.csv", expected / "NTT_37C_pKa_B.csv")
     # validate graph
     for f in ["NTT_37C_pKa_A.png", "NTT_37C_pKa_B.png"]:
         msg = compare_images(out / f, expected / f, 0.0001)
-        if msg:
+        if msg:  # pragma: no cover
             raise ImageComparisonFailure(msg)
 
 
 @pytest.mark.filterwarnings("ignore:OVER")
 def test_prtecan(tmp_path: Path) -> None:
-    """It runs XXX pr.tecan and generates correct results and graphs."""
+    """Test prtecan command with actual data."""
+    lfile = str(tpath / "Tecan" / "140220" / "list.pH")
+    sfile = str(tpath / "Tecan" / "140220" / "scheme.txt")
     out = tmp_path / "out3"
     out.mkdir()
     runner = CliRunner()
     result = runner.invoke(
         clop,
-        [
-            "prtecan",
-            "tests/Tecan/140220/list.pH",
-            "--out",
-            str(out),
-            "--fit",
-            "--scheme",
-            "tests/Tecan/140220/scheme.txt",
-            "--bg",
-        ],
+        ["prtecan", lfile, "--out", str(out), "--fit", "--scheme", sfile, "--bg"],
     )
     assert result.exit_code == 0
```

### Comparing `clophfit-0.5.4/tests/test_oldscripts.py` & `clophfit-0.6.0/tests/test_oldscripts.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/test_prenspire.py` & `clophfit-0.6.0/.ruff_cache/content/4003b7e84cad1ef3`

 * *Files 27% similar despite different names*

```diff
@@ -1,567 +1,535 @@
-00000000: 2222 2254 6573 7420 7072 656e 7370 6972  """Test prenspir
-00000010: 6520 6d6f 6475 6c65 2e22 2222 0a66 726f  e module.""".fro
-00000020: 6d20 5f5f 6675 7475 7265 5f5f 2069 6d70  m __future__ imp
-00000030: 6f72 7420 616e 6e6f 7461 7469 6f6e 730a  ort annotations.
-00000040: 0a66 726f 6d20 7061 7468 6c69 6220 696d  .from pathlib im
-00000050: 706f 7274 2050 6174 680a 0a69 6d70 6f72  port Path..impor
-00000060: 7420 7079 7465 7374 0a0a 6672 6f6d 2063  t pytest..from c
-00000070: 6c6f 7068 6669 742e 7072 656e 7370 6972  lophfit.prenspir
-00000080: 6520 696d 706f 7274 2045 6e73 7069 7265  e import Enspire
-00000090: 4669 6c65 0a66 726f 6d20 636c 6f70 6866  File.from clophf
-000000a0: 6974 2e70 7265 6e73 7069 7265 2069 6d70  it.prenspire imp
-000000b0: 6f72 7420 4578 704e 6f74 650a 0a64 6174  ort ExpNote..dat
-000000c0: 615f 6669 6c65 735f 6469 7220 3d20 5061  a_files_dir = Pa
-000000d0: 7468 285f 5f66 696c 655f 5f29 2e70 6172  th(__file__).par
-000000e0: 656e 7420 2f20 2245 6e53 7069 7265 220a  ent / "EnSpire".
-000000f0: 6573 6666 203d 2064 6174 615f 6669 6c65  esff = data_file
-00000100: 735f 6469 722e 6a6f 696e 7061 7468 0a0a  s_dir.joinpath..
-00000110: 0a63 6c61 7373 2054 6573 7445 6e73 7069  .class TestEnspi
-00000120: 7265 4669 6c65 3a0a 2020 2020 2222 2254  reFile:.    """T
-00000130: 6573 7420 456e 7370 6972 6546 696c 6520  est EnspireFile 
-00000140: 636c 6173 732e 2222 220a 0a20 2020 2040  class."""..    @
-00000150: 7079 7465 7374 2e66 6978 7475 7265 2861  pytest.fixture(a
-00000160: 7574 6f75 7365 3d54 7275 6529 0a20 2020  utouse=True).   
-00000170: 2064 6566 205f 696e 6974 2873 656c 6629   def _init(self)
-00000180: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00000190: 2020 2222 2252 6561 6420 696e 2064 6174    """Read in dat
-000001a0: 6120 6669 6c65 732e 2222 220a 2020 2020  a files.""".    
-000001b0: 2020 2020 7365 6c66 2e65 7366 3120 3d20      self.esf1 = 
-000001c0: 456e 7370 6972 6546 696c 6528 6573 6666  EnspireFile(esff
-000001d0: 2822 6831 3438 672d 7370 6574 7472 6f43  ("h148g-spettroC
-000001e0: 2e63 7376 2229 290a 2020 2020 2020 2020  .csv")).        
-000001f0: 7365 6c66 2e65 7366 3220 3d20 456e 7370  self.esf2 = Ensp
-00000200: 6972 6546 696c 6528 6573 6666 2822 4d31  ireFile(esff("M1
-00000210: 2d41 362d 4731 322e 6373 7622 2929 0a20  -A6-G12.csv")). 
-00000220: 2020 2020 2020 2073 656c 662e 6573 6633         self.esf3
-00000230: 203d 2045 6e73 7069 7265 4669 6c65 2865   = EnspireFile(e
-00000240: 7366 6628 2253 3230 324e 2d45 325f 7048  sff("S202N-E2_pH
-00000250: 732e 6373 7622 2929 0a0a 2020 2020 6465  s.csv"))..    de
-00000260: 6620 7465 7374 5f65 7863 6570 7469 6f6e  f test_exception
-00000270: 7328 7365 6c66 2920 2d3e 204e 6f6e 653a  s(self) -> None:
-00000280: 0a20 2020 2020 2020 2022 2222 5465 7374  .        """Test
-00000290: 2073 6f6d 6520 7261 6973 6564 2065 7863   some raised exc
-000002a0: 6570 7469 6f6e 732e 2222 220a 2020 2020  eptions.""".    
-000002b0: 2020 2020 2320 5465 7374 2067 6574 5f64      # Test get_d
-000002c0: 6174 615f 696e 6920 4578 6365 7074 696f  ata_ini Exceptio
-000002d0: 6e73 0a20 2020 2020 2020 2077 6974 6820  ns.        with 
-000002e0: 7079 7465 7374 2e72 6169 7365 7328 4578  pytest.raises(Ex
-000002f0: 6365 7074 696f 6e2c 206d 6174 6368 3d22  ception, match="
-00000300: 4e6f 206c 696e 6520 7374 6172 7469 6e67  No line starting
-00000310: 2077 6974 6820 2e22 293a 0a20 2020 2020   with ."):.     
-00000320: 2020 2020 2020 2045 6e73 7069 7265 4669         EnspireFi
-00000330: 6c65 2865 7366 6628 2268 3134 3867 2d73  le(esff("h148g-s
-00000340: 7065 7474 726f 432d 6964 7830 2e63 7376  pettroC-idx0.csv
-00000350: 2229 290a 2020 2020 2020 2020 7769 7468  ")).        with
-00000360: 2070 7974 6573 742e 7261 6973 6573 2845   pytest.raises(E
-00000370: 7863 6570 7469 6f6e 2c20 6d61 7463 683d  xception, match=
-00000380: 224d 756c 7469 706c 6520 6c69 6e65 7320  "Multiple lines 
-00000390: 7374 6172 7469 6e67 2077 6974 6820 2e22  starting with ."
-000003a0: 293a 0a20 2020 2020 2020 2020 2020 2045  ):.            E
-000003b0: 6e73 7069 7265 4669 6c65 2865 7366 6628  nspireFile(esff(
-000003c0: 2268 3134 3867 2d73 7065 7474 726f 432d  "h148g-spettroC-
-000003d0: 6964 7832 2e63 7376 2229 290a 2020 2020  idx2.csv")).    
-000003e0: 2020 2020 2320 5465 7374 2070 6c61 7465      # Test plate
-000003f0: 6d61 700a 2020 2020 2020 2020 7769 7468  map.        with
-00000400: 2070 7974 6573 742e 7261 6973 6573 2845   pytest.raises(E
-00000410: 7863 6570 7469 6f6e 2c20 6d61 7463 683d  xception, match=
-00000420: 2273 746f 703a 2050 6c61 7465 6d61 7020  "stop: Platemap 
-00000430: 666f 726d 6174 2075 6e65 7870 6563 7465  format unexpecte
-00000440: 6422 293a 0a20 2020 2020 2020 2020 2020  d"):.           
-00000450: 2045 6e73 7069 7265 4669 6c65 2865 7366   EnspireFile(esf
-00000460: 6628 224d 312d 4136 2d47 3132 5f31 3163  f("M1-A6-G12_11c
-00000470: 6f6c 756d 6e73 2e63 7376 2229 290a 2020  olumns.csv")).  
-00000480: 2020 2020 2020 2320 5465 7374 2074 6865        # Test the
-00000490: 2070 7265 7365 6e63 6520 6f66 2073 6f6d   presence of som
-000004a0: 6520 656d 7074 7920 6c69 6e65 730a 2020  e empty lines.  
-000004b0: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
-000004c0: 742e 7261 6973 6573 2845 7863 6570 7469  t.raises(Excepti
-000004d0: 6f6e 2c20 6d61 7463 683d 2245 7870 6563  on, match="Expec
-000004e0: 7469 6e67 2074 776f 2065 6d70 7479 206c  ting two empty l
-000004f0: 696e 6573 2062 6566 6f72 6520 5f69 6e69  ines before _ini
-00000500: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00000510: 456e 7370 6972 6546 696c 6528 6573 6666  EnspireFile(esff
-00000520: 2822 4d31 2d41 362d 4731 325f 6d69 7373  ("M1-A6-G12_miss
-00000530: 696e 675f 656d 7074 796c 696e 655f 696e  ing_emptyline_in
-00000540: 692e 6373 7622 2929 0a20 2020 2020 2020  i.csv")).       
-00000550: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
-00000560: 7365 7328 4578 6365 7074 696f 6e2c 206d  ses(Exception, m
-00000570: 6174 6368 3d22 4578 7065 6374 696e 6720  atch="Expecting 
-00000580: 616e 2065 6d70 7479 206c 696e 6520 6166  an empty line af
-00000590: 7465 7220 5f66 696e 2229 3a0a 2020 2020  ter _fin"):.    
-000005a0: 2020 2020 2020 2020 456e 7370 6972 6546          EnspireF
-000005b0: 696c 6528 6573 6666 2822 4d31 2d41 362d  ile(esff("M1-A6-
-000005c0: 4731 325f 6d69 7373 696e 675f 656d 7074  G12_missing_empt
-000005d0: 796c 696e 655f 6669 6e2e 6373 7622 2929  yline_fin.csv"))
-000005e0: 0a20 2020 2020 2020 2023 2054 6573 7420  .        # Test 
-000005f0: 6d75 6c74 6970 6c65 2065 6d69 7373 696f  multiple emissio
-00000600: 6e20 7761 7665 6c65 6267 7468 7320 696e  n wavelebgths in
-00000610: 2065 7863 6974 6174 696f 6e20 7370 6563   excitation spec
-00000620: 7472 610a 2020 2020 2020 2020 7769 7468  tra.        with
-00000630: 2070 7974 6573 742e 7261 6973 6573 280a   pytest.raises(.
-00000640: 2020 2020 2020 2020 2020 2020 4578 6365              Exce
-00000650: 7074 696f 6e2c 206d 6174 6368 3d22 4578  ption, match="Ex
-00000660: 6369 7461 7469 6f6e 2073 7065 6374 7261  citation spectra
-00000670: 2077 6974 6820 756e 6578 7065 6374 6564   with unexpected
-00000680: 2065 6d69 7373 696f 6e20 696e 204d 6561   emission in Mea
-00000690: 7341 220a 2020 2020 2020 2020 293a 0a20  sA".        ):. 
-000006a0: 2020 2020 2020 2020 2020 2045 6e73 7069             Enspi
-000006b0: 7265 4669 6c65 2865 7366 6628 2265 3264  reFile(esff("e2d
-000006c0: 616e 2d65 7877 6176 656c 656e 6774 682e  an-exwavelength.
-000006d0: 6373 7622 2929 2e65 7874 7261 6374 5f6d  csv")).extract_m
-000006e0: 6561 7375 7265 6d65 6e74 7328 290a 2020  easurements().  
-000006f0: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
-00000700: 742e 7261 6973 6573 280a 2020 2020 2020  t.raises(.      
-00000710: 2020 2020 2020 4578 6365 7074 696f 6e2c        Exception,
-00000720: 206d 6174 6368 3d22 4578 6369 7461 7469   match="Excitati
-00000730: 6f6e 2073 7065 6374 7261 2077 6974 6820  on spectra with 
-00000740: 756e 6578 7065 6374 6564 2065 6d69 7373  unexpected emiss
-00000750: 696f 6e20 696e 204d 6561 7341 220a 2020  ion in MeasA".  
-00000760: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-00000770: 2020 2020 2045 6e73 7069 7265 4669 6c65       EnspireFile
-00000780: 2865 7366 6628 2265 3264 616e 2d65 7877  (esff("e2dan-exw
-00000790: 6176 656c 656e 6774 6832 2e63 7376 2229  avelength2.csv")
-000007a0: 292e 6578 7472 6163 745f 6d65 6173 7572  ).extract_measur
-000007b0: 656d 656e 7473 2829 0a20 2020 2020 2020  ements().       
-000007c0: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
-000007d0: 7365 7328 0a20 2020 2020 2020 2020 2020  ses(.           
-000007e0: 2045 7863 6570 7469 6f6e 2c20 6d61 7463   Exception, matc
-000007f0: 683d 2245 6d69 7373 696f 6e20 7370 6563  h="Emission spec
-00000800: 7472 6120 7769 7468 2075 6e65 7870 6563  tra with unexpec
-00000810: 7465 6420 6578 6369 7461 7469 6f6e 2069  ted excitation i
-00000820: 6e20 4d65 6173 4322 0a20 2020 2020 2020  n MeasC".       
-00000830: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-00000840: 456e 7370 6972 6546 696c 6528 6573 6666  EnspireFile(esff
-00000850: 2822 6532 6461 6e2d 656d 7761 7665 6c65  ("e2dan-emwavele
-00000860: 6e67 7468 2e63 7376 2229 292e 6578 7472  ngth.csv")).extr
-00000870: 6163 745f 6d65 6173 7572 656d 656e 7473  act_measurements
-00000880: 2829 0a20 2020 2020 2020 2077 6974 6820  ().        with 
-00000890: 7079 7465 7374 2e72 6169 7365 7328 0a20  pytest.raises(. 
-000008a0: 2020 2020 2020 2020 2020 2045 7863 6570             Excep
-000008b0: 7469 6f6e 2c20 6d61 7463 683d 2755 6e6b  tion, match='Unk
-000008c0: 6e6f 776e 2022 4d6f 6e6f 6368 726f 6d61  nown "Monochroma
-000008d0: 746f 7222 3a20 5374 7261 6e67 6520 696e  tor": Strange in
-000008e0: 204d 6561 7342 270a 2020 2020 2020 2020   MeasB'.        
-000008f0: 293a 0a20 2020 2020 2020 2020 2020 2045  ):.            E
-00000900: 6e73 7069 7265 4669 6c65 2865 7366 6628  nspireFile(esff(
-00000910: 2265 3264 616e 2d65 7877 6176 656c 656e  "e2dan-exwavelen
-00000920: 6774 6873 7472 616e 6765 2e63 7376 2229  gthstrange.csv")
-00000930: 292e 6578 7472 6163 745f 6d65 6173 7572  ).extract_measur
-00000940: 656d 656e 7473 2829 0a0a 2020 2020 6465  ements()..    de
-00000950: 6620 7465 7374 5f67 6574 5f64 6174 615f  f test_get_data_
-00000960: 696e 6928 7365 6c66 2920 2d3e 204e 6f6e  ini(self) -> Non
-00000970: 653a 0a20 2020 2020 2020 2022 2222 5465  e:.        """Te
-00000980: 7374 2067 6574 5f64 6174 615f 696e 692e  st get_data_ini.
-00000990: 2222 220a 2020 2020 2020 2020 6173 7365  """.        asse
-000009a0: 7274 2073 656c 662e 6573 6631 2e5f 696e  rt self.esf1._in
-000009b0: 6920 3d3d 2031 320a 2020 2020 2020 2020  i == 12.        
-000009c0: 6173 7365 7274 2073 656c 662e 6573 6632  assert self.esf2
-000009d0: 2e5f 696e 6920 3d3d 2039 0a20 2020 2020  ._ini == 9.     
-000009e0: 2020 2061 7373 6572 7420 7365 6c66 2e65     assert self.e
-000009f0: 7366 332e 5f69 6e69 203d 3d20 390a 0a20  sf3._ini == 9.. 
-00000a00: 2020 2064 6566 2074 6573 745f 6669 6e28     def test_fin(
-00000a10: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00000a20: 2020 2020 2020 2022 2222 5465 7374 205f         """Test _
-00000a30: 6669 6e20 286c 696e 655f 696e 6465 7828  fin (line_index(
-00000a40: 2929 2e22 2222 0a20 2020 2020 2020 2023  )).""".        #
-00000a50: 2052 656d 656d 6265 7220 7468 6174 2066   Remember that f
-00000a60: 6972 7374 206c 696e 6520 6861 7320 696e  irst line has in
-00000a70: 6465 783d 300a 2020 2020 2020 2020 6173  dex=0.        as
-00000a80: 7365 7274 2073 656c 662e 6573 6631 2e5f  sert self.esf1._
-00000a90: 6669 6e20 3d3d 2031 3438 3937 0a20 2020  fin == 14897.   
-00000aa0: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-00000ab0: 2e65 7366 322e 5f66 696e 203d 3d20 3436  .esf2._fin == 46
-00000ac0: 310a 2020 2020 2020 2020 6173 7365 7274  1.        assert
-00000ad0: 2073 656c 662e 6573 6633 2e5f 6669 6e20   self.esf3._fin 
-00000ae0: 3d3d 2037 3233 330a 0a20 2020 2064 6566  == 7233..    def
-00000af0: 2074 6573 745f 6d65 7461 6461 7461 5f70   test_metadata_p
-00000b00: 6f73 7428 7365 6c66 2920 2d3e 204e 6f6e  ost(self) -> Non
-00000b10: 653a 0a20 2020 2020 2020 2022 2222 4964  e:.        """Id
-00000b20: 656e 7469 6679 2063 6f72 7265 6374 6c79  entify correctly
-00000b30: 2074 6865 2062 6567 696e 6e69 6e67 206f   the beginning o
-00000b40: 6620 6d65 7461 6461 7461 2061 6674 6572  f metadata after
-00000b50: 2064 6174 6120 626c 6f63 6b2e 2222 220a   data block.""".
-00000b60: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00000b70: 656c 662e 6573 6631 2e5f 6d65 7461 6461  elf.esf1._metada
-00000b80: 7461 5f70 6f73 745b 305d 203d 3d20 5b22  ta_post[0] == ["
-00000b90: 4261 7369 6320 6173 7361 7920 696e 666f  Basic assay info
-00000ba0: 726d 6174 696f 6e20 225d 0a20 2020 2020  rmation "].     
-00000bb0: 2020 2061 7373 6572 7420 7365 6c66 2e65     assert self.e
-00000bc0: 7366 322e 5f6d 6574 6164 6174 615f 706f  sf2._metadata_po
-00000bd0: 7374 5b30 5d20 3d3d 205b 2242 6173 6963  st[0] == ["Basic
-00000be0: 2061 7373 6179 2069 6e66 6f72 6d61 7469   assay informati
-00000bf0: 6f6e 2022 5d0a 2020 2020 2020 2020 6173  on "].        as
-00000c00: 7365 7274 2073 656c 662e 6573 6633 2e5f  sert self.esf3._
-00000c10: 6d65 7461 6461 7461 5f70 6f73 745b 305d  metadata_post[0]
-00000c20: 203d 3d20 5b22 4261 7369 6320 6173 7361   == ["Basic assa
-00000c30: 7920 696e 666f 726d 6174 696f 6e20 225d  y information "]
-00000c40: 0a0a 2020 2020 6465 6620 7465 7374 5f6c  ..    def test_l
-00000c50: 6f63 616c 6567 656e 5f69 6e5f 6d65 7461  ocalegen_in_meta
-00000c60: 6461 7461 5f70 6f73 7428 7365 6c66 2920  data_post(self) 
-00000c70: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00000c80: 2022 2222 5465 7374 206c 6f63 616c 6573   """Test locales
-00000c90: 2e22 2222 0a20 2020 2020 2020 2061 7373  .""".        ass
-00000ca0: 6572 7420 7365 6c66 2e65 7366 312e 5f6d  ert self.esf1._m
-00000cb0: 6574 6164 6174 615f 706f 7374 5b33 315d  etadata_post[31]
-00000cc0: 5b34 5d20 3d3d 2022 3330 3020 c2b5 6c22  [4] == "300 ..l"
-00000cd0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00000ce0: 7365 6c66 2e65 7366 322e 5f6d 6574 6164  self.esf2._metad
-00000cf0: 6174 615f 706f 7374 5b33 315d 5b34 5d20  ata_post[31][4] 
-00000d00: 3d3d 2022 3330 3020 c2b5 6c22 0a20 2020  == "300 ..l".   
-00000d10: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-00000d20: 2e65 7366 332e 5f6d 6574 6164 6174 615f  .esf3._metadata_
-00000d30: 706f 7374 5b33 315d 5b34 5d20 3d3d 2022  post[31][4] == "
-00000d40: 3330 3020 c2b5 6c22 0a0a 2020 2020 6465  300 ..l"..    de
-00000d50: 6620 7465 7374 5f64 6174 615f 6c69 7374  f test_data_list
-00000d60: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00000d70: 2020 2020 2020 2020 2222 2254 6573 7420          """Test 
-00000d80: 6461 7461 5f6c 6973 742e 2222 220a 2020  data_list.""".  
-00000d90: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
-00000da0: 662e 6573 6631 2e5f 6461 7461 5f6c 6973  f.esf1._data_lis
-00000db0: 745b 305d 5b32 5d20 3d3d 2022 4d65 6173  t[0][2] == "Meas
-00000dc0: 413a 5265 7375 6c74 220a 2020 2020 2020  A:Result".      
-00000dd0: 2020 6173 7365 7274 2073 656c 662e 6573    assert self.es
-00000de0: 6632 2e5f 6461 7461 5f6c 6973 745b 305d  f2._data_list[0]
-00000df0: 5b32 5d20 3d3d 2022 4d65 6173 413a 5761  [2] == "MeasA:Wa
-00000e00: 7665 6c65 6e67 7468 4578 6322 0a20 2020  velengthExc".   
-00000e10: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-00000e20: 2e65 7366 332e 5f64 6174 615f 6c69 7374  .esf3._data_list
-00000e30: 5b30 5d5b 325d 203d 3d20 224d 6561 7341  [0][2] == "MeasA
-00000e40: 3a52 6573 756c 7422 0a20 2020 2020 2020  :Result".       
-00000e50: 2061 7373 6572 7420 7365 6c66 2e65 7366   assert self.esf
-00000e60: 312e 5f64 6174 615f 6c69 7374 5b31 5d5b  1._data_list[1][
-00000e70: 325d 203d 3d20 2233 3135 3122 0a20 2020  2] == "3151".   
-00000e80: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-00000e90: 2e65 7366 322e 5f64 6174 615f 6c69 7374  .esf2._data_list
-00000ea0: 5b31 5d5b 345d 203d 3d20 2236 3639 3533  [1][4] == "66953
-00000eb0: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
-00000ec0: 2073 656c 662e 6573 6633 2e5f 6461 7461   self.esf3._data
-00000ed0: 5f6c 6973 745b 315d 5b32 5d20 3d3d 2022  _list[1][2] == "
-00000ee0: 3735 3034 220a 2020 2020 2020 2020 2320  7504".        # 
-00000ef0: 496d 706f 7274 616e 7420 746f 2063 6865  Important to che
-00000f00: 636b 2066 6f72 206c 6173 7420 6c69 6e65  ck for last line
-00000f10: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00000f20: 7365 6c66 2e65 7366 312e 5f64 6174 615f  self.esf1._data_
-00000f30: 6c69 7374 5b2d 315d 5b32 5d20 3d3d 2022  list[-1][2] == "
-00000f40: 3937 3631 3222 0a20 2020 2020 2020 2061  97612".        a
-00000f50: 7373 6572 7420 7365 6c66 2e65 7366 322e  ssert self.esf2.
-00000f60: 5f64 6174 615f 6c69 7374 5b2d 315d 5b34  _data_list[-1][4
-00000f70: 5d20 3d3d 2022 3339 3933 220a 2020 2020  ] == "3993".    
-00000f80: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
-00000f90: 6573 6633 2e5f 6461 7461 5f6c 6973 745b  esf3._data_list[
-00000fa0: 2d31 5d5b 325d 203d 3d20 2231 3738 3522  -1][2] == "1785"
-00000fb0: 0a0a 2020 2020 6465 6620 7465 7374 5f67  ..    def test_g
-00000fc0: 6574 5f6c 6973 745f 6672 6f6d 5f70 6c61  et_list_from_pla
-00000fd0: 7465 6d61 7028 7365 6c66 2920 2d3e 204e  temap(self) -> N
-00000fe0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00000ff0: 5465 7374 206c 6973 7420 6672 6f6d 2070  Test list from p
-00001000: 6c61 7465 6d61 702e 2222 220a 2020 2020  latemap.""".    
-00001010: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
-00001020: 6573 6631 2e5f 7765 6c6c 5f6c 6973 745f  esf1._well_list_
-00001030: 706c 6174 656d 6170 5b32 5d20 3d3d 2022  platemap[2] == "
-00001040: 4130 3322 0a20 2020 2020 2020 2061 7373  A03".        ass
-00001050: 6572 7420 7365 6c66 2e65 7366 322e 5f77  ert self.esf2._w
-00001060: 656c 6c5f 6c69 7374 5f70 6c61 7465 6d61  ell_list_platema
-00001070: 705b 315d 203d 3d20 2248 3132 220a 2020  p[1] == "H12".  
-00001080: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
-00001090: 662e 6573 6633 2e5f 7765 6c6c 5f6c 6973  f.esf3._well_lis
-000010a0: 745f 706c 6174 656d 6170 5b32 5d20 3d3d  t_platemap[2] ==
-000010b0: 2022 4130 3322 0a0a 2020 2020 6465 6620   "A03"..    def 
-000010c0: 7465 7374 5f6d 6574 6164 6174 6128 7365  test_metadata(se
-000010d0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-000010e0: 2020 2020 2022 2222 5465 7374 206d 6574       """Test met
-000010f0: 6164 6174 6120 6469 6374 696f 6e61 7279  adata dictionary
-00001100: 2e22 2222 0a20 2020 2020 2020 2061 7373  .""".        ass
-00001110: 6572 7420 7365 6c66 2e65 7366 332e 6d65  ert self.esf3.me
-00001120: 7461 6461 7461 5b22 4d65 6173 7572 656d  tadata["Measurem
-00001130: 656e 7420 6461 7465 225d 203d 3d20 2232  ent date"] == "2
-00001140: 3031 332d 3036 2d31 3420 3233 3a31 333a  013-06-14 23:13:
-00001150: 3531 220a 2020 2020 2020 2020 6173 7365  51".        asse
-00001160: 7274 2073 656c 662e 6573 6633 2e6d 6574  rt self.esf3.met
-00001170: 6164 6174 615b 2243 6861 6d62 6572 2074  adata["Chamber t
-00001180: 656d 7065 7261 7475 7265 2061 7420 7374  emperature at st
-00001190: 6172 7422 5d20 3d3d 2022 3139 2e35 3522  art"] == "19.55"
-000011a0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000011b0: 7365 6c66 2e65 7366 332e 6d65 7461 6461  self.esf3.metada
-000011c0: 7461 5b22 4368 616d 6265 7220 7465 6d70  ta["Chamber temp
-000011d0: 6572 6174 7572 6520 6174 2065 6e64 225d  erature at end"]
-000011e0: 203d 3d20 2233 362e 3522 0a20 2020 2020   == "36.5".     
-000011f0: 2020 2061 7373 6572 7420 7365 6c66 2e65     assert self.e
-00001200: 7366 332e 6d65 7461 6461 7461 5b22 416d  sf3.metadata["Am
-00001210: 6269 656e 7420 7465 6d70 6572 6174 7572  bient temperatur
-00001220: 6520 6174 2073 7461 7274 225d 203d 3d20  e at start"] == 
-00001230: 2234 2e37 220a 2020 2020 2020 2020 6173  "4.7".        as
-00001240: 7365 7274 2073 656c 662e 6573 6633 2e6d  sert self.esf3.m
-00001250: 6574 6164 6174 615b 2241 6d62 6965 6e74  etadata["Ambient
-00001260: 2074 656d 7065 7261 7475 7265 2061 7420   temperature at 
-00001270: 656e 6422 5d20 3d3d 2022 382e 3422 0a20  end"] == "8.4". 
-00001280: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
-00001290: 6c66 2e65 7366 312e 6d65 7461 6461 7461  lf.esf1.metadata
-000012a0: 5b22 5072 6f74 6f63 6f6c 206e 616d 6522  ["Protocol name"
-000012b0: 5d20 3d3d 2022 4563 6369 7461 7a69 6f6e  ] == "Eccitazion
-000012c0: 6520 4322 0a20 2020 2020 2020 2061 7373  e C".        ass
-000012d0: 6572 7420 280a 2020 2020 2020 2020 2020  ert (.          
-000012e0: 2020 7365 6c66 2e65 7366 312e 6d65 7461    self.esf1.meta
-000012f0: 6461 7461 5b22 4578 706f 7274 6564 2064  data["Exported d
-00001300: 6174 6122 5d0a 2020 2020 2020 2020 2020  ata"].          
-00001310: 2020 3d3d 2022 5765 6c6c 2c53 616d 706c    == "Well,Sampl
-00001320: 652c 4d65 6173 413a 5265 7375 6c74 2c4d  e,MeasA:Result,M
-00001330: 6561 7341 3a57 6176 656c 656e 6774 6822  easA:Wavelength"
-00001340: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00001350: 6465 6620 7465 7374 5f6d 6561 7375 7265  def test_measure
-00001360: 6d65 6e74 5f6d 6574 6164 6174 6128 7365  ment_metadata(se
-00001370: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00001380: 2020 2020 2022 2222 5465 7374 2064 6174       """Test dat
-00001390: 6120 6f62 6a65 6374 2e22 2222 0a20 2020  a object.""".   
-000013a0: 2020 2020 2073 656c 662e 6573 6633 2e65       self.esf3.e
-000013b0: 7874 7261 6374 5f6d 6561 7375 7265 6d65  xtract_measureme
-000013c0: 6e74 7328 290a 2020 2020 2020 2020 6173  nts().        as
-000013d0: 7365 7274 2073 656c 662e 6573 6633 2e6d  sert self.esf3.m
-000013e0: 6561 7375 7265 6d65 6e74 735b 2247 225d  easurements["G"]
-000013f0: 5b22 6d65 7461 6461 7461 225d 5b22 4d6f  ["metadata"]["Mo
-00001400: 6e6f 6368 726f 6d61 746f 7222 5d20 3d3d  nochromator"] ==
-00001410: 2022 4578 6369 7461 7469 6f6e 220a 2020   "Excitation".  
-00001420: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
-00001430: 662e 6573 6633 2e6d 6561 7375 7265 6d65  f.esf3.measureme
-00001440: 6e74 735b 2247 225d 5b22 6d65 7461 6461  nts["G"]["metada
-00001450: 7461 225d 5b22 5761 7665 6c65 6e67 7468  ta"]["Wavelength
-00001460: 225d 203d 3d20 2235 3335 220a 2020 2020  "] == "535".    
-00001470: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
-00001480: 6573 6633 2e6d 6561 7375 7265 6d65 6e74  esf3.measurement
-00001490: 735b 2247 225d 5b22 6d65 7461 6461 7461  s["G"]["metadata
-000014a0: 225d 5b22 7465 6d70 225d 203d 3d20 2233  "]["temp"] == "3
-000014b0: 3722 0a20 2020 2020 2020 2061 7373 6572  7".        asser
-000014c0: 7420 7365 6c66 2e65 7366 332e 6d65 6173  t self.esf3.meas
-000014d0: 7572 656d 656e 7473 5b22 4122 5d5b 226d  urements["A"]["m
-000014e0: 6574 6164 6174 6122 5d5b 224d 6f6e 6f63  etadata"]["Monoc
-000014f0: 6872 6f6d 6174 6f72 225d 203d 3d20 2245  hromator"] == "E
-00001500: 6d69 7373 696f 6e22 0a20 2020 2020 2020  mission".       
-00001510: 2061 7373 6572 7420 7365 6c66 2e65 7366   assert self.esf
-00001520: 332e 6d65 6173 7572 656d 656e 7473 5b22  3.measurements["
-00001530: 4122 5d5b 226d 6574 6164 6174 6122 5d5b  A"]["metadata"][
-00001540: 2257 6176 656c 656e 6774 6822 5d20 3d3d  "Wavelength"] ==
-00001550: 2022 3237 3822 0a20 2020 2020 2020 2061   "278".        a
-00001560: 7373 6572 7420 7365 6c66 2e65 7366 332e  ssert self.esf3.
-00001570: 6d65 6173 7572 656d 656e 7473 5b22 4122  measurements["A"
-00001580: 5d5b 226d 6574 6164 6174 6122 5d5b 2274  ]["metadata"]["t
-00001590: 656d 7022 5d20 3d3d 2022 3230 220a 0a20  emp"] == "20".. 
-000015a0: 2020 2064 6566 2074 6573 745f 6d65 6173     def test_meas
-000015b0: 7572 656d 656e 7473 2873 656c 6629 202d  urements(self) -
-000015c0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000015d0: 2222 2254 6573 7420 6461 7461 206f 626a  """Test data obj
-000015e0: 6563 742e 2222 220a 2020 2020 2020 2020  ect.""".        
-000015f0: 7365 6c66 2e65 7366 312e 6578 7472 6163  self.esf1.extrac
-00001600: 745f 6d65 6173 7572 656d 656e 7473 2829  t_measurements()
-00001610: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00001620: 7365 6c66 2e65 7366 312e 6d65 6173 7572  self.esf1.measur
-00001630: 656d 656e 7473 5b22 4122 5d5b 226c 616d  ements["A"]["lam
-00001640: 6264 6122 5d5b 305d 203d 3d20 3237 320a  bda"][0] == 272.
-00001650: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00001660: 656c 662e 6573 6631 2e6d 6561 7375 7265  elf.esf1.measure
-00001670: 6d65 6e74 735b 2241 225d 5b22 6c61 6d62  ments["A"]["lamb
-00001680: 6461 225d 5b32 3238 5d20 3d3d 2035 3030  da"][228] == 500
-00001690: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000016a0: 7365 6c66 2e65 7366 312e 6d65 6173 7572  self.esf1.measur
-000016b0: 656d 656e 7473 5b22 4122 5d5b 2241 3031  ements["A"]["A01
-000016c0: 225d 5b30 5d20 3d3d 2033 3135 310a 2020  "][0] == 3151.  
-000016d0: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
-000016e0: 662e 6573 6631 2e6d 6561 7375 7265 6d65  f.esf1.measureme
-000016f0: 6e74 735b 2241 225d 5b22 4130 3122 5d5b  nts["A"]["A01"][
-00001700: 3232 385d 203d 3d20 3537 330a 2020 2020  228] == 573.    
-00001710: 2020 2020 2320 496d 706f 7274 616e 7420      # Important 
-00001720: 746f 2063 6865 636b 2066 6f72 206c 6173  to check for las
-00001730: 7420 6c69 6e65 206f 6620 6373 766c 0a20  t line of csvl. 
-00001740: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
-00001750: 6c66 2e65 7366 312e 6d65 6173 7572 656d  lf.esf1.measurem
-00001760: 656e 7473 5b22 4122 5d5b 2247 3035 225d  ents["A"]["G05"]
-00001770: 5b32 3238 5d20 3d3d 2039 3736 3132 0a20  [228] == 97612. 
-00001780: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
-00001790: 6c66 2e65 7366 312e 6d65 6173 7572 656d  lf.esf1.measurem
-000017a0: 656e 7473 5b22 4122 5d5b 2241 3031 225d  ents["A"]["A01"]
-000017b0: 5b31 305d 203d 3d20 3234 3936 0a20 2020  [10] == 2496.   
-000017c0: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-000017d0: 2e65 7366 312e 6d65 6173 7572 656d 656e  .esf1.measuremen
-000017e0: 7473 5b22 4122 5d5b 2241 3032 225d 5b31  ts["A"]["A02"][1
-000017f0: 305d 203d 3d20 3137 3635 0a20 2020 2020  0] == 1765.     
-00001800: 2020 2061 7373 6572 7420 7365 6c66 2e65     assert self.e
-00001810: 7366 312e 6d65 6173 7572 656d 656e 7473  sf1.measurements
-00001820: 5b22 4122 5d5b 226c 616d 6264 6122 5d5b  ["A"]["lambda"][
-00001830: 3130 5d20 3d3d 2032 3832 0a20 2020 2020  10] == 282.     
-00001840: 2020 2061 7373 6572 7420 7365 6c66 2e65     assert self.e
-00001850: 7366 312e 6d65 6173 7572 656d 656e 7473  sf1.measurements
-00001860: 5b22 4122 5d5b 226d 6574 6164 6174 6122  ["A"]["metadata"
-00001870: 5d5b 2257 6176 656c 656e 6774 6822 5d20  ]["Wavelength"] 
-00001880: 3d3d 2022 3532 3022 0a20 2020 2020 2020  == "520".       
-00001890: 2073 656c 662e 6573 6632 2e65 7874 7261   self.esf2.extra
-000018a0: 6374 5f6d 6561 7375 7265 6d65 6e74 7328  ct_measurements(
-000018b0: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-000018c0: 2073 656c 662e 6573 6632 2e6d 6561 7375   self.esf2.measu
-000018d0: 7265 6d65 6e74 735b 2241 225d 5b22 6c61  rements["A"]["la
-000018e0: 6d62 6461 225d 5b32 5d20 3d3d 2032 3732  mbda"][2] == 272
-000018f0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00001900: 7365 6c66 2e65 7366 322e 6d65 6173 7572  self.esf2.measur
-00001910: 656d 656e 7473 5b22 4122 5d5b 2247 3132  ements["A"]["G12
-00001920: 225d 5b30 5d20 3d3d 2036 3639 3533 0a20  "][0] == 66953. 
-00001930: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
-00001940: 6c66 2e65 7366 322e 6d65 6173 7572 656d  lf.esf2.measurem
-00001950: 656e 7473 5b22 4122 5d5b 226d 6574 6164  ents["A"]["metad
-00001960: 6174 6122 5d5b 2257 6176 656c 656e 6774  ata"]["Wavelengt
-00001970: 6822 5d20 3d3d 2022 3531 3522 0a0a 2020  h"] == "515"..  
-00001980: 2020 2320 4075 6e69 7474 6573 742e 736b    # @unittest.sk
-00001990: 6970 2822 6465 6d6f 6e73 7472 6174 696e  ip("demonstratin
-000019a0: 6720 736b 6970 7069 6e67 2229 0a20 2020  g skipping").   
-000019b0: 2064 6566 2074 6573 745f 6368 6563 6b5f   def test_check_
-000019c0: 6c69 7374 735f 7761 726e 696e 6728 7365  lists_warning(se
-000019d0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-000019e0: 2020 2020 2022 2222 4974 2077 6172 6e73       """It warns
-000019f0: 2077 6865 6e20 2863 7376 2021 3d20 706c   when (csv != pl
-00001a00: 6174 656d 6170 292e 0a0a 2020 2020 2020  atemap)...      
-00001a10: 2020 2a2d 696e 636f 6d70 6c65 7465 2e63    *-incomplete.c
-00001a20: 7376 3a20 3520 7765 6c6c 7320 2847 312d  sv: 5 wells (G1-
-00001a30: 4735 2920 6172 6520 6d69 7373 696e 672e  G5) are missing.
-00001a40: 2028 5468 6579 2061 7265 2070 7265 7365   (They are prese
-00001a50: 6e74 2069 6e0a 2020 2020 2020 2020 506c  nt in.        Pl
-00001a60: 6174 656d 6170 2062 6563 6175 7365 2074  atemap because t
-00001a70: 6865 7920 7765 7265 2070 7265 7365 6e74  hey were present
-00001a80: 2064 7572 696e 6720 6163 7175 6973 6974   during acquisit
-00001a90: 696f 6e20 616e 6420 7468 656e 206e 6f74  ion and then not
-00001aa0: 0a20 2020 2020 2020 2065 7870 6f72 7465  .        exporte
-00001ab0: 6429 2e0a 0a20 2020 2020 2020 2022 2222  d)...        """
-00001ac0: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00001ad0: 7761 726e 696e 6773 0a0a 2020 2020 2020  warnings..      
-00001ae0: 2020 7769 7468 2077 6172 6e69 6e67 732e    with warnings.
-00001af0: 6361 7463 685f 7761 726e 696e 6773 2872  catch_warnings(r
-00001b00: 6563 6f72 643d 5472 7565 2920 6173 2077  ecord=True) as w
-00001b10: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00001b20: 4361 7573 6520 616c 6c20 7761 726e 696e  Cause all warnin
-00001b30: 6773 2074 6f20 616c 7761 7973 2062 6520  gs to always be 
-00001b40: 7472 6967 6765 7265 642e 0a20 2020 2020  triggered..     
-00001b50: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
-00001b60: 7369 6d70 6c65 6669 6c74 6572 2822 616c  simplefilter("al
-00001b70: 7761 7973 2229 0a20 2020 2020 2020 2020  ways").         
-00001b80: 2020 2065 6620 3d20 456e 7370 6972 6546     ef = EnspireF
-00001b90: 696c 6528 6573 6666 2822 6831 3438 672d  ile(esff("h148g-
-00001ba0: 7370 6574 7472 6f43 2d69 6e63 6f6d 706c  spettroC-incompl
-00001bb0: 6574 652e 6373 7622 2929 0a20 2020 2020  ete.csv")).     
-00001bc0: 2020 2020 2020 2065 662e 6578 7472 6163         ef.extrac
-00001bd0: 745f 6d65 6173 7572 656d 656e 7473 2829  t_measurements()
-00001be0: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00001bf0: 6572 7420 6c65 6e28 7729 203d 3d20 320a  ert len(w) == 2.
-00001c00: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00001c10: 7274 2069 7373 7562 636c 6173 7328 775b  rt issubclass(w[
-00001c20: 2d31 5d2e 6361 7465 676f 7279 2c20 5761  -1].category, Wa
-00001c30: 726e 696e 6729 0a20 2020 2020 2020 2020  rning).         
-00001c40: 2020 2061 7373 6572 7420 2270 6c61 7465     assert "plate
-00001c50: 6d61 7022 2069 6e20 7374 7228 775b 2d31  map" in str(w[-1
-00001c60: 5d2e 6d65 7373 6167 6529 0a0a 2020 2020  ].message)..    
-00001c70: 2320 706c 6163 656d 6172 6b20 6465 6620  # placemark def 
-00001c80: 7465 7374 5f67 6574 5f6d 6178 7828 7365  test_get_maxx(se
-00001c90: 6c66 293a 0a20 2020 2023 2070 6c61 6365  lf):.    # place
-00001ca0: 6d61 726b 2020 2020 2272 6561 6c6c 7920  mark    "really 
-00001cb0: 6e65 6564 2074 6f20 6265 2063 6f6d 706c  need to be compl
-00001cc0: 6574 6564 220a 2020 2020 2320 706c 6163  eted".    # plac
-00001cd0: 656d 6172 6b20 2020 2073 656c 662e 6173  emark    self.as
-00001ce0: 7365 7274 4571 7561 6c28 7365 6c66 2e73  sertEqual(self.s
-00001cf0: 2e67 6574 5f6d 6178 7828 7365 6c66 2e73  .get_maxx(self.s
-00001d00: 2e65 782c 2073 656c 662e 732e 7929 2c20  .ex, self.s.y), 
-00001d10: 3237 3229 0a0a 0a63 6c61 7373 2054 6573  272)...class Tes
-00001d20: 7445 7870 4e6f 7465 3a0a 2020 2020 2222  tExpNote:.    ""
-00001d30: 2245 7870 6572 696d 656e 7461 6c20 6e6f  "Experimental no
-00001d40: 7465 732e 2222 220a 0a20 2020 2040 7079  tes."""..    @py
-00001d50: 7465 7374 2e66 6978 7475 7265 2861 7574  test.fixture(aut
-00001d60: 6f75 7365 3d54 7275 6529 0a20 2020 2064  ouse=True).    d
-00001d70: 6566 205f 696e 6974 2873 656c 6629 202d  ef _init(self) -
-00001d80: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00001d90: 2222 2249 6e69 7469 616c 697a 6520 7465  """Initialize te
-00001da0: 7374 2063 6c61 7373 2e22 2222 0a20 2020  st class.""".   
-00001db0: 2020 2020 2073 656c 662e 6566 3120 3d20       self.ef1 = 
-00001dc0: 456e 7370 6972 6546 696c 6528 6573 6666  EnspireFile(esff
-00001dd0: 2822 6831 3438 672d 7370 6574 7472 6f43  ("h148g-spettroC
-00001de0: 2e63 7376 2229 290a 2020 2020 2020 2020  .csv")).        
-00001df0: 7365 6c66 2e65 6631 2e65 7874 7261 6374  self.ef1.extract
-00001e00: 5f6d 6561 7375 7265 6d65 6e74 7328 290a  _measurements().
-00001e10: 2020 2020 2020 2020 7365 6c66 2e65 6e31          self.en1
-00001e20: 203d 2045 7870 4e6f 7465 2865 7366 6628   = ExpNote(esff(
-00001e30: 2268 3134 3867 2d73 7065 7474 726f 432d  "h148g-spettroC-
-00001e40: 6e6f 7461 2229 290a 2020 2020 2020 2020  nota")).        
-00001e50: 7365 6c66 2e65 6e32 203d 2045 7870 4e6f  self.en2 = ExpNo
-00001e60: 7465 2865 7366 6628 224d 312d 4136 2d47  te(esff("M1-A6-G
-00001e70: 3132 2d6e 6f74 6122 2929 0a20 2020 2020  12-nota")).     
-00001e80: 2020 2073 656c 662e 656e 3320 3d20 4578     self.en3 = Ex
-00001e90: 704e 6f74 6528 6573 6666 2822 5332 3032  pNote(esff("S202
-00001ea0: 4e2d 4532 5f70 4873 2d6e 6f74 6122 2929  N-E2_pHs-nota"))
-00001eb0: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
-00001ec0: 3165 7272 203d 2045 7870 4e6f 7465 2865  1err = ExpNote(e
-00001ed0: 7366 6628 2268 3134 3867 2d73 7065 7474  sff("h148g-spett
-00001ee0: 726f 432d 6e6f 7461 2d45 7272 2229 290a  roC-nota-Err")).
-00001ef0: 0a20 2020 2064 6566 2074 6573 745f 6765  .    def test_ge
-00001f00: 745f 6c69 7374 5f66 726f 6d5f 6e6f 7465  t_list_from_note
-00001f10: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00001f20: 2020 2020 2020 2020 2222 2254 6573 7420          """Test 
-00001f30: 6765 745f 7765 6c6c 5f6c 6973 745f 6672  get_well_list_fr
-00001f40: 6f6d 5f6e 6f74 6520 6d65 7468 6f64 2e22  om_note method."
-00001f50: 2222 0a20 2020 2020 2020 2061 7373 6572  "".        asser
-00001f60: 7420 7365 6c66 2e65 6e31 2e77 656c 6c73  t self.en1.wells
-00001f70: 5b32 5d20 3d3d 2022 4130 3322 0a20 2020  [2] == "A03".   
-00001f80: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-00001f90: 2e65 6e32 2e77 656c 6c73 5b31 5d20 3d3d  .en2.wells[1] ==
-00001fa0: 2022 4831 3222 0a20 2020 2020 2020 2061   "H12".        a
-00001fb0: 7373 6572 7420 7365 6c66 2e65 6e33 2e77  ssert self.en3.w
-00001fc0: 656c 6c73 5b32 5d20 3d3d 2022 4130 3322  ells[2] == "A03"
-00001fd0: 0a0a 2020 2020 6465 6620 7465 7374 5f6e  ..    def test_n
-00001fe0: 6f74 655f 6c69 7374 2873 656c 6629 202d  ote_list(self) -
-00001ff0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00002000: 2222 2254 6573 7420 7765 6c6c 5f6c 6973  """Test well_lis
-00002010: 7420 6672 6f6d 206e 6f74 652e 2222 220a  t from note.""".
-00002020: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00002030: 656c 662e 656e 312e 6e6f 7465 5f6c 6973  elf.en1.note_lis
-00002040: 745b 335d 5b30 5d20 3d3d 2022 4130 3322  t[3][0] == "A03"
-00002050: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00002060: 7365 6c66 2e65 6e32 2e6e 6f74 655f 6c69  self.en2.note_li
-00002070: 7374 5b32 5d5b 305d 203d 3d20 2248 3132  st[2][0] == "H12
-00002080: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
-00002090: 2073 656c 662e 656e 312e 6e6f 7465 5f6c   self.en1.note_l
-000020a0: 6973 745b 3635 5d5b 315d 203d 3d20 2238  ist[65][1] == "8
-000020b0: 2e32 220a 2020 2020 2020 2020 6173 7365  .2".        asse
-000020c0: 7274 2073 656c 662e 656e 322e 6e6f 7465  rt self.en2.note
-000020d0: 5f6c 6973 745b 325d 5b31 5d20 3d3d 2022  _list[2][1] == "
-000020e0: 392e 3336 220a 0a20 2020 2064 6566 2074  9.36"..    def t
-000020f0: 6573 745f 6368 6563 6b5f 6c69 7374 2873  est_check_list(s
-00002100: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00002110: 2020 2020 2020 2222 2254 6573 7420 6368        """Test ch
-00002120: 6563 6b20 6c69 7374 2066 726f 6d20 6e6f  eck list from no
-00002130: 7465 2076 732e 2045 6e73 7069 7265 6669  te vs. Enspirefi
-00002140: 6c65 2e22 2222 0a20 2020 2020 2020 2061  le.""".        a
-00002150: 7373 6572 7420 7365 6c66 2e65 6e31 2e63  ssert self.en1.c
-00002160: 6865 636b 5f77 656c 6c73 2873 656c 662e  heck_wells(self.
-00002170: 6566 3129 2069 7320 5472 7565 0a20 2020  ef1) is True.   
-00002180: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-00002190: 2e65 6e31 6572 722e 6368 6563 6b5f 7765  .en1err.check_we
-000021a0: 6c6c 7328 7365 6c66 2e65 6631 2920 6973  lls(self.ef1) is
-000021b0: 2046 616c 7365 0a0a 2020 2020 6465 6620   False..    def 
-000021c0: 7465 7374 5f62 7569 6c64 5f74 6974 7261  test_build_titra
-000021d0: 7469 6f6e 7328 7365 6c66 2920 2d3e 204e  tions(self) -> N
-000021e0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-000021f0: 5465 7374 2074 6865 206d 6574 686f 6420  Test the method 
-00002200: 6578 7472 6163 745f 7469 7472 6174 696f  extract_titratio
-00002210: 6e73 2829 2e22 2222 0a20 2020 2020 2020  ns().""".       
-00002220: 2073 656c 662e 656e 312e 6275 696c 645f   self.en1.build_
-00002230: 7469 7472 6174 696f 6e73 2873 656c 662e  titrations(self.
-00002240: 6566 3129 0a20 2020 2020 2020 2061 7373  ef1).        ass
-00002250: 6572 7420 6c65 6e28 7365 6c66 2e65 6e31  ert len(self.en1
-00002260: 2e74 6974 7261 7469 6f6e 7329 203d 3d20  .titrations) == 
-00002270: 360a 2020 2020 2020 2020 7469 7420 3d20  6.        tit = 
-00002280: 7365 6c66 2e65 6e31 2e74 6974 7261 7469  self.en1.titrati
-00002290: 6f6e 735b 305d 0a20 2020 2020 2020 2061  ons[0].        a
-000022a0: 7373 6572 7420 7469 742e 636f 6e63 203d  ssert tit.conc =
-000022b0: 3d20 5b35 2e32 2c20 362e 332c 2037 2e34  = [5.2, 6.3, 7.4
-000022c0: 2c20 382e 312c 2038 2e32 5d0a 2020 2020  , 8.1, 8.2].    
-000022d0: 2020 2020 6173 7365 7274 2074 6974 2e64      assert tit.d
-000022e0: 6174 615b 2241 225d 5b28 352e 322c 2022  ata["A"][(5.2, "
-000022f0: 4130 3122 295d 5b32 3732 5d20 3d3d 2033  A01")][272] == 3
-00002300: 3135 310a 2020 2020 2020 2020 7469 7420  151.        tit 
-00002310: 3d20 7365 6c66 2e65 6e31 2e74 6974 7261  = self.en1.titra
-00002320: 7469 6f6e 735b 355d 0a20 2020 2020 2020  tions[5].       
-00002330: 2061 7373 6572 7420 7469 742e 6461 7461   assert tit.data
-00002340: 5b22 4122 5d5b 2836 3637 2e30 2c20 2245  ["A"][(667.0, "E
-00002350: 3131 2229 5d5b 3530 305d 203d 3d20 3837  11")][500] == 87
-00002360: 3334 0a                                  34.
+00000000: 0000 0000 0000 0000 0100 0000 0000 0000  ................
+00000010: 1400 0000 0000 0000 556e 7573 6564 4d65  ........UnusedMe
+00000020: 7468 6f64 4172 6775 6d65 6e74 1d00 0000  thodArgument....
+00000030: 0000 0000 556e 7573 6564 206d 6574 686f  ....Unused metho
+00000040: 6420 6172 6775 6d65 6e74 3a20 6065 6632  d argument: `ef2
+00000050: 6000 003d 1000 004d 1000 0000 0000 0000  `..=...M........
+00000060: 0000 0000 0000 0000 0000 003d 1000 0001  ...........=....
+00000070: 0000 0000 0000 0034 0000 0000 0000 002f  .......4......./
+00000080: 686f 6d65 2f64 616e 2f77 6f72 6b73 7061  home/dan/workspa
+00000090: 6365 2f43 6c6f 7048 6669 742f 7465 7374  ce/ClopHfit/test
+000000a0: 732f 7465 7374 5f70 7265 6e73 7069 7265  s/test_prenspire
+000000b0: 2e70 79b4 2000 0000 0000 0022 2222 5465  .py. ......"""Te
+000000c0: 7374 2070 7265 6e73 7069 7265 206d 6f64  st prenspire mod
+000000d0: 756c 652e 2222 220a 6672 6f6d 205f 5f66  ule.""".from __f
+000000e0: 7574 7572 655f 5f20 696d 706f 7274 2061  uture__ import a
+000000f0: 6e6e 6f74 6174 696f 6e73 0a0a 6672 6f6d  nnotations..from
+00000100: 2070 6174 686c 6962 2069 6d70 6f72 7420   pathlib import 
+00000110: 5061 7468 0a0a 696d 706f 7274 2070 7974  Path..import pyt
+00000120: 6573 740a 0a66 726f 6d20 636c 6f70 6866  est..from clophf
+00000130: 6974 2e70 7265 6e73 7069 7265 2069 6d70  it.prenspire imp
+00000140: 6f72 7420 456e 7370 6972 6546 696c 650a  ort EnspireFile.
+00000150: 6672 6f6d 2063 6c6f 7068 6669 742e 7072  from clophfit.pr
+00000160: 656e 7370 6972 6520 696d 706f 7274 2045  enspire import E
+00000170: 7870 4e6f 7465 0a0a 6461 7461 5f66 696c  xpNote..data_fil
+00000180: 6573 5f64 6972 203d 2050 6174 6828 5f5f  es_dir = Path(__
+00000190: 6669 6c65 5f5f 292e 7061 7265 6e74 202f  file__).parent /
+000001a0: 2022 456e 5370 6972 6522 0a65 7366 6620   "EnSpire".esff 
+000001b0: 3d20 6461 7461 5f66 696c 6573 5f64 6972  = data_files_dir
+000001c0: 2e6a 6f69 6e70 6174 680a 0a0a 4070 7974  .joinpath...@pyt
+000001d0: 6573 742e 6669 7874 7572 6528 7363 6f70  est.fixture(scop
+000001e0: 653d 226d 6f64 756c 6522 290a 6465 6620  e="module").def 
+000001f0: 6566 3128 2920 2d3e 2045 6e73 7069 7265  ef1() -> Enspire
+00000200: 4669 6c65 3a0a 2020 2020 2222 2252 6561  File:.    """Rea
+00000210: 6420 696e 2066 696c 652e 2222 220a 2020  d in file.""".  
+00000220: 2020 6566 203d 2045 6e73 7069 7265 4669    ef = EnspireFi
+00000230: 6c65 2865 7366 6628 2268 3134 3867 2d73  le(esff("h148g-s
+00000240: 7065 7474 726f 432e 6373 7622 2929 0a20  pettroC.csv")). 
+00000250: 2020 2065 662e 6578 7472 6163 745f 6d65     ef.extract_me
+00000260: 6173 7572 656d 656e 7473 2829 0a20 2020  asurements().   
+00000270: 2072 6574 7572 6e20 6566 0a0a 0a40 7079   return ef...@py
+00000280: 7465 7374 2e66 6978 7475 7265 2873 636f  test.fixture(sco
+00000290: 7065 3d22 6d6f 6475 6c65 2229 0a64 6566  pe="module").def
+000002a0: 2065 6632 2829 202d 3e20 456e 7370 6972   ef2() -> Enspir
+000002b0: 6546 696c 653a 0a20 2020 2022 2222 5265  eFile:.    """Re
+000002c0: 6164 2069 6e20 6669 6c65 2077 6974 686f  ad in file witho
+000002d0: 7574 2027 5361 6d70 6c65 7327 2063 6f6c  ut 'Samples' col
+000002e0: 756d 6e2e 2222 220a 2020 2020 6566 203d  umn.""".    ef =
+000002f0: 2045 6e73 7069 7265 4669 6c65 2865 7366   EnspireFile(esf
+00000300: 6628 2265 322d 542d 7769 7468 6f75 745f  f("e2-T-without_
+00000310: 7361 6d70 6c65 5f63 6f6c 756d 6e2e 6373  sample_column.cs
+00000320: 7622 2929 0a20 2020 2065 662e 6578 7472  v")).    ef.extr
+00000330: 6163 745f 6d65 6173 7572 656d 656e 7473  act_measurements
+00000340: 2829 0a20 2020 2072 6574 7572 6e20 6566  ().    return ef
+00000350: 0a0a 0a63 6c61 7373 2054 6573 7445 6e73  ...class TestEns
+00000360: 7069 7265 4669 6c65 3a0a 2020 2020 2222  pireFile:.    ""
+00000370: 2254 6573 7420 456e 7370 6972 6546 696c  "Test EnspireFil
+00000380: 6520 636c 6173 732e 2222 220a 0a20 2020  e class."""..   
+00000390: 2064 6566 2074 6573 745f 6578 6365 7074   def test_except
+000003a0: 696f 6e73 2873 656c 6629 202d 3e20 4e6f  ions(self) -> No
+000003b0: 6e65 3a0a 2020 2020 2020 2020 2222 2254  ne:.        """T
+000003c0: 6573 7420 736f 6d65 2072 6169 7365 6420  est some raised 
+000003d0: 6578 6365 7074 696f 6e73 2e22 2222 0a20  exceptions.""". 
+000003e0: 2020 2020 2020 2065 7366 6620 3d20 2864         esff = (d
+000003f0: 6174 615f 6669 6c65 735f 6469 7220 2f20  ata_files_dir / 
+00000400: 2265 7863 6570 7469 6f6e 7322 292e 6a6f  "exceptions").jo
+00000410: 696e 7061 7468 0a20 2020 2020 2020 2023  inpath.        #
+00000420: 2054 6573 7420 6765 745f 6461 7461 5f69   Test get_data_i
+00000430: 6e69 2045 7863 6570 7469 6f6e 730a 2020  ni Exceptions.  
+00000440: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
+00000450: 742e 7261 6973 6573 2845 7863 6570 7469  t.raises(Excepti
+00000460: 6f6e 2c20 6d61 7463 683d 224e 6f20 6c69  on, match="No li
+00000470: 6e65 2073 7461 7274 696e 6720 7769 7468  ne starting with
+00000480: 202e 2229 3a0a 2020 2020 2020 2020 2020   ."):.          
+00000490: 2020 456e 7370 6972 6546 696c 6528 6573    EnspireFile(es
+000004a0: 6666 2822 6831 3438 672d 7370 6574 7472  ff("h148g-spettr
+000004b0: 6f43 2d69 6478 302e 6373 7622 2929 0a20  oC-idx0.csv")). 
+000004c0: 2020 2020 2020 2077 6974 6820 7079 7465         with pyte
+000004d0: 7374 2e72 6169 7365 7328 4578 6365 7074  st.raises(Except
+000004e0: 696f 6e2c 206d 6174 6368 3d22 4d75 6c74  ion, match="Mult
+000004f0: 6970 6c65 206c 696e 6573 2073 7461 7274  iple lines start
+00000500: 696e 6720 7769 7468 202e 2229 3a0a 2020  ing with ."):.  
+00000510: 2020 2020 2020 2020 2020 456e 7370 6972            Enspir
+00000520: 6546 696c 6528 6573 6666 2822 6831 3438  eFile(esff("h148
+00000530: 672d 7370 6574 7472 6f43 2d69 6478 322e  g-spettroC-idx2.
+00000540: 6373 7622 2929 0a20 2020 2020 2020 2023  csv")).        #
+00000550: 2054 6573 7420 706c 6174 656d 6170 0a20   Test platemap. 
+00000560: 2020 2020 2020 2077 6974 6820 7079 7465         with pyte
+00000570: 7374 2e72 6169 7365 7328 4578 6365 7074  st.raises(Except
+00000580: 696f 6e2c 206d 6174 6368 3d22 7374 6f70  ion, match="stop
+00000590: 3a20 506c 6174 656d 6170 2066 6f72 6d61  : Platemap forma
+000005a0: 7420 756e 6578 7065 6374 6564 2229 3a0a  t unexpected"):.
+000005b0: 2020 2020 2020 2020 2020 2020 456e 7370              Ensp
+000005c0: 6972 6546 696c 6528 6573 6666 2822 4d31  ireFile(esff("M1
+000005d0: 2d41 362d 4731 325f 3131 636f 6c75 6d6e  -A6-G12_11column
+000005e0: 732e 6373 7622 2929 0a20 2020 2020 2020  s.csv")).       
+000005f0: 2023 2054 6573 7420 7468 6520 7072 6573   # Test the pres
+00000600: 656e 6365 206f 6620 736f 6d65 2065 6d70  ence of some emp
+00000610: 7479 206c 696e 6573 0a20 2020 2020 2020  ty lines.       
+00000620: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
+00000630: 7365 7328 4578 6365 7074 696f 6e2c 206d  ses(Exception, m
+00000640: 6174 6368 3d22 4578 7065 6374 696e 6720  atch="Expecting 
+00000650: 7477 6f20 656d 7074 7920 6c69 6e65 7320  two empty lines 
+00000660: 6265 666f 7265 205f 696e 6922 293a 0a20  before _ini"):. 
+00000670: 2020 2020 2020 2020 2020 2045 6e73 7069             Enspi
+00000680: 7265 4669 6c65 2865 7366 6628 224d 312d  reFile(esff("M1-
+00000690: 4136 2d47 3132 5f6d 6973 7369 6e67 5f65  A6-G12_missing_e
+000006a0: 6d70 7479 6c69 6e65 5f69 6e69 2e63 7376  mptyline_ini.csv
+000006b0: 2229 290a 2020 2020 2020 2020 7769 7468  ")).        with
+000006c0: 2070 7974 6573 742e 7261 6973 6573 2845   pytest.raises(E
+000006d0: 7863 6570 7469 6f6e 2c20 6d61 7463 683d  xception, match=
+000006e0: 2245 7870 6563 7469 6e67 2061 6e20 656d  "Expecting an em
+000006f0: 7074 7920 6c69 6e65 2061 6674 6572 205f  pty line after _
+00000700: 6669 6e22 293a 0a20 2020 2020 2020 2020  fin"):.         
+00000710: 2020 2045 6e73 7069 7265 4669 6c65 2865     EnspireFile(e
+00000720: 7366 6628 224d 312d 4136 2d47 3132 5f6d  sff("M1-A6-G12_m
+00000730: 6973 7369 6e67 5f65 6d70 7479 6c69 6e65  issing_emptyline
+00000740: 5f66 696e 2e63 7376 2229 290a 2020 2020  _fin.csv")).    
+00000750: 2020 2020 2320 5465 7374 206d 756c 7469      # Test multi
+00000760: 706c 6520 656d 6973 7369 6f6e 2077 6176  ple emission wav
+00000770: 656c 6562 6774 6873 2069 6e20 6578 6369  elebgths in exci
+00000780: 7461 7469 6f6e 2073 7065 6374 7261 0a20  tation spectra. 
+00000790: 2020 2020 2020 2077 6974 6820 7079 7465         with pyte
+000007a0: 7374 2e72 6169 7365 7328 0a20 2020 2020  st.raises(.     
+000007b0: 2020 2020 2020 2045 7863 6570 7469 6f6e         Exception
+000007c0: 2c20 6d61 7463 683d 2245 7863 6974 6174  , match="Excitat
+000007d0: 696f 6e20 7370 6563 7472 6120 7769 7468  ion spectra with
+000007e0: 2075 6e65 7870 6563 7465 6420 656d 6973   unexpected emis
+000007f0: 7369 6f6e 2069 6e20 4d65 6173 4122 0a20  sion in MeasA". 
+00000800: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00000810: 2020 2020 2020 456e 7370 6972 6546 696c        EnspireFil
+00000820: 6528 6573 6666 2822 6532 6461 6e2d 6578  e(esff("e2dan-ex
+00000830: 7761 7665 6c65 6e67 7468 2e63 7376 2229  wavelength.csv")
+00000840: 292e 6578 7472 6163 745f 6d65 6173 7572  ).extract_measur
+00000850: 656d 656e 7473 2829 0a20 2020 2020 2020  ements().       
+00000860: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
+00000870: 7365 7328 0a20 2020 2020 2020 2020 2020  ses(.           
+00000880: 2045 7863 6570 7469 6f6e 2c20 6d61 7463   Exception, matc
+00000890: 683d 2245 7863 6974 6174 696f 6e20 7370  h="Excitation sp
+000008a0: 6563 7472 6120 7769 7468 2075 6e65 7870  ectra with unexp
+000008b0: 6563 7465 6420 656d 6973 7369 6f6e 2069  ected emission i
+000008c0: 6e20 4d65 6173 4122 0a20 2020 2020 2020  n MeasA".       
+000008d0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+000008e0: 456e 7370 6972 6546 696c 6528 6573 6666  EnspireFile(esff
+000008f0: 2822 6532 6461 6e2d 6578 7761 7665 6c65  ("e2dan-exwavele
+00000900: 6e67 7468 322e 6373 7622 2929 2e65 7874  ngth2.csv")).ext
+00000910: 7261 6374 5f6d 6561 7375 7265 6d65 6e74  ract_measurement
+00000920: 7328 290a 2020 2020 2020 2020 7769 7468  s().        with
+00000930: 2070 7974 6573 742e 7261 6973 6573 280a   pytest.raises(.
+00000940: 2020 2020 2020 2020 2020 2020 4578 6365              Exce
+00000950: 7074 696f 6e2c 206d 6174 6368 3d22 456d  ption, match="Em
+00000960: 6973 7369 6f6e 2073 7065 6374 7261 2077  ission spectra w
+00000970: 6974 6820 756e 6578 7065 6374 6564 2065  ith unexpected e
+00000980: 7863 6974 6174 696f 6e20 696e 204d 6561  xcitation in Mea
+00000990: 7343 220a 2020 2020 2020 2020 293a 0a20  sC".        ):. 
+000009a0: 2020 2020 2020 2020 2020 2045 6e73 7069             Enspi
+000009b0: 7265 4669 6c65 2865 7366 6628 2265 3264  reFile(esff("e2d
+000009c0: 616e 2d65 6d77 6176 656c 656e 6774 682e  an-emwavelength.
+000009d0: 6373 7622 2929 2e65 7874 7261 6374 5f6d  csv")).extract_m
+000009e0: 6561 7375 7265 6d65 6e74 7328 290a 2020  easurements().  
+000009f0: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
+00000a00: 742e 7261 6973 6573 280a 2020 2020 2020  t.raises(.      
+00000a10: 2020 2020 2020 4578 6365 7074 696f 6e2c        Exception,
+00000a20: 206d 6174 6368 3d27 556e 6b6e 6f77 6e20   match='Unknown 
+00000a30: 224d 6f6e 6f63 6872 6f6d 6174 6f72 223a  "Monochromator":
+00000a40: 2053 7472 616e 6765 2069 6e20 4d65 6173   Strange in Meas
+00000a50: 4227 0a20 2020 2020 2020 2029 3a0a 2020  B'.        ):.  
+00000a60: 2020 2020 2020 2020 2020 456e 7370 6972            Enspir
+00000a70: 6546 696c 6528 6573 6666 2822 6532 6461  eFile(esff("e2da
+00000a80: 6e2d 6578 7761 7665 6c65 6e67 7468 7374  n-exwavelengthst
+00000a90: 7261 6e67 652e 6373 7622 2929 2e65 7874  range.csv")).ext
+00000aa0: 7261 6374 5f6d 6561 7375 7265 6d65 6e74  ract_measurement
+00000ab0: 7328 290a 0a20 2020 2064 6566 2074 6573  s()..    def tes
+00000ac0: 745f 6765 745f 6461 7461 5f69 6e69 2873  t_get_data_ini(s
+00000ad0: 656c 662c 2065 6631 3a20 456e 7370 6972  elf, ef1: Enspir
+00000ae0: 6546 696c 652c 2065 6632 3a20 456e 7370  eFile, ef2: Ensp
+00000af0: 6972 6546 696c 6529 202d 3e20 4e6f 6e65  ireFile) -> None
+00000b00: 3a0a 2020 2020 2020 2020 2222 2254 6573  :.        """Tes
+00000b10: 7420 6765 745f 6461 7461 5f69 6e69 2e22  t get_data_ini."
+00000b20: 2222 0a20 2020 2020 2020 2061 7373 6572  "".        asser
+00000b30: 7420 6566 312e 5f69 6e69 203d 3d20 3132  t ef1._ini == 12
+00000b40: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00000b50: 6566 322e 5f69 6e69 203d 3d20 390a 0a20  ef2._ini == 9.. 
+00000b60: 2020 2064 6566 2074 6573 745f 6669 6e28     def test_fin(
+00000b70: 7365 6c66 2c20 6566 313a 2045 6e73 7069  self, ef1: Enspi
+00000b80: 7265 4669 6c65 2c20 6566 323a 2045 6e73  reFile, ef2: Ens
+00000b90: 7069 7265 4669 6c65 2920 2d3e 204e 6f6e  pireFile) -> Non
+00000ba0: 653a 0a20 2020 2020 2020 2022 2222 5465  e:.        """Te
+00000bb0: 7374 205f 6669 6e20 286c 696e 655f 696e  st _fin (line_in
+00000bc0: 6465 7828 2929 2e22 2222 0a20 2020 2020  dex()).""".     
+00000bd0: 2020 2061 7373 6572 7420 6566 312e 5f66     assert ef1._f
+00000be0: 696e 203d 3d20 3134 3839 370a 2020 2020  in == 14897.    
+00000bf0: 2020 2020 6173 7365 7274 2065 6632 2e5f      assert ef2._
+00000c00: 6669 6e20 3d3d 2038 3536 0a0a 2020 2020  fin == 856..    
+00000c10: 6465 6620 7465 7374 5f6d 6574 6164 6174  def test_metadat
+00000c20: 615f 706f 7374 2873 656c 662c 2065 6631  a_post(self, ef1
+00000c30: 3a20 456e 7370 6972 6546 696c 652c 2065  : EnspireFile, e
+00000c40: 6632 3a20 456e 7370 6972 6546 696c 6529  f2: EnspireFile)
+00000c50: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00000c60: 2020 2222 2249 6465 6e74 6966 7920 636f    """Identify co
+00000c70: 7272 6563 746c 7920 7468 6520 6265 6769  rrectly the begi
+00000c80: 6e6e 696e 6720 6f66 206d 6574 6164 6174  nning of metadat
+00000c90: 6120 6166 7465 7220 6461 7461 2062 6c6f  a after data blo
+00000ca0: 636b 2e22 2222 0a20 2020 2020 2020 2061  ck.""".        a
+00000cb0: 7373 6572 7420 6566 312e 5f6d 6574 6164  ssert ef1._metad
+00000cc0: 6174 615f 706f 7374 5b30 5d20 3d3d 205b  ata_post[0] == [
+00000cd0: 2242 6173 6963 2061 7373 6179 2069 6e66  "Basic assay inf
+00000ce0: 6f72 6d61 7469 6f6e 2022 5d0a 2020 2020  ormation "].    
+00000cf0: 2020 2020 6173 7365 7274 2065 6632 2e5f      assert ef2._
+00000d00: 6d65 7461 6461 7461 5f70 6f73 745b 305d  metadata_post[0]
+00000d10: 203d 3d20 5b22 4261 7369 6320 6173 7361   == ["Basic assa
+00000d20: 7920 696e 666f 726d 6174 696f 6e20 225d  y information "]
+00000d30: 0a0a 2020 2020 6465 6620 7465 7374 5f6c  ..    def test_l
+00000d40: 6f63 616c 6567 656e 5f69 6e5f 6d65 7461  ocalegen_in_meta
+00000d50: 6461 7461 5f70 6f73 7428 0a20 2020 2020  data_post(.     
+00000d60: 2020 2073 656c 662c 2065 6631 3a20 456e     self, ef1: En
+00000d70: 7370 6972 6546 696c 652c 2065 6632 3a20  spireFile, ef2: 
+00000d80: 456e 7370 6972 6546 696c 650a 2020 2020  EnspireFile.    
+00000d90: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00000da0: 2020 2022 2222 5465 7374 206c 6f63 616c     """Test local
+00000db0: 6573 2e22 2222 0a20 2020 2020 2020 2061  es.""".        a
+00000dc0: 7373 6572 7420 6566 312e 5f6d 6574 6164  ssert ef1._metad
+00000dd0: 6174 615f 706f 7374 5b33 315d 5b34 5d20  ata_post[31][4] 
+00000de0: 3d3d 2022 3330 3020 c2b5 6c22 0a20 2020  == "300 ..l".   
+00000df0: 2020 2020 2061 7373 6572 7420 6566 322e       assert ef2.
+00000e00: 5f6d 6574 6164 6174 615f 706f 7374 5b33  _metadata_post[3
+00000e10: 315d 5b34 5d20 3d3d 2022 3330 3020 c2b5  1][4] == "300 ..
+00000e20: 6c22 0a0a 2020 2020 6465 6620 7465 7374  l"..    def test
+00000e30: 5f64 6174 615f 6c69 7374 2873 656c 662c  _data_list(self,
+00000e40: 2065 6631 3a20 456e 7370 6972 6546 696c   ef1: EnspireFil
+00000e50: 652c 2065 6632 3a20 456e 7370 6972 6546  e, ef2: EnspireF
+00000e60: 696c 6529 202d 3e20 4e6f 6e65 3a0a 2020  ile) -> None:.  
+00000e70: 2020 2020 2020 2222 2254 6573 7420 6461        """Test da
+00000e80: 7461 5f6c 6973 742e 2222 220a 2020 2020  ta_list.""".    
+00000e90: 2020 2020 6173 7365 7274 2065 6631 2e5f      assert ef1._
+00000ea0: 6461 7461 5f6c 6973 745b 305d 5b32 5d20  data_list[0][2] 
+00000eb0: 3d3d 2022 4d65 6173 413a 5265 7375 6c74  == "MeasA:Result
+00000ec0: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
+00000ed0: 2065 6632 2e5f 6461 7461 5f6c 6973 745b   ef2._data_list[
+00000ee0: 305d 5b32 5d20 3d3d 2022 4d65 6173 423a  0][2] == "MeasB:
+00000ef0: 5761 7665 6c65 6e67 7468 456d 7322 0a20  WavelengthEms". 
+00000f00: 2020 2020 2020 2061 7373 6572 7420 6566         assert ef
+00000f10: 312e 5f64 6174 615f 6c69 7374 5b31 5d5b  1._data_list[1][
+00000f20: 325d 203d 3d20 2233 3135 3122 0a20 2020  2] == "3151".   
+00000f30: 2020 2020 2061 7373 6572 7420 6566 322e       assert ef2.
+00000f40: 5f64 6174 615f 6c69 7374 5b31 5d5b 335d  _data_list[1][3]
+00000f50: 203d 3d20 2233 3733 3922 0a20 2020 2020   == "3739".     
+00000f60: 2020 2023 2049 6d70 6f72 7461 6e74 2074     # Important t
+00000f70: 6f20 6368 6563 6b20 666f 7220 6c61 7374  o check for last
+00000f80: 206c 696e 650a 2020 2020 2020 2020 6173   line.        as
+00000f90: 7365 7274 2065 6631 2e5f 6461 7461 5f6c  sert ef1._data_l
+00000fa0: 6973 745b 2d31 5d5b 325d 203d 3d20 2239  ist[-1][2] == "9
+00000fb0: 3736 3132 220a 2020 2020 2020 2020 6173  7612".        as
+00000fc0: 7365 7274 2065 6632 2e5f 6461 7461 5f6c  sert ef2._data_l
+00000fd0: 6973 745b 2d31 5d5b 335d 203d 3d20 2235  ist[-1][3] == "5
+00000fe0: 3132 220a 0a20 2020 2064 6566 2074 6573  12"..    def tes
+00000ff0: 745f 6765 745f 6c69 7374 5f66 726f 6d5f  t_get_list_from_
+00001000: 706c 6174 656d 6170 2873 656c 662c 2065  platemap(self, e
+00001010: 6631 3a20 456e 7370 6972 6546 696c 652c  f1: EnspireFile,
+00001020: 2065 6632 3a20 456e 7370 6972 6546 696c   ef2: EnspireFil
+00001030: 6529 202d 3e20 4e6f 6e65 3a0a 2020 2020  e) -> None:.    
+00001040: 2020 2020 2222 2254 6573 7420 6c69 7374      """Test list
+00001050: 2066 726f 6d20 706c 6174 656d 6170 2e22   from platemap."
+00001060: 2222 0a20 2020 2020 2020 2061 7373 6572  "".        asser
+00001070: 7420 6566 312e 5f77 656c 6c5f 6c69 7374  t ef1._well_list
+00001080: 5f70 6c61 7465 6d61 705b 325d 203d 3d20  _platemap[2] == 
+00001090: 2241 3033 220a 2020 2020 2020 2020 6173  "A03".        as
+000010a0: 7365 7274 2065 6632 2e5f 7765 6c6c 5f6c  sert ef2._well_l
+000010b0: 6973 745f 706c 6174 656d 6170 5b31 5d20  ist_platemap[1] 
+000010c0: 3d3d 2022 4630 3222 0a0a 2020 2020 6465  == "F02"..    de
+000010d0: 6620 7465 7374 5f6d 6574 6164 6174 6128  f test_metadata(
+000010e0: 7365 6c66 2c20 6566 313a 2045 6e73 7069  self, ef1: Enspi
+000010f0: 7265 4669 6c65 2c20 6566 323a 2045 6e73  reFile, ef2: Ens
+00001100: 7069 7265 4669 6c65 2920 2d3e 204e 6f6e  pireFile) -> Non
+00001110: 653a 0a20 2020 2020 2020 2022 2222 5465  e:.        """Te
+00001120: 7374 206d 6574 6164 6174 6120 6469 6374  st metadata dict
+00001130: 696f 6e61 7279 2e22 2222 0a20 2020 2020  ionary.""".     
+00001140: 2020 2061 7373 6572 7420 6566 312e 6d65     assert ef1.me
+00001150: 7461 6461 7461 5b22 4d65 6173 7572 656d  tadata["Measurem
+00001160: 656e 7420 6461 7465 225d 203d 3d20 2232  ent date"] == "2
+00001170: 3031 312d 3130 2d30 3320 3137 3a31 323a  011-10-03 17:12:
+00001180: 3333 220a 2020 2020 2020 2020 6173 7365  33".        asse
+00001190: 7274 2065 6631 2e6d 6574 6164 6174 615b  rt ef1.metadata[
+000011a0: 2243 6861 6d62 6572 2074 656d 7065 7261  "Chamber tempera
+000011b0: 7475 7265 2061 7420 7374 6172 7422 5d20  ture at start"] 
+000011c0: 3d3d 2022 3230 220a 2020 2020 2020 2020  == "20".        
+000011d0: 6173 7365 7274 2065 6631 2e6d 6574 6164  assert ef1.metad
+000011e0: 6174 615b 2243 6861 6d62 6572 2074 656d  ata["Chamber tem
+000011f0: 7065 7261 7475 7265 2061 7420 656e 6422  perature at end"
+00001200: 5d20 3d3d 2022 3230 220a 2020 2020 2020  ] == "20".      
+00001210: 2020 6173 7365 7274 2065 6631 2e6d 6574    assert ef1.met
+00001220: 6164 6174 615b 2241 6d62 6965 6e74 2074  adata["Ambient t
+00001230: 656d 7065 7261 7475 7265 2061 7420 7374  emperature at st
+00001240: 6172 7422 5d20 3d3d 2022 3622 0a20 2020  art"] == "6".   
+00001250: 2020 2020 2061 7373 6572 7420 6566 312e       assert ef1.
+00001260: 6d65 7461 6461 7461 5b22 416d 6269 656e  metadata["Ambien
+00001270: 7420 7465 6d70 6572 6174 7572 6520 6174  t temperature at
+00001280: 2065 6e64 225d 203d 3d20 2239 2e33 220a   end"] == "9.3".
+00001290: 2020 2020 2020 2020 6173 7365 7274 2065          assert e
+000012a0: 6631 2e6d 6574 6164 6174 615b 2250 726f  f1.metadata["Pro
+000012b0: 746f 636f 6c20 6e61 6d65 225d 203d 3d20  tocol name"] == 
+000012c0: 2245 6363 6974 617a 696f 6e65 2043 220a  "Eccitazione C".
+000012d0: 2020 2020 2020 2020 6173 7365 7274 2028          assert (
+000012e0: 0a20 2020 2020 2020 2020 2020 2065 6631  .            ef1
+000012f0: 2e6d 6574 6164 6174 615b 2245 7870 6f72  .metadata["Expor
+00001300: 7465 6420 6461 7461 225d 203d 3d20 2257  ted data"] == "W
+00001310: 656c 6c2c 5361 6d70 6c65 2c4d 6561 7341  ell,Sample,MeasA
+00001320: 3a52 6573 756c 742c 4d65 6173 413a 5761  :Result,MeasA:Wa
+00001330: 7665 6c65 6e67 7468 220a 2020 2020 2020  velength".      
+00001340: 2020 290a 0a20 2020 2064 6566 2074 6573    )..    def tes
+00001350: 745f 6d65 6173 7572 656d 656e 745f 6d65  t_measurement_me
+00001360: 7461 6461 7461 2873 656c 662c 2065 6631  tadata(self, ef1
+00001370: 3a20 456e 7370 6972 6546 696c 652c 2065  : EnspireFile, e
+00001380: 6632 3a20 456e 7370 6972 6546 696c 6529  f2: EnspireFile)
+00001390: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+000013a0: 2020 2222 2254 6573 7420 6461 7461 206f    """Test data o
+000013b0: 626a 6563 742e 2222 220a 2020 2020 2020  bject.""".      
+000013c0: 2020 6173 7365 7274 2065 6631 2e6d 6561    assert ef1.mea
+000013d0: 7375 7265 6d65 6e74 735b 2241 225d 5b22  surements["A"]["
+000013e0: 6d65 7461 6461 7461 225d 5b22 4d6f 6e6f  metadata"]["Mono
+000013f0: 6368 726f 6d61 746f 7222 5d20 3d3d 2022  chromator"] == "
+00001400: 4578 6369 7461 7469 6f6e 220a 2020 2020  Excitation".    
+00001410: 2020 2020 6173 7365 7274 2065 6631 2e6d      assert ef1.m
+00001420: 6561 7375 7265 6d65 6e74 735b 2241 225d  easurements["A"]
+00001430: 5b22 6d65 7461 6461 7461 225d 5b22 5761  ["metadata"]["Wa
+00001440: 7665 6c65 6e67 7468 225d 203d 3d20 2235  velength"] == "5
+00001450: 3230 220a 2020 2020 2020 2020 6173 7365  20".        asse
+00001460: 7274 2065 6631 2e6d 6561 7375 7265 6d65  rt ef1.measureme
+00001470: 6e74 735b 2241 225d 5b22 6d65 7461 6461  nts["A"]["metada
+00001480: 7461 225d 5b22 7465 6d70 225d 203d 3d20  ta"]["temp"] == 
+00001490: 2232 3022 0a20 2020 2020 2020 2061 7373  "20".        ass
+000014a0: 6572 7420 6566 322e 6d65 6173 7572 656d  ert ef2.measurem
+000014b0: 656e 7473 5b22 4322 5d5b 226d 6574 6164  ents["C"]["metad
+000014c0: 6174 6122 5d5b 224d 6f6e 6f63 6872 6f6d  ata"]["Monochrom
+000014d0: 6174 6f72 225d 203d 3d20 2245 6d69 7373  ator"] == "Emiss
+000014e0: 696f 6e22 0a20 2020 2020 2020 2061 7373  ion".        ass
+000014f0: 6572 7420 6566 322e 6d65 6173 7572 656d  ert ef2.measurem
+00001500: 656e 7473 5b22 4322 5d5b 226d 6574 6164  ents["C"]["metad
+00001510: 6174 6122 5d5b 2257 6176 656c 656e 6774  ata"]["Wavelengt
+00001520: 6822 5d20 3d3d 2022 3438 3022 0a20 2020  h"] == "480".   
+00001530: 2020 2020 2061 7373 6572 7420 6566 322e       assert ef2.
+00001540: 6d65 6173 7572 656d 656e 7473 5b22 4622  measurements["F"
+00001550: 5d5b 226d 6574 6164 6174 6122 5d5b 2274  ]["metadata"]["t
+00001560: 656d 7022 5d20 3d3d 2022 3335 220a 0a20  emp"] == "35".. 
+00001570: 2020 2064 6566 2074 6573 745f 6d65 6173     def test_meas
+00001580: 7572 656d 656e 7473 2873 656c 662c 2065  urements(self, e
+00001590: 6631 3a20 456e 7370 6972 6546 696c 652c  f1: EnspireFile,
+000015a0: 2065 6632 3a20 456e 7370 6972 6546 696c   ef2: EnspireFil
+000015b0: 6529 202d 3e20 4e6f 6e65 3a0a 2020 2020  e) -> None:.    
+000015c0: 2020 2020 2222 2254 6573 7420 6461 7461      """Test data
+000015d0: 206f 626a 6563 742e 2222 220a 2020 2020   object.""".    
+000015e0: 2020 2020 6173 7365 7274 2065 6631 2e6d      assert ef1.m
+000015f0: 6561 7375 7265 6d65 6e74 735b 2241 225d  easurements["A"]
+00001600: 5b22 6c61 6d62 6461 225d 5b30 5d20 3d3d  ["lambda"][0] ==
+00001610: 2032 3732 0a20 2020 2020 2020 2061 7373   272.        ass
+00001620: 6572 7420 6566 312e 6d65 6173 7572 656d  ert ef1.measurem
+00001630: 656e 7473 5b22 4122 5d5b 226c 616d 6264  ents["A"]["lambd
+00001640: 6122 5d5b 3232 385d 203d 3d20 3530 300a  a"][228] == 500.
+00001650: 2020 2020 2020 2020 6173 7365 7274 2065          assert e
+00001660: 6631 2e6d 6561 7375 7265 6d65 6e74 735b  f1.measurements[
+00001670: 2241 225d 5b22 4130 3122 5d5b 305d 203d  "A"]["A01"][0] =
+00001680: 3d20 3331 3531 0a20 2020 2020 2020 2061  = 3151.        a
+00001690: 7373 6572 7420 6566 312e 6d65 6173 7572  ssert ef1.measur
+000016a0: 656d 656e 7473 5b22 4122 5d5b 2241 3031  ements["A"]["A01
+000016b0: 225d 5b32 3238 5d20 3d3d 2035 3733 0a20  "][228] == 573. 
+000016c0: 2020 2020 2020 2023 2049 6d70 6f72 7461         # Importa
+000016d0: 6e74 2074 6f20 6368 6563 6b20 666f 7220  nt to check for 
+000016e0: 6c61 7374 206c 696e 6520 6f66 2063 7376  last line of csv
+000016f0: 6c0a 2020 2020 2020 2020 6173 7365 7274  l.        assert
+00001700: 2065 6631 2e6d 6561 7375 7265 6d65 6e74   ef1.measurement
+00001710: 735b 2241 225d 5b22 4730 3522 5d5b 3232  s["A"]["G05"][22
+00001720: 385d 203d 3d20 3937 3631 320a 2020 2020  8] == 97612.    
+00001730: 2020 2020 6173 7365 7274 2065 6631 2e6d      assert ef1.m
+00001740: 6561 7375 7265 6d65 6e74 735b 2241 225d  easurements["A"]
+00001750: 5b22 4130 3122 5d5b 3130 5d20 3d3d 2032  ["A01"][10] == 2
+00001760: 3439 360a 2020 2020 2020 2020 6173 7365  496.        asse
+00001770: 7274 2065 6631 2e6d 6561 7375 7265 6d65  rt ef1.measureme
+00001780: 6e74 735b 2241 225d 5b22 4130 3222 5d5b  nts["A"]["A02"][
+00001790: 3130 5d20 3d3d 2031 3736 350a 2020 2020  10] == 1765.    
+000017a0: 2020 2020 6173 7365 7274 2065 6631 2e6d      assert ef1.m
+000017b0: 6561 7375 7265 6d65 6e74 735b 2241 225d  easurements["A"]
+000017c0: 5b22 6c61 6d62 6461 225d 5b31 305d 203d  ["lambda"][10] =
+000017d0: 3d20 3238 320a 2020 2020 2020 2020 6173  = 282.        as
+000017e0: 7365 7274 2065 6631 2e6d 6561 7375 7265  sert ef1.measure
+000017f0: 6d65 6e74 735b 2241 225d 5b22 6d65 7461  ments["A"]["meta
+00001800: 6461 7461 225d 5b22 5761 7665 6c65 6e67  data"]["Waveleng
+00001810: 7468 225d 203d 3d20 2235 3230 220a 2020  th"] == "520".  
+00001820: 2020 2020 2020 6173 7365 7274 2065 6632        assert ef2
+00001830: 2e6d 6561 7375 7265 6d65 6e74 735b 2241  .measurements["A
+00001840: 225d 5b22 6c61 6d62 6461 225d 5b32 5d20  "]["lambda"][2] 
+00001850: 3d3d 2034 3032 0a20 2020 2020 2020 2061  == 402.        a
+00001860: 7373 6572 7420 6566 322e 6d65 6173 7572  ssert ef2.measur
+00001870: 656d 656e 7473 5b22 4222 5d5b 2246 3037  ements["B"]["F07
+00001880: 225d 5b31 5d20 3d3d 2031 3839 380a 2020  "][1] == 1898.  
+00001890: 2020 2020 2020 6173 7365 7274 2065 6632        assert ef2
+000018a0: 2e6d 6561 7375 7265 6d65 6e74 735b 2241  .measurements["A
+000018b0: 225d 5b22 6d65 7461 6461 7461 225d 5b22  "]["metadata"]["
+000018c0: 5761 7665 6c65 6e67 7468 225d 203d 3d20  Wavelength"] == 
+000018d0: 2235 3330 220a 0a20 2020 2064 6566 2074  "530"..    def t
+000018e0: 6573 745f 6368 6563 6b5f 6c69 7374 735f  est_check_lists_
+000018f0: 7761 726e 696e 6728 7365 6c66 2920 2d3e  warning(self) ->
+00001900: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00001910: 2222 4974 2077 6172 6e73 2077 6865 6e20  ""It warns when 
+00001920: 2863 7376 2021 3d20 706c 6174 656d 6170  (csv != platemap
+00001930: 292e 0a0a 2020 2020 2020 2020 2a2d 696e  )...        *-in
+00001940: 636f 6d70 6c65 7465 2e63 7376 3a20 3520  complete.csv: 5 
+00001950: 7765 6c6c 7320 2847 312d 4735 2920 6172  wells (G1-G5) ar
+00001960: 6520 6d69 7373 696e 672e 2028 5468 6579  e missing. (They
+00001970: 2061 7265 2070 7265 7365 6e74 2069 6e0a   are present in.
+00001980: 2020 2020 2020 2020 506c 6174 656d 6170          Platemap
+00001990: 2062 6563 6175 7365 2074 6865 7920 7765   because they we
+000019a0: 7265 2070 7265 7365 6e74 2064 7572 696e  re present durin
+000019b0: 6720 6163 7175 6973 6974 696f 6e20 616e  g acquisition an
+000019c0: 6420 7468 656e 206e 6f74 0a20 2020 2020  d then not.     
+000019d0: 2020 2065 7870 6f72 7465 6429 2e0a 0a20     exported)... 
+000019e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000019f0: 2020 2069 6d70 6f72 7420 7761 726e 696e     import warnin
+00001a00: 6773 0a0a 2020 2020 2020 2020 7769 7468  gs..        with
+00001a10: 2077 6172 6e69 6e67 732e 6361 7463 685f   warnings.catch_
+00001a20: 7761 726e 696e 6773 2872 6563 6f72 643d  warnings(record=
+00001a30: 5472 7565 2920 6173 2077 3a0a 2020 2020  True) as w:.    
+00001a40: 2020 2020 2020 2020 2320 4361 7573 6520          # Cause 
+00001a50: 616c 6c20 7761 726e 696e 6773 2074 6f20  all warnings to 
+00001a60: 616c 7761 7973 2062 6520 7472 6967 6765  always be trigge
+00001a70: 7265 642e 0a20 2020 2020 2020 2020 2020  red..           
+00001a80: 2077 6172 6e69 6e67 732e 7369 6d70 6c65   warnings.simple
+00001a90: 6669 6c74 6572 2822 616c 7761 7973 2229  filter("always")
+00001aa0: 0a20 2020 2020 2020 2020 2020 2065 6620  .            ef 
+00001ab0: 3d20 456e 7370 6972 6546 696c 6528 6573  = EnspireFile(es
+00001ac0: 6666 2822 6831 3438 672d 7370 6574 7472  ff("h148g-spettr
+00001ad0: 6f43 2d69 6e63 6f6d 706c 6574 652e 6373  oC-incomplete.cs
+00001ae0: 7622 2929 0a20 2020 2020 2020 2020 2020  v")).           
+00001af0: 2065 662e 6578 7472 6163 745f 6d65 6173   ef.extract_meas
+00001b00: 7572 656d 656e 7473 2829 0a20 2020 2020  urements().     
+00001b10: 2020 2020 2020 2061 7373 6572 7420 6c65         assert le
+00001b20: 6e28 7729 203d 3d20 320a 2020 2020 2020  n(w) == 2.      
+00001b30: 2020 2020 2020 6173 7365 7274 2069 7373        assert iss
+00001b40: 7562 636c 6173 7328 775b 2d31 5d2e 6361  ubclass(w[-1].ca
+00001b50: 7465 676f 7279 2c20 5761 726e 696e 6729  tegory, Warning)
+00001b60: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+00001b70: 6572 7420 2270 6c61 7465 6d61 7022 2069  ert "platemap" i
+00001b80: 6e20 7374 7228 775b 2d31 5d2e 6d65 7373  n str(w[-1].mess
+00001b90: 6167 6529 0a0a 2020 2020 2320 706c 6163  age)..    # plac
+00001ba0: 656d 6172 6b20 6465 6620 7465 7374 5f67  emark def test_g
+00001bb0: 6574 5f6d 6178 7828 7365 6c66 293a 0a20  et_maxx(self):. 
+00001bc0: 2020 2023 2070 6c61 6365 6d61 726b 2020     # placemark  
+00001bd0: 2020 2272 6561 6c6c 7920 6e65 6564 2074    "really need t
+00001be0: 6f20 6265 2063 6f6d 706c 6574 6564 220a  o be completed".
+00001bf0: 2020 2020 2320 706c 6163 656d 6172 6b20      # placemark 
+00001c00: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00001c10: 7561 6c28 7365 6c66 2e73 2e67 6574 5f6d  ual(self.s.get_m
+00001c20: 6178 7828 7365 6c66 2e73 2e65 782c 2073  axx(self.s.ex, s
+00001c30: 656c 662e 732e 7929 2c20 3237 3229 0a0a  elf.s.y), 272)..
+00001c40: 0a40 7079 7465 7374 2e66 6978 7475 7265  .@pytest.fixture
+00001c50: 2873 636f 7065 3d22 6d6f 6475 6c65 2229  (scope="module")
+00001c60: 0a64 6566 2065 6e31 2829 202d 3e20 4578  .def en1() -> Ex
+00001c70: 704e 6f74 653a 0a20 2020 2022 2222 5265  pNote:.    """Re
+00001c80: 6164 206e 6f74 6520 6669 6c65 2e22 2222  ad note file."""
+00001c90: 0a20 2020 2072 6574 7572 6e20 4578 704e  .    return ExpN
+00001ca0: 6f74 6528 6573 6666 2822 6831 3438 672d  ote(esff("h148g-
+00001cb0: 7370 6574 7472 6f43 2d6e 6f74 6122 2929  spettroC-nota"))
+00001cc0: 0a0a 0a40 7079 7465 7374 2e66 6978 7475  ...@pytest.fixtu
+00001cd0: 7265 2873 636f 7065 3d22 6d6f 6475 6c65  re(scope="module
+00001ce0: 2229 0a64 6566 2065 6e31 6572 7228 2920  ").def en1err() 
+00001cf0: 2d3e 2045 7870 4e6f 7465 3a0a 2020 2020  -> ExpNote:.    
+00001d00: 2222 2252 6561 6420 6e6f 7465 2066 696c  """Read note fil
+00001d10: 652e 2222 220a 2020 2020 7265 7475 726e  e.""".    return
+00001d20: 2045 7870 4e6f 7465 2865 7366 6628 2268   ExpNote(esff("h
+00001d30: 3134 3867 2d73 7065 7474 726f 432d 6e6f  148g-spettroC-no
+00001d40: 7461 2d45 7272 2229 290a 0a0a 636c 6173  ta-Err"))...clas
+00001d50: 7320 5465 7374 4578 704e 6f74 653a 0a20  s TestExpNote:. 
+00001d60: 2020 2022 2222 4578 7065 7269 6d65 6e74     """Experiment
+00001d70: 616c 206e 6f74 6573 2e22 2222 0a0a 2020  al notes."""..  
+00001d80: 2020 6465 6620 7465 7374 5f67 6574 5f6c    def test_get_l
+00001d90: 6973 745f 6672 6f6d 5f6e 6f74 6528 7365  ist_from_note(se
+00001da0: 6c66 2c20 656e 313a 2045 7870 4e6f 7465  lf, en1: ExpNote
+00001db0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00001dc0: 2020 2022 2222 5465 7374 2067 6574 5f77     """Test get_w
+00001dd0: 656c 6c5f 6c69 7374 5f66 726f 6d5f 6e6f  ell_list_from_no
+00001de0: 7465 206d 6574 686f 642e 2222 220a 2020  te method.""".  
+00001df0: 2020 2020 2020 6173 7365 7274 2065 6e31        assert en1
+00001e00: 2e77 656c 6c73 5b32 5d20 3d3d 2022 4130  .wells[2] == "A0
+00001e10: 3322 0a0a 2020 2020 6465 6620 7465 7374  3"..    def test
+00001e20: 5f6e 6f74 655f 6c69 7374 2873 656c 662c  _note_list(self,
+00001e30: 2065 6e31 3a20 4578 704e 6f74 6529 202d   en1: ExpNote) -
+00001e40: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00001e50: 2222 2254 6573 7420 7765 6c6c 5f6c 6973  """Test well_lis
+00001e60: 7420 6672 6f6d 206e 6f74 652e 2222 220a  t from note.""".
+00001e70: 2020 2020 2020 2020 6173 7365 7274 2065          assert e
+00001e80: 6e31 2e6e 6f74 655f 6c69 7374 5b33 5d5b  n1.note_list[3][
+00001e90: 305d 203d 3d20 2241 3033 220a 2020 2020  0] == "A03".    
+00001ea0: 2020 2020 6173 7365 7274 2065 6e31 2e6e      assert en1.n
+00001eb0: 6f74 655f 6c69 7374 5b36 355d 5b31 5d20  ote_list[65][1] 
+00001ec0: 3d3d 2022 382e 3222 0a0a 2020 2020 6465  == "8.2"..    de
+00001ed0: 6620 7465 7374 5f63 6865 636b 5f6c 6973  f test_check_lis
+00001ee0: 7428 7365 6c66 2c20 656e 313a 2045 7870  t(self, en1: Exp
+00001ef0: 4e6f 7465 2c20 6566 313a 2045 6e73 7069  Note, ef1: Enspi
+00001f00: 7265 4669 6c65 2c20 656e 3165 7272 3a20  reFile, en1err: 
+00001f10: 4578 704e 6f74 6529 202d 3e20 4e6f 6e65  ExpNote) -> None
+00001f20: 3a0a 2020 2020 2020 2020 2222 2254 6573  :.        """Tes
+00001f30: 7420 6368 6563 6b20 6c69 7374 2066 726f  t check list fro
+00001f40: 6d20 6e6f 7465 2076 732e 2045 6e73 7069  m note vs. Enspi
+00001f50: 7265 6669 6c65 2e22 2222 0a20 2020 2020  refile.""".     
+00001f60: 2020 2061 7373 6572 7420 656e 312e 6368     assert en1.ch
+00001f70: 6563 6b5f 7765 6c6c 7328 6566 3129 2069  eck_wells(ef1) i
+00001f80: 7320 5472 7565 0a20 2020 2020 2020 2061  s True.        a
+00001f90: 7373 6572 7420 656e 3165 7272 2e63 6865  ssert en1err.che
+00001fa0: 636b 5f77 656c 6c73 2865 6631 2920 6973  ck_wells(ef1) is
+00001fb0: 2046 616c 7365 0a0a 2020 2020 6465 6620   False..    def 
+00001fc0: 7465 7374 5f62 7569 6c64 5f74 6974 7261  test_build_titra
+00001fd0: 7469 6f6e 7328 7365 6c66 2c20 656e 313a  tions(self, en1:
+00001fe0: 2045 7870 4e6f 7465 2c20 6566 313a 2045   ExpNote, ef1: E
+00001ff0: 6e73 7069 7265 4669 6c65 2920 2d3e 204e  nspireFile) -> N
+00002000: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00002010: 5465 7374 2074 6865 206d 6574 686f 6420  Test the method 
+00002020: 6578 7472 6163 745f 7469 7472 6174 696f  extract_titratio
+00002030: 6e73 2829 2e22 2222 0a20 2020 2020 2020  ns().""".       
+00002040: 2065 6e31 2e62 7569 6c64 5f74 6974 7261   en1.build_titra
+00002050: 7469 6f6e 7328 6566 3129 0a20 2020 2020  tions(ef1).     
+00002060: 2020 2061 7373 6572 7420 6c65 6e28 656e     assert len(en
+00002070: 312e 7469 7472 6174 696f 6e73 2920 3d3d  1.titrations) ==
+00002080: 2036 0a20 2020 2020 2020 2074 6974 3020   6.        tit0 
+00002090: 3d20 656e 312e 7469 7472 6174 696f 6e73  = en1.titrations
+000020a0: 5b30 5d0a 2020 2020 2020 2020 6173 7365  [0].        asse
+000020b0: 7274 2074 6974 302e 636f 6e63 203d 3d20  rt tit0.conc == 
+000020c0: 5b35 2e32 2c20 362e 332c 2037 2e34 2c20  [5.2, 6.3, 7.4, 
+000020d0: 382e 312c 2038 2e32 5d0a 2020 2020 2020  8.1, 8.2].      
+000020e0: 2020 6173 7365 7274 2074 6974 302e 6461    assert tit0.da
+000020f0: 7461 5b22 4122 5d5b 2835 2e32 2c20 2241  ta["A"][(5.2, "A
+00002100: 3031 2229 5d5b 3237 325d 203d 3d20 3331  01")][272] == 31
+00002110: 3531 0a20 2020 2020 2020 2074 6974 3520  51.        tit5 
+00002120: 3d20 656e 312e 7469 7472 6174 696f 6e73  = en1.titrations
+00002130: 5b35 5d0a 2020 2020 2020 2020 6173 7365  [5].        asse
+00002140: 7274 2074 6974 352e 6461 7461 5b22 4122  rt tit5.data["A"
+00002150: 5d5b 2836 3637 2e30 2c20 2245 3131 2229  ][(667.0, "E11")
+00002160: 5d5b 3530 305d 203d 3d20 3837 3334 0a    ][500] == 8734.
```

### Comparing `clophfit-0.5.4/tests/test_prtecan.py` & `clophfit-0.6.0/tests/test_prtecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/EnSpire/24well_clop0_95.csv` & `clophfit-0.6.0/tests/EnSpire/24well_clop0_95.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/EnSpire/M1-A6-G12.csv` & `clophfit-0.6.0/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv`

 * *Files 0% similar despite different names*

```diff
@@ -500,15 +500,15 @@
 
 14.39 mm x------------------------------------------------------ x 113.38 mm
 74.24 mm                                                           74.24 mm
 
 Platemap:
 Plate				1
 
-	01	02	03	04	05	06	07	08	09	10	11	12	
+	02	03	04	05	06	07	08	09	10	11	12	
 A	  	  	  	  	  	  	  	  	  	  	  	  
 B	  	  	  	  	  	  	  	  	  	  	  	  
 C	  	  	  	  	  	  	  	  	  	  	  	  
 D	  	  	  	  	  	  	  	  	  	  	  	  
 E	  	  	  	  	  	  	  	  	  	  	  	  
 F	  	  	  	  	  	  	  	  	  	  	  	  
 G	  	  	  	  	  	  	  	  	  	  	  	-
```

### Comparing `clophfit-0.5.4/tests/EnSpire/M1-A6-G12_11columns.csv` & `clophfit-0.6.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv`

 * *Files 0% similar despite different names*

```diff
@@ -455,15 +455,14 @@
 H12	-	489	515	3206	
 H12	-	490	515	3266	
 H12	-	491	515	3414	
 H12	-	492	515	3702	
 H12	-	493	515	3606	
 H12	-	494	515	3911	
 H12	-	495	515	3993	
-
 Basic assay information 
 Assay ID: 				308
 Assay Started: 				2012-05-31 10:30:31
 Assay Finished: 				2012-05-31 10:39:25
 Assay Exported: 				2012-05-31 10:40:06
 Assay Started By: 				N/A
 Protocol ID: 				100115
@@ -500,15 +499,15 @@
 
 14.39 mm x------------------------------------------------------ x 113.38 mm
 74.24 mm                                                           74.24 mm
 
 Platemap:
 Plate				1
 
-	01	02	03	04	05	06	07	08	09	10	11	
+	01	02	03	04	05	06	07	08	09	10	11	12	
 A	  	  	  	  	  	  	  	  	  	  	  	  
 B	  	  	  	  	  	  	  	  	  	  	  	  
 C	  	  	  	  	  	  	  	  	  	  	  	  
 D	  	  	  	  	  	  	  	  	  	  	  	  
 E	  	  	  	  	  	  	  	  	  	  	  	  
 F	  	  	  	  	  	  	  	  	  	  	  	  
 G	  	  	  	  	  	  	  	  	  	  	  	-
```

### Comparing `clophfit-0.5.4/tests/EnSpire/M1-A6-G12_missing_emptyline_fin.csv` & `clophfit-0.6.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Plate information 
 Plate	Repeat	Barcode	Measurement date	Chamber temperature at start	Chamber temperature at end	Ambient temperature at start	Ambient temperature at end	
 1	1	=""	2012-05-31 10:39:13	19.6	19.65	3	1.8	
 
 
 No background information available.
 
-
 Well	Sample	MeasA:WavelengthExc	MeasA:WavelengthEms	MeasA:Result	
 G12	-	270	515	66953	
 G12	-	271	515	69382	
 G12	-	272	515	71492	
 G12	-	273	515	73537	
 G12	-	274	515	76078	
 G12	-	275	515	78199	
@@ -455,14 +454,15 @@
 H12	-	489	515	3206	
 H12	-	490	515	3266	
 H12	-	491	515	3414	
 H12	-	492	515	3702	
 H12	-	493	515	3606	
 H12	-	494	515	3911	
 H12	-	495	515	3993	
+
 Basic assay information 
 Assay ID: 				308
 Assay Started: 				2012-05-31 10:30:31
 Assay Finished: 				2012-05-31 10:39:25
 Assay Exported: 				2012-05-31 10:40:06
 Assay Started By: 				N/A
 Protocol ID: 				100115
```

### Comparing `clophfit-0.5.4/tests/EnSpire/e2-T-without_sample_column.csv` & `clophfit-0.6.0/tests/EnSpire/e2-T-without_sample_column.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/EnSpire/e2dan-emwavelength.csv` & `clophfit-0.6.0/tests/EnSpire/exceptions/e2dan-emwavelength.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/EnSpire/e2dan-exwavelength.csv` & `clophfit-0.6.0/tests/EnSpire/exceptions/e2dan-exwavelength.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/EnSpire/e2dan-exwavelength2.csv` & `clophfit-0.6.0/tests/EnSpire/exceptions/e2dan-exwavelength2.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/EnSpire/e2dan-exwavelengthstrange.csv` & `clophfit-0.6.0/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/EnSpire/h148g-spettroC-Efin.csv` & `clophfit-0.6.0/tests/EnSpire/h148g-spettroC.csv`

 * *Files 0% similar despite different names*

```diff
@@ -23043,320 +23043,320 @@
 0005a020: 0955 4e4b 3630 0938 3530 3636 0934 3936  .UNK60.85066.496
 0005a030: 0935 3230 090d 0a47 3035 0955 4e4b 3630  .520...G05.UNK60
 0005a040: 0938 3831 3431 0934 3937 0935 3230 090d  .88141.497.520..
 0005a050: 0a47 3035 0955 4e4b 3630 0939 3133 3536  .G05.UNK60.91356
 0005a060: 0934 3938 0935 3230 090d 0a47 3035 0955  .498.520...G05.U
 0005a070: 4e4b 3630 0939 3437 3430 0934 3939 0935  NK60.94740.499.5
 0005a080: 3230 090d 0a47 3035 0955 4e4b 3630 0939  20...G05.UNK60.9
-0005a090: 3736 3132 0935 3030 0935 3230 090d 0a42  7612.500.520...B
-0005a0a0: 6173 6963 2061 7373 6179 2069 6e66 6f72  asic assay infor
-0005a0b0: 6d61 7469 6f6e 200d 0a41 7373 6179 2049  mation ..Assay I
-0005a0c0: 443a 2009 0909 0934 300d 0a41 7373 6179  D: ....40..Assay
-0005a0d0: 2053 7461 7274 6564 3a20 0909 0909 3230   Started: ....20
-0005a0e0: 3131 2d31 302d 3033 2031 343a 3135 3a34  11-10-03 14:15:4
-0005a0f0: 340d 0a41 7373 6179 2046 696e 6973 6865  4..Assay Finishe
-0005a100: 643a 2009 0909 0932 3031 312d 3130 2d30  d: ....2011-10-0
-0005a110: 3320 3137 3a31 323a 3435 0d0a 4173 7361  3 17:12:45..Assa
-0005a120: 7920 4578 706f 7274 6564 3a20 0909 0909  y Exported: ....
-0005a130: 3230 3132 2d30 332d 3233 2031 313a 3437  2012-03-23 11:47
-0005a140: 3a33 330d 0a41 7373 6179 2053 7461 7274  :33..Assay Start
-0005a150: 6564 2042 793a 2009 0909 094e 2f41 0d0a  ed By: ....N/A..
-0005a160: 5072 6f74 6f63 6f6c 2049 443a 2009 0909  Protocol ID: ...
-0005a170: 0931 3030 3130 340d 0a50 726f 746f 636f  .100104..Protoco
-0005a180: 6c20 4e61 6d65 3a20 0909 0909 4563 6369  l Name: ....Ecci
-0005a190: 7461 7a69 6f6e 6520 430d 0a53 6572 6961  tazione C..Seria
-0005a1a0: 6c23 3a20 0909 0909 3d22 3233 3030 3034  l#: ....="230004
-0005a1b0: 3435 220d 0a0d 0a0d 0a0d 0a50 726f 746f  45"........Proto
-0005a1c0: 636f 6c20 696e 666f 726d 6174 696f 6e0d  col information.
-0005a1d0: 0a50 726f 746f 636f 6c3a 0d0a 5072 6f74  .Protocol:..Prot
-0005a1e0: 6f63 6f6c 206e 616d 6509 0909 0945 6363  ocol name....Ecc
-0005a1f0: 6974 617a 696f 6e65 2043 0d0a 4e75 6d62  itazione C..Numb
-0005a200: 6572 206f 6620 6173 7361 7920 7265 7065  er of assay repe
-0005a210: 6174 7309 0909 0931 0d0a 5374 6172 7420  ats....1..Start 
-0005a220: 6173 7361 7920 7265 7065 6174 2065 6163  assay repeat eac
-0005a230: 6809 0909 094e 2f41 0d0a 4e75 6d62 6572  h....N/A..Number
-0005a240: 206f 6620 706c 6174 6520 7265 7065 6174   of plate repeat
-0005a250: 7309 0909 0931 0d0a 5374 6172 7420 706c  s....1..Start pl
-0005a260: 6174 6520 7265 7065 6174 2065 6163 6809  ate repeat each.
-0005a270: 0909 094e 2f41 0d0a 4d6f 6465 206f 6620  ...N/A..Mode of 
-0005a280: 6d65 6173 7572 656d 656e 7409 0909 0942  measurement....B
-0005a290: 7920 526f 7773 2c20 6269 2d64 6972 6563  y Rows, bi-direc
-0005a2a0: 7469 6f6e 616c 0d0a 526f 7461 7465 6420  tional..Rotated 
-0005a2b0: 706c 6174 6509 0909 094e 6f0d 0a53 6f66  plate....No..Sof
-0005a2c0: 7420 6d6f 7665 0909 0909 4e6f 0d0a 5072  t move....No..Pr
-0005a2d0: 6f74 6f63 6f6c 206e 6f74 6573 0909 0909  otocol notes....
-0005a2e0: 5370 6574 7472 6f20 6563 6369 7461 7a69  Spettro eccitazi
-0005a2f0: 6f6e 650d 0a0d 0a50 6c61 7465 2074 7970  one....Plate typ
-0005a300: 653a 0d0a 4e61 6d65 206f 6620 7468 6520  e:..Name of the 
-0005a310: 706c 6174 6520 7479 7065 0909 0909 3936  plate type....96
-0005a320: 204f 7074 6950 6c61 7465 0d0a 4e75 6d62   OptiPlate..Numb
-0005a330: 6572 206f 6620 726f 7773 0909 0909 380d  er of rows....8.
-0005a340: 0a4e 756d 6265 7220 6f66 2063 6f6c 756d  .Number of colum
-0005a350: 6e73 0909 0909 3132 0d0a 4e75 6d62 6572  ns....12..Number
-0005a360: 206f 6620 7468 6520 7765 6c6c 7320 696e   of the wells in
-0005a370: 2074 6865 2070 6c61 7465 0909 0909 3936   the plate....96
-0005a380: 0d0a 4865 6967 6874 206f 6620 7468 6520  ..Height of the 
-0005a390: 706c 6174 6509 0909 0931 342e 3620 6d6d  plate....14.6 mm
-0005a3a0: 0d0a 4469 616d 6574 6572 206f 6620 7468  ..Diameter of th
-0005a3b0: 6520 7765 6c6c 0909 0909 372e 3133 206d  e well....7.13 m
-0005a3c0: 6d0d 0a56 6f6c 756d 6520 6f66 2074 6865  m..Volume of the
-0005a3d0: 2077 656c 6c09 0909 0933 3030 20b5 6c0d   well....300 .l.
-0005a3e0: 0a4f 7074 696d 697a 6564 0909 0909 4e2f  .Optimized....N/
-0005a3f0: 410d 0a0d 0a43 6f6f 7264 696e 6174 6573  A....Coordinates
-0005a400: 206f 6620 636f 726e 6572 733a 0d0a 3936   of corners:..96
-0005a410: 204f 7074 6950 6c61 7465 0d0a 3134 2e33   OptiPlate..14.3
-0005a420: 3820 6d6d 2078 2d2d 2d2d 2d2d 2d2d 2d2d  8 mm x----------
+0005a090: 3736 3132 0935 3030 0935 3230 090d 0a0d  7612.500.520....
+0005a0a0: 0a42 6173 6963 2061 7373 6179 2069 6e66  .Basic assay inf
+0005a0b0: 6f72 6d61 7469 6f6e 200d 0a41 7373 6179  ormation ..Assay
+0005a0c0: 2049 443a 2009 0909 0934 300d 0a41 7373   ID: ....40..Ass
+0005a0d0: 6179 2053 7461 7274 6564 3a20 0909 0909  ay Started: ....
+0005a0e0: 3230 3131 2d31 302d 3033 2031 343a 3135  2011-10-03 14:15
+0005a0f0: 3a34 340d 0a41 7373 6179 2046 696e 6973  :44..Assay Finis
+0005a100: 6865 643a 2009 0909 0932 3031 312d 3130  hed: ....2011-10
+0005a110: 2d30 3320 3137 3a31 323a 3435 0d0a 4173  -03 17:12:45..As
+0005a120: 7361 7920 4578 706f 7274 6564 3a20 0909  say Exported: ..
+0005a130: 0909 3230 3132 2d30 332d 3233 2031 313a  ..2012-03-23 11:
+0005a140: 3437 3a33 330d 0a41 7373 6179 2053 7461  47:33..Assay Sta
+0005a150: 7274 6564 2042 793a 2009 0909 094e 2f41  rted By: ....N/A
+0005a160: 0d0a 5072 6f74 6f63 6f6c 2049 443a 2009  ..Protocol ID: .
+0005a170: 0909 0931 3030 3130 340d 0a50 726f 746f  ...100104..Proto
+0005a180: 636f 6c20 4e61 6d65 3a20 0909 0909 4563  col Name: ....Ec
+0005a190: 6369 7461 7a69 6f6e 6520 430d 0a53 6572  citazione C..Ser
+0005a1a0: 6961 6c23 3a20 0909 0909 3d22 3233 3030  ial#: ....="2300
+0005a1b0: 3034 3435 220d 0a0d 0a0d 0a0d 0a50 726f  0445"........Pro
+0005a1c0: 746f 636f 6c20 696e 666f 726d 6174 696f  tocol informatio
+0005a1d0: 6e0d 0a50 726f 746f 636f 6c3a 0d0a 5072  n..Protocol:..Pr
+0005a1e0: 6f74 6f63 6f6c 206e 616d 6509 0909 0945  otocol name....E
+0005a1f0: 6363 6974 617a 696f 6e65 2043 0d0a 4e75  ccitazione C..Nu
+0005a200: 6d62 6572 206f 6620 6173 7361 7920 7265  mber of assay re
+0005a210: 7065 6174 7309 0909 0931 0d0a 5374 6172  peats....1..Star
+0005a220: 7420 6173 7361 7920 7265 7065 6174 2065  t assay repeat e
+0005a230: 6163 6809 0909 094e 2f41 0d0a 4e75 6d62  ach....N/A..Numb
+0005a240: 6572 206f 6620 706c 6174 6520 7265 7065  er of plate repe
+0005a250: 6174 7309 0909 0931 0d0a 5374 6172 7420  ats....1..Start 
+0005a260: 706c 6174 6520 7265 7065 6174 2065 6163  plate repeat eac
+0005a270: 6809 0909 094e 2f41 0d0a 4d6f 6465 206f  h....N/A..Mode o
+0005a280: 6620 6d65 6173 7572 656d 656e 7409 0909  f measurement...
+0005a290: 0942 7920 526f 7773 2c20 6269 2d64 6972  .By Rows, bi-dir
+0005a2a0: 6563 7469 6f6e 616c 0d0a 526f 7461 7465  ectional..Rotate
+0005a2b0: 6420 706c 6174 6509 0909 094e 6f0d 0a53  d plate....No..S
+0005a2c0: 6f66 7420 6d6f 7665 0909 0909 4e6f 0d0a  oft move....No..
+0005a2d0: 5072 6f74 6f63 6f6c 206e 6f74 6573 0909  Protocol notes..
+0005a2e0: 0909 5370 6574 7472 6f20 6563 6369 7461  ..Spettro eccita
+0005a2f0: 7a69 6f6e 650d 0a0d 0a50 6c61 7465 2074  zione....Plate t
+0005a300: 7970 653a 0d0a 4e61 6d65 206f 6620 7468  ype:..Name of th
+0005a310: 6520 706c 6174 6520 7479 7065 0909 0909  e plate type....
+0005a320: 3936 204f 7074 6950 6c61 7465 0d0a 4e75  96 OptiPlate..Nu
+0005a330: 6d62 6572 206f 6620 726f 7773 0909 0909  mber of rows....
+0005a340: 380d 0a4e 756d 6265 7220 6f66 2063 6f6c  8..Number of col
+0005a350: 756d 6e73 0909 0909 3132 0d0a 4e75 6d62  umns....12..Numb
+0005a360: 6572 206f 6620 7468 6520 7765 6c6c 7320  er of the wells 
+0005a370: 696e 2074 6865 2070 6c61 7465 0909 0909  in the plate....
+0005a380: 3936 0d0a 4865 6967 6874 206f 6620 7468  96..Height of th
+0005a390: 6520 706c 6174 6509 0909 0931 342e 3620  e plate....14.6 
+0005a3a0: 6d6d 0d0a 4469 616d 6574 6572 206f 6620  mm..Diameter of 
+0005a3b0: 7468 6520 7765 6c6c 0909 0909 372e 3133  the well....7.13
+0005a3c0: 206d 6d0d 0a56 6f6c 756d 6520 6f66 2074   mm..Volume of t
+0005a3d0: 6865 2077 656c 6c09 0909 0933 3030 20b5  he well....300 .
+0005a3e0: 6c0d 0a4f 7074 696d 697a 6564 0909 0909  l..Optimized....
+0005a3f0: 4e2f 410d 0a0d 0a43 6f6f 7264 696e 6174  N/A....Coordinat
+0005a400: 6573 206f 6620 636f 726e 6572 733a 0d0a  es of corners:..
+0005a410: 3936 204f 7074 6950 6c61 7465 0d0a 3134  96 OptiPlate..14
+0005a420: 2e33 3820 6d6d 2078 2d2d 2d2d 2d2d 2d2d  .38 mm x--------
 0005a430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0005a440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0005a450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2078 2031  ------------ x 1
-0005a460: 3133 2e33 3820 6d6d 0d0a 3131 2e32 3420  13.38 mm..11.24 
-0005a470: 6d6d 2020 2020 2020 2020 2020 2020 2020  mm              
+0005a450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2078  -------------- x
+0005a460: 2031 3133 2e33 3820 6d6d 0d0a 3131 2e32   113.38 mm..11.2
+0005a470: 3420 6d6d 2020 2020 2020 2020 2020 2020  4 mm            
 0005a480: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0005a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005a4a0: 2020 2020 2020 2020 2020 2020 2031 312e               11.
-0005a4b0: 3234 206d 6d0d 0a0d 0a31 342e 3339 206d  24 mm....14.39 m
-0005a4c0: 6d20 782d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  m x-------------
+0005a4a0: 2020 2020 2020 2020 2020 2020 2020 2031                 1
+0005a4b0: 312e 3234 206d 6d0d 0a0d 0a31 342e 3339  1.24 mm....14.39
+0005a4c0: 206d 6d20 782d 2d2d 2d2d 2d2d 2d2d 2d2d   mm x-----------
 0005a4d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0005a4e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0005a4f0: 2d2d 2d2d 2d2d 2d2d 2d20 7820 3131 332e  --------- x 113.
-0005a500: 3338 206d 6d0d 0a37 342e 3234 206d 6d20  38 mm..74.24 mm 
-0005a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005a4f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7820 3131  ----------- x 11
+0005a500: 332e 3338 206d 6d0d 0a37 342e 3234 206d  3.38 mm..74.24 m
+0005a510: 6d20 2020 2020 2020 2020 2020 2020 2020  m               
 0005a520: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0005a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005a540: 2020 2020 2020 2020 2020 3734 2e32 3420            74.24 
-0005a550: 6d6d 0d0a 0d0a 506c 6174 656d 6170 3a0d  mm....Platemap:.
-0005a560: 0a50 6c61 7465 0909 0909 310d 0a0d 0a09  .Plate....1.....
-0005a570: 3031 0930 3209 3033 0930 3409 3035 0930  01.02.03.04.05.0
-0005a580: 3609 3037 0930 3809 3039 0931 3009 3131  6.07.08.09.10.11
-0005a590: 0931 3209 0d0a 4109 554e 4b31 2009 554e  .12...A.UNK1 .UN
-0005a5a0: 4b32 2009 554e 4b33 2009 554e 4b34 2009  K2 .UNK3 .UNK4 .
-0005a5b0: 554e 4b35 2009 554e 4b36 2009 554e 4b37  UNK5 .UNK6 .UNK7
-0005a5c0: 2009 554e 4b38 2009 554e 4b39 2009 554e   .UNK8 .UNK9 .UN
-0005a5d0: 4b31 3009 554e 4b31 3109 2020 2020 200d  K10.UNK11.     .
-0005a5e0: 0a42 0955 4e4b 3132 0955 4e4b 3133 0955  .B.UNK12.UNK13.U
-0005a5f0: 4e4b 3134 0955 4e4b 3135 0955 4e4b 3136  NK14.UNK15.UNK16
-0005a600: 0955 4e4b 3137 0955 4e4b 3138 0955 4e4b  .UNK17.UNK18.UNK
-0005a610: 3139 0955 4e4b 3230 0955 4e4b 3231 0955  19.UNK20.UNK21.U
-0005a620: 4e4b 3232 0920 2020 2020 0d0a 4309 554e  NK22.     ..C.UN
-0005a630: 4b32 3309 554e 4b32 3409 554e 4b32 3509  K23.UNK24.UNK25.
-0005a640: 554e 4b32 3609 554e 4b32 3709 554e 4b32  UNK26.UNK27.UNK2
-0005a650: 3809 554e 4b32 3909 554e 4b33 3009 554e  8.UNK29.UNK30.UN
-0005a660: 4b33 3109 554e 4b33 3209 554e 4b33 3309  K31.UNK32.UNK33.
-0005a670: 2020 2020 200d 0a44 0955 4e4b 3334 0955       ..D.UNK34.U
-0005a680: 4e4b 3335 0955 4e4b 3336 0955 4e4b 3337  NK35.UNK36.UNK37
-0005a690: 0955 4e4b 3338 0955 4e4b 3339 0955 4e4b  .UNK38.UNK39.UNK
-0005a6a0: 3430 0955 4e4b 3431 0955 4e4b 3432 0955  40.UNK41.UNK42.U
-0005a6b0: 4e4b 3433 0955 4e4b 3434 0920 2020 2020  NK43.UNK44.     
-0005a6c0: 0d0a 4509 554e 4b34 3509 554e 4b34 3609  ..E.UNK45.UNK46.
-0005a6d0: 554e 4b34 3709 554e 4b34 3809 554e 4b34  UNK47.UNK48.UNK4
-0005a6e0: 3909 554e 4b35 3009 554e 4b35 3109 554e  9.UNK50.UNK51.UN
-0005a6f0: 4b35 3209 554e 4b35 3309 554e 4b35 3409  K52.UNK53.UNK54.
-0005a700: 554e 4b35 3509 2020 2020 200d 0a46 0955  UNK55.     ..F.U
-0005a710: 4e4b 3536 0955 4e4b 3537 0955 4e4b 3538  NK56.UNK57.UNK58
-0005a720: 0955 4e4b 3539 0955 4e4b 3630 0920 2020  .UNK59.UNK60.   
-0005a730: 2020 0920 2020 2020 0920 2020 2020 0920    .     .     . 
-0005a740: 2020 2020 0920 2020 2020 0920 2020 2020      .     .     
-0005a750: 0920 2020 2020 0d0a 4709 554e 4b35 3609  .     ..G.UNK56.
-0005a760: 554e 4b35 3709 554e 4b35 3809 554e 4b35  UNK57.UNK58.UNK5
-0005a770: 3909 554e 4b36 3009 2020 2020 2009 2020  9.UNK60.     .  
-0005a780: 2020 2009 2020 2020 2009 2020 2020 2009     .     .     .
-0005a790: 2020 2020 2009 2020 2020 2009 2020 2020       .     .    
-0005a7a0: 200d 0a48 0920 2020 2020 0920 2020 2020   ..H.     .     
-0005a7b0: 0920 2020 2020 0920 2020 2020 0920 2020  .     .     .   
-0005a7c0: 2020 0920 2020 2020 0920 2020 2020 0920    .     .     . 
-0005a7d0: 2020 2020 0920 2020 2020 0920 2020 2020      .     .     
-0005a7e0: 0920 2020 2020 0920 2020 2020 0d0a 0d0a  .     .     ....
-0005a7f0: 2055 4e4b 202d 2055 6e6b 6e6f 776e 0d0a   UNK - Unknown..
-0005a800: 0d0a 4361 6c63 756c 6174 696f 6e73 3a0d  ..Calculations:.
-0005a810: 0a4e 6f20 6361 6c63 756c 6174 696f 6e73  .No calculations
-0005a820: 2e0d 0a0d 0a41 7574 6f20 6578 706f 7274  .....Auto export
-0005a830: 2070 6172 616d 6574 6572 733a 0d0a 4578   parameters:..Ex
-0005a840: 706f 7274 2066 6f72 6d61 7409 0909 094c  port format....L
-0005a850: 6973 7443 0d0a 5069 6374 7572 6509 0909  istC..Picture...
-0005a860: 094e 6f0d 0a41 6464 2070 6c61 7465 206e  .No..Add plate n
-0005a870: 756d 6265 7220 746f 2074 6865 2066 696c  umber to the fil
-0005a880: 6520 6e61 6d65 0909 0909 5965 730d 0a45  e name....Yes..E
-0005a890: 6163 6820 706c 6174 6520 746f 2073 6570  ach plate to sep
-0005a8a0: 6172 6174 6520 6669 6c65 0909 0909 4e6f  arate file....No
-0005a8b0: 0d0a 4669 656c 6420 7365 7061 7261 746f  ..Field separato
-0005a8c0: 7220 746f 2075 7365 0909 0909 390d 0a46  r to use....9..F
-0005a8d0: 696c 6520 6e61 6d65 2066 6f72 6d61 7409  ile name format.
-0005a8e0: 0909 0943 3a5c 5573 6572 735c 5573 6572  ...C:\Users\User
-0005a8f0: 5c46 7261 6e63 6573 636f 5c3c 4461 7465  \Francesco\<Date
-0005a900: 3e5c 6831 3438 672d 7370 6574 7472 6f43  >\h148g-spettroC
-0005a910: 636f 6d70 6c65 746f 2e63 7376 0d0a 4578  completo.csv..Ex
-0005a920: 706f 7274 6564 2064 6174 6109 0909 0957  ported data....W
-0005a930: 656c 6c2c 5361 6d70 6c65 2c4d 6561 7341  ell,Sample,MeasA
-0005a940: 3a52 6573 756c 742c 4d65 6173 413a 5761  :Result,MeasA:Wa
-0005a950: 7665 6c65 6e67 7468 0d0a 0d0a 4f70 6572  velength....Oper
-0005a960: 6174 696f 6e73 3a0d 0a50 6c61 7465 2031  ations:..Plate 1
-0005a970: 0d0a 2020 5465 6d70 6572 6174 7572 6520  ..  Temperature 
-0005a980: 636f 6e74 726f 6c0d 0a20 2020 204d 6561  control..    Mea
-0005a990: 7375 7265 6d65 6e74 2063 6861 6d62 6572  surement chamber
-0005a9a0: 2074 656d 7065 7261 7475 7265 0909 0909   temperature....
-0005a9b0: 3230 20b0 430d 0a20 2020 2043 6f6e 6465  20 .C..    Conde
-0005a9c0: 6e73 6174 696f 6e20 7072 6576 656e 7469  nsation preventi
-0005a9d0: 6f6e 2066 6f72 2073 6561 6c65 6420 706c  on for sealed pl
-0005a9e0: 6174 6573 0909 0909 4e6f 0d0a 2020 2020  ates....No..    
-0005a9f0: 4661 7374 2073 7461 7274 0909 0909 5965  Fast start....Ye
-0005aa00: 730d 0a20 2020 2046 6173 7420 636f 6f6c  s..    Fast cool
-0005aa10: 696e 6709 0909 094e 6f0d 0a20 2020 2053  ing....No..    S
-0005aa20: 6574 2074 656d 7065 7261 7475 7265 2061  et temperature a
-0005aa30: 6e64 2063 6f6e 7469 6e75 6520 696d 6d65  nd continue imme
-0005aa40: 6469 6174 656c 7909 0909 094e 6f0d 0a20  diately....No.. 
-0005aa50: 2020 2053 6574 2074 656d 7065 7261 7475     Set temperatu
-0005aa60: 7265 2061 646a 7573 746d 656e 7420 6f66  re adjustment of
-0005aa70: 6609 0909 094e 6f0d 0a20 2020 2046 6972  f....No..    Fir
-0005aa80: 7374 2061 7373 6179 2f70 6c61 7465 2072  st assay/plate r
-0005aa90: 6570 6561 7420 6166 6665 6374 6564 0909  epeat affected..
-0005aaa0: 0909 310d 0a20 2053 6861 6b65 0d0a 2020  ..1..  Shake..  
-0005aab0: 2020 4475 7261 7469 6f6e 0909 0909 3520    Duration....5 
-0005aac0: 730d 0a20 2020 2053 7065 6564 0909 0909  s..    Speed....
-0005aad0: 3630 0d0a 2020 2020 4469 616d 6574 6572  60..    Diameter
-0005aae0: 0909 0909 3320 6d6d 0d0a 2020 2020 5368  ....3 mm..    Sh
-0005aaf0: 616b 6520 6d6f 6465 0909 0909 4c69 6e65  ake mode....Line
-0005ab00: 6172 0d0a 2020 2020 506c 6174 6520 6c6f  ar..    Plate lo
-0005ab10: 6361 7469 6f6e 0909 0909 496e 7369 6465  cation....Inside
-0005ab20: 0d0a 2020 2020 4669 7273 7420 6173 7361  ..    First assa
-0005ab30: 792f 706c 6174 6520 7265 7065 6174 2061  y/plate repeat a
-0005ab40: 6666 6563 7465 6409 0909 0931 0d0a 2020  ffected....1..  
-0005ab50: 2020 4c61 7374 2061 7373 6179 2f70 6c61    Last assay/pla
-0005ab60: 7465 2072 6570 6561 7420 6166 6665 6374  te repeat affect
-0005ab70: 6564 0909 0909 310d 0a20 2044 656c 6179  ed....1..  Delay
-0005ab80: 0d0a 2020 2020 4475 7261 7469 6f6e 0909  ..    Duration..
-0005ab90: 0909 3720 730d 0a20 2020 2050 6c61 7465  ..7 s..    Plate
-0005aba0: 206c 6f63 6174 696f 6e09 0909 0949 6e73   location....Ins
-0005abb0: 6964 650d 0a20 2020 2046 6972 7374 2061  ide..    First a
-0005abc0: 7373 6179 2f70 6c61 7465 2072 6570 6561  ssay/plate repea
-0005abd0: 7420 6166 6665 6374 6564 0909 0909 310d  t affected....1.
-0005abe0: 0a20 2020 204c 6173 7420 6173 7361 792f  .    Last assay/
-0005abf0: 706c 6174 6520 7265 7065 6174 2061 6666  plate repeat aff
-0005ac00: 6563 7465 6409 0909 0931 0d0a 2020 5370  ected....1..  Sp
-0005ac10: 6563 7472 756d 2073 6361 6e0d 0a20 2020  ectrum scan..   
-0005ac20: 204d 6561 7309 0909 0941 0d0a 2020 2020   Meas....A..    
-0005ac30: 5465 6368 0909 0909 466c 756f 7265 7363  Tech....Fluoresc
-0005ac40: 656e 6365 0d0a 2020 2020 4d6f 6e6f 6368  ence..    Monoch
-0005ac50: 726f 6d61 746f 7209 0909 0945 7863 6974  romator....Excit
-0005ac60: 6174 696f 6e0d 0a20 2020 204d 696e 2077  ation..    Min w
-0005ac70: 6176 656c 656e 6774 6809 0909 0932 3732  avelength....272
-0005ac80: 206e 6d0d 0a20 2020 204d 6178 2077 6176   nm..    Max wav
-0005ac90: 656c 656e 6774 6809 0909 0935 3030 206e  elength....500 n
-0005aca0: 6d0d 0a20 2020 2053 7465 7009 0909 0931  m..    Step....1
-0005acb0: 206e 6d0d 0a20 2020 204f 7468 6572 206d   nm..    Other m
-0005acc0: 6f6e 6f63 6872 6f6d 6174 6f72 0d0a 2020  onochromator..  
-0005acd0: 2020 5761 7665 6c65 6e67 7468 0909 0909    Wavelength....
-0005ace0: 3532 3020 6e6d 0d0a 0d0a 4d65 6173 7572  520 nm....Measur
-0005acf0: 656d 656e 7473 3a0d 0a4d 6561 7320 0909  ements:..Meas ..
-0005ad00: 0909 410d 0a45 7863 2e20 6669 6c74 6572  ..A..Exc. filter
-0005ad10: 0909 0909 4e2f 410d 0a55 7369 6e67 206f  ....N/A..Using o
-0005ad20: 6620 6578 6369 7461 7469 6f6e 2066 696c  f excitation fil
-0005ad30: 7465 7209 0909 0954 6f70 0d0a 4578 6369  ter....Top..Exci
-0005ad40: 7461 7469 6f6e 2077 6176 656c 656e 6774  tation wavelengt
-0005ad50: 6809 0909 0932 3732 206e 6d0d 0a45 6d69  h....272 nm..Emi
-0005ad60: 7373 696f 6e20 7761 7665 6c65 6e67 7468  ssion wavelength
-0005ad70: 0909 0909 3532 3020 6e6d 0d0a 4d65 6173  ....520 nm..Meas
-0005ad80: 7572 656d 656e 7420 6865 6967 6874 0909  urement height..
-0005ad90: 0909 3420 6d6d 0d0a 4e75 6d62 6572 206f  ..4 mm..Number o
-0005ada0: 6620 666c 6173 6865 7309 0909 0933 3030  f flashes....300
-0005adb0: 0d0a 4e75 6d62 6572 206f 6620 666c 6173  ..Number of flas
-0005adc0: 6865 7320 696e 7465 6772 6174 6564 0909  hes integrated..
-0005add0: 0909 3330 300d 0a46 6c61 7368 2070 6f77  ..300..Flash pow
-0005ade0: 6572 0909 0909 3130 3020 250d 0a45 7863  er....100 %..Exc
-0005adf0: 6974 6174 696f 6e20 6c69 6768 7409 0909  itation light...
-0005ae00: 0931 3030 250d 0a52 6566 6572 656e 6365  .100%..Reference
-0005ae10: 2065 7863 6974 6174 696f 6e20 6c69 6768   excitation ligh
-0005ae20: 7409 0909 0931 3030 250d 0a45 6d69 7373  t....100%..Emiss
-0005ae30: 696f 6e20 6c69 6768 7409 0909 0931 3030  ion light....100
-0005ae40: 250d 0a52 6566 6572 656e 6365 2041 4420  %..Reference AD 
-0005ae50: 6761 696e 0909 0909 320d 0a52 6566 6572  gain....2..Refer
-0005ae60: 656e 6365 2073 6967 6e61 6c09 0909 0931  ence signal....1
-0005ae70: 3032 3937 3932 3138 0d0a 4c61 7374 2065  02979218..Last e
-0005ae80: 6469 7465 6409 0909 0932 3031 312d 3039  dited....2011-09
-0005ae90: 2d33 3020 3131 3a34 383a 3030 0d0a 4c61  -30 11:48:00..La
-0005aea0: 7374 2065 6469 7465 6420 6279 0909 0909  st edited by....
-0005aeb0: 456e 5370 6972 650d 0a46 6163 746f 7279  EnSpire..Factory
-0005aec0: 2070 7265 7365 7409 0909 094e 6f0d 0a4f   preset....No..O
-0005aed0: 7074 696d 697a 6174 696f 6e73 0d0a 2020  ptimizations..  
-0005aee0: 4d65 6173 7572 656d 656e 7420 6865 6967  Measurement heig
-0005aef0: 6874 0909 0909 3230 3131 2d31 302d 3033  ht....2011-10-03
-0005af00: 2030 323a 3135 3a30 320d 0a20 2057 6176   02:15:02..  Wav
-0005af10: 656c 656e 6774 6809 0909 094e 2f41 0d0a  elength....N/A..
-0005af20: 2020 5a27 0909 0909 4e2f 410d 0a20 2046    Z'....N/A..  F
-0005af30: 6c61 7466 6965 6c64 0909 0909 4e2f 410d  latfield....N/A.
-0005af40: 0a0d 0a46 696c 7465 7273 3a0d 0a4d 6f6e  ...Filters:..Mon
-0005af50: 6f63 6872 6f6d 6174 6f72 2063 7574 6f66  ochromator cutof
-0005af60: 6620 3233 3009 0909 0931 3430 0d0a 4669  f 230....140..Fi
-0005af70: 6c74 6572 2070 6f6c 6172 697a 6174 696f  lter polarizatio
-0005af80: 6e09 0909 094e 6f6e 650d 0a44 6573 6372  n....None..Descr
-0005af90: 6970 7469 6f6e 0909 0909 5832 3330 636f  iption....X230co
-0005afa0: 204c 6f6e 6770 6173 733d 3233 306e 6d2c   Longpass=230nm,
-0005afb0: 2054 6d69 6e3d 3930 250d 0a55 7365 6420   Tmin=90%..Used 
-0005afc0: 7769 7468 0d0a 4c61 7374 2065 6469 7465  with..Last edite
-0005afd0: 6409 0909 0932 3031 302d 3031 2d31 300d  d....2010-01-10.
-0005afe0: 0a4c 6173 7420 6564 6974 6564 2062 7909  .Last edited by.
-0005aff0: 0909 0949 6e73 7461 6c6c 6174 696f 6e0d  ...Installation.
-0005b000: 0a46 6163 746f 7279 2070 7265 7365 7409  .Factory preset.
-0005b010: 0909 0959 6573 0d0a 0d0a 4d6f 6e6f 6368  ...Yes....Monoch
-0005b020: 726f 6d61 746f 7220 6375 746f 6666 2033  romator cutoff 3
-0005b030: 3630 0909 0909 3134 310d 0a46 696c 7465  60....141..Filte
-0005b040: 7220 706f 6c61 7269 7a61 7469 6f6e 0909  r polarization..
-0005b050: 0909 4e6f 6e65 0d0a 4465 7363 7269 7074  ..None..Descript
-0005b060: 696f 6e09 0909 0958 3336 3063 6f20 4c6f  ion....X360co Lo
-0005b070: 6e67 7061 7373 3d33 3630 6e6d 2c20 546d  ngpass=360nm, Tm
-0005b080: 696e 3d39 3025 0d0a 5573 6564 2077 6974  in=90%..Used wit
-0005b090: 680d 0a4c 6173 7420 6564 6974 6564 0909  h..Last edited..
-0005b0a0: 0909 3230 3130 2d30 312d 3130 0d0a 4c61  ..2010-01-10..La
-0005b0b0: 7374 2065 6469 7465 6420 6279 0909 0909  st edited by....
-0005b0c0: 496e 7374 616c 6c61 7469 6f6e 0d0a 4661  Installation..Fa
-0005b0d0: 6374 6f72 7920 7072 6573 6574 0909 0909  ctory preset....
-0005b0e0: 5965 730d 0a0d 0a4d 6f6e 6f63 6872 6f6d  Yes....Monochrom
-0005b0f0: 6174 6f72 2063 7574 6f66 6620 3538 3509  ator cutoff 585.
-0005b100: 0909 0931 3432 0d0a 4669 6c74 6572 2070  ...142..Filter p
-0005b110: 6f6c 6172 697a 6174 696f 6e09 0909 094e  olarization....N
-0005b120: 6f6e 650d 0a44 6573 6372 6970 7469 6f6e  one..Description
-0005b130: 0909 0909 5835 3835 636f 204c 6f6e 6770  ....X585co Longp
-0005b140: 6173 733d 3538 356e 6d2c 2054 6d69 6e3d  ass=585nm, Tmin=
-0005b150: 3735 250d 0a55 7365 6420 7769 7468 0d0a  75%..Used with..
-0005b160: 4c61 7374 2065 6469 7465 6409 0909 0932  Last edited....2
-0005b170: 3031 302d 3031 2d31 300d 0a4c 6173 7420  010-01-10..Last 
-0005b180: 6564 6974 6564 2062 7909 0909 0949 6e73  edited by....Ins
-0005b190: 7461 6c6c 6174 696f 6e0d 0a46 6163 746f  tallation..Facto
-0005b1a0: 7279 2070 7265 7365 7409 0909 0959 6573  ry preset....Yes
-0005b1b0: 0d0a 0d0a 496e 7374 7275 6d65 6e74 3a0d  ....Instrument:.
-0005b1c0: 0a53 6572 6961 6c20 6e75 6d62 6572 0909  .Serial number..
-0005b1d0: 0909 3233 3030 3034 3435 0d0a 4e69 636b  ..23000445..Nick
-0005b1e0: 6e61 6d65 0909 0909 456e 5370 6972 650d  name....EnSpire.
-0005b1f0: 0a0d 0a0d 0a0d 0a0d 0a4e 6f74 6966 6963  .........Notific
-0005b200: 6174 696f 6e73 2066 6f72 2070 6c61 7465  ations for plate
-0005b210: 2031 2c20 7265 7065 6174 2031 3a0d 0a57   1, repeat 1:..W
-0005b220: 4152 4e49 4e47 3a20 536f 6d65 206f 6620  ARNING: Some of 
-0005b230: 7468 6520 7265 7375 6c74 7320 6d61 7920  the results may 
-0005b240: 6265 2069 6e76 616c 6964 2064 7565 2074  be invalid due t
-0005b250: 6f20 7361 7475 7261 7469 6f6e 206f 6620  o saturation of 
-0005b260: 656c 6563 7472 6f6e 6963 732e 2054 6f20  electronics. To 
-0005b270: 6669 7820 7468 6520 7072 6f62 6c65 6d20  fix the problem 
-0005b280: 7472 7920 746f 206c 696d 6974 2074 6865  try to limit the
-0005b290: 2065 7863 6974 6174 696f 6e20 6c69 6768   excitation ligh
-0005b2a0: 7420 6f72 2064 6563 7265 6173 6520 7468  t or decrease th
-0005b2b0: 6520 6465 7465 6374 6f72 2067 6169 6e20  e detector gain 
-0005b2c0: 7573 696e 6720 7468 6520 6c61 6265 6c20  using the label 
-0005b2d0: 6564 6974 6f72 2e0a 496e 2061 2063 6173  editor..In a cas
-0005b2e0: 6520 6f66 206c 6162 656c 2075 7369 6e67  e of label using
-0005b2f0: 2046 6c75 6f72 6573 6365 6e63 6520 4d6f   Fluorescence Mo
-0005b300: 6e6f 6368 726f 6d61 746f 7220 796f 7520  nochromator you 
-0005b310: 6361 6e20 616c 736f 2074 7279 2074 6f20  can also try to 
-0005b320: 7573 6520 6c65 7373 2066 6c61 7368 6573  use less flashes
-0005b330: 2c20 6c6f 7765 7220 6578 6369 7461 7469  , lower excitati
-0005b340: 6f6e 2077 6176 656c 656e 6774 6820 6f72  on wavelength or
-0005b350: 2068 6967 6865 7220 656d 6973 7369 6f6e   higher emission
-0005b360: 2077 6176 656c 656e 6774 682e 0d0a 0d0a   wavelength.....
-0005b370: 5741 524e 494e 473a 204d 6561 7375 7265  WARNING: Measure
-0005b380: 6420 7369 676e 616c 2069 7320 7361 7475  d signal is satu
-0005b390: 7261 7465 6420 6f72 2074 6865 2073 616d  rated or the sam
-0005b3a0: 706c 6520 6973 2074 6f74 616c 6c79 206f  ple is totally o
-0005b3b0: 7061 7175 6520 696e 2074 6865 2066 6f6c  paque in the fol
-0005b3c0: 6c6f 7769 6e67 2077 656c 6c73 3a20 204d  lowing wells:  M
-0005b3d0: 4541 5320 413a 2042 3036 0d0a 0d0a 0d0a  EAS A: B06......
-0005b3e0: 0d0a 4578 706f 7274 6564 2077 6974 6820  ..Exported with 
-0005b3f0: 456e 5370 6972 6520 576f 726b 7374 6174  EnSpire Workstat
-0005b400: 696f 6e20 7665 7273 696f 6e20 342e 3130  ion version 4.10
-0005b410: 2e33 3030 352e 3134 3430 0d0a            .3005.1440..
+0005a540: 2020 2020 2020 2020 2020 2020 3734 2e32              74.2
+0005a550: 3420 6d6d 0d0a 0d0a 506c 6174 656d 6170  4 mm....Platemap
+0005a560: 3a0d 0a50 6c61 7465 0909 0909 310d 0a0d  :..Plate....1...
+0005a570: 0a09 3031 0930 3209 3033 0930 3409 3035  ..01.02.03.04.05
+0005a580: 0930 3609 3037 0930 3809 3039 0931 3009  .06.07.08.09.10.
+0005a590: 3131 0931 3209 0d0a 4109 554e 4b31 2009  11.12...A.UNK1 .
+0005a5a0: 554e 4b32 2009 554e 4b33 2009 554e 4b34  UNK2 .UNK3 .UNK4
+0005a5b0: 2009 554e 4b35 2009 554e 4b36 2009 554e   .UNK5 .UNK6 .UN
+0005a5c0: 4b37 2009 554e 4b38 2009 554e 4b39 2009  K7 .UNK8 .UNK9 .
+0005a5d0: 554e 4b31 3009 554e 4b31 3109 2020 2020  UNK10.UNK11.    
+0005a5e0: 200d 0a42 0955 4e4b 3132 0955 4e4b 3133   ..B.UNK12.UNK13
+0005a5f0: 0955 4e4b 3134 0955 4e4b 3135 0955 4e4b  .UNK14.UNK15.UNK
+0005a600: 3136 0955 4e4b 3137 0955 4e4b 3138 0955  16.UNK17.UNK18.U
+0005a610: 4e4b 3139 0955 4e4b 3230 0955 4e4b 3231  NK19.UNK20.UNK21
+0005a620: 0955 4e4b 3232 0920 2020 2020 0d0a 4309  .UNK22.     ..C.
+0005a630: 554e 4b32 3309 554e 4b32 3409 554e 4b32  UNK23.UNK24.UNK2
+0005a640: 3509 554e 4b32 3609 554e 4b32 3709 554e  5.UNK26.UNK27.UN
+0005a650: 4b32 3809 554e 4b32 3909 554e 4b33 3009  K28.UNK29.UNK30.
+0005a660: 554e 4b33 3109 554e 4b33 3209 554e 4b33  UNK31.UNK32.UNK3
+0005a670: 3309 2020 2020 200d 0a44 0955 4e4b 3334  3.     ..D.UNK34
+0005a680: 0955 4e4b 3335 0955 4e4b 3336 0955 4e4b  .UNK35.UNK36.UNK
+0005a690: 3337 0955 4e4b 3338 0955 4e4b 3339 0955  37.UNK38.UNK39.U
+0005a6a0: 4e4b 3430 0955 4e4b 3431 0955 4e4b 3432  NK40.UNK41.UNK42
+0005a6b0: 0955 4e4b 3433 0955 4e4b 3434 0920 2020  .UNK43.UNK44.   
+0005a6c0: 2020 0d0a 4509 554e 4b34 3509 554e 4b34    ..E.UNK45.UNK4
+0005a6d0: 3609 554e 4b34 3709 554e 4b34 3809 554e  6.UNK47.UNK48.UN
+0005a6e0: 4b34 3909 554e 4b35 3009 554e 4b35 3109  K49.UNK50.UNK51.
+0005a6f0: 554e 4b35 3209 554e 4b35 3309 554e 4b35  UNK52.UNK53.UNK5
+0005a700: 3409 554e 4b35 3509 2020 2020 200d 0a46  4.UNK55.     ..F
+0005a710: 0955 4e4b 3536 0955 4e4b 3537 0955 4e4b  .UNK56.UNK57.UNK
+0005a720: 3538 0955 4e4b 3539 0955 4e4b 3630 0920  58.UNK59.UNK60. 
+0005a730: 2020 2020 0920 2020 2020 0920 2020 2020      .     .     
+0005a740: 0920 2020 2020 0920 2020 2020 0920 2020  .     .     .   
+0005a750: 2020 0920 2020 2020 0d0a 4709 554e 4b35    .     ..G.UNK5
+0005a760: 3609 554e 4b35 3709 554e 4b35 3809 554e  6.UNK57.UNK58.UN
+0005a770: 4b35 3909 554e 4b36 3009 2020 2020 2009  K59.UNK60.     .
+0005a780: 2020 2020 2009 2020 2020 2009 2020 2020       .     .    
+0005a790: 2009 2020 2020 2009 2020 2020 2009 2020   .     .     .  
+0005a7a0: 2020 200d 0a48 0920 2020 2020 0920 2020     ..H.     .   
+0005a7b0: 2020 0920 2020 2020 0920 2020 2020 0920    .     .     . 
+0005a7c0: 2020 2020 0920 2020 2020 0920 2020 2020      .     .     
+0005a7d0: 0920 2020 2020 0920 2020 2020 0920 2020  .     .     .   
+0005a7e0: 2020 0920 2020 2020 0920 2020 2020 0d0a    .     .     ..
+0005a7f0: 0d0a 2055 4e4b 202d 2055 6e6b 6e6f 776e  .. UNK - Unknown
+0005a800: 0d0a 0d0a 4361 6c63 756c 6174 696f 6e73  ....Calculations
+0005a810: 3a0d 0a4e 6f20 6361 6c63 756c 6174 696f  :..No calculatio
+0005a820: 6e73 2e0d 0a0d 0a41 7574 6f20 6578 706f  ns.....Auto expo
+0005a830: 7274 2070 6172 616d 6574 6572 733a 0d0a  rt parameters:..
+0005a840: 4578 706f 7274 2066 6f72 6d61 7409 0909  Export format...
+0005a850: 094c 6973 7443 0d0a 5069 6374 7572 6509  .ListC..Picture.
+0005a860: 0909 094e 6f0d 0a41 6464 2070 6c61 7465  ...No..Add plate
+0005a870: 206e 756d 6265 7220 746f 2074 6865 2066   number to the f
+0005a880: 696c 6520 6e61 6d65 0909 0909 5965 730d  ile name....Yes.
+0005a890: 0a45 6163 6820 706c 6174 6520 746f 2073  .Each plate to s
+0005a8a0: 6570 6172 6174 6520 6669 6c65 0909 0909  eparate file....
+0005a8b0: 4e6f 0d0a 4669 656c 6420 7365 7061 7261  No..Field separa
+0005a8c0: 746f 7220 746f 2075 7365 0909 0909 390d  tor to use....9.
+0005a8d0: 0a46 696c 6520 6e61 6d65 2066 6f72 6d61  .File name forma
+0005a8e0: 7409 0909 0943 3a5c 5573 6572 735c 5573  t....C:\Users\Us
+0005a8f0: 6572 5c46 7261 6e63 6573 636f 5c3c 4461  er\Francesco\<Da
+0005a900: 7465 3e5c 6831 3438 672d 7370 6574 7472  te>\h148g-spettr
+0005a910: 6f43 636f 6d70 6c65 746f 2e63 7376 0d0a  oCcompleto.csv..
+0005a920: 4578 706f 7274 6564 2064 6174 6109 0909  Exported data...
+0005a930: 0957 656c 6c2c 5361 6d70 6c65 2c4d 6561  .Well,Sample,Mea
+0005a940: 7341 3a52 6573 756c 742c 4d65 6173 413a  sA:Result,MeasA:
+0005a950: 5761 7665 6c65 6e67 7468 0d0a 0d0a 4f70  Wavelength....Op
+0005a960: 6572 6174 696f 6e73 3a0d 0a50 6c61 7465  erations:..Plate
+0005a970: 2031 0d0a 2020 5465 6d70 6572 6174 7572   1..  Temperatur
+0005a980: 6520 636f 6e74 726f 6c0d 0a20 2020 204d  e control..    M
+0005a990: 6561 7375 7265 6d65 6e74 2063 6861 6d62  easurement chamb
+0005a9a0: 6572 2074 656d 7065 7261 7475 7265 0909  er temperature..
+0005a9b0: 0909 3230 20b0 430d 0a20 2020 2043 6f6e  ..20 .C..    Con
+0005a9c0: 6465 6e73 6174 696f 6e20 7072 6576 656e  densation preven
+0005a9d0: 7469 6f6e 2066 6f72 2073 6561 6c65 6420  tion for sealed 
+0005a9e0: 706c 6174 6573 0909 0909 4e6f 0d0a 2020  plates....No..  
+0005a9f0: 2020 4661 7374 2073 7461 7274 0909 0909    Fast start....
+0005aa00: 5965 730d 0a20 2020 2046 6173 7420 636f  Yes..    Fast co
+0005aa10: 6f6c 696e 6709 0909 094e 6f0d 0a20 2020  oling....No..   
+0005aa20: 2053 6574 2074 656d 7065 7261 7475 7265   Set temperature
+0005aa30: 2061 6e64 2063 6f6e 7469 6e75 6520 696d   and continue im
+0005aa40: 6d65 6469 6174 656c 7909 0909 094e 6f0d  mediately....No.
+0005aa50: 0a20 2020 2053 6574 2074 656d 7065 7261  .    Set tempera
+0005aa60: 7475 7265 2061 646a 7573 746d 656e 7420  ture adjustment 
+0005aa70: 6f66 6609 0909 094e 6f0d 0a20 2020 2046  off....No..    F
+0005aa80: 6972 7374 2061 7373 6179 2f70 6c61 7465  irst assay/plate
+0005aa90: 2072 6570 6561 7420 6166 6665 6374 6564   repeat affected
+0005aaa0: 0909 0909 310d 0a20 2053 6861 6b65 0d0a  ....1..  Shake..
+0005aab0: 2020 2020 4475 7261 7469 6f6e 0909 0909      Duration....
+0005aac0: 3520 730d 0a20 2020 2053 7065 6564 0909  5 s..    Speed..
+0005aad0: 0909 3630 0d0a 2020 2020 4469 616d 6574  ..60..    Diamet
+0005aae0: 6572 0909 0909 3320 6d6d 0d0a 2020 2020  er....3 mm..    
+0005aaf0: 5368 616b 6520 6d6f 6465 0909 0909 4c69  Shake mode....Li
+0005ab00: 6e65 6172 0d0a 2020 2020 506c 6174 6520  near..    Plate 
+0005ab10: 6c6f 6361 7469 6f6e 0909 0909 496e 7369  location....Insi
+0005ab20: 6465 0d0a 2020 2020 4669 7273 7420 6173  de..    First as
+0005ab30: 7361 792f 706c 6174 6520 7265 7065 6174  say/plate repeat
+0005ab40: 2061 6666 6563 7465 6409 0909 0931 0d0a   affected....1..
+0005ab50: 2020 2020 4c61 7374 2061 7373 6179 2f70      Last assay/p
+0005ab60: 6c61 7465 2072 6570 6561 7420 6166 6665  late repeat affe
+0005ab70: 6374 6564 0909 0909 310d 0a20 2044 656c  cted....1..  Del
+0005ab80: 6179 0d0a 2020 2020 4475 7261 7469 6f6e  ay..    Duration
+0005ab90: 0909 0909 3720 730d 0a20 2020 2050 6c61  ....7 s..    Pla
+0005aba0: 7465 206c 6f63 6174 696f 6e09 0909 0949  te location....I
+0005abb0: 6e73 6964 650d 0a20 2020 2046 6972 7374  nside..    First
+0005abc0: 2061 7373 6179 2f70 6c61 7465 2072 6570   assay/plate rep
+0005abd0: 6561 7420 6166 6665 6374 6564 0909 0909  eat affected....
+0005abe0: 310d 0a20 2020 204c 6173 7420 6173 7361  1..    Last assa
+0005abf0: 792f 706c 6174 6520 7265 7065 6174 2061  y/plate repeat a
+0005ac00: 6666 6563 7465 6409 0909 0931 0d0a 2020  ffected....1..  
+0005ac10: 5370 6563 7472 756d 2073 6361 6e0d 0a20  Spectrum scan.. 
+0005ac20: 2020 204d 6561 7309 0909 0941 0d0a 2020     Meas....A..  
+0005ac30: 2020 5465 6368 0909 0909 466c 756f 7265    Tech....Fluore
+0005ac40: 7363 656e 6365 0d0a 2020 2020 4d6f 6e6f  scence..    Mono
+0005ac50: 6368 726f 6d61 746f 7209 0909 0945 7863  chromator....Exc
+0005ac60: 6974 6174 696f 6e0d 0a20 2020 204d 696e  itation..    Min
+0005ac70: 2077 6176 656c 656e 6774 6809 0909 0932   wavelength....2
+0005ac80: 3732 206e 6d0d 0a20 2020 204d 6178 2077  72 nm..    Max w
+0005ac90: 6176 656c 656e 6774 6809 0909 0935 3030  avelength....500
+0005aca0: 206e 6d0d 0a20 2020 2053 7465 7009 0909   nm..    Step...
+0005acb0: 0931 206e 6d0d 0a20 2020 204f 7468 6572  .1 nm..    Other
+0005acc0: 206d 6f6e 6f63 6872 6f6d 6174 6f72 0d0a   monochromator..
+0005acd0: 2020 2020 5761 7665 6c65 6e67 7468 0909      Wavelength..
+0005ace0: 0909 3532 3020 6e6d 0d0a 0d0a 4d65 6173  ..520 nm....Meas
+0005acf0: 7572 656d 656e 7473 3a0d 0a4d 6561 7320  urements:..Meas 
+0005ad00: 0909 0909 410d 0a45 7863 2e20 6669 6c74  ....A..Exc. filt
+0005ad10: 6572 0909 0909 4e2f 410d 0a55 7369 6e67  er....N/A..Using
+0005ad20: 206f 6620 6578 6369 7461 7469 6f6e 2066   of excitation f
+0005ad30: 696c 7465 7209 0909 0954 6f70 0d0a 4578  ilter....Top..Ex
+0005ad40: 6369 7461 7469 6f6e 2077 6176 656c 656e  citation wavelen
+0005ad50: 6774 6809 0909 0932 3732 206e 6d0d 0a45  gth....272 nm..E
+0005ad60: 6d69 7373 696f 6e20 7761 7665 6c65 6e67  mission waveleng
+0005ad70: 7468 0909 0909 3532 3020 6e6d 0d0a 4d65  th....520 nm..Me
+0005ad80: 6173 7572 656d 656e 7420 6865 6967 6874  asurement height
+0005ad90: 0909 0909 3420 6d6d 0d0a 4e75 6d62 6572  ....4 mm..Number
+0005ada0: 206f 6620 666c 6173 6865 7309 0909 0933   of flashes....3
+0005adb0: 3030 0d0a 4e75 6d62 6572 206f 6620 666c  00..Number of fl
+0005adc0: 6173 6865 7320 696e 7465 6772 6174 6564  ashes integrated
+0005add0: 0909 0909 3330 300d 0a46 6c61 7368 2070  ....300..Flash p
+0005ade0: 6f77 6572 0909 0909 3130 3020 250d 0a45  ower....100 %..E
+0005adf0: 7863 6974 6174 696f 6e20 6c69 6768 7409  xcitation light.
+0005ae00: 0909 0931 3030 250d 0a52 6566 6572 656e  ...100%..Referen
+0005ae10: 6365 2065 7863 6974 6174 696f 6e20 6c69  ce excitation li
+0005ae20: 6768 7409 0909 0931 3030 250d 0a45 6d69  ght....100%..Emi
+0005ae30: 7373 696f 6e20 6c69 6768 7409 0909 0931  ssion light....1
+0005ae40: 3030 250d 0a52 6566 6572 656e 6365 2041  00%..Reference A
+0005ae50: 4420 6761 696e 0909 0909 320d 0a52 6566  D gain....2..Ref
+0005ae60: 6572 656e 6365 2073 6967 6e61 6c09 0909  erence signal...
+0005ae70: 0931 3032 3937 3932 3138 0d0a 4c61 7374  .102979218..Last
+0005ae80: 2065 6469 7465 6409 0909 0932 3031 312d   edited....2011-
+0005ae90: 3039 2d33 3020 3131 3a34 383a 3030 0d0a  09-30 11:48:00..
+0005aea0: 4c61 7374 2065 6469 7465 6420 6279 0909  Last edited by..
+0005aeb0: 0909 456e 5370 6972 650d 0a46 6163 746f  ..EnSpire..Facto
+0005aec0: 7279 2070 7265 7365 7409 0909 094e 6f0d  ry preset....No.
+0005aed0: 0a4f 7074 696d 697a 6174 696f 6e73 0d0a  .Optimizations..
+0005aee0: 2020 4d65 6173 7572 656d 656e 7420 6865    Measurement he
+0005aef0: 6967 6874 0909 0909 3230 3131 2d31 302d  ight....2011-10-
+0005af00: 3033 2030 323a 3135 3a30 320d 0a20 2057  03 02:15:02..  W
+0005af10: 6176 656c 656e 6774 6809 0909 094e 2f41  avelength....N/A
+0005af20: 0d0a 2020 5a27 0909 0909 4e2f 410d 0a20  ..  Z'....N/A.. 
+0005af30: 2046 6c61 7466 6965 6c64 0909 0909 4e2f   Flatfield....N/
+0005af40: 410d 0a0d 0a46 696c 7465 7273 3a0d 0a4d  A....Filters:..M
+0005af50: 6f6e 6f63 6872 6f6d 6174 6f72 2063 7574  onochromator cut
+0005af60: 6f66 6620 3233 3009 0909 0931 3430 0d0a  off 230....140..
+0005af70: 4669 6c74 6572 2070 6f6c 6172 697a 6174  Filter polarizat
+0005af80: 696f 6e09 0909 094e 6f6e 650d 0a44 6573  ion....None..Des
+0005af90: 6372 6970 7469 6f6e 0909 0909 5832 3330  cription....X230
+0005afa0: 636f 204c 6f6e 6770 6173 733d 3233 306e  co Longpass=230n
+0005afb0: 6d2c 2054 6d69 6e3d 3930 250d 0a55 7365  m, Tmin=90%..Use
+0005afc0: 6420 7769 7468 0d0a 4c61 7374 2065 6469  d with..Last edi
+0005afd0: 7465 6409 0909 0932 3031 302d 3031 2d31  ted....2010-01-1
+0005afe0: 300d 0a4c 6173 7420 6564 6974 6564 2062  0..Last edited b
+0005aff0: 7909 0909 0949 6e73 7461 6c6c 6174 696f  y....Installatio
+0005b000: 6e0d 0a46 6163 746f 7279 2070 7265 7365  n..Factory prese
+0005b010: 7409 0909 0959 6573 0d0a 0d0a 4d6f 6e6f  t....Yes....Mono
+0005b020: 6368 726f 6d61 746f 7220 6375 746f 6666  chromator cutoff
+0005b030: 2033 3630 0909 0909 3134 310d 0a46 696c   360....141..Fil
+0005b040: 7465 7220 706f 6c61 7269 7a61 7469 6f6e  ter polarization
+0005b050: 0909 0909 4e6f 6e65 0d0a 4465 7363 7269  ....None..Descri
+0005b060: 7074 696f 6e09 0909 0958 3336 3063 6f20  ption....X360co 
+0005b070: 4c6f 6e67 7061 7373 3d33 3630 6e6d 2c20  Longpass=360nm, 
+0005b080: 546d 696e 3d39 3025 0d0a 5573 6564 2077  Tmin=90%..Used w
+0005b090: 6974 680d 0a4c 6173 7420 6564 6974 6564  ith..Last edited
+0005b0a0: 0909 0909 3230 3130 2d30 312d 3130 0d0a  ....2010-01-10..
+0005b0b0: 4c61 7374 2065 6469 7465 6420 6279 0909  Last edited by..
+0005b0c0: 0909 496e 7374 616c 6c61 7469 6f6e 0d0a  ..Installation..
+0005b0d0: 4661 6374 6f72 7920 7072 6573 6574 0909  Factory preset..
+0005b0e0: 0909 5965 730d 0a0d 0a4d 6f6e 6f63 6872  ..Yes....Monochr
+0005b0f0: 6f6d 6174 6f72 2063 7574 6f66 6620 3538  omator cutoff 58
+0005b100: 3509 0909 0931 3432 0d0a 4669 6c74 6572  5....142..Filter
+0005b110: 2070 6f6c 6172 697a 6174 696f 6e09 0909   polarization...
+0005b120: 094e 6f6e 650d 0a44 6573 6372 6970 7469  .None..Descripti
+0005b130: 6f6e 0909 0909 5835 3835 636f 204c 6f6e  on....X585co Lon
+0005b140: 6770 6173 733d 3538 356e 6d2c 2054 6d69  gpass=585nm, Tmi
+0005b150: 6e3d 3735 250d 0a55 7365 6420 7769 7468  n=75%..Used with
+0005b160: 0d0a 4c61 7374 2065 6469 7465 6409 0909  ..Last edited...
+0005b170: 0932 3031 302d 3031 2d31 300d 0a4c 6173  .2010-01-10..Las
+0005b180: 7420 6564 6974 6564 2062 7909 0909 0949  t edited by....I
+0005b190: 6e73 7461 6c6c 6174 696f 6e0d 0a46 6163  nstallation..Fac
+0005b1a0: 746f 7279 2070 7265 7365 7409 0909 0959  tory preset....Y
+0005b1b0: 6573 0d0a 0d0a 496e 7374 7275 6d65 6e74  es....Instrument
+0005b1c0: 3a0d 0a53 6572 6961 6c20 6e75 6d62 6572  :..Serial number
+0005b1d0: 0909 0909 3233 3030 3034 3435 0d0a 4e69  ....23000445..Ni
+0005b1e0: 636b 6e61 6d65 0909 0909 456e 5370 6972  ckname....EnSpir
+0005b1f0: 650d 0a0d 0a0d 0a0d 0a0d 0a4e 6f74 6966  e..........Notif
+0005b200: 6963 6174 696f 6e73 2066 6f72 2070 6c61  ications for pla
+0005b210: 7465 2031 2c20 7265 7065 6174 2031 3a0d  te 1, repeat 1:.
+0005b220: 0a57 4152 4e49 4e47 3a20 536f 6d65 206f  .WARNING: Some o
+0005b230: 6620 7468 6520 7265 7375 6c74 7320 6d61  f the results ma
+0005b240: 7920 6265 2069 6e76 616c 6964 2064 7565  y be invalid due
+0005b250: 2074 6f20 7361 7475 7261 7469 6f6e 206f   to saturation o
+0005b260: 6620 656c 6563 7472 6f6e 6963 732e 2054  f electronics. T
+0005b270: 6f20 6669 7820 7468 6520 7072 6f62 6c65  o fix the proble
+0005b280: 6d20 7472 7920 746f 206c 696d 6974 2074  m try to limit t
+0005b290: 6865 2065 7863 6974 6174 696f 6e20 6c69  he excitation li
+0005b2a0: 6768 7420 6f72 2064 6563 7265 6173 6520  ght or decrease 
+0005b2b0: 7468 6520 6465 7465 6374 6f72 2067 6169  the detector gai
+0005b2c0: 6e20 7573 696e 6720 7468 6520 6c61 6265  n using the labe
+0005b2d0: 6c20 6564 6974 6f72 2e0a 496e 2061 2063  l editor..In a c
+0005b2e0: 6173 6520 6f66 206c 6162 656c 2075 7369  ase of label usi
+0005b2f0: 6e67 2046 6c75 6f72 6573 6365 6e63 6520  ng Fluorescence 
+0005b300: 4d6f 6e6f 6368 726f 6d61 746f 7220 796f  Monochromator yo
+0005b310: 7520 6361 6e20 616c 736f 2074 7279 2074  u can also try t
+0005b320: 6f20 7573 6520 6c65 7373 2066 6c61 7368  o use less flash
+0005b330: 6573 2c20 6c6f 7765 7220 6578 6369 7461  es, lower excita
+0005b340: 7469 6f6e 2077 6176 656c 656e 6774 6820  tion wavelength 
+0005b350: 6f72 2068 6967 6865 7220 656d 6973 7369  or higher emissi
+0005b360: 6f6e 2077 6176 656c 656e 6774 682e 0d0a  on wavelength...
+0005b370: 0d0a 5741 524e 494e 473a 204d 6561 7375  ..WARNING: Measu
+0005b380: 7265 6420 7369 676e 616c 2069 7320 7361  red signal is sa
+0005b390: 7475 7261 7465 6420 6f72 2074 6865 2073  turated or the s
+0005b3a0: 616d 706c 6520 6973 2074 6f74 616c 6c79  ample is totally
+0005b3b0: 206f 7061 7175 6520 696e 2074 6865 2066   opaque in the f
+0005b3c0: 6f6c 6c6f 7769 6e67 2077 656c 6c73 3a20  ollowing wells: 
+0005b3d0: 204d 4541 5320 413a 2042 3036 0d0a 0d0a   MEAS A: B06....
+0005b3e0: 0d0a 0d0a 4578 706f 7274 6564 2077 6974  ....Exported wit
+0005b3f0: 6820 456e 5370 6972 6520 576f 726b 7374  h EnSpire Workst
+0005b400: 6174 696f 6e20 7665 7273 696f 6e20 342e  ation version 4.
+0005b410: 3130 2e33 3030 352e 3134 3430 0d0a       10.3005.1440..
```

### Comparing `clophfit-0.5.4/tests/EnSpire/h148g-spettroC-idx0.csv` & `clophfit-0.6.0/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/EnSpire/h148g-spettroC-idx2.csv` & `clophfit-0.6.0/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/EnSpire/h148g-spettroC-incomplete.csv` & `clophfit-0.6.0/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/EnSpire/h148g-spettroC-nota` & `clophfit-0.6.0/tests/EnSpire/h148g-spettroC-nota`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/EnSpire/h148g-spettroC-nota-Err` & `clophfit-0.6.0/tests/EnSpire/h148g-spettroC-nota-Err`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/EnSpire/data/NTT_37C_pKa.csv` & `clophfit-0.6.0/tests/EnSpire/cli/NTT_37C_pKa.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/EnSpire/data/output/NTT_37C_pKa_A.csv` & `clophfit-0.6.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/EnSpire/data/output/NTT_37C_pKa_A.png` & `clophfit-0.6.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/EnSpire/data/output/NTT_37C_pKa_B.csv` & `clophfit-0.6.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/EnSpire/data/output/NTT_37C_pKa_B.png` & `clophfit-0.6.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/290212_100.xls` & `clophfit-0.6.0/tests/Tecan/290212_100.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/290212_150.xls` & `clophfit-0.6.0/tests/Tecan/290212_150.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/290212_20.xls` & `clophfit-0.6.0/tests/Tecan/290212_20.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/290212_5.78.xls` & `clophfit-0.6.0/tests/Tecan/290212_5.78.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/290212_50.xls` & `clophfit-0.6.0/tests/Tecan/290212_50.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/290212_6.38.xls` & `clophfit-0.6.0/tests/Tecan/290212_6.38.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/290212_6.83.xls` & `clophfit-0.6.0/tests/Tecan/290212_6.83.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/290212_7.24.xls` & `clophfit-0.6.0/tests/Tecan/290212_7.24.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/290212_7.67.xls` & `clophfit-0.6.0/tests/Tecan/290212_7.67.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/290212_8.23.xls` & `clophfit-0.6.0/tests/Tecan/290212_8.23.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/290212_8.82.xls` & `clophfit-0.6.0/tests/Tecan/290212_8.82.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/290212_9.31.xls` & `clophfit-0.6.0/tests/Tecan/290212_9.31.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/290513_5.5.xls` & `clophfit-0.6.0/tests/Tecan/290513_5.5.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/290513_5.5_bad.xls` & `clophfit-0.6.0/tests/Tecan/290513_5.5_bad.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/290513_7.2.xls` & `clophfit-0.6.0/tests/Tecan/290513_7.2.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/290513_8.8.xls` & `clophfit-0.6.0/tests/Tecan/290513_8.8.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/200214 pH data.ods` & `clophfit-0.6.0/tests/Tecan/140220/200214 pH data.ods`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/NaCl1_200214.xls` & `clophfit-0.6.0/tests/Tecan/140220/NaCl1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/NaCl2_200214.xls` & `clophfit-0.6.0/tests/Tecan/140220/NaCl2_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/NaCl3_200214.xls` & `clophfit-0.6.0/tests/Tecan/140220/NaCl3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/NaCl4_200214.xls` & `clophfit-0.6.0/tests/Tecan/140220/NaCl4_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/NaCl5_200214.xls` & `clophfit-0.6.0/tests/Tecan/140220/NaCl5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/NaCl6_200214.xls` & `clophfit-0.6.0/tests/Tecan/140220/NaCl6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/NaCl7_200214.xls` & `clophfit-0.6.0/tests/Tecan/140220/NaCl7_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/NaCl8_200214.xls` & `clophfit-0.6.0/tests/Tecan/140220/NaCl8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/fit0-1.csv` & `clophfit-0.6.0/tests/Tecan/140220/fit0-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/fit0.csv` & `clophfit-0.6.0/tests/Tecan/140220/fit0.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/fit1-1.csv` & `clophfit-0.6.0/tests/Tecan/140220/fit1-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/fit1.csv` & `clophfit-0.6.0/tests/Tecan/140220/fit1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/pH5.0_200214.xls` & `clophfit-0.6.0/tests/Tecan/140220/pH5.0_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/pH5.8_200214.xls` & `clophfit-0.6.0/tests/Tecan/140220/pH5.8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/pH6.5_200214.xls` & `clophfit-0.6.0/tests/Tecan/140220/pH6.5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/pH7.1_200214.xls` & `clophfit-0.6.0/tests/Tecan/140220/pH7.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/pH7.6_200214.xls` & `clophfit-0.6.0/tests/Tecan/140220/pH7.6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/pH8.3_200214.xls` & `clophfit-0.6.0/tests/Tecan/140220/pH8.3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/140220/pH9.1_200214.xls` & `clophfit-0.6.0/tests/Tecan/140220/pH9.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx` & `clophfit-0.6.0/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls` & `clophfit-0.6.0/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/exceptions/84wells_290212_20.xlsx` & `clophfit-0.6.0/tests/Tecan/exceptions/84wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/Tecan/exceptions/88wells_290212_20.xlsx` & `clophfit-0.6.0/tests/Tecan/exceptions/88wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/A01-20140311a.dat` & `clophfit-0.6.0/tests/data/A01-20140311a.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/A01.dat` & `clophfit-0.6.0/tests/data/A01.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/NTT-A04-Cl_note` & `clophfit-0.6.0/tests/data/NTT-A04-Cl_note`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/Meas/A04 Cl_A.csv` & `clophfit-0.6.0/tests/data/Meas/A04 Cl_A.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/Meas/A04 Cl_A.png` & `clophfit-0.6.0/tests/data/Meas/A04 Cl_A.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/Meas/A04 Cl_B.csv` & `clophfit-0.6.0/tests/data/Meas/A04 Cl_B.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/Meas/A04 Cl_B.png` & `clophfit-0.6.0/tests/data/Meas/A04 Cl_B.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/Meas/A04 Cl_C.csv` & `clophfit-0.6.0/tests/data/Meas/A04 Cl_C.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/Meas/A04 Cl_C.png` & `clophfit-0.6.0/tests/data/Meas/A04 Cl_C.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/Meas/A04 Cl_D.csv` & `clophfit-0.6.0/tests/data/Meas/A04 Cl_D.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/Meas/A04 Cl_D.png` & `clophfit-0.6.0/tests/data/Meas/A04 Cl_D.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/Meas/A04 Cl_E.csv` & `clophfit-0.6.0/tests/data/Meas/A04 Cl_E.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/Meas/A04 Cl_E.png` & `clophfit-0.6.0/tests/data/Meas/A04 Cl_E.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/Meas/A04 Cl_F.csv` & `clophfit-0.6.0/tests/data/Meas/A04 Cl_F.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/Meas/A04 Cl_F.png` & `clophfit-0.6.0/tests/data/Meas/A04 Cl_F.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/k/D05.dat-bs.png` & `clophfit-0.6.0/tests/data/k/D05.dat-bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/k/D05.dat.png` & `clophfit-0.6.0/tests/data/k/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.6.0/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.6.0/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.6.0/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.6.0/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/output/global/Cl/B05-20130628-cor.dat.png` & `clophfit-0.6.0/tests/data/output/global/Cl/B05-20130628-cor.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/tests/data/output/global/pH/D05.dat.png` & `clophfit-0.6.0/tests/data/output/global/pH/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/.gitignore` & `clophfit-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/LICENSE.txt` & `clophfit-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.5.4/README.md` & `clophfit-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.6354112.svg)](https://doi.org/10.5281/zenodo.6354112)
 
 This package provides a command line interface for fitting pH titration or
 binding assay data for macromolecules, such as fluorescence spectra. With this
 tool, users can easily analyze their data and obtain accurate fitting results.
 
-- Version: "0.5.4"
+- Version: "0.6.0"
 
 ## Installation
 
 You can get the library directly from
 [PyPI](https://pypi.org/project/ClopHfit/):
 
     pip install clophfit
```

### Comparing `clophfit-0.5.4/pyproject.toml` & `clophfit-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -44,19 +44,19 @@
   "macromolecule binding"
 ]
 license = "BSD-3-Clause"
 license-files = {paths = ["LICENSE.txt"]}
 name = "clophfit"
 readme = "README.md"
 requires-python = ">=3.8, <3.12"
-version = "0.5.4"
+version = "0.6.0"
 
 [project.optional-dependencies]
 dev = [
-  "commitizen < 3.2.2",
+  "commitizen < 3.2.3",
   "ipykernel",
   "jupyter",
   "ruff == 0.0.265",
   "pylsp-mypy",
   "python-lsp-ruff"
 ]
 docs = [
@@ -106,15 +106,15 @@
 '''
 line-length = 88
 skip-string-normalization = false
 
 [tool.commitizen]
 name = "cz_customize"
 tag_format = "v$version"
-version = "0.5.4"
+version = "0.6.0"
 version_files = [
   "pyproject.toml:version",
   "docs/conf.py:release",
   "README.md:Version"
 ]
 
 [tool.commitizen.customize]
@@ -169,17 +169,15 @@
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.report]
 # fail_under = 100
 exclude_lines = [
-  "pragma: no cover",
-  "pytest.raises",
-  "pytest.warns"
+  "pragma: no cover"
 ]
 show_missing = true
 
 [tool.coverage.run]
 branch = true
 omit = ["*__init__.py"]
 source = ["clophfit", "tests"]
```

### Comparing `clophfit-0.5.4/PKG-INFO` & `clophfit-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clophfit
-Version: 0.5.4
+Version: 0.6.0
 Summary: Cli for fitting macromolecule pH titration or binding assays data e.g. fluorescence spectra.
 Project-URL: Bug Tracker, https://github.com/darosio/ClopHfit/issues
 Project-URL: Changelog, https://darosio.github.io/ClopHfit/misc/CHANGELOG.html
 Project-URL: Discussions, https://github.com/darosio/ClopHfit/discussions
 Project-URL: Documentation, https://clophfit.readthedocs.io
 Project-URL: Github releases, https://github.com/darosio/ClopHfit/releases
 Project-URL: Homepage, https://github.com/darosio/ClopHfit
@@ -35,15 +35,15 @@
 Requires-Dist: rpy2<3.5.12
 Requires-Dist: scipy<1.10.2
 Requires-Dist: seaborn<0.12.3
 Requires-Dist: sympy<1.13.0
 Requires-Dist: tqdm<4.65.1
 Requires-Dist: xlrd<2.0.2
 Provides-Extra: dev
-Requires-Dist: commitizen<3.2.2; extra == 'dev'
+Requires-Dist: commitizen<3.2.3; extra == 'dev'
 Requires-Dist: ipykernel; extra == 'dev'
 Requires-Dist: jupyter; extra == 'dev'
 Requires-Dist: pylsp-mypy; extra == 'dev'
 Requires-Dist: python-lsp-ruff; extra == 'dev'
 Requires-Dist: ruff==0.0.265; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: autodocsumm==0.2.11; extra == 'docs'
@@ -71,15 +71,15 @@
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.6354112.svg)](https://doi.org/10.5281/zenodo.6354112)
 
 This package provides a command line interface for fitting pH titration or
 binding assay data for macromolecules, such as fluorescence spectra. With this
 tool, users can easily analyze their data and obtain accurate fitting results.
 
-- Version: "0.5.4"
+- Version: "0.6.0"
 
 ## Installation
 
 You can get the library directly from
 [PyPI](https://pypi.org/project/ClopHfit/):
 
     pip install clophfit
```

