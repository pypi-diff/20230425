# Comparing `tmp/pash-annotations-0.2.1.tar.gz` & `tmp/pash-annotations-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pash-annotations-0.2.1.tar", last modified: Mon Apr 24 22:15:34 2023, max compression
+gzip compressed data, was "pash-annotations-0.2.2.tar", last modified: Mon Apr 24 22:49:33 2023, max compression
```

## Comparing `pash-annotations-0.2.1.tar` & `pash-annotations-0.2.2.tar`

### file list

```diff
@@ -1,127 +1,129 @@
-drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.418661 pash-annotations-0.2.1/
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1073 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/LICENSE
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       44 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/MANIFEST.in
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3592 2023-04-24 22:15:34.418661 pash-annotations-0.2.1/PKG-INFO
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3445 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/README.md
-drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.406660 pash-annotations-0.2.1/pash_annotations/
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/__init__.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2928 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_cli.py
-drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.406660 pash-annotations-0.2.1/pash_annotations/annotation_generation/
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     4344 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/AnnotationGeneration.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/__init__.py
-drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.410661 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1650 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/Generator_Interface.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      358 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorAltBigramAuxReduce.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      345 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorAltBigramsAux.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      887 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorAwk.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      341 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorBigramsAux.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      724 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCat.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      335 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCol.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      765 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorComm.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      645 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCustomSort.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      466 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCustomTr.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      685 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCut.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      343 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorDiff.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2565 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorGrep.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      565 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorHead.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      301 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorMkfifo.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2142 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorMv.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      296 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorRm.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      607 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSed.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      352 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSeq.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      469 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSetDiff.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      700 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSort.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      696 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTail.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      429 2023-04-24 22:14:38.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTee.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      339 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTestOne.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      339 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTestTwo.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      688 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTr.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1196 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorUniq.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      684 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorWc.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      507 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorXargs.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     7753 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGenerator_Interface.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1160 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorAltBigramsAux.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1160 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorBigramsAux.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      388 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCol.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2086 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCustomSort.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      391 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCustomTr.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      653 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCut.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     5800 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorGrep.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      986 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSed.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      462 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSetDiff.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2081 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSort.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1169 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTestOne.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1171 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTestTwo.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3223 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTr.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2291 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorUniq.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      456 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorXargs.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     4647 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGenerator_Interface.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/__init__.py
-drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.410661 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      773 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/CommandProperties.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)    11088 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/InputOutputInfo.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      735 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/Inputs.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1921 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/ParallelizabilityInfo.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/__init__.py
-drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.410661 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2963 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/Aggregator.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1420 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/AggregatorKind.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)    18849 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/AggregatorSpec.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2119 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/Mapper.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     7602 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/MapperSpec.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     7801 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/Parallelizer.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1187 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/Splitter.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     6880 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/TransformerFlagOptionList.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/__init__.py
-drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.414661 pash-annotations-0.2.1/pash_annotations/config/
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/config/__init__.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2846 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/config/definitions.py
-drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.414661 pash-annotations-0.2.1/pash_annotations/datatypes/
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2943 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/AccessKind.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     4832 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/BasicDatatypes.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     5618 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/BasicDatatypesWithIO.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      568 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/BasicDatatypesWithIOVar.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      606 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/CommandInvocationInitial.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      627 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/CommandInvocationPrefix.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)    12792 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/CommandInvocationWithIO.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)    10730 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/CommandInvocationWithIOVars.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       51 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/Operand.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/datatypes/__init__.py
-drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.414661 pash-annotations-0.2.1/pash_annotations/parser/
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/__init__.py
-drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.402660 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/
-drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.414661 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      111 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/_default_data_for_commands.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      748 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/cat.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      536 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/col.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      533 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/comm.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       37 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/custom_sort.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       37 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/custom_tr.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      808 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/cut.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3405 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/diff.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      200 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/export.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3751 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/grep.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      511 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/head.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      334 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/mkfifo.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      977 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/mv.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      720 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/rm.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1000 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/sed.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      370 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/seq.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2225 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/sort.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      819 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/tail.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      375 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/tee.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      383 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/tr.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      871 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/uniq.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1348 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/xargs.json
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     5999 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/parser.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1415 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/parser/util_parser.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1671 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/util.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      304 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/util_flag_option.py
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      562 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/pash_annotations/util_standard.py
-drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:15:34.406660 pash-annotations-0.2.1/pash_annotations.egg-info/
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3592 2023-04-24 22:15:34.000000 pash-annotations-0.2.1/pash_annotations.egg-info/PKG-INFO
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     8174 2023-04-24 22:15:34.000000 pash-annotations-0.2.1/pash_annotations.egg-info/SOURCES.txt
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        1 2023-04-24 22:15:34.000000 pash-annotations-0.2.1/pash_annotations.egg-info/dependency_links.txt
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       17 2023-04-24 22:15:34.000000 pash-annotations-0.2.1/pash_annotations.egg-info/top_level.txt
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       38 2023-04-24 22:15:34.418661 pash-annotations-0.2.1/setup.cfg
--rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1305 2023-04-24 22:14:39.000000 pash-annotations-0.2.1/setup.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:49:33.641961 pash-annotations-0.2.2/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1073 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/LICENSE
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       44 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/MANIFEST.in
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3916 2023-04-24 22:49:33.641961 pash-annotations-0.2.2/PKG-INFO
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3769 2023-04-24 22:47:39.000000 pash-annotations-0.2.2/README.md
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:49:33.629961 pash-annotations-0.2.2/pash_annotations/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/__init__.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2928 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_cli.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:49:33.629961 pash-annotations-0.2.2/pash_annotations/annotation_generation/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     4344 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/AnnotationGeneration.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/__init__.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:49:33.637961 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1650 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/Generator_Interface.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      358 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorAltBigramAuxReduce.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      345 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorAltBigramsAux.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      883 2023-04-24 22:47:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorAwk.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      341 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorBigramsAux.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      724 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCat.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      335 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCol.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      765 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorComm.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      645 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCustomSort.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      466 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCustomTr.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      685 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCut.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      343 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorDiff.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2565 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorGrep.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      565 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorHead.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      301 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorMkfifo.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2142 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorMv.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      296 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorRm.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      607 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSed.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      352 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSeq.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      469 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSetDiff.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      700 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSort.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      696 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTail.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      429 2023-04-24 22:14:38.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTee.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      339 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTestOne.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      339 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTestTwo.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      688 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTr.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1196 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorUniq.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      684 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorWc.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      507 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorXargs.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     7753 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGenerator_Interface.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1160 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorAltBigramsAux.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1160 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorBigramsAux.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      388 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCol.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2086 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCustomSort.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      391 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCustomTr.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      653 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCut.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     5800 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorGrep.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      986 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSed.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      462 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSetDiff.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2081 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSort.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1169 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTestOne.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1171 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTestTwo.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3223 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTr.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2291 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorUniq.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      456 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorXargs.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     4647 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGenerator_Interface.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/__init__.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:49:33.637961 pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      773 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/CommandProperties.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)    11088 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/InputOutputInfo.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      735 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/Inputs.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1921 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/ParallelizabilityInfo.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/__init__.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:49:33.637961 pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2963 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/Aggregator.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1420 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/AggregatorKind.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)    18849 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/AggregatorSpec.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2119 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/Mapper.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     7602 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/MapperSpec.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     7801 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/Parallelizer.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1187 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/Splitter.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     6880 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/TransformerFlagOptionList.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/__init__.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:49:33.637961 pash-annotations-0.2.2/pash_annotations/config/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/config/__init__.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2846 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/config/definitions.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:49:33.637961 pash-annotations-0.2.2/pash_annotations/datatypes/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2943 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/datatypes/AccessKind.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     4832 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/datatypes/BasicDatatypes.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     5618 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/datatypes/BasicDatatypesWithIO.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      568 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/datatypes/BasicDatatypesWithIOVar.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      606 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/datatypes/CommandInvocationInitial.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      627 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/datatypes/CommandInvocationPrefix.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)    12792 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/datatypes/CommandInvocationWithIO.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)    10730 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/datatypes/CommandInvocationWithIOVars.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       51 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/datatypes/Operand.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/datatypes/__init__.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:49:33.637961 pash-annotations-0.2.2/pash_annotations/parser/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/__init__.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:49:33.629961 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:49:33.641961 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      111 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/_default_data_for_commands.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1701 2023-04-24 22:47:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/awk.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      748 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/cat.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      536 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/col.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      533 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/comm.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       37 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/custom_sort.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       37 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/custom_tr.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      808 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/cut.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3405 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/diff.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      200 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/export.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3751 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/grep.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      511 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/head.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      334 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/mkfifo.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      977 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/mv.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      720 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/rm.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1000 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/sed.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      370 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/seq.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     2225 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/sort.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      819 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/tail.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      375 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/tee.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      383 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/tr.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      871 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/uniq.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      516 2023-04-24 22:47:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/wc.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1348 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/xargs.json
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     5999 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/parser.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1415 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/parser/util_parser.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1671 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/util.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      304 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/util_flag_option.py
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)      562 2023-04-24 22:14:39.000000 pash-annotations-0.2.2/pash_annotations/util_standard.py
+drwxr-xr-x   0 kallas   (20001) pash-PG0  (7111)        0 2023-04-24 22:49:33.629961 pash-annotations-0.2.2/pash_annotations.egg-info/
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     3916 2023-04-24 22:49:33.000000 pash-annotations-0.2.2/pash_annotations.egg-info/PKG-INFO
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     8299 2023-04-24 22:49:33.000000 pash-annotations-0.2.2/pash_annotations.egg-info/SOURCES.txt
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)        1 2023-04-24 22:49:33.000000 pash-annotations-0.2.2/pash_annotations.egg-info/dependency_links.txt
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       17 2023-04-24 22:49:33.000000 pash-annotations-0.2.2/pash_annotations.egg-info/top_level.txt
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)       38 2023-04-24 22:49:33.641961 pash-annotations-0.2.2/setup.cfg
+-rw-r--r--   0 kallas   (20001) pash-PG0  (7111)     1305 2023-04-24 22:48:42.000000 pash-annotations-0.2.2/setup.py
```

### Comparing `pash-annotations-0.2.1/LICENSE` & `pash-annotations-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/PKG-INFO` & `pash-annotations-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pash-annotations
-Version: 0.2.1
+Version: 0.2.2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Annotations
 
 This repository contains a framework for generating annotations for command invocations.
@@ -18,14 +18,15 @@
 - the parsed command invocation data structure
 - the input-output information generated
 - the parallelizability information generated
 
 ## Adding an annotation
 
 - Add the command in the dictionary in (https://github.com/binpash/annotations/blob/main/pash_annotations/annotation_generation/AnnotationGeneration.py#L13)
+- Add a json file with the command flags in (https://github.com/binpash/annotations/tree/main/pash_annotations/parser/command_flag_option_info/data). This could be used to generate a first version of it: (https://github.com/binpash/annotations/blob/main/pash_annotations/parser/command_flag_option_info/manpage-to-json.sh).
 - Add an `InputOutputInfoGeneratorXXX.py` in (https://github.com/binpash/annotations/tree/main/pash_annotations/annotation_generation/annotation_generators)
 - (Optionally) add a `ParallelizabilityInfoGeneratorXXX.py` in (https://github.com/binpash/annotations/tree/main/pash_annotations/annotation_generation/annotation_generators)
 
 ## Parser
 Use command_flag_option_info JSON files to parse xbd-type terminal commands.
 Will split on spaces (`" "`) and equal signs (`"="`).
```

### Comparing `pash-annotations-0.2.1/README.md` & `pash-annotations-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 - the parsed command invocation data structure
 - the input-output information generated
 - the parallelizability information generated
 
 ## Adding an annotation
 
 - Add the command in the dictionary in (https://github.com/binpash/annotations/blob/main/pash_annotations/annotation_generation/AnnotationGeneration.py#L13)
+- Add a json file with the command flags in (https://github.com/binpash/annotations/tree/main/pash_annotations/parser/command_flag_option_info/data). This could be used to generate a first version of it: (https://github.com/binpash/annotations/blob/main/pash_annotations/parser/command_flag_option_info/manpage-to-json.sh).
 - Add an `InputOutputInfoGeneratorXXX.py` in (https://github.com/binpash/annotations/tree/main/pash_annotations/annotation_generation/annotation_generators)
 - (Optionally) add a `ParallelizabilityInfoGeneratorXXX.py` in (https://github.com/binpash/annotations/tree/main/pash_annotations/annotation_generation/annotation_generators)
 
 ## Parser
 Use command_flag_option_info JSON files to parse xbd-type terminal commands.
 Will split on spaces (`" "`) and equal signs (`"="`).
```

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_cli.py` & `pash-annotations-0.2.2/pash_annotations/annotation_cli.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/AnnotationGeneration.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/AnnotationGeneration.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/Generator_Interface.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/Generator_Interface.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorAwk.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorAwk.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,12 +9,12 @@
         ## Does this set -f as configuration input?
         if self.does_flag_option_list_contain_at_least_one_of(["-f"]):
             if self.get_operand_list_length() == 0:
                 self.set_implicit_use_of_stdin()
             else:
                 self.all_operands_are_streaming_inputs() # this is true also if empty
         else:
+            self.set_first_operand_as_config_arg_type_string()
             if self.get_operand_list_length() == 1:
                 self.set_implicit_use_of_stdin()
             else:
-                self.set_first_operand_as_config_arg_type_string()
                 self.all_but_first_operand_is_streaming_input()
```

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCat.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCat.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorComm.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorComm.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCustomSort.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCustomSort.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCut.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorCut.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorGrep.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorGrep.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorHead.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorHead.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorMv.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorMv.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSed.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSed.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSort.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorSort.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTail.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTail.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTr.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorTr.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorUniq.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorUniq.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorWc.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGeneratorWc.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGenerator_Interface.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/InputOutputInfoGenerator_Interface.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorAltBigramsAux.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorAltBigramsAux.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorBigramsAux.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorBigramsAux.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCustomSort.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCustomSort.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCut.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorCut.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorGrep.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorGrep.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSed.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSed.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSort.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorSort.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTestOne.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTestOne.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTestTwo.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTestTwo.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTr.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorTr.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorUniq.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGeneratorUniq.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGenerator_Interface.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/annotation_generators/ParallelizabilityInfoGenerator_Interface.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/CommandProperties.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/CommandProperties.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/InputOutputInfo.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/InputOutputInfo.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/Inputs.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/Inputs.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/ParallelizabilityInfo.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/ParallelizabilityInfo.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/Aggregator.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/Aggregator.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/AggregatorKind.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/AggregatorKind.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/AggregatorSpec.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/AggregatorSpec.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/Mapper.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/Mapper.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/MapperSpec.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/MapperSpec.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/Parallelizer.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/Parallelizer.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/Splitter.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/Splitter.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/annotation_generation/datatypes/parallelizability/TransformerFlagOptionList.py` & `pash-annotations-0.2.2/pash_annotations/annotation_generation/datatypes/parallelizability/TransformerFlagOptionList.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/config/definitions.py` & `pash-annotations-0.2.2/pash_annotations/config/definitions.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/datatypes/AccessKind.py` & `pash-annotations-0.2.2/pash_annotations/datatypes/AccessKind.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/datatypes/BasicDatatypes.py` & `pash-annotations-0.2.2/pash_annotations/datatypes/BasicDatatypes.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/datatypes/BasicDatatypesWithIO.py` & `pash-annotations-0.2.2/pash_annotations/datatypes/BasicDatatypesWithIO.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/datatypes/BasicDatatypesWithIOVar.py` & `pash-annotations-0.2.2/pash_annotations/datatypes/BasicDatatypesWithIOVar.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/datatypes/CommandInvocationInitial.py` & `pash-annotations-0.2.2/pash_annotations/datatypes/CommandInvocationInitial.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/datatypes/CommandInvocationPrefix.py` & `pash-annotations-0.2.2/pash_annotations/datatypes/CommandInvocationPrefix.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/datatypes/CommandInvocationWithIO.py` & `pash-annotations-0.2.2/pash_annotations/datatypes/CommandInvocationWithIO.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/datatypes/CommandInvocationWithIOVars.py` & `pash-annotations-0.2.2/pash_annotations/datatypes/CommandInvocationWithIOVars.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/cat.json` & `pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/cat.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/col.json` & `pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/col.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/comm.json` & `pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/comm.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/cut.json` & `pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/cut.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/diff.json` & `pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/diff.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/grep.json` & `pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/grep.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/mv.json` & `pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/mv.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/rm.json` & `pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/rm.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/sed.json` & `pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/sed.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/sort.json` & `pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/sort.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/tail.json` & `pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/tail.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/uniq.json` & `pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/uniq.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/parser/command_flag_option_info/data/xargs.json` & `pash-annotations-0.2.2/pash_annotations/parser/command_flag_option_info/data/xargs.json`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/parser/parser.py` & `pash-annotations-0.2.2/pash_annotations/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/parser/util_parser.py` & `pash-annotations-0.2.2/pash_annotations/parser/util_parser.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/util.py` & `pash-annotations-0.2.2/pash_annotations/util.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations/util_standard.py` & `pash-annotations-0.2.2/pash_annotations/util_standard.py`

 * *Files identical despite different names*

### Comparing `pash-annotations-0.2.1/pash_annotations.egg-info/PKG-INFO` & `pash-annotations-0.2.2/pash_annotations.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pash-annotations
-Version: 0.2.1
+Version: 0.2.2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Annotations
 
 This repository contains a framework for generating annotations for command invocations.
@@ -18,14 +18,15 @@
 - the parsed command invocation data structure
 - the input-output information generated
 - the parallelizability information generated
 
 ## Adding an annotation
 
 - Add the command in the dictionary in (https://github.com/binpash/annotations/blob/main/pash_annotations/annotation_generation/AnnotationGeneration.py#L13)
+- Add a json file with the command flags in (https://github.com/binpash/annotations/tree/main/pash_annotations/parser/command_flag_option_info/data). This could be used to generate a first version of it: (https://github.com/binpash/annotations/blob/main/pash_annotations/parser/command_flag_option_info/manpage-to-json.sh).
 - Add an `InputOutputInfoGeneratorXXX.py` in (https://github.com/binpash/annotations/tree/main/pash_annotations/annotation_generation/annotation_generators)
 - (Optionally) add a `ParallelizabilityInfoGeneratorXXX.py` in (https://github.com/binpash/annotations/tree/main/pash_annotations/annotation_generation/annotation_generators)
 
 ## Parser
 Use command_flag_option_info JSON files to parse xbd-type terminal commands.
 Will split on spaces (`" "`) and equal signs (`"="`).
```

### Comparing `pash-annotations-0.2.1/pash_annotations.egg-info/SOURCES.txt` & `pash-annotations-0.2.2/pash_annotations.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 pash_annotations/datatypes/CommandInvocationWithIOVars.py
 pash_annotations/datatypes/Operand.py
 pash_annotations/datatypes/__init__.py
 pash_annotations/parser/__init__.py
 pash_annotations/parser/parser.py
 pash_annotations/parser/util_parser.py
 pash_annotations/parser/command_flag_option_info/data/_default_data_for_commands.json
+pash_annotations/parser/command_flag_option_info/data/awk.json
 pash_annotations/parser/command_flag_option_info/data/cat.json
 pash_annotations/parser/command_flag_option_info/data/col.json
 pash_annotations/parser/command_flag_option_info/data/comm.json
 pash_annotations/parser/command_flag_option_info/data/custom_sort.json
 pash_annotations/parser/command_flag_option_info/data/custom_tr.json
 pash_annotations/parser/command_flag_option_info/data/cut.json
 pash_annotations/parser/command_flag_option_info/data/diff.json
@@ -106,8 +107,9 @@
 pash_annotations/parser/command_flag_option_info/data/sed.json
 pash_annotations/parser/command_flag_option_info/data/seq.json
 pash_annotations/parser/command_flag_option_info/data/sort.json
 pash_annotations/parser/command_flag_option_info/data/tail.json
 pash_annotations/parser/command_flag_option_info/data/tee.json
 pash_annotations/parser/command_flag_option_info/data/tr.json
 pash_annotations/parser/command_flag_option_info/data/uniq.json
+pash_annotations/parser/command_flag_option_info/data/wc.json
 pash_annotations/parser/command_flag_option_info/data/xargs.json
```

### Comparing `pash-annotations-0.2.1/setup.py` & `pash-annotations-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 ##
 ## TODO: Rename the package names (and the name of the whole library)
 ##
 setup(name='pash-annotations',
-      version='0.2.1',
+      version='0.2.2',
       py_modules=['pash_annotations.util_flag_option',
                   'pash_annotations.util_new',
                   'pash_annotations.util_standard',
                   'pash_annotations.annotation_cli'],
       packages=['pash_annotations',
                 'pash_annotations.annotation_generation',
                 'pash_annotations.annotation_generation.annotation_generators',
```

