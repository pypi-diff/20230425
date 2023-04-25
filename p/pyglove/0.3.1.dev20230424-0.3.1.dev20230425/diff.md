# Comparing `tmp/pyglove-0.3.1.dev20230424.tar.gz` & `tmp/pyglove-0.3.1.dev20230425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.3.1.dev20230424.tar", last modified: Mon Apr 24 08:06:52 2023, max compression
+gzip compressed data, was "pyglove-0.3.1.dev20230425.tar", last modified: Tue Apr 25 08:06:47 2023, max compression
```

## Comparing `pyglove-0.3.1.dev20230424.tar` & `pyglove-0.3.1.dev20230425.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.574168 pyglove-0.3.1.dev20230424/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-24 08:06:52.574168 pyglove-0.3.1.dev20230424/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-24 08:06:50.000000 pyglove-0.3.1.dev20230424/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.558168 pyglove-0.3.1.dev20230424/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.558168 pyglove-0.3.1.dev20230424/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.558168 pyglove-0.3.1.dev20230424/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.562168 pyglove-0.3.1.dev20230424/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64411 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.562168 pyglove-0.3.1.dev20230424/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.562168 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/docstr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/docstr_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.566168 pyglove-0.3.1.dev20230424/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.566168 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69715 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21002 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    32338 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    57913 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    25404 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    27851 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27187 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    51901 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27908 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    72331 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.570168 pyglove-0.3.1.dev20230424/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13822 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.570168 pyglove-0.3.1.dev20230424/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45005 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    23659 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    77073 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)    93868 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.570168 pyglove-0.3.1.dev20230424/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.570168 pyglove-0.3.1.dev20230424/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.574168 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50096 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.574168 pyglove-0.3.1.dev20230424/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.574168 pyglove-0.3.1.dev20230424/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/ext/scalars/step_wise_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/pyglove/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:06:52.558168 pyglove-0.3.1.dev20230424/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-24 08:06:52.000000 pyglove-0.3.1.dev20230424/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-04-24 08:06:52.000000 pyglove-0.3.1.dev20230424/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:06:52.000000 pyglove-0.3.1.dev20230424/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 08:06:52.000000 pyglove-0.3.1.dev20230424/pyglove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 08:06:52.000000 pyglove-0.3.1.dev20230424/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 08:06:52.574168 pyglove-0.3.1.dev20230424/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-24 08:06:41.000000 pyglove-0.3.1.dev20230424/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.308506 pyglove-0.3.1.dev20230425/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-25 08:06:47.308506 pyglove-0.3.1.dev20230425/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-25 08:06:45.000000 pyglove-0.3.1.dev20230425/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.280504 pyglove-0.3.1.dev20230425/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.284505 pyglove-0.3.1.dev20230425/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.284505 pyglove-0.3.1.dev20230425/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.288505 pyglove-0.3.1.dev20230425/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64411 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.296506 pyglove-0.3.1.dev20230425/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.296506 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.296506 pyglove-0.3.1.dev20230425/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.300506 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69715 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21002 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32338 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57913 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25404 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27851 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27187 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51901 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27908 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72331 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.300506 pyglove-0.3.1.dev20230425/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13822 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.304506 pyglove-0.3.1.dev20230425/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45005 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23659 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77129 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93868 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.304506 pyglove-0.3.1.dev20230425/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.304506 pyglove-0.3.1.dev20230425/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.304506 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50096 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.304506 pyglove-0.3.1.dev20230425/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.304506 pyglove-0.3.1.dev20230425/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/ext/scalars/step_wise_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/pyglove/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:47.284505 pyglove-0.3.1.dev20230425/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-25 08:06:47.000000 pyglove-0.3.1.dev20230425/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-04-25 08:06:47.000000 pyglove-0.3.1.dev20230425/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:06:47.000000 pyglove-0.3.1.dev20230425/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 08:06:47.000000 pyglove-0.3.1.dev20230425/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 08:06:47.000000 pyglove-0.3.1.dev20230425/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:06:47.308506 pyglove-0.3.1.dev20230425/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-25 08:06:30.000000 pyglove-0.3.1.dev20230425/setup.py
```

### Comparing `pyglove-0.3.1.dev20230424/LICENSE` & `pyglove-0.3.1.dev20230425/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/PKG-INFO` & `pyglove-0.3.1.dev20230425/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230424
+Version: 0.3.1.dev20230425
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230424/README.md` & `pyglove-0.3.1.dev20230425/README.md`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/__init__.py` & `pyglove-0.3.1.dev20230425/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/__init__.py` & `pyglove-0.3.1.dev20230425/pyglove/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/detouring/__init__.py` & `pyglove-0.3.1.dev20230425/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/detouring/class_detour.py` & `pyglove-0.3.1.dev20230425/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/__init__.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/base.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/base_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/categorical.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/categorical_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/custom.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/custom_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/deduping.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/deduping_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/dna_generator.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/numerical.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/numerical_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/random.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/random_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/space.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/space_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/sweeping.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/geno/sweeping_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/__init__.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/base.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/categorical.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/categorical_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/custom.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/custom_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/derived.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/derived_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/evolvable.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/iter.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/iter_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/numerical.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/numerical_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/object_template.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/hyper/object_template_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/logging.py` & `pyglove-0.3.1.dev20230425/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/logging_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/__init__.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/codegen.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/common_traits.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/common_traits.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/common_traits_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/docstr_utils.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/docstr_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/docstr_utils_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/docstr_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/formatting.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/missing.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/missing_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/thread_local.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/value_location.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/value_location.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/patching/__init__.py` & `pyglove-0.3.1.dev20230425/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/patching/object_factory.py` & `pyglove-0.3.1.dev20230425/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/patching/object_factory_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/patching/pattern_based.py` & `pyglove-0.3.1.dev20230425/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/patching/rule_based.py` & `pyglove-0.3.1.dev20230425/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/patching/rule_based_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/__init__.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/base.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/base_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/boilerplate.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/class_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/dict.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/dict.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/dict_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/dict_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/diff.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/diff.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/diff_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/diff_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/flags.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/flags_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/functor.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/functor.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/functor_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/functor_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/list.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/list.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/list_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/list_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/object.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/object.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/object_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/object_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/origin.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/origin.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/origin_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/origin_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/schema_utils_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/symbolize.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/tuning/__init__.py` & `pyglove-0.3.1.dev20230425/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/tuning/backend.py` & `pyglove-0.3.1.dev20230425/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/tuning/backend_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/tuning/early_stopping.py` & `pyglove-0.3.1.dev20230425/pyglove/core/tuning/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/tuning/local_backend.py` & `pyglove-0.3.1.dev20230425/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/tuning/protocols.py` & `pyglove-0.3.1.dev20230425/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/tuning/protocols_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/tuning/sample.py` & `pyglove-0.3.1.dev20230425/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/tuning/sample_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/__init__.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/callable_ext.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/callable_ext_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/callable_signature.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/callable_signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,25 +202,31 @@
         kwonly_args.append(arg_spec)
       elif param.kind == inspect.Parameter.VAR_POSITIONAL:
         varargs = arg_spec
       else:
         assert param.kind == inspect.Parameter.VAR_KEYWORD, param.kind
         varkw = arg_spec
 
+    return_value = None
+    if sig.return_annotation is not inspect.Parameter.empty:
+      return_value = class_schema.ValueSpec.from_annotation(
+          sig.return_annotation)
+
     if inspect.ismethod(func):
       callable_type = CallableType.METHOD
     else:
       callable_type = CallableType.FUNCTION
 
     return Signature(
         callable_type=callable_type,
         name=func.__name__,
         module_name=getattr(func, '__module__', 'wrapper'),
         qualname=func.__qualname__,
-        args=args, kwonlyargs=kwonly_args, varargs=varargs, varkw=varkw)
+        args=args, kwonlyargs=kwonly_args, varargs=varargs, varkw=varkw,
+        return_value=return_value)
 
   def make_function(
       self,
       body: List[str],
       exec_globals: Optional[Dict[str, Any]] = None,
       exec_locals: Optional[Dict[str, Any]] = None):
     """Makes a function with current signature."""
@@ -268,15 +274,16 @@
     # Generate function.
     fn = object_utils.make_function(
         self.name,
         args=args,
         body=body,
         exec_globals=exec_globals,
         exec_locals=exec_locals,
-        return_type=self.return_value or object_utils.MISSING_VALUE)
+        return_type=getattr(
+            self.return_value, 'annotation', object_utils.MISSING_VALUE))
     fn.__module__ = self.module_name
     fn.__name__ = self.name
     fn.__qualname__ = self.qualname
     return fn
 
 
 def get_signature(func: Callable) -> Signature:  # pylint:disable=g-bare-generic
```

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/callable_signature_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,30 +191,30 @@
     self.assertEqual(
         signature.varkw,
         callable_signature.Argument('kwargs', vs.Any()))
 
   def test_make_function(self):
     """Tests `Signature.make_function`."""
 
-    def func1(x, y=1):
+    def func1(x, y=1) -> int:
       del x, y
 
     def func2(x=1, *, y):
       del x, y
 
     def func3(x=1, *y):    # pylint: disable=keyword-arg-before-vararg
       del x, y
 
     def func4(*y):
       del y
 
     def func5(*, x=1, y):
       del x, y
 
-    def func6(x=1, *, y, **z):
+    def func6(x=1, *, y, **z) -> str:
       del x, y, z
 
     for func in [func1, func2, func3, func4, func5, func6]:
       new_func = callable_signature.get_signature(func).make_function(['pass'])
       old_signature = inspect.signature(func)
       new_signature = inspect.signature(new_func)
       self.assertEqual(old_signature, new_signature)
```

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/class_schema.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/class_schema.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/class_schema_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/class_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/class_schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/class_schema_utils_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/class_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/custom_typing.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/key_specs.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/key_specs_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/pytype_support.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/type_conversion.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/typed_missing.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/value_specs.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/value_specs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1624,16 +1624,17 @@
       else:
         raise TypeError(
             object_utils.message_on_path(
                 f'Keyword argument {arg_name!r} does not exist in {value!r}.',
                 path))
 
     # Check return value
-    if (self._return_value and signature.return_value and
-        not self._return_value.is_compatible(signature.return_value)):
+    if (self._return_value and signature.return_value
+        and not isinstance(signature.return_value, Any)
+        and not self._return_value.is_compatible(signature.return_value)):
       raise TypeError(
           object_utils.message_on_path(
               f'Value spec for return value is not compatible. '
               f'Expected: {self._return_value!r}, '
               f'Actual: {signature.return_value!r} ({value!r}).',
               path))
```

### Comparing `pyglove-0.3.1.dev20230424/pyglove/core/typing/value_specs_test.py` & `pyglove-0.3.1.dev20230425/pyglove/core/typing/value_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/__init__.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/early_stopping/base.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/__init__.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/base.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/base_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/mutators.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/neat.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/neat_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/nsga2.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/recombinators.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/selectors.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/where.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/evolution/where_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/mutfun/__init__.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/mutfun/base.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/mutfun/base_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/scalars/__init__.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/scalars/base.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/scalars/base_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/scalars/maths.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/scalars/maths_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/scalars/randoms.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/scalars/randoms_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/scalars/randoms_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/scalars/step_wise.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.3.1.dev20230425/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove/generators.py` & `pyglove-0.3.1.dev20230425/pyglove/generators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/pyglove.egg-info/PKG-INFO` & `pyglove-0.3.1.dev20230425/pyglove.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230424
+Version: 0.3.1.dev20230425
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230424/pyglove.egg-info/SOURCES.txt` & `pyglove-0.3.1.dev20230425/pyglove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230424/setup.py` & `pyglove-0.3.1.dev20230425/setup.py`

 * *Files identical despite different names*

