# Comparing `tmp/pash-annotations-0.2.tar.gz` & `tmp/pash-annotations-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pash-annotations-0.2.tar", last modified: Mon Oct  3 19:32:25 2022, max compression
+gzip compressed data, was "pash-annotations-0.2.1.tar", last modified: Mon Apr 24 22:15:34 2023, max compression
```

## Comparing `pash-annotations-0.2.tar` & `pash-annotations-0.2.1.tar`

### file list

```diff
@@ -1,125 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:25.702200 pash-annotations-0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-10-03 19:32:16.000000 pash-annotations-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-10-03 19:32:16.000000 pash-annotations-0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-10-03 19:32:25.702200 pash-annotations-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2930 2022-10-03 19:32:16.000000 pash-annotations-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:25.690199 pash-annotations-0.2/pash_annotations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2913 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:25.690199 pash-annotations-0.2/pash_annotations/annotation_generation/
--rw-r--r--   0 runner    (1001) docker     (121)     4305 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/AnnotationGeneration.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:25.694200 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/Generator_Interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorAltBigramAuxReduce.py
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorAltBigramsAux.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorBigramsAux.py
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCat.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCol.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorComm.py
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCustomSort.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCustomTr.py
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCut.py
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorDiff.py
--rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorGrep.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorHead.py
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorMkfifo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2142 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorMv.py
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorRm.py
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSed.py
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSeq.py
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSetDiff.py
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSort.py
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTail.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTee.py
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTestOne.py
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTestTwo.py
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorUniq.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorXargs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7753 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGenerator_Interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorAltBigramsAux.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorBigramsAux.py
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCol.py
--rw-r--r--   0 runner    (1001) docker     (121)     2086 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCustomSort.py
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCustomTr.py
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCut.py
--rw-r--r--   0 runner    (1001) docker     (121)     5800 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorGrep.py
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSed.py
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSetDiff.py
--rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSort.py
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTestOne.py
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTestTwo.py
--rw-r--r--   0 runner    (1001) docker     (121)     3223 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2291 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorUniq.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorXargs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4647 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGenerator_Interface.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:25.694200 pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/CommandProperties.py
--rw-r--r--   0 runner    (1001) docker     (121)    11088 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/InputOutputInfo.py
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/Inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/ParallelizabilityInfo.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:25.698200 pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/
--rw-r--r--   0 runner    (1001) docker     (121)     2963 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/Aggregator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/AggregatorKind.py
--rw-r--r--   0 runner    (1001) docker     (121)    18849 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/AggregatorSpec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/Mapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     7602 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/MapperSpec.py
--rw-r--r--   0 runner    (1001) docker     (121)     7801 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/Parallelizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/Splitter.py
--rw-r--r--   0 runner    (1001) docker     (121)     6880 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/TransformerFlagOptionList.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:25.698200 pash-annotations-0.2/pash_annotations/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2846 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/config/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:25.698200 pash-annotations-0.2/pash_annotations/datatypes/
--rw-r--r--   0 runner    (1001) docker     (121)     2943 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/datatypes/AccessKind.py
--rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/datatypes/BasicDatatypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5618 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/datatypes/BasicDatatypesWithIO.py
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/datatypes/BasicDatatypesWithIOVar.py
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/datatypes/CommandInvocationInitial.py
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/datatypes/CommandInvocationPrefix.py
--rw-r--r--   0 runner    (1001) docker     (121)    12792 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/datatypes/CommandInvocationWithIO.py
--rw-r--r--   0 runner    (1001) docker     (121)    10730 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/datatypes/CommandInvocationWithIOVars.py
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/datatypes/Operand.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:25.698200 pash-annotations-0.2/pash_annotations/parser/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:25.690199 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:25.698200 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/_default_data_for_commands.json
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/cat.json
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/col.json
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/comm.json
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/custom_sort.json
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/custom_tr.json
--rw-r--r--   0 runner    (1001) docker     (121)      808 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/cut.json
--rw-r--r--   0 runner    (1001) docker     (121)     3405 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/diff.json
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/export.json
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/grep.json
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/head.json
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/mkfifo.json
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/mv.json
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/rm.json
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/sed.json
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/seq.json
--rw-r--r--   0 runner    (1001) docker     (121)     2225 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/sort.json
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/tail.json
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/tee.json
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/tr.json
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/uniq.json
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/xargs.json
--rw-r--r--   0 runner    (1001) docker     (121)     5999 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/parser/util_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/util_flag_option.py
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-10-03 19:32:16.000000 pash-annotations-0.2/pash_annotations/util_standard.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 19:32:25.690199 pash-annotations-0.2/pash_annotations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-10-03 19:32:25.000000 pash-annotations-0.2/pash_annotations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7991 2022-10-03 19:32:25.000000 pash-annotations-0.2/pash_annotations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 19:32:25.000000 pash-annotations-0.2/pash_annotations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-03 19:32:25.000000 pash-annotations-0.2/pash_annotations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-03 19:32:25.702200 pash-annotations-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-10-03 19:32:16.000000 pash-annotations-0.2/setup.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.418661 pash-annotations-0.2.1/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1073 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/LICENSE
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       44 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/MANIFEST.in
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3592 2023-04-24 22:15:34.418661 pash-annotations-0.2.1/PKG-INFO
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3445 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/README.md
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.406660 pash-annotations-0.2.1/pash_annotations/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/__init__.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2928 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_cli.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.406660 pash-annotations-0.2.1/pash_annotations/annotation_generation/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     4344 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/AnnotationGeneration.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/__init__.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.410661 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1650 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/Generator_Interface.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      358 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorAltBigramAuxReduce.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      345 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorAltBigramsAux.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      887 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorAwk.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      341 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorBigramsAux.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      724 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCat.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      335 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCol.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      765 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorComm.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      645 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCustomSort.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      466 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCustomTr.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      685 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCut.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      343 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorDiff.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2565 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorGrep.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      565 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorHead.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      301 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorMkfifo.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2142 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorMv.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      296 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorRm.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      607 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSed.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      352 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSeq.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      469 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSetDiff.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      700 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSort.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      696 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTail.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      429 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTee.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      339 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTestOne.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      339 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTestTwo.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      688 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTr.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1196 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorUniq.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      684 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorWc.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      507 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorXargs.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     7753 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGenerator_Interface.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1160 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorAltBigramsAux.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1160 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorBigramsAux.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      388 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCol.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2086 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCustomSort.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      391 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCustomTr.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      653 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCut.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     5800 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorGrep.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      986 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSed.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      462 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSetDiff.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2081 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSort.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1169 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTestOne.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1171 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTestTwo.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3223 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTr.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2291 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorUniq.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      456 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorXargs.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     4647 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGenerator_Interface.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/__init__.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.410661 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      773 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/CommandProperties.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)    11088 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/InputOutputInfo.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      735 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/Inputs.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1921 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/ParallelizabilityInfo.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/__init__.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.410661 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2963 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/Aggregator.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1420 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/AggregatorKind.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)    18849 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/AggregatorSpec.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2119 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/Mapper.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     7602 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/MapperSpec.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     7801 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/Parallelizer.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1187 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/Splitter.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     6880 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/TransformerFlagOptionList.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/__init__.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.414661 pash-annotations-0.2.1/pash_annotations/config/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/config/__init__.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2846 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/config/definitions.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.414661 pash-annotations-0.2.1/pash_annotations/datatypes/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2943 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/AccessKind.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     4832 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/BasicDatatypes.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     5618 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/BasicDatatypesWithIO.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      568 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/BasicDatatypesWithIOVar.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      606 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/CommandInvocationInitial.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      627 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/CommandInvocationPrefix.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)    12792 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/CommandInvocationWithIO.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)    10730 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/CommandInvocationWithIOVars.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       51 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/Operand.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/__init__.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.414661 pash-annotations-0.2.1/pash_annotations/parser/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/__init__.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.402660 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.414661 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      111 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/_default_data_for_commands.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      748 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/cat.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      536 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/col.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      533 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/comm.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       37 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/custom_sort.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       37 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/custom_tr.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      808 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/cut.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3405 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/diff.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      200 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/export.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3751 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/grep.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      511 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/head.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      334 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/mkfifo.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      977 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/mv.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      720 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/rm.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1000 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/sed.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      370 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/seq.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2225 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/sort.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      819 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/tail.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      375 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/tee.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      383 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/tr.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      871 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/uniq.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1348 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/xargs.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     5999 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/parser.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1415 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/util_parser.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1671 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/util.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      304 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/util_flag_option.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      562 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/util_standard.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.406660 pash-annotations-0.2.1/pash_annotations.egg-info/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3592 2023-04-24 22:15:34.000000 pash-annotations-0.2.1/pash_annotations.egg-info/PKG-INFO
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     8174 2023-04-24 22:15:34.000000 pash-annotations-0.2.1/pash_annotations.egg-info/SOURCES.txt
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        1 2023-04-24 22:15:34.000000 pash-annotations-0.2.1/pash_annotations.egg-info/dependency_links.txt
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       17 2023-04-24 22:15:34.000000 pash-annotations-0.2.1/pash_annotations.egg-info/top_level.txt
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       38 2023-04-24 22:15:34.418661 pash-annotations-0.2.1/setup.cfg
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1305 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/setup.py
```

### Comparing `pash-annotations-0.2/LICENSE` & `pash-annotations-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/PKG-INFO` & `pash-annotations-0.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-Metadata-Version: 2.1
-Name: pash-annotations
-Version: 0.2
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Annotations
 
 This repository contains a framework for generating annotations for command invocations.
 It comprises a parser which turns a string into a command invocation data structure.
 For the time being, there are two sets of annotation generators:
 - input-output information which specifies how a command invocation interacts with the files, pipes, stdin, stdout, etc.
 - parallelizability information which describes how a command invocation can be parallelized - containing information about how to split inputs, mappers and aggregators, etc.
 
 ## Command-line tool
 `main.py` contains a command line tool which, provided a command invocation returns:
 - the parsed command invocation data structure
 - the input-output information generated
 - the parallelizability information generated
 
+## Adding an annotation
+
+- Add the command in the dictionary in (https://github.com/binpash/annotations/blob/main/pash_annotations/annotation_generation/AnnotationGeneration.py#L13)
+- Add an `InputOutputInfoGeneratorXXX.py` in (https://github.com/binpash/annotations/tree/main/pash_annotations/annotation_generation/annotation_generators)
+- (Optionally) add a `ParallelizabilityInfoGeneratorXXX.py` in (https://github.com/binpash/annotations/tree/main/pash_annotations/annotation_generation/annotation_generators)
+
 ## Parser
 Use command_flag_option_info JSON files to parse xbd-type terminal commands.
 Will split on spaces (`" "`) and equal signs (`"="`).
 
 ## Flag and Option Information
 The folder command_flag_option_info contains [command_name].json files with list of flags and options for each command. 
 For arguments that have two options (e.g. `-a` and `--all`), store them as a pair in the format [short version, long version].
@@ -55,8 +54,8 @@
 ## imports
 For clean imports, we add empty `__init__.py` modules in all non-root directories.
 Thus, `pytest` will add the root directory to sys.path and 
 we can import modules by prefixing the path from there.
 For instance, to import `Parallelizer.py`, we use 
 ```
 from annotation_generation.parallelizers.Parallelizer import Parallelizer
-```
+```
```

### Comparing `pash-annotations-0.2/README.md` & `pash-annotations-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,34 @@
+Metadata-Version: 2.1
+Name: pash-annotations
+Version: 0.2.1
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Annotations
 
 This repository contains a framework for generating annotations for command invocations.
 It comprises a parser which turns a string into a command invocation data structure.
 For the time being, there are two sets of annotation generators:
 - input-output information which specifies how a command invocation interacts with the files, pipes, stdin, stdout, etc.
 - parallelizability information which describes how a command invocation can be parallelized - containing information about how to split inputs, mappers and aggregators, etc.
 
 ## Command-line tool
 `main.py` contains a command line tool which, provided a command invocation returns:
 - the parsed command invocation data structure
 - the input-output information generated
 - the parallelizability information generated
 
+## Adding an annotation
+
+- Add the command in the dictionary in (https://github.com/binpash/annotations/blob/main/pash_annotations/annotation_generation/AnnotationGeneration.py#L13)
+- Add an `InputOutputInfoGeneratorXXX.py` in (https://github.com/binpash/annotations/tree/main/pash_annotations/annotation_generation/annotation_generators)
+- (Optionally) add a `ParallelizabilityInfoGeneratorXXX.py` in (https://github.com/binpash/annotations/tree/main/pash_annotations/annotation_generation/annotation_generators)
+
 ## Parser
 Use command_flag_option_info JSON files to parse xbd-type terminal commands.
 Will split on spaces (`" "`) and equal signs (`"="`).
 
 ## Flag and Option Information
 The folder command_flag_option_info contains [command_name].json files with list of flags and options for each command. 
 For arguments that have two options (e.g. `-a` and `--all`), store them as a pair in the format [short version, long version].
@@ -48,8 +61,8 @@
 ## imports
 For clean imports, we add empty `__init__.py` modules in all non-root directories.
 Thus, `pytest` will add the root directory to sys.path and 
 we can import modules by prefixing the path from there.
 For instance, to import `Parallelizer.py`, we use 
 ```
 from annotation_generation.parallelizers.Parallelizer import Parallelizer
-```
+```
```

### Comparing `pash-annotations-0.2/pash_annotations/annotation_cli.py` & `pash-annotations-0.2.1/pash_annotations/annotation_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from annotation_generation.datatypes.ParallelizabilityInfo import ParallelizabilityInfo
 from datatypes.CommandInvocationInitial import CommandInvocationInitial
 from parser.parser import parse
 
 parser = argparse.ArgumentParser()
 
 # add arguments to the parser
-parser.add_argument('--command_invocation', metavar='STRING', type=str,
+parser.add_argument('--command_invocation', metavar='STRING', type=str, required=True,
                     help='specifies the command invocation to check (enclosed by \")')
 parser.add_argument('--save_to', metavar='FILE', type=str, default=None,
                     help='store output in file (relative to where the script is called from); '
                          'will not overwrite existing files but then print instead')
 
 # parse the arguments
 options = parser.parse_args()
```

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/AnnotationGeneration.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/AnnotationGeneration.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,42 +7,44 @@
 from pash_annotations.annotation_generation.datatypes.ParallelizabilityInfo import ParallelizabilityInfo
 
 ### directory paths
 ROOT_DIR = os.path.realpath(os.path.join(os.path.dirname(__file__), '../..'))
 ANNOTATION_GENERATORS = "pash_annotations.annotation_generation.annotation_generators"
 
 DICT_CMD_NAME_TO_REPRESENTATION_IN_MODULE_NAMES = {
-    "grep": "Grep",
-    "mv":   "Mv",
-    "tr": "Tr",
+    "alt_bigrams_aux": "AltBigramsAux",
+    "alt_bigram_aux_reduce": "AltBigramAuxReduce",
+    "awk": "Awk",
+    "bigrams_aux": "BigramsAux",
+    "bigram_aux_map": "BigramAuxMap",
+    "bigram_aux_reduce": "BigramAuxReduce",
     "cat": "Cat",
-    "head": "Head",
-    "tail": "Tail",
-    "cut": "Cut",
-    "uniq": "Uniq",
+    "col": "Col",
     "comm": "Comm",
-    "sort": "Sort",
+    "custom_sort": "CustomSort",
+    "custom_tr": "CustomTr",
+    "cut": "Cut",
+    "diff": "Diff",
+    "grep": "Grep",
+    "head": "Head",
+    "mkfifo": "Mkfifo",
+    "mv":   "Mv",
+    "rm": "Rm",
     "sed": "Sed",
-    "col": "Col",
-    "xargs": "Xargs",
+    "set_diff": "SetDiff",
     "seq": "Seq",
+    "sort": "Sort",
+    "tail": "Tail",
+    "tee": "Tee",
     "test_one": "TestOne",
     "test_two": "TestTwo",
-    "alt_bigrams_aux": "AltBigramsAux",
-    "alt_bigram_aux_reduce": "AltBigramAuxReduce",
-    "mkfifo": "Mkfifo",
-    "diff": "Diff",
-    "rm": "Rm",
-    "tee": "Tee",
-    "custom_sort": "CustomSort",
-    "custom_tr": "CustomTr",
-    "set_diff": "SetDiff",
-    "bigrams_aux": "BigramsAux",
-    "bigram_aux_map": "BigramAuxMap",
-    "bigram_aux_reduce": "BigramAuxReduce"
+    "tr": "Tr",
+    "uniq": "Uniq",     
+    "wc": "Wc",
+    "xargs": "Xargs"
 }
 
 INPUTOUTPUT_INFO_FILENAME_MODULE_PREFIX = "InputOutputInfoGenerator"
 inputoutput_info_generator_prefix_abs = ANNOTATION_GENERATORS + '.' + INPUTOUTPUT_INFO_FILENAME_MODULE_PREFIX
 inputoutput_info_generator_file_module_names = \
     [(inputoutput_info_generator_prefix_abs + name, INPUTOUTPUT_INFO_FILENAME_MODULE_PREFIX + name)
             for name in DICT_CMD_NAME_TO_REPRESENTATION_IN_MODULE_NAMES.values()]
```

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/Generator_Interface.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/Generator_Interface.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCat.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCat.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorComm.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorComm.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCustomSort.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCustomSort.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCut.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCut.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorGrep.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorGrep.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorHead.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorHead.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorMv.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorMv.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSed.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSed.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSort.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSort.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTail.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTail.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTr.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTr.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorUniq.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorUniq.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGenerator_Interface.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGenerator_Interface.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorAltBigramsAux.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorAltBigramsAux.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorBigramsAux.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorBigramsAux.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCustomSort.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCustomSort.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCut.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCut.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorGrep.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorGrep.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSed.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSed.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSort.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSort.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTestOne.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTestOne.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTestTwo.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTestTwo.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTr.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTr.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorUniq.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorUniq.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGenerator_Interface.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGenerator_Interface.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/CommandProperties.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/CommandProperties.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/InputOutputInfo.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/InputOutputInfo.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/Inputs.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/Inputs.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/ParallelizabilityInfo.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/ParallelizabilityInfo.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/Aggregator.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/Aggregator.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/AggregatorKind.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/AggregatorKind.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/AggregatorSpec.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/AggregatorSpec.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/Mapper.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/Mapper.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/MapperSpec.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/MapperSpec.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/Parallelizer.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/Parallelizer.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/Splitter.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/Splitter.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/annotation_generation/datatypes/parallelizability/TransformerFlagOptionList.py` & `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/TransformerFlagOptionList.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/config/definitions.py` & `pash-annotations-0.2.1/pash_annotations/config/definitions.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/datatypes/AccessKind.py` & `pash-annotations-0.2.1/pash_annotations/datatypes/AccessKind.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/datatypes/BasicDatatypes.py` & `pash-annotations-0.2.1/pash_annotations/datatypes/BasicDatatypes.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/datatypes/BasicDatatypesWithIO.py` & `pash-annotations-0.2.1/pash_annotations/datatypes/BasicDatatypesWithIO.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/datatypes/BasicDatatypesWithIOVar.py` & `pash-annotations-0.2.1/pash_annotations/datatypes/BasicDatatypesWithIOVar.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/datatypes/CommandInvocationInitial.py` & `pash-annotations-0.2.1/pash_annotations/datatypes/CommandInvocationInitial.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/datatypes/CommandInvocationPrefix.py` & `pash-annotations-0.2.1/pash_annotations/datatypes/CommandInvocationPrefix.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/datatypes/CommandInvocationWithIO.py` & `pash-annotations-0.2.1/pash_annotations/datatypes/CommandInvocationWithIO.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/datatypes/CommandInvocationWithIOVars.py` & `pash-annotations-0.2.1/pash_annotations/datatypes/CommandInvocationWithIOVars.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/cat.json` & `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/cat.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/col.json` & `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/col.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/comm.json` & `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/comm.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/cut.json` & `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/cut.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/diff.json` & `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/diff.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/grep.json` & `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/grep.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/mv.json` & `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/mv.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/rm.json` & `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/rm.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/sed.json` & `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/sed.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/sort.json` & `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/sort.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/tail.json` & `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/tail.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/uniq.json` & `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/uniq.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/parser/command_flag_option_info/data/xargs.json` & `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/xargs.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/parser/parser.py` & `pash-annotations-0.2.1/pash_annotations/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/parser/util_parser.py` & `pash-annotations-0.2.1/pash_annotations/parser/util_parser.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/util.py` & `pash-annotations-0.2.1/pash_annotations/util.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations/util_standard.py` & `pash-annotations-0.2.1/pash_annotations/util_standard.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2/pash_annotations.egg-info/PKG-INFO` & `pash-annotations-0.2.1/pash_annotations.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pash-annotations
-Version: 0.2
+Version: 0.2.1
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Annotations
 
 This repository contains a framework for generating annotations for command invocations.
@@ -15,14 +15,20 @@
 
 ## Command-line tool
 `main.py` contains a command line tool which, provided a command invocation returns:
 - the parsed command invocation data structure
 - the input-output information generated
 - the parallelizability information generated
 
+## Adding an annotation
+
+- Add the command in the dictionary in (https://github.com/binpash/annotations/blob/main/pash_annotations/annotation_generation/AnnotationGeneration.py#L13)
+- Add an `InputOutputInfoGeneratorXXX.py` in (https://github.com/binpash/annotations/tree/main/pash_annotations/annotation_generation/annotation_generators)
+- (Optionally) add a `ParallelizabilityInfoGeneratorXXX.py` in (https://github.com/binpash/annotations/tree/main/pash_annotations/annotation_generation/annotation_generators)
+
 ## Parser
 Use command_flag_option_info JSON files to parse xbd-type terminal commands.
 Will split on spaces (`" "`) and equal signs (`"="`).
 
 ## Flag and Option Information
 The folder command_flag_option_info contains [command_name].json files with list of flags and options for each command. 
 For arguments that have two options (e.g. `-a` and `--all`), store them as a pair in the format [short version, long version].
```

### Comparing `pash-annotations-0.2/pash_annotations.egg-info/SOURCES.txt` & `pash-annotations-0.2.1/pash_annotations.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 pash_annotations.egg-info/dependency_links.txt
 pash_annotations.egg-info/top_level.txt
 pash_annotations/annotation_generation/AnnotationGeneration.py
 pash_annotations/annotation_generation/__init__.py
 pash_annotations/annotation_generation/annotation_generators/Generator_Interface.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorAltBigramAuxReduce.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorAltBigramsAux.py
+pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorAwk.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorBigramsAux.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCat.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCol.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorComm.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCustomSort.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCustomTr.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCut.py
@@ -35,14 +36,15 @@
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSort.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTail.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTee.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTestOne.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTestTwo.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTr.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorUniq.py
+pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorWc.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorXargs.py
 pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGenerator_Interface.py
 pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorAltBigramsAux.py
 pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorBigramsAux.py
 pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCol.py
 pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCustomSort.py
 pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCustomTr.py
```

### Comparing `pash-annotations-0.2/setup.py` & `pash-annotations-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 ##
 ## TODO: Rename the package names (and the name of the whole library)
 ##
 setup(name='pash-annotations',
-      version='0.2',
+      version='0.2.1',
       py_modules=['pash_annotations.util_flag_option',
                   'pash_annotations.util_new',
                   'pash_annotations.util_standard',
                   'pash_annotations.annotation_cli'],
       packages=['pash_annotations',
                 'pash_annotations.annotation_generation',
                 'pash_annotations.annotation_generation.annotation_generators',
```

