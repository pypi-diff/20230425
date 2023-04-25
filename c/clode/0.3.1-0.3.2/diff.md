# Comparing `tmp/clode-0.3.1.tar.gz` & `tmp/clode-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clode-0.3.1.tar", last modified: Wed Apr  5 17:31:12 2023, max compression
+gzip compressed data, was "clode-0.3.2.tar", last modified: Tue Apr 25 02:06:26 2023, max compression
```

## Comparing `clode-0.3.1.tar` & `clode-0.3.2.tar`

### file list

```diff
@@ -1,198 +1,199 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.757133 clode-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-05 17:29:08.000000 clode-0.3.1/.bazeliskrc
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-05 17:29:08.000000 clode-0.3.1/.bazelversion
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-05 17:29:08.000000 clode-0.3.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.737133 clode-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.741133 clode-0.3.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-05 17:29:08.000000 clode-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-05 17:29:08.000000 clode-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.741133 clode-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-05 17:29:08.000000 clode-0.3.1/.github/workflows/bazel_build_linux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-05 17:29:08.000000 clode-0.3.1/.github/workflows/bazel_build_windows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-05 17:29:08.000000 clode-0.3.1/.github/workflows/bazel_test_mac.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-05 17:29:08.000000 clode-0.3.1/.github/workflows/draft_pdf.yml
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-05 17:29:08.000000 clode-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 17:29:08.000000 clode-0.3.1/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-05 17:29:08.000000 clode-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-05 17:29:08.000000 clode-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-05 17:29:08.000000 clode-0.3.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-05 17:31:12.757133 clode-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-05 17:29:08.000000 clode-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-05 17:29:08.000000 clode-0.3.1/WORKSPACE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.741133 clode-0.3.1/bazel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/clode_http_archive.bzl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.741133 clode-0.3.1/bazel/external/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/external/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/external/fmtlib.BUILD
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/external/opencl_windows.BUILD
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/external/pybind11.BUILD
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/external/python.BUILD
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/external/spdlog.BUILD
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/external_deps.bzl
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/get_python_libs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.741133 clode-0.3.1/bazel/python/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/python/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/python/BUILD.tpl
--rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/python/python.bzl
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/python/python_native.bzl
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/python/variety.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.741133 clode-0.3.1/bazel/remote_config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/remote_config/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/remote_config/common.bzl
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/repositories.bzl
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/repository_locations.bzl
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-05 17:29:08.000000 clode-0.3.1/bazel/repository_locations_utils.bzl
--rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-04-05 17:29:08.000000 clode-0.3.1/bazelisk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.741133 clode-0.3.1/clode/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-05 17:29:08.000000 clode-0.3.1/clode/BUILD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.745133 clode-0.3.1/clode/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)    16729 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/CLODE.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/CLODE.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/CLODEfeatures.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/CLODEfeatures.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/CLODEpython.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/CLODEtrajectory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/CLODEtrajectory.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.745133 clode-0.3.1/clode/cpp/OpenCL/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/OpenCL/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)   299120 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/OpenCL/cl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   326155 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/OpenCL/cl2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/OpenCLResource.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/OpenCLResource.hpp
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/clODE_random.cl
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/clODE_struct_defs.cl
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/clODE_utilities.cl
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/features.cl
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/initializeObserver.cl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.745133 clode-0.3.1/clode/cpp/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/logging/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/logging/MatlabSink.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/logging/PythonSink.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.749133 clode-0.3.1/clode/cpp/observers/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/observers/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/observers/observer_basic.clh
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/observers/observer_basic_allVar.clh
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/observers/observer_local_maximum.clh
--rw-r--r--   0 runner    (1001) docker     (123)    14594 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/observers/observer_neighborhood_1.clh
--rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/observers/observer_neighborhood_2.clh
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/observers/observer_template.clh
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/observers/observer_threshold_1.clh
--rw-r--r--   0 runner    (1001) docker     (123)    17373 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/observers/observer_threshold_2.clh
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/observers.cl
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/odedriver.cl
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/realtype.cl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.749133 clode-0.3.1/clode/cpp/steppers/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/steppers/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/steppers/adaptive_bs23.clh
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/steppers/adaptive_dp45.clh
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/steppers/adaptive_explicit_step.clh
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/steppers/adaptive_he12.clh
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/steppers/adaptive_rkck.clh
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/steppers/fixed_explicit_Euler.clh
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/steppers/fixed_explicit_RK4.clh
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/steppers/fixed_explicit_Trapezoidal.clh
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/steppers/fixed_explicit_step.clh
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/steppers/fixed_explicit_stochastic_Euler.clh
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/steppers.cl
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/trajectory.cl
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-05 17:29:08.000000 clode-0.3.1/clode/cpp/transient.cl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.749133 clode-0.3.1/clode/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-05 17:29:08.000000 clode-0.3.1/clode/python/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-05 17:29:08.000000 clode-0.3.1/clode/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-04-05 17:29:08.000000 clode-0.3.1/clode/python/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-05 17:29:08.000000 clode-0.3.1/clode/python/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-05 17:29:08.000000 clode-0.3.1/clode/python/problem_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-05 17:29:08.000000 clode-0.3.1/clode/python/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-05 17:29:08.000000 clode-0.3.1/clode/python/solver_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-05 17:29:08.000000 clode-0.3.1/clode/python/stepper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-05 17:29:08.000000 clode-0.3.1/clode/python/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-05 17:29:08.000000 clode-0.3.1/clode/python/xpp_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.745133 clode-0.3.1/clode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-05 17:31:12.000000 clode-0.3.1/clode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-04-05 17:31:12.000000 clode-0.3.1/clode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 17:31:12.000000 clode-0.3.1/clode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-05 17:31:12.000000 clode-0.3.1/clode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.749133 clode-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-05 17:29:08.000000 clode-0.3.1/docs/feature_extraction.md
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-05 17:29:08.000000 clode-0.3.1/docs/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-05 17:29:08.000000 clode-0.3.1/docs/install.md
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-04-05 17:29:08.000000 clode-0.3.1/docs/matlab.md
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-05 17:29:08.000000 clode-0.3.1/docs/querying_opencl.md
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-05 17:29:08.000000 clode-0.3.1/docs/trajectory_simulation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-05 17:29:08.000000 clode-0.3.1/docs/xpp_files.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.753133 clode-0.3.1/matlab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/Chart.m
--rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/GridSimulation.m
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/InitialValueProblem.m
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/clODE.m
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/clODEfeatures.m
--rw-r--r--   0 runner    (1001) docker     (123)    15984 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/clODEfeaturesmex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/clODEmex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/clODEmexHelpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/clODEtrajectory.m
--rw-r--r--   0 runner    (1001) docker     (123)    14195 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/clODEtrajectorymex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/clickTrajectory.m
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/compileCLODEmex.m
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/cppclass.m
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/functionSignatures.json
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/generate_pointset.m
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/gridKeyPress.m
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/gridfigure.m
--rw-r--r--   0 runner    (1001) docker     (123)    91034 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/gridtool.m
--rw-r--r--   0 runner    (1001) docker     (123)    84265 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/gridtool_old.m
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/plot_twopar.m
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/queryOpenCL.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-05 17:29:08.000000 clode-0.3.1/matlab/trajectoryfigure.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.753133 clode-0.3.1/paper/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-05 17:29:08.000000 clode-0.3.1/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-05 17:29:08.000000 clode-0.3.1/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-05 17:29:08.000000 clode-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-05 17:29:08.000000 clode-0.3.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-05 17:29:08.000000 clode-0.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.757133 clode-0.3.1/samples/
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-05 17:29:08.000000 clode-0.3.1/samples/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-05 17:29:08.000000 clode-0.3.1/samples/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-05 17:29:08.000000 clode-0.3.1/samples/lacto_more_vars.cl
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-05 17:29:08.000000 clode-0.3.1/samples/lactotroph.cl
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-05 17:29:08.000000 clode-0.3.1/samples/lactotroph.ode
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-05 17:29:08.000000 clode-0.3.1/samples/lactotroph_noise.cl
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-05 17:29:08.000000 clode-0.3.1/samples/lactotroph_noise.ode
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-05 17:29:08.000000 clode-0.3.1/samples/listOpenCL.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-05 17:29:08.000000 clode-0.3.1/samples/plot_twopar.m
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-04-05 17:29:08.000000 clode-0.3.1/samples/run_twopar.m
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-05 17:29:08.000000 clode-0.3.1/samples/test.cl
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-05 17:29:08.000000 clode-0.3.1/samples/testCLODE.m
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-05 17:29:08.000000 clode-0.3.1/samples/testCLODEfeatures.m
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-05 17:29:08.000000 clode-0.3.1/samples/testCLODEmex.m
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-05 17:29:08.000000 clode-0.3.1/samples/testCLODEtrajectory.m
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-05 17:29:08.000000 clode-0.3.1/samples/testFeatures.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-05 17:29:08.000000 clode-0.3.1/samples/testFeatures_morevars.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-04-05 17:29:08.000000 clode-0.3.1/samples/testTrajectory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-05 17:29:08.000000 clode-0.3.1/samples/testTransient.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-04-05 17:29:08.000000 clode-0.3.1/samples/test_outputs_cpp.md
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-05 17:29:08.000000 clode-0.3.1/samples/windowsCompileListOpenCL.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 17:31:12.757133 clode-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-04-05 17:29:08.000000 clode-0.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-05 17:29:08.000000 clode-0.3.1/shell.nix
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.757133 clode-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 17:29:08.000000 clode-0.3.1/test/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 17:29:08.000000 clode-0.3.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-05 17:29:08.000000 clode-0.3.1/test/ornl_thompson_a1.cl
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-05 17:29:08.000000 clode-0.3.1/test/test.cl
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-05 17:29:08.000000 clode-0.3.1/test/test_lactotroph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-05 17:29:08.000000 clode-0.3.1/test/test_lactotroph_more_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-05 17:29:08.000000 clode-0.3.1/test/test_lactotroph_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-05 17:29:08.000000 clode-0.3.1/test/test_ornl_thompson_a1.py
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-04-05 17:29:08.000000 clode-0.3.1/test/test_pituitary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-05 17:29:08.000000 clode-0.3.1/test/test_vdp.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-05 17:29:08.000000 clode-0.3.1/test/test_vdp_long.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-05 17:29:08.000000 clode-0.3.1/test/text_xpp_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-05 17:29:08.000000 clode-0.3.1/test/van_der_pol_oscillator.cl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:31:12.757133 clode-0.3.1/test/xpp/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-05 17:29:08.000000 clode-0.3.1/test/xpp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-05 17:29:08.000000 clode-0.3.1/test/xpp/van_der_pol_oscillator.xpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.605488 clode-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 02:04:30.000000 clode-0.3.2/.bazeliskrc
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 02:04:30.000000 clode-0.3.2/.bazelversion
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-25 02:04:30.000000 clode-0.3.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.589488 clode-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.589488 clode-0.3.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-25 02:04:30.000000 clode-0.3.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 02:04:30.000000 clode-0.3.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.589488 clode-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-25 02:04:30.000000 clode-0.3.2/.github/workflows/bazel_build_linux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-25 02:04:30.000000 clode-0.3.2/.github/workflows/bazel_build_windows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-25 02:04:30.000000 clode-0.3.2/.github/workflows/bazel_test_mac.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-25 02:04:30.000000 clode-0.3.2/.github/workflows/draft_pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-25 02:04:30.000000 clode-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:04:30.000000 clode-0.3.2/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-25 02:04:30.000000 clode-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-25 02:04:30.000000 clode-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-25 02:04:30.000000 clode-0.3.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-25 02:06:26.605488 clode-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-25 02:04:30.000000 clode-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-25 02:04:30.000000 clode-0.3.2/WORKSPACE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.593488 clode-0.3.2/bazel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/clode_http_archive.bzl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.593488 clode-0.3.2/bazel/external/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/external/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/external/fmtlib.BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/external/opencl_windows.BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/external/pybind11.BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/external/python.BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/external/spdlog.BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/external_deps.bzl
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/get_python_libs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.593488 clode-0.3.2/bazel/python/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/python/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/python/BUILD.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/python/python.bzl
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/python/python_native.bzl
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/python/variety.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.593488 clode-0.3.2/bazel/remote_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/remote_config/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/remote_config/common.bzl
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/repositories.bzl
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/repository_locations.bzl
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-25 02:04:30.000000 clode-0.3.2/bazel/repository_locations_utils.bzl
+-rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-04-25 02:04:30.000000 clode-0.3.2/bazelisk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.593488 clode-0.3.2/clode/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-25 02:04:30.000000 clode-0.3.2/clode/BUILD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.597488 clode-0.3.2/clode/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/CLODE.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/CLODE.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/CLODEfeatures.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/CLODEfeatures.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/CLODEpython.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/CLODEtrajectory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/CLODEtrajectory.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.597488 clode-0.3.2/clode/cpp/OpenCL/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/OpenCL/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)   299120 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/OpenCL/cl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   326155 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/OpenCL/cl2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/OpenCLResource.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/OpenCLResource.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/clODE_random.cl
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/clODE_struct_defs.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/clODE_utilities.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/features.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/initializeObserver.cl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.597488 clode-0.3.2/clode/cpp/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/logging/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/logging/MatlabSink.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/logging/PythonSink.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.597488 clode-0.3.2/clode/cpp/observers/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/observers/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/observers/observer_basic.clh
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/observers/observer_basic_allVar.clh
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/observers/observer_local_maximum.clh
+-rw-r--r--   0 runner    (1001) docker     (123)    14594 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/observers/observer_neighborhood_1.clh
+-rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/observers/observer_neighborhood_2.clh
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/observers/observer_template.clh
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/observers/observer_threshold_1.clh
+-rw-r--r--   0 runner    (1001) docker     (123)    17373 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/observers/observer_threshold_2.clh
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/observers.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/odedriver.cl
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/realtype.cl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.597488 clode-0.3.2/clode/cpp/steppers/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/steppers/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/steppers/adaptive_bs23.clh
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/steppers/adaptive_dp45.clh
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/steppers/adaptive_explicit_step.clh
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/steppers/adaptive_he12.clh
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/steppers/adaptive_rkck.clh
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/steppers/fixed_explicit_Euler.clh
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/steppers/fixed_explicit_RK4.clh
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/steppers/fixed_explicit_Trapezoidal.clh
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/steppers/fixed_explicit_step.clh
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/steppers/fixed_explicit_stochastic_Euler.clh
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/steppers.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/trajectory.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-25 02:04:30.000000 clode-0.3.2/clode/cpp/transient.cl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.601488 clode-0.3.2/clode/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-25 02:04:30.000000 clode-0.3.2/clode/python/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-25 02:04:30.000000 clode-0.3.2/clode/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-04-25 02:04:30.000000 clode-0.3.2/clode/python/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-25 02:04:30.000000 clode-0.3.2/clode/python/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-25 02:04:30.000000 clode-0.3.2/clode/python/problem_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-25 02:04:30.000000 clode-0.3.2/clode/python/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 02:04:30.000000 clode-0.3.2/clode/python/solver_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-25 02:04:30.000000 clode-0.3.2/clode/python/stepper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-25 02:04:30.000000 clode-0.3.2/clode/python/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-25 02:04:30.000000 clode-0.3.2/clode/python/xpp_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.593488 clode-0.3.2/clode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-25 02:06:26.000000 clode-0.3.2/clode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-04-25 02:06:26.000000 clode-0.3.2/clode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 02:06:26.000000 clode-0.3.2/clode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-25 02:06:26.000000 clode-0.3.2/clode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.601488 clode-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-25 02:04:30.000000 clode-0.3.2/docs/feature_extraction.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-25 02:04:30.000000 clode-0.3.2/docs/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-25 02:04:30.000000 clode-0.3.2/docs/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-04-25 02:04:30.000000 clode-0.3.2/docs/matlab.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-25 02:04:30.000000 clode-0.3.2/docs/querying_opencl.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-25 02:04:30.000000 clode-0.3.2/docs/trajectory_simulation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-25 02:04:30.000000 clode-0.3.2/docs/xpp_files.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.601488 clode-0.3.2/matlab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/Chart.m
+-rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/GridSimulation.m
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/InitialValueProblem.m
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/clODE.m
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/clODEfeatures.m
+-rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/clODEfeaturesmex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/clODEmex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/clODEmexHelpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/clODEtrajectory.m
+-rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/clODEtrajectorymex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/clickTrajectory.m
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/compileCLODEmex.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/cppclass.m
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/functionSignatures.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/generate_pointset.m
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/gridKeyPress.m
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/gridfigure.m
+-rw-r--r--   0 runner    (1001) docker     (123)    91317 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/gridtool.m
+-rw-r--r--   0 runner    (1001) docker     (123)    84265 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/gridtool_old.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/plot_twopar.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/queryOpenCL.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-25 02:04:30.000000 clode-0.3.2/matlab/trajectoryfigure.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.601488 clode-0.3.2/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-25 02:04:30.000000 clode-0.3.2/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-25 02:04:30.000000 clode-0.3.2/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-25 02:04:30.000000 clode-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-25 02:04:30.000000 clode-0.3.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-25 02:04:30.000000 clode-0.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.605488 clode-0.3.2/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-25 02:04:30.000000 clode-0.3.2/samples/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-25 02:04:30.000000 clode-0.3.2/samples/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-25 02:04:30.000000 clode-0.3.2/samples/lacto_more_vars.cl
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-25 02:04:30.000000 clode-0.3.2/samples/lactotroph.cl
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-25 02:04:30.000000 clode-0.3.2/samples/lactotroph.ode
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-25 02:04:30.000000 clode-0.3.2/samples/lactotroph_noise.cl
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-25 02:04:30.000000 clode-0.3.2/samples/lactotroph_noise.ode
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-25 02:04:30.000000 clode-0.3.2/samples/listOpenCL.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-25 02:04:30.000000 clode-0.3.2/samples/plot_twopar.m
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-04-25 02:04:30.000000 clode-0.3.2/samples/run_twopar.m
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-25 02:04:30.000000 clode-0.3.2/samples/test.cl
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-25 02:04:30.000000 clode-0.3.2/samples/testCLODE.m
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-25 02:04:30.000000 clode-0.3.2/samples/testCLODEfeatures.m
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 02:04:30.000000 clode-0.3.2/samples/testCLODEmex.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-25 02:04:30.000000 clode-0.3.2/samples/testCLODEtrajectory.m
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-25 02:04:30.000000 clode-0.3.2/samples/testFeatures.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-25 02:04:30.000000 clode-0.3.2/samples/testFeatures_morevars.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-04-25 02:04:30.000000 clode-0.3.2/samples/testTrajectory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-25 02:04:30.000000 clode-0.3.2/samples/testTransient.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-04-25 02:04:30.000000 clode-0.3.2/samples/test_outputs_cpp.md
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-25 02:04:30.000000 clode-0.3.2/samples/windowsCompileListOpenCL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 02:06:26.609488 clode-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-04-25 02:04:30.000000 clode-0.3.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-25 02:04:30.000000 clode-0.3.2/shell.nix
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.605488 clode-0.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:04:30.000000 clode-0.3.2/test/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:04:30.000000 clode-0.3.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-25 02:04:30.000000 clode-0.3.2/test/ornl_thompson_a1.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-25 02:04:30.000000 clode-0.3.2/test/test.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-25 02:04:30.000000 clode-0.3.2/test/test_lactotroph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-25 02:04:30.000000 clode-0.3.2/test/test_lactotroph_more_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-25 02:04:30.000000 clode-0.3.2/test/test_lactotroph_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-25 02:04:30.000000 clode-0.3.2/test/test_ornl_thompson_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-04-25 02:04:30.000000 clode-0.3.2/test/test_pituitary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-25 02:04:30.000000 clode-0.3.2/test/test_vdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-25 02:04:30.000000 clode-0.3.2/test/test_vdp_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-25 02:04:30.000000 clode-0.3.2/test/text_xpp_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-25 02:04:30.000000 clode-0.3.2/test/van_der_pol_oscillator.cl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:06:26.605488 clode-0.3.2/test/xpp/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-25 02:04:30.000000 clode-0.3.2/test/xpp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-25 02:04:30.000000 clode-0.3.2/test/xpp/van_der_pol_oscillator.xpp
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-25 02:04:30.000000 clode-0.3.2/test/xpp/van_der_pol_oscillator_reference.cl
```

### Comparing `clode-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md` & `clode-0.3.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md` & `clode-0.3.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/.github/workflows/bazel_build_linux.yml` & `clode-0.3.2/.github/workflows/bazel_build_linux.yml`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/.github/workflows/bazel_build_windows.yml` & `clode-0.3.2/.github/workflows/bazel_build_windows.yml`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/.github/workflows/bazel_test_mac.yml` & `clode-0.3.2/.github/workflows/bazel_test_mac.yml`

 * *Files 2% similar despite different names*

```diff
@@ -39,8 +39,8 @@
           PYTHON=python3 make upload
 
       - name: Publish to PyPI
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
         run: |
-          make upload_prod
+          PYTHON=python3 make upload_prod
```

### Comparing `clode-0.3.1/.github/workflows/draft_pdf.yml` & `clode-0.3.2/.github/workflows/draft_pdf.yml`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/.gitignore` & `clode-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/LICENSE` & `clode-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/Makefile` & `clode-0.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/PKG-INFO` & `clode-0.3.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clode
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python package for solving ordinary differential equations on the GPU using OpenCL
 Author-email: Patrick Fletcher <patrick.allen.fletcher@gmail.com>
 Maintainer-email: Patrick Fletcher <patrick.allen.fletcher@gmail.com>, Wolf Byttner <wolf@byttner.org>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -22,20 +22,24 @@
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # clODE - an OpenCL based tool for solving ordinary differential equations (ODEs)
 
-clODE is a tool for solving ordinary differential equations (ODEs) using OpenCL.
-It lets users simulate 10,000s of ODEs simultaneously on a GPU, 
-and generates data three orders of magnitude faster than Matlab's ODE solvers
-or scipy's odeint.
-
-clODE is written in C++ and OpenCL, and has a Python interface.
-The right-hand-side (RHS) function is written in OpenCL,
-and is relatively simple in structure. The library is compiled
-using bazel and bazelisk, and it runs on Linux, Windows and MacOS.
+clODE is a tool for solving ordinary differential equations (ODEs) using OpenCL. It is tailored to numerically solving many instances of a given ODE system in parallel, each with different parameter sets and/or initial conditions.
+
+The ODE solver runs entirely on the OpenCL device, supporting independent solver state per simulation (e.g., adaptive timesteps). clODE can return the full trajectories, though this is somewhat memory intensive. Alternatively, clODE supports computing features of the ODE trajectory (e.g., oscillation period) on the fly without storing the trajectory itself, enabling much larger parameter sweeps to be run with significant speedup over serial computation.
+
+clODE is written in C++ and OpenCL, and can be used directly in C++ programs or via the provided Python interface. The library is compiled using bazel and bazelisk, and it runs on Linux, Windows and MacOS.
+
+## Installation
+
+See [installation](docs/install.md) for instructions on how to install CLODE.
+
+## Getting Started
+
+See [Getting Started](docs/getting_started.md) for an example of clODE usage.
 
 ## Source
 
 The source code is available on [GitHub](https://github.com/patrickfletcher/clODE).
```

### Comparing `clode-0.3.1/WORKSPACE` & `clode-0.3.2/WORKSPACE`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/bazel/clode_http_archive.bzl` & `clode-0.3.2/bazel/clode_http_archive.bzl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/bazel/external/python.BUILD` & `clode-0.3.2/bazel/external/python.BUILD`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/bazel/external_deps.bzl` & `clode-0.3.2/bazel/external_deps.bzl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/bazel/get_python_libs.py` & `clode-0.3.2/bazel/get_python_libs.py`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/bazel/python/BUILD.tpl` & `clode-0.3.2/bazel/python/BUILD.tpl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/bazel/python/python.bzl` & `clode-0.3.2/bazel/python/python.bzl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/bazel/python/variety.tpl` & `clode-0.3.2/bazel/python/variety.tpl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/bazel/remote_config/common.bzl` & `clode-0.3.2/bazel/remote_config/common.bzl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/bazel/repositories.bzl` & `clode-0.3.2/bazel/repositories.bzl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/bazel/repository_locations.bzl` & `clode-0.3.2/bazel/repository_locations.bzl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/bazel/repository_locations_utils.bzl` & `clode-0.3.2/bazel/repository_locations_utils.bzl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/bazelisk.py` & `clode-0.3.2/bazelisk.py`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/BUILD` & `clode-0.3.2/clode/cpp/BUILD`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/CLODE.cpp` & `clode-0.3.2/clode/cpp/CLODE.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
 			spdlog::error("CLODE::setX0:{}({})\n", er.what(), CLErrorString(er.err()).c_str());
 			throw er;
 		}
 		spdlog::debug("set X0\n");
 	}
 	else
 	{
-		spdlog::info("Invalid initial condition vector: Expected {}*{} elements, recieved {}}\n", nPts, nVar, newX0.size());
+		// spdlog::info("Invalid initial condition vector: Expected {}*{} elements, recieved {}}\n", nPts, nVar, newX0.size());
 		spdlog::info("...Initial conditions were not updated!\n");
 		//~ throw std::invalid_argument("Initial Condition vector has incorrect size.");
 	}
 }
 
 void CLODE::shiftX0()
 {
```

### Comparing `clode-0.3.1/clode/cpp/CLODE.hpp` & `clode-0.3.2/clode/cpp/CLODE.hpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/CLODEfeatures.cpp` & `clode-0.3.2/clode/cpp/CLODEfeatures.cpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/CLODEfeatures.hpp` & `clode-0.3.2/clode/cpp/CLODEfeatures.hpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/CLODEpython.cpp` & `clode-0.3.2/clode/cpp/CLODEpython.cpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/CLODEtrajectory.cpp` & `clode-0.3.2/clode/cpp/CLODEtrajectory.cpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/CLODEtrajectory.hpp` & `clode-0.3.2/clode/cpp/CLODEtrajectory.hpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/OpenCL/BUILD` & `clode-0.3.2/clode/cpp/OpenCL/BUILD`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/OpenCL/cl.hpp` & `clode-0.3.2/clode/cpp/OpenCL/cl.hpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/OpenCL/cl2.hpp` & `clode-0.3.2/clode/cpp/OpenCL/cl2.hpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/OpenCLResource.cpp` & `clode-0.3.2/clode/cpp/OpenCLResource.cpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/OpenCLResource.hpp` & `clode-0.3.2/clode/cpp/OpenCLResource.hpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/clODE_random.cl` & `clode-0.3.2/clode/cpp/clODE_random.cl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/clODE_utilities.cl` & `clode-0.3.2/clode/cpp/clODE_utilities.cl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/features.cl` & `clode-0.3.2/clode/cpp/features.cl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/initializeObserver.cl` & `clode-0.3.2/clode/cpp/initializeObserver.cl`

 * *Files 8% similar despite different names*

```diff
@@ -34,17 +34,19 @@
 		xi[j] = x0[j * nPts + i];
 
 	for (int j = 0; j < N_RNGSTATE; ++j)
 		rd.state[j] = RNGstate[j * nPts + i];
 
 	rd.randnUselast = 0;
 
-#ifdef STOCHASTIC_STEPPER
     for (int j = 0; j < N_WIENER; ++j)
+#ifdef STOCHASTIC_STEPPER
         wi[j] = randn(&rd) / sqrt(dt);
+#else
+        wi[j] = RCONST(0.0);
 #endif
 	getRHS(ti, xi, p, dxi, auxi, wi); //slope at initial point, needed for FSAL
 
 	ObserverData odata = OData[i]; //private copy of observer data
 
 	initializeObserverData(&ti, xi, dxi, auxi, &odata, opars);
```

### Comparing `clode-0.3.1/clode/cpp/logging/MatlabSink.hpp` & `clode-0.3.2/clode/cpp/logging/MatlabSink.hpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/logging/PythonSink.hpp` & `clode-0.3.2/clode/cpp/logging/PythonSink.hpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/observers/BUILD` & `clode-0.3.2/clode/cpp/observers/BUILD`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/observers/observer_basic.clh` & `clode-0.3.2/clode/cpp/observers/observer_basic.clh`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/observers/observer_basic_allVar.clh` & `clode-0.3.2/clode/cpp/observers/observer_basic_allVar.clh`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/observers/observer_local_maximum.clh` & `clode-0.3.2/clode/cpp/observers/observer_local_maximum.clh`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/observers/observer_neighborhood_1.clh` & `clode-0.3.2/clode/cpp/observers/observer_neighborhood_1.clh`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/observers/observer_neighborhood_2.clh` & `clode-0.3.2/clode/cpp/observers/observer_neighborhood_2.clh`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/observers/observer_template.clh` & `clode-0.3.2/clode/cpp/observers/observer_template.clh`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/observers/observer_threshold_1.clh` & `clode-0.3.2/clode/cpp/observers/observer_threshold_1.clh`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/observers/observer_threshold_2.clh` & `clode-0.3.2/clode/cpp/observers/observer_threshold_2.clh`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/observers.cl` & `clode-0.3.2/clode/cpp/observers.cl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/odedriver.cl` & `clode-0.3.2/clode/cpp/odedriver.cl`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,19 @@
         xi[j] = x0[j * nPts + i];
 
     for (int j = 0; j < N_RNGSTATE; ++j)
         rd.state[j] = RNGstate[j * nPts + i];
 
     rd.randnUselast = 0;
 
-#ifdef STOCHASTIC_STEPPER
     for (int j = 0; j < N_WIENER; ++j)
+#ifdef STOCHASTIC_STEPPER
         wi[j] = randn(&rd) / sqrt(dt);
+#else
+        wi[j] = RCONST(0.0);
 #endif
 	getRHS(ti, xi, p, dxi, auxi, wi); //slope at initial point, needed for FSAL steppers (bs23, dorpri5)
 
     //store the initial point --> could be set elsewhere using an "init" kernel?
     int storeix = 0;
     t[storeix + i] = tspan[0];
     for (int j = 0; j < N_VAR; ++j)
```

### Comparing `clode-0.3.1/clode/cpp/realtype.cl` & `clode-0.3.2/clode/cpp/realtype.cl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/steppers/BUILD` & `clode-0.3.2/clode/cpp/steppers/BUILD`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/steppers/adaptive_bs23.clh` & `clode-0.3.2/clode/cpp/steppers/adaptive_bs23.clh`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/steppers/adaptive_dp45.clh` & `clode-0.3.2/clode/cpp/steppers/adaptive_dp45.clh`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/steppers/adaptive_explicit_step.clh` & `clode-0.3.2/clode/cpp/steppers/adaptive_explicit_step.clh`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #define SAFETY_FACTOR RCONST(0.8)
 // #define EXPON RCONST(1.0)/LOCAL_ERROR_ORDER  //controls error per step -> local error only; err~tol
 #define EXPON RCONST(1.0)/(LOCAL_ERROR_ORDER+RCONST(1.0))  //controls error per unit step (err/dt~tol) -> global error proportional to tol (tolerance proportional) 
 
 //Wrapper to handle step-size adaptation.  note: wi should be zeros
 inline int stepper(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], 
 __constant struct SolverParams *sp, realtype *dt, __constant realtype *tspan, 
-realtype aux[], realtype wi[], rngData *rd)
+realtype aux[], realtype wi[], __private rngData *rd)
 {
     realtype tNew, normErr, relErr, err[N_VAR], newxi[N_VAR], newk1[N_VAR];
 
     realtype newDt = *dt;
     realtype threshold = sp->abstol / sp->reltol;
     realtype hmin = RCONST(16.0) * fabs(fabs(nextafter(*ti, RCONST(1.1)*tspan[1])) - *ti); //matches Matlab: hmin=16*eps(t)
```

### Comparing `clode-0.3.1/clode/cpp/steppers/adaptive_he12.clh` & `clode-0.3.2/clode/cpp/steppers/adaptive_he12.clh`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/steppers/adaptive_rkck.clh` & `clode-0.3.2/clode/cpp/steppers/adaptive_rkck.clh`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/steppers/fixed_explicit_Euler.clh` & `clode-0.3.2/clode/cpp/steppers/fixed_explicit_Euler.clh`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/steppers/fixed_explicit_RK4.clh` & `clode-0.3.2/clode/cpp/steppers/fixed_explicit_RK4.clh`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/steppers/fixed_explicit_Trapezoidal.clh` & `clode-0.3.2/clode/cpp/steppers/fixed_explicit_Trapezoidal.clh`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/steppers/fixed_explicit_step.clh` & `clode-0.3.2/clode/cpp/steppers/fixed_explicit_step.clh`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #include "realtype.cl"
 
 //TODO: seems like there's no need for this if we use naive time update, except to allow Wiener vars in any solver without cluttering the steppers
 
 //Wrapper to handle step-size adaptation.  note: wi should be zeros
 inline int stepper(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], 
 __constant struct SolverParams *sp, realtype *dt, __constant realtype *tspan, 
-realtype aux[], realtype wi[], rngData *rd)
+realtype aux[], realtype wi[], __private rngData *rd)
 {
     // xi and ti are updated inside do_step. 
     do_step(ti, xi, k1, pars, *dt, aux, wi);
 
     // naive time update - this is the one consistent with what's in each stepper...
     // *ti += *dt;
```

### Comparing `clode-0.3.1/clode/cpp/steppers.cl` & `clode-0.3.2/clode/cpp/steppers.cl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/trajectory.cl` & `clode-0.3.2/clode/cpp/trajectory.cl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/cpp/transient.cl` & `clode-0.3.2/clode/cpp/transient.cl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/python/BUILD` & `clode-0.3.2/clode/python/BUILD`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/python/features.py` & `clode-0.3.2/clode/python/features.py`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/python/observer.py` & `clode-0.3.2/clode/python/observer.py`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/python/trajectory.py` & `clode-0.3.2/clode/python/trajectory.py`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode/python/xpp_parser.py` & `clode-0.3.2/clode/python/xpp_parser.py`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/clode.egg-info/PKG-INFO` & `clode-0.3.2/clode.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clode
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python package for solving ordinary differential equations on the GPU using OpenCL
 Author-email: Patrick Fletcher <patrick.allen.fletcher@gmail.com>
 Maintainer-email: Patrick Fletcher <patrick.allen.fletcher@gmail.com>, Wolf Byttner <wolf@byttner.org>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -22,20 +22,24 @@
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # clODE - an OpenCL based tool for solving ordinary differential equations (ODEs)
 
-clODE is a tool for solving ordinary differential equations (ODEs) using OpenCL.
-It lets users simulate 10,000s of ODEs simultaneously on a GPU, 
-and generates data three orders of magnitude faster than Matlab's ODE solvers
-or scipy's odeint.
-
-clODE is written in C++ and OpenCL, and has a Python interface.
-The right-hand-side (RHS) function is written in OpenCL,
-and is relatively simple in structure. The library is compiled
-using bazel and bazelisk, and it runs on Linux, Windows and MacOS.
+clODE is a tool for solving ordinary differential equations (ODEs) using OpenCL. It is tailored to numerically solving many instances of a given ODE system in parallel, each with different parameter sets and/or initial conditions.
+
+The ODE solver runs entirely on the OpenCL device, supporting independent solver state per simulation (e.g., adaptive timesteps). clODE can return the full trajectories, though this is somewhat memory intensive. Alternatively, clODE supports computing features of the ODE trajectory (e.g., oscillation period) on the fly without storing the trajectory itself, enabling much larger parameter sweeps to be run with significant speedup over serial computation.
+
+clODE is written in C++ and OpenCL, and can be used directly in C++ programs or via the provided Python interface. The library is compiled using bazel and bazelisk, and it runs on Linux, Windows and MacOS.
+
+## Installation
+
+See [installation](docs/install.md) for instructions on how to install CLODE.
+
+## Getting Started
+
+See [Getting Started](docs/getting_started.md) for an example of clODE usage.
 
 ## Source
 
 The source code is available on [GitHub](https://github.com/patrickfletcher/clODE).
```

### Comparing `clode-0.3.1/clode.egg-info/SOURCES.txt` & `clode-0.3.2/clode.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -167,8 +167,9 @@
 test/test_ornl_thompson_a1.py
 test/test_pituitary.py
 test/test_vdp.py
 test/test_vdp_long.py
 test/text_xpp_converter.py
 test/van_der_pol_oscillator.cl
 test/xpp/.gitignore
-test/xpp/van_der_pol_oscillator.xpp
+test/xpp/van_der_pol_oscillator.xpp
+test/xpp/van_der_pol_oscillator_reference.cl
```

### Comparing `clode-0.3.1/docs/feature_extraction.md` & `clode-0.3.2/docs/feature_extraction.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,44 +8,44 @@
 
 Advanced observers can also capture local maxima, neighbourhoods,
 and thresholds.
 
 ## Observers
 
 CLODE's observers are highly configurable. You can choose the following:
+
 * basic - Captures one variable
 * basic_all_variables - Captures all variables
 * local_max - Captures local maxima
-* neighbourhood_1
 * neighbourhood_2
 * threshold_2 - Captures all values above a threshold
 
 ## Example
 
 The following example extracts features from the Van der Pol oscillator
 using the dormand_prince45 integrator.
 
-
 ### XPP
+
 ```xpp
 init x = 0.1 y = 0.1
 
 par mu = 0.1
 y' = mu * (1 - x*x) * y - x
 x' = y
 
 @ dt=0.05, total=5000, maxstor=20000000
 @ bounds=10000000, xp=t, yp=v
 @ xlo=0, xhi=5000, ylo=-75, yhi=0
 @ method=Euler
 
 ```
 
-
 ### Python
+
 ```python
 import numpy as np
 
 import clode
 
 
 def cuberoot(x):
@@ -76,8 +76,8 @@
     integrator.transient()
     integrator.features()
     observer_output = integrator.get_observer_results()
     
     return observer_output
 
 vdp_dormand_prince(100, "vdp_oscillator.xpp")
-```
+```
```

### Comparing `clode-0.3.1/docs/install.md` & `clode-0.3.2/docs/install.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,65 @@
 # Introduction
 
-# C++
+## C++
 
 To install the C++ library, you will need the following dependencies:
+
 * A C++ compiler (GCC, Clang, MSVC, etc.)
 * Bazel (4.0 or later recommended)
 * An OpenCL runtime (AMD APP SDK, Intel OpenCL SDK, NVIDIA CUDA, etc.)
 
 You can build the C++ libraries using Bazel:
 
-    bazel build //clode/cpp:cpp
+```
+bazel build //clode/cpp:cpp
+```
 
 There are three libraries that will be built:
+
 * libclode_features.a: The feature extraction library
 * libclode_trajectory.a: The trajectory extraction library
 * libopencl_resources.a: The OpenCL resources library (to find your OpenCL runtime)
 
-# Python
+## Python
 
 To install the Python library, you will need the following dependencies:
+
 * A C++ compiler (GCC, Clang, MSVC, etc.)
 * Python 3.8 or later
 * An OpenCL runtime (AMD APP SDK, Intel OpenCL SDK, NVIDIA CUDA, etc.)
 
 You can install the Python library using pip:
 
+```
     pip install clode
+```
 
 This will download Bazel to your machine (using Bazelisk)
 and build the C++ libraries. It will then install the Python library.
 
 ## Windows
 
-On Windows, Bazel will use MSVC to build the C++ libraries.
+On Windows, prior to installing via pip you will need the following dependencies in addition to those listed above:
+
+* The MSVC C++ compiler (e.g., Visual Studio Community installed to default path)
+* MSYS2 (add msys64/usr/bin to path)
+
+Bazel will use MSVC to build the C++ libraries.
 Further, Bazel will include the OpenCL SDK in the build.
 This means that you do not need to install the OpenCL SDK separately.
 
 Should you wish to change this behaviour, you can modify the
 library inside bazel/external/opencl_windows.BUILD and
 bazel/repository_locations.bzl.
 
-# License
+## License
+
 This project is licensed under the MIT License - see the [LICENSE](../LICENSE) file for details
 
-# Verifying the installation
+## Verifying the installation
 
 To verify that the installation was successful, you can run the following command:
 
-    python -c "import clode; print(clode.print_opencl())"
+```
+python -c "import clode; print(clode.print_opencl())"
+```
```

### Comparing `clode-0.3.1/docs/matlab.md` & `clode-0.3.2/docs/matlab.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,75 +1,78 @@
 # clODE Matlab interface
 
 clODE solves many instances of the same ODE system given different input paramter values and/or initial conditions.
 
-This document describes the Matlab MEX-file interface provided for running clODE from within Matlab. 
+This document describes the Matlab MEX-file interface provided for running clODE from within Matlab.
 
 ## Installation
 
-Download/clone this repository to a folder of your choice. Add the `/clODE/matlab` folder to your matlab path. 
+Download/clone this repository to a folder of your choice. Add the `/clODE/matlab` folder to your matlab path.
 
 To compile the mex files, first edit the appropriate path variables in `compileCLODEmex.m` to point to your OpenCL installation:
+
 ``` matlab
   opencl_include_dir = '/path/to/cl.hpp'; %all platforms
   opencl_lib_dir = '/path/to/libOpenCL.so'; %Linux
   opencl_lib_dir = '/path/to/OpenCL.lib'; %Windows
 ```
+
 Next, run the script. Requires a [C++ compiler compatible with Matlab MEX-file compilation](https://www.mathworks.com/support/requirements/supported-compilers.html).
 
-The specification of ODE systems can be done using XPPAUT style ODE files. To use this feature, please also [download XPPToolbox](https://github.com/patrickfletcher/xppToolbox) and [add it to your Matlab path](https://www.mathworks.com/help/matlab/ref/addpath.html). 
+The specification of ODE systems can be done using XPPAUT style ODE files. To use this feature, please also [download XPPToolbox](https://github.com/patrickfletcher/xppToolbox) and [add it to your Matlab path](https://www.mathworks.com/help/matlab/ref/addpath.html).
 
 ## Basics
 
 ODEs can be integrated with two main modes of result storage. Trajectories can be recorded in full (using the `clODEtrajectory` class), which may result in large memory requirements if the number of IVP instances gets large. Alternatively, features of the trajectories can be computed on the fly during integration without storing the full trajectories (using the `clODEfeatures` class).
 
 These classes can be used in scripts or via graphical interface elements, as described in the following sections. Some simple test examples are provided in the `/clODE/samples/` subdirectory.
 
 ## Setting up a solver
 
 clODE objects are created via the class constructors. At minimum, the constructors require one input, pointing to the ODE system definition. Additionally, the numerical precision, OpenCL device, ODE time stepping algorithm, and feature-detection method (for clODEfeatures only) can be specified. Examples:
+
 ``` matlab
 clo=clODE(odefile); %using an XPP ODE-file to specify the ODE, using default solver specification: precision='single', selectedDevice=1, stepper='dorpri5'.
 
 openclDevices=queryOpenCL(); %array of structs describing OpenCL devices available
 precision='double'; %'single' {default} or 'double' 
 selectedDevice=2; %1-based index into openclDevices.
 stepper='rk4'; %a valid time stepping algorithm name 
 clo=clODE(odefile,precision,selectedDevice,stepper); 
 
 clo=clODE(odestruct); %using a struct to specify the ODE system, e.g. output of ode2cl
 ```
+
 The returned `clo` object is used to run simulations. ODE system information is stored in the struct `clo.prob`.
 
 ### ODE system specification
 
 The easiest way to specify an ODE system is to use an ODE file as needed for XPPAUT. The `ode2cl` function from [XPPToolbox](https://github.com/patrickfletcher/xppToolbox) to parse XPPAUT files and automatically generate the OpenCL code required for execution on OpenCL devices. It also returns a struct containing detailed information about the ODE system for use in your programs that can be used to initialize a clODE solver.
 
 Handwritten OpenCL files are also supported. At minimum a struct containing the following information is used to specify the ODE system:
+
 ``` matlab
 problem.clRHSfilename='/path/to/RHSfile.cl'; %An OpenCL function that computes the system's vector field
 problem.nVar=integer; %number of state variables
 problem.nPar=integer; %number of parameters that may vary
 problem.nAux=integer; %number of auxiliary output quantities (user defined functions of state variables)
 problem.nWiener=integer; %number of Wiener random variables for stochastic simulations
 ```
+
 The `RHSfile.cl` file must implement a function with the following signature:
+
 ``` c
 void getRHS(realtype t, realtype x_[], realtype p_[], realtype dx_[], realtype aux_[], realtype w_[]);
 // realtype is float or double
 // Input arguments: x_[] - state variable array, p_[] - parameter array, w_[] - array of Wiener variable values provided by clODE if nWiener>0. 
 // Output arguments: dx_[] - slopes, aux_[] - values of auxiliary output quantities
 ```
 
 ## Setting up problem data
 
-
-
 ## clODEtrajectory
 
-
-
 ## clODEfeatures
 
-The following 
+The following
 
-###
+###
```

### Comparing `clode-0.3.1/docs/querying_opencl.md` & `clode-0.3.2/docs/querying_opencl.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Querying the machine OpenCL capabilities
+# Querying system OpenCL capabilities
 
 clODE can query the OpenCL capabilities of your machine. This is useful for debugging and for finding the best OpenCL device for your application.
 
 ## Example - Print OpenCL capabilities
 
 ```python
 import clode
 
 print(clode.print_opencl())
 ```
 
-## Output
+### Output
 
 ```
 [2023-04-05 17:19:48.614] [info] 
 Querying OpenCL platforms...
 [2023-04-05 17:19:48.733] [info] Number of platforms found: %u
 [2023-04-05 17:19:48.733] [info] 
 Platform 0. ------------------------------
@@ -39,19 +39,19 @@
 
 ## Example - Query OpenCL capabilities
 
 ```python
 import clode
 
 platforms = clode.query_opencl()
+print(platforms)
+print(clode.query_open_cl()[0].device_info)
 ```
 
-## Output
+### Output
 
 ```
->>> clode.query_open_cl()
 [<platform_info(name=Apple, vendor=Apple, version=OpenCL 1.2 (Nov  4 2022 20:34:31), device_count=1)>]
 
->>> clode.query_open_cl()[0].device_info
 [<device_info(name=Apple M1 Pro, vendor=Apple, version=OpenCL 1.2 , device_type=GPU, compute_units=16, max_clock=1000, max_work_group_size=256, device_memory_size=11453251584, max_memory_alloc_size=2147483648, extensions=cl_APPLE_SetMemObjectDestructor cl_APPLE_ContextLoggingFunctions cl_APPLE_clut cl_APPLE_query_kernel_names cl_APPLE_gl_sharing cl_khr_gl_event cl_khr_byte_addressable_store cl_khr_global_int32_base_atomics cl_khr_global_int32_extended_atomics cl_khr_local_int32_base_atomics cl_khr_local_int32_extended_atomics cl_khr_3d_image_writes cl_khr_image2d_from_buffer cl_khr_depth_images , double_support=0, device_available=1)>]
 
-```
+```
```

### Comparing `clode-0.3.1/docs/trajectory_simulation.md` & `clode-0.3.2/docs/trajectory_simulation.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 CLODE can simulate ODE trajectories using the CLODETrajectory class.
 
 ## Example
 
 The following example simulates the Van der Pol oscillator using the dormand_prince45 integrator.
 
-### XPP
+### OpenCL RHS function
 
-```xpp
+```c
 void getRHS(const realtype t,
             const realtype var[],
             const realtype par[],
             realtype derivatives[],
             realtype aux[],
             const realtype wiener[]) {
     realtype m = par[0];
@@ -26,25 +26,22 @@
     realtype dy1 = y2;
     realtype dy2 = (w - k * y2) / m;
 
     derivatives[0] = dy1;
     derivatives[1] = dy2;
     aux[0] = y1 - H;
 }
-
 ```
 
 ### Python
 
 ```python
 import clode
-
 import numpy as np
 
-
 def ornl_thompson_a1():
     num_simulations = 1
 
     m = 1 / 4
     w = 8
     k = 2
     H = 10
@@ -70,9 +67,8 @@
 
     integrator.initialize(x0, pars_v)
 
     integrator.trajectory()
 
     time_steps = integrator.get_time_steps()
     return integrator.get_trajectory()
-
-```
+```
```

### Comparing `clode-0.3.1/docs/xpp_files.md` & `clode-0.3.2/docs/xpp_files.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 clODE's Python library can read XPP files and convert them to OpenCL source files.
 
 To use this functionality, you must have the Python library installed.
 Simply send your .xpp file to the functions
 clode_features or clode_trajectory.
 
-
 ## Example
+
 You can also use the clode functions `read_ode_parameters`
 and `format_opencl_rhs`.
 
-
 ### Converting an XPP string to OpenCL
 
 ```python
 import clode
 
 with open("van_der_pol_oscillator.xpp", "r") as f:
     xpp_str = f.read()
@@ -33,21 +32,21 @@
 
 ```python
 import clode
 
 # The file will be named van_der_pol_oscillator.cl
 # and you can find it in the same directory as the .xpp file
 clode_cl_filename = clode.convert_xpp_file("van_der_pol_oscillator.xpp")
-``` 
-
+```
 
 ## Example
 
 For a fully-working example, look in `test/test_xpp_converter.py`.
 
 ## Limitations
 
 The XPP converter is not perfect. It is not guaranteed to work for all XPP files.
 Formatting will not be preserved.
 
 The following features are partially supported:
+
 * exponents
```

### Comparing `clode-0.3.1/matlab/Chart.m` & `clode-0.3.2/matlab/Chart.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/matlab/GridSimulation.m` & `clode-0.3.2/matlab/GridSimulation.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/matlab/InitialValueProblem.m` & `clode-0.3.2/matlab/InitialValueProblem.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/matlab/clODE.m` & `clode-0.3.2/matlab/clODE.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/matlab/clODEfeatures.m` & `clode-0.3.2/matlab/clODEfeatures.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/matlab/clODEfeaturesmex.cpp` & `clode-0.3.2/matlab/clODEfeaturesmex.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         //opencl device selection: assume the matlab caller selects by plaformID and deviceID, as returned by queryOpenCL 
         unsigned int platformID = (unsigned int)mxGetScalar(prhs[4]); 
         unsigned int deviceID = (unsigned int)mxGetScalar(prhs[5]);
         std::string observer = mxArrayToString(prhs[6]);
 	
 		// OpenCLResource opencl(platformID, deviceID);
 		// insResult = instanceTab.insert(indPtrPair_type(newHandle, std::make_shared<class_type>(newProblem,stepper,observer,clSinglePrecision, opencl)));
-		insResult = instanceTab.insert(indPtrPair_type(newHandle, std::make_shared<class_type>(newProblem,stepper,observer,clSinglePrecision, platformID, deviceID)));
+		insResult = instanceTab.insert(indPtrPair_type(newHandle, std::make_shared<class_type>(newProblem,stepper,observer,clSinglePrecision, platformID, deviceID, CLODE_ROOT)));
 
         if (!insResult.second) // sanity check
             mexPrintf("Oh, bad news.  Tried to add an existing handle."); // shouldn't ever happen
         else
             mexLock(); // add to the lock count
 
 		// return the handle
```

### Comparing `clode-0.3.1/matlab/clODEmex.cpp` & `clode-0.3.2/matlab/clODEmex.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 		// OpenCLResource opencl(devicetype,vendor);
 
         //opencl device selection: assume the matlab caller selects by plaformID and deviceID, as returned by queryOpenCL 
         unsigned int platformID = (unsigned int)mxGetScalar(prhs[4]); 
         unsigned int deviceID = (unsigned int)mxGetScalar(prhs[5]);
 		// OpenCLResource opencl(platformID, deviceID);
 		// insResult = instanceTab.insert(indPtrPair_type(newHandle, std::make_shared<class_type>(newProblem,stepper,clSinglePrecision, opencl)));
-		insResult = instanceTab.insert(indPtrPair_type(newHandle, std::make_shared<class_type>(newProblem,stepper,clSinglePrecision, platformID, deviceID)));
+		insResult = instanceTab.insert(indPtrPair_type(newHandle, std::make_shared<class_type>(newProblem,stepper,clSinglePrecision, platformID, deviceID, CLODE_ROOT)));
 
         if (!insResult.second) // sanity check
             mexPrintf("Oh, bad news.  Tried to add an existing handle."); // shouldn't ever happen
         else
             mexLock(); // add to the lock count
 
 		// return the handle
```

### Comparing `clode-0.3.1/matlab/clODEmexHelpers.hpp` & `clode-0.3.2/matlab/clODEmexHelpers.hpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/matlab/clODEtrajectory.m` & `clode-0.3.2/matlab/clODEtrajectory.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/matlab/clODEtrajectorymex.cpp` & `clode-0.3.2/matlab/clODEtrajectorymex.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 
         //opencl device selection: assume the matlab caller selects by plaformID and deviceID, as returned by queryOpenCL 
         unsigned int platformID = (unsigned int)mxGetScalar(prhs[4]); 
         unsigned int deviceID = (unsigned int)mxGetScalar(prhs[5]);
 
 		// OpenCLResource opencl(platformID, deviceID);
 		// insResult = instanceTab.insert(indPtrPair_type(newHandle, std::make_shared<class_type>(newProblem,stepper,clSinglePrecision, opencl)));
-		insResult = instanceTab.insert(indPtrPair_type(newHandle, std::make_shared<class_type>(newProblem,stepper,clSinglePrecision, platformID, deviceID)));
+		insResult = instanceTab.insert(indPtrPair_type(newHandle, std::make_shared<class_type>(newProblem,stepper,clSinglePrecision, platformID, deviceID, CLODE_ROOT)));
 
         if (!insResult.second) // sanity check
             mexPrintf("Oh, bad news.  Tried to add an existing handle."); // shouldn't ever happen
         else
             mexLock(); // add to the lock count
 
 		// return the handle
```

### Comparing `clode-0.3.1/matlab/clickTrajectory.m` & `clode-0.3.2/matlab/clickTrajectory.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/matlab/compileCLODEmex.m` & `clode-0.3.2/matlab/compileCLODEmex.m`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 % Script to compile clODE mex interface, so it can be used from Matlab.
 % Make sure to set the correct paths to files in the Configuration block!
 close all
 clear
 
 %TODO: auto detect paths for some common setups? e.g. CUDA
 
+thisdir = pwd;
+
 % %%%%%%%%%%%%%%%% CONFIGURATION %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 
 if ismac % Code to run on Mac plaform
     opencl_include_dir = pwd; %cl.hpp for OpenCL C++ bindings
     opencl_lib_dir = ''; %leave empty; taken care of by the -framework option
     libopencl='';
     compflags='COMPFLAGS="$COMPFLAGS -std=c++11 -framework OpenCL"';
@@ -34,52 +36,54 @@
     ldflags='';
     opencl_lib_dir=['-L',opencl_lib_dir];
     
 else
     disp('Cannot recognize platform')
 end
 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
-
-cd ../src/
+cd ../clode/cpp
 clode_path=[pwd filesep]; 
-cd ../matlab/
 clode_path=strrep(clode_path,'\','/'); 
 
+spdlog_path = 'D:/GitHub/spdlog/include';
+
+cd(thisdir)
+
 debugchar='';
 % debugchar='-g';
 
 verbosechar='';
 % verbosechar='-v';
 
 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 % Compile commands:
 
 %% queryOpenCL
 
 mex('queryOpenCL.cpp',[clode_path,'OpenCLResource.cpp'],...
     debugchar,verbosechar,compflags,...
-    ['-I' clode_path], ['-I' opencl_include_dir],...
+    ['-I' spdlog_path], ['-I' clode_path], ['-I' opencl_include_dir],...
     ldflags, opencl_lib_dir, libopencl );
 
 
 %% CLODE
 mex('clODEmex.cpp',[clode_path,'OpenCLResource.cpp'],[clode_path,'CLODE.cpp'],...
     debugchar,verbosechar,compflags,...
     ['-DCLODE_ROOT=\"' clode_path '\"'],...
-    ['-I' clode_path], ['-I' opencl_include_dir],...
+    ['-I' spdlog_path], ['-I' clode_path], ['-I' opencl_include_dir],...
     ldflags, opencl_lib_dir, libopencl );
 
 %% CLODEfeatures
 mex('clODEfeaturesmex.cpp',[clode_path,'OpenCLResource.cpp'],[clode_path,'CLODE.cpp'],...
     [clode_path,'CLODEfeatures.cpp'],...
     debugchar,verbosechar,compflags,...
     ['-DCLODE_ROOT=\"' clode_path '\"'],...
-    ['-I' clode_path], ['-I' opencl_include_dir],...
+    ['-I' spdlog_path], ['-I' clode_path], ['-I' opencl_include_dir],...
     ldflags, opencl_lib_dir, libopencl );
 
 %% CLODEtrajectory
 mex('clODEtrajectorymex.cpp',[clode_path,'OpenCLResource.cpp'],[clode_path,'CLODE.cpp'],...
     [clode_path,'CLODEtrajectory.cpp'],...
     debugchar,verbosechar,compflags,...
     ['-DCLODE_ROOT=\"' clode_path '\"'],...
-    ['-I' clode_path], ['-I' opencl_include_dir],...
+    ['-I' spdlog_path], ['-I' clode_path], ['-I' opencl_include_dir],...
     ldflags, opencl_lib_dir, libopencl );
```

### Comparing `clode-0.3.1/matlab/cppclass.m` & `clode-0.3.2/matlab/cppclass.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/matlab/generate_pointset.m` & `clode-0.3.2/matlab/generate_pointset.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/matlab/gridKeyPress.m` & `clode-0.3.2/matlab/gridKeyPress.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/matlab/gridfigure.m` & `clode-0.3.2/matlab/gridfigure.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/matlab/gridtool.m` & `clode-0.3.2/matlab/gridtool.m`

 * *Files 0% similar despite different names*

```diff
@@ -1223,21 +1223,26 @@
                 case 'go'
                     app.clo_g.shiftX0();
                     app.clo_g.features(1);
                     app.clo_g.getF();
                     
 %                 case 'shift'
                 case 'point'
-                    newX0=repmat(app.gridvars.val(app.gridvars.type=="ic")',app.nPts,1);
-                    app.clo_g.setX0(newX0);
+                    if app.gridtab{'x','type'}=="par" && app.gridtab{'y','type'}=="par"
+                        newX0=repmat(app.gridvars.val(app.gridvars.type=="ic")',app.nPts,1);
+                        app.clo_g.setX0(newX0);
+                    end
                     app.clo_g.transient();
 
                 case 'pointgo'
-                    newX0=repmat(app.gridvars.val(app.gridvars.type=="ic")',app.nPts,1);
-                    app.clo_g.setX0(newX0);
+                    if app.gridtab{'x','type'}=="par" && app.gridtab{'y','type'}=="par"
+                        newX0=repmat(app.gridvars.val(app.gridvars.type=="ic")',app.nPts,1);
+                        app.clo_g.setX0(newX0);
+                    end
+%                     app.clo_g.shiftX0();
                     app.clo_g.transient();
                     app.clo_g.shiftX0();
                     app.clo_g.features(1);
                     app.clo_g.getF();
                     
                 case 'random'
                     x0lb=app.gridvars.lb(app.gridvars.type=="ic")';
```

### Comparing `clode-0.3.1/matlab/gridtool_old.m` & `clode-0.3.2/matlab/gridtool_old.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/matlab/plot_twopar.m` & `clode-0.3.2/matlab/plot_twopar.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/matlab/queryOpenCL.cpp` & `clode-0.3.2/matlab/queryOpenCL.cpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/paper/paper.bib` & `clode-0.3.2/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/paper/paper.md` & `clode-0.3.2/paper/paper.md`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/pyproject.toml` & `clode-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/BUILD` & `clode-0.3.2/samples/BUILD`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/Makefile` & `clode-0.3.2/samples/Makefile`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/lacto_more_vars.cl` & `clode-0.3.2/samples/lacto_more_vars.cl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/lactotroph.cl` & `clode-0.3.2/samples/lactotroph.cl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/lactotroph.ode` & `clode-0.3.2/samples/lactotroph.ode`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/lactotroph_noise.cl` & `clode-0.3.2/samples/lactotroph_noise.cl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/lactotroph_noise.ode` & `clode-0.3.2/samples/lactotroph_noise.ode`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/plot_twopar.m` & `clode-0.3.2/samples/plot_twopar.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/run_twopar.m` & `clode-0.3.2/samples/run_twopar.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/test.cl` & `clode-0.3.2/samples/test.cl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/testCLODE.m` & `clode-0.3.2/samples/testCLODE.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/testCLODEfeatures.m` & `clode-0.3.2/samples/testCLODEfeatures.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/testCLODEmex.m` & `clode-0.3.2/samples/testCLODEmex.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/testCLODEtrajectory.m` & `clode-0.3.2/samples/testCLODEtrajectory.m`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/testFeatures.cpp` & `clode-0.3.2/samples/testFeatures.cpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/testFeatures_morevars.cpp` & `clode-0.3.2/samples/testFeatures_morevars.cpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/testTrajectory.cpp` & `clode-0.3.2/samples/testTrajectory.cpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/testTransient.cpp` & `clode-0.3.2/samples/testTransient.cpp`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/samples/test_outputs_cpp.md` & `clode-0.3.2/samples/test_outputs_cpp.md`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/setup.py` & `clode-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/test/ornl_thompson_a1.cl` & `clode-0.3.2/test/ornl_thompson_a1.cl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/test/test.cl` & `clode-0.3.2/test/test.cl`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/test/test_lactotroph.py` & `clode-0.3.2/test/test_lactotroph.py`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/test/test_lactotroph_more_vars.py` & `clode-0.3.2/test/test_lactotroph_more_vars.py`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/test/test_lactotroph_trajectory.py` & `clode-0.3.2/test/test_lactotroph_trajectory.py`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/test/test_ornl_thompson_a1.py` & `clode-0.3.2/test/test_ornl_thompson_a1.py`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/test/test_pituitary.py` & `clode-0.3.2/test/test_pituitary.py`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/test/test_vdp.py` & `clode-0.3.2/test/test_vdp.py`

 * *Files identical despite different names*

### Comparing `clode-0.3.1/test/text_xpp_converter.py` & `clode-0.3.2/test/text_xpp_converter.py`

 * *Files identical despite different names*

