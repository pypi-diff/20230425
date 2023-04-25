# Comparing `tmp/copulas-0.8.0.dev0.tar.gz` & `tmp/copulas-0.8.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copulas-0.8.0.dev0.tar", last modified: Thu Jan  5 18:22:13 2023, max compression
+gzip compressed data, was "copulas-0.8.1.dev0.tar", last modified: Tue Apr 25 09:57:38 2023, max compression
```

## Comparing `copulas-0.8.0.dev0.tar` & `copulas-0.8.1.dev0.tar`

### file list

```diff
@@ -1,222 +1,224 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.288625 copulas-0.8.0.dev0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6966 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9383 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4822 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    15606 2023-01-05 18:22:13.288793 copulas-0.8.0.dev0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5226 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6616 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.256563 copulas-0.8.0.dev0/copulas/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6945 2023-01-05 18:21:47.000000 copulas-0.8.0.dev0/copulas/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.259158 copulas-0.8.0.dev0/copulas/bivariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5087 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/bivariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13952 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/bivariate/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4536 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/bivariate/clayton.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4641 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/bivariate/frank.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4216 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/bivariate/gumbel.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2069 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/bivariate/independence.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      347 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/bivariate/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6831 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/datasets.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.260021 copulas-0.8.0.dev0/copulas/multivariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      362 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/multivariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5600 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/multivariate/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11381 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/multivariate/gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22020 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/multivariate/tree.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12913 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/multivariate/vine.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.260198 copulas-0.8.0.dev0/copulas/optimize/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4927 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/optimize/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.262624 copulas-0.8.0.dev0/copulas/univariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      825 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/univariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19976 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/univariate/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1016 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/univariate/beta.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      906 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/univariate/gamma.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      728 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/univariate/gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6093 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/univariate/gaussian_kde.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      921 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/univariate/log_laplace.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      944 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/univariate/selection.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      823 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/univariate/student_t.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1932 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/univariate/truncated_gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      754 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/univariate/uniform.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4665 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/copulas/visualization.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.257669 copulas-0.8.0.dev0/copulas.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    15606 2023-01-05 18:22:13.000000 copulas-0.8.0.dev0/copulas.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7597 2023-01-05 18:22:13.000000 copulas-0.8.0.dev0/copulas.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-01-05 18:22:13.000000 copulas-0.8.0.dev0/copulas.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-01-05 18:22:13.000000 copulas-0.8.0.dev0/copulas.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1702 2023-01-05 18:22:13.000000 copulas-0.8.0.dev0/copulas.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        8 2023-01-05 18:22:13.000000 copulas-0.8.0.dev0/copulas.egg-info/top_level.txt
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.264054 copulas-0.8.0.dev0/docs/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      608 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/docs/Makefile
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       28 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/docs/authors.rst
--rwxr-xr-x   0 andrewmontanez   (501) staff       (20)     5852 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/docs/conf.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/docs/contributing.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       29 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/docs/history.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.267344 copulas-0.8.0.dev0/docs/images/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    15307 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/docs/images/copulas-200.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    26688 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/docs/images/copulas.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    52079 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/docs/images/copulas_sample_dataset.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   886153 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/docs/images/dai-logo-white.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4753 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/docs/images/dice_cdf.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    23772 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/docs/images/pdf_cdf.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9447 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/docs/images/pit.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   128308 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/docs/images/quickstart.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      651 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/docs/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       29 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/docs/install.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      769 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/docs/make.bat
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1446 2023-01-05 18:22:13.289340 copulas-0.8.0.dev0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4029 2023-01-05 18:21:47.000000 copulas-0.8.0.dev0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.267858 copulas-0.8.0.dev0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4710 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.268664 copulas-0.8.0.dev0/tests/end-to-end/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1663 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.268981 copulas-0.8.0.dev0/tests/end-to-end/bivariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       51 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/bivariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1301 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/bivariate/test_base.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.269700 copulas-0.8.0.dev0/tests/end-to-end/multivariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       54 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/multivariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1146 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/multivariate/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6948 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/multivariate/test_gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1910 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/multivariate/test_vine.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1670 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      184 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/test_visualization.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.270848 copulas-0.8.0.dev0/tests/end-to-end/univariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/univariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5170 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/univariate/test_beta.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5090 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/univariate/test_gamma.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5032 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/univariate/test_gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5576 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/univariate/test_gaussian_kde.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5210 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/univariate/test_student_t.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5276 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/end-to-end/univariate/test_truncated_gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9510 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/large_scale_evaluation.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.271138 copulas-0.8.0.dev0/tests/numerical/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3795 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       40 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.271454 copulas-0.8.0.dev0/tests/numerical/cdf/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       44 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.271675 copulas-0.8.0.dev0/tests/numerical/cdf/input/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/input/bivariate_cdf_input.csv
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.274530 copulas-0.8.0.dev0/tests/numerical/cdf/output/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_1_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_2_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      220 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_3_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      220 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_3_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      220 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/output/frank_cdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      220 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/output/frank_cdf_test_case_1_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      223 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/output/frank_cdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      223 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/output/frank_cdf_test_case_2_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/output/frank_cdf_test_case_3_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/output/frank_cdf_test_case_3_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      216 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/output/gumbel_cdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      216 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/output/gumbel_cdf_test_case_1_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      217 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/output/gumbel_cdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      217 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/output/gumbel_cdf_test_case_2_output_R.csv
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.274999 copulas-0.8.0.dev0/tests/numerical/cdf/scripts/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      604 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/scripts/bivariate_cdf_input.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2090 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/scripts/bivariate_cdf_output.R
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1678 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/scripts/bivariate_cdf_output.m
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.252910 copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.275500 copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/clayton/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      808 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      744 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_2.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      743 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_3.json
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.275974 copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/frank/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      733 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      737 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_2.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      733 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_3.json
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.276301 copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/gumbel/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      738 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      738 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_2.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1077 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/cdf/test_cdf.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.276631 copulas-0.8.0.dev0/tests/numerical/fit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       44 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/fit/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.276956 copulas-0.8.0.dev0/tests/numerical/fit/input/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       54 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/fit/input/bivariate_fit_test_case_1_input.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       72 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/fit/input/bivariate_fit_test_case_2_input.csv
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.277258 copulas-0.8.0.dev0/tests/numerical/fit/scripts/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1008 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/fit/scripts/bivariate_fit_output.R
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      780 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/fit/scripts/bivariate_fit_output.m
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.253343 copulas-0.8.0.dev0/tests/numerical/fit/test_cases/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.277576 copulas-0.8.0.dev0/tests/numerical/fit/test_cases/clayton/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      826 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      828 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_2.json
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.277924 copulas-0.8.0.dev0/tests/numerical/fit/test_cases/frank/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      820 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      820 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_2.json
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.278254 copulas-0.8.0.dev0/tests/numerical/fit/test_cases/gumbel/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      823 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      823 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_2.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      966 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/fit/test_fit.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.278626 copulas-0.8.0.dev0/tests/numerical/pdf/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       44 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.278825 copulas-0.8.0.dev0/tests/numerical/pdf/input/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/input/bivariate_pdf_input.csv
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.281345 copulas-0.8.0.dev0/tests/numerical/pdf/output/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_1_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_2_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_3_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_3_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/output/frank_pdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/output/frank_pdf_test_case_1_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      214 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/output/frank_pdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      214 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/output/frank_pdf_test_case_2_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      208 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/output/frank_pdf_test_case_3_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      208 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/output/frank_pdf_test_case_3_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/output/gumbel_pdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/output/gumbel_pdf_test_case_1_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/output/gumbel_pdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/output/gumbel_pdf_test_case_2_output_R.csv
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.281856 copulas-0.8.0.dev0/tests/numerical/pdf/scripts/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      603 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/scripts/bivariate_pdf_input.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2070 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/scripts/bivariate_pdf_output.R
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1694 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/scripts/bivariate_pdf_output.m
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.253833 copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.282438 copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/clayton/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      743 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      744 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_2.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      743 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_3.json
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.282908 copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/frank/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      733 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      737 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_2.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      733 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_3.json
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.283216 copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/gumbel/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      738 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      738 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_2.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1086 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/numerical/pdf/test_pdf.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.283600 copulas-0.8.0.dev0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.284939 copulas-0.8.0.dev0/tests/unit/bivariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/bivariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      490 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/bivariate/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3907 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/bivariate/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3549 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/bivariate/test_clayton.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3583 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/bivariate/test_frank.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3567 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/bivariate/test_gumbel.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1412 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/bivariate/test_independence.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.285956 copulas-0.8.0.dev0/tests/unit/multivariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       48 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/multivariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      382 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/multivariate/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18716 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/multivariate/test_gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    24177 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/multivariate/test_tree.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6015 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/multivariate/test_vine.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.286361 copulas-0.8.0.dev0/tests/unit/optimize/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       53 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/optimize/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      899 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/optimize/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12972 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/test___init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-05 18:22:13.288465 copulas-0.8.0.dev0/tests/unit/univariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       46 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/univariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7497 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/univariate/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2432 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/univariate/test_beta.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1428 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/univariate/test_gamma.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1305 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/univariate/test_gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6788 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/univariate/test_gaussian_kde.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1412 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/univariate/test_log_laplace.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3059 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/univariate/test_selection.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1197 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/univariate/test_student_t.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1532 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/univariate/test_truncated_gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1387 2023-01-05 18:17:33.000000 copulas-0.8.0.dev0/tests/unit/univariate/test_uniform.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.896158 copulas-0.8.1.dev0/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       60 2023-04-25 09:51:55.000000 copulas-0.8.1.dev0/AUTHORS.rst
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     6966 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/CONTRIBUTING.rst
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     9846 2023-04-25 09:51:55.000000 copulas-0.8.1.dev0/HISTORY.md
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     4822 2023-04-25 09:51:55.000000 copulas-0.8.1.dev0/LICENSE
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      284 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/MANIFEST.in
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)    18980 2023-04-25 09:57:38.896158 copulas-0.8.1.dev0/PKG-INFO
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     5226 2023-04-25 09:51:55.000000 copulas-0.8.1.dev0/README.md
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     6616 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/RELEASE.md
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.880158 copulas-0.8.1.dev0/copulas/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     7052 2023-04-25 09:51:55.000000 copulas-0.8.1.dev0/copulas/__init__.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      823 2023-04-25 09:51:55.000000 copulas-0.8.1.dev0/copulas/_addons.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.880158 copulas-0.8.1.dev0/copulas/bivariate/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     5087 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/bivariate/__init__.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)    13952 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/copulas/bivariate/base.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     4536 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/bivariate/clayton.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     4641 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/bivariate/frank.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     4216 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/bivariate/gumbel.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     2069 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/bivariate/independence.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      347 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/bivariate/utils.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     6831 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/copulas/datasets.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.880158 copulas-0.8.1.dev0/copulas/multivariate/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      362 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/multivariate/__init__.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     5600 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/copulas/multivariate/base.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)    11166 2023-04-25 09:51:55.000000 copulas-0.8.1.dev0/copulas/multivariate/gaussian.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)    22020 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/multivariate/tree.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)    12913 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/copulas/multivariate/vine.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.880158 copulas-0.8.1.dev0/copulas/optimize/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     4927 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/optimize/__init__.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.880158 copulas-0.8.1.dev0/copulas/univariate/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      825 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/univariate/__init__.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)    19976 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/copulas/univariate/base.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1016 2022-06-07 13:22:39.000000 copulas-0.8.1.dev0/copulas/univariate/beta.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      906 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/univariate/gamma.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      728 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/univariate/gaussian.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     6093 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/copulas/univariate/gaussian_kde.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      921 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/univariate/log_laplace.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      944 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/univariate/selection.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      823 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/univariate/student_t.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1932 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/copulas/univariate/truncated_gaussian.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      754 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/univariate/uniform.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     4665 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/copulas/visualization.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.880158 copulas-0.8.1.dev0/copulas.egg-info/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)    18980 2023-04-25 09:57:38.000000 copulas-0.8.1.dev0/copulas.egg-info/PKG-INFO
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     7643 2023-04-25 09:57:38.000000 copulas-0.8.1.dev0/copulas.egg-info/SOURCES.txt
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)        1 2023-04-25 09:57:38.000000 copulas-0.8.1.dev0/copulas.egg-info/dependency_links.txt
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)        1 2023-04-25 09:57:38.000000 copulas-0.8.1.dev0/copulas.egg-info/not-zip-safe
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1693 2023-04-25 09:57:38.000000 copulas-0.8.1.dev0/copulas.egg-info/requires.txt
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)        8 2023-04-25 09:57:38.000000 copulas-0.8.1.dev0/copulas.egg-info/top_level.txt
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.884158 copulas-0.8.1.dev0/docs/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      608 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/docs/Makefile
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       28 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/docs/authors.rst
+-rwxrwxr-x   0 pacho     (1000) pacho     (1000)     5852 2023-04-25 09:51:55.000000 copulas-0.8.1.dev0/docs/conf.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       33 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/docs/contributing.rst
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       29 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/docs/history.rst
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.884158 copulas-0.8.1.dev0/docs/images/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)    15307 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/docs/images/copulas-200.png
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)    26688 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/docs/images/copulas.png
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)    52079 2023-04-25 09:51:55.000000 copulas-0.8.1.dev0/docs/images/copulas_sample_dataset.png
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)   886153 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/docs/images/dai-logo-white.png
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     4753 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/docs/images/dice_cdf.png
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)    23772 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/docs/images/pdf_cdf.png
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     9447 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/docs/images/pit.png
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)   128308 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/docs/images/quickstart.png
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      651 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/docs/index.rst
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       29 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/docs/install.rst
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      769 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/docs/make.bat
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1446 2023-04-25 09:57:38.896158 copulas-0.8.1.dev0/setup.cfg
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     4020 2023-04-25 09:51:55.000000 copulas-0.8.1.dev0/setup.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.884158 copulas-0.8.1.dev0/tests/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     4710 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/__init__.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.884158 copulas-0.8.1.dev0/tests/end-to-end/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1663 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/end-to-end/README.md
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       41 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/end-to-end/__init__.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.884158 copulas-0.8.1.dev0/tests/end-to-end/bivariate/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       51 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/tests/end-to-end/bivariate/__init__.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1301 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/tests/end-to-end/bivariate/test_base.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.884158 copulas-0.8.1.dev0/tests/end-to-end/multivariate/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       54 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/end-to-end/multivariate/__init__.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1146 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/tests/end-to-end/multivariate/test_base.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     6948 2022-06-07 13:22:39.000000 copulas-0.8.1.dev0/tests/end-to-end/multivariate/test_gaussian.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1910 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/end-to-end/multivariate/test_vine.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1670 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/tests/end-to-end/test___init__.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      184 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/end-to-end/test_visualization.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.884158 copulas-0.8.1.dev0/tests/end-to-end/univariate/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       52 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/end-to-end/univariate/__init__.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     5170 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/tests/end-to-end/univariate/test_beta.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     5090 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/tests/end-to-end/univariate/test_gamma.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     5032 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/tests/end-to-end/univariate/test_gaussian.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     5576 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/tests/end-to-end/univariate/test_gaussian_kde.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     5210 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/tests/end-to-end/univariate/test_student_t.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     5276 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/tests/end-to-end/univariate/test_truncated_gaussian.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     9510 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/large_scale_evaluation.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.888158 copulas-0.8.1.dev0/tests/numerical/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     3795 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/README.md
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       40 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/numerical/__init__.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.888158 copulas-0.8.1.dev0/tests/numerical/cdf/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       44 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/numerical/cdf/__init__.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.888158 copulas-0.8.1.dev0/tests/numerical/cdf/input/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      120 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/input/bivariate_cdf_input.csv
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.888158 copulas-0.8.1.dev0/tests/numerical/cdf/output/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      219 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_1_output_Matlab.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      219 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_1_output_R.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      218 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_2_output_Matlab.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      218 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_2_output_R.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      220 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_3_output_Matlab.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      220 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_3_output_R.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      220 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/output/frank_cdf_test_case_1_output_Matlab.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      220 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/output/frank_cdf_test_case_1_output_R.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      223 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/output/frank_cdf_test_case_2_output_Matlab.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      223 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/output/frank_cdf_test_case_2_output_R.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      219 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/output/frank_cdf_test_case_3_output_Matlab.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      219 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/output/frank_cdf_test_case_3_output_R.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      216 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/output/gumbel_cdf_test_case_1_output_Matlab.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      216 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/output/gumbel_cdf_test_case_1_output_R.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      217 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/output/gumbel_cdf_test_case_2_output_Matlab.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      217 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/output/gumbel_cdf_test_case_2_output_R.csv
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.888158 copulas-0.8.1.dev0/tests/numerical/cdf/scripts/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      604 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/numerical/cdf/scripts/bivariate_cdf_input.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     2090 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/scripts/bivariate_cdf_output.R
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1678 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/scripts/bivariate_cdf_output.m
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.876158 copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.888158 copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/clayton/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      808 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_1.json
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      744 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_2.json
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      743 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_3.json
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.888158 copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/frank/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      733 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_1.json
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      737 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_2.json
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      733 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_3.json
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.888158 copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/gumbel/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      738 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_1.json
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      738 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_2.json
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1077 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/numerical/cdf/test_cdf.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.888158 copulas-0.8.1.dev0/tests/numerical/fit/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       44 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/numerical/fit/__init__.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.888158 copulas-0.8.1.dev0/tests/numerical/fit/input/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       54 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/fit/input/bivariate_fit_test_case_1_input.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       72 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/fit/input/bivariate_fit_test_case_2_input.csv
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.888158 copulas-0.8.1.dev0/tests/numerical/fit/scripts/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1008 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/fit/scripts/bivariate_fit_output.R
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      780 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/fit/scripts/bivariate_fit_output.m
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.876158 copulas-0.8.1.dev0/tests/numerical/fit/test_cases/
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.888158 copulas-0.8.1.dev0/tests/numerical/fit/test_cases/clayton/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      826 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_1.json
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      828 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_2.json
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.888158 copulas-0.8.1.dev0/tests/numerical/fit/test_cases/frank/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      820 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_1.json
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      820 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_2.json
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.888158 copulas-0.8.1.dev0/tests/numerical/fit/test_cases/gumbel/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      823 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_1.json
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      823 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_2.json
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      966 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/numerical/fit/test_fit.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.892158 copulas-0.8.1.dev0/tests/numerical/pdf/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       44 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/numerical/pdf/__init__.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.892158 copulas-0.8.1.dev0/tests/numerical/pdf/input/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      120 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/input/bivariate_pdf_input.csv
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.892158 copulas-0.8.1.dev0/tests/numerical/pdf/output/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      211 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_1_output_Matlab.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      211 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_1_output_R.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      212 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_2_output_Matlab.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      212 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_2_output_R.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      212 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_3_output_Matlab.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      212 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_3_output_R.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      211 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/output/frank_pdf_test_case_1_output_Matlab.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      211 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/output/frank_pdf_test_case_1_output_R.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      214 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/output/frank_pdf_test_case_2_output_Matlab.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      214 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/output/frank_pdf_test_case_2_output_R.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      208 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/output/frank_pdf_test_case_3_output_Matlab.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      208 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/output/frank_pdf_test_case_3_output_R.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      212 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/output/gumbel_pdf_test_case_1_output_Matlab.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      212 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/output/gumbel_pdf_test_case_1_output_R.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      218 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/output/gumbel_pdf_test_case_2_output_Matlab.csv
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      218 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/output/gumbel_pdf_test_case_2_output_R.csv
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.892158 copulas-0.8.1.dev0/tests/numerical/pdf/scripts/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      603 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/numerical/pdf/scripts/bivariate_pdf_input.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     2070 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/scripts/bivariate_pdf_output.R
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1694 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/scripts/bivariate_pdf_output.m
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.876158 copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.892158 copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/clayton/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      743 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_1.json
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      744 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_2.json
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      743 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_3.json
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.892158 copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/frank/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      733 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_1.json
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      737 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_2.json
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      733 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_3.json
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.892158 copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/gumbel/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      738 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_1.json
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      738 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_2.json
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1086 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/numerical/pdf/test_pdf.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.892158 copulas-0.8.1.dev0/tests/unit/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       35 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/unit/__init__.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.892158 copulas-0.8.1.dev0/tests/unit/bivariate/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       45 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/unit/bivariate/__init__.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      490 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/unit/bivariate/test___init__.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     3907 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/tests/unit/bivariate/test_base.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     3549 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/unit/bivariate/test_clayton.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     3583 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/unit/bivariate/test_frank.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     3567 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/unit/bivariate/test_gumbel.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1412 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/unit/bivariate/test_independence.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.892158 copulas-0.8.1.dev0/tests/unit/multivariate/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       48 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/unit/multivariate/__init__.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      382 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/tests/unit/multivariate/test_base.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)    18721 2023-04-25 09:51:55.000000 copulas-0.8.1.dev0/tests/unit/multivariate/test_gaussian.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)    24177 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/unit/multivariate/test_tree.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     6015 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/tests/unit/multivariate/test_vine.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.896158 copulas-0.8.1.dev0/tests/unit/optimize/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       53 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/tests/unit/optimize/__init__.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)      899 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/unit/optimize/test___init__.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)    12972 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/tests/unit/test___init__.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1379 2023-04-25 09:51:55.000000 copulas-0.8.1.dev0/tests/unit/test__addons.py
+drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2023-04-25 09:57:38.896158 copulas-0.8.1.dev0/tests/unit/univariate/
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)       46 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/unit/univariate/__init__.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     7497 2022-04-28 14:45:42.000000 copulas-0.8.1.dev0/tests/unit/univariate/test_base.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     2432 2022-06-07 13:22:39.000000 copulas-0.8.1.dev0/tests/unit/univariate/test_beta.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1428 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/unit/univariate/test_gamma.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1305 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/unit/univariate/test_gaussian.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     6788 2021-11-24 16:22:24.000000 copulas-0.8.1.dev0/tests/unit/univariate/test_gaussian_kde.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1412 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/unit/univariate/test_log_laplace.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     3059 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/unit/univariate/test_selection.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1197 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/unit/univariate/test_student_t.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1532 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/unit/univariate/test_truncated_gaussian.py
+-rw-rw-r--   0 pacho     (1000) pacho     (1000)     1387 2021-11-05 09:20:41.000000 copulas-0.8.1.dev0/tests/unit/univariate/test_uniform.py
```

### Comparing `copulas-0.8.0.dev0/CONTRIBUTING.rst` & `copulas-0.8.1.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/HISTORY.md` & `copulas-0.8.1.dev0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # History
 
+## v0.8.0 - 2023-01-06
+
+This release adds support for python 3.10 and 3.11. Additionally, it drops support for python 3.6.
+
+### Maintenance
+
+* Support python 3.10 and above - PR[#338](https://github.com/sdv-dev/Copulas/pull/338) by @pvk-developer
+* Copulas Package Maintenance Updates - Issue[#336](https://github.com/sdv-dev/Copulas/issues/336) by @pvk-developer
+* Add support for python 3.10 - PR[#329](https://github.com/sdv-dev/Copulas/pull/329) by @katxiao
+
 ## v0.7.0 - 2022-05-10
 
 This release adds `gaussian` as a fallback distribution in case the user specified one fails. It also improves the `fit` of the `beta` distribution by properly estimatig the `loc` and `scale` parameters.
 
 ### General Improvements
 
 * Add gaussian as fallback - Issue[#320](https://github.com/sdv-dev/Copulas/issues/320) by @fealho
```

### Comparing `copulas-0.8.0.dev0/LICENSE` & `copulas-0.8.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/PKG-INFO` & `copulas-0.8.1.dev0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,384 @@
 Metadata-Version: 2.1
 Name: copulas
-Version: 0.8.0.dev0
+Version: 0.8.1.dev0
 Summary: Create tabular synthetic data using copulas-based modeling.
 Home-page: https://github.com/sdv-dev/Copulas
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
+Description: <div align="center">
+        <br/>
+        <p align="center">
+            <i>This repository is part of <a href="https://sdv.dev">The Synthetic Data Vault Project</a>, a project from <a href="https://datacebo.com">DataCebo</a>.</i>
+        </p>
+        
+        [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--%20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
+        [![PyPi Shield](https://img.shields.io/pypi/v/copulas.svg)](https://pypi.python.org/pypi/copulas)
+        [![Downloads](https://pepy.tech/badge/copulas)](https://pepy.tech/project/copulas)
+        [![Unit Tests](https://github.com/sdv-dev/Copulas/actions/workflows/unit.yml/badge.svg)](https://github.com/sdv-dev/Copulas/actions/workflows/unit.yml)
+        [![Coverage Status](https://codecov.io/gh/sdv-dev/Copulas/branch/master/graph/badge.svg)](https://codecov.io/gh/sdv-dev/Copulas)
+        [![Slack](https://img.shields.io/badge/Community-Slack-blue?style=plastic&logo=slack)](https://bit.ly/sdv-slack-invite)
+        
+        <div align="left">
+        <br/>
+        <p align="center">
+        <a href="https://github.com/sdv-dev/Copulas">
+        <img align="center" width=40% src="https://github.com/sdv-dev/SDV/blob/master/docs/images/Copulas-DataCebo.png"></img>
+        </a>
+        </p>
+        </div>
+        
+        </div>
+        
+        # Overview
+        
+        **Copulas** is a Python library for modeling multivariate distributions and sampling from them
+        using copula functions.
+        Given a table of numerical data, use Copulas to learn the distribution and
+        generate new synthetic data following the same statistical properties.
+        
+        **Key Features:**
+        
+        * **Model multivariate data.** Choose from a variety of univariate
+        distributions and copulas – including Archimedian Copulas, Gaussian Copulas and Vine Copulas.
+        
+        * **Compare real and synthetic data visually** after building your model. Visualizations
+        are available as 1D histograms, 2D scatterplots and 3D scatterplots.
+        
+        * **Access & manipulate learned parameters.** With complete access to the internals
+        of the model, set or tune parameters to your choosing.
+        
+        # Install
+        
+        Install the Copulas library using pip or conda.
+        
+        ```bash
+        pip install copulas
+        ```
+        
+        ```bash
+        conda install -c conda-forge copulas
+        ```
+        
+        # Usage
+        
+        Get started using a demo dataset. This dataset contains 3 numerical columns.
+        
+        ```python
+        from copulas.datasets import sample_trivariate_xyz
+        
+        real_data = sample_trivariate_xyz()
+        real_data.head()
+        ```
+        
+        <img src="docs/images/copulas_sample_dataset.png" width="300">
+        
+        Model the data using a copula and use it to create synthetic data.
+        The Copulas library offers many options including Gaussian Copula,
+        Vine Copulas and Archimedian Copulas.
+        
+        ```python
+        from copulas.multivariate import GaussianMultivariate
+        
+        copula = GaussianMultivariate()
+        copula.fit(real_data)
+        
+        synthetic_data = copula.sample(len(real_data))
+        ```
+        
+        Visualize the real and synthetic data side-by-side. Let's do this in 3D so see our full dataset.
+        
+        ```python
+        from copulas.visualization import compare_3d
+        
+        compare_3d(real_data, synthetic_data)
+        ```
+        
+        ![Quickstart](docs/images/quickstart.png)
+        
+        # Tutorials
+        Click below to run the code yourself on a Colab Notebook and discover new features.
+        
+        [![Tutorial Notebook](https://img.shields.io/badge/Tutorial-Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252)](https://bit.ly/copulas-demo)
+        
+        # Community & Support
+        
+        Learn more about Copulas library from our [documentation](https://sdv.dev/Copulas/) site.
+        
+        **Questions or issues?** Join our [Slack channel](https://bit.ly/sdv-slack-invite)
+        to discuss more about Copulas and synthetic data.
+        If you find a bug or have a feature request, you can also
+        [open an issue](https://github.com/sdv-dev/Copulas/issues/new/choose) on our GitHub.
+        
+        **Interested in contributing to Copulas?** Read our
+        [Contribution Guide](https://sdv.dev/Copulas/contributing.html) to get started.
+        
+        # Credits
+        
+        The Copulas open source project first started at the Data to AI Lab at MIT in 2018.
+        Thank you to our team of contributors who have built and maintained the library over the years!
+        
+        [View Contributors](https://github.com/sdv-dev/Copulas/graphs/contributors)
+        
+        ---
+        
+        
+        <div align="center">
+        <a href="https://datacebo.com"><img align="center" width=40% src="https://github.com/sdv-dev/SDV/blob/master/docs/images/DataCebo.png"></img></a>
+        </div>
+        <br/>
+        <br/>
+        
+        [The Synthetic Data Vault Project](https://sdv.dev) was first created at MIT's [Data to AI Lab](
+        https://dai.lids.mit.edu/) in 2016. After 4 years of research and traction with enterprise, we
+        created [DataCebo](https://datacebo.com) in 2020 with the goal of growing the project.
+        Today, DataCebo is the proud developer of SDV, the largest ecosystem for
+        synthetic data generation & evaluation. It is home to multiple libraries that support synthetic
+        data, including:
+        
+        * 🔄 Data discovery & transformation. Reverse the transforms to reproduce realistic data.
+        * 🧠 Multiple machine learning models -- ranging from Copulas to Deep Learning -- to create tabular,
+          multi table and time series data.
+        * 📊 Measuring quality and privacy of synthetic data, and comparing different synthetic data
+          generation models.
+        
+        [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
+        integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
+        for specific needs.
+        
+        
+        # History
+        
+        ## v0.8.0 - 2023-01-06
+        
+        This release adds support for python 3.10 and 3.11. Additionally, it drops support for python 3.6.
+        
+        ### Maintenance
+        
+        * Support python 3.10 and above - PR[#338](https://github.com/sdv-dev/Copulas/pull/338) by @pvk-developer
+        * Copulas Package Maintenance Updates - Issue[#336](https://github.com/sdv-dev/Copulas/issues/336) by @pvk-developer
+        * Add support for python 3.10 - PR[#329](https://github.com/sdv-dev/Copulas/pull/329) by @katxiao
+        
+        ## v0.7.0 - 2022-05-10
+        
+        This release adds `gaussian` as a fallback distribution in case the user specified one fails. It also improves the `fit` of the `beta` distribution by properly estimatig the `loc` and `scale` parameters.
+        
+        ### General Improvements
+        
+        * Add gaussian as fallback - Issue[#320](https://github.com/sdv-dev/Copulas/issues/320) by @fealho
+        * Improve the fit of the Beta distribution: Use the new loc and scale - Issue[#317](https://github.com/sdv-dev/Copulas/issues/317) by @pvk-developer
+        
+        ## v0.6.1 - 2022-02-25
+        
+        This release improves the `random_state` functionality by taking in RandomState objects in addition to
+        random seeds.
+        
+        ### General Improvements
+        
+        * Use random_state instead of random_seed - Issue[#113](https://github.com/sdv-dev/Copulas/issues/113) by @katxiao
+        
+        ## v0.6.0 - 2021-05-13
+        
+        This release makes Copulas compatible with Python 3.9! It also improves library maintenance by
+        updating dependencies, reorganizing the CI workflows, adding pip check to the workflows and
+        removing unused files.
+        
+        ### General Improvements
+        
+        * Add support for Python 3.9 - Issue[#282](https://github.com/sdv-dev/Copulas/issues/282) by @amontanez24
+        * Remove entry point in setup.py - Issue[#280](https://github.com/sdv-dev/Copulas/issues/280) by @amontanez24
+        * Update pandas dependency range - Issue[#266](https://github.com/sdv-dev/Copulas/issues/266) by @katxiao
+        * Fix repository language - Issue[#272](https://github.com/sdv-dev/Copulas/issues/272) by @pvk-developer
+        * Add pip check to CI workflows - Issue[#274](https://github.com/sdv-dev/Copulas/issues/274) by @pvk-developer
+        * Reorganize workflows and add codecov - PR[#267](https://github.com/sdv-dev/Copulas/pull/267) by @csala
+        * Constrain jinja2 versions - PR[#269](https://github.com/sdv-dev/Copulas/pull/269/files) by @fealho
+        
+        ## v0.5.1 - 2021-08-13
+        
+        This release improves performance by changing the way scipy stats is used,
+        calling their methods directly without creating intermediate instances.
+        
+        It also fixes a bug introduced by the scipy 1.7.0 release where some
+        distributions fail to fit because scipy validates the learned parameters.
+        
+        ### Issues Closed
+         * Exception: Optimization converged to parameters that are outside the range allowed by the distribution. - Issue [#264](https://github.com/sdv-dev/Copulas/issues/264) by @csala
+         * Use scipy stats models directly without creating instances - Issue [#261](https://github.com/sdv-dev/Copulas/issues/261) by @csala
+        
+        ## v0.5.0 - 2021-01-24
+        
+        This release introduces conditional sampling for the GaussianMultivariate modeling.
+        The new conditioning feature allows passing a dictionary with the values to use to condition
+        the rest of the columns.
+        
+        It also fixes a bug that prevented constant distributions to be restored from a dictionary
+        and updates some dependencies.
+        
+        ### New Features
+        
+        * Conditional sampling from Gaussian copula - Issue [#154](https://github.com/sdv-dev/Copulas/issues/154) by @csala
+        
+        ### Bug Fixes
+        
+        * ScipyModel subclasses fail to restore constant values when using `from_dict` - Issue [#212](https://github.com/sdv-dev/Copulas/issues/212) by @csala
+        
+        ## v0.4.0 - 2021-01-27
+        
+        This release introduces a few changes to optimize processing speed by re-implementing
+        the Gaussian KDE pdf to use vectorized root finding methods and also adding the option
+        to subsample the data during univariate selection.
+        
+        ### General Improvements
+        
+        * Make `gaussian_kde` faster - Issue [#200](https://github.com/sdv-dev/Copulas/issues/200) by @k15z and @fealho
+        * Use sub-sampling in `select_univariate` - Issue [#183](https://github.com/sdv-dev/Copulas/issues/183) by @csala
+        
+        ## v0.3.3 - 2020-09-18
+        
+        ### General Improvements
+        
+        * Use `corr` instead of `cov` in the GaussianMultivariate - Issue [#195](https://github.com/sdv-dev/Copulas/issues/195) by @rollervan
+        * Add arguments to GaussianKDE - Issue [#181](https://github.com/sdv-dev/Copulas/issues/181) by @rollervan
+        
+        ### New Features
+        
+        * Log Laplace Distribution - Issue [#188](https://github.com/sdv-dev/Copulas/issues/188) by @rollervan
+        
+        ## v0.3.2 - 2020-08-08
+        
+        ### General Improvements
+        
+        * Support Python 3.8 - Issue [#185](https://github.com/sdv-dev/Copulas/issues/185) by @csala
+        * Support scipy >1.3 - Issue [#180](https://github.com/sdv-dev/Copulas/issues/180) by @csala
+        
+        ### New Features
+        
+        * Add Uniform Univariate - Issue [#179](https://github.com/sdv-dev/Copulas/issues/179) by @rollervan
+        
+        ## v0.3.1 - 2020-07-09
+        
+        ### General Improvements
+        
+        * Raise numpy version upper bound to 2 - Issue [#178](https://github.com/sdv-dev/Copulas/issues/178) by @csala
+        
+        ### New Features
+        
+        * Add Student T Univariate - Issue [#172](https://github.com/sdv-dev/Copulas/issues/172) by @gbonomib
+        
+        ### Bug Fixes
+        
+        * Error in Quickstarts : Unknown projection '3d' - Issue [#174](https://github.com/sdv-dev/Copulas/issues/174) by @csala
+        
+        ## v0.3.0 - 2020-03-27
+        
+        Important revamp of the internal implementation of the project, the testing
+        infrastructure and the documentation by Kevin Alex Zhang @k15z, Carles Sala
+        @csala and Kalyan Veeramachaneni @kveerama
+        
+        ### Enhancements
+        
+        * Reimplementation of the existing Univariate distributions.
+        * Addition of new Beta and Gamma Univariates.
+        * New Univariate API with automatic selection of the optimal distribution.
+        * Several improvements and fixes on the Bivariate and Multivariate Copulas implementation.
+        * New visualization module with simple plotting patterns to visualize probability distributions.
+        * New datasets module with toy datasets sampling functions.
+        * New testing infrastructure with end-to-end, numerical and large scale testing.
+        * Improved tutorials and documentation.
+        
+        ## v0.2.5 - 2020-01-17
+        
+        ### General Improvements
+        
+        * Convert import_object to get_instance - Issue [#114](https://github.com/sdv-dev/Copulas/issues/114) by @JDTheRipperPC
+        
+        ## v0.2.4 - 2019-12-23
+        
+        ### New Features
+        
+        * Allow creating copula classes directly - Issue [#117](https://github.com/sdv-dev/Copulas/issues/117) by @csala
+        
+        ### General Improvements
+        
+        * Remove `select_copula` from `Bivariate` - Issue [#118](https://github.com/sdv-dev/Copulas/issues/118) by @csala
+        * Rename TruncNorm to TruncGaussian and make it non standard - Issue [#102](https://github.com/sdv-dev/Copulas/issues/102) by @csala @JDTheRipperPC
+        
+        ### Bugs fixed
+        
+        * Error on Frank and Gumble sampling - Issue [#112](https://github.com/sdv-dev/Copulas/issues/112) by @csala
+        
+        ## v0.2.3 - 2019-09-17
+        
+        ### New Features
+        
+        * Add support to Python 3.7 - Issue [#53](https://github.com/sdv-dev/Copulas/issues/53) by @JDTheRipperPC
+        
+        ### General Improvements
+        
+        * Document RELEASE workflow - Issue [#105](https://github.com/sdv-dev/Copulas/issues/105) by @JDTheRipperPC
+        * Improve serialization of univariate distributions - Issue [#99](https://github.com/sdv-dev/Copulas/issues/99) by @ManuelAlvarezC and @JDTheRipperPC
+        
+        ### Bugs fixed
+        
+        * The method 'select_copula' of Bivariate return wrong CopulaType - Issue [#101](https://github.com/sdv-dev/Copulas/issues/101) by @JDTheRipperPC
+        
+        ## v0.2.2 - 2019-07-31
+        
+        ### New Features
+        
+        * `truncnorm` distribution and a generic wrapper for `scipy.rv_continous` distributions - Issue [#27](https://github.com/sdv-dev/Copulas/issues/27) by @amontanez, @csala and @ManuelAlvarezC
+        * `Independence` bivariate copulas - Issue [#46](https://github.com/sdv-dev/Copulas/issues/46) by @aliciasun, @csala and @ManuelAlvarezC
+        * Option to select seed on random number generator - Issue [#63](https://github.com/sdv-dev/Copulas/issues/63) by @echo66 and @ManuelAlvarezC
+        * Option on Vine copulas to select number of rows to sample - Issue [#77](https://github.com/sdv-dev/Copulas/issues/77) by @ManuelAlvarezC
+        * Make copulas accept both scalars and arrays as arguments - Issues [#85](https://github.com/sdv-dev/Copulas/issues/85) and [#90](https://github.com/sdv-dev/Copulas/issues/90) by @ManuelAlvarezC
+        
+        ### General Improvements
+        
+        * Ability to properly handle constant data - Issues [#57](https://github.com/sdv-dev/Copulas/issues/57) and [#82](https://github.com/sdv-dev/Copulas/issues/82) by @csala and @ManuelAlvarezC
+        * Tests for analytics properties of copulas - Issue [#61](https://github.com/sdv-dev/Copulas/issues/61) by @ManuelAlvarezC
+        * Improved documentation - Issue [#96](https://github.com/sdv-dev/Copulas/issues/96) by @ManuelAlvarezC
+        
+        ### Bugs fixed
+        
+        * Fix bug on Vine copulas, that made it crash during the bivariate copula selection - Issue [#64](https://github.com/sdv-dev/Copulas/issues/64) by @echo66 and @ManuelAlvarezC
+        
+        ## v0.2.1 - Vine serialization
+        
+        * Add serialization to Vine copulas.
+        * Add `distribution` as argument for the Gaussian Copula.
+        * Improve Bivariate Copulas code structure to remove code duplication.
+        * Fix bug in Vine Copulas sampling: 'Edge' object has no attribute 'index'
+        * Improve code documentation.
+        * Improve code style and linting tools configuration.
+        
+        ## v0.2.0 - Unified API
+        
+        * New API for stats methods.
+        * Standarize input and output to `numpy.ndarray`.
+        * Increase unittest coverage to 90%.
+        * Add methods to load/save copulas.
+        * Improve Gaussian copula sampling accuracy.
+        
+        ## v0.1.1 - Minor Improvements
+        
+        * Different Copula types separated in subclasses
+        * Extensive Unit Testing
+        * More pythonic names in the public API.
+        * Stop using third party elements that will be deprected soon.
+        * Add methods to sample new data on bivariate copulas.
+        * New KDE Univariate copula
+        * Improved examples with additional demo data.
+        
+        ## v0.1.0 - First Release
+        
+        * First release on PyPI.
+        
 Keywords: copulas
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -19,366 +387,7 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7,<3.12
 Description-Content-Type: text/markdown
 Provides-Extra: tutorials
 Provides-Extra: test
 Provides-Extra: dev
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-<div align="center">
-<br/>
-<p align="center">
-    <i>This repository is part of <a href="https://sdv.dev">The Synthetic Data Vault Project</a>, a project from <a href="https://datacebo.com">DataCebo</a>.</i>
-</p>
-
-[![Development Status](https://img.shields.io/badge/Development%20Status-2%20--%20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
-[![PyPi Shield](https://img.shields.io/pypi/v/copulas.svg)](https://pypi.python.org/pypi/copulas)
-[![Downloads](https://pepy.tech/badge/copulas)](https://pepy.tech/project/copulas)
-[![Unit Tests](https://github.com/sdv-dev/Copulas/actions/workflows/unit.yml/badge.svg)](https://github.com/sdv-dev/Copulas/actions/workflows/unit.yml)
-[![Coverage Status](https://codecov.io/gh/sdv-dev/Copulas/branch/master/graph/badge.svg)](https://codecov.io/gh/sdv-dev/Copulas)
-[![Slack](https://img.shields.io/badge/Community-Slack-blue?style=plastic&logo=slack)](https://bit.ly/sdv-slack-invite)
-
-<div align="left">
-<br/>
-<p align="center">
-<a href="https://github.com/sdv-dev/Copulas">
-<img align="center" width=40% src="https://github.com/sdv-dev/SDV/blob/master/docs/images/Copulas-DataCebo.png"></img>
-</a>
-</p>
-</div>
-
-</div>
-
-# Overview
-
-**Copulas** is a Python library for modeling multivariate distributions and sampling from them
-using copula functions.
-Given a table of numerical data, use Copulas to learn the distribution and
-generate new synthetic data following the same statistical properties.
-
-**Key Features:**
-
-* **Model multivariate data.** Choose from a variety of univariate
-distributions and copulas – including Archimedian Copulas, Gaussian Copulas and Vine Copulas.
-
-* **Compare real and synthetic data visually** after building your model. Visualizations
-are available as 1D histograms, 2D scatterplots and 3D scatterplots.
-
-* **Access & manipulate learned parameters.** With complete access to the internals
-of the model, set or tune parameters to your choosing.
-
-# Install
-
-Install the Copulas library using pip or conda.
-
-```bash
-pip install copulas
-```
-
-```bash
-conda install -c conda-forge copulas
-```
-
-# Usage
-
-Get started using a demo dataset. This dataset contains 3 numerical columns.
-
-```python
-from copulas.datasets import sample_trivariate_xyz
-
-real_data = sample_trivariate_xyz()
-real_data.head()
-```
-
-<img src="docs/images/copulas_sample_dataset.png" width="300">
-
-Model the data using a copula and use it to create synthetic data.
-The Copulas library offers many options including Gaussian Copula,
-Vine Copulas and Archimedian Copulas.
-
-```python
-from copulas.multivariate import GaussianMultivariate
-
-copula = GaussianMultivariate()
-copula.fit(real_data)
-
-synthetic_data = copula.sample(len(real_data))
-```
-
-Visualize the real and synthetic data side-by-side. Let's do this in 3D so see our full dataset.
-
-```python
-from copulas.visualization import compare_3d
-
-compare_3d(real_data, synthetic_data)
-```
-
-![Quickstart](docs/images/quickstart.png)
-
-# Tutorials
-Click below to run the code yourself on a Colab Notebook and discover new features.
-
-[![Tutorial Notebook](https://img.shields.io/badge/Tutorial-Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252)](https://bit.ly/copulas-demo)
-
-# Community & Support
-
-Learn more about Copulas library from our [documentation](https://sdv.dev/Copulas/) site.
-
-**Questions or issues?** Join our [Slack channel](https://bit.ly/sdv-slack-invite)
-to discuss more about Copulas and synthetic data.
-If you find a bug or have a feature request, you can also
-[open an issue](https://github.com/sdv-dev/Copulas/issues/new/choose) on our GitHub.
-
-**Interested in contributing to Copulas?** Read our
-[Contribution Guide](https://sdv.dev/Copulas/contributing.html) to get started.
-
-# Credits
-
-The Copulas open source project first started at the Data to AI Lab at MIT in 2018.
-Thank you to our team of contributors who have built and maintained the library over the years!
-
-[View Contributors](https://github.com/sdv-dev/Copulas/graphs/contributors)
-
----
-
-
-<div align="center">
-<a href="https://datacebo.com"><img align="center" width=40% src="https://github.com/sdv-dev/SDV/blob/master/docs/images/DataCebo.png"></img></a>
-</div>
-<br/>
-<br/>
-
-[The Synthetic Data Vault Project](https://sdv.dev) was first created at MIT's [Data to AI Lab](
-https://dai.lids.mit.edu/) in 2016. After 4 years of research and traction with enterprise, we
-created [DataCebo](https://datacebo.com) in 2020 with the goal of growing the project.
-Today, DataCebo is the proud developer of SDV, the largest ecosystem for
-synthetic data generation & evaluation. It is home to multiple libraries that support synthetic
-data, including:
-
-* 🔄 Data discovery & transformation. Reverse the transforms to reproduce realistic data.
-* 🧠 Multiple machine learning models -- ranging from Copulas to Deep Learning -- to create tabular,
-  multi table and time series data.
-* 📊 Measuring quality and privacy of synthetic data, and comparing different synthetic data
-  generation models.
-
-[Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
-integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
-for specific needs.
-
-
-# History
-
-## v0.7.0 - 2022-05-10
-
-This release adds `gaussian` as a fallback distribution in case the user specified one fails. It also improves the `fit` of the `beta` distribution by properly estimatig the `loc` and `scale` parameters.
-
-### General Improvements
-
-* Add gaussian as fallback - Issue[#320](https://github.com/sdv-dev/Copulas/issues/320) by @fealho
-* Improve the fit of the Beta distribution: Use the new loc and scale - Issue[#317](https://github.com/sdv-dev/Copulas/issues/317) by @pvk-developer
-
-## v0.6.1 - 2022-02-25
-
-This release improves the `random_state` functionality by taking in RandomState objects in addition to
-random seeds.
-
-### General Improvements
-
-* Use random_state instead of random_seed - Issue[#113](https://github.com/sdv-dev/Copulas/issues/113) by @katxiao
-
-## v0.6.0 - 2021-05-13
-
-This release makes Copulas compatible with Python 3.9! It also improves library maintenance by
-updating dependencies, reorganizing the CI workflows, adding pip check to the workflows and
-removing unused files.
-
-### General Improvements
-
-* Add support for Python 3.9 - Issue[#282](https://github.com/sdv-dev/Copulas/issues/282) by @amontanez24
-* Remove entry point in setup.py - Issue[#280](https://github.com/sdv-dev/Copulas/issues/280) by @amontanez24
-* Update pandas dependency range - Issue[#266](https://github.com/sdv-dev/Copulas/issues/266) by @katxiao
-* Fix repository language - Issue[#272](https://github.com/sdv-dev/Copulas/issues/272) by @pvk-developer
-* Add pip check to CI workflows - Issue[#274](https://github.com/sdv-dev/Copulas/issues/274) by @pvk-developer
-* Reorganize workflows and add codecov - PR[#267](https://github.com/sdv-dev/Copulas/pull/267) by @csala
-* Constrain jinja2 versions - PR[#269](https://github.com/sdv-dev/Copulas/pull/269/files) by @fealho
-
-## v0.5.1 - 2021-08-13
-
-This release improves performance by changing the way scipy stats is used,
-calling their methods directly without creating intermediate instances.
-
-It also fixes a bug introduced by the scipy 1.7.0 release where some
-distributions fail to fit because scipy validates the learned parameters.
-
-### Issues Closed
- * Exception: Optimization converged to parameters that are outside the range allowed by the distribution. - Issue [#264](https://github.com/sdv-dev/Copulas/issues/264) by @csala
- * Use scipy stats models directly without creating instances - Issue [#261](https://github.com/sdv-dev/Copulas/issues/261) by @csala
-
-## v0.5.0 - 2021-01-24
-
-This release introduces conditional sampling for the GaussianMultivariate modeling.
-The new conditioning feature allows passing a dictionary with the values to use to condition
-the rest of the columns.
-
-It also fixes a bug that prevented constant distributions to be restored from a dictionary
-and updates some dependencies.
-
-### New Features
-
-* Conditional sampling from Gaussian copula - Issue [#154](https://github.com/sdv-dev/Copulas/issues/154) by @csala
-
-### Bug Fixes
-
-* ScipyModel subclasses fail to restore constant values when using `from_dict` - Issue [#212](https://github.com/sdv-dev/Copulas/issues/212) by @csala
-
-## v0.4.0 - 2021-01-27
-
-This release introduces a few changes to optimize processing speed by re-implementing
-the Gaussian KDE pdf to use vectorized root finding methods and also adding the option
-to subsample the data during univariate selection.
-
-### General Improvements
-
-* Make `gaussian_kde` faster - Issue [#200](https://github.com/sdv-dev/Copulas/issues/200) by @k15z and @fealho
-* Use sub-sampling in `select_univariate` - Issue [#183](https://github.com/sdv-dev/Copulas/issues/183) by @csala
-
-## v0.3.3 - 2020-09-18
-
-### General Improvements
-
-* Use `corr` instead of `cov` in the GaussianMultivariate - Issue [#195](https://github.com/sdv-dev/Copulas/issues/195) by @rollervan
-* Add arguments to GaussianKDE - Issue [#181](https://github.com/sdv-dev/Copulas/issues/181) by @rollervan
-
-### New Features
-
-* Log Laplace Distribution - Issue [#188](https://github.com/sdv-dev/Copulas/issues/188) by @rollervan
-
-## v0.3.2 - 2020-08-08
-
-### General Improvements
-
-* Support Python 3.8 - Issue [#185](https://github.com/sdv-dev/Copulas/issues/185) by @csala
-* Support scipy >1.3 - Issue [#180](https://github.com/sdv-dev/Copulas/issues/180) by @csala
-
-### New Features
-
-* Add Uniform Univariate - Issue [#179](https://github.com/sdv-dev/Copulas/issues/179) by @rollervan
-
-## v0.3.1 - 2020-07-09
-
-### General Improvements
-
-* Raise numpy version upper bound to 2 - Issue [#178](https://github.com/sdv-dev/Copulas/issues/178) by @csala
-
-### New Features
-
-* Add Student T Univariate - Issue [#172](https://github.com/sdv-dev/Copulas/issues/172) by @gbonomib
-
-### Bug Fixes
-
-* Error in Quickstarts : Unknown projection '3d' - Issue [#174](https://github.com/sdv-dev/Copulas/issues/174) by @csala
-
-## v0.3.0 - 2020-03-27
-
-Important revamp of the internal implementation of the project, the testing
-infrastructure and the documentation by Kevin Alex Zhang @k15z, Carles Sala
-@csala and Kalyan Veeramachaneni @kveerama
-
-### Enhancements
-
-* Reimplementation of the existing Univariate distributions.
-* Addition of new Beta and Gamma Univariates.
-* New Univariate API with automatic selection of the optimal distribution.
-* Several improvements and fixes on the Bivariate and Multivariate Copulas implementation.
-* New visualization module with simple plotting patterns to visualize probability distributions.
-* New datasets module with toy datasets sampling functions.
-* New testing infrastructure with end-to-end, numerical and large scale testing.
-* Improved tutorials and documentation.
-
-## v0.2.5 - 2020-01-17
-
-### General Improvements
-
-* Convert import_object to get_instance - Issue [#114](https://github.com/sdv-dev/Copulas/issues/114) by @JDTheRipperPC
-
-## v0.2.4 - 2019-12-23
-
-### New Features
-
-* Allow creating copula classes directly - Issue [#117](https://github.com/sdv-dev/Copulas/issues/117) by @csala
-
-### General Improvements
-
-* Remove `select_copula` from `Bivariate` - Issue [#118](https://github.com/sdv-dev/Copulas/issues/118) by @csala
-* Rename TruncNorm to TruncGaussian and make it non standard - Issue [#102](https://github.com/sdv-dev/Copulas/issues/102) by @csala @JDTheRipperPC
-
-### Bugs fixed
-
-* Error on Frank and Gumble sampling - Issue [#112](https://github.com/sdv-dev/Copulas/issues/112) by @csala
-
-## v0.2.3 - 2019-09-17
-
-### New Features
-
-* Add support to Python 3.7 - Issue [#53](https://github.com/sdv-dev/Copulas/issues/53) by @JDTheRipperPC
-
-### General Improvements
-
-* Document RELEASE workflow - Issue [#105](https://github.com/sdv-dev/Copulas/issues/105) by @JDTheRipperPC
-* Improve serialization of univariate distributions - Issue [#99](https://github.com/sdv-dev/Copulas/issues/99) by @ManuelAlvarezC and @JDTheRipperPC
-
-### Bugs fixed
-
-* The method 'select_copula' of Bivariate return wrong CopulaType - Issue [#101](https://github.com/sdv-dev/Copulas/issues/101) by @JDTheRipperPC
-
-## v0.2.2 - 2019-07-31
-
-### New Features
-
-* `truncnorm` distribution and a generic wrapper for `scipy.rv_continous` distributions - Issue [#27](https://github.com/sdv-dev/Copulas/issues/27) by @amontanez, @csala and @ManuelAlvarezC
-* `Independence` bivariate copulas - Issue [#46](https://github.com/sdv-dev/Copulas/issues/46) by @aliciasun, @csala and @ManuelAlvarezC
-* Option to select seed on random number generator - Issue [#63](https://github.com/sdv-dev/Copulas/issues/63) by @echo66 and @ManuelAlvarezC
-* Option on Vine copulas to select number of rows to sample - Issue [#77](https://github.com/sdv-dev/Copulas/issues/77) by @ManuelAlvarezC
-* Make copulas accept both scalars and arrays as arguments - Issues [#85](https://github.com/sdv-dev/Copulas/issues/85) and [#90](https://github.com/sdv-dev/Copulas/issues/90) by @ManuelAlvarezC
-
-### General Improvements
-
-* Ability to properly handle constant data - Issues [#57](https://github.com/sdv-dev/Copulas/issues/57) and [#82](https://github.com/sdv-dev/Copulas/issues/82) by @csala and @ManuelAlvarezC
-* Tests for analytics properties of copulas - Issue [#61](https://github.com/sdv-dev/Copulas/issues/61) by @ManuelAlvarezC
-* Improved documentation - Issue [#96](https://github.com/sdv-dev/Copulas/issues/96) by @ManuelAlvarezC
-
-### Bugs fixed
-
-* Fix bug on Vine copulas, that made it crash during the bivariate copula selection - Issue [#64](https://github.com/sdv-dev/Copulas/issues/64) by @echo66 and @ManuelAlvarezC
-
-## v0.2.1 - Vine serialization
-
-* Add serialization to Vine copulas.
-* Add `distribution` as argument for the Gaussian Copula.
-* Improve Bivariate Copulas code structure to remove code duplication.
-* Fix bug in Vine Copulas sampling: 'Edge' object has no attribute 'index'
-* Improve code documentation.
-* Improve code style and linting tools configuration.
-
-## v0.2.0 - Unified API
-
-* New API for stats methods.
-* Standarize input and output to `numpy.ndarray`.
-* Increase unittest coverage to 90%.
-* Add methods to load/save copulas.
-* Improve Gaussian copula sampling accuracy.
-
-## v0.1.1 - Minor Improvements
-
-* Different Copula types separated in subclasses
-* Extensive Unit Testing
-* More pythonic names in the public API.
-* Stop using third party elements that will be deprected soon.
-* Add methods to sample new data on bivariate copulas.
-* New KDE Univariate copula
-* Improved examples with additional demo data.
-
-## v0.1.0 - First Release
-
-* First release on PyPI.
```

#### html2text {}

```diff
@@ -1,20 +1,11 @@
-Metadata-Version: 2.1 Name: copulas Version: 0.8.0.dev0 Summary: Create tabular
+Metadata-Version: 2.1 Name: copulas Version: 0.8.1.dev0 Summary: Create tabular
 synthetic data using copulas-based modeling. Home-page: https://github.com/sdv-
 dev/Copulas Author: DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1
-Keywords: copulas Classifier: Development Status :: 2 - Pre-Alpha Classifier:
-Intended Audience :: Developers Classifier: License :: Free for non-commercial
-use Classifier: Natural Language :: English Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.7,<3.12
-Description-Content-Type: text/markdown Provides-Extra: tutorials Provides-
-Extra: test Provides-Extra: dev License-File: LICENSE License-File: AUTHORS.rst
+Description:
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
 [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--
 %20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-
 +Pre-Alpha) [![PyPi Shield](https://img.shields.io/pypi/v/copulas.svg)](https:/
 /pypi.python.org/pypi/copulas) [![Downloads](https://pepy.tech/badge/copulas)]
@@ -76,17 +67,23 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## v0.7.0 - 2022-05-10 This release
-adds `gaussian` as a fallback distribution in case the user specified one
-fails. It also improves the `fit` of the `beta` distribution by properly
+libraries for specific needs. # History ## v0.8.0 - 2023-01-06 This release
+adds support for python 3.10 and 3.11. Additionally, it drops support for
+python 3.6. ### Maintenance * Support python 3.10 and above - PR[#338](https://
+github.com/sdv-dev/Copulas/pull/338) by @pvk-developer * Copulas Package
+Maintenance Updates - Issue[#336](https://github.com/sdv-dev/Copulas/issues/
+336) by @pvk-developer * Add support for python 3.10 - PR[#329](https://
+github.com/sdv-dev/Copulas/pull/329) by @katxiao ## v0.7.0 - 2022-05-10 This
+release adds `gaussian` as a fallback distribution in case the user specified
+one fails. It also improves the `fit` of the `beta` distribution by properly
 estimatig the `loc` and `scale` parameters. ### General Improvements * Add
 gaussian as fallback - Issue[#320](https://github.com/sdv-dev/Copulas/issues/
 320) by @fealho * Improve the fit of the Beta distribution: Use the new loc and
 scale - Issue[#317](https://github.com/sdv-dev/Copulas/issues/317) by @pvk-
 developer ## v0.6.1 - 2022-02-25 This release improves the `random_state`
 functionality by taking in RandomState objects in addition to random seeds. ###
 General Improvements * Use random_state instead of random_seed - Issue[#113]
@@ -198,7 +195,17 @@
 `numpy.ndarray`. * Increase unittest coverage to 90%. * Add methods to load/
 save copulas. * Improve Gaussian copula sampling accuracy. ## v0.1.1 - Minor
 Improvements * Different Copula types separated in subclasses * Extensive Unit
 Testing * More pythonic names in the public API. * Stop using third party
 elements that will be deprected soon. * Add methods to sample new data on
 bivariate copulas. * New KDE Univariate copula * Improved examples with
 additional demo data. ## v0.1.0 - First Release * First release on PyPI.
+Keywords: copulas Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-
+Alpha Classifier: Intended Audience :: Developers Classifier: License :: Free
+for non-commercial use Classifier: Natural Language :: English Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
+>=3.7,<3.12 Description-Content-Type: text/markdown Provides-Extra: tutorials
+Provides-Extra: test Provides-Extra: dev
```

### Comparing `copulas-0.8.0.dev0/README.md` & `copulas-0.8.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/RELEASE.md` & `copulas-0.8.1.dev0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/__init__.py` & `copulas-0.8.1.dev0/copulas/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for Copulas."""
 
 __author__ = 'DataCebo, Inc.'
 __email__ = 'info@sdv.dev'
-__version__ = '0.8.0.dev0'
+__version__ = '0.8.1.dev0'
 
 import contextlib
 import importlib
 from copy import deepcopy
 
 import numpy as np
 import pandas as pd
 
+from copulas._addons import _find_addons
+
+_find_addons(group='copulas_modules', parent_globals=globals())
+
 EPSILON = np.finfo(np.float32).eps
 
 
 class NotFittedError(Exception):
     """NotFittedError class."""
```

### Comparing `copulas-0.8.0.dev0/copulas/bivariate/__init__.py` & `copulas-0.8.1.dev0/copulas/bivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/bivariate/base.py` & `copulas-0.8.1.dev0/copulas/bivariate/base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/bivariate/clayton.py` & `copulas-0.8.1.dev0/copulas/bivariate/clayton.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/bivariate/frank.py` & `copulas-0.8.1.dev0/copulas/bivariate/frank.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/bivariate/gumbel.py` & `copulas-0.8.1.dev0/copulas/bivariate/gumbel.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/bivariate/independence.py` & `copulas-0.8.1.dev0/copulas/bivariate/independence.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/datasets.py` & `copulas-0.8.1.dev0/copulas/datasets.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/multivariate/base.py` & `copulas-0.8.1.dev0/copulas/multivariate/base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/multivariate/gaussian.py` & `copulas-0.8.1.dev0/copulas/multivariate/gaussian.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Args:
         distribution (str or dict):
             Fully qualified name of the class to be used for modeling the marginal
             distributions or a dictionary mapping column names to the fully qualified
             distribution names.
     """
 
-    covariance = None
+    correlation = None
     columns = None
     univariates = None
 
     @store_args
     def __init__(self, distribution=DEFAULT_DISTRIBUTION, random_state=None):
         self.random_state = validate_random_state(random_state)
         self.distribution = distribution
@@ -61,37 +61,37 @@
         for column_name, univariate in zip(self.columns, self.univariates):
             if column_name in X:
                 column = X[column_name]
                 U.append(univariate.cdf(column.to_numpy()).clip(EPSILON, 1 - EPSILON))
 
         return stats.norm.ppf(np.column_stack(U))
 
-    def _get_covariance(self, X):
-        """Compute covariance matrix with transformed data.
+    def _get_correlation(self, X):
+        """Compute correlation matrix with transformed data.
 
         Args:
             X (numpy.ndarray):
-                Data for which the covariance needs to be computed.
+                Data for which the correlation needs to be computed.
 
         Returns:
             numpy.ndarray:
-                computed covariance matrix.
+                computed correlation matrix.
         """
         result = self._transform_to_normal(X)
-        covariance = pd.DataFrame(data=result).corr().to_numpy()
-        covariance = np.nan_to_num(covariance, nan=0.0)
+        correlation = pd.DataFrame(data=result).corr().to_numpy()
+        correlation = np.nan_to_num(correlation, nan=0.0)
         # If singular, add some noise to the diagonal
-        if np.linalg.cond(covariance) > 1.0 / sys.float_info.epsilon:
-            covariance = covariance + np.identity(covariance.shape[0]) * EPSILON
+        if np.linalg.cond(correlation) > 1.0 / sys.float_info.epsilon:
+            correlation = correlation + np.identity(correlation.shape[0]) * EPSILON
 
-        return pd.DataFrame(covariance, index=self.columns, columns=self.columns)
+        return pd.DataFrame(correlation, index=self.columns, columns=self.columns)
 
     @check_valid_values
     def fit(self, X):
-        """Compute the distribution for each variable and then its covariance matrix.
+        """Compute the distribution for each variable and then its correlation matrix.
 
         Arguments:
             X (pandas.DataFrame):
                 Values of the random variables.
         """
         LOGGER.info('Fitting %s', self)
 
@@ -122,16 +122,16 @@
 
             columns.append(column_name)
             univariates.append(univariate)
 
         self.columns = columns
         self.univariates = univariates
 
-        LOGGER.debug('Computing covariance')
-        self.covariance = self._get_covariance(X)
+        LOGGER.debug('Computing correlation')
+        self.correlation = self._get_correlation(X)
         self.fitted = True
 
         LOGGER.debug('GaussianMultivariate fitted successfully')
 
     def probability_density(self, X):
         """Compute the probability density for each point in X.
 
@@ -145,15 +145,15 @@
 
         Raises:
             NotFittedError:
                 if the model is not fitted.
         """
         self.check_fit()
         transformed = self._transform_to_normal(X)
-        return stats.multivariate_normal.pdf(transformed, cov=self.covariance)
+        return stats.multivariate_normal.pdf(transformed, cov=self.correlation)
 
     def cumulative_distribution(self, X):
         """Compute the cumulative distribution value for each point in X.
 
         Arguments:
             X (pandas.DataFrame):
                 Values for which the cumulative distribution will be computed.
@@ -164,15 +164,15 @@
 
         Raises:
             NotFittedError:
                 if the model is not fitted.
         """
         self.check_fit()
         transformed = self._transform_to_normal(X)
-        return stats.multivariate_normal.cdf(transformed, cov=self.covariance)
+        return stats.multivariate_normal.cdf(transformed, cov=self.correlation)
 
     def _get_conditional_distribution(self, conditions):
         """Compute the parameters of a conditional multivariate normal distribution.
 
         The parameters of the conditioned distribution are computed as specified here:
         https://en.wikipedia.org/wiki/Multivariate_normal_distribution#Conditional_distributions
 
@@ -188,20 +188,20 @@
                 * covariance (numpy.array):
                     covariance matrix to use for the conditioned
                   multivariate normal.
                 * columns (list):
                     names of the columns that will be sampled conditionally.
         """
         columns2 = conditions.index
-        columns1 = self.covariance.columns.difference(columns2)
+        columns1 = self.correlation.columns.difference(columns2)
 
-        sigma11 = self.covariance.loc[columns1, columns1].to_numpy()
-        sigma12 = self.covariance.loc[columns1, columns2].to_numpy()
-        sigma21 = self.covariance.loc[columns2, columns1].to_numpy()
-        sigma22 = self.covariance.loc[columns2, columns2].to_numpy()
+        sigma11 = self.correlation.loc[columns1, columns1].to_numpy()
+        sigma12 = self.correlation.loc[columns1, columns2].to_numpy()
+        sigma21 = self.correlation.loc[columns2, columns1].to_numpy()
+        sigma22 = self.correlation.loc[columns2, columns2].to_numpy()
 
         mu1 = np.zeros(len(columns1))
         mu2 = np.zeros(len(columns2))
 
         sigma12sigma22inv = sigma12 @ np.linalg.inv(sigma22)
 
         mu_bar = mu1 + sigma12sigma22inv @ (conditions - mu2)
@@ -216,15 +216,15 @@
         multivariate.
 
         If conditions are given, they are transformed to their equivalent standard
         normal values using their marginals and then the values are sampled from
         a standard normal multivariate conditioned on the given condition values.
         """
         if conditions is None:
-            covariance = self.covariance
+            covariance = self.correlation
             columns = self.columns
             means = np.zeros(len(columns))
         else:
             conditions = pd.Series(conditions)
             normal_conditions = self._transform_to_normal(conditions)[0]
             normal_conditions = pd.Series(normal_conditions, index=conditions.index)
             means, covariance, columns = self._get_conditional_distribution(normal_conditions)
@@ -273,19 +273,17 @@
 
         Returns:
             dict:
                 Parameters of this distribution.
         """
         self.check_fit()
         univariates = [univariate.to_dict() for univariate in self.univariates]
-        warnings.warn('`covariance` will be renamed to `correlation` in v0.4.0',
-                      DeprecationWarning)
 
         return {
-            'covariance': self.covariance.to_numpy().tolist(),
+            'correlation': self.correlation.to_numpy().tolist(),
             'univariates': univariates,
             'columns': self.columns,
             'type': get_qualified_name(self),
         }
 
     @classmethod
     def from_dict(cls, copula_dict):
@@ -304,14 +302,12 @@
         instance.univariates = []
         columns = copula_dict['columns']
         instance.columns = columns
 
         for parameters in copula_dict['univariates']:
             instance.univariates.append(Univariate.from_dict(parameters))
 
-        covariance = copula_dict['covariance']
-        instance.covariance = pd.DataFrame(covariance, index=columns, columns=columns)
+        correlation = copula_dict['correlation']
+        instance.correlation = pd.DataFrame(correlation, index=columns, columns=columns)
         instance.fitted = True
-        warnings.warn('`covariance` will be renamed to `correlation` in v0.4.0',
-                      DeprecationWarning)
 
         return instance
```

### Comparing `copulas-0.8.0.dev0/copulas/multivariate/tree.py` & `copulas-0.8.1.dev0/copulas/multivariate/tree.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/multivariate/vine.py` & `copulas-0.8.1.dev0/copulas/multivariate/vine.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/optimize/__init__.py` & `copulas-0.8.1.dev0/copulas/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/univariate/__init__.py` & `copulas-0.8.1.dev0/copulas/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/univariate/base.py` & `copulas-0.8.1.dev0/copulas/univariate/base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/univariate/beta.py` & `copulas-0.8.1.dev0/copulas/univariate/beta.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/univariate/gamma.py` & `copulas-0.8.1.dev0/copulas/univariate/gamma.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/univariate/gaussian.py` & `copulas-0.8.1.dev0/copulas/univariate/gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/univariate/gaussian_kde.py` & `copulas-0.8.1.dev0/copulas/univariate/gaussian_kde.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/univariate/log_laplace.py` & `copulas-0.8.1.dev0/copulas/univariate/log_laplace.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/univariate/selection.py` & `copulas-0.8.1.dev0/copulas/univariate/selection.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/univariate/student_t.py` & `copulas-0.8.1.dev0/copulas/univariate/student_t.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/univariate/truncated_gaussian.py` & `copulas-0.8.1.dev0/copulas/univariate/truncated_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/univariate/uniform.py` & `copulas-0.8.1.dev0/copulas/univariate/uniform.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas/visualization.py` & `copulas-0.8.1.dev0/copulas/visualization.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/copulas.egg-info/PKG-INFO` & `copulas-0.8.1.dev0/copulas.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,384 @@
 Metadata-Version: 2.1
 Name: copulas
-Version: 0.8.0.dev0
+Version: 0.8.1.dev0
 Summary: Create tabular synthetic data using copulas-based modeling.
 Home-page: https://github.com/sdv-dev/Copulas
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
+Description: <div align="center">
+        <br/>
+        <p align="center">
+            <i>This repository is part of <a href="https://sdv.dev">The Synthetic Data Vault Project</a>, a project from <a href="https://datacebo.com">DataCebo</a>.</i>
+        </p>
+        
+        [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--%20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
+        [![PyPi Shield](https://img.shields.io/pypi/v/copulas.svg)](https://pypi.python.org/pypi/copulas)
+        [![Downloads](https://pepy.tech/badge/copulas)](https://pepy.tech/project/copulas)
+        [![Unit Tests](https://github.com/sdv-dev/Copulas/actions/workflows/unit.yml/badge.svg)](https://github.com/sdv-dev/Copulas/actions/workflows/unit.yml)
+        [![Coverage Status](https://codecov.io/gh/sdv-dev/Copulas/branch/master/graph/badge.svg)](https://codecov.io/gh/sdv-dev/Copulas)
+        [![Slack](https://img.shields.io/badge/Community-Slack-blue?style=plastic&logo=slack)](https://bit.ly/sdv-slack-invite)
+        
+        <div align="left">
+        <br/>
+        <p align="center">
+        <a href="https://github.com/sdv-dev/Copulas">
+        <img align="center" width=40% src="https://github.com/sdv-dev/SDV/blob/master/docs/images/Copulas-DataCebo.png"></img>
+        </a>
+        </p>
+        </div>
+        
+        </div>
+        
+        # Overview
+        
+        **Copulas** is a Python library for modeling multivariate distributions and sampling from them
+        using copula functions.
+        Given a table of numerical data, use Copulas to learn the distribution and
+        generate new synthetic data following the same statistical properties.
+        
+        **Key Features:**
+        
+        * **Model multivariate data.** Choose from a variety of univariate
+        distributions and copulas – including Archimedian Copulas, Gaussian Copulas and Vine Copulas.
+        
+        * **Compare real and synthetic data visually** after building your model. Visualizations
+        are available as 1D histograms, 2D scatterplots and 3D scatterplots.
+        
+        * **Access & manipulate learned parameters.** With complete access to the internals
+        of the model, set or tune parameters to your choosing.
+        
+        # Install
+        
+        Install the Copulas library using pip or conda.
+        
+        ```bash
+        pip install copulas
+        ```
+        
+        ```bash
+        conda install -c conda-forge copulas
+        ```
+        
+        # Usage
+        
+        Get started using a demo dataset. This dataset contains 3 numerical columns.
+        
+        ```python
+        from copulas.datasets import sample_trivariate_xyz
+        
+        real_data = sample_trivariate_xyz()
+        real_data.head()
+        ```
+        
+        <img src="docs/images/copulas_sample_dataset.png" width="300">
+        
+        Model the data using a copula and use it to create synthetic data.
+        The Copulas library offers many options including Gaussian Copula,
+        Vine Copulas and Archimedian Copulas.
+        
+        ```python
+        from copulas.multivariate import GaussianMultivariate
+        
+        copula = GaussianMultivariate()
+        copula.fit(real_data)
+        
+        synthetic_data = copula.sample(len(real_data))
+        ```
+        
+        Visualize the real and synthetic data side-by-side. Let's do this in 3D so see our full dataset.
+        
+        ```python
+        from copulas.visualization import compare_3d
+        
+        compare_3d(real_data, synthetic_data)
+        ```
+        
+        ![Quickstart](docs/images/quickstart.png)
+        
+        # Tutorials
+        Click below to run the code yourself on a Colab Notebook and discover new features.
+        
+        [![Tutorial Notebook](https://img.shields.io/badge/Tutorial-Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252)](https://bit.ly/copulas-demo)
+        
+        # Community & Support
+        
+        Learn more about Copulas library from our [documentation](https://sdv.dev/Copulas/) site.
+        
+        **Questions or issues?** Join our [Slack channel](https://bit.ly/sdv-slack-invite)
+        to discuss more about Copulas and synthetic data.
+        If you find a bug or have a feature request, you can also
+        [open an issue](https://github.com/sdv-dev/Copulas/issues/new/choose) on our GitHub.
+        
+        **Interested in contributing to Copulas?** Read our
+        [Contribution Guide](https://sdv.dev/Copulas/contributing.html) to get started.
+        
+        # Credits
+        
+        The Copulas open source project first started at the Data to AI Lab at MIT in 2018.
+        Thank you to our team of contributors who have built and maintained the library over the years!
+        
+        [View Contributors](https://github.com/sdv-dev/Copulas/graphs/contributors)
+        
+        ---
+        
+        
+        <div align="center">
+        <a href="https://datacebo.com"><img align="center" width=40% src="https://github.com/sdv-dev/SDV/blob/master/docs/images/DataCebo.png"></img></a>
+        </div>
+        <br/>
+        <br/>
+        
+        [The Synthetic Data Vault Project](https://sdv.dev) was first created at MIT's [Data to AI Lab](
+        https://dai.lids.mit.edu/) in 2016. After 4 years of research and traction with enterprise, we
+        created [DataCebo](https://datacebo.com) in 2020 with the goal of growing the project.
+        Today, DataCebo is the proud developer of SDV, the largest ecosystem for
+        synthetic data generation & evaluation. It is home to multiple libraries that support synthetic
+        data, including:
+        
+        * 🔄 Data discovery & transformation. Reverse the transforms to reproduce realistic data.
+        * 🧠 Multiple machine learning models -- ranging from Copulas to Deep Learning -- to create tabular,
+          multi table and time series data.
+        * 📊 Measuring quality and privacy of synthetic data, and comparing different synthetic data
+          generation models.
+        
+        [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
+        integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
+        for specific needs.
+        
+        
+        # History
+        
+        ## v0.8.0 - 2023-01-06
+        
+        This release adds support for python 3.10 and 3.11. Additionally, it drops support for python 3.6.
+        
+        ### Maintenance
+        
+        * Support python 3.10 and above - PR[#338](https://github.com/sdv-dev/Copulas/pull/338) by @pvk-developer
+        * Copulas Package Maintenance Updates - Issue[#336](https://github.com/sdv-dev/Copulas/issues/336) by @pvk-developer
+        * Add support for python 3.10 - PR[#329](https://github.com/sdv-dev/Copulas/pull/329) by @katxiao
+        
+        ## v0.7.0 - 2022-05-10
+        
+        This release adds `gaussian` as a fallback distribution in case the user specified one fails. It also improves the `fit` of the `beta` distribution by properly estimatig the `loc` and `scale` parameters.
+        
+        ### General Improvements
+        
+        * Add gaussian as fallback - Issue[#320](https://github.com/sdv-dev/Copulas/issues/320) by @fealho
+        * Improve the fit of the Beta distribution: Use the new loc and scale - Issue[#317](https://github.com/sdv-dev/Copulas/issues/317) by @pvk-developer
+        
+        ## v0.6.1 - 2022-02-25
+        
+        This release improves the `random_state` functionality by taking in RandomState objects in addition to
+        random seeds.
+        
+        ### General Improvements
+        
+        * Use random_state instead of random_seed - Issue[#113](https://github.com/sdv-dev/Copulas/issues/113) by @katxiao
+        
+        ## v0.6.0 - 2021-05-13
+        
+        This release makes Copulas compatible with Python 3.9! It also improves library maintenance by
+        updating dependencies, reorganizing the CI workflows, adding pip check to the workflows and
+        removing unused files.
+        
+        ### General Improvements
+        
+        * Add support for Python 3.9 - Issue[#282](https://github.com/sdv-dev/Copulas/issues/282) by @amontanez24
+        * Remove entry point in setup.py - Issue[#280](https://github.com/sdv-dev/Copulas/issues/280) by @amontanez24
+        * Update pandas dependency range - Issue[#266](https://github.com/sdv-dev/Copulas/issues/266) by @katxiao
+        * Fix repository language - Issue[#272](https://github.com/sdv-dev/Copulas/issues/272) by @pvk-developer
+        * Add pip check to CI workflows - Issue[#274](https://github.com/sdv-dev/Copulas/issues/274) by @pvk-developer
+        * Reorganize workflows and add codecov - PR[#267](https://github.com/sdv-dev/Copulas/pull/267) by @csala
+        * Constrain jinja2 versions - PR[#269](https://github.com/sdv-dev/Copulas/pull/269/files) by @fealho
+        
+        ## v0.5.1 - 2021-08-13
+        
+        This release improves performance by changing the way scipy stats is used,
+        calling their methods directly without creating intermediate instances.
+        
+        It also fixes a bug introduced by the scipy 1.7.0 release where some
+        distributions fail to fit because scipy validates the learned parameters.
+        
+        ### Issues Closed
+         * Exception: Optimization converged to parameters that are outside the range allowed by the distribution. - Issue [#264](https://github.com/sdv-dev/Copulas/issues/264) by @csala
+         * Use scipy stats models directly without creating instances - Issue [#261](https://github.com/sdv-dev/Copulas/issues/261) by @csala
+        
+        ## v0.5.0 - 2021-01-24
+        
+        This release introduces conditional sampling for the GaussianMultivariate modeling.
+        The new conditioning feature allows passing a dictionary with the values to use to condition
+        the rest of the columns.
+        
+        It also fixes a bug that prevented constant distributions to be restored from a dictionary
+        and updates some dependencies.
+        
+        ### New Features
+        
+        * Conditional sampling from Gaussian copula - Issue [#154](https://github.com/sdv-dev/Copulas/issues/154) by @csala
+        
+        ### Bug Fixes
+        
+        * ScipyModel subclasses fail to restore constant values when using `from_dict` - Issue [#212](https://github.com/sdv-dev/Copulas/issues/212) by @csala
+        
+        ## v0.4.0 - 2021-01-27
+        
+        This release introduces a few changes to optimize processing speed by re-implementing
+        the Gaussian KDE pdf to use vectorized root finding methods and also adding the option
+        to subsample the data during univariate selection.
+        
+        ### General Improvements
+        
+        * Make `gaussian_kde` faster - Issue [#200](https://github.com/sdv-dev/Copulas/issues/200) by @k15z and @fealho
+        * Use sub-sampling in `select_univariate` - Issue [#183](https://github.com/sdv-dev/Copulas/issues/183) by @csala
+        
+        ## v0.3.3 - 2020-09-18
+        
+        ### General Improvements
+        
+        * Use `corr` instead of `cov` in the GaussianMultivariate - Issue [#195](https://github.com/sdv-dev/Copulas/issues/195) by @rollervan
+        * Add arguments to GaussianKDE - Issue [#181](https://github.com/sdv-dev/Copulas/issues/181) by @rollervan
+        
+        ### New Features
+        
+        * Log Laplace Distribution - Issue [#188](https://github.com/sdv-dev/Copulas/issues/188) by @rollervan
+        
+        ## v0.3.2 - 2020-08-08
+        
+        ### General Improvements
+        
+        * Support Python 3.8 - Issue [#185](https://github.com/sdv-dev/Copulas/issues/185) by @csala
+        * Support scipy >1.3 - Issue [#180](https://github.com/sdv-dev/Copulas/issues/180) by @csala
+        
+        ### New Features
+        
+        * Add Uniform Univariate - Issue [#179](https://github.com/sdv-dev/Copulas/issues/179) by @rollervan
+        
+        ## v0.3.1 - 2020-07-09
+        
+        ### General Improvements
+        
+        * Raise numpy version upper bound to 2 - Issue [#178](https://github.com/sdv-dev/Copulas/issues/178) by @csala
+        
+        ### New Features
+        
+        * Add Student T Univariate - Issue [#172](https://github.com/sdv-dev/Copulas/issues/172) by @gbonomib
+        
+        ### Bug Fixes
+        
+        * Error in Quickstarts : Unknown projection '3d' - Issue [#174](https://github.com/sdv-dev/Copulas/issues/174) by @csala
+        
+        ## v0.3.0 - 2020-03-27
+        
+        Important revamp of the internal implementation of the project, the testing
+        infrastructure and the documentation by Kevin Alex Zhang @k15z, Carles Sala
+        @csala and Kalyan Veeramachaneni @kveerama
+        
+        ### Enhancements
+        
+        * Reimplementation of the existing Univariate distributions.
+        * Addition of new Beta and Gamma Univariates.
+        * New Univariate API with automatic selection of the optimal distribution.
+        * Several improvements and fixes on the Bivariate and Multivariate Copulas implementation.
+        * New visualization module with simple plotting patterns to visualize probability distributions.
+        * New datasets module with toy datasets sampling functions.
+        * New testing infrastructure with end-to-end, numerical and large scale testing.
+        * Improved tutorials and documentation.
+        
+        ## v0.2.5 - 2020-01-17
+        
+        ### General Improvements
+        
+        * Convert import_object to get_instance - Issue [#114](https://github.com/sdv-dev/Copulas/issues/114) by @JDTheRipperPC
+        
+        ## v0.2.4 - 2019-12-23
+        
+        ### New Features
+        
+        * Allow creating copula classes directly - Issue [#117](https://github.com/sdv-dev/Copulas/issues/117) by @csala
+        
+        ### General Improvements
+        
+        * Remove `select_copula` from `Bivariate` - Issue [#118](https://github.com/sdv-dev/Copulas/issues/118) by @csala
+        * Rename TruncNorm to TruncGaussian and make it non standard - Issue [#102](https://github.com/sdv-dev/Copulas/issues/102) by @csala @JDTheRipperPC
+        
+        ### Bugs fixed
+        
+        * Error on Frank and Gumble sampling - Issue [#112](https://github.com/sdv-dev/Copulas/issues/112) by @csala
+        
+        ## v0.2.3 - 2019-09-17
+        
+        ### New Features
+        
+        * Add support to Python 3.7 - Issue [#53](https://github.com/sdv-dev/Copulas/issues/53) by @JDTheRipperPC
+        
+        ### General Improvements
+        
+        * Document RELEASE workflow - Issue [#105](https://github.com/sdv-dev/Copulas/issues/105) by @JDTheRipperPC
+        * Improve serialization of univariate distributions - Issue [#99](https://github.com/sdv-dev/Copulas/issues/99) by @ManuelAlvarezC and @JDTheRipperPC
+        
+        ### Bugs fixed
+        
+        * The method 'select_copula' of Bivariate return wrong CopulaType - Issue [#101](https://github.com/sdv-dev/Copulas/issues/101) by @JDTheRipperPC
+        
+        ## v0.2.2 - 2019-07-31
+        
+        ### New Features
+        
+        * `truncnorm` distribution and a generic wrapper for `scipy.rv_continous` distributions - Issue [#27](https://github.com/sdv-dev/Copulas/issues/27) by @amontanez, @csala and @ManuelAlvarezC
+        * `Independence` bivariate copulas - Issue [#46](https://github.com/sdv-dev/Copulas/issues/46) by @aliciasun, @csala and @ManuelAlvarezC
+        * Option to select seed on random number generator - Issue [#63](https://github.com/sdv-dev/Copulas/issues/63) by @echo66 and @ManuelAlvarezC
+        * Option on Vine copulas to select number of rows to sample - Issue [#77](https://github.com/sdv-dev/Copulas/issues/77) by @ManuelAlvarezC
+        * Make copulas accept both scalars and arrays as arguments - Issues [#85](https://github.com/sdv-dev/Copulas/issues/85) and [#90](https://github.com/sdv-dev/Copulas/issues/90) by @ManuelAlvarezC
+        
+        ### General Improvements
+        
+        * Ability to properly handle constant data - Issues [#57](https://github.com/sdv-dev/Copulas/issues/57) and [#82](https://github.com/sdv-dev/Copulas/issues/82) by @csala and @ManuelAlvarezC
+        * Tests for analytics properties of copulas - Issue [#61](https://github.com/sdv-dev/Copulas/issues/61) by @ManuelAlvarezC
+        * Improved documentation - Issue [#96](https://github.com/sdv-dev/Copulas/issues/96) by @ManuelAlvarezC
+        
+        ### Bugs fixed
+        
+        * Fix bug on Vine copulas, that made it crash during the bivariate copula selection - Issue [#64](https://github.com/sdv-dev/Copulas/issues/64) by @echo66 and @ManuelAlvarezC
+        
+        ## v0.2.1 - Vine serialization
+        
+        * Add serialization to Vine copulas.
+        * Add `distribution` as argument for the Gaussian Copula.
+        * Improve Bivariate Copulas code structure to remove code duplication.
+        * Fix bug in Vine Copulas sampling: 'Edge' object has no attribute 'index'
+        * Improve code documentation.
+        * Improve code style and linting tools configuration.
+        
+        ## v0.2.0 - Unified API
+        
+        * New API for stats methods.
+        * Standarize input and output to `numpy.ndarray`.
+        * Increase unittest coverage to 90%.
+        * Add methods to load/save copulas.
+        * Improve Gaussian copula sampling accuracy.
+        
+        ## v0.1.1 - Minor Improvements
+        
+        * Different Copula types separated in subclasses
+        * Extensive Unit Testing
+        * More pythonic names in the public API.
+        * Stop using third party elements that will be deprected soon.
+        * Add methods to sample new data on bivariate copulas.
+        * New KDE Univariate copula
+        * Improved examples with additional demo data.
+        
+        ## v0.1.0 - First Release
+        
+        * First release on PyPI.
+        
 Keywords: copulas
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -19,366 +387,7 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7,<3.12
 Description-Content-Type: text/markdown
 Provides-Extra: tutorials
 Provides-Extra: test
 Provides-Extra: dev
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-<div align="center">
-<br/>
-<p align="center">
-    <i>This repository is part of <a href="https://sdv.dev">The Synthetic Data Vault Project</a>, a project from <a href="https://datacebo.com">DataCebo</a>.</i>
-</p>
-
-[![Development Status](https://img.shields.io/badge/Development%20Status-2%20--%20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
-[![PyPi Shield](https://img.shields.io/pypi/v/copulas.svg)](https://pypi.python.org/pypi/copulas)
-[![Downloads](https://pepy.tech/badge/copulas)](https://pepy.tech/project/copulas)
-[![Unit Tests](https://github.com/sdv-dev/Copulas/actions/workflows/unit.yml/badge.svg)](https://github.com/sdv-dev/Copulas/actions/workflows/unit.yml)
-[![Coverage Status](https://codecov.io/gh/sdv-dev/Copulas/branch/master/graph/badge.svg)](https://codecov.io/gh/sdv-dev/Copulas)
-[![Slack](https://img.shields.io/badge/Community-Slack-blue?style=plastic&logo=slack)](https://bit.ly/sdv-slack-invite)
-
-<div align="left">
-<br/>
-<p align="center">
-<a href="https://github.com/sdv-dev/Copulas">
-<img align="center" width=40% src="https://github.com/sdv-dev/SDV/blob/master/docs/images/Copulas-DataCebo.png"></img>
-</a>
-</p>
-</div>
-
-</div>
-
-# Overview
-
-**Copulas** is a Python library for modeling multivariate distributions and sampling from them
-using copula functions.
-Given a table of numerical data, use Copulas to learn the distribution and
-generate new synthetic data following the same statistical properties.
-
-**Key Features:**
-
-* **Model multivariate data.** Choose from a variety of univariate
-distributions and copulas – including Archimedian Copulas, Gaussian Copulas and Vine Copulas.
-
-* **Compare real and synthetic data visually** after building your model. Visualizations
-are available as 1D histograms, 2D scatterplots and 3D scatterplots.
-
-* **Access & manipulate learned parameters.** With complete access to the internals
-of the model, set or tune parameters to your choosing.
-
-# Install
-
-Install the Copulas library using pip or conda.
-
-```bash
-pip install copulas
-```
-
-```bash
-conda install -c conda-forge copulas
-```
-
-# Usage
-
-Get started using a demo dataset. This dataset contains 3 numerical columns.
-
-```python
-from copulas.datasets import sample_trivariate_xyz
-
-real_data = sample_trivariate_xyz()
-real_data.head()
-```
-
-<img src="docs/images/copulas_sample_dataset.png" width="300">
-
-Model the data using a copula and use it to create synthetic data.
-The Copulas library offers many options including Gaussian Copula,
-Vine Copulas and Archimedian Copulas.
-
-```python
-from copulas.multivariate import GaussianMultivariate
-
-copula = GaussianMultivariate()
-copula.fit(real_data)
-
-synthetic_data = copula.sample(len(real_data))
-```
-
-Visualize the real and synthetic data side-by-side. Let's do this in 3D so see our full dataset.
-
-```python
-from copulas.visualization import compare_3d
-
-compare_3d(real_data, synthetic_data)
-```
-
-![Quickstart](docs/images/quickstart.png)
-
-# Tutorials
-Click below to run the code yourself on a Colab Notebook and discover new features.
-
-[![Tutorial Notebook](https://img.shields.io/badge/Tutorial-Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252)](https://bit.ly/copulas-demo)
-
-# Community & Support
-
-Learn more about Copulas library from our [documentation](https://sdv.dev/Copulas/) site.
-
-**Questions or issues?** Join our [Slack channel](https://bit.ly/sdv-slack-invite)
-to discuss more about Copulas and synthetic data.
-If you find a bug or have a feature request, you can also
-[open an issue](https://github.com/sdv-dev/Copulas/issues/new/choose) on our GitHub.
-
-**Interested in contributing to Copulas?** Read our
-[Contribution Guide](https://sdv.dev/Copulas/contributing.html) to get started.
-
-# Credits
-
-The Copulas open source project first started at the Data to AI Lab at MIT in 2018.
-Thank you to our team of contributors who have built and maintained the library over the years!
-
-[View Contributors](https://github.com/sdv-dev/Copulas/graphs/contributors)
-
----
-
-
-<div align="center">
-<a href="https://datacebo.com"><img align="center" width=40% src="https://github.com/sdv-dev/SDV/blob/master/docs/images/DataCebo.png"></img></a>
-</div>
-<br/>
-<br/>
-
-[The Synthetic Data Vault Project](https://sdv.dev) was first created at MIT's [Data to AI Lab](
-https://dai.lids.mit.edu/) in 2016. After 4 years of research and traction with enterprise, we
-created [DataCebo](https://datacebo.com) in 2020 with the goal of growing the project.
-Today, DataCebo is the proud developer of SDV, the largest ecosystem for
-synthetic data generation & evaluation. It is home to multiple libraries that support synthetic
-data, including:
-
-* 🔄 Data discovery & transformation. Reverse the transforms to reproduce realistic data.
-* 🧠 Multiple machine learning models -- ranging from Copulas to Deep Learning -- to create tabular,
-  multi table and time series data.
-* 📊 Measuring quality and privacy of synthetic data, and comparing different synthetic data
-  generation models.
-
-[Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
-integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
-for specific needs.
-
-
-# History
-
-## v0.7.0 - 2022-05-10
-
-This release adds `gaussian` as a fallback distribution in case the user specified one fails. It also improves the `fit` of the `beta` distribution by properly estimatig the `loc` and `scale` parameters.
-
-### General Improvements
-
-* Add gaussian as fallback - Issue[#320](https://github.com/sdv-dev/Copulas/issues/320) by @fealho
-* Improve the fit of the Beta distribution: Use the new loc and scale - Issue[#317](https://github.com/sdv-dev/Copulas/issues/317) by @pvk-developer
-
-## v0.6.1 - 2022-02-25
-
-This release improves the `random_state` functionality by taking in RandomState objects in addition to
-random seeds.
-
-### General Improvements
-
-* Use random_state instead of random_seed - Issue[#113](https://github.com/sdv-dev/Copulas/issues/113) by @katxiao
-
-## v0.6.0 - 2021-05-13
-
-This release makes Copulas compatible with Python 3.9! It also improves library maintenance by
-updating dependencies, reorganizing the CI workflows, adding pip check to the workflows and
-removing unused files.
-
-### General Improvements
-
-* Add support for Python 3.9 - Issue[#282](https://github.com/sdv-dev/Copulas/issues/282) by @amontanez24
-* Remove entry point in setup.py - Issue[#280](https://github.com/sdv-dev/Copulas/issues/280) by @amontanez24
-* Update pandas dependency range - Issue[#266](https://github.com/sdv-dev/Copulas/issues/266) by @katxiao
-* Fix repository language - Issue[#272](https://github.com/sdv-dev/Copulas/issues/272) by @pvk-developer
-* Add pip check to CI workflows - Issue[#274](https://github.com/sdv-dev/Copulas/issues/274) by @pvk-developer
-* Reorganize workflows and add codecov - PR[#267](https://github.com/sdv-dev/Copulas/pull/267) by @csala
-* Constrain jinja2 versions - PR[#269](https://github.com/sdv-dev/Copulas/pull/269/files) by @fealho
-
-## v0.5.1 - 2021-08-13
-
-This release improves performance by changing the way scipy stats is used,
-calling their methods directly without creating intermediate instances.
-
-It also fixes a bug introduced by the scipy 1.7.0 release where some
-distributions fail to fit because scipy validates the learned parameters.
-
-### Issues Closed
- * Exception: Optimization converged to parameters that are outside the range allowed by the distribution. - Issue [#264](https://github.com/sdv-dev/Copulas/issues/264) by @csala
- * Use scipy stats models directly without creating instances - Issue [#261](https://github.com/sdv-dev/Copulas/issues/261) by @csala
-
-## v0.5.0 - 2021-01-24
-
-This release introduces conditional sampling for the GaussianMultivariate modeling.
-The new conditioning feature allows passing a dictionary with the values to use to condition
-the rest of the columns.
-
-It also fixes a bug that prevented constant distributions to be restored from a dictionary
-and updates some dependencies.
-
-### New Features
-
-* Conditional sampling from Gaussian copula - Issue [#154](https://github.com/sdv-dev/Copulas/issues/154) by @csala
-
-### Bug Fixes
-
-* ScipyModel subclasses fail to restore constant values when using `from_dict` - Issue [#212](https://github.com/sdv-dev/Copulas/issues/212) by @csala
-
-## v0.4.0 - 2021-01-27
-
-This release introduces a few changes to optimize processing speed by re-implementing
-the Gaussian KDE pdf to use vectorized root finding methods and also adding the option
-to subsample the data during univariate selection.
-
-### General Improvements
-
-* Make `gaussian_kde` faster - Issue [#200](https://github.com/sdv-dev/Copulas/issues/200) by @k15z and @fealho
-* Use sub-sampling in `select_univariate` - Issue [#183](https://github.com/sdv-dev/Copulas/issues/183) by @csala
-
-## v0.3.3 - 2020-09-18
-
-### General Improvements
-
-* Use `corr` instead of `cov` in the GaussianMultivariate - Issue [#195](https://github.com/sdv-dev/Copulas/issues/195) by @rollervan
-* Add arguments to GaussianKDE - Issue [#181](https://github.com/sdv-dev/Copulas/issues/181) by @rollervan
-
-### New Features
-
-* Log Laplace Distribution - Issue [#188](https://github.com/sdv-dev/Copulas/issues/188) by @rollervan
-
-## v0.3.2 - 2020-08-08
-
-### General Improvements
-
-* Support Python 3.8 - Issue [#185](https://github.com/sdv-dev/Copulas/issues/185) by @csala
-* Support scipy >1.3 - Issue [#180](https://github.com/sdv-dev/Copulas/issues/180) by @csala
-
-### New Features
-
-* Add Uniform Univariate - Issue [#179](https://github.com/sdv-dev/Copulas/issues/179) by @rollervan
-
-## v0.3.1 - 2020-07-09
-
-### General Improvements
-
-* Raise numpy version upper bound to 2 - Issue [#178](https://github.com/sdv-dev/Copulas/issues/178) by @csala
-
-### New Features
-
-* Add Student T Univariate - Issue [#172](https://github.com/sdv-dev/Copulas/issues/172) by @gbonomib
-
-### Bug Fixes
-
-* Error in Quickstarts : Unknown projection '3d' - Issue [#174](https://github.com/sdv-dev/Copulas/issues/174) by @csala
-
-## v0.3.0 - 2020-03-27
-
-Important revamp of the internal implementation of the project, the testing
-infrastructure and the documentation by Kevin Alex Zhang @k15z, Carles Sala
-@csala and Kalyan Veeramachaneni @kveerama
-
-### Enhancements
-
-* Reimplementation of the existing Univariate distributions.
-* Addition of new Beta and Gamma Univariates.
-* New Univariate API with automatic selection of the optimal distribution.
-* Several improvements and fixes on the Bivariate and Multivariate Copulas implementation.
-* New visualization module with simple plotting patterns to visualize probability distributions.
-* New datasets module with toy datasets sampling functions.
-* New testing infrastructure with end-to-end, numerical and large scale testing.
-* Improved tutorials and documentation.
-
-## v0.2.5 - 2020-01-17
-
-### General Improvements
-
-* Convert import_object to get_instance - Issue [#114](https://github.com/sdv-dev/Copulas/issues/114) by @JDTheRipperPC
-
-## v0.2.4 - 2019-12-23
-
-### New Features
-
-* Allow creating copula classes directly - Issue [#117](https://github.com/sdv-dev/Copulas/issues/117) by @csala
-
-### General Improvements
-
-* Remove `select_copula` from `Bivariate` - Issue [#118](https://github.com/sdv-dev/Copulas/issues/118) by @csala
-* Rename TruncNorm to TruncGaussian and make it non standard - Issue [#102](https://github.com/sdv-dev/Copulas/issues/102) by @csala @JDTheRipperPC
-
-### Bugs fixed
-
-* Error on Frank and Gumble sampling - Issue [#112](https://github.com/sdv-dev/Copulas/issues/112) by @csala
-
-## v0.2.3 - 2019-09-17
-
-### New Features
-
-* Add support to Python 3.7 - Issue [#53](https://github.com/sdv-dev/Copulas/issues/53) by @JDTheRipperPC
-
-### General Improvements
-
-* Document RELEASE workflow - Issue [#105](https://github.com/sdv-dev/Copulas/issues/105) by @JDTheRipperPC
-* Improve serialization of univariate distributions - Issue [#99](https://github.com/sdv-dev/Copulas/issues/99) by @ManuelAlvarezC and @JDTheRipperPC
-
-### Bugs fixed
-
-* The method 'select_copula' of Bivariate return wrong CopulaType - Issue [#101](https://github.com/sdv-dev/Copulas/issues/101) by @JDTheRipperPC
-
-## v0.2.2 - 2019-07-31
-
-### New Features
-
-* `truncnorm` distribution and a generic wrapper for `scipy.rv_continous` distributions - Issue [#27](https://github.com/sdv-dev/Copulas/issues/27) by @amontanez, @csala and @ManuelAlvarezC
-* `Independence` bivariate copulas - Issue [#46](https://github.com/sdv-dev/Copulas/issues/46) by @aliciasun, @csala and @ManuelAlvarezC
-* Option to select seed on random number generator - Issue [#63](https://github.com/sdv-dev/Copulas/issues/63) by @echo66 and @ManuelAlvarezC
-* Option on Vine copulas to select number of rows to sample - Issue [#77](https://github.com/sdv-dev/Copulas/issues/77) by @ManuelAlvarezC
-* Make copulas accept both scalars and arrays as arguments - Issues [#85](https://github.com/sdv-dev/Copulas/issues/85) and [#90](https://github.com/sdv-dev/Copulas/issues/90) by @ManuelAlvarezC
-
-### General Improvements
-
-* Ability to properly handle constant data - Issues [#57](https://github.com/sdv-dev/Copulas/issues/57) and [#82](https://github.com/sdv-dev/Copulas/issues/82) by @csala and @ManuelAlvarezC
-* Tests for analytics properties of copulas - Issue [#61](https://github.com/sdv-dev/Copulas/issues/61) by @ManuelAlvarezC
-* Improved documentation - Issue [#96](https://github.com/sdv-dev/Copulas/issues/96) by @ManuelAlvarezC
-
-### Bugs fixed
-
-* Fix bug on Vine copulas, that made it crash during the bivariate copula selection - Issue [#64](https://github.com/sdv-dev/Copulas/issues/64) by @echo66 and @ManuelAlvarezC
-
-## v0.2.1 - Vine serialization
-
-* Add serialization to Vine copulas.
-* Add `distribution` as argument for the Gaussian Copula.
-* Improve Bivariate Copulas code structure to remove code duplication.
-* Fix bug in Vine Copulas sampling: 'Edge' object has no attribute 'index'
-* Improve code documentation.
-* Improve code style and linting tools configuration.
-
-## v0.2.0 - Unified API
-
-* New API for stats methods.
-* Standarize input and output to `numpy.ndarray`.
-* Increase unittest coverage to 90%.
-* Add methods to load/save copulas.
-* Improve Gaussian copula sampling accuracy.
-
-## v0.1.1 - Minor Improvements
-
-* Different Copula types separated in subclasses
-* Extensive Unit Testing
-* More pythonic names in the public API.
-* Stop using third party elements that will be deprected soon.
-* Add methods to sample new data on bivariate copulas.
-* New KDE Univariate copula
-* Improved examples with additional demo data.
-
-## v0.1.0 - First Release
-
-* First release on PyPI.
```

#### html2text {}

```diff
@@ -1,20 +1,11 @@
-Metadata-Version: 2.1 Name: copulas Version: 0.8.0.dev0 Summary: Create tabular
+Metadata-Version: 2.1 Name: copulas Version: 0.8.1.dev0 Summary: Create tabular
 synthetic data using copulas-based modeling. Home-page: https://github.com/sdv-
 dev/Copulas Author: DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1
-Keywords: copulas Classifier: Development Status :: 2 - Pre-Alpha Classifier:
-Intended Audience :: Developers Classifier: License :: Free for non-commercial
-use Classifier: Natural Language :: English Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.7,<3.12
-Description-Content-Type: text/markdown Provides-Extra: tutorials Provides-
-Extra: test Provides-Extra: dev License-File: LICENSE License-File: AUTHORS.rst
+Description:
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
 [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--
 %20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-
 +Pre-Alpha) [![PyPi Shield](https://img.shields.io/pypi/v/copulas.svg)](https:/
 /pypi.python.org/pypi/copulas) [![Downloads](https://pepy.tech/badge/copulas)]
@@ -76,17 +67,23 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## v0.7.0 - 2022-05-10 This release
-adds `gaussian` as a fallback distribution in case the user specified one
-fails. It also improves the `fit` of the `beta` distribution by properly
+libraries for specific needs. # History ## v0.8.0 - 2023-01-06 This release
+adds support for python 3.10 and 3.11. Additionally, it drops support for
+python 3.6. ### Maintenance * Support python 3.10 and above - PR[#338](https://
+github.com/sdv-dev/Copulas/pull/338) by @pvk-developer * Copulas Package
+Maintenance Updates - Issue[#336](https://github.com/sdv-dev/Copulas/issues/
+336) by @pvk-developer * Add support for python 3.10 - PR[#329](https://
+github.com/sdv-dev/Copulas/pull/329) by @katxiao ## v0.7.0 - 2022-05-10 This
+release adds `gaussian` as a fallback distribution in case the user specified
+one fails. It also improves the `fit` of the `beta` distribution by properly
 estimatig the `loc` and `scale` parameters. ### General Improvements * Add
 gaussian as fallback - Issue[#320](https://github.com/sdv-dev/Copulas/issues/
 320) by @fealho * Improve the fit of the Beta distribution: Use the new loc and
 scale - Issue[#317](https://github.com/sdv-dev/Copulas/issues/317) by @pvk-
 developer ## v0.6.1 - 2022-02-25 This release improves the `random_state`
 functionality by taking in RandomState objects in addition to random seeds. ###
 General Improvements * Use random_state instead of random_seed - Issue[#113]
@@ -198,7 +195,17 @@
 `numpy.ndarray`. * Increase unittest coverage to 90%. * Add methods to load/
 save copulas. * Improve Gaussian copula sampling accuracy. ## v0.1.1 - Minor
 Improvements * Different Copula types separated in subclasses * Extensive Unit
 Testing * More pythonic names in the public API. * Stop using third party
 elements that will be deprected soon. * Add methods to sample new data on
 bivariate copulas. * New KDE Univariate copula * Improved examples with
 additional demo data. ## v0.1.0 - First Release * First release on PyPI.
+Keywords: copulas Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-
+Alpha Classifier: Intended Audience :: Developers Classifier: License :: Free
+for non-commercial use Classifier: Natural Language :: English Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
+>=3.7,<3.12 Description-Content-Type: text/markdown Provides-Extra: tutorials
+Provides-Extra: test Provides-Extra: dev
```

### Comparing `copulas-0.8.0.dev0/copulas.egg-info/SOURCES.txt` & `copulas-0.8.1.dev0/copulas.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 LICENSE
 MANIFEST.in
 README.md
 RELEASE.md
 setup.cfg
 setup.py
 copulas/__init__.py
+copulas/_addons.py
 copulas/datasets.py
 copulas/visualization.py
 copulas.egg-info/PKG-INFO
 copulas.egg-info/SOURCES.txt
 copulas.egg-info/dependency_links.txt
 copulas.egg-info/not-zip-safe
 copulas.egg-info/requires.txt
@@ -147,14 +148,15 @@
 tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_1.json
 tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_2.json
 tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_3.json
 tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_1.json
 tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_2.json
 tests/unit/__init__.py
 tests/unit/test___init__.py
+tests/unit/test__addons.py
 tests/unit/bivariate/__init__.py
 tests/unit/bivariate/test___init__.py
 tests/unit/bivariate/test_base.py
 tests/unit/bivariate/test_clayton.py
 tests/unit/bivariate/test_frank.py
 tests/unit/bivariate/test_gumbel.py
 tests/unit/bivariate/test_independence.py
```

### Comparing `copulas-0.8.0.dev0/copulas.egg-info/requires.txt` & `copulas-0.8.1.dev0/copulas.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 
 [:python_version < "3.10"]
 numpy<2,>=1.20.0
-pandas<2,>=1.1.3
+pandas>=1.1.3
 scipy<2,>=1.5.4
 
 [:python_version >= "3.10"]
 matplotlib<4,>=3.6.0
 numpy<2,>=1.23.3
 scipy<2,>=1.9.2
 
 [:python_version >= "3.10" and python_version < "3.11"]
-pandas<2,>=1.3.4
+pandas>=1.3.4
 
 [:python_version >= "3.11"]
-pandas<2,>=1.5.0
+pandas>=1.5.0
 
 [:python_version >= "3.7" and python_version < "3.10"]
 matplotlib<4,>=3.4.0
 
 [dev]
 pytest<7,>=6.2.5
 pytest-cov<3,>=2.6.0
```

### Comparing `copulas-0.8.0.dev0/docs/Makefile` & `copulas-0.8.1.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/docs/conf.py` & `copulas-0.8.1.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/docs/images/copulas-200.png` & `copulas-0.8.1.dev0/docs/images/copulas-200.png`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/docs/images/copulas.png` & `copulas-0.8.1.dev0/docs/images/copulas.png`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/docs/images/copulas_sample_dataset.png` & `copulas-0.8.1.dev0/docs/images/copulas_sample_dataset.png`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/docs/images/dai-logo-white.png` & `copulas-0.8.1.dev0/docs/images/dai-logo-white.png`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/docs/images/dice_cdf.png` & `copulas-0.8.1.dev0/docs/images/dice_cdf.png`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/docs/images/pdf_cdf.png` & `copulas-0.8.1.dev0/docs/images/pdf_cdf.png`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/docs/images/pit.png` & `copulas-0.8.1.dev0/docs/images/pit.png`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/docs/images/quickstart.png` & `copulas-0.8.1.dev0/docs/images/quickstart.png`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/docs/index.rst` & `copulas-0.8.1.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/docs/make.bat` & `copulas-0.8.1.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/setup.cfg` & `copulas-0.8.1.dev0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.8.0.dev0
+current_version = 0.8.1.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `copulas-0.8.0.dev0/setup.py` & `copulas-0.8.1.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     history = history_file.read()
 
 install_requires = [
     "matplotlib>=3.4.0,<4;python_version>='3.7' and python_version<'3.10'",
     "matplotlib>=3.6.0,<4;python_version>='3.10'",
     "numpy>=1.20.0,<2;python_version<'3.10'",
     "numpy>=1.23.3,<2;python_version>='3.10'",
-    "pandas>=1.1.3,<2;python_version<'3.10'",
-    "pandas>=1.3.4,<2;python_version>='3.10' and python_version<'3.11'",
-    "pandas>=1.5.0,<2;python_version>='3.11'",
+    "pandas>=1.1.3;python_version<'3.10'",
+    "pandas>=1.3.4;python_version>='3.10' and python_version<'3.11'",
+    "pandas>=1.5.0;python_version>='3.11'",
     "scipy>=1.5.4,<2;python_version<'3.10'",
     "scipy>=1.9.2,<2;python_version>='3.10'",
 ]
 
 development_requires = [
     # general
     'pip>=9.0.1',
@@ -133,10 +133,10 @@
     name='copulas',
     packages=find_packages(include=['copulas', 'copulas.*']),
     python_requires='>=3.7,<3.12',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/Copulas',
-    version='0.8.0.dev0',
+    version='0.8.1.dev0',
     zip_safe=False,
 )
```

### Comparing `copulas-0.8.0.dev0/tests/__init__.py` & `copulas-0.8.1.dev0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/end-to-end/README.md` & `copulas-0.8.1.dev0/tests/end-to-end/README.md`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/end-to-end/bivariate/test_base.py` & `copulas-0.8.1.dev0/tests/end-to-end/bivariate/test_base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/end-to-end/multivariate/test_base.py` & `copulas-0.8.1.dev0/tests/end-to-end/multivariate/test_base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/end-to-end/multivariate/test_gaussian.py` & `copulas-0.8.1.dev0/tests/end-to-end/multivariate/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/end-to-end/multivariate/test_vine.py` & `copulas-0.8.1.dev0/tests/end-to-end/multivariate/test_vine.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/end-to-end/test___init__.py` & `copulas-0.8.1.dev0/tests/end-to-end/test___init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/end-to-end/univariate/test_beta.py` & `copulas-0.8.1.dev0/tests/end-to-end/univariate/test_beta.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/end-to-end/univariate/test_gamma.py` & `copulas-0.8.1.dev0/tests/end-to-end/univariate/test_gamma.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/end-to-end/univariate/test_gaussian.py` & `copulas-0.8.1.dev0/tests/end-to-end/univariate/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/end-to-end/univariate/test_gaussian_kde.py` & `copulas-0.8.1.dev0/tests/end-to-end/univariate/test_gaussian_kde.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/end-to-end/univariate/test_student_t.py` & `copulas-0.8.1.dev0/tests/end-to-end/univariate/test_student_t.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/end-to-end/univariate/test_truncated_gaussian.py` & `copulas-0.8.1.dev0/tests/end-to-end/univariate/test_truncated_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/large_scale_evaluation.py` & `copulas-0.8.1.dev0/tests/large_scale_evaluation.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/README.md` & `copulas-0.8.1.dev0/tests/numerical/README.md`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/cdf/scripts/bivariate_cdf_input.py` & `copulas-0.8.1.dev0/tests/numerical/cdf/scripts/bivariate_cdf_input.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/cdf/scripts/bivariate_cdf_output.R` & `copulas-0.8.1.dev0/tests/numerical/cdf/scripts/bivariate_cdf_output.R`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/cdf/scripts/bivariate_cdf_output.m` & `copulas-0.8.1.dev0/tests/numerical/cdf/scripts/bivariate_cdf_output.m`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_1.json` & `copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_2.json` & `copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_3.json` & `copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_3.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_1.json` & `copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_2.json` & `copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_3.json` & `copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_3.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_1.json` & `copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_2.json` & `copulas-0.8.1.dev0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/cdf/test_cdf.py` & `copulas-0.8.1.dev0/tests/numerical/cdf/test_cdf.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/fit/scripts/bivariate_fit_output.R` & `copulas-0.8.1.dev0/tests/numerical/fit/scripts/bivariate_fit_output.R`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/fit/scripts/bivariate_fit_output.m` & `copulas-0.8.1.dev0/tests/numerical/fit/scripts/bivariate_fit_output.m`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_1.json` & `copulas-0.8.1.dev0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_2.json` & `copulas-0.8.1.dev0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_1.json` & `copulas-0.8.1.dev0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_2.json` & `copulas-0.8.1.dev0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_1.json` & `copulas-0.8.1.dev0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_2.json` & `copulas-0.8.1.dev0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/fit/test_fit.py` & `copulas-0.8.1.dev0/tests/numerical/fit/test_fit.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/pdf/scripts/bivariate_pdf_input.py` & `copulas-0.8.1.dev0/tests/numerical/pdf/scripts/bivariate_pdf_input.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/pdf/scripts/bivariate_pdf_output.R` & `copulas-0.8.1.dev0/tests/numerical/pdf/scripts/bivariate_pdf_output.R`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/pdf/scripts/bivariate_pdf_output.m` & `copulas-0.8.1.dev0/tests/numerical/pdf/scripts/bivariate_pdf_output.m`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_1.json` & `copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_2.json` & `copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_3.json` & `copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_3.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_1.json` & `copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_2.json` & `copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_3.json` & `copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_3.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_1.json` & `copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_2.json` & `copulas-0.8.1.dev0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/numerical/pdf/test_pdf.py` & `copulas-0.8.1.dev0/tests/numerical/pdf/test_pdf.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/bivariate/test_base.py` & `copulas-0.8.1.dev0/tests/unit/bivariate/test_base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/bivariate/test_clayton.py` & `copulas-0.8.1.dev0/tests/unit/bivariate/test_clayton.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/bivariate/test_frank.py` & `copulas-0.8.1.dev0/tests/unit/bivariate/test_frank.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/bivariate/test_gumbel.py` & `copulas-0.8.1.dev0/tests/unit/bivariate/test_gumbel.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/bivariate/test_independence.py` & `copulas-0.8.1.dev0/tests/unit/bivariate/test_independence.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/multivariate/test_gaussian.py` & `copulas-0.8.1.dev0/tests/unit/multivariate/test_gaussian.py`

 * *Files 6% similar despite different names*

```diff
@@ -181,46 +181,46 @@
         np.testing.assert_allclose(expected, passed)
 
         assert dist_b.cdf.call_count == 1
         expected = np.array([5, 6, 7])
         passed = dist_b.cdf.call_args[0][0]
         np.testing.assert_allclose(expected, passed)
 
-    def test__get_covariance(self):
-        """_get_covariance computes the covariance matrix of normalized values."""
+    def test__get_correlation(self):
+        """_get_correlation computes the correlation matrix of normalized values."""
         # Setup
         copula = GaussianMultivariate(GaussianUnivariate)
         copula.fit(self.data)
 
-        expected_covariance = np.array([
+        expected_correlation = np.array([
             [1., -0.01261819, -0.19821644],
             [-0.01261819, 1., -0.16896087],
             [-0.19821644, -0.16896087, 1.]
         ])
 
         # Run
-        covariance = copula._get_covariance(self.data)
+        correlation = copula._get_correlation(self.data)
 
         # Check
-        assert np.isclose(covariance, expected_covariance).all().all()
+        assert np.isclose(correlation, expected_correlation).all().all()
 
     def test_fit_default_distribution(self):
-        """On fit, a distribution is created for each column along the covariance and means"""
+        """On fit, a distribution is created for each column along the correlation and means"""
 
         copula = GaussianMultivariate(GaussianUnivariate)
         copula.fit(self.data)
 
         for i, key in enumerate(self.data.columns):
             assert copula.columns[i] == key
             assert copula.univariates[i].__class__ == GaussianUnivariate
             assert copula.univariates[i]._params['loc'] == self.data[key].mean()
             assert copula.univariates[i]._params['scale'] == np.std(self.data[key])
 
-        expected_covariance = copula._get_covariance(self.data)
-        assert (copula.covariance == expected_covariance).all().all()
+        expected_correlation = copula._get_correlation(self.data)
+        assert (copula.correlation == expected_correlation).all().all()
 
     def test_fit_distribution_arg(self):
         """On fit, the distributions for each column use instances of copula.distribution."""
         # Setup
         distribution = 'copulas.univariate.gaussian_kde.GaussianKDE'
         copula = GaussianMultivariate(distribution=distribution)
 
@@ -230,16 +230,16 @@
         # Check
         assert copula.distribution == 'copulas.univariate.gaussian_kde.GaussianKDE'
 
         for i, key in enumerate(self.data.columns):
             assert copula.columns[i] == key
             assert get_qualified_name(copula.univariates[i].__class__) == copula.distribution
 
-        expected_covariance = copula._get_covariance(self.data)
-        assert (copula.covariance == expected_covariance).all().all()
+        expected_correlation = copula._get_correlation(self.data)
+        assert (copula.correlation == expected_correlation).all().all()
 
     def test_fit_distribution_selector(self):
         """
         On fit, it should use the correct distributions for those that are
         specified and default to using the base class otherwise.
         """
         copula = GaussianMultivariate(distribution={
@@ -265,16 +265,16 @@
         copula.fit(self.data.to_numpy())
 
         # Check
         for key, (column, univariate) in enumerate(zip(self.data.columns, copula.univariates)):
             assert univariate._params['loc'] == np.mean(self.data[column])
             assert univariate._params['scale'] == np.std(self.data[column])
 
-        expected_covariance = copula._get_covariance(pd.DataFrame(self.data.to_numpy()))
-        assert (copula.covariance == expected_covariance).all().all()
+        expected_correlation = copula._get_correlation(pd.DataFrame(self.data.to_numpy()))
+        assert (copula.correlation == expected_correlation).all().all()
 
     @patch('copulas.univariate.truncated_gaussian.TruncatedGaussian._fit')
     @patch('copulas.multivariate.gaussian.warnings')
     def test_fit_broken_distribution(self, warnings_mock, truncated_mock):
         """Fit should use a gaussian if the passed distribution crashes."""
         # Setup
         truncated_mock.side_effect = ValueError()
@@ -386,16 +386,16 @@
         # Run
         result = instance.sample(5)
 
         # Check
         assert result.equals(expected_result)
 
         assert normal_mock.called_once_with(
-            np.zeros(instance.covariance.shape[0]),
-            instance.covariance,
+            np.zeros(instance.correlation.shape[0]),
+            instance.correlation,
             5
         )
 
     def test_sample_random_state(self):
         """When random_state is set the samples are the same."""
         # Setup
         instance = GaussianMultivariate(GaussianUnivariate, random_state=0)
@@ -419,15 +419,15 @@
             columns=['A', 'B', 'C']
         )
 
         # Run
         result = instance.sample(5)
 
         # Check
-        pd.testing.assert_frame_equal(result, expected_result, check_less_precise=True)
+        pd.testing.assert_frame_equal(result, expected_result)
 
     def test_to_dict(self):
         """To_dict returns the parameters to replicate the copula."""
         # Setup
         copula = GaussianMultivariate()
         copula.fit(self.data)
 
@@ -435,16 +435,16 @@
         result = copula.to_dict()
 
         # Asserts
         assert result['type'] == 'copulas.multivariate.gaussian.GaussianMultivariate'
         assert result['columns'] == ['column1', 'column2', 'column3']
         assert len(result['univariates']) == 3
 
-        expected_cov = copula._get_covariance(self.data).to_numpy().tolist()
-        np.testing.assert_equal(result['covariance'], expected_cov)
+        expected_cov = copula._get_correlation(self.data).to_numpy().tolist()
+        np.testing.assert_equal(result['correlation'], expected_cov)
 
         for univariate, result_univariate in zip(copula.univariates, result['univariates']):
             assert univariate.to_dict() == result_univariate
 
     def test_from_dict(self):
         """from_dict generates a new instance from its parameters."""
         # Setup
@@ -462,15 +462,15 @@
 
         for new_univariate, old_univariate in zip(copula.univariates, new_copula.univariates):
             assert new_univariate.to_dict() == old_univariate.to_dict()
 
     def test_sample_constant_column(self):
         """Gaussian copula can sample after being fit with a constant column.
 
-        This process will raise warnings when computing the covariance matrix
+        This process will raise warnings when computing the correlation matrix
         """
         # Setup
         instance = GaussianMultivariate()
         X = np.array([
             [1.0, 2.0],
             [1.0, 3.0],
             [1.0, 4.0],
@@ -486,20 +486,20 @@
         results = result[~result.isna()].all()
         assert results.all()
         assert result.loc[:, 0].equals(pd.Series([1.0, 1.0, 1.0, 1.0, 1.0], name=0))
 
         # This is to check that the samples on the non constant column are not constant too.
         assert len(result.loc[:, 1].unique()) > 1
 
-        covariance = instance.covariance
-        assert (~pd.isna(covariance)).all().all()
+        correlation = instance.correlation
+        assert (~pd.isna(correlation)).all().all()
 
     def test__get_conditional_distribution(self):
         gm = GaussianMultivariate()
-        gm.covariance = pd.DataFrame({
+        gm.correlation = pd.DataFrame({
             'a': [1, 0.2, 0.3],
             'b': [0.2, 1, 0.4],
             'c': [0.3, 0.4, 1],
         }, index=['a', 'b', 'c'])
 
         conditions = pd.Series({
             'b': 1
```

### Comparing `copulas-0.8.0.dev0/tests/unit/multivariate/test_tree.py` & `copulas-0.8.1.dev0/tests/unit/multivariate/test_tree.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/multivariate/test_vine.py` & `copulas-0.8.1.dev0/tests/unit/multivariate/test_vine.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/optimize/test___init__.py` & `copulas-0.8.1.dev0/tests/unit/optimize/test___init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/test___init__.py` & `copulas-0.8.1.dev0/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/univariate/test_base.py` & `copulas-0.8.1.dev0/tests/unit/univariate/test_base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/univariate/test_beta.py` & `copulas-0.8.1.dev0/tests/unit/univariate/test_beta.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/univariate/test_gamma.py` & `copulas-0.8.1.dev0/tests/unit/univariate/test_gamma.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/univariate/test_gaussian.py` & `copulas-0.8.1.dev0/tests/unit/univariate/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/univariate/test_gaussian_kde.py` & `copulas-0.8.1.dev0/tests/unit/univariate/test_gaussian_kde.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/univariate/test_log_laplace.py` & `copulas-0.8.1.dev0/tests/unit/univariate/test_log_laplace.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/univariate/test_selection.py` & `copulas-0.8.1.dev0/tests/unit/univariate/test_selection.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/univariate/test_student_t.py` & `copulas-0.8.1.dev0/tests/unit/univariate/test_student_t.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/univariate/test_truncated_gaussian.py` & `copulas-0.8.1.dev0/tests/unit/univariate/test_truncated_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.8.0.dev0/tests/unit/univariate/test_uniform.py` & `copulas-0.8.1.dev0/tests/unit/univariate/test_uniform.py`

 * *Files identical despite different names*

