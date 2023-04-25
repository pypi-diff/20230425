# Comparing `tmp/arch-5.4.0.tar.gz` & `tmp/arch-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arch-5.4.0.tar", last modified: Wed Apr 12 18:04:55 2023, max compression
+gzip compressed data, was "arch-5.5.0.tar", last modified: Tue Apr 25 13:26:04 2023, max compression
```

## Comparing `arch-5.4.0.tar` & `arch-5.5.0.tar`

### file list

```diff
@@ -1,295 +1,295 @@
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.458027 arch-5.4.0/
--rw-r--r--   0 kevin     (1000) kevin     (1000)       38 2022-03-22 08:30:31.000000 arch-5.4.0/.codacy.yml
--rw-r--r--   0 kevin     (1000) kevin     (1000)       17 2022-03-22 08:30:31.000000 arch-5.4.0/.codebeatignore
--rw-r--r--   0 kevin     (1000) kevin     (1000)      839 2022-08-15 08:35:45.000000 arch-5.4.0/.coveragerc
--rw-r--r--   0 kevin     (1000) kevin     (1000)       30 2021-07-22 17:04:35.000000 arch-5.4.0/.gitattributes
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.418027 arch-5.4.0/.github/
--rw-r--r--   0 kevin     (1000) kevin     (1000)       33 2023-04-12 18:03:48.000000 arch-5.4.0/.github/codeql.yml
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.418027 arch-5.4.0/.github/workflows/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      878 2023-04-12 18:03:48.000000 arch-5.4.0/.github/workflows/codeql.yml
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1195 2023-04-12 18:03:48.000000 arch-5.4.0/.github/workflows/generate-documentation.yml
--rw-r--r--   0 kevin     (1000) kevin     (1000)      286 2022-03-22 08:30:31.000000 arch-5.4.0/.gitignore
--rw-r--r--   0 kevin     (1000) kevin     (1000)       73 2021-07-22 17:04:35.000000 arch-5.4.0/.landscape.yml
--rw-r--r--   0 kevin     (1000) kevin     (1000)      432 2021-07-22 17:04:35.000000 arch-5.4.0/.pep8speaks.yml
--rw-r--r--   0 kevin     (1000) kevin     (1000)      674 2023-04-12 18:03:48.000000 arch-5.4.0/.readthedocs.yaml
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1660 2022-08-15 08:35:45.000000 arch-5.4.0/LICENSE.md
--rw-r--r--   0 kevin     (1000) kevin     (1000)      276 2022-03-22 08:30:31.000000 arch-5.4.0/MANIFEST.in
--rw-r--r--   0 kevin     (1000) kevin     (1000)    12027 2023-04-12 18:04:55.458027 arch-5.4.0/PKG-INFO
--rw-r--r--   0 kevin     (1000) kevin     (1000)    11203 2022-08-15 08:35:45.000000 arch-5.4.0/README.md
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1137 2023-04-12 18:03:48.000000 arch-5.4.0/appveyor.yml
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.388027 arch-5.4.0/arch/
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.388027 arch-5.4.0/arch/__future__/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.4.0/arch/__future__/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      654 2021-07-22 17:04:35.000000 arch-5.4.0/arch/__future__/_utility.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.4.0/arch/__future__/reindexing.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      300 2022-03-22 08:30:31.000000 arch-5.4.0/arch/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      160 2023-04-12 18:04:55.000000 arch-5.4.0/arch/_version.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.418027 arch-5.4.0/arch/bootstrap/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      804 2021-07-22 17:04:35.000000 arch-5.4.0/arch/bootstrap/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)   970405 2023-04-12 18:04:53.000000 arch-5.4.0/arch/bootstrap/_samplers.c
--rw-r--r--   0 kevin     (1000) kevin     (1000)      155 2021-07-22 17:04:35.000000 arch-5.4.0/arch/bootstrap/_samplers.pyi
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1169 2022-08-15 08:35:45.000000 arch-5.4.0/arch/bootstrap/_samplers.pyx
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1104 2021-07-22 17:04:35.000000 arch-5.4.0/arch/bootstrap/_samplers_python.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    65342 2023-04-12 18:03:48.000000 arch-5.4.0/arch/bootstrap/base.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    29910 2023-04-12 18:03:48.000000 arch-5.4.0/arch/bootstrap/multiple_comparison.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.388027 arch-5.4.0/arch/compat/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.4.0/arch/compat/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1196 2021-07-22 17:04:35.000000 arch-5.4.0/arch/compat/numba.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      311 2022-08-15 08:35:45.000000 arch-5.4.0/arch/compat/pandas.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      326 2021-07-22 17:04:35.000000 arch-5.4.0/arch/compat/statsmodels.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      947 2021-07-22 17:04:35.000000 arch-5.4.0/arch/conftest.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.388027 arch-5.4.0/arch/covariance/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.4.0/arch/covariance/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    18250 2023-04-12 18:03:48.000000 arch-5.4.0/arch/covariance/kernel.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.388027 arch-5.4.0/arch/data/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.4.0/arch/data/__init__.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.388027 arch-5.4.0/arch/data/binary/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      348 2021-07-22 17:04:35.000000 arch-5.4.0/arch/data/binary/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1609 2021-07-22 17:04:35.000000 arch-5.4.0/arch/data/binary/binary.csv.gz
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.388027 arch-5.4.0/arch/data/core_cpi/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      362 2023-04-12 18:03:48.000000 arch-5.4.0/arch/data/core_cpi/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2749 2021-07-22 17:04:35.000000 arch-5.4.0/arch/data/core_cpi/core-cpi.csv.gz
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.388027 arch-5.4.0/arch/data/crude/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      359 2023-04-12 18:03:48.000000 arch-5.4.0/arch/data/crude/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3078 2021-07-22 17:04:35.000000 arch-5.4.0/arch/data/crude/crude.csv.gz
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.388027 arch-5.4.0/arch/data/default/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      326 2023-04-12 18:03:48.000000 arch-5.4.0/arch/data/default/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6572 2021-07-22 17:04:35.000000 arch-5.4.0/arch/data/default/default.csv.gz
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.388027 arch-5.4.0/arch/data/frenchdata/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      492 2023-04-12 18:03:48.000000 arch-5.4.0/arch/data/frenchdata/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    10817 2021-07-22 17:04:35.000000 arch-5.4.0/arch/data/frenchdata/frenchdata.csv.gz
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.388027 arch-5.4.0/arch/data/nasdaq/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      336 2023-04-12 18:03:48.000000 arch-5.4.0/arch/data/nasdaq/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)   114929 2021-07-22 17:04:35.000000 arch-5.4.0/arch/data/nasdaq/nasdaq.csv.gz
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.388027 arch-5.4.0/arch/data/sp500/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      326 2023-04-12 18:03:48.000000 arch-5.4.0/arch/data/sp500/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)   102735 2021-07-22 17:04:35.000000 arch-5.4.0/arch/data/sp500/sp500.csv.gz
--rw-r--r--   0 kevin     (1000) kevin     (1000)      695 2021-07-22 17:04:35.000000 arch-5.4.0/arch/data/utility.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.388027 arch-5.4.0/arch/data/vix/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      296 2023-04-12 18:03:48.000000 arch-5.4.0/arch/data/vix/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6031 2021-07-22 17:04:35.000000 arch-5.4.0/arch/data/vix/vix.csv.gz
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.388027 arch-5.4.0/arch/data/wti/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      376 2023-04-12 18:03:48.000000 arch-5.4.0/arch/data/wti/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    39069 2021-07-22 17:04:35.000000 arch-5.4.0/arch/data/wti/wti.csv.gz
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.4.0/arch/py.typed
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.398027 arch-5.4.0/arch/tests/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/__init__.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.398027 arch-5.4.0/arch/tests/bootstrap/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/bootstrap/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      935 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/bootstrap/test_block_length.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    33640 2022-03-21 10:25:11.000000 arch-5.4.0/arch/tests/bootstrap/test_bootstrap.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    18339 2022-08-15 08:35:45.000000 arch-5.4.0/arch/tests/bootstrap/test_multiple_comparison.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.398027 arch-5.4.0/arch/tests/covariance/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/covariance/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     8699 2023-04-12 18:03:48.000000 arch-5.4.0/arch/tests/covariance/test_covariance.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      717 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/test_compat.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      501 2022-08-15 08:35:45.000000 arch-5.4.0/arch/tests/test_data.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2049 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/test_examples.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      629 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/test_tester.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.398027 arch-5.4.0/arch/tests/unitroot/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/unitroot/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2251 2023-04-12 18:03:48.000000 arch-5.4.0/arch/tests/unitroot/cointegration_data.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.398027 arch-5.4.0/arch/tests/unitroot/data/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/unitroot/data/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)   223090 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/unitroot/data/zivot-andrews.csv
--rw-r--r--   0 kevin     (1000) kevin     (1000)     7262 2022-03-21 10:25:11.000000 arch-5.4.0/arch/tests/unitroot/test_dynamic_ols.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     8998 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/unitroot/test_engle_granger.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    13322 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/unitroot/test_fmols_ccr.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6111 2022-03-21 10:25:11.000000 arch-5.4.0/arch/tests/unitroot/test_phillips_ouliaris.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    25212 2022-08-15 08:35:45.000000 arch-5.4.0/arch/tests/unitroot/test_unitroot.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.408027 arch-5.4.0/arch/tests/univariate/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/univariate/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5680 2022-08-15 08:35:45.000000 arch-5.4.0/arch/tests/univariate/test_arch_in_mean.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      288 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/univariate/test_base.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     7354 2022-08-15 08:35:45.000000 arch-5.4.0/arch/tests/univariate/test_distribution.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    37254 2022-08-15 08:35:45.000000 arch-5.4.0/arch/tests/univariate/test_forecast.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    49861 2023-04-12 18:03:48.000000 arch-5.4.0/arch/tests/univariate/test_mean.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2412 2023-04-12 18:03:48.000000 arch-5.4.0/arch/tests/univariate/test_moment.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    46010 2022-08-15 08:35:45.000000 arch-5.4.0/arch/tests/univariate/test_recursions.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2022 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/univariate/test_rescale.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    81881 2022-08-15 08:35:45.000000 arch-5.4.0/arch/tests/univariate/test_variance_forecasting.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    60204 2022-08-15 08:35:45.000000 arch-5.4.0/arch/tests/univariate/test_volatility.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.408027 arch-5.4.0/arch/tests/utility/
--rw-r--r--   0 kevin     (1000) kevin     (1000)       21 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/utility/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9195 2022-08-15 08:35:45.000000 arch-5.4.0/arch/tests/utility/test_array.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2360 2023-04-12 18:03:48.000000 arch-5.4.0/arch/tests/utility/test_cov.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      572 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/utility/test_io.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3582 2022-08-15 08:35:45.000000 arch-5.4.0/arch/tests/utility/test_timeseries.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      188 2021-07-22 17:04:35.000000 arch-5.4.0/arch/tests/utility/test_utility.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2200 2022-08-15 08:35:45.000000 arch-5.4.0/arch/typing.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.408027 arch-5.4.0/arch/unitroot/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      413 2021-07-22 17:04:35.000000 arch-5.4.0/arch/unitroot/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9585 2022-08-15 08:35:45.000000 arch-5.4.0/arch/unitroot/_engle_granger.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    16960 2022-08-15 08:35:45.000000 arch-5.4.0/arch/unitroot/_phillips_ouliaris.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     7668 2022-08-15 08:35:45.000000 arch-5.4.0/arch/unitroot/_shared.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    40919 2023-04-12 18:03:48.000000 arch-5.4.0/arch/unitroot/cointegration.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.408027 arch-5.4.0/arch/unitroot/critical_values/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.4.0/arch/unitroot/critical_values/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1320 2021-07-22 17:04:35.000000 arch-5.4.0/arch/unitroot/critical_values/dfgls.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    12737 2022-08-15 08:35:45.000000 arch-5.4.0/arch/unitroot/critical_values/dickey_fuller.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    22746 2021-07-22 17:04:35.000000 arch-5.4.0/arch/unitroot/critical_values/engle_granger.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3415 2021-07-22 17:04:35.000000 arch-5.4.0/arch/unitroot/critical_values/kpss.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    93787 2021-07-22 17:04:35.000000 arch-5.4.0/arch/unitroot/critical_values/phillips_ouliaris.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.428027 arch-5.4.0/arch/unitroot/critical_values/simulation/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2144 2022-08-15 08:35:45.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/adf_simulation.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3356 2023-04-12 18:03:48.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/adf_z_critical_values_simulation.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3863 2022-03-21 10:25:11.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/adf_z_critical_values_simulation_joblib.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4308 2022-08-15 08:35:45.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/adf_z_critical_values_simulation_large_cluster.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2336 2022-08-15 08:35:45.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/adf_z_simlation_process.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4333 2022-08-15 08:35:45.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/dfgls_critical_values_simulation.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4346 2022-03-21 10:25:11.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/dfgls_simulation_process.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)       43 2021-07-22 17:04:35.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/eg_setup.bat
--rw-r--r--   0 kevin     (1000) kevin     (1000)       45 2021-07-22 17:04:35.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/eg_setup.ps1
--rw-r--r--   0 kevin     (1000) kevin     (1000)       96 2021-07-22 17:04:35.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/eg_setup.sh
--rw-r--r--   0 kevin     (1000) kevin     (1000)     7497 2023-04-12 18:03:48.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/engle_granger_simulation.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4728 2021-07-22 17:04:35.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/engle_granger_simulation_process.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3162 2022-03-21 10:25:11.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/kpss_critical_values_simulation.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1721 2023-04-12 18:03:48.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/kpss_simulation_process.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    10613 2023-04-12 18:03:48.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/phillips-ouliaris-simulation-process.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    13181 2022-08-15 08:35:45.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/phillips-ouliaris-simulation.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      731 2021-07-22 17:04:35.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/phillips_ouliaris.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)       23 2021-07-22 17:04:35.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/requirements.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4447 2022-08-15 08:35:45.000000 arch-5.4.0/arch/unitroot/critical_values/simulation/shared.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3897 2021-07-22 17:04:35.000000 arch-5.4.0/arch/unitroot/critical_values/zivot_andrews.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    69616 2022-08-15 08:35:45.000000 arch-5.4.0/arch/unitroot/unitroot.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.428027 arch-5.4.0/arch/univariate/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1148 2021-07-22 17:04:35.000000 arch-5.4.0/arch/univariate/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    75620 2022-08-15 08:35:45.000000 arch-5.4.0/arch/univariate/base.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    40955 2022-08-15 08:35:45.000000 arch-5.4.0/arch/univariate/distribution.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    70285 2023-04-12 18:03:48.000000 arch-5.4.0/arch/univariate/mean.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)  1822633 2023-04-12 18:04:54.000000 arch-5.4.0/arch/univariate/recursions.c
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3792 2022-08-15 08:35:45.000000 arch-5.4.0/arch/univariate/recursions.pyi
--rw-r--r--   0 kevin     (1000) kevin     (1000)    35368 2022-08-15 08:35:45.000000 arch-5.4.0/arch/univariate/recursions.pyx
--rw-r--r--   0 kevin     (1000) kevin     (1000)    33857 2023-04-12 18:03:48.000000 arch-5.4.0/arch/univariate/recursions_python.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)   121906 2023-04-12 18:03:48.000000 arch-5.4.0/arch/univariate/volatility.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.418027 arch-5.4.0/arch/utility/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1536 2021-07-22 17:04:35.000000 arch-5.4.0/arch/utility/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9358 2023-04-12 18:03:48.000000 arch-5.4.0/arch/utility/array.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1761 2022-08-15 08:35:45.000000 arch-5.4.0/arch/utility/cov.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2093 2021-07-22 17:04:35.000000 arch-5.4.0/arch/utility/exceptions.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      668 2022-08-15 08:35:45.000000 arch-5.4.0/arch/utility/io.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2158 2022-08-15 08:35:45.000000 arch-5.4.0/arch/utility/testing.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5445 2022-08-15 08:35:45.000000 arch-5.4.0/arch/utility/timeseries.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.418027 arch-5.4.0/arch/vendor/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      215 2021-07-22 17:04:35.000000 arch-5.4.0/arch/vendor/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6011 2022-08-15 08:35:45.000000 arch-5.4.0/arch/vendor/property_cached.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.418027 arch-5.4.0/arch.egg-info/
--rw-r--r--   0 kevin     (1000) kevin     (1000)    12027 2023-04-12 18:04:55.000000 arch-5.4.0/arch.egg-info/PKG-INFO
--rw-r--r--   0 kevin     (1000) kevin     (1000)    11964 2023-04-12 18:04:55.000000 arch-5.4.0/arch.egg-info/SOURCES.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2023-04-12 18:04:55.000000 arch-5.4.0/arch.egg-info/dependency_links.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2023-04-12 18:04:54.000000 arch-5.4.0/arch.egg-info/not-zip-safe
--rw-r--r--   0 kevin     (1000) kevin     (1000)       76 2023-04-12 18:04:55.000000 arch-5.4.0/arch.egg-info/requires.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)        5 2023-04-12 18:04:55.000000 arch-5.4.0/arch.egg-info/top_level.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)      671 2021-07-22 17:04:35.000000 arch-5.4.0/azure-pipelines.yml
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.428027 arch-5.4.0/ci/
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.428027 arch-5.4.0/ci/azure/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5342 2023-04-12 18:03:48.000000 arch-5.4.0/ci/azure/azure_template_posix.yml
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1632 2023-04-12 18:03:48.000000 arch-5.4.0/ci/azure/azure_template_windows.yml
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1135 2023-04-12 18:03:48.000000 arch-5.4.0/ci/azure/install-posix.sh
--rw-r--r--   0 kevin     (1000) kevin     (1000)       68 2021-07-22 17:04:35.000000 arch-5.4.0/ci/azure/update_path.sh
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.428027 arch-5.4.0/ci/github-actions/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1342 2021-07-22 17:04:35.000000 arch-5.4.0/ci/github-actions/push-docs-gh-pages.sh
--rw-r--r--   0 kevin     (1000) kevin     (1000)      258 2021-07-22 17:04:35.000000 arch-5.4.0/ci/install-statsmodels-main.sh
--rw-r--r--   0 kevin     (1000) kevin     (1000)      490 2022-03-21 10:25:11.000000 arch-5.4.0/ci/performance.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.428027 arch-5.4.0/doc/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      646 2021-07-22 17:04:35.000000 arch-5.4.0/doc/Makefile
--rw-r--r--   0 kevin     (1000) kevin     (1000)      757 2021-07-22 17:04:35.000000 arch-5.4.0/doc/make.bat
--rw-r--r--   0 kevin     (1000) kevin     (1000)      449 2023-04-12 18:03:48.000000 arch-5.4.0/doc/requirements.txt
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.428027 arch-5.4.0/doc/source/
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.428027 arch-5.4.0/doc/source/_static/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_static/.gitignore
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.428027 arch-5.4.0/doc/source/_static/css/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      184 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_static/css/small_fixes.css
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.438027 arch-5.4.0/doc/source/_static/images/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1207 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_static/images/android-chrome-192x192.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2174 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_static/images/android-chrome-512x512.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1101 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_static/images/apple-touch-icon.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)      266 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_static/images/browserconfig.xml
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3349 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_static/images/color-logo-256.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)      904 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_static/images/favicon-16x16.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1105 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_static/images/favicon-32x32.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1144 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_static/images/mstile-150x150.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)      991 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_static/images/safari-pinned-tab.svg
--rw-r--r--   0 kevin     (1000) kevin     (1000)      474 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_static/images/site.webmanifest
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.438027 arch-5.4.0/doc/source/_templates/
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.438027 arch-5.4.0/doc/source/_templates/autosummary/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      117 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_templates/autosummary/attribute.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      843 2022-03-21 10:25:11.000000 arch-5.4.0/doc/source/_templates/autosummary/class.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      118 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_templates/autosummary/member.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      117 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_templates/autosummary/method.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      113 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_templates/autosummary/minimal_module.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1193 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/_templates/layout.html
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2550 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/api.rst
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.438027 arch-5.4.0/doc/source/bootstrap/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1336 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/bootstrap/background.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      926 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/bootstrap/bootstrap.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)    13853 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/bootstrap/bootstrap_histogram.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)    10086 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/bootstrap/confidence-intervals.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      781 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/bootstrap/iid-bootstraps.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2429 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/bootstrap/low-level-interface.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2155 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/bootstrap/parameter-covariance-estimation.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6414 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/bootstrap/semiparametric-parametric-bootstrap.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      908 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/bootstrap/timeseries-bootstraps.rst
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.438027 arch-5.4.0/doc/source/changes/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      468 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/changes/1.0.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)      341 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/changes/2.0.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)      846 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/changes/3.0.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9167 2022-03-21 10:25:11.000000 arch-5.4.0/doc/source/changes/4.0.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3539 2023-04-12 18:03:48.000000 arch-5.4.0/doc/source/changes/5.0.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)      169 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/changes.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9790 2023-04-12 18:03:48.000000 arch-5.4.0/doc/source/conf.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.438027 arch-5.4.0/doc/source/covariance/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      563 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/covariance/covariance.rst
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.448027 arch-5.4.0/doc/source/images/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     7192 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/images/bw-logo.svg
--rw-r--r--   0 kevin     (1000) kevin     (1000)     7102 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/images/color-logo-no-text.svg
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6435 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/images/color-logo-unprocessed.svg
--rw-r--r--   0 kevin     (1000) kevin     (1000)    15514 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/images/color-logo.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)     8225 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/images/color-logo.svg
--rw-r--r--   0 kevin     (1000) kevin     (1000)    15086 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/images/favicon.ico
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4536 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/images/favicon.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2034 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/images/favicon.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1998 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/images/favicon.svg
--rw-r--r--   0 kevin     (1000) kevin     (1000)    46243 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/images/hero.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1376 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/images/hero.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)   116976 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/images/hero.svg
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1998 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/images/logo.svg
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1544 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/index.rst
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.448027 arch-5.4.0/doc/source/multiple-comparison/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      622 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/multiple-comparison/background.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2215 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/multiple-comparison/multiple-comparison-reference.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      557 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/multiple-comparison/multiple-comparisons.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      444 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/names_wordlist.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2386 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/spelling_wordlist.txt
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.448027 arch-5.4.0/doc/source/unitroot/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      616 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/unitroot/cointegration.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1952 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/unitroot/introduction.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      371 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/unitroot/tests.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1830 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/unitroot/unitroot.rst
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.448027 arch-5.4.0/doc/source/univariate/
--rw-r--r--   0 kevin     (1000) kevin     (1000)       64 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/univariate/background.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      532 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/univariate/distribution.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9556 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/univariate/forecasting.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4987 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/univariate/introduction.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1087 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/univariate/mean.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      474 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/univariate/results.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1024 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/univariate/univariate.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      277 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/univariate/utility.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1440 2021-07-22 17:04:35.000000 arch-5.4.0/doc/source/univariate/volatility.rst
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-12 18:04:55.458027 arch-5.4.0/examples/
--rw-r--r--   0 kevin     (1000) kevin     (1000)    49989 2022-03-21 10:25:11.000000 arch-5.4.0/examples/bootstrap_examples.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)   166071 2022-03-21 10:25:11.000000 arch-5.4.0/examples/multiple-comparison_examples.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)   493128 2021-07-22 17:04:35.000000 arch-5.4.0/examples/unitroot_cointegration_examples.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)   191311 2021-07-22 17:04:35.000000 arch-5.4.0/examples/unitroot_examples.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)   214078 2021-07-22 17:04:35.000000 arch-5.4.0/examples/univariate_forecasting_with_exogenous_variables.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6087 2023-04-12 18:03:48.000000 arch-5.4.0/examples/univariate_using_fixed_variance.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)   517387 2021-07-22 17:04:35.000000 arch-5.4.0/examples/univariate_volatility_forecasting.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)   763575 2023-04-12 18:03:48.000000 arch-5.4.0/examples/univariate_volatility_modeling.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)   752792 2023-04-12 18:03:48.000000 arch-5.4.0/examples/univariate_volatility_scenarios.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)       75 2022-03-22 08:30:31.000000 arch-5.4.0/lgtm.yml
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2022-08-15 08:35:45.000000 arch-5.4.0/py.typed
--rw-r--r--   0 kevin     (1000) kevin     (1000)      457 2023-04-12 18:03:48.000000 arch-5.4.0/pyproject.toml
--rw-r--r--   0 kevin     (1000) kevin     (1000)      458 2023-04-12 18:03:48.000000 arch-5.4.0/requirements-dev.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)       76 2021-07-22 17:04:35.000000 arch-5.4.0/requirements.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2748 2023-04-12 18:04:55.458027 arch-5.4.0/setup.cfg
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6506 2023-04-12 18:03:48.000000 arch-5.4.0/setup.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.205133 arch-5.5.0/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       38 2022-03-22 08:30:31.000000 arch-5.5.0/.codacy.yml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       17 2022-03-22 08:30:31.000000 arch-5.5.0/.codebeatignore
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      839 2022-08-15 08:35:45.000000 arch-5.5.0/.coveragerc
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       30 2021-07-22 17:04:35.000000 arch-5.5.0/.gitattributes
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.145133 arch-5.5.0/.github/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       33 2023-04-12 18:03:48.000000 arch-5.5.0/.github/codeql.yml
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.145133 arch-5.5.0/.github/workflows/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      878 2023-04-12 18:03:48.000000 arch-5.5.0/.github/workflows/codeql.yml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1198 2023-04-25 13:25:41.000000 arch-5.5.0/.github/workflows/generate-documentation.yml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      286 2022-03-22 08:30:31.000000 arch-5.5.0/.gitignore
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       73 2021-07-22 17:04:35.000000 arch-5.5.0/.landscape.yml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      432 2021-07-22 17:04:35.000000 arch-5.5.0/.pep8speaks.yml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      674 2023-04-12 18:03:48.000000 arch-5.5.0/.readthedocs.yaml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1660 2022-08-15 08:35:45.000000 arch-5.5.0/LICENSE.md
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      276 2022-03-22 08:30:31.000000 arch-5.5.0/MANIFEST.in
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    12029 2023-04-25 13:26:04.205133 arch-5.5.0/PKG-INFO
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    11205 2023-04-25 13:25:41.000000 arch-5.5.0/README.md
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1103 2023-04-25 13:25:41.000000 arch-5.5.0/appveyor.yml
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.105133 arch-5.5.0/arch/
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.105133 arch-5.5.0/arch/__future__/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.5.0/arch/__future__/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      654 2021-07-22 17:04:35.000000 arch-5.5.0/arch/__future__/_utility.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.5.0/arch/__future__/reindexing.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      300 2022-03-22 08:30:31.000000 arch-5.5.0/arch/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      160 2023-04-25 13:26:04.000000 arch-5.5.0/arch/_version.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.155133 arch-5.5.0/arch/bootstrap/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      804 2021-07-22 17:04:35.000000 arch-5.5.0/arch/bootstrap/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   970405 2023-04-25 13:26:03.000000 arch-5.5.0/arch/bootstrap/_samplers.c
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      155 2021-07-22 17:04:35.000000 arch-5.5.0/arch/bootstrap/_samplers.pyi
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1169 2022-08-15 08:35:45.000000 arch-5.5.0/arch/bootstrap/_samplers.pyx
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1104 2021-07-22 17:04:35.000000 arch-5.5.0/arch/bootstrap/_samplers_python.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    65385 2023-04-25 13:25:41.000000 arch-5.5.0/arch/bootstrap/base.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    29911 2023-04-25 13:25:41.000000 arch-5.5.0/arch/bootstrap/multiple_comparison.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.105133 arch-5.5.0/arch/compat/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.5.0/arch/compat/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1196 2021-07-22 17:04:35.000000 arch-5.5.0/arch/compat/numba.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      311 2022-08-15 08:35:45.000000 arch-5.5.0/arch/compat/pandas.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      326 2021-07-22 17:04:35.000000 arch-5.5.0/arch/compat/statsmodels.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1258 2023-04-25 13:25:41.000000 arch-5.5.0/arch/conftest.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.105133 arch-5.5.0/arch/covariance/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.5.0/arch/covariance/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    18250 2023-04-12 18:03:48.000000 arch-5.5.0/arch/covariance/kernel.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.105133 arch-5.5.0/arch/data/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.5.0/arch/data/__init__.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.105133 arch-5.5.0/arch/data/binary/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      348 2021-07-22 17:04:35.000000 arch-5.5.0/arch/data/binary/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1609 2021-07-22 17:04:35.000000 arch-5.5.0/arch/data/binary/binary.csv.gz
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.105133 arch-5.5.0/arch/data/core_cpi/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      362 2023-04-12 18:03:48.000000 arch-5.5.0/arch/data/core_cpi/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2749 2021-07-22 17:04:35.000000 arch-5.5.0/arch/data/core_cpi/core-cpi.csv.gz
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.115133 arch-5.5.0/arch/data/crude/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      359 2023-04-12 18:03:48.000000 arch-5.5.0/arch/data/crude/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3078 2021-07-22 17:04:35.000000 arch-5.5.0/arch/data/crude/crude.csv.gz
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.115133 arch-5.5.0/arch/data/default/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      326 2023-04-12 18:03:48.000000 arch-5.5.0/arch/data/default/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6572 2021-07-22 17:04:35.000000 arch-5.5.0/arch/data/default/default.csv.gz
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.115133 arch-5.5.0/arch/data/frenchdata/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      492 2023-04-12 18:03:48.000000 arch-5.5.0/arch/data/frenchdata/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    10817 2021-07-22 17:04:35.000000 arch-5.5.0/arch/data/frenchdata/frenchdata.csv.gz
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.115133 arch-5.5.0/arch/data/nasdaq/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      336 2023-04-12 18:03:48.000000 arch-5.5.0/arch/data/nasdaq/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   114929 2021-07-22 17:04:35.000000 arch-5.5.0/arch/data/nasdaq/nasdaq.csv.gz
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.115133 arch-5.5.0/arch/data/sp500/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      326 2023-04-12 18:03:48.000000 arch-5.5.0/arch/data/sp500/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   102735 2021-07-22 17:04:35.000000 arch-5.5.0/arch/data/sp500/sp500.csv.gz
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      695 2021-07-22 17:04:35.000000 arch-5.5.0/arch/data/utility.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.115133 arch-5.5.0/arch/data/vix/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      296 2023-04-12 18:03:48.000000 arch-5.5.0/arch/data/vix/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6031 2021-07-22 17:04:35.000000 arch-5.5.0/arch/data/vix/vix.csv.gz
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.115133 arch-5.5.0/arch/data/wti/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      376 2023-04-12 18:03:48.000000 arch-5.5.0/arch/data/wti/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    39069 2021-07-22 17:04:35.000000 arch-5.5.0/arch/data/wti/wti.csv.gz
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.5.0/arch/py.typed
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.115133 arch-5.5.0/arch/tests/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/__init__.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.125133 arch-5.5.0/arch/tests/bootstrap/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/bootstrap/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      935 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/bootstrap/test_block_length.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    33640 2022-03-21 10:25:11.000000 arch-5.5.0/arch/tests/bootstrap/test_bootstrap.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    18325 2023-04-25 13:25:41.000000 arch-5.5.0/arch/tests/bootstrap/test_multiple_comparison.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.125133 arch-5.5.0/arch/tests/covariance/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/covariance/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     8704 2023-04-25 13:25:41.000000 arch-5.5.0/arch/tests/covariance/test_covariance.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      717 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/test_compat.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      501 2022-08-15 08:35:45.000000 arch-5.5.0/arch/tests/test_data.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2049 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/test_examples.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      629 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/test_tester.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.125133 arch-5.5.0/arch/tests/unitroot/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/unitroot/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2251 2023-04-12 18:03:48.000000 arch-5.5.0/arch/tests/unitroot/cointegration_data.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.125133 arch-5.5.0/arch/tests/unitroot/data/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/unitroot/data/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   223090 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/unitroot/data/zivot-andrews.csv
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     7262 2022-03-21 10:25:11.000000 arch-5.5.0/arch/tests/unitroot/test_dynamic_ols.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     8998 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/unitroot/test_engle_granger.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    13322 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/unitroot/test_fmols_ccr.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6111 2022-03-21 10:25:11.000000 arch-5.5.0/arch/tests/unitroot/test_phillips_ouliaris.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    25212 2022-08-15 08:35:45.000000 arch-5.5.0/arch/tests/unitroot/test_unitroot.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.125133 arch-5.5.0/arch/tests/univariate/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/univariate/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5680 2022-08-15 08:35:45.000000 arch-5.5.0/arch/tests/univariate/test_arch_in_mean.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      288 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/univariate/test_base.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     7354 2022-08-15 08:35:45.000000 arch-5.5.0/arch/tests/univariate/test_distribution.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    37254 2022-08-15 08:35:45.000000 arch-5.5.0/arch/tests/univariate/test_forecast.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    49837 2023-04-25 13:25:41.000000 arch-5.5.0/arch/tests/univariate/test_mean.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2412 2023-04-12 18:03:48.000000 arch-5.5.0/arch/tests/univariate/test_moment.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    46010 2022-08-15 08:35:45.000000 arch-5.5.0/arch/tests/univariate/test_recursions.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2022 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/univariate/test_rescale.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    81881 2022-08-15 08:35:45.000000 arch-5.5.0/arch/tests/univariate/test_variance_forecasting.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    60204 2022-08-15 08:35:45.000000 arch-5.5.0/arch/tests/univariate/test_volatility.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.135133 arch-5.5.0/arch/tests/utility/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       21 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/utility/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     9195 2022-08-15 08:35:45.000000 arch-5.5.0/arch/tests/utility/test_array.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2360 2023-04-12 18:03:48.000000 arch-5.5.0/arch/tests/utility/test_cov.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      572 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/utility/test_io.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3582 2022-08-15 08:35:45.000000 arch-5.5.0/arch/tests/utility/test_timeseries.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      188 2021-07-22 17:04:35.000000 arch-5.5.0/arch/tests/utility/test_utility.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2200 2022-08-15 08:35:45.000000 arch-5.5.0/arch/typing.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.135133 arch-5.5.0/arch/unitroot/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      413 2021-07-22 17:04:35.000000 arch-5.5.0/arch/unitroot/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     9585 2022-08-15 08:35:45.000000 arch-5.5.0/arch/unitroot/_engle_granger.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    16960 2022-08-15 08:35:45.000000 arch-5.5.0/arch/unitroot/_phillips_ouliaris.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     7668 2022-08-15 08:35:45.000000 arch-5.5.0/arch/unitroot/_shared.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    40919 2023-04-12 18:03:48.000000 arch-5.5.0/arch/unitroot/cointegration.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.135133 arch-5.5.0/arch/unitroot/critical_values/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.5.0/arch/unitroot/critical_values/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1320 2021-07-22 17:04:35.000000 arch-5.5.0/arch/unitroot/critical_values/dfgls.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    12737 2022-08-15 08:35:45.000000 arch-5.5.0/arch/unitroot/critical_values/dickey_fuller.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    22746 2021-07-22 17:04:35.000000 arch-5.5.0/arch/unitroot/critical_values/engle_granger.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3415 2021-07-22 17:04:35.000000 arch-5.5.0/arch/unitroot/critical_values/kpss.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    93787 2021-07-22 17:04:35.000000 arch-5.5.0/arch/unitroot/critical_values/phillips_ouliaris.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.165133 arch-5.5.0/arch/unitroot/critical_values/simulation/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2144 2022-08-15 08:35:45.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/adf_simulation.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3356 2023-04-12 18:03:48.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/adf_z_critical_values_simulation.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3863 2022-03-21 10:25:11.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/adf_z_critical_values_simulation_joblib.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4308 2022-08-15 08:35:45.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/adf_z_critical_values_simulation_large_cluster.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2336 2022-08-15 08:35:45.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/adf_z_simlation_process.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4333 2022-08-15 08:35:45.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/dfgls_critical_values_simulation.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4346 2022-03-21 10:25:11.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/dfgls_simulation_process.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       43 2021-07-22 17:04:35.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/eg_setup.bat
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       45 2021-07-22 17:04:35.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/eg_setup.ps1
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       96 2021-07-22 17:04:35.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/eg_setup.sh
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     7497 2023-04-12 18:03:48.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/engle_granger_simulation.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4728 2021-07-22 17:04:35.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/engle_granger_simulation_process.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3162 2022-03-21 10:25:11.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/kpss_critical_values_simulation.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1721 2023-04-12 18:03:48.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/kpss_simulation_process.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    10613 2023-04-12 18:03:48.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/phillips-ouliaris-simulation-process.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    13181 2022-08-15 08:35:45.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/phillips-ouliaris-simulation.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      731 2021-07-22 17:04:35.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/phillips_ouliaris.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       23 2021-07-22 17:04:35.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/requirements.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4447 2022-08-15 08:35:45.000000 arch-5.5.0/arch/unitroot/critical_values/simulation/shared.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3897 2021-07-22 17:04:35.000000 arch-5.5.0/arch/unitroot/critical_values/zivot_andrews.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    69648 2023-04-25 13:25:41.000000 arch-5.5.0/arch/unitroot/unitroot.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.165133 arch-5.5.0/arch/univariate/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1148 2021-07-22 17:04:35.000000 arch-5.5.0/arch/univariate/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    75620 2022-08-15 08:35:45.000000 arch-5.5.0/arch/univariate/base.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    40955 2022-08-15 08:35:45.000000 arch-5.5.0/arch/univariate/distribution.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    70285 2023-04-12 18:03:48.000000 arch-5.5.0/arch/univariate/mean.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)  1818160 2023-04-25 13:26:02.000000 arch-5.5.0/arch/univariate/recursions.c
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3792 2022-08-15 08:35:45.000000 arch-5.5.0/arch/univariate/recursions.pyi
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    35811 2023-04-25 13:25:41.000000 arch-5.5.0/arch/univariate/recursions.pyx
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    33857 2023-04-12 18:03:48.000000 arch-5.5.0/arch/univariate/recursions_python.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   121950 2023-04-25 13:25:41.000000 arch-5.5.0/arch/univariate/volatility.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.145133 arch-5.5.0/arch/utility/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1536 2021-07-22 17:04:35.000000 arch-5.5.0/arch/utility/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     9358 2023-04-12 18:03:48.000000 arch-5.5.0/arch/utility/array.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1779 2023-04-25 13:25:41.000000 arch-5.5.0/arch/utility/cov.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2093 2021-07-22 17:04:35.000000 arch-5.5.0/arch/utility/exceptions.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      668 2022-08-15 08:35:45.000000 arch-5.5.0/arch/utility/io.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2158 2022-08-15 08:35:45.000000 arch-5.5.0/arch/utility/testing.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5445 2022-08-15 08:35:45.000000 arch-5.5.0/arch/utility/timeseries.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.145133 arch-5.5.0/arch/vendor/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      215 2021-07-22 17:04:35.000000 arch-5.5.0/arch/vendor/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6011 2022-08-15 08:35:45.000000 arch-5.5.0/arch/vendor/property_cached.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.155133 arch-5.5.0/arch.egg-info/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    12029 2023-04-25 13:26:04.000000 arch-5.5.0/arch.egg-info/PKG-INFO
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    11964 2023-04-25 13:26:04.000000 arch-5.5.0/arch.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2023-04-25 13:26:04.000000 arch-5.5.0/arch.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2023-04-12 18:04:54.000000 arch-5.5.0/arch.egg-info/not-zip-safe
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       76 2023-04-25 13:26:04.000000 arch-5.5.0/arch.egg-info/requires.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        5 2023-04-25 13:26:04.000000 arch-5.5.0/arch.egg-info/top_level.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      671 2021-07-22 17:04:35.000000 arch-5.5.0/azure-pipelines.yml
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.165133 arch-5.5.0/ci/
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.165133 arch-5.5.0/ci/azure/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5440 2023-04-25 13:25:41.000000 arch-5.5.0/ci/azure/azure_template_posix.yml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1632 2023-04-12 18:03:48.000000 arch-5.5.0/ci/azure/azure_template_windows.yml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1135 2023-04-12 18:03:48.000000 arch-5.5.0/ci/azure/install-posix.sh
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       68 2021-07-22 17:04:35.000000 arch-5.5.0/ci/azure/update_path.sh
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.165133 arch-5.5.0/ci/github-actions/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1342 2021-07-22 17:04:35.000000 arch-5.5.0/ci/github-actions/push-docs-gh-pages.sh
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      258 2021-07-22 17:04:35.000000 arch-5.5.0/ci/install-statsmodels-main.sh
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      490 2022-03-21 10:25:11.000000 arch-5.5.0/ci/performance.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.165133 arch-5.5.0/doc/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      646 2021-07-22 17:04:35.000000 arch-5.5.0/doc/Makefile
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      757 2021-07-22 17:04:35.000000 arch-5.5.0/doc/make.bat
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      452 2023-04-25 13:25:41.000000 arch-5.5.0/doc/requirements.txt
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.165133 arch-5.5.0/doc/source/
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.165133 arch-5.5.0/doc/source/_static/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/_static/.gitignore
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.165133 arch-5.5.0/doc/source/_static/css/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      301 2023-04-25 13:25:41.000000 arch-5.5.0/doc/source/_static/css/small_fixes.css
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.175133 arch-5.5.0/doc/source/_static/images/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1207 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/_static/images/android-chrome-192x192.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2174 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/_static/images/android-chrome-512x512.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1101 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/_static/images/apple-touch-icon.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      266 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/_static/images/browserconfig.xml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3349 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/_static/images/color-logo-256.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      904 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/_static/images/favicon-16x16.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1105 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/_static/images/favicon-32x32.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1144 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/_static/images/mstile-150x150.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      991 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/_static/images/safari-pinned-tab.svg
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      474 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/_static/images/site.webmanifest
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.175133 arch-5.5.0/doc/source/_templates/
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.175133 arch-5.5.0/doc/source/_templates/autosummary/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      117 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/_templates/autosummary/attribute.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      843 2022-03-21 10:25:11.000000 arch-5.5.0/doc/source/_templates/autosummary/class.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      118 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/_templates/autosummary/member.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      117 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/_templates/autosummary/method.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      113 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/_templates/autosummary/minimal_module.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1193 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/_templates/layout.html
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2550 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/api.rst
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.175133 arch-5.5.0/doc/source/bootstrap/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1336 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/bootstrap/background.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      926 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/bootstrap/bootstrap.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    13853 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/bootstrap/bootstrap_histogram.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    10086 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/bootstrap/confidence-intervals.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      781 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/bootstrap/iid-bootstraps.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2429 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/bootstrap/low-level-interface.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2155 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/bootstrap/parameter-covariance-estimation.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6414 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/bootstrap/semiparametric-parametric-bootstrap.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      908 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/bootstrap/timeseries-bootstraps.rst
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.175133 arch-5.5.0/doc/source/changes/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      468 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/changes/1.0.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      341 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/changes/2.0.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      846 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/changes/3.0.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     9167 2022-03-21 10:25:11.000000 arch-5.5.0/doc/source/changes/4.0.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3696 2023-04-25 13:25:41.000000 arch-5.5.0/doc/source/changes/5.0.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      169 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/changes.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     9704 2023-04-25 13:25:41.000000 arch-5.5.0/doc/source/conf.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.175133 arch-5.5.0/doc/source/covariance/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      563 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/covariance/covariance.rst
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.185133 arch-5.5.0/doc/source/images/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     7192 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/images/bw-logo.svg
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     7102 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/images/color-logo-no-text.svg
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6435 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/images/color-logo-unprocessed.svg
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    15514 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/images/color-logo.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     8225 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/images/color-logo.svg
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    15086 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/images/favicon.ico
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4536 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/images/favicon.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2034 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/images/favicon.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1998 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/images/favicon.svg
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    46243 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/images/hero.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1376 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/images/hero.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   116976 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/images/hero.svg
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1998 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/images/logo.svg
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1651 2023-04-25 13:25:41.000000 arch-5.5.0/doc/source/index.rst
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.185133 arch-5.5.0/doc/source/multiple-comparison/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      622 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/multiple-comparison/background.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2215 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/multiple-comparison/multiple-comparison-reference.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      557 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/multiple-comparison/multiple-comparisons.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      444 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/names_wordlist.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2386 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/spelling_wordlist.txt
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.185133 arch-5.5.0/doc/source/unitroot/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      616 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/unitroot/cointegration.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1952 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/unitroot/introduction.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      371 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/unitroot/tests.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1830 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/unitroot/unitroot.rst
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.195133 arch-5.5.0/doc/source/univariate/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       64 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/univariate/background.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      532 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/univariate/distribution.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     9556 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/univariate/forecasting.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4987 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/univariate/introduction.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1087 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/univariate/mean.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      474 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/univariate/results.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1024 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/univariate/univariate.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      277 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/univariate/utility.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1440 2021-07-22 17:04:35.000000 arch-5.5.0/doc/source/univariate/volatility.rst
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-04-25 13:26:04.205133 arch-5.5.0/examples/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    49989 2022-03-21 10:25:11.000000 arch-5.5.0/examples/bootstrap_examples.ipynb
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   166071 2022-03-21 10:25:11.000000 arch-5.5.0/examples/multiple-comparison_examples.ipynb
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   493128 2021-07-22 17:04:35.000000 arch-5.5.0/examples/unitroot_cointegration_examples.ipynb
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   191311 2021-07-22 17:04:35.000000 arch-5.5.0/examples/unitroot_examples.ipynb
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   214078 2021-07-22 17:04:35.000000 arch-5.5.0/examples/univariate_forecasting_with_exogenous_variables.ipynb
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6087 2023-04-12 18:03:48.000000 arch-5.5.0/examples/univariate_using_fixed_variance.ipynb
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   517387 2021-07-22 17:04:35.000000 arch-5.5.0/examples/univariate_volatility_forecasting.ipynb
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   763575 2023-04-12 18:03:48.000000 arch-5.5.0/examples/univariate_volatility_modeling.ipynb
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   752792 2023-04-12 18:03:48.000000 arch-5.5.0/examples/univariate_volatility_scenarios.ipynb
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       75 2022-03-22 08:30:31.000000 arch-5.5.0/lgtm.yml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2022-08-15 08:35:45.000000 arch-5.5.0/py.typed
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      457 2023-04-12 18:03:48.000000 arch-5.5.0/pyproject.toml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      464 2023-04-25 13:25:41.000000 arch-5.5.0/requirements-dev.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       76 2021-07-22 17:04:35.000000 arch-5.5.0/requirements.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2812 2023-04-25 13:26:04.205133 arch-5.5.0/setup.cfg
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6506 2023-04-12 18:03:48.000000 arch-5.5.0/setup.py
```

### Comparing `arch-5.4.0/.coveragerc` & `arch-5.5.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/.github/workflows/codeql.yml` & `arch-5.5.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/.github/workflows/generate-documentation.yml` & `arch-5.5.0/.github/workflows/generate-documentation.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,24 @@
     runs-on: ubuntu-latest
     defaults:
       run:
         shell: bash
     strategy:
       fail-fast: false
       matrix:
-        python-version: [3.8]
+        python-version: ["3.10"]
     steps:
     - name: Checkout
       uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - name: Install pandoc
       uses: r-lib/actions/setup-pandoc@v2
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip wheel "setuptools>=61"
         python -m pip install -r requirements.txt
         python -m pip install -r requirements-dev.txt
```

### Comparing `arch-5.4.0/.readthedocs.yaml` & `arch-5.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/LICENSE.md` & `arch-5.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/PKG-INFO` & `arch-5.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arch
-Version: 5.4.0
+Version: 5.5.0
 Summary: ARCH for Python
 Home-page: https://github.com/bashtage/arch
 Author: Kevin Sheppard
 Author-email: kevin.sheppard@economics.ox.ac.uk
 License: NCSA
 Keywords: arch,ARCH,variance,econometrics,volatility,finance,GARCH,bootstrap,random walk,unit root,Dickey Fuller,time series,confidence intervals,multiple comparisons,Reality Check,SPA,StepM
 Classifier: Development Status :: 5 - Production/Stable
@@ -298,15 +298,15 @@
 ### Developing
 
 The development requirements are:
 
 - Cython (0.29+, if not using ARCH_NO_BINARY=1)
 - pytest (For tests)
 - sphinx (to build docs)
-- sphinx_material (to build docs)
+- sphinx-immaterial (to build docs)
 - jupyter, notebook and nbsphinx (to build docs)
 
 ### Installation Notes
 
 1. If Cython is not installed, the package will be installed
     as-if `ARCH_NO_BINARY=1` was set.
 2. Setup does not verify these requirements. Please ensure these are
```

### Comparing `arch-5.4.0/README.md` & `arch-5.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
 ### Developing
 
 The development requirements are:
 
 - Cython (0.29+, if not using ARCH_NO_BINARY=1)
 - pytest (For tests)
 - sphinx (to build docs)
-- sphinx_material (to build docs)
+- sphinx-immaterial (to build docs)
 - jupyter, notebook and nbsphinx (to build docs)
 
 ### Installation Notes
 
 1. If Cython is not installed, the package will be installed
     as-if `ARCH_NO_BINARY=1` was set.
 2. Setup does not verify these requirements. Please ensure these are
```

### Comparing `arch-5.4.0/appveyor.yml` & `arch-5.5.0/appveyor.yml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   - cmd: SET OMP_NUM_THREADS=1
   - cmd: SET OPENBLAS_NUM_THREADS=1
   - ps: Start-FileDownload "https://repo.continuum.io/miniconda/Miniconda$env:PY_MAJOR_VER-latest-Windows-$env:PYTHON_ARCH.exe" C:\Miniconda.exe; echo "Finished downloading miniconda"
   - cmd: C:\Miniconda.exe /S /D=C:\Py
   - cmd: SET PATH=C:\Py;C:\Py\Scripts;C:\Py\Library\bin;%PATH%
   - cmd: conda config --set always_yes yes
   - cmd: conda update conda --quiet
-  - cmd: conda install numpy cython "pytest<7.1" pandas scipy patsy statsmodels matplotlib nbconvert nbformat pip pyyaml "setuptools>=61,<64" pyqt pyparsing --quiet
-  - cmd: conda install -c numba numba llvmlite
   - cmd: python -m pip install --upgrade pip
+  - cmd: conda install numpy cython pandas scipy patsy statsmodels matplotlib nbconvert nbformat pip pyyaml pyqt pyparsing --quiet
+  - cmd: conda install -c numba numba llvmlite
   - cmd: pip install "pytest>=7,<7.1" pytest-xdist!=1.30 property_cached
   - cmd: pip install -e .
 
 test_script:
   - cmd: pytest -n 2 arch -m "(not slow)" --durations=25
```

### Comparing `arch-5.4.0/arch/__future__/_utility.py` & `arch-5.5.0/arch/__future__/_utility.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/bootstrap/__init__.py` & `arch-5.5.0/arch/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/bootstrap/_samplers.c` & `arch-5.5.0/arch/bootstrap/_samplers.c`

 * *Files 0% similar despite different names*

```diff
@@ -1104,195 +1104,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":775
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":775
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":776
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":776
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":777
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":777
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":778
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":778
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":782
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":782
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":783
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":783
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":784
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":784
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":785
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":785
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":789
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":789
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":790
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":790
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":799
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":799
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":800
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":800
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":801
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":801
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":803
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":803
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":804
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":804
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":805
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":805
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":807
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":807
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":808
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":808
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":810
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":810
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":811
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":811
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":812
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":812
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1323,42 +1323,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":814
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":814
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":815
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":815
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":816
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":816
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":818
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":818
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2965,15 +2965,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_indices, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_u, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
  *         # experimental exception made for __getbuffer__ and __releasebuffer__
  *         # -- the details of this may change.
  *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
  *             # This implementation of getbuffer is geared towards Cython
  *             # requirements, and does not yet fulfill the PEP.
  */
 
@@ -3017,344 +3017,344 @@
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":265
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":265
  * 
  *             cdef int i, ndim
  *             cdef int endian_detector = 1             # <<<<<<<<<<<<<<
  *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
  * 
  */
   __pyx_v_endian_detector = 1;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":266
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":266
  *             cdef int i, ndim
  *             cdef int endian_detector = 1
  *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
  * 
  *             ndim = PyArray_NDIM(self)
  */
   __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":268
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":268
  *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
  * 
  *             ndim = PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  */
   __pyx_v_ndim = PyArray_NDIM(__pyx_v_self);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
  *             ndim = PyArray_NDIM(self)
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")
  */
   __pyx_t_2 = (((__pyx_v_flags & PyBUF_C_CONTIGUOUS) == PyBUF_C_CONTIGUOUS) != 0);
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L4_bool_binop_done;
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":271
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":271
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):             # <<<<<<<<<<<<<<
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  */
   __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_C_CONTIGUOUS) != 0)) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
  *             ndim = PyArray_NDIM(self)
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")
  */
   if (unlikely(__pyx_t_1)) {
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  */
     __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 272, __pyx_L1_error)
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
  *             ndim = PyArray_NDIM(self)
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")
  */
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  */
   __pyx_t_2 = (((__pyx_v_flags & PyBUF_F_CONTIGUOUS) == PyBUF_F_CONTIGUOUS) != 0);
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L7_bool_binop_done;
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":275
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":275
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):             # <<<<<<<<<<<<<<
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  * 
  */
   __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_F_CONTIGUOUS) != 0)) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L7_bool_binop_done:;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  */
   if (unlikely(__pyx_t_1)) {
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
  * 
  *             info.buf = PyArray_DATA(self)
  */
     __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 276, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 276, __pyx_L1_error)
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  */
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":278
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":278
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  * 
  *             info.buf = PyArray_DATA(self)             # <<<<<<<<<<<<<<
  *             info.ndim = ndim
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  */
   __pyx_v_info->buf = PyArray_DATA(__pyx_v_self);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":279
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":279
  * 
  *             info.buf = PyArray_DATA(self)
  *             info.ndim = ndim             # <<<<<<<<<<<<<<
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  *                 # Allocate new buffer for strides and shape info.
  */
   __pyx_v_info->ndim = __pyx_v_ndim;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
  *             info.buf = PyArray_DATA(self)
  *             info.ndim = ndim
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 # Allocate new buffer for strides and shape info.
  *                 # This is allocated as one block, strides first.
  */
   __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":283
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":283
  *                 # Allocate new buffer for strides and shape info.
  *                 # This is allocated as one block, strides first.
  *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)             # <<<<<<<<<<<<<<
  *                 info.shape = info.strides + ndim
  *                 for i in range(ndim):
  */
     __pyx_v_info->strides = ((Py_ssize_t *)PyObject_Malloc((((sizeof(Py_ssize_t)) * 2) * ((size_t)__pyx_v_ndim))));
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":284
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":284
  *                 # This is allocated as one block, strides first.
  *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
  *                 info.shape = info.strides + ndim             # <<<<<<<<<<<<<<
  *                 for i in range(ndim):
  *                     info.strides[i] = PyArray_STRIDES(self)[i]
  */
     __pyx_v_info->shape = (__pyx_v_info->strides + __pyx_v_ndim);
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":285
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":285
  *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
  *                 info.shape = info.strides + ndim
  *                 for i in range(ndim):             # <<<<<<<<<<<<<<
  *                     info.strides[i] = PyArray_STRIDES(self)[i]
  *                     info.shape[i] = PyArray_DIMS(self)[i]
  */
     __pyx_t_4 = __pyx_v_ndim;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":286
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":286
  *                 info.shape = info.strides + ndim
  *                 for i in range(ndim):
  *                     info.strides[i] = PyArray_STRIDES(self)[i]             # <<<<<<<<<<<<<<
  *                     info.shape[i] = PyArray_DIMS(self)[i]
  *             else:
  */
       (__pyx_v_info->strides[__pyx_v_i]) = (PyArray_STRIDES(__pyx_v_self)[__pyx_v_i]);
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":287
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":287
  *                 for i in range(ndim):
  *                     info.strides[i] = PyArray_STRIDES(self)[i]
  *                     info.shape[i] = PyArray_DIMS(self)[i]             # <<<<<<<<<<<<<<
  *             else:
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
  */
       (__pyx_v_info->shape[__pyx_v_i]) = (PyArray_DIMS(__pyx_v_self)[__pyx_v_i]);
     }
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
  *             info.buf = PyArray_DATA(self)
  *             info.ndim = ndim
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 # Allocate new buffer for strides and shape info.
  *                 # This is allocated as one block, strides first.
  */
     goto __pyx_L9;
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":289
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":289
  *                     info.shape[i] = PyArray_DIMS(self)[i]
  *             else:
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
  *             info.suboffsets = NULL
  */
   /*else*/ {
     __pyx_v_info->strides = ((Py_ssize_t *)PyArray_STRIDES(__pyx_v_self));
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":290
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":290
  *             else:
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  *             info.suboffsets = NULL
  *             info.itemsize = PyArray_ITEMSIZE(self)
  */
     __pyx_v_info->shape = ((Py_ssize_t *)PyArray_DIMS(__pyx_v_self));
   }
   __pyx_L9:;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":291
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":291
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
  *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
  *             info.itemsize = PyArray_ITEMSIZE(self)
  *             info.readonly = not PyArray_ISWRITEABLE(self)
  */
   __pyx_v_info->suboffsets = NULL;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":292
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":292
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
  *             info.suboffsets = NULL
  *             info.itemsize = PyArray_ITEMSIZE(self)             # <<<<<<<<<<<<<<
  *             info.readonly = not PyArray_ISWRITEABLE(self)
  * 
  */
   __pyx_v_info->itemsize = PyArray_ITEMSIZE(__pyx_v_self);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":293
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":293
  *             info.suboffsets = NULL
  *             info.itemsize = PyArray_ITEMSIZE(self)
  *             info.readonly = not PyArray_ISWRITEABLE(self)             # <<<<<<<<<<<<<<
  * 
  *             cdef int t
  */
   __pyx_v_info->readonly = (!(PyArray_ISWRITEABLE(__pyx_v_self) != 0));
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":296
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":296
  * 
  *             cdef int t
  *             cdef char* f = NULL             # <<<<<<<<<<<<<<
  *             cdef dtype descr = <dtype>PyArray_DESCR(self)
  *             cdef int offset
  */
   __pyx_v_f = NULL;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":297
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":297
  *             cdef int t
  *             cdef char* f = NULL
  *             cdef dtype descr = <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  *             cdef int offset
  * 
  */
   __pyx_t_7 = PyArray_DESCR(__pyx_v_self);
   __pyx_t_3 = ((PyObject *)__pyx_t_7);
   __Pyx_INCREF(__pyx_t_3);
   __pyx_v_descr = ((PyArray_Descr *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":300
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":300
  *             cdef int offset
  * 
  *             info.obj = self             # <<<<<<<<<<<<<<
  * 
  *             if not PyDataType_HASFIELDS(descr):
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   __Pyx_GOTREF(__pyx_v_info->obj);
   __Pyx_DECREF(__pyx_v_info->obj);
   __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
  *             info.obj = self
  * 
  *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or
  */
   __pyx_t_1 = ((!(PyDataType_HASFIELDS(__pyx_v_descr) != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":303
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":303
  * 
  *             if not PyDataType_HASFIELDS(descr):
  *                 t = descr.type_num             # <<<<<<<<<<<<<<
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):
  */
     __pyx_t_4 = __pyx_v_descr->type_num;
     __pyx_v_t = __pyx_t_4;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
  *             if not PyDataType_HASFIELDS(descr):
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  */
     __pyx_t_2 = ((__pyx_v_descr->byteorder == '>') != 0);
@@ -3366,15 +3366,15 @@
     if (!__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L14_bool_binop_done;
     }
     __pyx_L15_next_or:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":305
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":305
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
  *                     raise ValueError(u"Non-native byte order not supported")
  *                 if   t == NPY_BYTE:        f = "b"
  */
     __pyx_t_2 = ((__pyx_v_descr->byteorder == '<') != 0);
@@ -3383,235 +3383,235 @@
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L14_bool_binop_done;
     }
     __pyx_t_2 = ((!(__pyx_v_little_endian != 0)) != 0);
     __pyx_t_1 = __pyx_t_2;
     __pyx_L14_bool_binop_done:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
  *             if not PyDataType_HASFIELDS(descr):
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  */
     if (unlikely(__pyx_t_1)) {
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"
  */
       __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 306, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(1, 306, __pyx_L1_error)
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
  *             if not PyDataType_HASFIELDS(descr):
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  */
     }
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":307
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":307
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  *                 if   t == NPY_BYTE:        f = "b"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_UBYTE:       f = "B"
  *                 elif t == NPY_SHORT:       f = "h"
  */
     switch (__pyx_v_t) {
       case NPY_BYTE:
       __pyx_v_f = ((char *)"b");
       break;
       case NPY_UBYTE:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":308
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":308
  *                     raise ValueError(u"Non-native byte order not supported")
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_SHORT:       f = "h"
  *                 elif t == NPY_USHORT:      f = "H"
  */
       __pyx_v_f = ((char *)"B");
       break;
       case NPY_SHORT:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":309
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":309
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"
  *                 elif t == NPY_SHORT:       f = "h"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_USHORT:      f = "H"
  *                 elif t == NPY_INT:         f = "i"
  */
       __pyx_v_f = ((char *)"h");
       break;
       case NPY_USHORT:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":310
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":310
  *                 elif t == NPY_UBYTE:       f = "B"
  *                 elif t == NPY_SHORT:       f = "h"
  *                 elif t == NPY_USHORT:      f = "H"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_INT:         f = "i"
  *                 elif t == NPY_UINT:        f = "I"
  */
       __pyx_v_f = ((char *)"H");
       break;
       case NPY_INT:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":311
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":311
  *                 elif t == NPY_SHORT:       f = "h"
  *                 elif t == NPY_USHORT:      f = "H"
  *                 elif t == NPY_INT:         f = "i"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_UINT:        f = "I"
  *                 elif t == NPY_LONG:        f = "l"
  */
       __pyx_v_f = ((char *)"i");
       break;
       case NPY_UINT:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":312
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":312
  *                 elif t == NPY_USHORT:      f = "H"
  *                 elif t == NPY_INT:         f = "i"
  *                 elif t == NPY_UINT:        f = "I"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_LONG:        f = "l"
  *                 elif t == NPY_ULONG:       f = "L"
  */
       __pyx_v_f = ((char *)"I");
       break;
       case NPY_LONG:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":313
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":313
  *                 elif t == NPY_INT:         f = "i"
  *                 elif t == NPY_UINT:        f = "I"
  *                 elif t == NPY_LONG:        f = "l"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_ULONG:       f = "L"
  *                 elif t == NPY_LONGLONG:    f = "q"
  */
       __pyx_v_f = ((char *)"l");
       break;
       case NPY_ULONG:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":314
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":314
  *                 elif t == NPY_UINT:        f = "I"
  *                 elif t == NPY_LONG:        f = "l"
  *                 elif t == NPY_ULONG:       f = "L"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_LONGLONG:    f = "q"
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  */
       __pyx_v_f = ((char *)"L");
       break;
       case NPY_LONGLONG:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":315
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":315
  *                 elif t == NPY_LONG:        f = "l"
  *                 elif t == NPY_ULONG:       f = "L"
  *                 elif t == NPY_LONGLONG:    f = "q"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  *                 elif t == NPY_FLOAT:       f = "f"
  */
       __pyx_v_f = ((char *)"q");
       break;
       case NPY_ULONGLONG:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":316
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":316
  *                 elif t == NPY_ULONG:       f = "L"
  *                 elif t == NPY_LONGLONG:    f = "q"
  *                 elif t == NPY_ULONGLONG:   f = "Q"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_FLOAT:       f = "f"
  *                 elif t == NPY_DOUBLE:      f = "d"
  */
       __pyx_v_f = ((char *)"Q");
       break;
       case NPY_FLOAT:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":317
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":317
  *                 elif t == NPY_LONGLONG:    f = "q"
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  *                 elif t == NPY_FLOAT:       f = "f"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_DOUBLE:      f = "d"
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  */
       __pyx_v_f = ((char *)"f");
       break;
       case NPY_DOUBLE:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":318
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":318
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  *                 elif t == NPY_FLOAT:       f = "f"
  *                 elif t == NPY_DOUBLE:      f = "d"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  */
       __pyx_v_f = ((char *)"d");
       break;
       case NPY_LONGDOUBLE:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":319
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":319
  *                 elif t == NPY_FLOAT:       f = "f"
  *                 elif t == NPY_DOUBLE:      f = "d"
  *                 elif t == NPY_LONGDOUBLE:  f = "g"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  */
       __pyx_v_f = ((char *)"g");
       break;
       case NPY_CFLOAT:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":320
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":320
  *                 elif t == NPY_DOUBLE:      f = "d"
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  *                 elif t == NPY_CFLOAT:      f = "Zf"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
  */
       __pyx_v_f = ((char *)"Zf");
       break;
       case NPY_CDOUBLE:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":321
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":321
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  *                 elif t == NPY_CDOUBLE:     f = "Zd"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
  *                 elif t == NPY_OBJECT:      f = "O"
  */
       __pyx_v_f = ((char *)"Zd");
       break;
       case NPY_CLONGDOUBLE:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":322
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":322
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_OBJECT:      f = "O"
  *                 else:
  */
       __pyx_v_f = ((char *)"Zg");
       break;
       case NPY_OBJECT:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":323
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":323
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
  *                 elif t == NPY_OBJECT:      f = "O"             # <<<<<<<<<<<<<<
  *                 else:
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  */
       __pyx_v_f = ((char *)"O");
       break;
       default:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":325
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":325
  *                 elif t == NPY_OBJECT:      f = "O"
  *                 else:
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
  *                 info.format = f
  *                 return
  */
       __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 325, __pyx_L1_error)
@@ -3624,91 +3624,91 @@
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(1, 325, __pyx_L1_error)
       break;
     }
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":326
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":326
  *                 else:
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  *                 info.format = f             # <<<<<<<<<<<<<<
  *                 return
  *             else:
  */
     __pyx_v_info->format = __pyx_v_f;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":327
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":327
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  *                 info.format = f
  *                 return             # <<<<<<<<<<<<<<
  *             else:
  *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
  *             info.obj = self
  * 
  *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or
  */
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":329
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":329
  *                 return
  *             else:
  *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)             # <<<<<<<<<<<<<<
  *                 info.format[0] = c'^' # Native data types, manual alignment
  *                 offset = 0
  */
   /*else*/ {
     __pyx_v_info->format = ((char *)PyObject_Malloc(0xFF));
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":330
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":330
  *             else:
  *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
  *                 info.format[0] = c'^' # Native data types, manual alignment             # <<<<<<<<<<<<<<
  *                 offset = 0
  *                 f = _util_dtypestring(descr, info.format + 1,
  */
     (__pyx_v_info->format[0]) = '^';
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":331
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":331
  *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
  *                 info.format[0] = c'^' # Native data types, manual alignment
  *                 offset = 0             # <<<<<<<<<<<<<<
  *                 f = _util_dtypestring(descr, info.format + 1,
  *                                       info.format + _buffer_format_string_len,
  */
     __pyx_v_offset = 0;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":332
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":332
  *                 info.format[0] = c'^' # Native data types, manual alignment
  *                 offset = 0
  *                 f = _util_dtypestring(descr, info.format + 1,             # <<<<<<<<<<<<<<
  *                                       info.format + _buffer_format_string_len,
  *                                       &offset)
  */
     __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_descr, (__pyx_v_info->format + 1), (__pyx_v_info->format + 0xFF), (&__pyx_v_offset)); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(1, 332, __pyx_L1_error)
     __pyx_v_f = __pyx_t_9;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":335
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":335
  *                                       info.format + _buffer_format_string_len,
  *                                       &offset)
  *                 f[0] = c'\0' # Terminate format string             # <<<<<<<<<<<<<<
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  */
     (__pyx_v_f[0]) = '\x00';
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
  *         # experimental exception made for __getbuffer__ and __releasebuffer__
  *         # -- the details of this may change.
  *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
  *             # This implementation of getbuffer is geared towards Cython
  *             # requirements, and does not yet fulfill the PEP.
  */
 
@@ -3732,15 +3732,15 @@
   }
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_descr);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
  *                 f[0] = c'\0' # Terminate format string
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)
  */
 
@@ -3756,83 +3756,83 @@
 }
 
 static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__releasebuffer__", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  */
   __pyx_t_1 = (PyArray_HASFIELDS(__pyx_v_self) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":339
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":339
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)             # <<<<<<<<<<<<<<
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  *                 PyObject_Free(info.strides)
  */
     PyObject_Free(__pyx_v_info->format);
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  */
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 PyObject_Free(info.strides)
  *                 # info.shape was stored after info.strides in the same block
  */
   __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":341
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":341
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  *                 PyObject_Free(info.strides)             # <<<<<<<<<<<<<<
  *                 # info.shape was stored after info.strides in the same block
  * 
  */
     PyObject_Free(__pyx_v_info->strides);
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 PyObject_Free(info.strides)
  *                 # info.shape was stored after info.strides in the same block
  */
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
  *                 f[0] = c'\0' # Terminate format string
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":820
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":820
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3841,29 +3841,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":821
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":821
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 821, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":820
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":820
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3874,15 +3874,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":823
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":823
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3891,29 +3891,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":824
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":824
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 824, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":823
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":823
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3924,15 +3924,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":826
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":826
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3941,29 +3941,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":827
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":827
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":826
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":826
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3974,15 +3974,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":829
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":829
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3991,29 +3991,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":830
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":830
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 830, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":829
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":829
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4024,15 +4024,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":832
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":832
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4041,29 +4041,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":833
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":833
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 833, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":832
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":832
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4074,89 +4074,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":835
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":835
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":837
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":837
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":839
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":839
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":835
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":835
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":841
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":841
  *         return ()
  * 
  * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
  *     # Recursive utility function used in __getbuffer__ to get format
  *     # string. The new location in the format string is returned.
  */
 
@@ -4180,33 +4180,33 @@
   long __pyx_t_8;
   char *__pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_util_dtypestring", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":846
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":846
  * 
  *     cdef dtype child
  *     cdef int endian_detector = 1             # <<<<<<<<<<<<<<
  *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
  *     cdef tuple fields
  */
   __pyx_v_endian_detector = 1;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":847
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":847
  *     cdef dtype child
  *     cdef int endian_detector = 1
  *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
  *     cdef tuple fields
  * 
  */
   __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":850
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":850
  *     cdef tuple fields
  * 
  *     for childname in descr.names:             # <<<<<<<<<<<<<<
  *         fields = descr.fields[childname]
  *         child, new_offset = fields
  */
   if (unlikely(__pyx_v_descr->names == Py_None)) {
@@ -4221,15 +4221,15 @@
     #else
     __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 850, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_childname, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":851
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":851
  * 
  *     for childname in descr.names:
  *         fields = descr.fields[childname]             # <<<<<<<<<<<<<<
  *         child, new_offset = fields
  * 
  */
     if (unlikely(__pyx_v_descr->fields == Py_None)) {
@@ -4238,15 +4238,15 @@
     }
     __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_descr->fields, __pyx_v_childname); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 851, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (!(likely(PyTuple_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(1, 851, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_fields, ((PyObject*)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":852
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":852
  *     for childname in descr.names:
  *         fields = descr.fields[childname]
  *         child, new_offset = fields             # <<<<<<<<<<<<<<
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:
  */
     if (likely(__pyx_v_fields != Py_None)) {
@@ -4273,15 +4273,15 @@
     }
     if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_dtype))))) __PYX_ERR(1, 852, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_child, ((PyArray_Descr *)__pyx_t_3));
     __pyx_t_3 = 0;
     __Pyx_XDECREF_SET(__pyx_v_new_offset, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":854
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":854
  *         child, new_offset = fields
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  */
     __pyx_t_4 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 854, __pyx_L1_error)
@@ -4290,37 +4290,37 @@
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 854, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_6 = ((((__pyx_v_end - __pyx_v_f) - ((int)__pyx_t_5)) < 15) != 0);
     if (unlikely(__pyx_t_6)) {
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
  * 
  *         if ((child.byteorder == c'>' and little_endian) or
  */
       __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 855, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(1, 855, __pyx_L1_error)
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":854
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":854
  *         child, new_offset = fields
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  */
     }
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")
  */
     __pyx_t_7 = ((__pyx_v_child->byteorder == '>') != 0);
@@ -4332,15 +4332,15 @@
     if (!__pyx_t_7) {
     } else {
       __pyx_t_6 = __pyx_t_7;
       goto __pyx_L7_bool_binop_done;
     }
     __pyx_L8_next_or:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":858
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":858
  * 
  *         if ((child.byteorder == c'>' and little_endian) or
  *             (child.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
  *             raise ValueError(u"Non-native byte order not supported")
  *             # One could encode it in the format string and have Cython
  */
     __pyx_t_7 = ((__pyx_v_child->byteorder == '<') != 0);
@@ -4349,46 +4349,46 @@
       __pyx_t_6 = __pyx_t_7;
       goto __pyx_L7_bool_binop_done;
     }
     __pyx_t_7 = ((!(__pyx_v_little_endian != 0)) != 0);
     __pyx_t_6 = __pyx_t_7;
     __pyx_L7_bool_binop_done:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")
  */
     if (unlikely(__pyx_t_6)) {
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":859
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":859
  *         if ((child.byteorder == c'>' and little_endian) or
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
  *             # One could encode it in the format string and have Cython
  *             # complain instead, BUT: < and > in format strings also imply
  */
       __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 859, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(1, 859, __pyx_L1_error)
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")
  */
     }
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":869
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":869
  * 
  *         # Output padding bytes
  *         while offset[0] < new_offset:             # <<<<<<<<<<<<<<
  *             f[0] = 120 # "x"; pad byte
  *             f += 1
  */
     while (1) {
@@ -4396,108 +4396,108 @@
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_new_offset, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 869, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 869, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (!__pyx_t_6) break;
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":870
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":870
  *         # Output padding bytes
  *         while offset[0] < new_offset:
  *             f[0] = 120 # "x"; pad byte             # <<<<<<<<<<<<<<
  *             f += 1
  *             offset[0] += 1
  */
       (__pyx_v_f[0]) = 0x78;
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":871
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":871
  *         while offset[0] < new_offset:
  *             f[0] = 120 # "x"; pad byte
  *             f += 1             # <<<<<<<<<<<<<<
  *             offset[0] += 1
  * 
  */
       __pyx_v_f = (__pyx_v_f + 1);
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":872
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":872
  *             f[0] = 120 # "x"; pad byte
  *             f += 1
  *             offset[0] += 1             # <<<<<<<<<<<<<<
  * 
  *         offset[0] += child.itemsize
  */
       __pyx_t_8 = 0;
       (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + 1);
     }
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":874
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":874
  *             offset[0] += 1
  * 
  *         offset[0] += child.itemsize             # <<<<<<<<<<<<<<
  * 
  *         if not PyDataType_HASFIELDS(child):
  */
     __pyx_t_8 = 0;
     (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + __pyx_v_child->elsize);
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":876
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":876
  *         offset[0] += child.itemsize
  * 
  *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
  *             t = child.type_num
  *             if end - f < 5:
  */
     __pyx_t_6 = ((!(PyDataType_HASFIELDS(__pyx_v_child) != 0)) != 0);
     if (__pyx_t_6) {
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":877
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":877
  * 
  *         if not PyDataType_HASFIELDS(child):
  *             t = child.type_num             # <<<<<<<<<<<<<<
  *             if end - f < 5:
  *                 raise RuntimeError(u"Format string allocated too short.")
  */
       __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_child->type_num); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 877, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_XDECREF_SET(__pyx_v_t, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
  *         if not PyDataType_HASFIELDS(child):
  *             t = child.type_num
  *             if end - f < 5:             # <<<<<<<<<<<<<<
  *                 raise RuntimeError(u"Format string allocated too short.")
  * 
  */
       __pyx_t_6 = (((__pyx_v_end - __pyx_v_f) < 5) != 0);
       if (unlikely(__pyx_t_6)) {
 
-        /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
+        /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
  *             t = child.type_num
  *             if end - f < 5:
  *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
  * 
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  */
         __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 879, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_Raise(__pyx_t_4, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __PYX_ERR(1, 879, __pyx_L1_error)
 
-        /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
+        /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
  *         if not PyDataType_HASFIELDS(child):
  *             t = child.type_num
  *             if end - f < 5:             # <<<<<<<<<<<<<<
  *                 raise RuntimeError(u"Format string allocated too short.")
  * 
  */
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":882
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":882
  * 
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  *             if   t == NPY_BYTE:        f[0] =  98 #"b"             # <<<<<<<<<<<<<<
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_BYTE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 882, __pyx_L1_error)
@@ -4507,15 +4507,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 882, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 98;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":883
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":883
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  *             if   t == NPY_BYTE:        f[0] =  98 #"b"
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"             # <<<<<<<<<<<<<<
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UBYTE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 883, __pyx_L1_error)
@@ -4525,15 +4525,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 883, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 66;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":884
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":884
  *             if   t == NPY_BYTE:        f[0] =  98 #"b"
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"             # <<<<<<<<<<<<<<
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_SHORT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 884, __pyx_L1_error)
@@ -4543,15 +4543,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 884, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x68;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":885
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":885
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"             # <<<<<<<<<<<<<<
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_USHORT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 885, __pyx_L1_error)
@@ -4561,15 +4561,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 885, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 72;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":886
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":886
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  *             elif t == NPY_INT:         f[0] = 105 #"i"             # <<<<<<<<<<<<<<
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_INT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 886, __pyx_L1_error)
@@ -4579,15 +4579,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 886, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x69;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":887
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":887
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  *             elif t == NPY_UINT:        f[0] =  73 #"I"             # <<<<<<<<<<<<<<
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UINT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 887, __pyx_L1_error)
@@ -4597,15 +4597,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 887, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 73;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":888
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":888
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  *             elif t == NPY_LONG:        f[0] = 108 #"l"             # <<<<<<<<<<<<<<
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 888, __pyx_L1_error)
@@ -4615,15 +4615,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 888, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x6C;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":889
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":889
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"             # <<<<<<<<<<<<<<
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 889, __pyx_L1_error)
@@ -4633,15 +4633,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 889, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 76;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":890
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":890
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"             # <<<<<<<<<<<<<<
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGLONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 890, __pyx_L1_error)
@@ -4651,15 +4651,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 890, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x71;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":891
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":891
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"             # <<<<<<<<<<<<<<
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONGLONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 891, __pyx_L1_error)
@@ -4669,15 +4669,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 891, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 81;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":892
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":892
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"             # <<<<<<<<<<<<<<
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_FLOAT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 892, __pyx_L1_error)
@@ -4687,15 +4687,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 892, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x66;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":893
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":893
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"             # <<<<<<<<<<<<<<
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_DOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 893, __pyx_L1_error)
@@ -4705,15 +4705,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 893, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x64;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":894
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":894
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"             # <<<<<<<<<<<<<<
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 894, __pyx_L1_error)
@@ -4723,15 +4723,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 894, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x67;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":895
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":895
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf             # <<<<<<<<<<<<<<
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CFLOAT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 895, __pyx_L1_error)
@@ -4743,15 +4743,15 @@
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 90;
         (__pyx_v_f[1]) = 0x66;
         __pyx_v_f = (__pyx_v_f + 1);
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":896
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":896
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd             # <<<<<<<<<<<<<<
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 896, __pyx_L1_error)
@@ -4763,15 +4763,15 @@
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 90;
         (__pyx_v_f[1]) = 0x64;
         __pyx_v_f = (__pyx_v_f + 1);
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":897
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":897
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg             # <<<<<<<<<<<<<<
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
  *             else:
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CLONGDOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 897, __pyx_L1_error)
@@ -4783,15 +4783,15 @@
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 90;
         (__pyx_v_f[1]) = 0x67;
         __pyx_v_f = (__pyx_v_f + 1);
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":898
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":898
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"             # <<<<<<<<<<<<<<
  *             else:
  *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_OBJECT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 898, __pyx_L1_error)
@@ -4801,15 +4801,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 898, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (likely(__pyx_t_6)) {
         (__pyx_v_f[0]) = 79;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":900
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":900
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
  *             else:
  *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
  *             f += 1
  *         else:
  */
       /*else*/ {
@@ -4820,67 +4820,67 @@
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_Raise(__pyx_t_4, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __PYX_ERR(1, 900, __pyx_L1_error)
       }
       __pyx_L15:;
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":901
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":901
  *             else:
  *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  *             f += 1             # <<<<<<<<<<<<<<
  *         else:
  *             # Cython ignores struct boundary information ("T{...}"),
  */
       __pyx_v_f = (__pyx_v_f + 1);
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":876
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":876
  *         offset[0] += child.itemsize
  * 
  *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
  *             t = child.type_num
  *             if end - f < 5:
  */
       goto __pyx_L13;
     }
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":905
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":905
  *             # Cython ignores struct boundary information ("T{...}"),
  *             # so don't output it
  *             f = _util_dtypestring(child, f, end, offset)             # <<<<<<<<<<<<<<
  *     return f
  * 
  */
     /*else*/ {
       __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_child, __pyx_v_f, __pyx_v_end, __pyx_v_offset); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(1, 905, __pyx_L1_error)
       __pyx_v_f = __pyx_t_9;
     }
     __pyx_L13:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":850
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":850
  *     cdef tuple fields
  * 
  *     for childname in descr.names:             # <<<<<<<<<<<<<<
  *         fields = descr.fields[childname]
  *         child, new_offset = fields
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":906
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":906
  *             # so don't output it
  *             f = _util_dtypestring(child, f, end, offset)
  *     return f             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_f;
   goto __pyx_L0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":841
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":841
  *         return ()
  * 
  * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
  *     # Recursive utility function used in __getbuffer__ to get format
  *     # string. The new location in the format string is returned.
  */
 
@@ -4897,138 +4897,138 @@
   __Pyx_XDECREF(__pyx_v_childname);
   __Pyx_XDECREF(__pyx_v_new_offset);
   __Pyx_XDECREF(__pyx_v_t);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1022
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1022
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1023
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1023
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1025
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1025
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1026
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1026
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1028
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1028
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1029
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1029
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1025
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1025
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_array()
  */
 
@@ -5044,15 +5044,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_array()
  *     except Exception:
  */
   {
@@ -5060,53 +5060,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1035
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1035
  * cdef inline int import_array() except -1:
  *     try:
  *         _import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1035, __pyx_L3_error)
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1036
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1036
  *     try:
  *         _import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1036, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
  *         _import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1037, __pyx_L5_except_error)
@@ -5114,30 +5114,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 1037, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_array()
  */
 
@@ -5152,15 +5152,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1039
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1039
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5176,15 +5176,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5192,53 +5192,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1041
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1041
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1041, __pyx_L3_error)
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1042
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1042
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1042, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1043, __pyx_L5_except_error)
@@ -5246,30 +5246,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 1043, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1039
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1039
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5284,15 +5284,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5308,15 +5308,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5324,81 +5324,81 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1047
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1047
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1047, __pyx_L3_error)
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1048
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1048
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1048, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1049
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1049
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1049, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 1049, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19368,81 +19368,81 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_C_contiguous); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
  * 
  *             info.buf = PyArray_DATA(self)
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_Fortran_contiguou); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_Non_native_byte_order_not_suppor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
  * 
  *         if ((child.byteorder == c'>' and little_endian) or
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 855, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
  *             t = child.type_num
  *             if end - f < 5:
  *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
  * 
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor_2); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 879, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
  *         _import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 1037, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 1043, __pyx_L1_error)
```

### Comparing `arch-5.4.0/arch/bootstrap/_samplers.pyx` & `arch-5.5.0/arch/bootstrap/_samplers.pyx`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/bootstrap/_samplers_python.py` & `arch-5.5.0/arch/bootstrap/_samplers_python.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/bootstrap/base.py` & `arch-5.5.0/arch/bootstrap/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1456,15 +1456,15 @@
     def _resample(self) -> tuple[tuple[ArrayLike, ...], dict[str, ArrayLike]]:
         """
         Resample all data using the values in _index
         """
         pos_indices, kw_indices = cast(
             Tuple[List[Int64Array], Dict[str, Int64Array]], self._index
         )
-        pos_data = []
+        pos_data: list[np.ndarray | pd.DataFrame | pd.Series] = []
         for i, values in enumerate(self._args):
             if isinstance(values, (pd.Series, pd.DataFrame)):
                 pos_data.append(values.iloc[pos_indices[i]])
             else:
                 assert isinstance(values, np.ndarray)
                 pos_data.append(values[pos_indices[i]])
         named_data: dict[str, pd.DataFrame | pd.Series | AnyArray] = {}
@@ -1489,15 +1489,15 @@
 
     Parameters
     ----------
     block_size : int
         Size of block to use
     args
         Positional arguments to bootstrap
-    seed : {{Generator, RandomState, int}}, optional
+    seed : {Generator, RandomState, int}, optional
         Seed to use to ensure reproducable results. If an int, passes the
         value to value to ``np.random.default_rng``. If None, a fresh
         Generator is constructed with system-provided entropy.
     random_state : RandomState, optional
         ``RandomState`` to use to ensure reproducable results. Cannot
         be used with ``seed``
```

### Comparing `arch-5.4.0/arch/bootstrap/multiple_comparison.py` & `arch-5.5.0/arch/bootstrap/multiple_comparison.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,15 +521,15 @@
     bootstrap : str, optional
         Bootstrap to use.  Options are
         'stationary' or 'sb': Stationary bootstrap (Default)
         'circular' or 'cbb': Circular block bootstrap
         'moving block' or 'mbb': Moving block bootstrap
     studentize : bool
         Flag indicating to studentize loss differentials. Default is True
-    nested=False
+    nested : bool
         Flag indicating to use a nested bootstrap to compute variances for
         studentization.  Default is False.  Note that this can be slow since
         the procedure requires k extra bootstraps.
     seed : {int, Generator, RandomState}, optional
         Seed value to use when creating the bootstrap used in the comparison.
         If an integer or None, the NumPy default_rng is used with the seed
         value.  If a Generator or a RandomState, the argument is used.
```

### Comparing `arch-5.4.0/arch/compat/numba.py` & `arch-5.5.0/arch/compat/numba.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/covariance/kernel.py` & `arch-5.5.0/arch/covariance/kernel.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/data/binary/binary.csv.gz` & `arch-5.5.0/arch/data/binary/binary.csv.gz`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/data/core_cpi/core-cpi.csv.gz` & `arch-5.5.0/arch/data/core_cpi/core-cpi.csv.gz`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/data/crude/crude.csv.gz` & `arch-5.5.0/arch/data/crude/crude.csv.gz`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/data/default/default.csv.gz` & `arch-5.5.0/arch/data/default/default.csv.gz`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/data/frenchdata/frenchdata.csv.gz` & `arch-5.5.0/arch/data/frenchdata/frenchdata.csv.gz`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/data/nasdaq/nasdaq.csv.gz` & `arch-5.5.0/arch/data/nasdaq/nasdaq.csv.gz`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/data/sp500/sp500.csv.gz` & `arch-5.5.0/arch/data/sp500/sp500.csv.gz`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/data/utility.py` & `arch-5.5.0/arch/data/utility.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/data/vix/vix.csv.gz` & `arch-5.5.0/arch/data/vix/vix.csv.gz`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/data/wti/wti.csv.gz` & `arch-5.5.0/arch/data/wti/wti.csv.gz`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/bootstrap/test_block_length.py` & `arch-5.5.0/arch/tests/bootstrap/test_block_length.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/bootstrap/test_bootstrap.py` & `arch-5.5.0/arch/tests/bootstrap/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/bootstrap/test_multiple_comparison.py` & `arch-5.5.0/arch/tests/bootstrap/test_multiple_comparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,15 @@
 
     def test_errors(self):
         stepm = StepM(self.benchmark, self.models, size=0.10)
         with pytest.raises(RuntimeError):
             stepm.superior_models
 
     def test_exact_ties(self):
-        adj_models: pd.DataFrame = self.models_df - 100.0
+        adj_models = self.models_df - 100.0
         adj_models.iloc[:, :2] -= adj_models.iloc[:, :2].mean()
         adj_models.iloc[:, :2] += self.benchmark_df.mean().iloc[0]
         stepm = StepM(self.benchmark_df, adj_models, size=0.10)
         stepm.compute()
         assert_equal(len(stepm.superior_models), self.models.shape[1] - 2)
```

### Comparing `arch-5.4.0/arch/tests/covariance/test_covariance.py` & `arch-5.5.0/arch/tests/covariance/test_covariance.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,21 +65,21 @@
     ndim, use_pandas = request.param
     burn = 100
     size: Tuple[int, ...] = (500 + burn,)
     if ndim == 2:
         size += (3,)
     e = rs.standard_normal(size)
     if ndim == 1:
-        phi = rs.uniform(0, 0.9, 1)
+        phi = rs.uniform(0, 0.9)
         for i in range(1, size[0]):
             e[i] += e[i - 1] * phi
     else:
-        phi = np.diag(rs.uniform(0, 0.9, size[1]))
+        phi_arr = np.diag(rs.uniform(0, 0.9, size[1]))
         for i in range(1, size[0]):
-            e[i] += e[i - 1] @ phi
+            e[i] += e[i - 1] @ phi_arr
     e = e[burn:]
     if use_pandas:
         if ndim == 1:
             return pd.Series(e, name="x")
         else:
             return pd.DataFrame(e, columns=[f"x{i}" for i in range(e.shape[1])])
     return e
```

### Comparing `arch-5.4.0/arch/tests/test_compat.py` & `arch-5.5.0/arch/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/test_examples.py` & `arch-5.5.0/arch/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/test_tester.py` & `arch-5.5.0/arch/tests/test_tester.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/unitroot/cointegration_data.py` & `arch-5.5.0/arch/tests/unitroot/cointegration_data.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/unitroot/data/zivot-andrews.csv` & `arch-5.5.0/arch/tests/unitroot/data/zivot-andrews.csv`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/unitroot/test_dynamic_ols.py` & `arch-5.5.0/arch/tests/unitroot/test_dynamic_ols.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/unitroot/test_engle_granger.py` & `arch-5.5.0/arch/tests/unitroot/test_engle_granger.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/unitroot/test_fmols_ccr.py` & `arch-5.5.0/arch/tests/unitroot/test_fmols_ccr.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/unitroot/test_phillips_ouliaris.py` & `arch-5.5.0/arch/tests/unitroot/test_phillips_ouliaris.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/unitroot/test_unitroot.py` & `arch-5.5.0/arch/tests/unitroot/test_unitroot.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/univariate/test_arch_in_mean.py` & `arch-5.5.0/arch/tests/univariate/test_arch_in_mean.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/univariate/test_distribution.py` & `arch-5.5.0/arch/tests/univariate/test_distribution.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/univariate/test_forecast.py` & `arch-5.5.0/arch/tests/univariate/test_forecast.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/univariate/test_mean.py` & `arch-5.5.0/arch/tests/univariate/test_mean.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,15 @@
         params = np.asarray(res.params)
         fcast = np.zeros(t + 6)
         for i in range(21, t):
             fcast[: i + 1] = self.y[: i + 1]
             fcast[i + 1 :] = 0.0
             for h in range(6):
                 fcast[i + h + 1] = params[0]
-                fcast[i + h + 1] += params[1] * fcast[i + h : i + h + 1]
+                fcast[i + h + 1] += params[1] * fcast[i + h]
                 fcast[i + h + 1] += params[2] * fcast[i + h - 4 : i + h + 1].mean()
                 fcast[i + h + 1] += params[3] * fcast[i + h - 21 : i + h + 1].mean()
             direct.iloc[i, :] = fcast[i + 1 : i + 7]
         assert isinstance(forecasts, ARCHModelForecast)
         # TODO
         # assert_frame_equal(direct, forecasts)
         forecasts = res.forecast(res.params, horizon=6, reindex=False)
@@ -332,15 +332,15 @@
         params = np.asarray(res.params)
         fcast = np.zeros(t + 6)
         for i in range(21, t):
             fcast[: i + 1] = self.y[: i + 1]
             fcast[i + 1 :] = 0.0
             for h in range(6):
                 fcast[i + h + 1] = params[0]
-                fcast[i + h + 1] += params[1] * fcast[i + h : i + h + 1]
+                fcast[i + h + 1] += params[1] * fcast[i + h]
                 fcast[i + h + 1] += params[2] * fcast[i + h - 4 : i + h + 1].mean()
                 fcast[i + h + 1] += params[3] * fcast[i + h - 21 : i + h + 1].mean()
             direct.iloc[i, :] = fcast[i + 1 : i + 7]
         assert isinstance(forecasts, ARCHModelForecast)
         # TODO
         # assert_frame_equal(direct, forecasts)
```

### Comparing `arch-5.4.0/arch/tests/univariate/test_moment.py` & `arch-5.5.0/arch/tests/univariate/test_moment.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/univariate/test_recursions.py` & `arch-5.5.0/arch/tests/univariate/test_recursions.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/univariate/test_rescale.py` & `arch-5.5.0/arch/tests/univariate/test_rescale.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/univariate/test_variance_forecasting.py` & `arch-5.5.0/arch/tests/univariate/test_variance_forecasting.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/univariate/test_volatility.py` & `arch-5.5.0/arch/tests/univariate/test_volatility.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/utility/test_array.py` & `arch-5.5.0/arch/tests/utility/test_array.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/utility/test_cov.py` & `arch-5.5.0/arch/tests/utility/test_cov.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/utility/test_io.py` & `arch-5.5.0/arch/tests/utility/test_io.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/tests/utility/test_timeseries.py` & `arch-5.5.0/arch/tests/utility/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/typing.py` & `arch-5.5.0/arch/typing.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/_engle_granger.py` & `arch-5.5.0/arch/unitroot/_engle_granger.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/_phillips_ouliaris.py` & `arch-5.5.0/arch/unitroot/_phillips_ouliaris.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/_shared.py` & `arch-5.5.0/arch/unitroot/_shared.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/cointegration.py` & `arch-5.5.0/arch/unitroot/cointegration.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/dfgls.py` & `arch-5.5.0/arch/unitroot/critical_values/dfgls.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/dickey_fuller.py` & `arch-5.5.0/arch/unitroot/critical_values/dickey_fuller.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/engle_granger.py` & `arch-5.5.0/arch/unitroot/critical_values/engle_granger.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/kpss.py` & `arch-5.5.0/arch/unitroot/critical_values/kpss.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/phillips_ouliaris.py` & `arch-5.5.0/arch/unitroot/critical_values/phillips_ouliaris.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/simulation/adf_simulation.py` & `arch-5.5.0/arch/unitroot/critical_values/simulation/adf_simulation.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/simulation/adf_z_critical_values_simulation.py` & `arch-5.5.0/arch/unitroot/critical_values/simulation/adf_z_critical_values_simulation.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/simulation/adf_z_critical_values_simulation_joblib.py` & `arch-5.5.0/arch/unitroot/critical_values/simulation/adf_z_critical_values_simulation_joblib.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/simulation/adf_z_critical_values_simulation_large_cluster.py` & `arch-5.5.0/arch/unitroot/critical_values/simulation/adf_z_critical_values_simulation_large_cluster.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/simulation/adf_z_simlation_process.py` & `arch-5.5.0/arch/unitroot/critical_values/simulation/adf_z_simlation_process.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/simulation/dfgls_critical_values_simulation.py` & `arch-5.5.0/arch/unitroot/critical_values/simulation/dfgls_critical_values_simulation.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/simulation/dfgls_simulation_process.py` & `arch-5.5.0/arch/unitroot/critical_values/simulation/dfgls_simulation_process.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/simulation/engle_granger_simulation.py` & `arch-5.5.0/arch/unitroot/critical_values/simulation/engle_granger_simulation.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/simulation/engle_granger_simulation_process.py` & `arch-5.5.0/arch/unitroot/critical_values/simulation/engle_granger_simulation_process.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/simulation/kpss_critical_values_simulation.py` & `arch-5.5.0/arch/unitroot/critical_values/simulation/kpss_critical_values_simulation.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/simulation/kpss_simulation_process.py` & `arch-5.5.0/arch/unitroot/critical_values/simulation/kpss_simulation_process.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/simulation/phillips-ouliaris-simulation-process.py` & `arch-5.5.0/arch/unitroot/critical_values/simulation/phillips-ouliaris-simulation-process.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/simulation/phillips-ouliaris-simulation.py` & `arch-5.5.0/arch/unitroot/critical_values/simulation/phillips-ouliaris-simulation.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/simulation/phillips_ouliaris.py` & `arch-5.5.0/arch/unitroot/critical_values/simulation/phillips_ouliaris.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/simulation/shared.py` & `arch-5.5.0/arch/unitroot/critical_values/simulation/shared.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/critical_values/zivot_andrews.py` & `arch-5.5.0/arch/unitroot/critical_values/zivot_andrews.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/unitroot/unitroot.py` & `arch-5.5.0/arch/unitroot/unitroot.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,19 +271,19 @@
         xpx_sub = xpx[:i, :i]
         try:
             b = solve(xpx_sub, xpy[:i])
         except LinAlgError:
             raise InfeasibleTestException(
                 singular_array_error.format(max_lags=maxlag, lag=m - i)
             )
-        sigma2[i - m] = (ypy - b.T @ xpx_sub @ b) / nobs
+        sigma2[i - m] = squeeze(ypy - b.T @ xpx_sub @ b) / nobs
         if lower_method == "t-stat":
             xpxi = inv(xpx_sub)
             stderr = sqrt(sigma2[i - m] * xpxi[-1, -1])
-            tstat[i - m] = b[-1] / stderr
+            tstat[i - m] = squeeze(b[-1]) / stderr
 
     return _select_best_ic(method, nobs, sigma2, tstat)
 
 
 def _autolag_ols(
     endog: ArrayLike1D,
     exog: ArrayLike2D,
@@ -342,19 +342,19 @@
 
     sigma2 = empty(maxlag + 1)
     tstat = empty(maxlag + 1)
     nobs = float(endog.shape[0])
     tstat[0] = inf
     for i in range(startlag, startlag + maxlag + 1):
         b = solve(r[:i, :i], qpy[:i])
-        sigma2[i - startlag] = (ypy - b.T @ xpx[:i, :i] @ b) / nobs
+        sigma2[i - startlag] = squeeze(ypy - b.T @ xpx[:i, :i] @ b) / nobs
         if lower_method == "t-stat" and i > startlag:
             xpxi = inv(xpx[:i, :i])
             stderr = sqrt(sigma2[i - startlag] * xpxi[-1, -1])
-            tstat[i - startlag] = b[-1] / stderr
+            tstat[i - startlag] = squeeze(b[-1]) / stderr
 
     return _select_best_ic(method, nobs, sigma2, tstat)
 
 
 def _df_select_lags(
     y: Float64Array,
     trend: Literal["n", "c", "ct", "ctt"],
```

### Comparing `arch-5.4.0/arch/univariate/__init__.py` & `arch-5.5.0/arch/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/univariate/base.py` & `arch-5.5.0/arch/univariate/base.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/univariate/distribution.py` & `arch-5.5.0/arch/univariate/distribution.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/univariate/mean.py` & `arch-5.5.0/arch/univariate/mean.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/univariate/recursions.c` & `arch-5.5.0/arch/univariate/recursions.c`

 * *Files 1% similar despite different names*

```diff
@@ -1106,195 +1106,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":775
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":775
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":776
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":776
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":777
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":777
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":778
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":778
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":782
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":782
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":783
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":783
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":784
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":784
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":785
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":785
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":789
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":789
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":790
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":790
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":799
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":799
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":800
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":800
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":801
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":801
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":803
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":803
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":804
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":804
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":805
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":805
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":807
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":807
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":808
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":808
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":810
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":810
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":811
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":811
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":812
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":812
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1334,42 +1334,42 @@
 struct __pyx_obj_4arch_10univariate_10recursions_EGARCHUpdater;
 struct __pyx_obj_4arch_10univariate_10recursions_ARCHInMeanRecursion;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":814
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":814
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":815
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":815
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":816
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":816
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":818
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":818
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1405,15 +1405,15 @@
 
 
 /* "arch/univariate/recursions.pyx":666
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])
  * 
  * cdef class HARCHUpdater(VolatilityUpdater):             # <<<<<<<<<<<<<<
  *     cdef:
- *         np.int32_t[::1] lags
+ *         const np.int32_t[::1] lags
  */
 struct __pyx_obj_4arch_10univariate_10recursions_HARCHUpdater {
   struct __pyx_obj_4arch_10univariate_10recursions_VolatilityUpdater __pyx_base;
   __Pyx_memviewslice lags;
   double backcast;
 };
 
@@ -1628,15 +1628,15 @@
 
 
 /* "arch/univariate/recursions.pyx":666
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])
  * 
  * cdef class HARCHUpdater(VolatilityUpdater):             # <<<<<<<<<<<<<<
  *     cdef:
- *         np.int32_t[::1] lags
+ *         const np.int32_t[::1] lags
  */
 
 struct __pyx_vtabstruct_4arch_10univariate_10recursions_HARCHUpdater {
   struct __pyx_vtabstruct_4arch_10univariate_10recursions_VolatilityUpdater __pyx_base;
 };
 static struct __pyx_vtabstruct_4arch_10univariate_10recursions_HARCHUpdater *__pyx_vtabptr_4arch_10univariate_10recursions_HARCHUpdater;
 
@@ -2479,29 +2479,37 @@
                 int ndim,
                 __Pyx_TypeInfo *dtype,
                 __Pyx_BufFmt_StackElem stack[],
                 __Pyx_memviewslice *memviewslice,
                 PyObject *original_obj);
 
 /* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(PyObject *, int writable_flag);
+
+/* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_double(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int32_t__const__(PyObject *, int writable_flag);
+
+/* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_double__const__(PyObject *, int writable_flag);
+
+/* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int32_t(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(PyObject *, int writable_flag);
 
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_double(const char *itemp);
 static CYTHON_INLINE int __pyx_memview_set_double(const char *itemp, PyObject *obj);
 
 /* MemviewDtypeToObject.proto */
-static CYTHON_INLINE PyObject *__pyx_memview_get_nn___pyx_t_5numpy_int32_t(const char *itemp);
-static CYTHON_INLINE int __pyx_memview_set_nn___pyx_t_5numpy_int32_t(const char *itemp, PyObject *obj);
+static CYTHON_INLINE PyObject *__pyx_memview_get_nn___pyx_t_5numpy_int32_t__const__(const char *itemp);
 
 /* RealImag.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     #define __Pyx_CREAL(z) ((z).real())
     #define __Pyx_CIMAG(z) ((z).imag())
   #else
@@ -2615,17 +2623,14 @@
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_npy_int32(npy_int32 value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
-/* CIntFromPy.proto */
-static CYTHON_INLINE npy_int32 __Pyx_PyInt_As_npy_int32(PyObject *);
-
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
 
 /* CheckBinaryVersion.proto */
@@ -2745,15 +2750,17 @@
 static void __pyx_memoryview_broadcast_leading(__Pyx_memviewslice *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *, int, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *, int, size_t, void *, int); /*proto*/
 static void __pyx_memoryview__slice_assign_scalar(char *, Py_ssize_t *, Py_ssize_t *, int, size_t, void *); /*proto*/
 static PyObject *__pyx_unpickle_Enum__set_state(struct __pyx_MemviewEnum_obj *, PyObject *); /*proto*/
+static __Pyx_TypeInfo __Pyx_TypeInfo_double__const__ = { "const double", NULL, sizeof(double const ), { 0 }, 0, 'R', 0, 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t__const__ = { "const int32_t", NULL, sizeof(__pyx_t_5numpy_int32_t const ), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int32_t const ) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int32_t const ), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t = { "int32_t", NULL, sizeof(__pyx_t_5numpy_int32_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int32_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int32_t), 0 };
 #define __Pyx_MODULE_NAME "arch.univariate.recursions"
 extern int __pyx_module_is_main_arch__univariate__recursions;
 int __pyx_module_is_main_arch__univariate__recursions = 0;
 
 /* Implementation of 'arch.univariate.recursions' */
 static PyObject *__pyx_builtin_range;
@@ -3609,15 +3616,15 @@
 }
 
 /* "arch/univariate/recursions.pyx":47
  * 
  * 
  * def harch_core(             # <<<<<<<<<<<<<<
  *     Py_ssize_t t,
- *     double[::1] parameters,
+ *     const double[::1] parameters,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_1harch_core(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_4arch_10univariate_10recursions_harch_core[] = "\n    Compute variance recursion step for HARCH model\n\n    Parameters\n    ----------\n    t: int\n        Location of variance to compute. Assumes variance has been computed\n        at times t-1, t-2, ...\n    parameters : 1-d array, float64\n        Model parameters\n    resids : 1-d array, float64\n        Residuals to use in the recursion\n    sigma2 : 1-d array, float64\n        Conditional variances with same shape as resids\n    lags : 1-d array, int\n        Lag lengths in the HARCH\n    backcast : float64\n        Value to use when initializing the recursion\n    var_bounds : 2-d array\n        nobs by 2-element array of upper and lower bounds for conditional\n        variances for each time period\n\n    Returns\n    -------\n    float\n        Conditional variance at time t\n    ";
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_1harch_core = {"harch_core", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_1harch_core, METH_VARARGS|METH_KEYWORDS, __pyx_doc_4arch_10univariate_10recursions_harch_core};
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_1harch_core(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -3711,20 +3718,20 @@
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
     }
     __pyx_v_t = __Pyx_PyIndex_AsSsize_t(values[0]); if (unlikely((__pyx_v_t == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 48, __pyx_L3_error)
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 49, __pyx_L3_error)
-    __pyx_v_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_resids.memview)) __PYX_ERR(0, 50, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[1], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 49, __pyx_L3_error)
+    __pyx_v_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[2], 0); if (unlikely(!__pyx_v_resids.memview)) __PYX_ERR(0, 50, __pyx_L3_error)
     __pyx_v_sigma2 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sigma2.memview)) __PYX_ERR(0, 51, __pyx_L3_error)
-    __pyx_v_lags = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int32_t(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_lags.memview)) __PYX_ERR(0, 52, __pyx_L3_error)
+    __pyx_v_lags = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int32_t__const__(values[4], 0); if (unlikely(!__pyx_v_lags.memview)) __PYX_ERR(0, 52, __pyx_L3_error)
     __pyx_v_backcast = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_backcast == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L3_error)
-    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[6], PyBUF_WRITABLE); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 54, __pyx_L3_error)
+    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double__const__(values[6], 0); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 54, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("harch_core", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 47, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("arch.univariate.recursions.harch_core", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
@@ -3764,15 +3771,15 @@
  * 
  *     sigma2[t] = parameters[0]             # <<<<<<<<<<<<<<
  *     for i in range(lags.shape[0]):
  *         param = parameters[i + 1] / lags[i]
  */
   __pyx_t_1 = 0;
   __pyx_t_2 = __pyx_v_t;
-  *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_2)) )) = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) )));
+  *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_2)) )) = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) )));
 
   /* "arch/univariate/recursions.pyx":88
  * 
  *     sigma2[t] = parameters[0]
  *     for i in range(lags.shape[0]):             # <<<<<<<<<<<<<<
  *         param = parameters[i + 1] / lags[i]
  *         for j in range(lags[i]):
@@ -3787,25 +3794,25 @@
  *     for i in range(lags.shape[0]):
  *         param = parameters[i + 1] / lags[i]             # <<<<<<<<<<<<<<
  *         for j in range(lags[i]):
  *             if (t - j - 1) >= 0:
  */
     __pyx_t_1 = (__pyx_v_i + 1);
     __pyx_t_2 = __pyx_v_i;
-    __pyx_v_param = ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) ))) / ((double)(*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int32_t *) __pyx_v_lags.data) + __pyx_t_2)) )))));
+    __pyx_v_param = (((double)(*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) )))) / ((double)(*((__pyx_t_5numpy_int32_t const  *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int32_t const  *) __pyx_v_lags.data) + __pyx_t_2)) )))));
 
     /* "arch/univariate/recursions.pyx":90
  *     for i in range(lags.shape[0]):
  *         param = parameters[i + 1] / lags[i]
  *         for j in range(lags[i]):             # <<<<<<<<<<<<<<
  *             if (t - j - 1) >= 0:
  *                 sigma2[t] += param * resids[t - j - 1] * resids[t - j - 1]
  */
     __pyx_t_2 = __pyx_v_i;
-    __pyx_t_6 = (*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int32_t *) __pyx_v_lags.data) + __pyx_t_2)) )));
+    __pyx_t_6 = (*((__pyx_t_5numpy_int32_t const  *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int32_t const  *) __pyx_v_lags.data) + __pyx_t_2)) )));
     __pyx_t_7 = __pyx_t_6;
     for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
       __pyx_v_j = __pyx_t_8;
 
       /* "arch/univariate/recursions.pyx":91
  *         param = parameters[i + 1] / lags[i]
  *         for j in range(lags[i]):
@@ -3822,15 +3829,15 @@
  *                 sigma2[t] += param * resids[t - j - 1] * resids[t - j - 1]             # <<<<<<<<<<<<<<
  *             else:
  *                 sigma2[t] += param * backcast
  */
         __pyx_t_2 = ((__pyx_v_t - __pyx_v_j) - 1);
         __pyx_t_1 = ((__pyx_v_t - __pyx_v_j) - 1);
         __pyx_t_10 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_10)) )) += ((__pyx_v_param * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_2)) )))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_1)) ))));
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_10)) )) += ((__pyx_v_param * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_2)) )))) * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_1)) ))));
 
         /* "arch/univariate/recursions.pyx":91
  *         param = parameters[i + 1] / lags[i]
  *         for j in range(lags[i]):
  *             if (t - j - 1) >= 0:             # <<<<<<<<<<<<<<
  *                 sigma2[t] += param * resids[t - j - 1] * resids[t - j - 1]
  *             else:
@@ -3859,15 +3866,15 @@
  *     bounds_check(&sigma2[t], &var_bounds[t, 0])             # <<<<<<<<<<<<<<
  *     return sigma2[t]
  * 
  */
   __pyx_t_1 = __pyx_v_t;
   __pyx_t_2 = __pyx_v_t;
   __pyx_t_10 = 0;
-  __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_1)) )))), (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_2 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_10)) )))));
+  __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_1)) )))), (&(*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_2 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_10)) )))));
 
   /* "arch/univariate/recursions.pyx":97
  * 
  *     bounds_check(&sigma2[t], &var_bounds[t, 0])
  *     return sigma2[t]             # <<<<<<<<<<<<<<
  * 
  * 
@@ -3881,15 +3888,15 @@
   goto __pyx_L0;
 
   /* "arch/univariate/recursions.pyx":47
  * 
  * 
  * def harch_core(             # <<<<<<<<<<<<<<
  *     Py_ssize_t t,
- *     double[::1] parameters,
+ *     const double[::1] parameters,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_AddTraceback("arch.univariate.recursions.harch_core", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
@@ -3903,16 +3910,16 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":100
  * 
  * 
- * def harch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                     double[::1] resids,
+ * def harch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                     const double[::1] resids,
  *                     double[::1] sigma2,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_3harch_recursion(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_4arch_10univariate_10recursions_2harch_recursion[] = "\n    Parameters\n    ----------\n    parameters : 1-d array, float64\n        Model parameters\n    resids : 1-d array, float64\n        Residuals to use in the recursion\n    sigma2 : 1-d array, float64\n        Conditional variances with same shape as resids\n    lags : 1-d array, int\n        Lag lengths in the HARCH\n    nobs : int\n        Length of resids\n    backcast : float64\n        Value to use when initializing the recursion\n    var_bounds : 2-d array\n        nobs by 2-element array of upper and lower bounds for conditional\n        variances for each time period\n    ";
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_3harch_recursion = {"harch_recursion", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_3harch_recursion, METH_VARARGS|METH_KEYWORDS, __pyx_doc_4arch_10univariate_10recursions_2harch_recursion};
@@ -4006,21 +4013,21 @@
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
     }
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 100, __pyx_L3_error)
-    __pyx_v_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_resids.memview)) __PYX_ERR(0, 101, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 100, __pyx_L3_error)
+    __pyx_v_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[1], 0); if (unlikely(!__pyx_v_resids.memview)) __PYX_ERR(0, 101, __pyx_L3_error)
     __pyx_v_sigma2 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sigma2.memview)) __PYX_ERR(0, 102, __pyx_L3_error)
     __pyx_v_lags = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int32_t(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_lags.memview)) __PYX_ERR(0, 103, __pyx_L3_error)
     __pyx_v_nobs = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_nobs == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 104, __pyx_L3_error)
     __pyx_v_backcast = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_backcast == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
-    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[6], PyBUF_WRITABLE); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 106, __pyx_L3_error)
+    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double__const__(values[6], 0); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 106, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("harch_recursion", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 100, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("arch.univariate.recursions.harch_recursion", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
@@ -4089,15 +4096,15 @@
  *     for t in range(nobs):
  *         sigma2[t] = parameters[0]             # <<<<<<<<<<<<<<
  *         for i in range(num_lags):
  *             param = parameters[i + 1] / lags[i]
  */
     __pyx_t_4 = 0;
     __pyx_t_5 = __pyx_v_t;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) )) = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_4)) )));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) )) = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_4)) )));
 
     /* "arch/univariate/recursions.pyx":133
  *     for t in range(nobs):
  *         sigma2[t] = parameters[0]
  *         for i in range(num_lags):             # <<<<<<<<<<<<<<
  *             param = parameters[i + 1] / lags[i]
  *             for j in range(lags[i]):
@@ -4112,15 +4119,15 @@
  *         for i in range(num_lags):
  *             param = parameters[i + 1] / lags[i]             # <<<<<<<<<<<<<<
  *             for j in range(lags[i]):
  *                 if (t - j - 1) >= 0:
  */
       __pyx_t_4 = (__pyx_v_i + 1);
       __pyx_t_5 = __pyx_v_i;
-      __pyx_v_param = ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_4)) ))) / ((double)(*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int32_t *) __pyx_v_lags.data) + __pyx_t_5)) )))));
+      __pyx_v_param = (((double)(*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_4)) )))) / ((double)(*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int32_t *) __pyx_v_lags.data) + __pyx_t_5)) )))));
 
       /* "arch/univariate/recursions.pyx":135
  *         for i in range(num_lags):
  *             param = parameters[i + 1] / lags[i]
  *             for j in range(lags[i]):             # <<<<<<<<<<<<<<
  *                 if (t - j - 1) >= 0:
  *                     sigma2[t] += param * resids[t - j - 1] * resids[t - j - 1]
@@ -4147,15 +4154,15 @@
  *                     sigma2[t] += param * resids[t - j - 1] * resids[t - j - 1]             # <<<<<<<<<<<<<<
  *                 else:
  *                     sigma2[t] += param * backcast
  */
           __pyx_t_5 = ((__pyx_v_t - __pyx_v_j) - 1);
           __pyx_t_4 = ((__pyx_v_t - __pyx_v_j) - 1);
           __pyx_t_13 = __pyx_v_t;
-          *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_13)) )) += ((__pyx_v_param * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_5)) )))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_4)) ))));
+          *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_13)) )) += ((__pyx_v_param * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_5)) )))) * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_4)) ))));
 
           /* "arch/univariate/recursions.pyx":136
  *             param = parameters[i + 1] / lags[i]
  *             for j in range(lags[i]):
  *                 if (t - j - 1) >= 0:             # <<<<<<<<<<<<<<
  *                     sigma2[t] += param * resids[t - j - 1] * resids[t - j - 1]
  *                 else:
@@ -4184,23 +4191,23 @@
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])             # <<<<<<<<<<<<<<
  * 
  *     return np.asarray(sigma2)
  */
     __pyx_t_4 = __pyx_v_t;
     __pyx_t_5 = __pyx_v_t;
     __pyx_t_13 = 0;
-    __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) )))), (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_5 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_13)) )))));
+    __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) )))), (&(*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_5 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_13)) )))));
   }
 
   /* "arch/univariate/recursions.pyx":142
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])
  * 
  *     return np.asarray(sigma2)             # <<<<<<<<<<<<<<
  * 
- * def arch_recursion(double[::1] parameters,
+ * def arch_recursion(const double[::1] parameters,
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_np); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_asarray); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
@@ -4225,16 +4232,16 @@
   __pyx_r = __pyx_t_14;
   __pyx_t_14 = 0;
   goto __pyx_L0;
 
   /* "arch/univariate/recursions.pyx":100
  * 
  * 
- * def harch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                     double[::1] resids,
+ * def harch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                     const double[::1] resids,
  *                     double[::1] sigma2,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_14);
   __Pyx_XDECREF(__pyx_t_15);
@@ -4252,16 +4259,16 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":144
  *     return np.asarray(sigma2)
  * 
- * def arch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                    double[::1] resids,
+ * def arch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                    const double[::1] resids,
  *                    double[::1] sigma2,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_5arch_recursion(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_4arch_10univariate_10recursions_4arch_recursion[] = "\n    Parameters\n    ----------\n    parameters : 1-d array, float64\n        Model parameters\n    resids : 1-d array, float64\n        Residuals to use in the recursion\n    sigma2 : 1-d array, float64\n        Conditional variances with same shape as resids\n    p : int\n        Number of lags in ARCH model\n    nobs : int\n        Length of resids\n    backcast : float64\n        Value to use when initializing the recursion\n    var_bounds : 2-d array\n        nobs by 2-element array of upper and lower bounds for conditional\n        variances for each time period\n    ";
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_5arch_recursion = {"arch_recursion", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_5arch_recursion, METH_VARARGS|METH_KEYWORDS, __pyx_doc_4arch_10univariate_10recursions_4arch_recursion};
@@ -4355,21 +4362,21 @@
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
     }
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 144, __pyx_L3_error)
-    __pyx_v_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_resids.memview)) __PYX_ERR(0, 145, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 144, __pyx_L3_error)
+    __pyx_v_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[1], 0); if (unlikely(!__pyx_v_resids.memview)) __PYX_ERR(0, 145, __pyx_L3_error)
     __pyx_v_sigma2 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sigma2.memview)) __PYX_ERR(0, 146, __pyx_L3_error)
     __pyx_v_p = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_p == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 147, __pyx_L3_error)
     __pyx_v_nobs = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_nobs == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 148, __pyx_L3_error)
     __pyx_v_backcast = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_backcast == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 149, __pyx_L3_error)
-    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[6], PyBUF_WRITABLE); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 150, __pyx_L3_error)
+    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double__const__(values[6], 0); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 150, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("arch_recursion", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 144, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("arch.univariate.recursions.arch_recursion", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
@@ -4424,15 +4431,15 @@
  *     for t in range(nobs):
  *         sigma2[t] = parameters[0]             # <<<<<<<<<<<<<<
  *         for i in range(p):
  *             if (t - i - 1) < 0:
  */
     __pyx_t_4 = 0;
     __pyx_t_5 = __pyx_v_t;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) )) = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_4)) )));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) )) = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_4)) )));
 
     /* "arch/univariate/recursions.pyx":177
  *     for t in range(nobs):
  *         sigma2[t] = parameters[0]
  *         for i in range(p):             # <<<<<<<<<<<<<<
  *             if (t - i - 1) < 0:
  *                 sigma2[t] += parameters[i + 1] * backcast
@@ -4457,15 +4464,15 @@
  *             if (t - i - 1) < 0:
  *                 sigma2[t] += parameters[i + 1] * backcast             # <<<<<<<<<<<<<<
  *             else:
  *                 sigma2[t] += parameters[i + 1] * resids[t - i - 1] * \
  */
         __pyx_t_4 = (__pyx_v_i + 1);
         __pyx_t_5 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * __pyx_v_backcast);
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * __pyx_v_backcast);
 
         /* "arch/univariate/recursions.pyx":178
  *         sigma2[t] = parameters[0]
  *         for i in range(p):
  *             if (t - i - 1) < 0:             # <<<<<<<<<<<<<<
  *                 sigma2[t] += parameters[i + 1] * backcast
  *             else:
@@ -4497,30 +4504,30 @@
  *                 sigma2[t] += parameters[i + 1] * backcast
  *             else:
  *                 sigma2[t] += parameters[i + 1] * resids[t - i - 1] * \             # <<<<<<<<<<<<<<
  *                              resids[t - i - 1]
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])
  */
         __pyx_t_11 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_11)) )) += (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_5)) )))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_10)) ))));
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_11)) )) += (((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_5)) )))) * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_10)) ))));
       }
       __pyx_L7:;
     }
 
     /* "arch/univariate/recursions.pyx":183
  *                 sigma2[t] += parameters[i + 1] * resids[t - i - 1] * \
  *                              resids[t - i - 1]
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])             # <<<<<<<<<<<<<<
  * 
  *     return np.asarray(sigma2)
  */
     __pyx_t_10 = __pyx_v_t;
     __pyx_t_5 = __pyx_v_t;
     __pyx_t_4 = 0;
-    __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_10)) )))), (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_5 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_4)) )))));
+    __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_10)) )))), (&(*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_5 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_4)) )))));
   }
 
   /* "arch/univariate/recursions.pyx":185
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])
  * 
  *     return np.asarray(sigma2)             # <<<<<<<<<<<<<<
  * 
@@ -4553,16 +4560,16 @@
   __pyx_r = __pyx_t_12;
   __pyx_t_12 = 0;
   goto __pyx_L0;
 
   /* "arch/univariate/recursions.pyx":144
  *     return np.asarray(sigma2)
  * 
- * def arch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                    double[::1] resids,
+ * def arch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                    const double[::1] resids,
  *                    double[::1] sigma2,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_13);
@@ -4581,15 +4588,15 @@
 }
 
 /* "arch/univariate/recursions.pyx":187
  *     return np.asarray(sigma2)
  * 
  * def garch_core(             # <<<<<<<<<<<<<<
  *     Py_ssize_t t,
- *     double[::1] parameters,
+ *     const double[::1] parameters,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_7garch_core(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_4arch_10univariate_10recursions_6garch_core[] = "\n    Compute variance recursion step for GARCH and related models\n\n    Parameters\n    ----------\n    t : int\n        The time period to update\n    parameters : ndarray\n        Model parameters\n    resids : ndarray\n        Residuals\n    sigma2 : ndarray\n        Conditional variances with same shape as resids\n    backcast : float\n        Value to use when initializing the recursion\n    var_bounds : 2-d array\n        nobs by 2-element array of upper and lower bounds for conditional\n        transformed variances for each time period\n    p : int\n        Number of symmetric innovations in model\n    o : int\n        Number of asymmetric innovations in model\n    q : int\n        Number of lags of the (transformed) variance in the model\n    power : float\n        The power used in the model\n    ";
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_7garch_core = {"garch_core", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_7garch_core, METH_VARARGS|METH_KEYWORDS, __pyx_doc_4arch_10univariate_10recursions_6garch_core};
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_7garch_core(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -4713,19 +4720,19 @@
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
       values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
       values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
       values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
     }
     __pyx_v_t = __Pyx_PyIndex_AsSsize_t(values[0]); if (unlikely((__pyx_v_t == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L3_error)
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 189, __pyx_L3_error)
-    __pyx_v_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_resids.memview)) __PYX_ERR(0, 190, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[1], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 189, __pyx_L3_error)
+    __pyx_v_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[2], 0); if (unlikely(!__pyx_v_resids.memview)) __PYX_ERR(0, 190, __pyx_L3_error)
     __pyx_v_sigma2 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sigma2.memview)) __PYX_ERR(0, 191, __pyx_L3_error)
     __pyx_v_backcast = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_backcast == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 192, __pyx_L3_error)
-    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 193, __pyx_L3_error)
+    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double__const__(values[5], 0); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 193, __pyx_L3_error)
     __pyx_v_p = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_p == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 194, __pyx_L3_error)
     __pyx_v_o = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_o == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 195, __pyx_L3_error)
     __pyx_v_q = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_q == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 196, __pyx_L3_error)
     __pyx_v_power = __pyx_PyFloat_AsDouble(values[9]); if (unlikely((__pyx_v_power == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
@@ -4775,15 +4782,15 @@
  *     loc = 0
  *     sigma2[t] = parameters[loc]             # <<<<<<<<<<<<<<
  *     loc += 1
  *     for j in range(p):
  */
   __pyx_t_1 = __pyx_v_loc;
   __pyx_t_2 = __pyx_v_t;
-  *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_2)) )) = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) )));
+  *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_2)) )) = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) )));
 
   /* "arch/univariate/recursions.pyx":231
  *     loc = 0
  *     sigma2[t] = parameters[loc]
  *     loc += 1             # <<<<<<<<<<<<<<
  *     for j in range(p):
  *         if (t - 1 - j) < 0:
@@ -4817,15 +4824,15 @@
  *         if (t - 1 - j) < 0:
  *             sigma2[t] += parameters[loc] * backcast             # <<<<<<<<<<<<<<
  *         else:
  *             sigma2[t] += parameters[loc] * (fabs(resids[t - 1 - j]) ** power)
  */
       __pyx_t_1 = __pyx_v_loc;
       __pyx_t_2 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_2)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) ))) * __pyx_v_backcast);
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_2)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) ))) * __pyx_v_backcast);
 
       /* "arch/univariate/recursions.pyx":233
  *     loc += 1
  *     for j in range(p):
  *         if (t - 1 - j) < 0:             # <<<<<<<<<<<<<<
  *             sigma2[t] += parameters[loc] * backcast
  *         else:
@@ -4840,15 +4847,15 @@
  *         loc += 1
  *     for j in range(o):
  */
     /*else*/ {
       __pyx_t_1 = __pyx_v_loc;
       __pyx_t_2 = ((__pyx_v_t - 1) - __pyx_v_j);
       __pyx_t_7 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_7)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) ))) * pow(fabs((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_2)) )))), __pyx_v_power));
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_7)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) ))) * pow(fabs((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_2)) )))), __pyx_v_power));
     }
     __pyx_L5:;
 
     /* "arch/univariate/recursions.pyx":237
  *         else:
  *             sigma2[t] += parameters[loc] * (fabs(resids[t - 1 - j]) ** power)
  *         loc += 1             # <<<<<<<<<<<<<<
@@ -4885,15 +4892,15 @@
  *         if (t - 1 - j) < 0:
  *             sigma2[t] += parameters[loc] * 0.5 * backcast             # <<<<<<<<<<<<<<
  *         else:
  *             sigma2[t] += (
  */
       __pyx_t_2 = __pyx_v_loc;
       __pyx_t_1 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_1)) )) += (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_2)) ))) * 0.5) * __pyx_v_backcast);
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_1)) )) += (((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_2)) ))) * 0.5) * __pyx_v_backcast);
 
       /* "arch/univariate/recursions.pyx":239
  *         loc += 1
  *     for j in range(o):
  *         if (t - 1 - j) < 0:             # <<<<<<<<<<<<<<
  *             sigma2[t] += parameters[loc] * 0.5 * backcast
  *         else:
@@ -4941,15 +4948,15 @@
  *             sigma2[t] += parameters[loc] * 0.5 * backcast
  *         else:
  *             sigma2[t] += (             # <<<<<<<<<<<<<<
  *                 parameters[loc]
  *                 * (fabs(resids[t - 1 - j]) ** power)
  */
       __pyx_t_8 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_8)) )) += (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_2)) ))) * pow(fabs((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_1)) )))), __pyx_v_power)) * ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_7)) ))) < 0.0));
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_8)) )) += (((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_2)) ))) * pow(fabs((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_1)) )))), __pyx_v_power)) * ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_7)) ))) < 0.0));
     }
     __pyx_L8:;
 
     /* "arch/univariate/recursions.pyx":247
  *                 * (resids[t - 1 - j] < 0)
  *             )
  *         loc += 1             # <<<<<<<<<<<<<<
@@ -4986,15 +4993,15 @@
  *         if (t - 1 - j) < 0:
  *             sigma2[t] += parameters[loc] * backcast             # <<<<<<<<<<<<<<
  *         else:
  *             sigma2[t] += parameters[loc] * sigma2[t - 1 - j]
  */
       __pyx_t_7 = __pyx_v_loc;
       __pyx_t_1 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_1)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_7)) ))) * __pyx_v_backcast);
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_1)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_7)) ))) * __pyx_v_backcast);
 
       /* "arch/univariate/recursions.pyx":249
  *         loc += 1
  *     for j in range(q):
  *         if (t - 1 - j) < 0:             # <<<<<<<<<<<<<<
  *             sigma2[t] += parameters[loc] * backcast
  *         else:
@@ -5009,15 +5016,15 @@
  *         loc += 1
  *     bounds_check(&sigma2[t], &var_bounds[t, 0])
  */
     /*else*/ {
       __pyx_t_7 = __pyx_v_loc;
       __pyx_t_1 = ((__pyx_v_t - 1) - __pyx_v_j);
       __pyx_t_2 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_2)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_7)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_1)) ))));
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_2)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_7)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_1)) ))));
     }
     __pyx_L11:;
 
     /* "arch/univariate/recursions.pyx":253
  *         else:
  *             sigma2[t] += parameters[loc] * sigma2[t - 1 - j]
  *         loc += 1             # <<<<<<<<<<<<<<
@@ -5033,15 +5040,15 @@
  *     bounds_check(&sigma2[t], &var_bounds[t, 0])             # <<<<<<<<<<<<<<
  * 
  *     return sigma2[t]
  */
   __pyx_t_1 = __pyx_v_t;
   __pyx_t_7 = __pyx_v_t;
   __pyx_t_2 = 0;
-  __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_1)) )))), (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_7 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_2)) )))));
+  __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_1)) )))), (&(*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_7 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_2)) )))));
 
   /* "arch/univariate/recursions.pyx":256
  *     bounds_check(&sigma2[t], &var_bounds[t, 0])
  * 
  *     return sigma2[t]             # <<<<<<<<<<<<<<
  * 
  * 
@@ -5055,15 +5062,15 @@
   goto __pyx_L0;
 
   /* "arch/univariate/recursions.pyx":187
  *     return np.asarray(sigma2)
  * 
  * def garch_core(             # <<<<<<<<<<<<<<
  *     Py_ssize_t t,
- *     double[::1] parameters,
+ *     const double[::1] parameters,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("arch.univariate.recursions.garch_core", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
@@ -5076,17 +5083,17 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":259
  * 
  * 
- * def garch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                     double[::1] fresids,
- *                     double[::1] sresids,
+ * def garch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                     const double[::1] fresids,
+ *                     const double[::1] sresids,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_9garch_recursion(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_4arch_10univariate_10recursions_8garch_recursion[] = "\n    Compute variance recursion for GARCH and related models\n\n    Parameters\n    ----------\n    parameters : 1-d array, float64\n        Model parameters\n    fresids : 1-d array, float64\n        Absolute value of residuals raised to the power in the model.  For\n        example, in a standard GARCH model, the power is 2.0.\n    sresids : 1-d array, float64\n        Variable containing the sign of the residuals (-1.0, 0.0, 1.0)\n    sigma2 : 1-d array, float64\n        Conditional variances with same shape as resids\n    p : int\n        Number of symmetric innovations in model\n    o : int\n        Number of asymmetric innovations in model\n    q : int\n        Number of lags of the (transformed) variance in the model\n    nobs : int\n        Length of resids\n    backcast : float64\n        Value to use when initializing the recursion\n    var_bounds : 2-d array\n        nobs by 2-element array of upper and lower bounds for conditional\n        transformed variances for each time period\n    ";
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_9garch_recursion = {"garch_recursion", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_9garch_recursion, METH_VARARGS|METH_KEYWORDS, __pyx_doc_4arch_10univariate_10recursions_8garch_recursion};
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_9garch_recursion(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -5209,24 +5216,24 @@
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
       values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
       values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
       values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
     }
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 259, __pyx_L3_error)
-    __pyx_v_fresids = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_fresids.memview)) __PYX_ERR(0, 260, __pyx_L3_error)
-    __pyx_v_sresids = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sresids.memview)) __PYX_ERR(0, 261, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 259, __pyx_L3_error)
+    __pyx_v_fresids = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[1], 0); if (unlikely(!__pyx_v_fresids.memview)) __PYX_ERR(0, 260, __pyx_L3_error)
+    __pyx_v_sresids = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[2], 0); if (unlikely(!__pyx_v_sresids.memview)) __PYX_ERR(0, 261, __pyx_L3_error)
     __pyx_v_sigma2 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sigma2.memview)) __PYX_ERR(0, 262, __pyx_L3_error)
     __pyx_v_p = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_p == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 263, __pyx_L3_error)
     __pyx_v_o = __Pyx_PyInt_As_int(values[5]); if (unlikely((__pyx_v_o == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 264, __pyx_L3_error)
     __pyx_v_q = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_q == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 265, __pyx_L3_error)
     __pyx_v_nobs = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_nobs == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 266, __pyx_L3_error)
     __pyx_v_backcast = __pyx_PyFloat_AsDouble(values[8]); if (unlikely((__pyx_v_backcast == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 267, __pyx_L3_error)
-    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[9], PyBUF_WRITABLE); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 268, __pyx_L3_error)
+    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double__const__(values[9], 0); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 268, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("garch_recursion", 1, 10, 10, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 259, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("arch.univariate.recursions.garch_recursion", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
@@ -5291,15 +5298,15 @@
  *         loc = 0
  *         sigma2[t] = parameters[loc]             # <<<<<<<<<<<<<<
  *         loc += 1
  *         for j in range(p):
  */
     __pyx_t_4 = __pyx_v_loc;
     __pyx_t_5 = __pyx_v_t;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) )) = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_4)) )));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) )) = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_4)) )));
 
     /* "arch/univariate/recursions.pyx":304
  *         loc = 0
  *         sigma2[t] = parameters[loc]
  *         loc += 1             # <<<<<<<<<<<<<<
  *         for j in range(p):
  *             if (t - 1 - j) < 0:
@@ -5333,15 +5340,15 @@
  *             if (t - 1 - j) < 0:
  *                 sigma2[t] += parameters[loc] * backcast             # <<<<<<<<<<<<<<
  *             else:
  *                 sigma2[t] += parameters[loc] * fresids[t - 1 - j]
  */
         __pyx_t_4 = __pyx_v_loc;
         __pyx_t_5 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * __pyx_v_backcast);
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * __pyx_v_backcast);
 
         /* "arch/univariate/recursions.pyx":306
  *         loc += 1
  *         for j in range(p):
  *             if (t - 1 - j) < 0:             # <<<<<<<<<<<<<<
  *                 sigma2[t] += parameters[loc] * backcast
  *             else:
@@ -5356,15 +5363,15 @@
  *             loc += 1
  *         for j in range(o):
  */
       /*else*/ {
         __pyx_t_4 = __pyx_v_loc;
         __pyx_t_5 = ((__pyx_v_t - 1) - __pyx_v_j);
         __pyx_t_10 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_10)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_fresids.data) + __pyx_t_5)) ))));
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_10)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_fresids.data) + __pyx_t_5)) ))));
       }
       __pyx_L7:;
 
       /* "arch/univariate/recursions.pyx":310
  *             else:
  *                 sigma2[t] += parameters[loc] * fresids[t - 1 - j]
  *             loc += 1             # <<<<<<<<<<<<<<
@@ -5401,15 +5408,15 @@
  *             if (t - 1 - j) < 0:
  *                 sigma2[t] += parameters[loc] * 0.5 * backcast             # <<<<<<<<<<<<<<
  *             else:
  *                 sigma2[t] += parameters[loc] * fresids[t - 1 - j] * (sresids[t-1-j] < 0)
  */
         __pyx_t_5 = __pyx_v_loc;
         __pyx_t_4 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) )) += (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_5)) ))) * 0.5) * __pyx_v_backcast);
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) )) += (((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_5)) ))) * 0.5) * __pyx_v_backcast);
 
         /* "arch/univariate/recursions.pyx":312
  *             loc += 1
  *         for j in range(o):
  *             if (t - 1 - j) < 0:             # <<<<<<<<<<<<<<
  *                 sigma2[t] += parameters[loc] * 0.5 * backcast
  *             else:
@@ -5425,15 +5432,15 @@
  *         for j in range(q):
  */
       /*else*/ {
         __pyx_t_5 = __pyx_v_loc;
         __pyx_t_4 = ((__pyx_v_t - 1) - __pyx_v_j);
         __pyx_t_10 = ((__pyx_v_t - 1) - __pyx_v_j);
         __pyx_t_11 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_11)) )) += (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_5)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_fresids.data) + __pyx_t_4)) )))) * ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sresids.data) + __pyx_t_10)) ))) < 0.0));
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_11)) )) += (((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_5)) ))) * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_fresids.data) + __pyx_t_4)) )))) * ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_sresids.data) + __pyx_t_10)) ))) < 0.0));
       }
       __pyx_L10:;
 
       /* "arch/univariate/recursions.pyx":316
  *             else:
  *                 sigma2[t] += parameters[loc] * fresids[t - 1 - j] * (sresids[t-1-j] < 0)
  *             loc += 1             # <<<<<<<<<<<<<<
@@ -5470,15 +5477,15 @@
  *             if (t - 1 - j) < 0:
  *                 sigma2[t] += parameters[loc] * backcast             # <<<<<<<<<<<<<<
  *             else:
  *                 sigma2[t] += parameters[loc] * sigma2[t - 1 - j]
  */
         __pyx_t_10 = __pyx_v_loc;
         __pyx_t_4 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_10)) ))) * __pyx_v_backcast);
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_10)) ))) * __pyx_v_backcast);
 
         /* "arch/univariate/recursions.pyx":318
  *             loc += 1
  *         for j in range(q):
  *             if (t - 1 - j) < 0:             # <<<<<<<<<<<<<<
  *                 sigma2[t] += parameters[loc] * backcast
  *             else:
@@ -5493,15 +5500,15 @@
  *             loc += 1
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])
  */
       /*else*/ {
         __pyx_t_10 = __pyx_v_loc;
         __pyx_t_4 = ((__pyx_v_t - 1) - __pyx_v_j);
         __pyx_t_5 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_10)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) ))));
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_10)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) ))));
       }
       __pyx_L13:;
 
       /* "arch/univariate/recursions.pyx":322
  *             else:
  *                 sigma2[t] += parameters[loc] * sigma2[t - 1 - j]
  *             loc += 1             # <<<<<<<<<<<<<<
@@ -5517,23 +5524,23 @@
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])             # <<<<<<<<<<<<<<
  * 
  *     return np.asarray(sigma2)
  */
     __pyx_t_4 = __pyx_v_t;
     __pyx_t_10 = __pyx_v_t;
     __pyx_t_5 = 0;
-    __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) )))), (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_10 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_5)) )))));
+    __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) )))), (&(*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_10 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_5)) )))));
   }
 
   /* "arch/univariate/recursions.pyx":325
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])
  * 
  *     return np.asarray(sigma2)             # <<<<<<<<<<<<<<
  * 
- * def egarch_recursion(double[::1] parameters,
+ * def egarch_recursion(const double[::1] parameters,
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_np); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 325, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_asarray); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 325, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
@@ -5558,17 +5565,17 @@
   __pyx_r = __pyx_t_12;
   __pyx_t_12 = 0;
   goto __pyx_L0;
 
   /* "arch/univariate/recursions.pyx":259
  * 
  * 
- * def garch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                     double[::1] fresids,
- *                     double[::1] sresids,
+ * def garch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                     const double[::1] fresids,
+ *                     const double[::1] sresids,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_13);
   __Pyx_XDECREF(__pyx_t_14);
@@ -5585,16 +5592,16 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":327
  *     return np.asarray(sigma2)
  * 
- * def egarch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                      double[::1] resids,
+ * def egarch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                      const double[::1] resids,
  *                      double[::1] sigma2,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_11egarch_recursion(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_4arch_10univariate_10recursions_10egarch_recursion[] = "\n    Compute variance recursion for EGARCH models\n\n    Parameters\n    ----------\n    parameters : 1-d array, float64\n        Model parameters\n    resids : 1-d array, float64\n        Residuals to use in the recursion\n    sigma2 : 1-d array, float64\n        Conditional variances with same shape as resids\n    p : int\n        Number of symmetric innovations in model\n    o : int\n        Number of asymmetric innovations in model\n    q : int\n        Number of lags of the (transformed) variance in the model\n    nobs : int\n        Length of resids\n    backcast : float64\n        Value to use when initializing the recursion\n    var_bounds : 2-d array\n        nobs by 2-element array of upper and lower bounds for conditional\n        variances for each time period\n    lnsigma2 : 1-d array, float64\n        Temporary array (overwritten) with same shape as resids\n    std_resids : 1-d array, float64\n        Temporary array (overwritten) with same shape as resids\n    abs_std_resids : 1-d array, float64\n        Temporary array (overwritten) with same shape as resids\n    ";
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_11egarch_recursion = {"egarch_recursion", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_11egarch_recursion, METH_VARARGS|METH_KEYWORDS, __pyx_doc_4arch_10univariate_10recursions_10egarch_recursion};
@@ -5738,23 +5745,23 @@
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
       values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
       values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
       values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
       values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
       values[11] = PyTuple_GET_ITEM(__pyx_args, 11);
     }
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 327, __pyx_L3_error)
-    __pyx_v_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_resids.memview)) __PYX_ERR(0, 328, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 327, __pyx_L3_error)
+    __pyx_v_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[1], 0); if (unlikely(!__pyx_v_resids.memview)) __PYX_ERR(0, 328, __pyx_L3_error)
     __pyx_v_sigma2 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sigma2.memview)) __PYX_ERR(0, 329, __pyx_L3_error)
     __pyx_v_p = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_p == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 330, __pyx_L3_error)
     __pyx_v_o = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_o == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 331, __pyx_L3_error)
     __pyx_v_q = __Pyx_PyInt_As_int(values[5]); if (unlikely((__pyx_v_q == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 332, __pyx_L3_error)
     __pyx_v_nobs = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_nobs == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 333, __pyx_L3_error)
     __pyx_v_backcast = __pyx_PyFloat_AsDouble(values[7]); if (unlikely((__pyx_v_backcast == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 334, __pyx_L3_error)
-    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[8], PyBUF_WRITABLE); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 335, __pyx_L3_error)
+    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double__const__(values[8], 0); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 335, __pyx_L3_error)
     __pyx_v_lnsigma2 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[9], PyBUF_WRITABLE); if (unlikely(!__pyx_v_lnsigma2.memview)) __PYX_ERR(0, 336, __pyx_L3_error)
     __pyx_v_std_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[10], PyBUF_WRITABLE); if (unlikely(!__pyx_v_std_resids.memview)) __PYX_ERR(0, 337, __pyx_L3_error)
     __pyx_v_abs_std_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[11], PyBUF_WRITABLE); if (unlikely(!__pyx_v_abs_std_resids.memview)) __PYX_ERR(0, 338, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("egarch_recursion", 1, 12, 12, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 327, __pyx_L3_error)
@@ -5824,15 +5831,15 @@
  *         loc = 0
  *         lnsigma2[t] = parameters[loc]             # <<<<<<<<<<<<<<
  *         loc += 1
  *         for j in range(p):
  */
     __pyx_t_4 = __pyx_v_loc;
     __pyx_t_5 = __pyx_v_t;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lnsigma2.data) + __pyx_t_5)) )) = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_4)) )));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lnsigma2.data) + __pyx_t_5)) )) = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_4)) )));
 
     /* "arch/univariate/recursions.pyx":377
  *         loc = 0
  *         lnsigma2[t] = parameters[loc]
  *         loc += 1             # <<<<<<<<<<<<<<
  *         for j in range(p):
  *             if (t - 1 - j) >= 0:
@@ -5867,15 +5874,15 @@
  *                 lnsigma2[t] += parameters[loc] * (abs_std_resids[t - 1 - j] - SQRT2_OV_PI)             # <<<<<<<<<<<<<<
  *             loc += 1
  *         for j in range(o):
  */
         __pyx_t_4 = __pyx_v_loc;
         __pyx_t_5 = ((__pyx_v_t - 1) - __pyx_v_j);
         __pyx_t_10 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lnsigma2.data) + __pyx_t_10)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_abs_std_resids.data) + __pyx_t_5)) ))) - 0.7978845608028654));
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lnsigma2.data) + __pyx_t_10)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_abs_std_resids.data) + __pyx_t_5)) ))) - 0.7978845608028654));
 
         /* "arch/univariate/recursions.pyx":379
  *         loc += 1
  *         for j in range(p):
  *             if (t - 1 - j) >= 0:             # <<<<<<<<<<<<<<
  *                 lnsigma2[t] += parameters[loc] * (abs_std_resids[t - 1 - j] - SQRT2_OV_PI)
  *             loc += 1
@@ -5920,15 +5927,15 @@
  *                 lnsigma2[t] += parameters[loc] * std_resids[t - 1 - j]             # <<<<<<<<<<<<<<
  *             loc += 1
  *         for j in range(q):
  */
         __pyx_t_5 = __pyx_v_loc;
         __pyx_t_4 = ((__pyx_v_t - 1) - __pyx_v_j);
         __pyx_t_10 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lnsigma2.data) + __pyx_t_10)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_5)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_std_resids.data) + __pyx_t_4)) ))));
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lnsigma2.data) + __pyx_t_10)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_5)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_std_resids.data) + __pyx_t_4)) ))));
 
         /* "arch/univariate/recursions.pyx":383
  *             loc += 1
  *         for j in range(o):
  *             if (t - 1 - j) >= 0:             # <<<<<<<<<<<<<<
  *                 lnsigma2[t] += parameters[loc] * std_resids[t - 1 - j]
  *             loc += 1
@@ -5972,15 +5979,15 @@
  *             if (t - 1 - j) < 0:
  *                 lnsigma2[t] += parameters[loc] * backcast             # <<<<<<<<<<<<<<
  *             else:
  *                 lnsigma2[t] += parameters[loc] * lnsigma2[t - 1 - j]
  */
         __pyx_t_4 = __pyx_v_loc;
         __pyx_t_5 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lnsigma2.data) + __pyx_t_5)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * __pyx_v_backcast);
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lnsigma2.data) + __pyx_t_5)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * __pyx_v_backcast);
 
         /* "arch/univariate/recursions.pyx":387
  *             loc += 1
  *         for j in range(q):
  *             if (t - 1 - j) < 0:             # <<<<<<<<<<<<<<
  *                 lnsigma2[t] += parameters[loc] * backcast
  *             else:
@@ -5995,15 +6002,15 @@
  *             loc += 1
  *         if lnsigma2[t] > LNSIGMA_MAX:
  */
       /*else*/ {
         __pyx_t_4 = __pyx_v_loc;
         __pyx_t_5 = ((__pyx_v_t - 1) - __pyx_v_j);
         __pyx_t_10 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lnsigma2.data) + __pyx_t_10)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lnsigma2.data) + __pyx_t_5)) ))));
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lnsigma2.data) + __pyx_t_10)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lnsigma2.data) + __pyx_t_5)) ))));
       }
       __pyx_L13:;
 
       /* "arch/univariate/recursions.pyx":391
  *             else:
  *                 lnsigma2[t] += parameters[loc] * lnsigma2[t - 1 - j]
  *             loc += 1             # <<<<<<<<<<<<<<
@@ -6060,28 +6067,28 @@
  *         if sigma2[t] < var_bounds[t, 0]:             # <<<<<<<<<<<<<<
  *             sigma2[t] = var_bounds[t, 0]
  *             lnsigma2[t] = log(sigma2[t])
  */
     __pyx_t_5 = __pyx_v_t;
     __pyx_t_4 = __pyx_v_t;
     __pyx_t_10 = 0;
-    __pyx_t_9 = (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) ))) < (*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_4 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_10)) )))) != 0);
+    __pyx_t_9 = (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) ))) < (*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_4 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_10)) )))) != 0);
     if (__pyx_t_9) {
 
       /* "arch/univariate/recursions.pyx":396
  *         sigma2[t] = exp(lnsigma2[t])
  *         if sigma2[t] < var_bounds[t, 0]:
  *             sigma2[t] = var_bounds[t, 0]             # <<<<<<<<<<<<<<
  *             lnsigma2[t] = log(sigma2[t])
  *         elif sigma2[t] > var_bounds[t, 1]:
  */
       __pyx_t_10 = __pyx_v_t;
       __pyx_t_4 = 0;
       __pyx_t_5 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) )) = (*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_10 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_4)) )));
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) )) = (*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_10 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_4)) )));
 
       /* "arch/univariate/recursions.pyx":397
  *         if sigma2[t] < var_bounds[t, 0]:
  *             sigma2[t] = var_bounds[t, 0]
  *             lnsigma2[t] = log(sigma2[t])             # <<<<<<<<<<<<<<
  *         elif sigma2[t] > var_bounds[t, 1]:
  *             sigma2[t] = var_bounds[t, 1] + log(sigma2[t]) - log(var_bounds[t, 1])
@@ -6106,15 +6113,15 @@
  *         elif sigma2[t] > var_bounds[t, 1]:             # <<<<<<<<<<<<<<
  *             sigma2[t] = var_bounds[t, 1] + log(sigma2[t]) - log(var_bounds[t, 1])
  *             lnsigma2[t] = log(sigma2[t])
  */
     __pyx_t_4 = __pyx_v_t;
     __pyx_t_10 = __pyx_v_t;
     __pyx_t_5 = 1;
-    __pyx_t_9 = (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) ))) > (*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_10 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_5)) )))) != 0);
+    __pyx_t_9 = (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) ))) > (*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_10 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_5)) )))) != 0);
     if (__pyx_t_9) {
 
       /* "arch/univariate/recursions.pyx":399
  *             lnsigma2[t] = log(sigma2[t])
  *         elif sigma2[t] > var_bounds[t, 1]:
  *             sigma2[t] = var_bounds[t, 1] + log(sigma2[t]) - log(var_bounds[t, 1])             # <<<<<<<<<<<<<<
  *             lnsigma2[t] = log(sigma2[t])
@@ -6122,15 +6129,15 @@
  */
       __pyx_t_5 = __pyx_v_t;
       __pyx_t_10 = 1;
       __pyx_t_4 = __pyx_v_t;
       __pyx_t_11 = __pyx_v_t;
       __pyx_t_12 = 1;
       __pyx_t_13 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_13)) )) = (((*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_5 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_10)) ))) + log((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) ))))) - log((*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_11 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_12)) )))));
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_13)) )) = (((*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_5 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_10)) ))) + log((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) ))))) - log((*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_11 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_12)) )))));
 
       /* "arch/univariate/recursions.pyx":400
  *         elif sigma2[t] > var_bounds[t, 1]:
  *             sigma2[t] = var_bounds[t, 1] + log(sigma2[t]) - log(var_bounds[t, 1])
  *             lnsigma2[t] = log(sigma2[t])             # <<<<<<<<<<<<<<
  *         std_resids[t] = resids[t] / sqrt(sigma2[t])
  *         abs_std_resids[t] = fabs(std_resids[t])
@@ -6155,15 +6162,15 @@
  *         std_resids[t] = resids[t] / sqrt(sigma2[t])             # <<<<<<<<<<<<<<
  *         abs_std_resids[t] = fabs(std_resids[t])
  * 
  */
     __pyx_t_12 = __pyx_v_t;
     __pyx_t_11 = __pyx_v_t;
     __pyx_t_4 = __pyx_v_t;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_std_resids.data) + __pyx_t_4)) )) = ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_12)) ))) / sqrt((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_11)) )))));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_std_resids.data) + __pyx_t_4)) )) = (((double)(*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_12)) )))) / sqrt((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_11)) )))));
 
     /* "arch/univariate/recursions.pyx":402
  *             lnsigma2[t] = log(sigma2[t])
  *         std_resids[t] = resids[t] / sqrt(sigma2[t])
  *         abs_std_resids[t] = fabs(std_resids[t])             # <<<<<<<<<<<<<<
  * 
  *     return np.asarray(sigma2)
@@ -6207,16 +6214,16 @@
   __pyx_r = __pyx_t_14;
   __pyx_t_14 = 0;
   goto __pyx_L0;
 
   /* "arch/univariate/recursions.pyx":327
  *     return np.asarray(sigma2)
  * 
- * def egarch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                      double[::1] resids,
+ * def egarch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                      const double[::1] resids,
  *                      double[::1] sigma2,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_14);
   __Pyx_XDECREF(__pyx_t_15);
@@ -6236,17 +6243,17 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":408
  * 
  * 
- * def midas_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                     double[::1] weights,
- *                     double[::1] resids,
+ * def midas_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                     const double[::1] weights,
+ *                     const double[::1] resids,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_13midas_recursion(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_4arch_10univariate_10recursions_12midas_recursion[] = "\n    Parameters\n    ----------\n    parameters : 1-d array, float64\n        Model parameters\n    weights : 1-d array, float64\n        Weights for MIDAS recursions\n    resids : 1-d array, float64\n        Residuals to use in the recursion\n    sigma2 : 1-d array, float64\n        Conditional variances with same shape as resids\n    nobs : int\n        Length of resids\n    backcast : float64\n        Value to use when initializing the recursion\n    var_bounds : 2-d array\n        nobs by 2-element array of upper and lower bounds for conditional\n        variances for each time period\n    ";
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_13midas_recursion = {"midas_recursion", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_13midas_recursion, METH_VARARGS|METH_KEYWORDS, __pyx_doc_4arch_10univariate_10recursions_12midas_recursion};
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_13midas_recursion(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -6339,17 +6346,17 @@
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
     }
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 408, __pyx_L3_error)
-    __pyx_v_weights = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_weights.memview)) __PYX_ERR(0, 409, __pyx_L3_error)
-    __pyx_v_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_resids.memview)) __PYX_ERR(0, 410, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 408, __pyx_L3_error)
+    __pyx_v_weights = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[1], 0); if (unlikely(!__pyx_v_weights.memview)) __PYX_ERR(0, 409, __pyx_L3_error)
+    __pyx_v_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[2], 0); if (unlikely(!__pyx_v_resids.memview)) __PYX_ERR(0, 410, __pyx_L3_error)
     __pyx_v_sigma2 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sigma2.memview)) __PYX_ERR(0, 411, __pyx_L3_error)
     __pyx_v_nobs = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_nobs == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 412, __pyx_L3_error)
     __pyx_v_backcast = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_backcast == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 413, __pyx_L3_error)
     __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[6], PyBUF_WRITABLE); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 414, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
@@ -6414,35 +6421,35 @@
  * 
  *     m = weights.shape[0]
  *     omega = parameters[0]             # <<<<<<<<<<<<<<
  *     alpha = parameters[1]
  *     gamma = parameters[2]
  */
   __pyx_t_1 = 0;
-  __pyx_v_omega = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) )));
+  __pyx_v_omega = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) )));
 
   /* "arch/univariate/recursions.pyx":441
  *     m = weights.shape[0]
  *     omega = parameters[0]
  *     alpha = parameters[1]             # <<<<<<<<<<<<<<
  *     gamma = parameters[2]
  * 
  */
   __pyx_t_1 = 1;
-  __pyx_v_alpha = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) )));
+  __pyx_v_alpha = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) )));
 
   /* "arch/univariate/recursions.pyx":442
  *     omega = parameters[0]
  *     alpha = parameters[1]
  *     gamma = parameters[2]             # <<<<<<<<<<<<<<
  * 
  *     aw = np.zeros(m, dtype=np.float64)
  */
   __pyx_t_1 = 2;
-  __pyx_v_gamma = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) )));
+  __pyx_v_gamma = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) )));
 
   /* "arch/univariate/recursions.pyx":444
  *     gamma = parameters[2]
  * 
  *     aw = np.zeros(m, dtype=np.float64)             # <<<<<<<<<<<<<<
  *     gw = np.zeros(m, dtype=np.float64)
  *     for i in range(m):
@@ -6535,26 +6542,26 @@
  *     for i in range(m):
  *         aw[i] = alpha * weights[i]             # <<<<<<<<<<<<<<
  *         gw[i] = gamma * weights[i]
  * 
  */
     __pyx_t_1 = __pyx_v_i;
     __pyx_t_11 = __pyx_v_i;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_aw.data) + __pyx_t_11)) )) = (__pyx_v_alpha * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_weights.data) + __pyx_t_1)) ))));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_aw.data) + __pyx_t_11)) )) = (__pyx_v_alpha * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_weights.data) + __pyx_t_1)) ))));
 
     /* "arch/univariate/recursions.pyx":448
  *     for i in range(m):
  *         aw[i] = alpha * weights[i]
  *         gw[i] = gamma * weights[i]             # <<<<<<<<<<<<<<
  * 
  *     resids2 = np.zeros(nobs, dtype=np.float64)
  */
     __pyx_t_1 = __pyx_v_i;
     __pyx_t_11 = __pyx_v_i;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_gw.data) + __pyx_t_11)) )) = (__pyx_v_gamma * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_weights.data) + __pyx_t_1)) ))));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_gw.data) + __pyx_t_11)) )) = (__pyx_v_gamma * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_weights.data) + __pyx_t_1)) ))));
   }
 
   /* "arch/univariate/recursions.pyx":450
  *         gw[i] = gamma * weights[i]
  * 
  *     resids2 = np.zeros(nobs, dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
@@ -6610,15 +6617,15 @@
  *         resids2[t] = resids[t] * resids[t]             # <<<<<<<<<<<<<<
  *         sigma2[t] = omega
  *         for i in range(m):
  */
     __pyx_t_1 = __pyx_v_t;
     __pyx_t_11 = __pyx_v_t;
     __pyx_t_14 = __pyx_v_t;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids2.data) + __pyx_t_14)) )) = ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_1)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_11)) ))));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids2.data) + __pyx_t_14)) )) = ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_1)) ))) * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_11)) ))));
 
     /* "arch/univariate/recursions.pyx":454
  *     for t in range(nobs):
  *         resids2[t] = resids[t] * resids[t]
  *         sigma2[t] = omega             # <<<<<<<<<<<<<<
  *         for i in range(m):
  *             if (t - i - 1) >= 0:
@@ -6656,15 +6663,15 @@
  *                 sigma2[t] +=  (aw[i] + 0.5 * gw[i]) * backcast
  */
         __pyx_t_11 = __pyx_v_i;
         __pyx_t_1 = __pyx_v_i;
         __pyx_t_14 = ((__pyx_v_t - __pyx_v_i) - 1);
         __pyx_t_17 = ((__pyx_v_t - __pyx_v_i) - 1);
         __pyx_t_18 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_18)) )) += (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_aw.data) + __pyx_t_11)) ))) + ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_gw.data) + __pyx_t_1)) ))) * ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_14)) ))) < 0.0))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids2.data) + __pyx_t_17)) ))));
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_18)) )) += (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_aw.data) + __pyx_t_11)) ))) + ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_gw.data) + __pyx_t_1)) ))) * ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_14)) ))) < 0.0))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids2.data) + __pyx_t_17)) ))));
 
         /* "arch/univariate/recursions.pyx":456
  *         sigma2[t] = omega
  *         for i in range(m):
  *             if (t - i - 1) >= 0:             # <<<<<<<<<<<<<<
  *                 sigma2[t] += (aw[i] + gw[i] * (resids[t - i - 1] < 0)) * resids2[t - i - 1]
  *             else:
@@ -6702,15 +6709,15 @@
   }
 
   /* "arch/univariate/recursions.pyx":463
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])
  * 
  *     return np.asarray(sigma2)             # <<<<<<<<<<<<<<
  * 
- * cdef double[::1] _figarch_weights(double[::1] parameters,
+ * cdef double[::1] _figarch_weights(const double[::1] parameters,
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
@@ -6735,17 +6742,17 @@
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* "arch/univariate/recursions.pyx":408
  * 
  * 
- * def midas_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                     double[::1] weights,
- *                     double[::1] resids,
+ * def midas_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                     const double[::1] weights,
+ *                     const double[::1] resids,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
@@ -6767,15 +6774,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":465
  *     return np.asarray(sigma2)
  * 
- * cdef double[::1] _figarch_weights(double[::1] parameters,             # <<<<<<<<<<<<<<
+ * cdef double[::1] _figarch_weights(const double[::1] parameters,             # <<<<<<<<<<<<<<
  *                                   int p,
  *                                   int q,
  */
 
 static __Pyx_memviewslice __pyx_f_4arch_10univariate_10recursions__figarch_weights(__Pyx_memviewslice __pyx_v_parameters, int __pyx_v_p, int __pyx_v_q, int __pyx_v_trunc_lag) {
   double __pyx_v_phi;
   double __pyx_v_d;
@@ -6808,46 +6815,46 @@
  * 
  *     phi = parameters[0] if p else 0.0             # <<<<<<<<<<<<<<
  *     d = parameters[1] if p else parameters[0]
  *     beta = parameters[p + q] if q else 0.0
  */
   if ((__pyx_v_p != 0)) {
     __pyx_t_2 = 0;
-    __pyx_t_1 = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_2)) )));
+    __pyx_t_1 = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_2)) )));
   } else {
     __pyx_t_1 = 0.0;
   }
   __pyx_v_phi = __pyx_t_1;
 
   /* "arch/univariate/recursions.pyx":475
  * 
  *     phi = parameters[0] if p else 0.0
  *     d = parameters[1] if p else parameters[0]             # <<<<<<<<<<<<<<
  *     beta = parameters[p + q] if q else 0.0
  * 
  */
   if ((__pyx_v_p != 0)) {
     __pyx_t_2 = 1;
-    __pyx_t_1 = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_2)) )));
+    __pyx_t_1 = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_2)) )));
   } else {
     __pyx_t_2 = 0;
-    __pyx_t_1 = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_2)) )));
+    __pyx_t_1 = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_2)) )));
   }
   __pyx_v_d = __pyx_t_1;
 
   /* "arch/univariate/recursions.pyx":476
  *     phi = parameters[0] if p else 0.0
  *     d = parameters[1] if p else parameters[0]
  *     beta = parameters[p + q] if q else 0.0             # <<<<<<<<<<<<<<
  * 
  *     # Recursive weight computation
  */
   if ((__pyx_v_q != 0)) {
     __pyx_t_2 = (__pyx_v_p + __pyx_v_q);
-    __pyx_t_1 = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_2)) )));
+    __pyx_t_1 = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_2)) )));
   } else {
     __pyx_t_1 = 0.0;
   }
   __pyx_v_beta = __pyx_t_1;
 
   /* "arch/univariate/recursions.pyx":479
  * 
@@ -6988,15 +6995,15 @@
   __PYX_INC_MEMVIEW(&__pyx_v_lam, 0);
   __pyx_r = __pyx_v_lam;
   goto __pyx_L0;
 
   /* "arch/univariate/recursions.pyx":465
  *     return np.asarray(sigma2)
  * 
- * cdef double[::1] _figarch_weights(double[::1] parameters,             # <<<<<<<<<<<<<<
+ * cdef double[::1] _figarch_weights(const double[::1] parameters,             # <<<<<<<<<<<<<<
  *                                   int p,
  *                                   int q,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
@@ -7018,15 +7025,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":490
  * 
  * 
- * def figarch_weights(double[::1] parameters, int p, int q, int trunc_lag):             # <<<<<<<<<<<<<<
+ * def figarch_weights(const double[::1] parameters, int p, int q, int trunc_lag):             # <<<<<<<<<<<<<<
  *     return np.asarray(_figarch_weights(parameters, p, q, trunc_lag))
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_15figarch_weights(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_15figarch_weights = {"figarch_weights", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_15figarch_weights, METH_VARARGS|METH_KEYWORDS, 0};
@@ -7090,15 +7097,15 @@
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 490, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 490, __pyx_L3_error)
     __pyx_v_p = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_p == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 490, __pyx_L3_error)
     __pyx_v_q = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_q == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 490, __pyx_L3_error)
     __pyx_v_trunc_lag = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_trunc_lag == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 490, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("figarch_weights", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 490, __pyx_L3_error)
@@ -7125,15 +7132,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("figarch_weights", 0);
 
   /* "arch/univariate/recursions.pyx":491
  * 
- * def figarch_weights(double[::1] parameters, int p, int q, int trunc_lag):
+ * def figarch_weights(const double[::1] parameters, int p, int q, int trunc_lag):
  *     return np.asarray(_figarch_weights(parameters, p, q, trunc_lag))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -7165,15 +7172,15 @@
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "arch/univariate/recursions.pyx":490
  * 
  * 
- * def figarch_weights(double[::1] parameters, int p, int q, int trunc_lag):             # <<<<<<<<<<<<<<
+ * def figarch_weights(const double[::1] parameters, int p, int q, int trunc_lag):             # <<<<<<<<<<<<<<
  *     return np.asarray(_figarch_weights(parameters, p, q, trunc_lag))
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -7189,16 +7196,16 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":494
  * 
  * 
- * def figarch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                       double[::1] fresids,
+ * def figarch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                       const double[::1] fresids,
  *                       double[::1] sigma2,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_17figarch_recursion(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_17figarch_recursion = {"figarch_recursion", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_17figarch_recursion, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_17figarch_recursion(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -7311,16 +7318,16 @@
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
       values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
       values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
     }
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 494, __pyx_L3_error)
-    __pyx_v_fresids = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_fresids.memview)) __PYX_ERR(0, 495, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 494, __pyx_L3_error)
+    __pyx_v_fresids = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[1], 0); if (unlikely(!__pyx_v_fresids.memview)) __PYX_ERR(0, 495, __pyx_L3_error)
     __pyx_v_sigma2 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sigma2.memview)) __PYX_ERR(0, 496, __pyx_L3_error)
     __pyx_v_p = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_p == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 497, __pyx_L3_error)
     __pyx_v_q = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_q == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 498, __pyx_L3_error)
     __pyx_v_nobs = __Pyx_PyInt_As_int(values[5]); if (unlikely((__pyx_v_nobs == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 499, __pyx_L3_error)
     __pyx_v_trunc_lag = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_trunc_lag == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 500, __pyx_L3_error)
     __pyx_v_backcast = __pyx_PyFloat_AsDouble(values[7]); if (unlikely((__pyx_v_backcast == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 501, __pyx_L3_error)
     __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[8], PyBUF_WRITABLE); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 502, __pyx_L3_error)
@@ -7377,26 +7384,26 @@
  *     cdef double [::1] lam
  * 
  *     omega = parameters[0]             # <<<<<<<<<<<<<<
  *     beta = parameters[1 + p + q] if q else 0.0
  *     omega_tilde = omega / (1 - beta)
  */
   __pyx_t_1 = 0;
-  __pyx_v_omega = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) )));
+  __pyx_v_omega = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) )));
 
   /* "arch/univariate/recursions.pyx":508
  * 
  *     omega = parameters[0]
  *     beta = parameters[1 + p + q] if q else 0.0             # <<<<<<<<<<<<<<
  *     omega_tilde = omega / (1 - beta)
  *     lam = _figarch_weights(parameters[1:], p, q, trunc_lag)
  */
   if ((__pyx_v_q != 0)) {
     __pyx_t_1 = ((1 + __pyx_v_p) + __pyx_v_q);
-    __pyx_t_2 = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) )));
+    __pyx_t_2 = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) )));
   } else {
     __pyx_t_2 = 0.0;
   }
   __pyx_v_beta = __pyx_t_2;
 
   /* "arch/univariate/recursions.pyx":509
  *     omega = parameters[0]
@@ -7522,15 +7529,15 @@
  *             sigma2[t] += lam[i] * fresids[t - i - 1]             # <<<<<<<<<<<<<<
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])
  * 
  */
       __pyx_t_1 = __pyx_v_i;
       __pyx_t_13 = ((__pyx_v_t - __pyx_v_i) - 1);
       __pyx_t_14 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_14)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lam.data) + __pyx_t_1)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_fresids.data) + __pyx_t_13)) ))));
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_14)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lam.data) + __pyx_t_1)) ))) * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_fresids.data) + __pyx_t_13)) ))));
     }
 
     /* "arch/univariate/recursions.pyx":518
  *         for i in range(min(t, trunc_lag)):
  *             sigma2[t] += lam[i] * fresids[t - i - 1]
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])             # <<<<<<<<<<<<<<
  * 
@@ -7576,16 +7583,16 @@
   __pyx_r = __pyx_t_15;
   __pyx_t_15 = 0;
   goto __pyx_L0;
 
   /* "arch/univariate/recursions.pyx":494
  * 
  * 
- * def figarch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                       double[::1] fresids,
+ * def figarch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                       const double[::1] fresids,
  *                       double[::1] sigma2,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __PYX_XDEC_MEMVIEW(&__pyx_t_3, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_t_5, 1);
@@ -7605,17 +7612,17 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":523
  * 
  * 
- * def aparch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                     double[::1] resids,
- *                     double[::1] abs_resids,
+ * def aparch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                      const double[::1] resids,
+ *                      const double[::1] abs_resids,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_19aparch_recursion(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_4arch_10univariate_10recursions_18aparch_recursion[] = "\n    Compute variance recursion for Asymmetric Power ARCH\n\n    Parameters\n    ----------\n    parameters : ndarray\n        Model parameters\n    resids : ndarray\n        Residuals.\n    aresids : ndarray\n        Absolute value of residuals.\n    sigma2 : ndarray\n        Conditional variances with same shape as resids\n    sigma_delta : ndarray\n        Conditional variance to the power delta with same shape as resids\n    p : int\n        Number of symmetric innovations in model\n    o : int\n        Number of asymmetric innovations in model\n    q : int\n        Number of lags of the (transformed) variance in the model\n    nobs : int\n        Length of resids\n    backcast : float\n        Value to use when initializing the recursion\n    var_bounds : 2-d array\n        nobs by 2-element array of upper and lower bounds for conditional\n        transformed variances for each time period\n    ";
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_19aparch_recursion = {"aparch_recursion", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_19aparch_recursion, METH_VARARGS|METH_KEYWORDS, __pyx_doc_4arch_10univariate_10recursions_18aparch_recursion};
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_19aparch_recursion(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -7748,25 +7755,25 @@
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
       values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
       values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
       values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
       values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
     }
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 523, __pyx_L3_error)
-    __pyx_v_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_resids.memview)) __PYX_ERR(0, 524, __pyx_L3_error)
-    __pyx_v_abs_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_abs_resids.memview)) __PYX_ERR(0, 525, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 523, __pyx_L3_error)
+    __pyx_v_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[1], 0); if (unlikely(!__pyx_v_resids.memview)) __PYX_ERR(0, 524, __pyx_L3_error)
+    __pyx_v_abs_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[2], 0); if (unlikely(!__pyx_v_abs_resids.memview)) __PYX_ERR(0, 525, __pyx_L3_error)
     __pyx_v_sigma2 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sigma2.memview)) __PYX_ERR(0, 526, __pyx_L3_error)
     __pyx_v_sigma_delta = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sigma_delta.memview)) __PYX_ERR(0, 527, __pyx_L3_error)
     __pyx_v_p = __Pyx_PyInt_As_int(values[5]); if (unlikely((__pyx_v_p == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 528, __pyx_L3_error)
     __pyx_v_o = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_o == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 529, __pyx_L3_error)
     __pyx_v_q = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_q == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 530, __pyx_L3_error)
     __pyx_v_nobs = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_nobs == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 531, __pyx_L3_error)
     __pyx_v_backcast = __pyx_PyFloat_AsDouble(values[9]); if (unlikely((__pyx_v_backcast == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 532, __pyx_L3_error)
-    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[10], PyBUF_WRITABLE); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 533, __pyx_L3_error)
+    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double__const__(values[10], 0); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 533, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("aparch_recursion", 1, 11, 11, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 523, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("arch.univariate.recursions.aparch_recursion", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
@@ -7809,15 +7816,15 @@
  *     cdef Py_ssize_t t, j
  * 
  *     delta = parameters[1 + p + o + q]             # <<<<<<<<<<<<<<
  *     for t in range(nobs):
  *         sigma_delta[t] = parameters[0]
  */
   __pyx_t_1 = (((1 + __pyx_v_p) + __pyx_v_o) + __pyx_v_q);
-  __pyx_v_delta = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) )));
+  __pyx_v_delta = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) )));
 
   /* "arch/univariate/recursions.pyx":567
  * 
  *     delta = parameters[1 + p + o + q]
  *     for t in range(nobs):             # <<<<<<<<<<<<<<
  *         sigma_delta[t] = parameters[0]
  *         for j in range(p):
@@ -7832,15 +7839,15 @@
  *     for t in range(nobs):
  *         sigma_delta[t] = parameters[0]             # <<<<<<<<<<<<<<
  *         for j in range(p):
  *             if (t - 1 - j) < 0:
  */
     __pyx_t_1 = 0;
     __pyx_t_5 = __pyx_v_t;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma_delta.data) + __pyx_t_5)) )) = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) )));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma_delta.data) + __pyx_t_5)) )) = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) )));
 
     /* "arch/univariate/recursions.pyx":569
  *     for t in range(nobs):
  *         sigma_delta[t] = parameters[0]
  *         for j in range(p):             # <<<<<<<<<<<<<<
  *             if (t - 1 - j) < 0:
  *                 shock = sqrt(backcast)
@@ -7884,15 +7891,15 @@
  *             else:
  *                 shock = abs_resids[t - 1 - j]             # <<<<<<<<<<<<<<
  *                 if o > j:
  *                     shock -= parameters[1 + p + j] * resids[t - 1 - j]
  */
       /*else*/ {
         __pyx_t_1 = ((__pyx_v_t - 1) - __pyx_v_j);
-        __pyx_v_shock = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_abs_resids.data) + __pyx_t_1)) )));
+        __pyx_v_shock = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_abs_resids.data) + __pyx_t_1)) )));
 
         /* "arch/univariate/recursions.pyx":574
  *             else:
  *                 shock = abs_resids[t - 1 - j]
  *                 if o > j:             # <<<<<<<<<<<<<<
  *                     shock -= parameters[1 + p + j] * resids[t - 1 - j]
  *             sigma_delta[t] += parameters[1 + j] * (shock ** delta)
@@ -7905,15 +7912,15 @@
  *                 if o > j:
  *                     shock -= parameters[1 + p + j] * resids[t - 1 - j]             # <<<<<<<<<<<<<<
  *             sigma_delta[t] += parameters[1 + j] * (shock ** delta)
  *         for j in range(q):
  */
           __pyx_t_1 = ((1 + __pyx_v_p) + __pyx_v_j);
           __pyx_t_5 = ((__pyx_v_t - 1) - __pyx_v_j);
-          __pyx_v_shock = (__pyx_v_shock - ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_5)) )))));
+          __pyx_v_shock = (__pyx_v_shock - ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) ))) * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_5)) )))));
 
           /* "arch/univariate/recursions.pyx":574
  *             else:
  *                 shock = abs_resids[t - 1 - j]
  *                 if o > j:             # <<<<<<<<<<<<<<
  *                     shock -= parameters[1 + p + j] * resids[t - 1 - j]
  *             sigma_delta[t] += parameters[1 + j] * (shock ** delta)
@@ -7927,15 +7934,15 @@
  *                     shock -= parameters[1 + p + j] * resids[t - 1 - j]
  *             sigma_delta[t] += parameters[1 + j] * (shock ** delta)             # <<<<<<<<<<<<<<
  *         for j in range(q):
  *             if (t - 1 - j) < 0:
  */
       __pyx_t_5 = (1 + __pyx_v_j);
       __pyx_t_1 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma_delta.data) + __pyx_t_1)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_5)) ))) * pow(__pyx_v_shock, __pyx_v_delta));
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma_delta.data) + __pyx_t_1)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_5)) ))) * pow(__pyx_v_shock, __pyx_v_delta));
     }
 
     /* "arch/univariate/recursions.pyx":577
  *                     shock -= parameters[1 + p + j] * resids[t - 1 - j]
  *             sigma_delta[t] += parameters[1 + j] * (shock ** delta)
  *         for j in range(q):             # <<<<<<<<<<<<<<
  *             if (t - 1 - j) < 0:
@@ -7961,15 +7968,15 @@
  *             if (t - 1 - j) < 0:
  *                 sigma_delta[t] += parameters[1 + p + o + j] * backcast ** (delta / 2.0)             # <<<<<<<<<<<<<<
  *             else:
  *                 sigma_delta[t] += parameters[1 + p + o + j] * sigma_delta[t - 1 - j]
  */
         __pyx_t_5 = (((1 + __pyx_v_p) + __pyx_v_o) + __pyx_v_j);
         __pyx_t_1 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma_delta.data) + __pyx_t_1)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_5)) ))) * pow(__pyx_v_backcast, (__pyx_v_delta / 2.0)));
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma_delta.data) + __pyx_t_1)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_5)) ))) * pow(__pyx_v_backcast, (__pyx_v_delta / 2.0)));
 
         /* "arch/univariate/recursions.pyx":578
  *             sigma_delta[t] += parameters[1 + j] * (shock ** delta)
  *         for j in range(q):
  *             if (t - 1 - j) < 0:             # <<<<<<<<<<<<<<
  *                 sigma_delta[t] += parameters[1 + p + o + j] * backcast ** (delta / 2.0)
  *             else:
@@ -7984,15 +7991,15 @@
  *         sigma2[t] = sigma_delta[t] ** (2.0 / delta)
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])
  */
       /*else*/ {
         __pyx_t_5 = (((1 + __pyx_v_p) + __pyx_v_o) + __pyx_v_j);
         __pyx_t_1 = ((__pyx_v_t - 1) - __pyx_v_j);
         __pyx_t_10 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma_delta.data) + __pyx_t_10)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_5)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma_delta.data) + __pyx_t_1)) ))));
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma_delta.data) + __pyx_t_10)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_5)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma_delta.data) + __pyx_t_1)) ))));
       }
       __pyx_L11:;
     }
 
     /* "arch/univariate/recursions.pyx":582
  *             else:
  *                 sigma_delta[t] += parameters[1 + p + o + j] * sigma_delta[t - 1 - j]
@@ -8010,15 +8017,15 @@
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])             # <<<<<<<<<<<<<<
  *         sigma_delta[t] = sigma2[t] ** (delta / 2.0)
  *     return np.asarray(sigma2)
  */
     __pyx_t_1 = __pyx_v_t;
     __pyx_t_5 = __pyx_v_t;
     __pyx_t_10 = 0;
-    __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_1)) )))), (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_5 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_10)) )))));
+    __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_1)) )))), (&(*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_5 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_10)) )))));
 
     /* "arch/univariate/recursions.pyx":584
  *         sigma2[t] = sigma_delta[t] ** (2.0 / delta)
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])
  *         sigma_delta[t] = sigma2[t] ** (delta / 2.0)             # <<<<<<<<<<<<<<
  *     return np.asarray(sigma2)
  * 
@@ -8062,17 +8069,17 @@
   __pyx_r = __pyx_t_11;
   __pyx_t_11 = 0;
   goto __pyx_L0;
 
   /* "arch/univariate/recursions.pyx":523
  * 
  * 
- * def aparch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                     double[::1] resids,
- *                     double[::1] abs_resids,
+ * def aparch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                      const double[::1] resids,
+ *                      const double[::1] abs_resids,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_13);
@@ -8125,15 +8132,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":592
  *         pass
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_17VolatilityUpdater_3initialize_update(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_17VolatilityUpdater_3initialize_update = {"initialize_update", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_17VolatilityUpdater_3initialize_update, METH_VARARGS|METH_KEYWORDS, 0};
@@ -8187,15 +8194,15 @@
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 592, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 592, __pyx_L3_error)
     __pyx_v_backcast = values[1];
     __pyx_v_nobs = __Pyx_PyIndex_AsSsize_t(values[2]); if (unlikely((__pyx_v_nobs == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 592, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("initialize_update", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 592, __pyx_L3_error)
   __pyx_L3_error:;
@@ -8224,15 +8231,15 @@
 }
 
 /* "arch/univariate/recursions.pyx":595
  *         pass
  * 
  *     cdef void update(self,             # <<<<<<<<<<<<<<
  *                      Py_ssize_t t,
- *                      double[::1] parameters,
+ *                      const double[::1] parameters,
  */
 
 static void __pyx_f_4arch_10univariate_10recursions_17VolatilityUpdater_update(CYTHON_UNUSED struct __pyx_obj_4arch_10univariate_10recursions_VolatilityUpdater *__pyx_v_self, CYTHON_UNUSED Py_ssize_t __pyx_v_t, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_parameters, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_resids, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_sigma2, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_var_bounds) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("update", 0);
 
   /* function exit code */
@@ -8240,15 +8247,15 @@
 }
 
 /* "arch/univariate/recursions.pyx":604
  *         pass
  * 
  *     def _update_tester(self,             # <<<<<<<<<<<<<<
  *                        Py_ssize_t t,
- *                        double[::1] parameters,
+ *                        const double[::1] parameters,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_17VolatilityUpdater_5_update_tester(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_17VolatilityUpdater_5_update_tester = {"_update_tester", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_17VolatilityUpdater_5_update_tester, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_17VolatilityUpdater_5_update_tester(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   Py_ssize_t __pyx_v_t;
@@ -8321,18 +8328,18 @@
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
     }
     __pyx_v_t = __Pyx_PyIndex_AsSsize_t(values[0]); if (unlikely((__pyx_v_t == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 605, __pyx_L3_error)
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 606, __pyx_L3_error)
-    __pyx_v_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_resids.memview)) __PYX_ERR(0, 607, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[1], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 606, __pyx_L3_error)
+    __pyx_v_resids = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[2], 0); if (unlikely(!__pyx_v_resids.memview)) __PYX_ERR(0, 607, __pyx_L3_error)
     __pyx_v_sigma2 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sigma2.memview)) __PYX_ERR(0, 608, __pyx_L3_error)
-    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 609, __pyx_L3_error)
+    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double__const__(values[4], 0); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 609, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_update_tester", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 604, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("arch.univariate.recursions.VolatilityUpdater._update_tester", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
@@ -8348,27 +8355,27 @@
 static PyObject *__pyx_pf_4arch_10univariate_10recursions_17VolatilityUpdater_4_update_tester(struct __pyx_obj_4arch_10univariate_10recursions_VolatilityUpdater *__pyx_v_self, Py_ssize_t __pyx_v_t, __Pyx_memviewslice __pyx_v_parameters, __Pyx_memviewslice __pyx_v_resids, __Pyx_memviewslice __pyx_v_sigma2, __Pyx_memviewslice __pyx_v_var_bounds) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_update_tester", 0);
 
   /* "arch/univariate/recursions.pyx":610
  *                        double[::1] sigma2,
- *                        double[:,::1] var_bounds):
+ *                        const double[:,::1] var_bounds):
  *         self.update(t, parameters, resids, sigma2, var_bounds)             # <<<<<<<<<<<<<<
  * 
  * cdef class GARCHUpdater(VolatilityUpdater):
  */
   ((struct __pyx_vtabstruct_4arch_10univariate_10recursions_VolatilityUpdater *)__pyx_v_self->__pyx_vtab)->update(__pyx_v_self, __pyx_v_t, __pyx_v_parameters, __pyx_v_resids, __pyx_v_sigma2, __pyx_v_var_bounds);
 
   /* "arch/univariate/recursions.pyx":604
  *         pass
  * 
  *     def _update_tester(self,             # <<<<<<<<<<<<<<
  *                        Py_ssize_t t,
- *                        double[::1] parameters,
+ *                        const double[::1] parameters,
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __PYX_XDEC_MEMVIEW(&__pyx_v_parameters, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_resids, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_sigma2, 1);
@@ -8803,15 +8810,15 @@
   __pyx_v_self->power = __pyx_v_power;
 
   /* "arch/univariate/recursions.pyx":622
  *         self.q = q
  *         self.power = power
  *         self.backcast = -1.0             # <<<<<<<<<<<<<<
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
  */
   __pyx_v_self->backcast = -1.0;
 
   /* "arch/univariate/recursions.pyx":617
  *         double power, backcast
  * 
  *     def __init__(self, int p, int o, int q, double power):             # <<<<<<<<<<<<<<
@@ -8824,15 +8831,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":624
  *         self.backcast = -1.0
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         self.backcast = backcast
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_12GARCHUpdater_3initialize_update(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_12GARCHUpdater_3initialize_update = {"initialize_update", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_12GARCHUpdater_3initialize_update, METH_VARARGS|METH_KEYWORDS, 0};
@@ -8886,15 +8893,15 @@
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 624, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 624, __pyx_L3_error)
     __pyx_v_backcast = values[1];
     __pyx_v_nobs = __Pyx_PyIndex_AsSsize_t(values[2]); if (unlikely((__pyx_v_nobs == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 624, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("initialize_update", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 624, __pyx_L3_error)
   __pyx_L3_error:;
@@ -8916,26 +8923,26 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("initialize_update", 0);
 
   /* "arch/univariate/recursions.pyx":625
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
  *         self.backcast = backcast             # <<<<<<<<<<<<<<
  * 
  *     cdef void update(self,
  */
   __pyx_t_1 = __pyx_PyFloat_AsDouble(__pyx_v_backcast); if (unlikely((__pyx_t_1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 625, __pyx_L1_error)
   __pyx_v_self->backcast = __pyx_t_1;
 
   /* "arch/univariate/recursions.pyx":624
  *         self.backcast = -1.0
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         self.backcast = backcast
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
@@ -8950,15 +8957,15 @@
 }
 
 /* "arch/univariate/recursions.pyx":627
  *         self.backcast = backcast
  * 
  *     cdef void update(self,             # <<<<<<<<<<<<<<
  *                      Py_ssize_t t,
- *                      double[::1] parameters,
+ *                      const double[::1] parameters,
  */
 
 static void __pyx_f_4arch_10univariate_10recursions_12GARCHUpdater_update(struct __pyx_obj_4arch_10univariate_10recursions_GARCHUpdater *__pyx_v_self, Py_ssize_t __pyx_v_t, __Pyx_memviewslice __pyx_v_parameters, __Pyx_memviewslice __pyx_v_resids, __Pyx_memviewslice __pyx_v_sigma2, __Pyx_memviewslice __pyx_v_var_bounds) {
   int __pyx_v_p;
   int __pyx_v_o;
   int __pyx_v_q;
   double __pyx_v_power;
@@ -9017,15 +9024,15 @@
  *         loc = 0
  *         sigma2[t] = parameters[loc]             # <<<<<<<<<<<<<<
  *         loc += 1
  *         for j in range(p):
  */
   __pyx_t_3 = __pyx_v_loc;
   __pyx_t_4 = __pyx_v_t;
-  *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) )) = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_3)) )));
+  *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) )) = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_3)) )));
 
   /* "arch/univariate/recursions.pyx":641
  *         loc = 0
  *         sigma2[t] = parameters[loc]
  *         loc += 1             # <<<<<<<<<<<<<<
  *         for j in range(p):
  *             if (t - 1 - j) < 0:
@@ -9059,15 +9066,15 @@
  *             if (t - 1 - j) < 0:
  *                 sigma2[t] += parameters[loc] * backcast             # <<<<<<<<<<<<<<
  *             else:
  *                 sigma2[t] += parameters[loc] * (fabs(resids[t - 1 - j]) ** power)
  */
       __pyx_t_3 = __pyx_v_loc;
       __pyx_t_4 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_3)) ))) * __pyx_v_backcast);
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_3)) ))) * __pyx_v_backcast);
 
       /* "arch/univariate/recursions.pyx":643
  *         loc += 1
  *         for j in range(p):
  *             if (t - 1 - j) < 0:             # <<<<<<<<<<<<<<
  *                 sigma2[t] += parameters[loc] * backcast
  *             else:
@@ -9082,15 +9089,15 @@
  *             loc += 1
  *         for j in range(o):
  */
     /*else*/ {
       __pyx_t_3 = __pyx_v_loc;
       __pyx_t_4 = ((__pyx_v_t - 1) - __pyx_v_j);
       __pyx_t_8 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_8)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_3)) ))) * pow(fabs((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_4)) )))), __pyx_v_power));
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_8)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_3)) ))) * pow(fabs((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_4)) )))), __pyx_v_power));
     }
     __pyx_L5:;
 
     /* "arch/univariate/recursions.pyx":647
  *             else:
  *                 sigma2[t] += parameters[loc] * (fabs(resids[t - 1 - j]) ** power)
  *             loc += 1             # <<<<<<<<<<<<<<
@@ -9127,15 +9134,15 @@
  *             if (t - 1 - j) < 0:
  *                 sigma2[t] += parameters[loc] * 0.5 * backcast             # <<<<<<<<<<<<<<
  *             else:
  *                 sigma2[t] += (
  */
       __pyx_t_4 = __pyx_v_loc;
       __pyx_t_3 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_3)) )) += (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * 0.5) * __pyx_v_backcast);
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_3)) )) += (((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * 0.5) * __pyx_v_backcast);
 
       /* "arch/univariate/recursions.pyx":649
  *             loc += 1
  *         for j in range(o):
  *             if (t - 1 - j) < 0:             # <<<<<<<<<<<<<<
  *                 sigma2[t] += parameters[loc] * 0.5 * backcast
  *             else:
@@ -9183,15 +9190,15 @@
  *                 sigma2[t] += parameters[loc] * 0.5 * backcast
  *             else:
  *                 sigma2[t] += (             # <<<<<<<<<<<<<<
  *                         parameters[loc]
  *                         * (fabs(resids[t - 1 - j]) ** power)
  */
       __pyx_t_9 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_9)) )) += (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * pow(fabs((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_3)) )))), __pyx_v_power)) * ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_8)) ))) < 0.0));
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_9)) )) += (((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_4)) ))) * pow(fabs((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_3)) )))), __pyx_v_power)) * ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_8)) ))) < 0.0));
     }
     __pyx_L8:;
 
     /* "arch/univariate/recursions.pyx":657
  *                         * (resids[t - 1 - j] < 0)
  *                 )
  *             loc += 1             # <<<<<<<<<<<<<<
@@ -9228,15 +9235,15 @@
  *             if (t - 1 - j) < 0:
  *                 sigma2[t] += parameters[loc] * backcast             # <<<<<<<<<<<<<<
  *             else:
  *                 sigma2[t] += parameters[loc] * sigma2[t - 1 - j]
  */
       __pyx_t_8 = __pyx_v_loc;
       __pyx_t_3 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_3)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_8)) ))) * __pyx_v_backcast);
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_3)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_8)) ))) * __pyx_v_backcast);
 
       /* "arch/univariate/recursions.pyx":659
  *             loc += 1
  *         for j in range(q):
  *             if (t - 1 - j) < 0:             # <<<<<<<<<<<<<<
  *                 sigma2[t] += parameters[loc] * backcast
  *             else:
@@ -9251,15 +9258,15 @@
  *             loc += 1
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])
  */
     /*else*/ {
       __pyx_t_8 = __pyx_v_loc;
       __pyx_t_3 = ((__pyx_v_t - 1) - __pyx_v_j);
       __pyx_t_4 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_8)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_3)) ))));
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_8)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_3)) ))));
     }
     __pyx_L11:;
 
     /* "arch/univariate/recursions.pyx":663
  *             else:
  *                 sigma2[t] += parameters[loc] * sigma2[t - 1 - j]
  *             loc += 1             # <<<<<<<<<<<<<<
@@ -9275,22 +9282,22 @@
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])             # <<<<<<<<<<<<<<
  * 
  * cdef class HARCHUpdater(VolatilityUpdater):
  */
   __pyx_t_3 = __pyx_v_t;
   __pyx_t_8 = __pyx_v_t;
   __pyx_t_4 = 0;
-  __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_3)) )))), (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_8 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_4)) )))));
+  __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_3)) )))), (&(*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_8 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_4)) )))));
 
   /* "arch/univariate/recursions.pyx":627
  *         self.backcast = backcast
  * 
  *     cdef void update(self,             # <<<<<<<<<<<<<<
  *                      Py_ssize_t t,
- *                      double[::1] parameters,
+ *                      const double[::1] parameters,
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 /* "(tree fragment)":1
@@ -9614,15 +9621,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":671
  *         double backcast
  * 
- *     def __init__(self, np.int32_t[::1] lags):             # <<<<<<<<<<<<<<
+ *     def __init__(self, const np.int32_t[::1] lags):             # <<<<<<<<<<<<<<
  *         self.lags = lags
  *         self.backcast = -1.0
  */
 
 /* Python wrapper */
 static int __pyx_pw_4arch_10univariate_10recursions_12HARCHUpdater_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_4arch_10univariate_10recursions_12HARCHUpdater_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -9655,15 +9662,15 @@
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 671, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
-    __pyx_v_lags = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int32_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_lags.memview)) __PYX_ERR(0, 671, __pyx_L3_error)
+    __pyx_v_lags = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int32_t__const__(values[0], 0); if (unlikely(!__pyx_v_lags.memview)) __PYX_ERR(0, 671, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 671, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("arch.univariate.recursions.HARCHUpdater.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
@@ -9679,36 +9686,36 @@
 static int __pyx_pf_4arch_10univariate_10recursions_12HARCHUpdater___init__(struct __pyx_obj_4arch_10univariate_10recursions_HARCHUpdater *__pyx_v_self, __Pyx_memviewslice __pyx_v_lags) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 0);
 
   /* "arch/univariate/recursions.pyx":672
  * 
- *     def __init__(self, np.int32_t[::1] lags):
+ *     def __init__(self, const np.int32_t[::1] lags):
  *         self.lags = lags             # <<<<<<<<<<<<<<
  *         self.backcast = -1.0
  * 
  */
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->lags, 0);
   __PYX_INC_MEMVIEW(&__pyx_v_lags, 0);
   __pyx_v_self->lags = __pyx_v_lags;
 
   /* "arch/univariate/recursions.pyx":673
- *     def __init__(self, np.int32_t[::1] lags):
+ *     def __init__(self, const np.int32_t[::1] lags):
  *         self.lags = lags
  *         self.backcast = -1.0             # <<<<<<<<<<<<<<
  * 
  *     def __setstate__(self, state):
  */
   __pyx_v_self->backcast = -1.0;
 
   /* "arch/univariate/recursions.pyx":671
  *         double backcast
  * 
- *     def __init__(self, np.int32_t[::1] lags):             # <<<<<<<<<<<<<<
+ *     def __init__(self, const np.int32_t[::1] lags):             # <<<<<<<<<<<<<<
  *         self.lags = lags
  *         self.backcast = -1.0
  */
 
   /* function exit code */
   __pyx_r = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_lags, 1);
@@ -9817,24 +9824,24 @@
   __Pyx_RefNannySetupContext("__reduce__", 0);
 
   /* "arch/univariate/recursions.pyx":679
  * 
  *     def __reduce__(self):
  *         return HARCHUpdater, (np.asarray(self.lags),), (self.backcast,)             # <<<<<<<<<<<<<<
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 679, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 679, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_v_self->lags.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 679, __pyx_L1_error)}
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->lags, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int32_t, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->lags, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int32_t__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 679, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
@@ -9896,15 +9903,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":681
  *         return HARCHUpdater, (np.asarray(self.lags),), (self.backcast,)
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         self.backcast = backcast
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_12HARCHUpdater_7initialize_update(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_12HARCHUpdater_7initialize_update = {"initialize_update", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_12HARCHUpdater_7initialize_update, METH_VARARGS|METH_KEYWORDS, 0};
@@ -9958,15 +9965,15 @@
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 681, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 681, __pyx_L3_error)
     __pyx_v_backcast = values[1];
     __pyx_v_nobs = __Pyx_PyIndex_AsSsize_t(values[2]); if (unlikely((__pyx_v_nobs == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 681, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("initialize_update", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 681, __pyx_L3_error)
   __pyx_L3_error:;
@@ -9988,26 +9995,26 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("initialize_update", 0);
 
   /* "arch/univariate/recursions.pyx":682
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
  *         self.backcast = backcast             # <<<<<<<<<<<<<<
  * 
  *     cdef void update(self,
  */
   __pyx_t_1 = __pyx_PyFloat_AsDouble(__pyx_v_backcast); if (unlikely((__pyx_t_1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 682, __pyx_L1_error)
   __pyx_v_self->backcast = __pyx_t_1;
 
   /* "arch/univariate/recursions.pyx":681
  *         return HARCHUpdater, (np.asarray(self.lags),), (self.backcast,)
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         self.backcast = backcast
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
@@ -10022,15 +10029,15 @@
 }
 
 /* "arch/univariate/recursions.pyx":684
  *         self.backcast = backcast
  * 
  *     cdef void update(self,             # <<<<<<<<<<<<<<
  *                      Py_ssize_t t,
- *                      double[::1] parameters,
+ *                      const double[::1] parameters,
  */
 
 static void __pyx_f_4arch_10univariate_10recursions_12HARCHUpdater_update(struct __pyx_obj_4arch_10univariate_10recursions_HARCHUpdater *__pyx_v_self, Py_ssize_t __pyx_v_t, __Pyx_memviewslice __pyx_v_parameters, __Pyx_memviewslice __pyx_v_resids, __Pyx_memviewslice __pyx_v_sigma2, __Pyx_memviewslice __pyx_v_var_bounds) {
   double __pyx_v_backcast;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   double __pyx_v_param;
@@ -10066,15 +10073,15 @@
  * 
  *         sigma2[t] = parameters[0]             # <<<<<<<<<<<<<<
  *         for i in range(self.lags.shape[0]):
  *             param = parameters[i + 1] / self.lags[i]
  */
   __pyx_t_2 = 0;
   __pyx_t_3 = __pyx_v_t;
-  *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_3)) )) = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_2)) )));
+  *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_3)) )) = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_2)) )));
 
   /* "arch/univariate/recursions.pyx":697
  * 
  *         sigma2[t] = parameters[0]
  *         for i in range(self.lags.shape[0]):             # <<<<<<<<<<<<<<
  *             param = parameters[i + 1] / self.lags[i]
  *             for j in range(self.lags[i]):
@@ -10091,26 +10098,26 @@
  *             param = parameters[i + 1] / self.lags[i]             # <<<<<<<<<<<<<<
  *             for j in range(self.lags[i]):
  *                 if (t - j - 1) >= 0:
  */
     __pyx_t_2 = (__pyx_v_i + 1);
     if (unlikely(!__pyx_v_self->lags.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 698, __pyx_L1_error)}
     __pyx_t_3 = __pyx_v_i;
-    __pyx_v_param = ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_2)) ))) / ((double)(*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int32_t *) __pyx_v_self->lags.data) + __pyx_t_3)) )))));
+    __pyx_v_param = (((double)(*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_2)) )))) / ((double)(*((__pyx_t_5numpy_int32_t const  *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int32_t const  *) __pyx_v_self->lags.data) + __pyx_t_3)) )))));
 
     /* "arch/univariate/recursions.pyx":699
  *         for i in range(self.lags.shape[0]):
  *             param = parameters[i + 1] / self.lags[i]
  *             for j in range(self.lags[i]):             # <<<<<<<<<<<<<<
  *                 if (t - j - 1) >= 0:
  *                     sigma2[t] += param * resids[t - j - 1] * resids[t - j - 1]
  */
     if (unlikely(!__pyx_v_self->lags.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 699, __pyx_L1_error)}
     __pyx_t_3 = __pyx_v_i;
-    __pyx_t_7 = (*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int32_t *) __pyx_v_self->lags.data) + __pyx_t_3)) )));
+    __pyx_t_7 = (*((__pyx_t_5numpy_int32_t const  *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int32_t const  *) __pyx_v_self->lags.data) + __pyx_t_3)) )));
     __pyx_t_8 = __pyx_t_7;
     for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_8; __pyx_t_9+=1) {
       __pyx_v_j = __pyx_t_9;
 
       /* "arch/univariate/recursions.pyx":700
  *             param = parameters[i + 1] / self.lags[i]
  *             for j in range(self.lags[i]):
@@ -10127,15 +10134,15 @@
  *                     sigma2[t] += param * resids[t - j - 1] * resids[t - j - 1]             # <<<<<<<<<<<<<<
  *                 else:
  *                     sigma2[t] += param * backcast
  */
         __pyx_t_3 = ((__pyx_v_t - __pyx_v_j) - 1);
         __pyx_t_2 = ((__pyx_v_t - __pyx_v_j) - 1);
         __pyx_t_11 = __pyx_v_t;
-        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_11)) )) += ((__pyx_v_param * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_3)) )))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_2)) ))));
+        *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_11)) )) += ((__pyx_v_param * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_3)) )))) * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_2)) ))));
 
         /* "arch/univariate/recursions.pyx":700
  *             param = parameters[i + 1] / self.lags[i]
  *             for j in range(self.lags[i]):
  *                 if (t - j - 1) >= 0:             # <<<<<<<<<<<<<<
  *                     sigma2[t] += param * resids[t - j - 1] * resids[t - j - 1]
  *                 else:
@@ -10164,22 +10171,22 @@
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])             # <<<<<<<<<<<<<<
  * 
  * cdef class EWMAUpdater(VolatilityUpdater):
  */
   __pyx_t_2 = __pyx_v_t;
   __pyx_t_3 = __pyx_v_t;
   __pyx_t_11 = 0;
-  __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_2)) )))), (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_3 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_11)) )))));
+  __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_2)) )))), (&(*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_3 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_11)) )))));
 
   /* "arch/univariate/recursions.pyx":684
  *         self.backcast = backcast
  * 
  *     cdef void update(self,             # <<<<<<<<<<<<<<
  *                      Py_ssize_t t,
- *                      double[::1] parameters,
+ *                      const double[::1] parameters,
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("arch.univariate.recursions.HARCHUpdater.update", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
@@ -10308,53 +10315,53 @@
   __pyx_t_5.data = NULL;
 
   /* "arch/univariate/recursions.pyx":716
  *         self.estimate_lam = lam is None
  *         self.params = np.zeros(3)
  *         if lam is not None:             # <<<<<<<<<<<<<<
  *             self.params[1] = 1.0 - lam
- *             self.params[2] =lam
+ *             self.params[2] = lam
  */
   __pyx_t_1 = (__pyx_v_lam != Py_None);
   __pyx_t_6 = (__pyx_t_1 != 0);
   if (__pyx_t_6) {
 
     /* "arch/univariate/recursions.pyx":717
  *         self.params = np.zeros(3)
  *         if lam is not None:
  *             self.params[1] = 1.0 - lam             # <<<<<<<<<<<<<<
- *             self.params[2] =lam
+ *             self.params[2] = lam
  * 
  */
     __pyx_t_2 = __Pyx_PyFloat_SubtractCObj(__pyx_float_1_0, __pyx_v_lam, 1.0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 717, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_7 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_7 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 717, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (unlikely(!__pyx_v_self->params.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 717, __pyx_L1_error)}
     __pyx_t_8 = 1;
     *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->params.data) + __pyx_t_8)) )) = __pyx_t_7;
 
     /* "arch/univariate/recursions.pyx":718
  *         if lam is not None:
  *             self.params[1] = 1.0 - lam
- *             self.params[2] =lam             # <<<<<<<<<<<<<<
+ *             self.params[2] = lam             # <<<<<<<<<<<<<<
  * 
  *     def __setstate__(self, state):
  */
     __pyx_t_7 = __pyx_PyFloat_AsDouble(__pyx_v_lam); if (unlikely((__pyx_t_7 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 718, __pyx_L1_error)
     if (unlikely(!__pyx_v_self->params.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 718, __pyx_L1_error)}
     __pyx_t_8 = 2;
     *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->params.data) + __pyx_t_8)) )) = __pyx_t_7;
 
     /* "arch/univariate/recursions.pyx":716
  *         self.estimate_lam = lam is None
  *         self.params = np.zeros(3)
  *         if lam is not None:             # <<<<<<<<<<<<<<
  *             self.params[1] = 1.0 - lam
- *             self.params[2] =lam
+ *             self.params[2] = lam
  */
   }
 
   /* "arch/univariate/recursions.pyx":713
  *         double backcast
  * 
  *     def __init__(self, object lam):             # <<<<<<<<<<<<<<
@@ -10374,15 +10381,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":720
- *             self.params[2] =lam
+ *             self.params[2] = lam
  * 
  *     def __setstate__(self, state):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t i
  *         self.backcast = state[0]
  */
 
 /* Python wrapper */
@@ -10461,15 +10468,15 @@
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(!__pyx_v_self->params.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 725, __pyx_L1_error)}
     __pyx_t_4 = __pyx_v_i;
     *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->params.data) + __pyx_t_4)) )) = __pyx_t_2;
   }
 
   /* "arch/univariate/recursions.pyx":720
- *             self.params[2] =lam
+ *             self.params[2] = lam
  * 
  *     def __setstate__(self, state):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t i
  *         self.backcast = state[0]
  */
 
   /* function exit code */
@@ -10546,15 +10553,15 @@
   __pyx_t_1 = 0;
 
   /* "arch/univariate/recursions.pyx":729
  *     def __reduce__(self):
  *         lam = None if self.estimate_lam else self.params[2]
  *         return EWMAUpdater, (lam,), (self.backcast, np.asarray(self.params))             # <<<<<<<<<<<<<<
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 729, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_lam);
   __Pyx_GIVEREF(__pyx_v_lam);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_lam);
@@ -10631,15 +10638,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":731
  *         return EWMAUpdater, (lam,), (self.backcast, np.asarray(self.params))
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         if self.estimate_lam:
  *             self.params[1] = 1.0 - parameters[0]
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_11EWMAUpdater_7initialize_update(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_11EWMAUpdater_7initialize_update = {"initialize_update", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_11EWMAUpdater_7initialize_update, METH_VARARGS|METH_KEYWORDS, 0};
@@ -10693,15 +10700,15 @@
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 731, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 731, __pyx_L3_error)
     __pyx_v_backcast = values[1];
     __pyx_v_nobs = __Pyx_PyIndex_AsSsize_t(values[2]); if (unlikely((__pyx_v_nobs == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 731, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("initialize_update", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 731, __pyx_L3_error)
   __pyx_L3_error:;
@@ -10726,49 +10733,49 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("initialize_update", 0);
 
   /* "arch/univariate/recursions.pyx":732
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
  *         if self.estimate_lam:             # <<<<<<<<<<<<<<
  *             self.params[1] = 1.0 - parameters[0]
  *             self.params[2] = parameters[0]
  */
   __pyx_t_1 = (__pyx_v_self->estimate_lam != 0);
   if (__pyx_t_1) {
 
     /* "arch/univariate/recursions.pyx":733
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
  *         if self.estimate_lam:
  *             self.params[1] = 1.0 - parameters[0]             # <<<<<<<<<<<<<<
  *             self.params[2] = parameters[0]
  *         self.backcast = backcast
  */
     __pyx_t_2 = 0;
     if (unlikely(!__pyx_v_self->params.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 733, __pyx_L1_error)}
     __pyx_t_3 = 1;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->params.data) + __pyx_t_3)) )) = (1.0 - (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_2)) ))));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->params.data) + __pyx_t_3)) )) = (1.0 - (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_2)) ))));
 
     /* "arch/univariate/recursions.pyx":734
  *         if self.estimate_lam:
  *             self.params[1] = 1.0 - parameters[0]
  *             self.params[2] = parameters[0]             # <<<<<<<<<<<<<<
  *         self.backcast = backcast
  * 
  */
     __pyx_t_2 = 0;
     if (unlikely(!__pyx_v_self->params.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 734, __pyx_L1_error)}
     __pyx_t_3 = 2;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->params.data) + __pyx_t_3)) )) = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_2)) )));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->params.data) + __pyx_t_3)) )) = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_2)) )));
 
     /* "arch/univariate/recursions.pyx":732
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
  *         if self.estimate_lam:             # <<<<<<<<<<<<<<
  *             self.params[1] = 1.0 - parameters[0]
  *             self.params[2] = parameters[0]
  */
   }
 
   /* "arch/univariate/recursions.pyx":735
@@ -10780,15 +10787,15 @@
  */
   __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_v_backcast); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 735, __pyx_L1_error)
   __pyx_v_self->backcast = __pyx_t_4;
 
   /* "arch/univariate/recursions.pyx":731
  *         return EWMAUpdater, (lam,), (self.backcast, np.asarray(self.params))
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         if self.estimate_lam:
  *             self.params[1] = 1.0 - parameters[0]
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
@@ -10803,15 +10810,15 @@
 }
 
 /* "arch/univariate/recursions.pyx":737
  *         self.backcast = backcast
  * 
  *     cdef void update(self,             # <<<<<<<<<<<<<<
  *                      Py_ssize_t t,
- *                      double[::1] parameters,
+ *                      const double[::1] parameters,
  */
 
 static void __pyx_f_4arch_10univariate_10recursions_11EWMAUpdater_update(struct __pyx_obj_4arch_10univariate_10recursions_EWMAUpdater *__pyx_v_self, Py_ssize_t __pyx_v_t, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_parameters, __Pyx_memviewslice __pyx_v_resids, __Pyx_memviewslice __pyx_v_sigma2, __Pyx_memviewslice __pyx_v_var_bounds) {
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   int __pyx_t_3;
@@ -10894,36 +10901,36 @@
  *             sigma2[t] += self.backcast
  *         else:
  *             sigma2[t] += (self.params[1] * resids[t-1] * resids[t-1] +             # <<<<<<<<<<<<<<
  *                           self.params[2] * sigma2[t-1])
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])
  */
     __pyx_t_7 = __pyx_v_t;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_7)) )) += ((((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->params.data) + __pyx_t_1)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_2)) )))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_4)) )))) + ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->params.data) + __pyx_t_5)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_6)) )))));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_7)) )) += ((((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->params.data) + __pyx_t_1)) ))) * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_2)) )))) * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_4)) )))) + ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->params.data) + __pyx_t_5)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_6)) )))));
   }
   __pyx_L3:;
 
   /* "arch/univariate/recursions.pyx":751
  *             sigma2[t] += (self.params[1] * resids[t-1] * resids[t-1] +
  *                           self.params[2] * sigma2[t-1])
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])             # <<<<<<<<<<<<<<
  * 
  * cdef class MIDASUpdater(VolatilityUpdater):
  */
   __pyx_t_6 = __pyx_v_t;
   __pyx_t_5 = __pyx_v_t;
   __pyx_t_4 = 0;
-  __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_6)) )))), (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_5 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_4)) )))));
+  __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_6)) )))), (&(*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_5 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_4)) )))));
 
   /* "arch/univariate/recursions.pyx":737
  *         self.backcast = backcast
  * 
  *     cdef void update(self,             # <<<<<<<<<<<<<<
  *                      Py_ssize_t t,
- *                      double[::1] parameters,
+ *                      const double[::1] parameters,
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("arch.univariate.recursions.EWMAUpdater.update", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
@@ -11941,15 +11948,15 @@
     __pyx_v_i = __pyx_t_4;
 
     /* "arch/univariate/recursions.pyx":811
  *             j += 1.0
  *         for i in range(m):
  *             self.weights[i] /= sum_w             # <<<<<<<<<<<<<<
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
  */
     if (unlikely(!__pyx_v_self->weights.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 811, __pyx_L1_error)}
     __pyx_t_5 = __pyx_v_i;
     *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->weights.data) + __pyx_t_5)) )) /= __pyx_v_sum_w;
   }
 
   /* "arch/univariate/recursions.pyx":798
@@ -11971,15 +11978,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":813
  *             self.weights[i] /= sum_w
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         cdef double alpha, gamma, theta
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_12MIDASUpdater_7initialize_update(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_12MIDASUpdater_7initialize_update = {"initialize_update", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_12MIDASUpdater_7initialize_update, METH_VARARGS|METH_KEYWORDS, 0};
@@ -12033,15 +12040,15 @@
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 813, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 813, __pyx_L3_error)
     __pyx_v_backcast = values[1];
     __pyx_v_nobs = __Pyx_PyIndex_AsSsize_t(values[2]); if (unlikely((__pyx_v_nobs == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 813, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("initialize_update", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 813, __pyx_L3_error)
   __pyx_L3_error:;
@@ -12083,27 +12090,27 @@
  *         cdef double alpha, gamma, theta
  * 
  *         self.update_weights(parameters[2 + <int>self.asym])             # <<<<<<<<<<<<<<
  *         alpha = parameters[1]
  *         if self.asym:
  */
   __pyx_t_1 = (2 + ((int)__pyx_v_self->asym));
-  __pyx_t_2 = ((struct __pyx_vtabstruct_4arch_10univariate_10recursions_MIDASUpdater *)__pyx_v_self->__pyx_base.__pyx_vtab)->update_weights(__pyx_v_self, (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) )))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 816, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_4arch_10univariate_10recursions_MIDASUpdater *)__pyx_v_self->__pyx_base.__pyx_vtab)->update_weights(__pyx_v_self, (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) )))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 816, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "arch/univariate/recursions.pyx":817
  * 
  *         self.update_weights(parameters[2 + <int>self.asym])
  *         alpha = parameters[1]             # <<<<<<<<<<<<<<
  *         if self.asym:
  *             gamma = parameters[2]
  */
   __pyx_t_1 = 1;
-  __pyx_v_alpha = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) )));
+  __pyx_v_alpha = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) )));
 
   /* "arch/univariate/recursions.pyx":818
  *         self.update_weights(parameters[2 + <int>self.asym])
  *         alpha = parameters[1]
  *         if self.asym:             # <<<<<<<<<<<<<<
  *             gamma = parameters[2]
  *         else:
@@ -12115,15 +12122,15 @@
  *         alpha = parameters[1]
  *         if self.asym:
  *             gamma = parameters[2]             # <<<<<<<<<<<<<<
  *         else:
  *             gamma = 0.0
  */
     __pyx_t_1 = 2;
-    __pyx_v_gamma = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) )));
+    __pyx_v_gamma = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) )));
 
     /* "arch/univariate/recursions.pyx":818
  *         self.update_weights(parameters[2 + <int>self.asym])
  *         alpha = parameters[1]
  *         if self.asym:             # <<<<<<<<<<<<<<
  *             gamma = parameters[2]
  *         else:
@@ -12248,15 +12255,15 @@
  * 
  */
   }
 
   /* "arch/univariate/recursions.pyx":813
  *             self.weights[i] /= sum_w
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         cdef double alpha, gamma, theta
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
@@ -12276,15 +12283,15 @@
 }
 
 /* "arch/univariate/recursions.pyx":830
  *             self.resids2 = np.empty(nobs)
  * 
  *     cdef void update(self,             # <<<<<<<<<<<<<<
  *                      Py_ssize_t t,
- *                      double[::1] parameters,
+ *                      const double[::1] parameters,
  */
 
 static void __pyx_f_4arch_10univariate_10recursions_12MIDASUpdater_update(struct __pyx_obj_4arch_10univariate_10recursions_MIDASUpdater *__pyx_v_self, Py_ssize_t __pyx_v_t, __Pyx_memviewslice __pyx_v_parameters, __Pyx_memviewslice __pyx_v_resids, __Pyx_memviewslice __pyx_v_sigma2, __Pyx_memviewslice __pyx_v_var_bounds) {
   Py_ssize_t __pyx_v_i;
   double __pyx_v_omega;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
@@ -12305,15 +12312,15 @@
  *         cdef double param, omega, alpha, gamma
  * 
  *         omega = parameters[0]             # <<<<<<<<<<<<<<
  *         if t > 0:
  *             self.resids2[t-1] = resids[t-1] * resids[t-1]
  */
   __pyx_t_1 = 0;
-  __pyx_v_omega = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_1)) )));
+  __pyx_v_omega = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_1)) )));
 
   /* "arch/univariate/recursions.pyx":842
  * 
  *         omega = parameters[0]
  *         if t > 0:             # <<<<<<<<<<<<<<
  *             self.resids2[t-1] = resids[t-1] * resids[t-1]
  * 
@@ -12328,15 +12335,15 @@
  * 
  *         sigma2[t] = omega
  */
     __pyx_t_1 = (__pyx_v_t - 1);
     __pyx_t_3 = (__pyx_v_t - 1);
     if (unlikely(!__pyx_v_self->resids2.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 843, __pyx_L1_error)}
     __pyx_t_4 = (__pyx_v_t - 1);
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->resids2.data) + __pyx_t_4)) )) = ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_1)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_3)) ))));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->resids2.data) + __pyx_t_4)) )) = ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_1)) ))) * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_3)) ))));
 
     /* "arch/univariate/recursions.pyx":842
  * 
  *         omega = parameters[0]
  *         if t > 0:             # <<<<<<<<<<<<<<
  *             self.resids2[t-1] = resids[t-1] * resids[t-1]
  * 
@@ -12386,15 +12393,15 @@
       __pyx_t_3 = __pyx_v_i;
       if (unlikely(!__pyx_v_self->gw.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 848, __pyx_L1_error)}
       __pyx_t_1 = __pyx_v_i;
       __pyx_t_4 = ((__pyx_v_t - __pyx_v_i) - 1);
       if (unlikely(!__pyx_v_self->resids2.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 848, __pyx_L1_error)}
       __pyx_t_8 = ((__pyx_v_t - __pyx_v_i) - 1);
       __pyx_t_9 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_9)) )) += (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->aw.data) + __pyx_t_3)) ))) + ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->gw.data) + __pyx_t_1)) ))) * ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_4)) ))) < 0.0))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->resids2.data) + __pyx_t_8)) ))));
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_9)) )) += (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->aw.data) + __pyx_t_3)) ))) + ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->gw.data) + __pyx_t_1)) ))) * ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_4)) ))) < 0.0))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->resids2.data) + __pyx_t_8)) ))));
 
       /* "arch/univariate/recursions.pyx":847
  *         sigma2[t] = omega
  *         for i in range(self.m):
  *             if (t - i - 1) >= 0:             # <<<<<<<<<<<<<<
  *                 sigma2[t] += (self.aw[i] + self.gw[i] * (resids[t - i - 1] < 0)) * self.resids2[t - i - 1]
  *             else:
@@ -12425,23 +12432,23 @@
  *             bounds_check(&sigma2[t], &var_bounds[t, 0])             # <<<<<<<<<<<<<<
  * 
  * cdef class FIGARCHUpdater(VolatilityUpdater):
  */
     __pyx_t_4 = __pyx_v_t;
     __pyx_t_8 = __pyx_v_t;
     __pyx_t_1 = 0;
-    __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) )))), (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_8 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_1)) )))));
+    __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_4)) )))), (&(*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_8 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_1)) )))));
   }
 
   /* "arch/univariate/recursions.pyx":830
  *             self.resids2 = np.empty(nobs)
  * 
  *     cdef void update(self,             # <<<<<<<<<<<<<<
  *                      Py_ssize_t t,
- *                      double[::1] parameters,
+ *                      const double[::1] parameters,
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("arch.univariate.recursions.MIDASUpdater.update", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
@@ -12967,15 +12974,15 @@
   __Pyx_RefNannySetupContext("__reduce__", 0);
 
   /* "arch/univariate/recursions.pyx":885
  * 
  *     def __reduce__(self):
  *         return FIGARCHUpdater, (self.p, self.q, self.power, self.truncation), (self.backcast, np.asarray(self.lam), np.asarray(self.fresids))             # <<<<<<<<<<<<<<
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->p); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 885, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->q); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 885, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = PyFloat_FromDouble(__pyx_v_self->power); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 885, __pyx_L1_error)
@@ -13096,15 +13103,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":887
  *         return FIGARCHUpdater, (self.p, self.q, self.power, self.truncation), (self.backcast, np.asarray(self.lam), np.asarray(self.fresids))
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         self.lam = _figarch_weights(parameters[1:], self.p, self.q, self.truncation)
  *         self.backcast = backcast
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_14FIGARCHUpdater_7initialize_update(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_14FIGARCHUpdater_7initialize_update = {"initialize_update", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_14FIGARCHUpdater_7initialize_update, METH_VARARGS|METH_KEYWORDS, 0};
@@ -13158,15 +13165,15 @@
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 887, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 887, __pyx_L3_error)
     __pyx_v_backcast = values[1];
     __pyx_v_nobs = __Pyx_PyIndex_AsSsize_t(values[2]); if (unlikely((__pyx_v_nobs == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 887, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("initialize_update", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 887, __pyx_L3_error)
   __pyx_L3_error:;
@@ -13196,15 +13203,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("initialize_update", 0);
 
   /* "arch/univariate/recursions.pyx":888
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
  *         self.lam = _figarch_weights(parameters[1:], self.p, self.q, self.truncation)             # <<<<<<<<<<<<<<
  *         self.backcast = backcast
  *         if self.fresids.shape[0] < nobs:
  */
   __pyx_t_1.data = __pyx_v_parameters.data;
   __pyx_t_1.memview = __pyx_v_parameters.memview;
   __PYX_INC_MEMVIEW(&__pyx_t_1, 0);
@@ -13232,15 +13239,15 @@
   __pyx_t_1.data = NULL;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->lam, 0);
   __pyx_v_self->lam = __pyx_t_3;
   __pyx_t_3.memview = NULL;
   __pyx_t_3.data = NULL;
 
   /* "arch/univariate/recursions.pyx":889
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
  *         self.lam = _figarch_weights(parameters[1:], self.p, self.q, self.truncation)
  *         self.backcast = backcast             # <<<<<<<<<<<<<<
  *         if self.fresids.shape[0] < nobs:
  *             self.fresids = np.empty(nobs)
  */
   __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_v_backcast); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 889, __pyx_L1_error)
   __pyx_v_self->backcast = __pyx_t_4;
@@ -13301,15 +13308,15 @@
  * 
  */
   }
 
   /* "arch/univariate/recursions.pyx":887
  *         return FIGARCHUpdater, (self.p, self.q, self.power, self.truncation), (self.backcast, np.asarray(self.lam), np.asarray(self.fresids))
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         self.lam = _figarch_weights(parameters[1:], self.p, self.q, self.truncation)
  *         self.backcast = backcast
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
@@ -13330,15 +13337,15 @@
 }
 
 /* "arch/univariate/recursions.pyx":893
  *             self.fresids = np.empty(nobs)
  * 
  *     cdef void update(self,             # <<<<<<<<<<<<<<
  *                      Py_ssize_t t,
- *                      double[::1] parameters,
+ *                      const double[::1] parameters,
  */
 
 static void __pyx_f_4arch_10univariate_10recursions_14FIGARCHUpdater_update(struct __pyx_obj_4arch_10univariate_10recursions_FIGARCHUpdater *__pyx_v_self, Py_ssize_t __pyx_v_t, __Pyx_memviewslice __pyx_v_parameters, __Pyx_memviewslice __pyx_v_resids, __Pyx_memviewslice __pyx_v_sigma2, __Pyx_memviewslice __pyx_v_var_bounds) {
   Py_ssize_t __pyx_v_i;
   double __pyx_v_bc_weight;
   double __pyx_v_omega;
   double __pyx_v_beta;
@@ -13380,26 +13387,26 @@
  *         cdef int p = self.p, q = self.q, trunc_lag = self.truncation
  * 
  *         omega = parameters[0]             # <<<<<<<<<<<<<<
  *         beta = parameters[1 + p + q] if q else 0.0
  *         omega_tilde = omega / (1 - beta)
  */
   __pyx_t_2 = 0;
-  __pyx_v_omega = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_2)) )));
+  __pyx_v_omega = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_2)) )));
 
   /* "arch/univariate/recursions.pyx":906
  * 
  *         omega = parameters[0]
  *         beta = parameters[1 + p + q] if q else 0.0             # <<<<<<<<<<<<<<
  *         omega_tilde = omega / (1 - beta)
  * 
  */
   if ((__pyx_v_q != 0)) {
     __pyx_t_2 = ((1 + __pyx_v_p) + __pyx_v_q);
-    __pyx_t_3 = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_2)) )));
+    __pyx_t_3 = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_2)) )));
   } else {
     __pyx_t_3 = 0.0;
   }
   __pyx_v_beta = __pyx_t_3;
 
   /* "arch/univariate/recursions.pyx":907
  *         omega = parameters[0]
@@ -13426,15 +13433,15 @@
  *             self.fresids[t-1] = fabs(resids[t-1]) ** self.power             # <<<<<<<<<<<<<<
  * 
  *         bc_weight = 0.0
  */
     __pyx_t_2 = (__pyx_v_t - 1);
     if (unlikely(!__pyx_v_self->fresids.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 910, __pyx_L1_error)}
     __pyx_t_5 = (__pyx_v_t - 1);
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->fresids.data) + __pyx_t_5)) )) = pow(fabs((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_2)) )))), __pyx_v_self->power);
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->fresids.data) + __pyx_t_5)) )) = pow(fabs((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_2)) )))), __pyx_v_self->power);
 
     /* "arch/univariate/recursions.pyx":909
  *         omega_tilde = omega / (1 - beta)
  * 
  *         if t > 0:             # <<<<<<<<<<<<<<
  *             self.fresids[t-1] = fabs(resids[t-1]) ** self.power
  * 
@@ -13524,22 +13531,22 @@
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_5 = __pyx_v_t;
   __pyx_t_2 = __pyx_v_t;
   __pyx_t_10 = 0;
-  __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) )))), (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_2 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_10)) )))));
+  __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_5)) )))), (&(*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_2 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_10)) )))));
 
   /* "arch/univariate/recursions.pyx":893
  *             self.fresids = np.empty(nobs)
  * 
  *     cdef void update(self,             # <<<<<<<<<<<<<<
  *                      Py_ssize_t t,
- *                      double[::1] parameters,
+ *                      const double[::1] parameters,
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("arch.univariate.recursions.FIGARCHUpdater.update", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
@@ -14405,15 +14412,15 @@
 }
 
 /* "arch/univariate/recursions.pyx":966
  *                 self.backcast[i] = backcast[i]
  * 
  *     cdef void update(self,             # <<<<<<<<<<<<<<
  *                      Py_ssize_t t,
- *                      double[::1] parameters,
+ *                      const double[::1] parameters,
  */
 
 static void __pyx_f_4arch_10univariate_10recursions_22RiskMetrics2006Updater_update(struct __pyx_obj_4arch_10univariate_10recursions_RiskMetrics2006Updater *__pyx_v_self, Py_ssize_t __pyx_v_t, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_parameters, __Pyx_memviewslice __pyx_v_resids, __Pyx_memviewslice __pyx_v_sigma2, __Pyx_memviewslice __pyx_v_var_bounds) {
   Py_ssize_t __pyx_v_i;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
@@ -14489,15 +14496,15 @@
  *             for i in range(self.kmax):
  *                 self.last_sigma2s[i] = ((1 - self.smoothing_parameters[i]) * resids[t - 1] ** 2 +             # <<<<<<<<<<<<<<
  *                                         self.smoothing_parameters[i] * self.last_sigma2s[i])
  *                 sigma2[t] += self.last_sigma2s[i] * self.combination_weights[i]
  */
       if (unlikely(!__pyx_v_self->last_sigma2s.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 979, __pyx_L1_error)}
       __pyx_t_9 = __pyx_v_i;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->last_sigma2s.data) + __pyx_t_9)) )) = (((1.0 - (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->smoothing_parameters.data) + __pyx_t_1)) )))) * pow((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_6)) ))), 2.0)) + ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->smoothing_parameters.data) + __pyx_t_7)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->last_sigma2s.data) + __pyx_t_8)) )))));
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->last_sigma2s.data) + __pyx_t_9)) )) = (((1.0 - (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->smoothing_parameters.data) + __pyx_t_1)) )))) * pow(((double)(*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_6)) )))), 2.0)) + ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->smoothing_parameters.data) + __pyx_t_7)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->last_sigma2s.data) + __pyx_t_8)) )))));
 
       /* "arch/univariate/recursions.pyx":981
  *                 self.last_sigma2s[i] = ((1 - self.smoothing_parameters[i]) * resids[t - 1] ** 2 +
  *                                         self.smoothing_parameters[i] * self.last_sigma2s[i])
  *                 sigma2[t] += self.last_sigma2s[i] * self.combination_weights[i]             # <<<<<<<<<<<<<<
  *         else:
  *             for i in range(self.kmax):
@@ -14569,22 +14576,22 @@
  *         bounds_check(&sigma2[t], &var_bounds[t, 0])             # <<<<<<<<<<<<<<
  * 
  * cdef class EGARCHUpdater(VolatilityUpdater):
  */
   __pyx_t_8 = __pyx_v_t;
   __pyx_t_7 = __pyx_v_t;
   __pyx_t_6 = 0;
-  __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_8)) )))), (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_7 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_6)) )))));
+  __pyx_f_4arch_10univariate_10recursions_bounds_check((&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_8)) )))), (&(*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_7 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_6)) )))));
 
   /* "arch/univariate/recursions.pyx":966
  *                 self.backcast[i] = backcast[i]
  * 
  *     cdef void update(self,             # <<<<<<<<<<<<<<
  *                      Py_ssize_t t,
- *                      double[::1] parameters,
+ *                      const double[::1] parameters,
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("arch.univariate.recursions.RiskMetrics2006Updater.update", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
@@ -15447,15 +15454,15 @@
     __pyx_t_6.data = NULL;
 
     /* "arch/univariate/recursions.pyx":1044
  *             self.lnsigma2 = np.empty(nobs)
  *             self.abs_std_resids = np.empty(nobs)
  *             self.std_resids = np.empty(nobs)             # <<<<<<<<<<<<<<
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
  */
     __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1044, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1044, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_nobs); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1044, __pyx_L1_error)
@@ -15512,15 +15519,15 @@
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
 /* "arch/univariate/recursions.pyx":1046
  *             self.std_resids = np.empty(nobs)
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         self.backcast = backcast
  *         self._resize(nobs)
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_13EGARCHUpdater_7initialize_update(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_13EGARCHUpdater_7initialize_update = {"initialize_update", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_13EGARCHUpdater_7initialize_update, METH_VARARGS|METH_KEYWORDS, 0};
@@ -15574,15 +15581,15 @@
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 1046, __pyx_L3_error)
+    __pyx_v_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_parameters.memview)) __PYX_ERR(0, 1046, __pyx_L3_error)
     __pyx_v_backcast = values[1];
     __pyx_v_nobs = __Pyx_PyIndex_AsSsize_t(values[2]); if (unlikely((__pyx_v_nobs == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1046, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("initialize_update", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1046, __pyx_L3_error)
   __pyx_L3_error:;
@@ -15604,35 +15611,35 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("initialize_update", 0);
 
   /* "arch/univariate/recursions.pyx":1047
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
  *         self.backcast = backcast             # <<<<<<<<<<<<<<
  *         self._resize(nobs)
  * 
  */
   __pyx_t_1 = __pyx_PyFloat_AsDouble(__pyx_v_backcast); if (unlikely((__pyx_t_1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1047, __pyx_L1_error)
   __pyx_v_self->backcast = __pyx_t_1;
 
   /* "arch/univariate/recursions.pyx":1048
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
  *         self.backcast = backcast
  *         self._resize(nobs)             # <<<<<<<<<<<<<<
  * 
  *     cdef void update(self,
  */
   ((struct __pyx_vtabstruct_4arch_10univariate_10recursions_EGARCHUpdater *)__pyx_v_self->__pyx_base.__pyx_vtab)->_resize(__pyx_v_self, __pyx_v_nobs);
 
   /* "arch/univariate/recursions.pyx":1046
  *             self.std_resids = np.empty(nobs)
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         self.backcast = backcast
  *         self._resize(nobs)
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
@@ -15647,15 +15654,15 @@
 }
 
 /* "arch/univariate/recursions.pyx":1050
  *         self._resize(nobs)
  * 
  *     cdef void update(self,             # <<<<<<<<<<<<<<
  *                      Py_ssize_t t,
- *                      double[::1] parameters,
+ *                      const double[::1] parameters,
  */
 
 static void __pyx_f_4arch_10univariate_10recursions_13EGARCHUpdater_update(struct __pyx_obj_4arch_10univariate_10recursions_EGARCHUpdater *__pyx_v_self, Py_ssize_t __pyx_v_t, __Pyx_memviewslice __pyx_v_parameters, __Pyx_memviewslice __pyx_v_resids, __Pyx_memviewslice __pyx_v_sigma2, __Pyx_memviewslice __pyx_v_var_bounds) {
   Py_ssize_t __pyx_v_j;
   Py_ssize_t __pyx_v_loc;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
@@ -15690,15 +15697,15 @@
  *             self.abs_std_resids[t-1] = fabs(self.std_resids[t-1])
  * 
  */
     __pyx_t_2 = (__pyx_v_t - 1);
     __pyx_t_3 = (__pyx_v_t - 1);
     if (unlikely(!__pyx_v_self->std_resids.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1060, __pyx_L1_error)}
     __pyx_t_4 = (__pyx_v_t - 1);
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->std_resids.data) + __pyx_t_4)) )) = ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_2)) ))) / sqrt((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_3)) )))));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->std_resids.data) + __pyx_t_4)) )) = (((double)(*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_resids.data) + __pyx_t_2)) )))) / sqrt((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_3)) )))));
 
     /* "arch/univariate/recursions.pyx":1061
  *         if t > 0:
  *             self.std_resids[t-1] = resids[t-1] / sqrt(sigma2[t-1])
  *             self.abs_std_resids[t-1] = fabs(self.std_resids[t-1])             # <<<<<<<<<<<<<<
  * 
  *         self.lnsigma2[t] = parameters[0]
@@ -15724,15 +15731,15 @@
  *         self.lnsigma2[t] = parameters[0]             # <<<<<<<<<<<<<<
  *         loc = 1
  *         for j in range(self.p):
  */
   __pyx_t_3 = 0;
   if (unlikely(!__pyx_v_self->lnsigma2.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1063, __pyx_L1_error)}
   __pyx_t_2 = __pyx_v_t;
-  *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->lnsigma2.data) + __pyx_t_2)) )) = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_3)) )));
+  *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->lnsigma2.data) + __pyx_t_2)) )) = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_3)) )));
 
   /* "arch/univariate/recursions.pyx":1064
  * 
  *         self.lnsigma2[t] = parameters[0]
  *         loc = 1             # <<<<<<<<<<<<<<
  *         for j in range(self.p):
  *             if (t - 1 - j) >= 0:
@@ -15769,15 +15776,15 @@
  *         for j in range(self.o):
  */
       __pyx_t_3 = __pyx_v_loc;
       if (unlikely(!__pyx_v_self->abs_std_resids.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1067, __pyx_L1_error)}
       __pyx_t_2 = ((__pyx_v_t - 1) - __pyx_v_j);
       if (unlikely(!__pyx_v_self->lnsigma2.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1067, __pyx_L1_error)}
       __pyx_t_4 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->lnsigma2.data) + __pyx_t_4)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_3)) ))) * ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->abs_std_resids.data) + __pyx_t_2)) ))) - 0.7978845608028654));
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->lnsigma2.data) + __pyx_t_4)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_3)) ))) * ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->abs_std_resids.data) + __pyx_t_2)) ))) - 0.7978845608028654));
 
       /* "arch/univariate/recursions.pyx":1066
  *         loc = 1
  *         for j in range(self.p):
  *             if (t - 1 - j) >= 0:             # <<<<<<<<<<<<<<
  *                 self.lnsigma2[t] += parameters[loc] * (self.abs_std_resids[t - 1 - j] - SQRT2_OV_PI)
  *             loc += 1
@@ -15824,15 +15831,15 @@
  *         for j in range(self.q):
  */
       __pyx_t_2 = __pyx_v_loc;
       if (unlikely(!__pyx_v_self->std_resids.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1071, __pyx_L1_error)}
       __pyx_t_3 = ((__pyx_v_t - 1) - __pyx_v_j);
       if (unlikely(!__pyx_v_self->lnsigma2.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1071, __pyx_L1_error)}
       __pyx_t_4 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->lnsigma2.data) + __pyx_t_4)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_2)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->std_resids.data) + __pyx_t_3)) ))));
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->lnsigma2.data) + __pyx_t_4)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_2)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->std_resids.data) + __pyx_t_3)) ))));
 
       /* "arch/univariate/recursions.pyx":1070
  *             loc += 1
  *         for j in range(self.o):
  *             if (t - 1 - j) >= 0:             # <<<<<<<<<<<<<<
  *                 self.lnsigma2[t] += parameters[loc] * self.std_resids[t - 1 - j]
  *             loc += 1
@@ -15877,15 +15884,15 @@
  *                 self.lnsigma2[t] += parameters[loc] * self.backcast             # <<<<<<<<<<<<<<
  *             else:
  *                 self.lnsigma2[t] += parameters[loc] * self.lnsigma2[t - 1 - j]
  */
       __pyx_t_3 = __pyx_v_loc;
       if (unlikely(!__pyx_v_self->lnsigma2.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1075, __pyx_L1_error)}
       __pyx_t_2 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->lnsigma2.data) + __pyx_t_2)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_3)) ))) * __pyx_v_self->backcast);
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->lnsigma2.data) + __pyx_t_2)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_3)) ))) * __pyx_v_self->backcast);
 
       /* "arch/univariate/recursions.pyx":1074
  *             loc += 1
  *         for j in range(self.q):
  *             if (t - 1 - j) < 0:             # <<<<<<<<<<<<<<
  *                 self.lnsigma2[t] += parameters[loc] * self.backcast
  *             else:
@@ -15902,15 +15909,15 @@
  */
     /*else*/ {
       __pyx_t_3 = __pyx_v_loc;
       if (unlikely(!__pyx_v_self->lnsigma2.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1077, __pyx_L1_error)}
       __pyx_t_2 = ((__pyx_v_t - 1) - __pyx_v_j);
       if (unlikely(!__pyx_v_self->lnsigma2.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1077, __pyx_L1_error)}
       __pyx_t_4 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->lnsigma2.data) + __pyx_t_4)) )) += ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_parameters.data) + __pyx_t_3)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->lnsigma2.data) + __pyx_t_2)) ))));
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->lnsigma2.data) + __pyx_t_4)) )) += ((*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_parameters.data) + __pyx_t_3)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->lnsigma2.data) + __pyx_t_2)) ))));
     }
     __pyx_L12:;
 
     /* "arch/univariate/recursions.pyx":1078
  *             else:
  *                 self.lnsigma2[t] += parameters[loc] * self.lnsigma2[t - 1 - j]
  *             loc += 1             # <<<<<<<<<<<<<<
@@ -15970,28 +15977,28 @@
  *         if sigma2[t] < var_bounds[t, 0]:             # <<<<<<<<<<<<<<
  *             sigma2[t] = var_bounds[t, 0]
  *             self.lnsigma2[t] = log(sigma2[t])
  */
   __pyx_t_2 = __pyx_v_t;
   __pyx_t_3 = __pyx_v_t;
   __pyx_t_4 = 0;
-  __pyx_t_1 = (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_2)) ))) < (*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_3 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_4)) )))) != 0);
+  __pyx_t_1 = (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_2)) ))) < (*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_3 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_4)) )))) != 0);
   if (__pyx_t_1) {
 
     /* "arch/univariate/recursions.pyx":1083
  *         sigma2[t] = exp(self.lnsigma2[t])
  *         if sigma2[t] < var_bounds[t, 0]:
  *             sigma2[t] = var_bounds[t, 0]             # <<<<<<<<<<<<<<
  *             self.lnsigma2[t] = log(sigma2[t])
  *         elif sigma2[t] > var_bounds[t, 1]:
  */
     __pyx_t_4 = __pyx_v_t;
     __pyx_t_3 = 0;
     __pyx_t_2 = __pyx_v_t;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_2)) )) = (*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_4 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_3)) )));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_2)) )) = (*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_4 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_3)) )));
 
     /* "arch/univariate/recursions.pyx":1084
  *         if sigma2[t] < var_bounds[t, 0]:
  *             sigma2[t] = var_bounds[t, 0]
  *             self.lnsigma2[t] = log(sigma2[t])             # <<<<<<<<<<<<<<
  *         elif sigma2[t] > var_bounds[t, 1]:
  *             sigma2[t] = var_bounds[t, 1] + log(sigma2[t]) - log(var_bounds[t, 1])
@@ -16017,15 +16024,15 @@
  *         elif sigma2[t] > var_bounds[t, 1]:             # <<<<<<<<<<<<<<
  *             sigma2[t] = var_bounds[t, 1] + log(sigma2[t]) - log(var_bounds[t, 1])
  *             self.lnsigma2[t] = log(sigma2[t])
  */
   __pyx_t_3 = __pyx_v_t;
   __pyx_t_4 = __pyx_v_t;
   __pyx_t_2 = 1;
-  __pyx_t_1 = (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_3)) ))) > (*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_4 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_2)) )))) != 0);
+  __pyx_t_1 = (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_3)) ))) > (*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_4 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_2)) )))) != 0);
   if (__pyx_t_1) {
 
     /* "arch/univariate/recursions.pyx":1086
  *             self.lnsigma2[t] = log(sigma2[t])
  *         elif sigma2[t] > var_bounds[t, 1]:
  *             sigma2[t] = var_bounds[t, 1] + log(sigma2[t]) - log(var_bounds[t, 1])             # <<<<<<<<<<<<<<
  *             self.lnsigma2[t] = log(sigma2[t])
@@ -16033,15 +16040,15 @@
  */
     __pyx_t_2 = __pyx_v_t;
     __pyx_t_4 = 1;
     __pyx_t_3 = __pyx_v_t;
     __pyx_t_8 = __pyx_v_t;
     __pyx_t_9 = 1;
     __pyx_t_10 = __pyx_v_t;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_10)) )) = (((*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_2 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_4)) ))) + log((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_3)) ))))) - log((*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_8 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_9)) )))));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_10)) )) = (((*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_2 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_4)) ))) + log((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_sigma2.data) + __pyx_t_3)) ))))) - log((*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_var_bounds.data + __pyx_t_8 * __pyx_v_var_bounds.strides[0]) )) + __pyx_t_9)) )))));
 
     /* "arch/univariate/recursions.pyx":1087
  *         elif sigma2[t] > var_bounds[t, 1]:
  *             sigma2[t] = var_bounds[t, 1] + log(sigma2[t]) - log(var_bounds[t, 1])
  *             self.lnsigma2[t] = log(sigma2[t])             # <<<<<<<<<<<<<<
  * 
  * 
@@ -16062,15 +16069,15 @@
   __pyx_L14:;
 
   /* "arch/univariate/recursions.pyx":1050
  *         self._resize(nobs)
  * 
  *     cdef void update(self,             # <<<<<<<<<<<<<<
  *                      Py_ssize_t t,
- *                      double[::1] parameters,
+ *                      const double[::1] parameters,
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("arch.univariate.recursions.EGARCHUpdater.update", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
@@ -16175,16 +16182,16 @@
   return __pyx_r;
 }
 
 /* "arch/univariate/recursions.pyx":1097
  *         self.volatility_updater = updater
  * 
  *     def recursion(self,             # <<<<<<<<<<<<<<
- *                   double[::1] y,
- *                   double[:,::1] x,
+ *                   const double[::1] y,
+ *                   const double[:,::1] x,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_19ARCHInMeanRecursion_3recursion(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_4arch_10univariate_10recursions_19ARCHInMeanRecursion_3recursion = {"recursion", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4arch_10univariate_10recursions_19ARCHInMeanRecursion_3recursion, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_4arch_10univariate_10recursions_19ARCHInMeanRecursion_3recursion(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_y = { 0, 0, { 0 }, { 0 }, { 0 } };
@@ -16276,20 +16283,20 @@
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
     }
-    __pyx_v_y = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_y.memview)) __PYX_ERR(0, 1098, __pyx_L3_error)
-    __pyx_v_x = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_x.memview)) __PYX_ERR(0, 1099, __pyx_L3_error)
-    __pyx_v_mean_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_mean_parameters.memview)) __PYX_ERR(0, 1100, __pyx_L3_error)
-    __pyx_v_variance_params = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_variance_params.memview)) __PYX_ERR(0, 1101, __pyx_L3_error)
+    __pyx_v_y = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_y.memview)) __PYX_ERR(0, 1098, __pyx_L3_error)
+    __pyx_v_x = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double__const__(values[1], 0); if (unlikely(!__pyx_v_x.memview)) __PYX_ERR(0, 1099, __pyx_L3_error)
+    __pyx_v_mean_parameters = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[2], 0); if (unlikely(!__pyx_v_mean_parameters.memview)) __PYX_ERR(0, 1100, __pyx_L3_error)
+    __pyx_v_variance_params = __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(values[3], 0); if (unlikely(!__pyx_v_variance_params.memview)) __PYX_ERR(0, 1101, __pyx_L3_error)
     __pyx_v_sigma2 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sigma2.memview)) __PYX_ERR(0, 1102, __pyx_L3_error)
-    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 1103, __pyx_L3_error)
+    __pyx_v_var_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double__const__(values[5], 0); if (unlikely(!__pyx_v_var_bounds.memview)) __PYX_ERR(0, 1103, __pyx_L3_error)
     __pyx_v_power = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_power == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1104, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("recursion", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1097, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("arch.univariate.recursions.ARCHInMeanRecursion.recursion", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -16383,15 +16390,15 @@
  *             Py_ssize_t t, i, nobs = y.shape[0], k = x.shape[1]
  *             double[::1] resids = np.empty(nobs)
  *             double gamma = mean_parameters[k]             # <<<<<<<<<<<<<<
  * 
  *         for t in range(nobs):
  */
   __pyx_t_6 = __pyx_v_k;
-  __pyx_v_gamma = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_mean_parameters.data) + __pyx_t_6)) )));
+  __pyx_v_gamma = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_mean_parameters.data) + __pyx_t_6)) )));
 
   /* "arch/univariate/recursions.pyx":1110
  *             double gamma = mean_parameters[k]
  * 
  *         for t in range(nobs):             # <<<<<<<<<<<<<<
  *             self.volatility_updater.update(t, variance_params, resids, sigma2, var_bounds)
  *             resids[t] = y[t]
@@ -16415,15 +16422,15 @@
  *             self.volatility_updater.update(t, variance_params, resids, sigma2, var_bounds)
  *             resids[t] = y[t]             # <<<<<<<<<<<<<<
  *             for i in range(k):
  *                 resids[t] -= x[t,i] * mean_parameters[i]
  */
     __pyx_t_6 = __pyx_v_t;
     __pyx_t_10 = __pyx_v_t;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_10)) )) = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_y.data) + __pyx_t_6)) )));
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_10)) )) = (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_y.data) + __pyx_t_6)) )));
 
     /* "arch/univariate/recursions.pyx":1113
  *             self.volatility_updater.update(t, variance_params, resids, sigma2, var_bounds)
  *             resids[t] = y[t]
  *             for i in range(k):             # <<<<<<<<<<<<<<
  *                 resids[t] -= x[t,i] * mean_parameters[i]
  *             if power == 0.0:
@@ -16440,15 +16447,15 @@
  *             if power == 0.0:
  *                 resids[t] -= gamma * log(sigma2[t])
  */
       __pyx_t_6 = __pyx_v_t;
       __pyx_t_10 = __pyx_v_i;
       __pyx_t_14 = __pyx_v_i;
       __pyx_t_15 = __pyx_v_t;
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_15)) )) -= ((*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_x.data + __pyx_t_6 * __pyx_v_x.strides[0]) )) + __pyx_t_10)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_mean_parameters.data) + __pyx_t_14)) ))));
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_resids.data) + __pyx_t_15)) )) -= ((*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_x.data + __pyx_t_6 * __pyx_v_x.strides[0]) )) + __pyx_t_10)) ))) * (*((double const  *) ( /* dim=0 */ ((char *) (((double const  *) __pyx_v_mean_parameters.data) + __pyx_t_14)) ))));
     }
 
     /* "arch/univariate/recursions.pyx":1115
  *             for i in range(k):
  *                 resids[t] -= x[t,i] * mean_parameters[i]
  *             if power == 0.0:             # <<<<<<<<<<<<<<
  *                 resids[t] -= gamma * log(sigma2[t])
@@ -16526,16 +16533,16 @@
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "arch/univariate/recursions.pyx":1097
  *         self.volatility_updater = updater
  * 
  *     def recursion(self,             # <<<<<<<<<<<<<<
- *                   double[::1] y,
- *                   double[:,::1] x,
+ *                   const double[::1] y,
+ *                   const double[:,::1] x,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -18038,15 +18045,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
  *         # experimental exception made for __getbuffer__ and __releasebuffer__
  *         # -- the details of this may change.
  *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
  *             # This implementation of getbuffer is geared towards Cython
  *             # requirements, and does not yet fulfill the PEP.
  */
 
@@ -18090,344 +18097,344 @@
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":265
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":265
  * 
  *             cdef int i, ndim
  *             cdef int endian_detector = 1             # <<<<<<<<<<<<<<
  *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
  * 
  */
   __pyx_v_endian_detector = 1;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":266
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":266
  *             cdef int i, ndim
  *             cdef int endian_detector = 1
  *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
  * 
  *             ndim = PyArray_NDIM(self)
  */
   __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":268
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":268
  *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
  * 
  *             ndim = PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  */
   __pyx_v_ndim = PyArray_NDIM(__pyx_v_self);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
  *             ndim = PyArray_NDIM(self)
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")
  */
   __pyx_t_2 = (((__pyx_v_flags & PyBUF_C_CONTIGUOUS) == PyBUF_C_CONTIGUOUS) != 0);
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L4_bool_binop_done;
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":271
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":271
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):             # <<<<<<<<<<<<<<
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  */
   __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_C_CONTIGUOUS) != 0)) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
  *             ndim = PyArray_NDIM(self)
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")
  */
   if (unlikely(__pyx_t_1)) {
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  */
     __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 272, __pyx_L1_error)
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
  *             ndim = PyArray_NDIM(self)
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")
  */
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  */
   __pyx_t_2 = (((__pyx_v_flags & PyBUF_F_CONTIGUOUS) == PyBUF_F_CONTIGUOUS) != 0);
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L7_bool_binop_done;
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":275
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":275
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):             # <<<<<<<<<<<<<<
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  * 
  */
   __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_F_CONTIGUOUS) != 0)) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L7_bool_binop_done:;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  */
   if (unlikely(__pyx_t_1)) {
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
  * 
  *             info.buf = PyArray_DATA(self)
  */
     __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 276, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 276, __pyx_L1_error)
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  */
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":278
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":278
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  * 
  *             info.buf = PyArray_DATA(self)             # <<<<<<<<<<<<<<
  *             info.ndim = ndim
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  */
   __pyx_v_info->buf = PyArray_DATA(__pyx_v_self);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":279
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":279
  * 
  *             info.buf = PyArray_DATA(self)
  *             info.ndim = ndim             # <<<<<<<<<<<<<<
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  *                 # Allocate new buffer for strides and shape info.
  */
   __pyx_v_info->ndim = __pyx_v_ndim;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
  *             info.buf = PyArray_DATA(self)
  *             info.ndim = ndim
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 # Allocate new buffer for strides and shape info.
  *                 # This is allocated as one block, strides first.
  */
   __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":283
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":283
  *                 # Allocate new buffer for strides and shape info.
  *                 # This is allocated as one block, strides first.
  *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)             # <<<<<<<<<<<<<<
  *                 info.shape = info.strides + ndim
  *                 for i in range(ndim):
  */
     __pyx_v_info->strides = ((Py_ssize_t *)PyObject_Malloc((((sizeof(Py_ssize_t)) * 2) * ((size_t)__pyx_v_ndim))));
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":284
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":284
  *                 # This is allocated as one block, strides first.
  *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
  *                 info.shape = info.strides + ndim             # <<<<<<<<<<<<<<
  *                 for i in range(ndim):
  *                     info.strides[i] = PyArray_STRIDES(self)[i]
  */
     __pyx_v_info->shape = (__pyx_v_info->strides + __pyx_v_ndim);
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":285
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":285
  *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
  *                 info.shape = info.strides + ndim
  *                 for i in range(ndim):             # <<<<<<<<<<<<<<
  *                     info.strides[i] = PyArray_STRIDES(self)[i]
  *                     info.shape[i] = PyArray_DIMS(self)[i]
  */
     __pyx_t_4 = __pyx_v_ndim;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":286
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":286
  *                 info.shape = info.strides + ndim
  *                 for i in range(ndim):
  *                     info.strides[i] = PyArray_STRIDES(self)[i]             # <<<<<<<<<<<<<<
  *                     info.shape[i] = PyArray_DIMS(self)[i]
  *             else:
  */
       (__pyx_v_info->strides[__pyx_v_i]) = (PyArray_STRIDES(__pyx_v_self)[__pyx_v_i]);
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":287
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":287
  *                 for i in range(ndim):
  *                     info.strides[i] = PyArray_STRIDES(self)[i]
  *                     info.shape[i] = PyArray_DIMS(self)[i]             # <<<<<<<<<<<<<<
  *             else:
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
  */
       (__pyx_v_info->shape[__pyx_v_i]) = (PyArray_DIMS(__pyx_v_self)[__pyx_v_i]);
     }
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
  *             info.buf = PyArray_DATA(self)
  *             info.ndim = ndim
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 # Allocate new buffer for strides and shape info.
  *                 # This is allocated as one block, strides first.
  */
     goto __pyx_L9;
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":289
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":289
  *                     info.shape[i] = PyArray_DIMS(self)[i]
  *             else:
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
  *             info.suboffsets = NULL
  */
   /*else*/ {
     __pyx_v_info->strides = ((Py_ssize_t *)PyArray_STRIDES(__pyx_v_self));
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":290
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":290
  *             else:
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  *             info.suboffsets = NULL
  *             info.itemsize = PyArray_ITEMSIZE(self)
  */
     __pyx_v_info->shape = ((Py_ssize_t *)PyArray_DIMS(__pyx_v_self));
   }
   __pyx_L9:;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":291
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":291
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
  *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
  *             info.itemsize = PyArray_ITEMSIZE(self)
  *             info.readonly = not PyArray_ISWRITEABLE(self)
  */
   __pyx_v_info->suboffsets = NULL;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":292
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":292
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
  *             info.suboffsets = NULL
  *             info.itemsize = PyArray_ITEMSIZE(self)             # <<<<<<<<<<<<<<
  *             info.readonly = not PyArray_ISWRITEABLE(self)
  * 
  */
   __pyx_v_info->itemsize = PyArray_ITEMSIZE(__pyx_v_self);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":293
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":293
  *             info.suboffsets = NULL
  *             info.itemsize = PyArray_ITEMSIZE(self)
  *             info.readonly = not PyArray_ISWRITEABLE(self)             # <<<<<<<<<<<<<<
  * 
  *             cdef int t
  */
   __pyx_v_info->readonly = (!(PyArray_ISWRITEABLE(__pyx_v_self) != 0));
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":296
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":296
  * 
  *             cdef int t
  *             cdef char* f = NULL             # <<<<<<<<<<<<<<
  *             cdef dtype descr = <dtype>PyArray_DESCR(self)
  *             cdef int offset
  */
   __pyx_v_f = NULL;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":297
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":297
  *             cdef int t
  *             cdef char* f = NULL
  *             cdef dtype descr = <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  *             cdef int offset
  * 
  */
   __pyx_t_7 = PyArray_DESCR(__pyx_v_self);
   __pyx_t_3 = ((PyObject *)__pyx_t_7);
   __Pyx_INCREF(__pyx_t_3);
   __pyx_v_descr = ((PyArray_Descr *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":300
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":300
  *             cdef int offset
  * 
  *             info.obj = self             # <<<<<<<<<<<<<<
  * 
  *             if not PyDataType_HASFIELDS(descr):
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   __Pyx_GOTREF(__pyx_v_info->obj);
   __Pyx_DECREF(__pyx_v_info->obj);
   __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
  *             info.obj = self
  * 
  *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or
  */
   __pyx_t_1 = ((!(PyDataType_HASFIELDS(__pyx_v_descr) != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":303
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":303
  * 
  *             if not PyDataType_HASFIELDS(descr):
  *                 t = descr.type_num             # <<<<<<<<<<<<<<
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):
  */
     __pyx_t_4 = __pyx_v_descr->type_num;
     __pyx_v_t = __pyx_t_4;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
  *             if not PyDataType_HASFIELDS(descr):
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  */
     __pyx_t_2 = ((__pyx_v_descr->byteorder == '>') != 0);
@@ -18439,15 +18446,15 @@
     if (!__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L14_bool_binop_done;
     }
     __pyx_L15_next_or:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":305
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":305
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
  *                     raise ValueError(u"Non-native byte order not supported")
  *                 if   t == NPY_BYTE:        f = "b"
  */
     __pyx_t_2 = ((__pyx_v_descr->byteorder == '<') != 0);
@@ -18456,235 +18463,235 @@
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L14_bool_binop_done;
     }
     __pyx_t_2 = ((!(__pyx_v_little_endian != 0)) != 0);
     __pyx_t_1 = __pyx_t_2;
     __pyx_L14_bool_binop_done:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
  *             if not PyDataType_HASFIELDS(descr):
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  */
     if (unlikely(__pyx_t_1)) {
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"
  */
       __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 306, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(2, 306, __pyx_L1_error)
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
  *             if not PyDataType_HASFIELDS(descr):
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  */
     }
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":307
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":307
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  *                 if   t == NPY_BYTE:        f = "b"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_UBYTE:       f = "B"
  *                 elif t == NPY_SHORT:       f = "h"
  */
     switch (__pyx_v_t) {
       case NPY_BYTE:
       __pyx_v_f = ((char *)"b");
       break;
       case NPY_UBYTE:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":308
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":308
  *                     raise ValueError(u"Non-native byte order not supported")
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_SHORT:       f = "h"
  *                 elif t == NPY_USHORT:      f = "H"
  */
       __pyx_v_f = ((char *)"B");
       break;
       case NPY_SHORT:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":309
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":309
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"
  *                 elif t == NPY_SHORT:       f = "h"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_USHORT:      f = "H"
  *                 elif t == NPY_INT:         f = "i"
  */
       __pyx_v_f = ((char *)"h");
       break;
       case NPY_USHORT:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":310
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":310
  *                 elif t == NPY_UBYTE:       f = "B"
  *                 elif t == NPY_SHORT:       f = "h"
  *                 elif t == NPY_USHORT:      f = "H"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_INT:         f = "i"
  *                 elif t == NPY_UINT:        f = "I"
  */
       __pyx_v_f = ((char *)"H");
       break;
       case NPY_INT:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":311
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":311
  *                 elif t == NPY_SHORT:       f = "h"
  *                 elif t == NPY_USHORT:      f = "H"
  *                 elif t == NPY_INT:         f = "i"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_UINT:        f = "I"
  *                 elif t == NPY_LONG:        f = "l"
  */
       __pyx_v_f = ((char *)"i");
       break;
       case NPY_UINT:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":312
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":312
  *                 elif t == NPY_USHORT:      f = "H"
  *                 elif t == NPY_INT:         f = "i"
  *                 elif t == NPY_UINT:        f = "I"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_LONG:        f = "l"
  *                 elif t == NPY_ULONG:       f = "L"
  */
       __pyx_v_f = ((char *)"I");
       break;
       case NPY_LONG:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":313
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":313
  *                 elif t == NPY_INT:         f = "i"
  *                 elif t == NPY_UINT:        f = "I"
  *                 elif t == NPY_LONG:        f = "l"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_ULONG:       f = "L"
  *                 elif t == NPY_LONGLONG:    f = "q"
  */
       __pyx_v_f = ((char *)"l");
       break;
       case NPY_ULONG:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":314
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":314
  *                 elif t == NPY_UINT:        f = "I"
  *                 elif t == NPY_LONG:        f = "l"
  *                 elif t == NPY_ULONG:       f = "L"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_LONGLONG:    f = "q"
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  */
       __pyx_v_f = ((char *)"L");
       break;
       case NPY_LONGLONG:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":315
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":315
  *                 elif t == NPY_LONG:        f = "l"
  *                 elif t == NPY_ULONG:       f = "L"
  *                 elif t == NPY_LONGLONG:    f = "q"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  *                 elif t == NPY_FLOAT:       f = "f"
  */
       __pyx_v_f = ((char *)"q");
       break;
       case NPY_ULONGLONG:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":316
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":316
  *                 elif t == NPY_ULONG:       f = "L"
  *                 elif t == NPY_LONGLONG:    f = "q"
  *                 elif t == NPY_ULONGLONG:   f = "Q"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_FLOAT:       f = "f"
  *                 elif t == NPY_DOUBLE:      f = "d"
  */
       __pyx_v_f = ((char *)"Q");
       break;
       case NPY_FLOAT:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":317
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":317
  *                 elif t == NPY_LONGLONG:    f = "q"
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  *                 elif t == NPY_FLOAT:       f = "f"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_DOUBLE:      f = "d"
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  */
       __pyx_v_f = ((char *)"f");
       break;
       case NPY_DOUBLE:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":318
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":318
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  *                 elif t == NPY_FLOAT:       f = "f"
  *                 elif t == NPY_DOUBLE:      f = "d"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  */
       __pyx_v_f = ((char *)"d");
       break;
       case NPY_LONGDOUBLE:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":319
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":319
  *                 elif t == NPY_FLOAT:       f = "f"
  *                 elif t == NPY_DOUBLE:      f = "d"
  *                 elif t == NPY_LONGDOUBLE:  f = "g"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  */
       __pyx_v_f = ((char *)"g");
       break;
       case NPY_CFLOAT:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":320
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":320
  *                 elif t == NPY_DOUBLE:      f = "d"
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  *                 elif t == NPY_CFLOAT:      f = "Zf"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
  */
       __pyx_v_f = ((char *)"Zf");
       break;
       case NPY_CDOUBLE:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":321
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":321
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  *                 elif t == NPY_CDOUBLE:     f = "Zd"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
  *                 elif t == NPY_OBJECT:      f = "O"
  */
       __pyx_v_f = ((char *)"Zd");
       break;
       case NPY_CLONGDOUBLE:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":322
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":322
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_OBJECT:      f = "O"
  *                 else:
  */
       __pyx_v_f = ((char *)"Zg");
       break;
       case NPY_OBJECT:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":323
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":323
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
  *                 elif t == NPY_OBJECT:      f = "O"             # <<<<<<<<<<<<<<
  *                 else:
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  */
       __pyx_v_f = ((char *)"O");
       break;
       default:
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":325
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":325
  *                 elif t == NPY_OBJECT:      f = "O"
  *                 else:
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
  *                 info.format = f
  *                 return
  */
       __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 325, __pyx_L1_error)
@@ -18697,91 +18704,91 @@
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(2, 325, __pyx_L1_error)
       break;
     }
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":326
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":326
  *                 else:
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  *                 info.format = f             # <<<<<<<<<<<<<<
  *                 return
  *             else:
  */
     __pyx_v_info->format = __pyx_v_f;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":327
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":327
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  *                 info.format = f
  *                 return             # <<<<<<<<<<<<<<
  *             else:
  *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
  *             info.obj = self
  * 
  *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or
  */
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":329
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":329
  *                 return
  *             else:
  *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)             # <<<<<<<<<<<<<<
  *                 info.format[0] = c'^' # Native data types, manual alignment
  *                 offset = 0
  */
   /*else*/ {
     __pyx_v_info->format = ((char *)PyObject_Malloc(0xFF));
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":330
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":330
  *             else:
  *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
  *                 info.format[0] = c'^' # Native data types, manual alignment             # <<<<<<<<<<<<<<
  *                 offset = 0
  *                 f = _util_dtypestring(descr, info.format + 1,
  */
     (__pyx_v_info->format[0]) = '^';
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":331
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":331
  *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
  *                 info.format[0] = c'^' # Native data types, manual alignment
  *                 offset = 0             # <<<<<<<<<<<<<<
  *                 f = _util_dtypestring(descr, info.format + 1,
  *                                       info.format + _buffer_format_string_len,
  */
     __pyx_v_offset = 0;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":332
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":332
  *                 info.format[0] = c'^' # Native data types, manual alignment
  *                 offset = 0
  *                 f = _util_dtypestring(descr, info.format + 1,             # <<<<<<<<<<<<<<
  *                                       info.format + _buffer_format_string_len,
  *                                       &offset)
  */
     __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_descr, (__pyx_v_info->format + 1), (__pyx_v_info->format + 0xFF), (&__pyx_v_offset)); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(2, 332, __pyx_L1_error)
     __pyx_v_f = __pyx_t_9;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":335
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":335
  *                                       info.format + _buffer_format_string_len,
  *                                       &offset)
  *                 f[0] = c'\0' # Terminate format string             # <<<<<<<<<<<<<<
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  */
     (__pyx_v_f[0]) = '\x00';
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
  *         # experimental exception made for __getbuffer__ and __releasebuffer__
  *         # -- the details of this may change.
  *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
  *             # This implementation of getbuffer is geared towards Cython
  *             # requirements, and does not yet fulfill the PEP.
  */
 
@@ -18805,15 +18812,15 @@
   }
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_descr);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
  *                 f[0] = c'\0' # Terminate format string
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)
  */
 
@@ -18829,83 +18836,83 @@
 }
 
 static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__releasebuffer__", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  */
   __pyx_t_1 = (PyArray_HASFIELDS(__pyx_v_self) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":339
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":339
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)             # <<<<<<<<<<<<<<
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  *                 PyObject_Free(info.strides)
  */
     PyObject_Free(__pyx_v_info->format);
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  */
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 PyObject_Free(info.strides)
  *                 # info.shape was stored after info.strides in the same block
  */
   __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":341
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":341
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  *                 PyObject_Free(info.strides)             # <<<<<<<<<<<<<<
  *                 # info.shape was stored after info.strides in the same block
  * 
  */
     PyObject_Free(__pyx_v_info->strides);
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 PyObject_Free(info.strides)
  *                 # info.shape was stored after info.strides in the same block
  */
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
  *                 f[0] = c'\0' # Terminate format string
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":820
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":820
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18914,29 +18921,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":821
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":821
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 821, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":820
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":820
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18947,15 +18954,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":823
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":823
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18964,29 +18971,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":824
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":824
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 824, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":823
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":823
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18997,15 +19004,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":826
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":826
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19014,29 +19021,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":827
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":827
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":826
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":826
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19047,15 +19054,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":829
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":829
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19064,29 +19071,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":830
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":830
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 830, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":829
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":829
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19097,15 +19104,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":832
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":832
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19114,29 +19121,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":833
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":833
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 833, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":832
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":832
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19147,89 +19154,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":835
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":835
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":837
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":837
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":839
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":839
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":835
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":835
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":841
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":841
  *         return ()
  * 
  * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
  *     # Recursive utility function used in __getbuffer__ to get format
  *     # string. The new location in the format string is returned.
  */
 
@@ -19253,33 +19260,33 @@
   long __pyx_t_8;
   char *__pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_util_dtypestring", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":846
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":846
  * 
  *     cdef dtype child
  *     cdef int endian_detector = 1             # <<<<<<<<<<<<<<
  *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
  *     cdef tuple fields
  */
   __pyx_v_endian_detector = 1;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":847
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":847
  *     cdef dtype child
  *     cdef int endian_detector = 1
  *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
  *     cdef tuple fields
  * 
  */
   __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":850
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":850
  *     cdef tuple fields
  * 
  *     for childname in descr.names:             # <<<<<<<<<<<<<<
  *         fields = descr.fields[childname]
  *         child, new_offset = fields
  */
   if (unlikely(__pyx_v_descr->names == Py_None)) {
@@ -19294,15 +19301,15 @@
     #else
     __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 850, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_childname, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":851
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":851
  * 
  *     for childname in descr.names:
  *         fields = descr.fields[childname]             # <<<<<<<<<<<<<<
  *         child, new_offset = fields
  * 
  */
     if (unlikely(__pyx_v_descr->fields == Py_None)) {
@@ -19311,15 +19318,15 @@
     }
     __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_descr->fields, __pyx_v_childname); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 851, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (!(likely(PyTuple_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(2, 851, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_fields, ((PyObject*)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":852
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":852
  *     for childname in descr.names:
  *         fields = descr.fields[childname]
  *         child, new_offset = fields             # <<<<<<<<<<<<<<
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:
  */
     if (likely(__pyx_v_fields != Py_None)) {
@@ -19346,15 +19353,15 @@
     }
     if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_dtype))))) __PYX_ERR(2, 852, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_child, ((PyArray_Descr *)__pyx_t_3));
     __pyx_t_3 = 0;
     __Pyx_XDECREF_SET(__pyx_v_new_offset, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":854
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":854
  *         child, new_offset = fields
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  */
     __pyx_t_4 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 854, __pyx_L1_error)
@@ -19363,37 +19370,37 @@
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 854, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_6 = ((((__pyx_v_end - __pyx_v_f) - ((int)__pyx_t_5)) < 15) != 0);
     if (unlikely(__pyx_t_6)) {
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
  * 
  *         if ((child.byteorder == c'>' and little_endian) or
  */
       __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 855, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(2, 855, __pyx_L1_error)
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":854
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":854
  *         child, new_offset = fields
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  */
     }
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")
  */
     __pyx_t_7 = ((__pyx_v_child->byteorder == '>') != 0);
@@ -19405,15 +19412,15 @@
     if (!__pyx_t_7) {
     } else {
       __pyx_t_6 = __pyx_t_7;
       goto __pyx_L7_bool_binop_done;
     }
     __pyx_L8_next_or:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":858
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":858
  * 
  *         if ((child.byteorder == c'>' and little_endian) or
  *             (child.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
  *             raise ValueError(u"Non-native byte order not supported")
  *             # One could encode it in the format string and have Cython
  */
     __pyx_t_7 = ((__pyx_v_child->byteorder == '<') != 0);
@@ -19422,46 +19429,46 @@
       __pyx_t_6 = __pyx_t_7;
       goto __pyx_L7_bool_binop_done;
     }
     __pyx_t_7 = ((!(__pyx_v_little_endian != 0)) != 0);
     __pyx_t_6 = __pyx_t_7;
     __pyx_L7_bool_binop_done:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")
  */
     if (unlikely(__pyx_t_6)) {
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":859
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":859
  *         if ((child.byteorder == c'>' and little_endian) or
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
  *             # One could encode it in the format string and have Cython
  *             # complain instead, BUT: < and > in format strings also imply
  */
       __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 859, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(2, 859, __pyx_L1_error)
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")
  */
     }
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":869
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":869
  * 
  *         # Output padding bytes
  *         while offset[0] < new_offset:             # <<<<<<<<<<<<<<
  *             f[0] = 120 # "x"; pad byte
  *             f += 1
  */
     while (1) {
@@ -19469,108 +19476,108 @@
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_new_offset, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 869, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 869, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (!__pyx_t_6) break;
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":870
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":870
  *         # Output padding bytes
  *         while offset[0] < new_offset:
  *             f[0] = 120 # "x"; pad byte             # <<<<<<<<<<<<<<
  *             f += 1
  *             offset[0] += 1
  */
       (__pyx_v_f[0]) = 0x78;
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":871
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":871
  *         while offset[0] < new_offset:
  *             f[0] = 120 # "x"; pad byte
  *             f += 1             # <<<<<<<<<<<<<<
  *             offset[0] += 1
  * 
  */
       __pyx_v_f = (__pyx_v_f + 1);
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":872
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":872
  *             f[0] = 120 # "x"; pad byte
  *             f += 1
  *             offset[0] += 1             # <<<<<<<<<<<<<<
  * 
  *         offset[0] += child.itemsize
  */
       __pyx_t_8 = 0;
       (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + 1);
     }
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":874
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":874
  *             offset[0] += 1
  * 
  *         offset[0] += child.itemsize             # <<<<<<<<<<<<<<
  * 
  *         if not PyDataType_HASFIELDS(child):
  */
     __pyx_t_8 = 0;
     (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + __pyx_v_child->elsize);
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":876
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":876
  *         offset[0] += child.itemsize
  * 
  *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
  *             t = child.type_num
  *             if end - f < 5:
  */
     __pyx_t_6 = ((!(PyDataType_HASFIELDS(__pyx_v_child) != 0)) != 0);
     if (__pyx_t_6) {
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":877
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":877
  * 
  *         if not PyDataType_HASFIELDS(child):
  *             t = child.type_num             # <<<<<<<<<<<<<<
  *             if end - f < 5:
  *                 raise RuntimeError(u"Format string allocated too short.")
  */
       __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_child->type_num); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 877, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_XDECREF_SET(__pyx_v_t, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
  *         if not PyDataType_HASFIELDS(child):
  *             t = child.type_num
  *             if end - f < 5:             # <<<<<<<<<<<<<<
  *                 raise RuntimeError(u"Format string allocated too short.")
  * 
  */
       __pyx_t_6 = (((__pyx_v_end - __pyx_v_f) < 5) != 0);
       if (unlikely(__pyx_t_6)) {
 
-        /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
+        /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
  *             t = child.type_num
  *             if end - f < 5:
  *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
  * 
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  */
         __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 879, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_Raise(__pyx_t_4, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __PYX_ERR(2, 879, __pyx_L1_error)
 
-        /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
+        /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
  *         if not PyDataType_HASFIELDS(child):
  *             t = child.type_num
  *             if end - f < 5:             # <<<<<<<<<<<<<<
  *                 raise RuntimeError(u"Format string allocated too short.")
  * 
  */
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":882
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":882
  * 
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  *             if   t == NPY_BYTE:        f[0] =  98 #"b"             # <<<<<<<<<<<<<<
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_BYTE); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 882, __pyx_L1_error)
@@ -19580,15 +19587,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 882, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 98;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":883
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":883
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  *             if   t == NPY_BYTE:        f[0] =  98 #"b"
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"             # <<<<<<<<<<<<<<
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UBYTE); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 883, __pyx_L1_error)
@@ -19598,15 +19605,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 883, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 66;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":884
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":884
  *             if   t == NPY_BYTE:        f[0] =  98 #"b"
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"             # <<<<<<<<<<<<<<
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_SHORT); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 884, __pyx_L1_error)
@@ -19616,15 +19623,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 884, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x68;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":885
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":885
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"             # <<<<<<<<<<<<<<
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_USHORT); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 885, __pyx_L1_error)
@@ -19634,15 +19641,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 885, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 72;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":886
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":886
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  *             elif t == NPY_INT:         f[0] = 105 #"i"             # <<<<<<<<<<<<<<
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_INT); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 886, __pyx_L1_error)
@@ -19652,15 +19659,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 886, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x69;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":887
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":887
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  *             elif t == NPY_UINT:        f[0] =  73 #"I"             # <<<<<<<<<<<<<<
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UINT); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 887, __pyx_L1_error)
@@ -19670,15 +19677,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 887, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 73;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":888
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":888
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  *             elif t == NPY_LONG:        f[0] = 108 #"l"             # <<<<<<<<<<<<<<
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 888, __pyx_L1_error)
@@ -19688,15 +19695,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 888, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x6C;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":889
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":889
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"             # <<<<<<<<<<<<<<
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 889, __pyx_L1_error)
@@ -19706,15 +19713,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 889, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 76;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":890
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":890
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"             # <<<<<<<<<<<<<<
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGLONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 890, __pyx_L1_error)
@@ -19724,15 +19731,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 890, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x71;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":891
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":891
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"             # <<<<<<<<<<<<<<
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONGLONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 891, __pyx_L1_error)
@@ -19742,15 +19749,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 891, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 81;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":892
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":892
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"             # <<<<<<<<<<<<<<
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_FLOAT); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 892, __pyx_L1_error)
@@ -19760,15 +19767,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 892, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x66;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":893
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":893
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"             # <<<<<<<<<<<<<<
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_DOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 893, __pyx_L1_error)
@@ -19778,15 +19785,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 893, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x64;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":894
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":894
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"             # <<<<<<<<<<<<<<
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 894, __pyx_L1_error)
@@ -19796,15 +19803,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 894, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x67;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":895
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":895
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf             # <<<<<<<<<<<<<<
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CFLOAT); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 895, __pyx_L1_error)
@@ -19816,15 +19823,15 @@
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 90;
         (__pyx_v_f[1]) = 0x66;
         __pyx_v_f = (__pyx_v_f + 1);
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":896
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":896
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd             # <<<<<<<<<<<<<<
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 896, __pyx_L1_error)
@@ -19836,15 +19843,15 @@
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 90;
         (__pyx_v_f[1]) = 0x64;
         __pyx_v_f = (__pyx_v_f + 1);
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":897
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":897
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg             # <<<<<<<<<<<<<<
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
  *             else:
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CLONGDOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 897, __pyx_L1_error)
@@ -19856,15 +19863,15 @@
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 90;
         (__pyx_v_f[1]) = 0x67;
         __pyx_v_f = (__pyx_v_f + 1);
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":898
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":898
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"             # <<<<<<<<<<<<<<
  *             else:
  *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_OBJECT); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 898, __pyx_L1_error)
@@ -19874,15 +19881,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 898, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (likely(__pyx_t_6)) {
         (__pyx_v_f[0]) = 79;
         goto __pyx_L15;
       }
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":900
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":900
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
  *             else:
  *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
  *             f += 1
  *         else:
  */
       /*else*/ {
@@ -19893,67 +19900,67 @@
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_Raise(__pyx_t_4, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __PYX_ERR(2, 900, __pyx_L1_error)
       }
       __pyx_L15:;
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":901
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":901
  *             else:
  *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  *             f += 1             # <<<<<<<<<<<<<<
  *         else:
  *             # Cython ignores struct boundary information ("T{...}"),
  */
       __pyx_v_f = (__pyx_v_f + 1);
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":876
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":876
  *         offset[0] += child.itemsize
  * 
  *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
  *             t = child.type_num
  *             if end - f < 5:
  */
       goto __pyx_L13;
     }
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":905
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":905
  *             # Cython ignores struct boundary information ("T{...}"),
  *             # so don't output it
  *             f = _util_dtypestring(child, f, end, offset)             # <<<<<<<<<<<<<<
  *     return f
  * 
  */
     /*else*/ {
       __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_child, __pyx_v_f, __pyx_v_end, __pyx_v_offset); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(2, 905, __pyx_L1_error)
       __pyx_v_f = __pyx_t_9;
     }
     __pyx_L13:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":850
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":850
  *     cdef tuple fields
  * 
  *     for childname in descr.names:             # <<<<<<<<<<<<<<
  *         fields = descr.fields[childname]
  *         child, new_offset = fields
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":906
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":906
  *             # so don't output it
  *             f = _util_dtypestring(child, f, end, offset)
  *     return f             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_f;
   goto __pyx_L0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":841
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":841
  *         return ()
  * 
  * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
  *     # Recursive utility function used in __getbuffer__ to get format
  *     # string. The new location in the format string is returned.
  */
 
@@ -19970,138 +19977,138 @@
   __Pyx_XDECREF(__pyx_v_childname);
   __Pyx_XDECREF(__pyx_v_new_offset);
   __Pyx_XDECREF(__pyx_v_t);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1022
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1022
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1023
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1023
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1025
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1025
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1026
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1026
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1028
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1028
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1029
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1029
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1025
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1025
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_array()
  */
 
@@ -20117,15 +20124,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_array()
  *     except Exception:
  */
   {
@@ -20133,53 +20140,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1035
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1035
  * cdef inline int import_array() except -1:
  *     try:
  *         _import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1035, __pyx_L3_error)
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1036
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1036
  *     try:
  *         _import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1036, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
  *         _import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1037, __pyx_L5_except_error)
@@ -20187,30 +20194,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 1037, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_array()
  */
 
@@ -20225,15 +20232,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1039
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1039
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20249,15 +20256,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -20265,53 +20272,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1041
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1041
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1041, __pyx_L3_error)
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1042
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1042
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1042, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1043, __pyx_L5_except_error)
@@ -20319,30 +20326,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 1043, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1039
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1039
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20357,15 +20364,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
+/* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20381,15 +20388,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -20397,81 +20404,81 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1047
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1047
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1047, __pyx_L3_error)
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1048
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1048
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1048, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1049
+      /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1049
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1049, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 1049, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+    /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -35568,81 +35575,81 @@
   __pyx_tuple__3 = PyTuple_Pack(3, __pyx_int_46664382, __pyx_int_119629453, __pyx_int_188721270); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
   __pyx_tuple__4 = PyTuple_Pack(3, __pyx_int_210499617, __pyx_int_198014708, __pyx_int_85186564); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_C_contiguous); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
  * 
  *             info.buf = PyArray_DATA(self)
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_Fortran_contiguou); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_Non_native_byte_order_not_suppor); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
  * 
  *         if ((child.byteorder == c'>' and little_endian) or
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 855, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
  *             t = child.type_num
  *             if end - f < 5:
  *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
  * 
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor_2); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 879, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
  *         _import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 1037, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "../../../../tmp/build-env-jxovi0m3/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+  /* "../../../../tmp/build-env-7dd9b035/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 1043, __pyx_L1_error)
@@ -35845,147 +35852,147 @@
   __Pyx_GIVEREF(__pyx_tuple__30);
 
   /* "arch/univariate/recursions.pyx":47
  * 
  * 
  * def harch_core(             # <<<<<<<<<<<<<<
  *     Py_ssize_t t,
- *     double[::1] parameters,
+ *     const double[::1] parameters,
  */
   __pyx_tuple__31 = PyTuple_Pack(10, __pyx_n_s_t, __pyx_n_s_parameters, __pyx_n_s_resids, __pyx_n_s_sigma2, __pyx_n_s_lags, __pyx_n_s_backcast, __pyx_n_s_var_bounds, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_param); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__31);
   __Pyx_GIVEREF(__pyx_tuple__31);
   __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(7, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_harch_core, 47, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 47, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":100
  * 
  * 
- * def harch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                     double[::1] resids,
+ * def harch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                     const double[::1] resids,
  *                     double[::1] sigma2,
  */
   __pyx_tuple__33 = PyTuple_Pack(12, __pyx_n_s_parameters, __pyx_n_s_resids, __pyx_n_s_sigma2, __pyx_n_s_lags, __pyx_n_s_nobs, __pyx_n_s_backcast, __pyx_n_s_var_bounds, __pyx_n_s_t, __pyx_n_s_i, __pyx_n_s_num_lags, __pyx_n_s_j, __pyx_n_s_param); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
   __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(7, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_harch_recursion, 100, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 100, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":144
  *     return np.asarray(sigma2)
  * 
- * def arch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                    double[::1] resids,
+ * def arch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                    const double[::1] resids,
  *                    double[::1] sigma2,
  */
   __pyx_tuple__35 = PyTuple_Pack(10, __pyx_n_s_parameters, __pyx_n_s_resids, __pyx_n_s_sigma2, __pyx_n_s_p, __pyx_n_s_nobs, __pyx_n_s_backcast, __pyx_n_s_var_bounds, __pyx_n_s_t, __pyx_n_s_i, __pyx_n_s_param); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
   __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(7, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_arch_recursion, 144, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 144, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":187
  *     return np.asarray(sigma2)
  * 
  * def garch_core(             # <<<<<<<<<<<<<<
  *     Py_ssize_t t,
- *     double[::1] parameters,
+ *     const double[::1] parameters,
  */
   __pyx_tuple__37 = PyTuple_Pack(12, __pyx_n_s_t, __pyx_n_s_parameters, __pyx_n_s_resids, __pyx_n_s_sigma2, __pyx_n_s_backcast, __pyx_n_s_var_bounds, __pyx_n_s_p, __pyx_n_s_o, __pyx_n_s_q, __pyx_n_s_power, __pyx_n_s_j, __pyx_n_s_loc); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__37);
   __Pyx_GIVEREF(__pyx_tuple__37);
   __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(10, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_garch_core, 187, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 187, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":259
  * 
  * 
- * def garch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                     double[::1] fresids,
- *                     double[::1] sresids,
+ * def garch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                     const double[::1] fresids,
+ *                     const double[::1] sresids,
  */
   __pyx_tuple__39 = PyTuple_Pack(13, __pyx_n_s_parameters, __pyx_n_s_fresids, __pyx_n_s_sresids, __pyx_n_s_sigma2, __pyx_n_s_p, __pyx_n_s_o, __pyx_n_s_q, __pyx_n_s_nobs, __pyx_n_s_backcast, __pyx_n_s_var_bounds, __pyx_n_s_t, __pyx_n_s_j, __pyx_n_s_loc); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__39);
   __Pyx_GIVEREF(__pyx_tuple__39);
   __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(10, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_garch_recursion, 259, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 259, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":327
  *     return np.asarray(sigma2)
  * 
- * def egarch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                      double[::1] resids,
+ * def egarch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                      const double[::1] resids,
  *                      double[::1] sigma2,
  */
   __pyx_tuple__41 = PyTuple_Pack(15, __pyx_n_s_parameters, __pyx_n_s_resids, __pyx_n_s_sigma2, __pyx_n_s_p, __pyx_n_s_o, __pyx_n_s_q, __pyx_n_s_nobs, __pyx_n_s_backcast, __pyx_n_s_var_bounds, __pyx_n_s_lnsigma2, __pyx_n_s_std_resids, __pyx_n_s_abs_std_resids, __pyx_n_s_t, __pyx_n_s_j, __pyx_n_s_loc); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__41);
   __Pyx_GIVEREF(__pyx_tuple__41);
   __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(12, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_egarch_recursion, 327, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 327, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":408
  * 
  * 
- * def midas_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                     double[::1] weights,
- *                     double[::1] resids,
+ * def midas_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                     const double[::1] weights,
+ *                     const double[::1] resids,
  */
   __pyx_tuple__43 = PyTuple_Pack(18, __pyx_n_s_parameters, __pyx_n_s_weights, __pyx_n_s_resids, __pyx_n_s_sigma2, __pyx_n_s_nobs, __pyx_n_s_backcast, __pyx_n_s_var_bounds, __pyx_n_s_m, __pyx_n_s_t, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_param, __pyx_n_s_omega, __pyx_n_s_alpha, __pyx_n_s_gamma, __pyx_n_s_aw, __pyx_n_s_gw, __pyx_n_s_resids2); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__43);
   __Pyx_GIVEREF(__pyx_tuple__43);
   __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(7, 0, 18, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_midas_recursion, 408, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 408, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":490
  * 
  * 
- * def figarch_weights(double[::1] parameters, int p, int q, int trunc_lag):             # <<<<<<<<<<<<<<
+ * def figarch_weights(const double[::1] parameters, int p, int q, int trunc_lag):             # <<<<<<<<<<<<<<
  *     return np.asarray(_figarch_weights(parameters, p, q, trunc_lag))
  * 
  */
   __pyx_tuple__45 = PyTuple_Pack(4, __pyx_n_s_parameters, __pyx_n_s_p, __pyx_n_s_q, __pyx_n_s_trunc_lag); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 490, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__45);
   __Pyx_GIVEREF(__pyx_tuple__45);
   __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_figarch_weights, 490, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 490, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":494
  * 
  * 
- * def figarch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                       double[::1] fresids,
+ * def figarch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                       const double[::1] fresids,
  *                       double[::1] sigma2,
  */
   __pyx_tuple__47 = PyTuple_Pack(18, __pyx_n_s_parameters, __pyx_n_s_fresids, __pyx_n_s_sigma2, __pyx_n_s_p, __pyx_n_s_q, __pyx_n_s_nobs, __pyx_n_s_trunc_lag, __pyx_n_s_backcast, __pyx_n_s_var_bounds, __pyx_n_s_t, __pyx_n_s_i, __pyx_n_s_bc1, __pyx_n_s_bc2, __pyx_n_s_bc_weight, __pyx_n_s_omega, __pyx_n_s_beta, __pyx_n_s_omega_tilde, __pyx_n_s_lam); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__47);
   __Pyx_GIVEREF(__pyx_tuple__47);
   __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(9, 0, 18, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_figarch_recursion, 494, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 494, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":523
  * 
  * 
- * def aparch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                     double[::1] resids,
- *                     double[::1] abs_resids,
+ * def aparch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                      const double[::1] resids,
+ *                      const double[::1] abs_resids,
  */
   __pyx_tuple__49 = PyTuple_Pack(15, __pyx_n_s_parameters, __pyx_n_s_resids, __pyx_n_s_abs_resids, __pyx_n_s_sigma2, __pyx_n_s_sigma_delta, __pyx_n_s_p, __pyx_n_s_o, __pyx_n_s_q, __pyx_n_s_nobs, __pyx_n_s_backcast, __pyx_n_s_var_bounds, __pyx_n_s_delta, __pyx_n_s_shock, __pyx_n_s_t, __pyx_n_s_j); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 523, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__49);
   __Pyx_GIVEREF(__pyx_tuple__49);
   __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(11, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_aparch_recursion, 523, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 523, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":592
  *         pass
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
   __pyx_tuple__51 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_parameters, __pyx_n_s_backcast, __pyx_n_s_nobs); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 592, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__51);
   __Pyx_GIVEREF(__pyx_tuple__51);
   __pyx_codeobj__52 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_initialize_update, 592, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__52)) __PYX_ERR(0, 592, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":604
  *         pass
  * 
  *     def _update_tester(self,             # <<<<<<<<<<<<<<
  *                        Py_ssize_t t,
- *                        double[::1] parameters,
+ *                        const double[::1] parameters,
  */
   __pyx_tuple__53 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_t, __pyx_n_s_parameters, __pyx_n_s_resids, __pyx_n_s_sigma2, __pyx_n_s_var_bounds); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(0, 604, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__53);
   __Pyx_GIVEREF(__pyx_tuple__53);
   __pyx_codeobj__54 = (PyObject*)__Pyx_PyCode_New(6, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_update_tester, 604, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__54)) __PYX_ERR(0, 604, __pyx_L1_error)
 
   /* "(tree fragment)":1
@@ -36008,15 +36015,15 @@
   __Pyx_GOTREF(__pyx_tuple__57);
   __Pyx_GIVEREF(__pyx_tuple__57);
   __pyx_codeobj__58 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__57, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__58)) __PYX_ERR(1, 16, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":624
  *         self.backcast = -1.0
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         self.backcast = backcast
  * 
  */
   __pyx_tuple__59 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_parameters, __pyx_n_s_backcast, __pyx_n_s_nobs); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(0, 624, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__59);
   __Pyx_GIVEREF(__pyx_tuple__59);
   __pyx_codeobj__60 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__59, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_initialize_update, 624, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__60)) __PYX_ERR(0, 624, __pyx_L1_error)
@@ -36065,25 +36072,25 @@
   __Pyx_GOTREF(__pyx_tuple__67);
   __Pyx_GIVEREF(__pyx_tuple__67);
   __pyx_codeobj__68 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_reduce, 678, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__68)) __PYX_ERR(0, 678, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":681
  *         return HARCHUpdater, (np.asarray(self.lags),), (self.backcast,)
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         self.backcast = backcast
  * 
  */
   __pyx_tuple__69 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_parameters, __pyx_n_s_backcast, __pyx_n_s_nobs); if (unlikely(!__pyx_tuple__69)) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__69);
   __Pyx_GIVEREF(__pyx_tuple__69);
   __pyx_codeobj__70 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_initialize_update, 681, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__70)) __PYX_ERR(0, 681, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":720
- *             self.params[2] =lam
+ *             self.params[2] = lam
  * 
  *     def __setstate__(self, state):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t i
  *         self.backcast = state[0]
  */
   __pyx_tuple__71 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_i, __pyx_n_s_params); if (unlikely(!__pyx_tuple__71)) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__71);
@@ -36101,15 +36108,15 @@
   __Pyx_GOTREF(__pyx_tuple__73);
   __Pyx_GIVEREF(__pyx_tuple__73);
   __pyx_codeobj__74 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__73, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_reduce, 727, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__74)) __PYX_ERR(0, 727, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":731
  *         return EWMAUpdater, (lam,), (self.backcast, np.asarray(self.params))
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         if self.estimate_lam:
  *             self.params[1] = 1.0 - parameters[0]
  */
   __pyx_tuple__75 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_parameters, __pyx_n_s_backcast, __pyx_n_s_nobs); if (unlikely(!__pyx_tuple__75)) __PYX_ERR(0, 731, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__75);
   __Pyx_GIVEREF(__pyx_tuple__75);
   __pyx_codeobj__76 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__75, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_initialize_update, 731, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__76)) __PYX_ERR(0, 731, __pyx_L1_error)
@@ -36137,15 +36144,15 @@
   __Pyx_GOTREF(__pyx_tuple__79);
   __Pyx_GIVEREF(__pyx_tuple__79);
   __pyx_codeobj__80 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__79, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_reduce, 787, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__80)) __PYX_ERR(0, 787, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":813
  *             self.weights[i] /= sum_w
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         cdef double alpha, gamma, theta
  * 
  */
   __pyx_tuple__81 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_parameters, __pyx_n_s_backcast, __pyx_n_s_nobs, __pyx_n_s_alpha, __pyx_n_s_gamma, __pyx_n_s_theta, __pyx_n_s_i); if (unlikely(!__pyx_tuple__81)) __PYX_ERR(0, 813, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__81);
   __Pyx_GIVEREF(__pyx_tuple__81);
   __pyx_codeobj__82 = (PyObject*)__Pyx_PyCode_New(4, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__81, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_initialize_update, 813, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__82)) __PYX_ERR(0, 813, __pyx_L1_error)
@@ -36173,15 +36180,15 @@
   __Pyx_GOTREF(__pyx_tuple__85);
   __Pyx_GIVEREF(__pyx_tuple__85);
   __pyx_codeobj__86 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_reduce, 884, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__86)) __PYX_ERR(0, 884, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":887
  *         return FIGARCHUpdater, (self.p, self.q, self.power, self.truncation), (self.backcast, np.asarray(self.lam), np.asarray(self.fresids))
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         self.lam = _figarch_weights(parameters[1:], self.p, self.q, self.truncation)
  *         self.backcast = backcast
  */
   __pyx_tuple__87 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_parameters, __pyx_n_s_backcast, __pyx_n_s_nobs); if (unlikely(!__pyx_tuple__87)) __PYX_ERR(0, 887, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__87);
   __Pyx_GIVEREF(__pyx_tuple__87);
   __pyx_codeobj__88 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__87, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_initialize_update, 887, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__88)) __PYX_ERR(0, 887, __pyx_L1_error)
@@ -36245,29 +36252,29 @@
   __Pyx_GOTREF(__pyx_tuple__97);
   __Pyx_GIVEREF(__pyx_tuple__97);
   __pyx_codeobj__98 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__97, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_reduce, 1024, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__98)) __PYX_ERR(0, 1024, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":1046
  *             self.std_resids = np.empty(nobs)
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         self.backcast = backcast
  *         self._resize(nobs)
  */
   __pyx_tuple__99 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_parameters, __pyx_n_s_backcast, __pyx_n_s_nobs); if (unlikely(!__pyx_tuple__99)) __PYX_ERR(0, 1046, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__99);
   __Pyx_GIVEREF(__pyx_tuple__99);
   __pyx_codeobj__100 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__99, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_initialize_update, 1046, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__100)) __PYX_ERR(0, 1046, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":1097
  *         self.volatility_updater = updater
  * 
  *     def recursion(self,             # <<<<<<<<<<<<<<
- *                   double[::1] y,
- *                   double[:,::1] x,
+ *                   const double[::1] y,
+ *                   const double[:,::1] x,
  */
   __pyx_tuple__101 = PyTuple_Pack(14, __pyx_n_s_self, __pyx_n_s_y, __pyx_n_s_x, __pyx_n_s_mean_parameters, __pyx_n_s_variance_params, __pyx_n_s_sigma2, __pyx_n_s_var_bounds, __pyx_n_s_power, __pyx_n_s_t, __pyx_n_s_i, __pyx_n_s_nobs, __pyx_n_s_k, __pyx_n_s_resids, __pyx_n_s_gamma); if (unlikely(!__pyx_tuple__101)) __PYX_ERR(0, 1097, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__101);
   __Pyx_GIVEREF(__pyx_tuple__101);
   __pyx_codeobj__102 = (PyObject*)__Pyx_PyCode_New(8, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__101, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_arch_univariate_recursions_pyx, __pyx_n_s_recursion, 1097, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__102)) __PYX_ERR(0, 1097, __pyx_L1_error)
 
   /* "(tree fragment)":1
@@ -36992,148 +36999,148 @@
   __pyx_t_2 = __pyx_f_5numpy_import_array(); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 35, __pyx_L1_error)
 
   /* "arch/univariate/recursions.pyx":47
  * 
  * 
  * def harch_core(             # <<<<<<<<<<<<<<
  *     Py_ssize_t t,
- *     double[::1] parameters,
+ *     const double[::1] parameters,
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_1harch_core, 0, __pyx_n_s_harch_core, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_harch_core, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "arch/univariate/recursions.pyx":100
  * 
  * 
- * def harch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                     double[::1] resids,
+ * def harch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                     const double[::1] resids,
  *                     double[::1] sigma2,
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_3harch_recursion, 0, __pyx_n_s_harch_recursion, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_harch_recursion, __pyx_t_1) < 0) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "arch/univariate/recursions.pyx":144
  *     return np.asarray(sigma2)
  * 
- * def arch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                    double[::1] resids,
+ * def arch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                    const double[::1] resids,
  *                    double[::1] sigma2,
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_5arch_recursion, 0, __pyx_n_s_arch_recursion, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_arch_recursion, __pyx_t_1) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "arch/univariate/recursions.pyx":187
  *     return np.asarray(sigma2)
  * 
  * def garch_core(             # <<<<<<<<<<<<<<
  *     Py_ssize_t t,
- *     double[::1] parameters,
+ *     const double[::1] parameters,
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_7garch_core, 0, __pyx_n_s_garch_core, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_garch_core, __pyx_t_1) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "arch/univariate/recursions.pyx":259
  * 
  * 
- * def garch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                     double[::1] fresids,
- *                     double[::1] sresids,
+ * def garch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                     const double[::1] fresids,
+ *                     const double[::1] sresids,
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_9garch_recursion, 0, __pyx_n_s_garch_recursion, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_garch_recursion, __pyx_t_1) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "arch/univariate/recursions.pyx":327
  *     return np.asarray(sigma2)
  * 
- * def egarch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                      double[::1] resids,
+ * def egarch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                      const double[::1] resids,
  *                      double[::1] sigma2,
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_11egarch_recursion, 0, __pyx_n_s_egarch_recursion, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_egarch_recursion, __pyx_t_1) < 0) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "arch/univariate/recursions.pyx":408
  * 
  * 
- * def midas_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                     double[::1] weights,
- *                     double[::1] resids,
+ * def midas_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                     const double[::1] weights,
+ *                     const double[::1] resids,
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_13midas_recursion, 0, __pyx_n_s_midas_recursion, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_midas_recursion, __pyx_t_1) < 0) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "arch/univariate/recursions.pyx":490
  * 
  * 
- * def figarch_weights(double[::1] parameters, int p, int q, int trunc_lag):             # <<<<<<<<<<<<<<
+ * def figarch_weights(const double[::1] parameters, int p, int q, int trunc_lag):             # <<<<<<<<<<<<<<
  *     return np.asarray(_figarch_weights(parameters, p, q, trunc_lag))
  * 
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_15figarch_weights, 0, __pyx_n_s_figarch_weights, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 490, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_figarch_weights, __pyx_t_1) < 0) __PYX_ERR(0, 490, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "arch/univariate/recursions.pyx":494
  * 
  * 
- * def figarch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                       double[::1] fresids,
+ * def figarch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                       const double[::1] fresids,
  *                       double[::1] sigma2,
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_17figarch_recursion, 0, __pyx_n_s_figarch_recursion, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__48)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_figarch_recursion, __pyx_t_1) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "arch/univariate/recursions.pyx":523
  * 
  * 
- * def aparch_recursion(double[::1] parameters,             # <<<<<<<<<<<<<<
- *                     double[::1] resids,
- *                     double[::1] abs_resids,
+ * def aparch_recursion(const double[::1] parameters,             # <<<<<<<<<<<<<<
+ *                      const double[::1] resids,
+ *                      const double[::1] abs_resids,
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_19aparch_recursion, 0, __pyx_n_s_aparch_recursion, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 523, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_aparch_recursion, __pyx_t_1) < 0) __PYX_ERR(0, 523, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "arch/univariate/recursions.pyx":592
  *         pass
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_17VolatilityUpdater_3initialize_update, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_VolatilityUpdater_initialize_upd, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__52)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 592, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_4arch_10univariate_10recursions_VolatilityUpdater->tp_dict, __pyx_n_s_initialize_update, __pyx_t_1) < 0) __PYX_ERR(0, 592, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_4arch_10univariate_10recursions_VolatilityUpdater);
 
   /* "arch/univariate/recursions.pyx":604
  *         pass
  * 
  *     def _update_tester(self,             # <<<<<<<<<<<<<<
  *                        Py_ssize_t t,
- *                        double[::1] parameters,
+ *                        const double[::1] parameters,
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_17VolatilityUpdater_5_update_tester, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_VolatilityUpdater__update_tester, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__54)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 604, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_4arch_10univariate_10recursions_VolatilityUpdater->tp_dict, __pyx_n_s_update_tester, __pyx_t_1) < 0) __PYX_ERR(0, 604, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_4arch_10univariate_10recursions_VolatilityUpdater);
 
@@ -37159,15 +37166,15 @@
   if (PyDict_SetItem((PyObject *)__pyx_ptype_4arch_10univariate_10recursions_VolatilityUpdater->tp_dict, __pyx_n_s_setstate_cython, __pyx_t_1) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_4arch_10univariate_10recursions_VolatilityUpdater);
 
   /* "arch/univariate/recursions.pyx":624
  *         self.backcast = -1.0
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         self.backcast = backcast
  * 
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_12GARCHUpdater_3initialize_update, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_GARCHUpdater_initialize_update, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__60)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 624, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_4arch_10univariate_10recursions_GARCHUpdater->tp_dict, __pyx_n_s_initialize_update, __pyx_t_1) < 0) __PYX_ERR(0, 624, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -37221,26 +37228,26 @@
   if (PyDict_SetItem((PyObject *)__pyx_ptype_4arch_10univariate_10recursions_HARCHUpdater->tp_dict, __pyx_n_s_reduce, __pyx_t_1) < 0) __PYX_ERR(0, 678, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_4arch_10univariate_10recursions_HARCHUpdater);
 
   /* "arch/univariate/recursions.pyx":681
  *         return HARCHUpdater, (np.asarray(self.lags),), (self.backcast,)
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         self.backcast = backcast
  * 
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_12HARCHUpdater_7initialize_update, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_HARCHUpdater_initialize_update, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__70)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_4arch_10univariate_10recursions_HARCHUpdater->tp_dict, __pyx_n_s_initialize_update, __pyx_t_1) < 0) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_4arch_10univariate_10recursions_HARCHUpdater);
 
   /* "arch/univariate/recursions.pyx":720
- *             self.params[2] =lam
+ *             self.params[2] = lam
  * 
  *     def __setstate__(self, state):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t i
  *         self.backcast = state[0]
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_11EWMAUpdater_3__setstate__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_EWMAUpdater___setstate, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__72)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
@@ -37260,15 +37267,15 @@
   if (PyDict_SetItem((PyObject *)__pyx_ptype_4arch_10univariate_10recursions_EWMAUpdater->tp_dict, __pyx_n_s_reduce, __pyx_t_1) < 0) __PYX_ERR(0, 727, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_4arch_10univariate_10recursions_EWMAUpdater);
 
   /* "arch/univariate/recursions.pyx":731
  *         return EWMAUpdater, (lam,), (self.backcast, np.asarray(self.params))
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         if self.estimate_lam:
  *             self.params[1] = 1.0 - parameters[0]
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_11EWMAUpdater_7initialize_update, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_EWMAUpdater_initialize_update, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__76)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 731, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_4arch_10univariate_10recursions_EWMAUpdater->tp_dict, __pyx_n_s_initialize_update, __pyx_t_1) < 0) __PYX_ERR(0, 731, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -37299,15 +37306,15 @@
   if (PyDict_SetItem((PyObject *)__pyx_ptype_4arch_10univariate_10recursions_MIDASUpdater->tp_dict, __pyx_n_s_reduce, __pyx_t_1) < 0) __PYX_ERR(0, 787, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_4arch_10univariate_10recursions_MIDASUpdater);
 
   /* "arch/univariate/recursions.pyx":813
  *             self.weights[i] /= sum_w
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         cdef double alpha, gamma, theta
  * 
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_12MIDASUpdater_7initialize_update, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_MIDASUpdater_initialize_update, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 813, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_4arch_10univariate_10recursions_MIDASUpdater->tp_dict, __pyx_n_s_initialize_update, __pyx_t_1) < 0) __PYX_ERR(0, 813, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -37338,15 +37345,15 @@
   if (PyDict_SetItem((PyObject *)__pyx_ptype_4arch_10univariate_10recursions_FIGARCHUpdater->tp_dict, __pyx_n_s_reduce, __pyx_t_1) < 0) __PYX_ERR(0, 884, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_4arch_10univariate_10recursions_FIGARCHUpdater);
 
   /* "arch/univariate/recursions.pyx":887
  *         return FIGARCHUpdater, (self.p, self.q, self.power, self.truncation), (self.backcast, np.asarray(self.lam), np.asarray(self.fresids))
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         self.lam = _figarch_weights(parameters[1:], self.p, self.q, self.truncation)
  *         self.backcast = backcast
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_14FIGARCHUpdater_7initialize_update, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_FIGARCHUpdater_initialize_update, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__88)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 887, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_4arch_10univariate_10recursions_FIGARCHUpdater->tp_dict, __pyx_n_s_initialize_update, __pyx_t_1) < 0) __PYX_ERR(0, 887, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -37421,30 +37428,30 @@
   if (PyDict_SetItem((PyObject *)__pyx_ptype_4arch_10univariate_10recursions_EGARCHUpdater->tp_dict, __pyx_n_s_reduce, __pyx_t_3) < 0) __PYX_ERR(0, 1024, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_4arch_10univariate_10recursions_EGARCHUpdater);
 
   /* "arch/univariate/recursions.pyx":1046
  *             self.std_resids = np.empty(nobs)
  * 
- *     def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
+ *     def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):             # <<<<<<<<<<<<<<
  *         self.backcast = backcast
  *         self._resize(nobs)
  */
   __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_13EGARCHUpdater_7initialize_update, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_EGARCHUpdater_initialize_update, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__100)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1046, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_4arch_10univariate_10recursions_EGARCHUpdater->tp_dict, __pyx_n_s_initialize_update, __pyx_t_3) < 0) __PYX_ERR(0, 1046, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_4arch_10univariate_10recursions_EGARCHUpdater);
 
   /* "arch/univariate/recursions.pyx":1097
  *         self.volatility_updater = updater
  * 
  *     def recursion(self,             # <<<<<<<<<<<<<<
- *                   double[::1] y,
- *                   double[:,::1] x,
+ *                   const double[::1] y,
+ *                   const double[:,::1] x,
  */
   __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4arch_10univariate_10recursions_19ARCHInMeanRecursion_3recursion, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ARCHInMeanRecursion_recursion, NULL, __pyx_n_s_arch_univariate_recursions, __pyx_d, ((PyObject *)__pyx_codeobj__102)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1097, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_4arch_10univariate_10recursions_ARCHInMeanRecursion->tp_dict, __pyx_n_s_recursion, __pyx_t_3) < 0) __PYX_ERR(0, 1097, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_4arch_10univariate_10recursions_ARCHInMeanRecursion);
 
@@ -41941,14 +41948,37 @@
     retval = -1;
 no_fail:
     __Pyx_RefNannyFinishContext();
     return retval;
 }
 
 /* ObjectToMemviewSlice */
+    static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_double__const__(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, __Pyx_IS_C_CONTIG,
+                                                 (PyBUF_C_CONTIGUOUS | PyBUF_FORMAT) | writable_flag, 1,
+                                                 &__Pyx_TypeInfo_double__const__, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
+/* ObjectToMemviewSlice */
     static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_double(PyObject *obj, int writable_flag) {
     __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
     __Pyx_BufFmt_StackElem stack[1];
     int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
     int retcode;
     if (obj == Py_None) {
         result.memview = (struct __pyx_memoryview_obj *) Py_None;
@@ -41964,14 +41994,60 @@
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
     return result;
 }
 
 /* ObjectToMemviewSlice */
+    static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int32_t__const__(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, __Pyx_IS_C_CONTIG,
+                                                 (PyBUF_C_CONTIGUOUS | PyBUF_FORMAT) | writable_flag, 1,
+                                                 &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t__const__, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
+/* ObjectToMemviewSlice */
+    static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_double__const__(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_FOLLOW), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, __Pyx_IS_C_CONTIG,
+                                                 (PyBUF_C_CONTIGUOUS | PyBUF_FORMAT) | writable_flag, 2,
+                                                 &__Pyx_TypeInfo_double__const__, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
+/* ObjectToMemviewSlice */
     static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int32_t(PyObject *obj, int writable_flag) {
     __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
     __Pyx_BufFmt_StackElem stack[1];
     int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
     int retcode;
     if (obj == Py_None) {
         result.memview = (struct __pyx_memoryview_obj *) Py_None;
@@ -42022,23 +42098,16 @@
     if ((value == (double)-1) && PyErr_Occurred())
         return 0;
     *(double *) itemp = value;
     return 1;
 }
 
 /* MemviewDtypeToObject */
-    static CYTHON_INLINE PyObject *__pyx_memview_get_nn___pyx_t_5numpy_int32_t(const char *itemp) {
-    return (PyObject *) __Pyx_PyInt_From_npy_int32(*(__pyx_t_5numpy_int32_t *) itemp);
-}
-static CYTHON_INLINE int __pyx_memview_set_nn___pyx_t_5numpy_int32_t(const char *itemp, PyObject *obj) {
-    __pyx_t_5numpy_int32_t value = __Pyx_PyInt_As_npy_int32(obj);
-    if ((value == ((npy_int32)-1)) && PyErr_Occurred())
-        return 0;
-    *(__pyx_t_5numpy_int32_t *) itemp = value;
-    return 1;
+    static CYTHON_INLINE PyObject *__pyx_memview_get_nn___pyx_t_5numpy_int32_t__const__(const char *itemp) {
+    return (PyObject *) __Pyx_PyInt_From_npy_int32(*(__pyx_t_5numpy_int32_t const  *) itemp);
 }
 
 /* Declarations */
     #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
@@ -42914,210 +42983,14 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
-/* CIntFromPy */
-    static CYTHON_INLINE npy_int32 __Pyx_PyInt_As_npy_int32(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const npy_int32 neg_one = (npy_int32) -1, const_zero = (npy_int32) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-#if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_Check(x))) {
-        if (sizeof(npy_int32) < sizeof(long)) {
-            __PYX_VERIFY_RETURN_INT(npy_int32, long, PyInt_AS_LONG(x))
-        } else {
-            long val = PyInt_AS_LONG(x);
-            if (is_unsigned && unlikely(val < 0)) {
-                goto raise_neg_overflow;
-            }
-            return (npy_int32) val;
-        }
-    } else
-#endif
-    if (likely(PyLong_Check(x))) {
-        if (is_unsigned) {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (npy_int32) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(npy_int32, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(npy_int32) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) >= 2 * PyLong_SHIFT) {
-                            return (npy_int32) (((((npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0]));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(npy_int32) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) >= 3 * PyLong_SHIFT) {
-                            return (npy_int32) (((((((npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0]));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(npy_int32) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) >= 4 * PyLong_SHIFT) {
-                            return (npy_int32) (((((((((npy_int32)digits[3]) << PyLong_SHIFT) | (npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0]));
-                        }
-                    }
-                    break;
-            }
-#endif
-#if CYTHON_COMPILING_IN_CPYTHON
-            if (unlikely(Py_SIZE(x) < 0)) {
-                goto raise_neg_overflow;
-            }
-#else
-            {
-                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
-                if (unlikely(result < 0))
-                    return (npy_int32) -1;
-                if (unlikely(result == 1))
-                    goto raise_neg_overflow;
-            }
-#endif
-            if (sizeof(npy_int32) <= sizeof(unsigned long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(npy_int32, unsigned long, PyLong_AsUnsignedLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(npy_int32) <= sizeof(unsigned PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(npy_int32, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
-#endif
-            }
-        } else {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (npy_int32) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(npy_int32, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(npy_int32,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(npy_int32) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) - 1 > 2 * PyLong_SHIFT) {
-                            return (npy_int32) (((npy_int32)-1)*(((((npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
-                        }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(npy_int32) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) - 1 > 2 * PyLong_SHIFT) {
-                            return (npy_int32) ((((((npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
-                        }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(npy_int32) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) - 1 > 3 * PyLong_SHIFT) {
-                            return (npy_int32) (((npy_int32)-1)*(((((((npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(npy_int32) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) - 1 > 3 * PyLong_SHIFT) {
-                            return (npy_int32) ((((((((npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
-                        }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(npy_int32) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) - 1 > 4 * PyLong_SHIFT) {
-                            return (npy_int32) (((npy_int32)-1)*(((((((((npy_int32)digits[3]) << PyLong_SHIFT) | (npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(npy_int32) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) - 1 > 4 * PyLong_SHIFT) {
-                            return (npy_int32) ((((((((((npy_int32)digits[3]) << PyLong_SHIFT) | (npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
-                        }
-                    }
-                    break;
-            }
-#endif
-            if (sizeof(npy_int32) <= sizeof(long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(npy_int32, long, PyLong_AsLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(npy_int32) <= sizeof(PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(npy_int32, PY_LONG_LONG, PyLong_AsLongLong(x))
-#endif
-            }
-        }
-        {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
-            npy_int32 val;
-            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
-            if (likely(v) && !PyLong_Check(v)) {
-                PyObject *tmp = v;
-                v = PyNumber_Long(tmp);
-                Py_DECREF(tmp);
-            }
- #endif
-            if (likely(v)) {
-                int one = 1; int is_little = (int)*(unsigned char *)&one;
-                unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
-                Py_DECREF(v);
-                if (likely(!ret))
-                    return val;
-            }
-#endif
-            return (npy_int32) -1;
-        }
-    } else {
-        npy_int32 val;
-        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (npy_int32) -1;
-        val = __Pyx_PyInt_As_npy_int32(tmp);
-        Py_DECREF(tmp);
-        return val;
-    }
-raise_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to npy_int32");
-    return (npy_int32) -1;
-raise_neg_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to npy_int32");
-    return (npy_int32) -1;
-}
-
 /* CIntToPy */
     static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum NPY_TYPES neg_one = (enum NPY_TYPES) -1, const_zero = (enum NPY_TYPES) 0;
```

### Comparing `arch-5.4.0/arch/univariate/recursions.pyi` & `arch-5.5.0/arch/univariate/recursions.pyi`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/univariate/recursions.pyx` & `arch-5.5.0/arch/univariate/recursions.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -42,20 +42,20 @@
             sigma2[0] = var_bounds[1] + 1000
         else:
             sigma2[0] = var_bounds[1] + log(sigma2[0] / var_bounds[1])
 
 
 def harch_core(
     Py_ssize_t t,
-    double[::1] parameters,
-    double[::1] resids,
+    const double[::1] parameters,
+    const double[::1] resids,
     double[::1] sigma2,
-    np.int32_t[::1] lags,
+    const np.int32_t[::1] lags,
     double backcast,
-    double[:, ::1] var_bounds,
+    const double[:, ::1] var_bounds,
 ):
     """
     Compute variance recursion step for HARCH model
 
     Parameters
     ----------
     t: int
@@ -93,21 +93,21 @@
             else:
                 sigma2[t] += param * backcast
 
     bounds_check(&sigma2[t], &var_bounds[t, 0])
     return sigma2[t]
 
 
-def harch_recursion(double[::1] parameters,
-                    double[::1] resids,
+def harch_recursion(const double[::1] parameters,
+                    const double[::1] resids,
                     double[::1] sigma2,
                     np.int32_t[::1] lags,
                     int nobs,
                     double backcast,
-                    double[:, ::1] var_bounds):
+                    const double[:, ::1] var_bounds):
     """
     Parameters
     ----------
     parameters : 1-d array, float64
         Model parameters
     resids : 1-d array, float64
         Residuals to use in the recursion
@@ -137,21 +137,21 @@
                     sigma2[t] += param * resids[t - j - 1] * resids[t - j - 1]
                 else:
                     sigma2[t] += param * backcast
         bounds_check(&sigma2[t], &var_bounds[t, 0])
 
     return np.asarray(sigma2)
 
-def arch_recursion(double[::1] parameters,
-                   double[::1] resids,
+def arch_recursion(const double[::1] parameters,
+                   const double[::1] resids,
                    double[::1] sigma2,
                    int p,
                    int nobs,
                    double backcast,
-                   double[:, ::1] var_bounds):
+                   const double[:, ::1] var_bounds):
     """
     Parameters
     ----------
     parameters : 1-d array, float64
         Model parameters
     resids : 1-d array, float64
         Residuals to use in the recursion
@@ -182,19 +182,19 @@
                              resids[t - i - 1]
         bounds_check(&sigma2[t], &var_bounds[t, 0])
 
     return np.asarray(sigma2)
 
 def garch_core(
     Py_ssize_t t,
-    double[::1] parameters,
-    double[::1] resids,
+    const double[::1] parameters,
+    const double[::1] resids,
     double[::1] sigma2,
     double backcast,
-    double[:,::1] var_bounds,
+    const double[:,::1] var_bounds,
     int p,
     int o,
     int q,
     double power,
 ):
     """
     Compute variance recursion step for GARCH and related models
@@ -252,24 +252,24 @@
             sigma2[t] += parameters[loc] * sigma2[t - 1 - j]
         loc += 1
     bounds_check(&sigma2[t], &var_bounds[t, 0])
 
     return sigma2[t]
 
 
-def garch_recursion(double[::1] parameters,
-                    double[::1] fresids,
-                    double[::1] sresids,
+def garch_recursion(const double[::1] parameters,
+                    const double[::1] fresids,
+                    const double[::1] sresids,
                     double[::1] sigma2,
                     int p,
                     int o,
                     int q,
                     int nobs,
                     double backcast,
-                    double[:, ::1] var_bounds):
+                    const double[:, ::1] var_bounds):
     """
     Compute variance recursion for GARCH and related models
 
     Parameters
     ----------
     parameters : 1-d array, float64
         Model parameters
@@ -320,23 +320,23 @@
             else:
                 sigma2[t] += parameters[loc] * sigma2[t - 1 - j]
             loc += 1
         bounds_check(&sigma2[t], &var_bounds[t, 0])
 
     return np.asarray(sigma2)
 
-def egarch_recursion(double[::1] parameters,
-                     double[::1] resids,
+def egarch_recursion(const double[::1] parameters,
+                     const double[::1] resids,
                      double[::1] sigma2,
                      int p,
                      int o,
                      int q,
                      int nobs,
                      double backcast,
-                     double[:, ::1] var_bounds,
+                     const double[:, ::1] var_bounds,
                      double[::1] lnsigma2,
                      double[::1] std_resids,
                      double[::1] abs_std_resids):
     """
     Compute variance recursion for EGARCH models
 
     Parameters
@@ -401,17 +401,17 @@
         std_resids[t] = resids[t] / sqrt(sigma2[t])
         abs_std_resids[t] = fabs(std_resids[t])
 
     return np.asarray(sigma2)
 
 
 
-def midas_recursion(double[::1] parameters,
-                    double[::1] weights,
-                    double[::1] resids,
+def midas_recursion(const double[::1] parameters,
+                    const double[::1] weights,
+                    const double[::1] resids,
                     double[::1] sigma2,
                     int nobs,
                     double backcast,
                     double[:, ::1] var_bounds):
     """
     Parameters
     ----------
@@ -458,15 +458,15 @@
             else:
                 sigma2[t] +=  (aw[i] + 0.5 * gw[i]) * backcast
 
         bounds_check(&sigma2[t], &var_bounds[t, 0])
 
     return np.asarray(sigma2)
 
-cdef double[::1] _figarch_weights(double[::1] parameters,
+cdef double[::1] _figarch_weights(const double[::1] parameters,
                                   int p,
                                   int q,
                                   int trunc_lag):
 
     cdef double phi, d, beta
     cdef double [::1] lam, delta
     cdef Py_ssize_t i
@@ -483,20 +483,20 @@
     for i in range(1, trunc_lag):
         delta[i] = (i - d) / (i + 1) * delta[i - 1]
         lam[i] = beta * lam[i - 1] + (delta[i] - phi * delta[i - 1])
 
     return lam
 
 
-def figarch_weights(double[::1] parameters, int p, int q, int trunc_lag):
+def figarch_weights(const double[::1] parameters, int p, int q, int trunc_lag):
     return np.asarray(_figarch_weights(parameters, p, q, trunc_lag))
 
 
-def figarch_recursion(double[::1] parameters,
-                      double[::1] fresids,
+def figarch_recursion(const double[::1] parameters,
+                      const double[::1] fresids,
                       double[::1] sigma2,
                       int p,
                       int q,
                       int nobs,
                       int trunc_lag,
                       double backcast,
                       double[:, ::1] var_bounds):
@@ -516,25 +516,25 @@
         for i in range(min(t, trunc_lag)):
             sigma2[t] += lam[i] * fresids[t - i - 1]
         bounds_check(&sigma2[t], &var_bounds[t, 0])
 
     return np.asarray(sigma2)
 
 
-def aparch_recursion(double[::1] parameters,
-                    double[::1] resids,
-                    double[::1] abs_resids,
-                    double[::1] sigma2,
-                    double[::1] sigma_delta,
-                    int p,
-                    int o,
-                    int q,
-                    int nobs,
-                    double backcast,
-                    double[:, ::1] var_bounds):
+def aparch_recursion(const double[::1] parameters,
+                     const double[::1] resids,
+                     const double[::1] abs_resids,
+                     double[::1] sigma2,
+                     double[::1] sigma_delta,
+                     int p,
+                     int o,
+                     int q,
+                     int nobs,
+                     double backcast,
+                     const double[:, ::1] var_bounds):
     """
     Compute variance recursion for Asymmetric Power ARCH
 
     Parameters
     ----------
     parameters : ndarray
         Model parameters
@@ -585,55 +585,55 @@
     return np.asarray(sigma2)
 
 
 cdef class VolatilityUpdater:
     def __init__(self):
         pass
 
-    def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+    def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
         pass
 
     cdef void update(self,
                      Py_ssize_t t,
-                     double[::1] parameters,
-                     double[::1] resids,
+                     const double[::1] parameters,
+                     const double[::1] resids,
                      double[::1] sigma2,
-                     double[:,::1] var_bounds
+                     const double[:,::1] var_bounds
                      ):
         pass
 
     def _update_tester(self,
                        Py_ssize_t t,
-                       double[::1] parameters,
-                       double[::1] resids,
+                       const double[::1] parameters,
+                       const double[::1] resids,
                        double[::1] sigma2,
-                       double[:,::1] var_bounds):
+                       const double[:,::1] var_bounds):
         self.update(t, parameters, resids, sigma2, var_bounds)
 
 cdef class GARCHUpdater(VolatilityUpdater):
     cdef:
         int p, o, q
         double power, backcast
 
     def __init__(self, int p, int o, int q, double power):
         self.p = p
         self.o = o
         self.q = q
         self.power = power
         self.backcast = -1.0
 
-    def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+    def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
         self.backcast = backcast
 
     cdef void update(self,
                      Py_ssize_t t,
-                     double[::1] parameters,
-                     double[::1] resids,
+                     const double[::1] parameters,
+                     const double[::1] resids,
                      double[::1] sigma2,
-                     double[:,::1] var_bounds
+                     const double[:,::1] var_bounds
                      ):
         cdef:
             int p = self.p, o = self.o, q = self.q
             double power = self.power, backcast = self.backcast
             Py_ssize_t j, loc
 
         loc = 0
@@ -661,36 +661,36 @@
             else:
                 sigma2[t] += parameters[loc] * sigma2[t - 1 - j]
             loc += 1
         bounds_check(&sigma2[t], &var_bounds[t, 0])
 
 cdef class HARCHUpdater(VolatilityUpdater):
     cdef:
-        np.int32_t[::1] lags
+        const np.int32_t[::1] lags
         double backcast
 
-    def __init__(self, np.int32_t[::1] lags):
+    def __init__(self, const np.int32_t[::1] lags):
         self.lags = lags
         self.backcast = -1.0
 
     def __setstate__(self, state):
         self.backcast = state[0]
 
     def __reduce__(self):
         return HARCHUpdater, (np.asarray(self.lags),), (self.backcast,)
 
-    def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+    def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
         self.backcast = backcast
 
     cdef void update(self,
                      Py_ssize_t t,
-                     double[::1] parameters,
-                     double[::1] resids,
+                     const double[::1] parameters,
+                     const double[::1] resids,
                      double[::1] sigma2,
-                     double[:,::1] var_bounds
+                     const double[:,::1] var_bounds
                      ):
         cdef:
             double backcast = self.backcast
             Py_ssize_t i, j
             double param
 
         sigma2[t] = parameters[0]
@@ -711,39 +711,39 @@
         double backcast
 
     def __init__(self, object lam):
         self.estimate_lam = lam is None
         self.params = np.zeros(3)
         if lam is not None:
             self.params[1] = 1.0 - lam
-            self.params[2] =lam
+            self.params[2] = lam
 
     def __setstate__(self, state):
         cdef Py_ssize_t i
         self.backcast = state[0]
         params = state[1]
         for i in range(3):
             self.params[i] = params[i]
 
     def __reduce__(self):
         lam = None if self.estimate_lam else self.params[2]
         return EWMAUpdater, (lam,), (self.backcast, np.asarray(self.params))
 
-    def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+    def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
         if self.estimate_lam:
             self.params[1] = 1.0 - parameters[0]
             self.params[2] = parameters[0]
         self.backcast = backcast
 
     cdef void update(self,
                      Py_ssize_t t,
-                     double[::1] parameters,
-                     double[::1] resids,
+                     const double[::1] parameters,
+                     const double[::1] resids,
                      double[::1] sigma2,
-                     double[:,::1] var_bounds
+                     const double[:,::1] var_bounds
                      ):
 
         sigma2[t] = self.params[0]
         if t == 0:
             sigma2[t] += self.backcast
         else:
             sigma2[t] += (self.params[1] * resids[t-1] * resids[t-1] +
@@ -806,15 +806,15 @@
         for i in range(m):
             self.weights[i] = exp(lgamma(theta + j) - lgamma(j + 1) - lgamma(theta))
             sum_w += self.weights[i]
             j += 1.0
         for i in range(m):
             self.weights[i] /= sum_w
 
-    def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+    def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
         cdef double alpha, gamma, theta
 
         self.update_weights(parameters[2 + <int>self.asym])
         alpha = parameters[1]
         if self.asym:
             gamma = parameters[2]
         else:
@@ -825,18 +825,18 @@
             self.gw[i] = gamma * self.weights[i]
         self.backcast = backcast
         if self.resids2.shape[0] < nobs:
             self.resids2 = np.empty(nobs)
 
     cdef void update(self,
                      Py_ssize_t t,
-                     double[::1] parameters,
-                     double[::1] resids,
+                     const double[::1] parameters,
+                     const double[::1] resids,
                      double[::1] sigma2,
-                     double[:,::1] var_bounds
+                     const double[:,::1] var_bounds
                      ):
         cdef Py_ssize_t i
         cdef int j
         cdef double param, omega, alpha, gamma
 
         omega = parameters[0]
         if t > 0:
@@ -880,26 +880,26 @@
         assert self.fresids.shape[0] == temp.shape[0]
         for i in range(temp.shape[0]):
             self.fresids[i] = temp[i]
 
     def __reduce__(self):
         return FIGARCHUpdater, (self.p, self.q, self.power, self.truncation), (self.backcast, np.asarray(self.lam), np.asarray(self.fresids))
 
-    def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+    def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
         self.lam = _figarch_weights(parameters[1:], self.p, self.q, self.truncation)
         self.backcast = backcast
         if self.fresids.shape[0] < nobs:
             self.fresids = np.empty(nobs)
 
     cdef void update(self,
                      Py_ssize_t t,
-                     double[::1] parameters,
-                     double[::1] resids,
+                     const double[::1] parameters,
+                     const double[::1] resids,
                      double[::1] sigma2,
-                     double[:,::1] var_bounds
+                     const double[:,::1] var_bounds
                      ):
         cdef Py_ssize_t i
         cdef double bc1, bc2, bc_weight, omega, beta, omega_tilde
         cdef double [::1] lam
         cdef int p = self.p, q = self.q, trunc_lag = self.truncation
 
         omega = parameters[0]
@@ -961,18 +961,18 @@
                 self.backcast[i] = backcast
         else:
             for i in range(self.kmax):
                 self.backcast[i] = backcast[i]
 
     cdef void update(self,
                      Py_ssize_t t,
-                     double[::1] parameters,
-                     double[::1] resids,
+                     const double[::1] parameters,
+                     const double[::1] resids,
                      double[::1] sigma2,
-                     double[:,::1] var_bounds
+                     const double[:,::1] var_bounds
                      ):
         cdef:
             Py_ssize_t i
 
         sigma2[t] = 0.0
         if t > 0:
             for i in range(self.kmax):
@@ -1039,24 +1039,24 @@
 
     cdef void _resize(self, Py_ssize_t nobs):
         if self.lnsigma2.shape[0] < nobs:
             self.lnsigma2 = np.empty(nobs)
             self.abs_std_resids = np.empty(nobs)
             self.std_resids = np.empty(nobs)
 
-    def initialize_update(self, double[::1] parameters, object backcast, Py_ssize_t nobs):
+    def initialize_update(self, const double[::1] parameters, object backcast, Py_ssize_t nobs):
         self.backcast = backcast
         self._resize(nobs)
 
     cdef void update(self,
                      Py_ssize_t t,
-                     double[::1] parameters,
-                     double[::1] resids,
+                     const double[::1] parameters,
+                     const double[::1] resids,
                      double[::1] sigma2,
-                     double[:,::1] var_bounds
+                     const double[:,::1] var_bounds
                      ):
         cdef Py_ssize_t j, loc
 
         if t > 0:
             self.std_resids[t-1] = resids[t-1] / sqrt(sigma2[t-1])
             self.abs_std_resids[t-1] = fabs(self.std_resids[t-1])
 
@@ -1091,20 +1091,20 @@
     cdef:
         VolatilityUpdater volatility_updater
 
     def __init__(self, VolatilityUpdater updater):
         self.volatility_updater = updater
 
     def recursion(self,
-                  double[::1] y,
-                  double[:,::1] x,
-                  double[::1] mean_parameters,
-                  double[::1] variance_params,
+                  const double[::1] y,
+                  const double[:,::1] x,
+                  const double[::1] mean_parameters,
+                  const double[::1] variance_params,
                   double[::1] sigma2,
-                  double[:,::1] var_bounds,
+                  const double[:,::1] var_bounds,
                   double power):
         cdef:
             Py_ssize_t t, i, nobs = y.shape[0], k = x.shape[1]
             double[::1] resids = np.empty(nobs)
             double gamma = mean_parameters[k]
 
         for t in range(nobs):
```

### Comparing `arch-5.4.0/arch/univariate/recursions_python.py` & `arch-5.5.0/arch/univariate/recursions_python.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/univariate/volatility.py` & `arch-5.5.0/arch/univariate/volatility.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
         """
         Compute the variance for a single observation
 
         Parameters
         ----------
         index : int
             The numerical index of the variance to compute
-        variance_params : ndarray
+        parameters : ndarray
             The variance model parameters
         resids :
             The residual array. Only uses ``resids[:index]`` when computing
             ``sigma2[index]``
         sigma2 : ndarray
             The array containing the variances. Only uses ``sigma2[:index]``
             when computing ``sigma2[index]``. The computed value is stored
@@ -982,14 +982,16 @@
 
     .. math::
 
         \sigma_{t}^{\lambda}=\omega
         + \sum_{i=1}^{p}\alpha_{i}\left|\epsilon_{t-i}\right|^{\lambda}
         +\sum_{j=1}^{o}\gamma_{j}\left|\epsilon_{t-j}\right|^{\lambda}
         I\left[\epsilon_{t-j}<0\right]+\sum_{k=1}^{q}\beta_{k}\sigma_{t-k}^{\lambda}
+
+    where :math:`\lambda` is the ``power``.
     """
 
     def __init__(self, p: int = 1, o: int = 0, q: int = 1, power: float = 2.0) -> None:
         super().__init__()
         self.p: int = int(p)
         self.o: int = int(o)
         self.q: int = int(q)
@@ -1421,15 +1423,15 @@
     In a Heterogeneous ARCH process, variance dynamics are
 
     .. math::
 
         \sigma_{t}^{2}=\omega + \sum_{i=1}^{m}\alpha_{l_{i}}
         \left(l_{i}^{-1}\sum_{j=1}^{l_{i}}\epsilon_{t-j}^{2}\right)
 
-    In the common case where lags=[1,5,22], the model is
+    In the common case where ``lags=[1,5,22]``, the model is
 
     .. math::
 
         \sigma_{t}^{2}=\omega+\alpha_{1}\epsilon_{t-1}^{2}
         +\alpha_{5} \left(\frac{1}{5}\sum_{j=1}^{5}\epsilon_{t-j}^{2}\right)
         +\alpha_{22} \left(\frac{1}{22}\sum_{j=1}^{22}\epsilon_{t-j}^{2}\right)
```

### Comparing `arch-5.4.0/arch/utility/__init__.py` & `arch-5.5.0/arch/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/utility/array.py` & `arch-5.5.0/arch/utility/array.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/utility/cov.py` & `arch-5.5.0/arch/utility/cov.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from numpy import asarray
+from numpy import asarray, squeeze
 
 from arch.typing import Float64Array
 
 
 def cov_nw(
     y: Float64Array, lags: int = 0, demean: bool = True, axis: int = 0, ddof: int = 0
 ) -> Float64Array | float:
@@ -55,9 +55,9 @@
     cov = z.T.dot(z)
     for j in range(1, lags + 1):
         w = 1 - j / (lags + 1)
         gamma = z[j:].T.dot(z[:-j])
         cov += w * (gamma + gamma.T)
     cov = cov / (n - ddof)
     if is_1d:
-        return float(cov)
+        return float(squeeze(cov))
     return asarray(cov)
```

### Comparing `arch-5.4.0/arch/utility/exceptions.py` & `arch-5.5.0/arch/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/utility/io.py` & `arch-5.5.0/arch/utility/io.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/utility/testing.py` & `arch-5.5.0/arch/utility/testing.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/utility/timeseries.py` & `arch-5.5.0/arch/utility/timeseries.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch/vendor/property_cached.py` & `arch-5.5.0/arch/vendor/property_cached.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/arch.egg-info/PKG-INFO` & `arch-5.5.0/arch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arch
-Version: 5.4.0
+Version: 5.5.0
 Summary: ARCH for Python
 Home-page: https://github.com/bashtage/arch
 Author: Kevin Sheppard
 Author-email: kevin.sheppard@economics.ox.ac.uk
 License: NCSA
 Keywords: arch,ARCH,variance,econometrics,volatility,finance,GARCH,bootstrap,random walk,unit root,Dickey Fuller,time series,confidence intervals,multiple comparisons,Reality Check,SPA,StepM
 Classifier: Development Status :: 5 - Production/Stable
@@ -298,15 +298,15 @@
 ### Developing
 
 The development requirements are:
 
 - Cython (0.29+, if not using ARCH_NO_BINARY=1)
 - pytest (For tests)
 - sphinx (to build docs)
-- sphinx_material (to build docs)
+- sphinx-immaterial (to build docs)
 - jupyter, notebook and nbsphinx (to build docs)
 
 ### Installation Notes
 
 1. If Cython is not installed, the package will be installed
     as-if `ARCH_NO_BINARY=1` was set.
 2. Setup does not verify these requirements. Please ensure these are
```

### Comparing `arch-5.4.0/arch.egg-info/SOURCES.txt` & `arch-5.5.0/arch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/azure-pipelines.yml` & `arch-5.5.0/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/ci/azure/azure_template_posix.yml` & `arch-5.5.0/ci/azure/azure_template_posix.yml`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,17 @@
       python38_numpy118:
         python.version: '3.8'
         MATPLOTLIB: 3.3.0
         NUMPY: 1.19.0
         PANDAS: 1.1.0
       python_311:
         python.version: '3.11'
+      python_311_copy_on_write:
+        python.version: '3.11'
+        ARCH_TEST_COPY_ON_WRITE: 1
       python_310:
         python.version: '3.10'
         test.install: true
       python_39_no_binary:
         python.version: '3.9'
         ARCH_NO_BINARY: true
         PYTEST_OPTS: '--skip-slow'
```

### Comparing `arch-5.4.0/ci/azure/azure_template_windows.yml` & `arch-5.5.0/ci/azure/azure_template_windows.yml`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/ci/azure/install-posix.sh` & `arch-5.5.0/ci/azure/install-posix.sh`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/ci/github-actions/push-docs-gh-pages.sh` & `arch-5.5.0/ci/github-actions/push-docs-gh-pages.sh`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/Makefile` & `arch-5.5.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/make.bat` & `arch-5.5.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/_static/images/android-chrome-192x192.png` & `arch-5.5.0/doc/source/_static/images/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/_static/images/android-chrome-512x512.png` & `arch-5.5.0/doc/source/_static/images/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/_static/images/apple-touch-icon.png` & `arch-5.5.0/doc/source/_static/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/_static/images/color-logo-256.png` & `arch-5.5.0/doc/source/_static/images/color-logo-256.png`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/_static/images/favicon-16x16.png` & `arch-5.5.0/doc/source/_static/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/_static/images/favicon-32x32.png` & `arch-5.5.0/doc/source/_static/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/_static/images/mstile-150x150.png` & `arch-5.5.0/doc/source/_static/images/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/_static/images/safari-pinned-tab.svg` & `arch-5.5.0/doc/source/_static/images/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/_templates/autosummary/class.rst` & `arch-5.5.0/doc/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/_templates/layout.html` & `arch-5.5.0/doc/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/api.rst` & `arch-5.5.0/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/bootstrap/background.rst` & `arch-5.5.0/doc/source/bootstrap/background.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/bootstrap/bootstrap.rst` & `arch-5.5.0/doc/source/bootstrap/bootstrap.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/bootstrap/bootstrap_histogram.png` & `arch-5.5.0/doc/source/bootstrap/bootstrap_histogram.png`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/bootstrap/confidence-intervals.rst` & `arch-5.5.0/doc/source/bootstrap/confidence-intervals.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/bootstrap/iid-bootstraps.rst` & `arch-5.5.0/doc/source/bootstrap/iid-bootstraps.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/bootstrap/low-level-interface.rst` & `arch-5.5.0/doc/source/bootstrap/low-level-interface.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/bootstrap/parameter-covariance-estimation.rst` & `arch-5.5.0/doc/source/bootstrap/parameter-covariance-estimation.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/bootstrap/semiparametric-parametric-bootstrap.rst` & `arch-5.5.0/doc/source/bootstrap/semiparametric-parametric-bootstrap.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/bootstrap/timeseries-bootstraps.rst` & `arch-5.5.0/doc/source/bootstrap/timeseries-bootstraps.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/changes/3.0.txt` & `arch-5.5.0/doc/source/changes/3.0.txt`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/changes/4.0.txt` & `arch-5.5.0/doc/source/changes/4.0.txt`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/changes/5.0.txt` & `arch-5.5.0/doc/source/changes/5.0.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 Version 5
 =========
 
+Release 5.5
+===========
+- NumPy 1.25 fixes
+- Initial pandas copy-on-write support
+- Switched doc theme to sphinx-immaterial
+- Small fixes for typing issues
+
 Release 5.4
 ===========
 - Compatability release with pandas 2.0
 - Add testing and wheel support for Python 3.11
 
 Release 5.3
 ===========
```

### Comparing `arch-5.4.0/doc/source/conf.py` & `arch-5.5.0/doc/source/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,20 +11,14 @@
 import shutil
 from typing import Dict, List
 
 from packaging.version import parse
 
 import arch
 
-on_rtd = os.environ.get("READTHEDOCS", None) == "True"
-# If extensions (or modules to document with autodoc) are in another directory,
-# add these directories to sys.path here. If the directory is relative to the
-# documentation root, use os.path.abspath to make it absolute, like shown here.
-# sys.path.insert(0, os.path.abspath("."))
-
 ##########################################################
 # Copy Examples
 ##########################################################
 root = os.path.split(os.path.abspath(__file__))[0]
 example_path = os.path.join(root, "..", "..", "examples")
 examples = glob.glob(os.path.join(example_path, "*.ipynb"))
 for example in examples:
@@ -40,17 +34,17 @@
 author = "Kevin Sheppard"
 nitpicky = True
 
 # The short X.Y version
 full_version = parse(arch.__version__)
 short_version = version = arch.__version__
 if full_version.is_devrelease:
-    short_version = f"v{full_version.base_version} (+{full_version.dev})"
-# The full version, including alpha/beta/rc tags.
-release = arch.__version__
+    release = f"v{full_version.base_version} (+{full_version.dev})"
+else:
+    release = short_version
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = "1.0"
 
@@ -64,20 +58,21 @@
     "sphinx.ext.todo",
     "sphinx.ext.doctest",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinx.ext.viewcode",
     "sphinx.ext.coverage",
     "sphinx.ext.ifconfig",
-    "numpydoc",
-    # "sphinx.ext.napoleon",
+    # "numpydoc",
+    "sphinx.ext.napoleon",
     "sphinx_autodoc_typehints",
     "IPython.sphinxext.ipython_console_highlighting",
     "IPython.sphinxext.ipython_directive",
     "nbsphinx",
+    "sphinx_immaterial",
 ]
 
 try:
     import sphinxcontrib.spelling  # noqa: F401
 except ImportError as err:  # noqa: F841
     pass
 else:
@@ -116,79 +111,94 @@
 pygments_style = "colorful"  # "sphinx"
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "default"
-# on_rtd is whether we are on readthedocs.org
-if not on_rtd:  # only import and set the theme if we"re building docs locally
-    import sphinx_material
-
-    # Adds an HTML table visitor to apply Bootstrap table classes
-    html_theme_path = sphinx_material.html_theme_path()
-    html_context = sphinx_material.get_html_context()
-    html_theme = "sphinx_material"
-
-    # Register the theme as an extension to generate a sitemap.xml
-    extensions.append("sphinx_material")
-
-    # sphinx_material theme options (see theme.conf for more information)
-    html_theme_options = {
-        "base_url": "https://bashtage.github.io/arch/",
-        "repo_url": "https://github.com/bashtage/arch/",
-        "repo_name": "ARCH",
-        # Set the name of the project to appear in the sidebar
-        "nav_title": project + " " + short_version,
-        "globaltoc_depth": 2,
-        "globaltoc_collapse": True,
-        "globaltoc_includehidden": True,
-        "theme_color": "#2196f3",
-        "color_primary": "blue ",
-        "color_accent": "indigo",
-        "html_minify": True,
-        "css_minify": True,
-        "master_doc": False,
-        "version_dropdown": True,
-        "version_info": {
-            "Release": "https://bashtage.github.io/arch/",
-            "Development": "https://bashtage.github.io/arch/devel/",
-            "RTD (Release)": "https://arch.readthedocs.io/",
+# Adds an HTML table visitor to apply Bootstrap table classes
+html_theme = "sphinx_immaterial"
+html_title = f"{project} {release}"
+# sphinx_immaterial theme options
+html_theme_options = {
+    "icon": {
+        "repo": "fontawesome/brands/github"
+    },
+
+    "site_url": "https://bashtage.github.io/arch/",
+    "repo_url": "https://github.com/bashtage/arch/",
+    "repo_name": "arch",
+    "repo_type": "github",
+    "palette": {"primary": "blue", "accent": "indigo"},
+    "globaltoc_collapse": True,
+    "toc_title": "Contents",
+    "version_dropdown": True,
+    "version_info": [
+        {
+            "version": "https://bashtage.github.io/arch/",
+            "title": "Release",
+            "aliases": [],
+        },
+        {
+            "version": "https://bashtage.github.io/arch/devel/",
+            "title": "Development",
+            "aliases": [],
+        },
+        {
+            "title": "RTD (Release)",
+            "version": "https://arch.readthedocs.io/",
+            "aliases": [],
+        },
+    ],
+    "toc_title_is_page_title": True,
+    "social": [
+        {
+            "icon": "fontawesome/brands/github",
+            "link": "https://github.com/bashtage/arch",
+            "name": "Source on github.com",
         },
-    }
+        {
+            "icon": "fontawesome/brands/python",
+            "link": "https://pypi.org/project/arch/",
+        },
+        {
+            "icon": "fontawesome/solid/quote-left",
+            "link": "https://doi.org/10.5281/zenodo.593254",
+        },
+    ],
+    #        "globaltoc_depth": 2,
+    #        "globaltoc_includehidden": True,
+}
 
 html_favicon = "images/favicon.ico"
 html_logo = "images/bw-logo.svg"
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-if not on_rtd:
-    html_static_path = ["_static"]
-    html_css_files = ["css/small_fixes.css"]
+html_static_path = ["_static"]
+html_css_files = ["css/small_fixes.css"]
 
 # Custom sidebar templates, must be a dictionary that maps document names
 # to template names.
 #
 # The default sidebars (for documents that don"t match any pattern) are
 # defined by theme itself.  Builtin themes are using these templates by
 # default: ``["localtoc.html", "relations.html", "sourcelink.html",
 # "searchbox.html"]``.
 #
 # html_sidebars = {}
-if not on_rtd:
-    html_sidebars = {
+html_sidebars = {
         "**": ["logo-text.html", "globaltoc.html", "searchbox.html", "localtoc.html"]
-    }
+}
 
 # If false, no module index is generated.
 html_domain_indices = True
 
 # -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
@@ -286,11 +296,14 @@
 
 numpydoc_xref_aliases = {
     "Figure": "matplotlib.figure.Figure",
     "Axes": "matplotlib.axes.Axes",
     "AxesSubplot": "matplotlib.axes.Axes",
     "DataFrame": "pandas.DataFrame",
     "Series": "pandas.Series",
+    "ndarray": "numpy.ndarray",
+    "RandomState": "numpy.random.RandomState",
+    "VarianceForecast": "arch.univariate.volatility.VarianceForecast",
 }
 
 autosummary_generate = True
 autoclass_content = "class"
```

### Comparing `arch-5.4.0/doc/source/covariance/covariance.rst` & `arch-5.5.0/doc/source/covariance/covariance.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/images/bw-logo.svg` & `arch-5.5.0/doc/source/images/bw-logo.svg`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/images/color-logo-no-text.svg` & `arch-5.5.0/doc/source/images/color-logo-no-text.svg`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/images/color-logo-unprocessed.svg` & `arch-5.5.0/doc/source/images/color-logo-unprocessed.svg`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/images/color-logo.png` & `arch-5.5.0/doc/source/images/color-logo.png`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/images/color-logo.svg` & `arch-5.5.0/doc/source/images/color-logo.svg`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/images/favicon.ico` & `arch-5.5.0/doc/source/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/images/favicon.png` & `arch-5.5.0/doc/source/images/favicon.png`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/images/favicon.py` & `arch-5.5.0/doc/source/images/favicon.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/images/favicon.svg` & `arch-5.5.0/doc/source/images/favicon.svg`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/images/hero.png` & `arch-5.5.0/doc/source/images/hero.png`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/images/hero.py` & `arch-5.5.0/doc/source/images/hero.py`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/images/hero.svg` & `arch-5.5.0/doc/source/images/hero.svg`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/images/logo.svg` & `arch-5.5.0/doc/source/images/logo.svg`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/index.rst` & `arch-5.5.0/doc/source/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+:hero: Univariate volatility modeling, bootstrapping, multiple comparison procedures and unit root tests.
+
 .. image:: images/color-logo.svg
    :width: 33.3%
    :alt: arch logo
 
 .. note::
 
   `Stable documentation <https://bashtage.github.io/arch/>`_ for the latest release
```

### Comparing `arch-5.4.0/doc/source/multiple-comparison/background.rst` & `arch-5.5.0/doc/source/multiple-comparison/background.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/multiple-comparison/multiple-comparison-reference.rst` & `arch-5.5.0/doc/source/multiple-comparison/multiple-comparison-reference.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/multiple-comparison/multiple-comparisons.rst` & `arch-5.5.0/doc/source/multiple-comparison/multiple-comparisons.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/spelling_wordlist.txt` & `arch-5.5.0/doc/source/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/unitroot/cointegration.rst` & `arch-5.5.0/doc/source/unitroot/cointegration.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/unitroot/introduction.rst` & `arch-5.5.0/doc/source/unitroot/introduction.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/unitroot/unitroot.rst` & `arch-5.5.0/doc/source/unitroot/unitroot.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/univariate/distribution.rst` & `arch-5.5.0/doc/source/univariate/distribution.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/univariate/forecasting.rst` & `arch-5.5.0/doc/source/univariate/forecasting.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/univariate/introduction.rst` & `arch-5.5.0/doc/source/univariate/introduction.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/univariate/mean.rst` & `arch-5.5.0/doc/source/univariate/mean.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/univariate/univariate.rst` & `arch-5.5.0/doc/source/univariate/univariate.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/doc/source/univariate/volatility.rst` & `arch-5.5.0/doc/source/univariate/volatility.rst`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/examples/bootstrap_examples.ipynb` & `arch-5.5.0/examples/bootstrap_examples.ipynb`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/examples/multiple-comparison_examples.ipynb` & `arch-5.5.0/examples/multiple-comparison_examples.ipynb`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/examples/unitroot_cointegration_examples.ipynb` & `arch-5.5.0/examples/unitroot_cointegration_examples.ipynb`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/examples/unitroot_examples.ipynb` & `arch-5.5.0/examples/unitroot_examples.ipynb`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/examples/univariate_forecasting_with_exogenous_variables.ipynb` & `arch-5.5.0/examples/univariate_forecasting_with_exogenous_variables.ipynb`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/examples/univariate_using_fixed_variance.ipynb` & `arch-5.5.0/examples/univariate_using_fixed_variance.ipynb`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/examples/univariate_volatility_forecasting.ipynb` & `arch-5.5.0/examples/univariate_volatility_forecasting.ipynb`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/examples/univariate_volatility_modeling.ipynb` & `arch-5.5.0/examples/univariate_volatility_modeling.ipynb`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/examples/univariate_volatility_scenarios.ipynb` & `arch-5.5.0/examples/univariate_volatility_scenarios.ipynb`

 * *Files identical despite different names*

### Comparing `arch-5.4.0/setup.cfg` & `arch-5.5.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 	error:Values in x were outside bounds:RuntimeWarning:
 	error:The random_state property is deprecated:FutureWarning
 	error:random_state is deprecated:FutureWarning
 	error:seed is deprecated:FutureWarning
 	error:get_state is deprecated:FutureWarning
 	error:Passing None has been deprecated:pytest.PytestRemovedIn8Warning:
 	error:y is poorly scaled:arch.utility.exceptions.DataScaleWarning:
+	error:Conversion of an array with ndim:DeprecationWarning:arch
 markers = 
 	slow: mark a test as slow
 
 [isort]
 sections = FUTURE,COMPAT,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER
 known_first_party = arch
 known_third_party = Cython,numpy,matplotlib,pandas,patsy,pytest,statsmodels,seaborn
```

### Comparing `arch-5.4.0/setup.py` & `arch-5.5.0/setup.py`

 * *Files identical despite different names*

