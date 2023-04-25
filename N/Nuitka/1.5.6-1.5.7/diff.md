# Comparing `tmp/Nuitka-1.5.6.tar.gz` & `tmp/Nuitka-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Nuitka-1.5.6.tar", last modified: Wed Apr 12 06:01:51 2023, max compression
+gzip compressed data, was "Nuitka-1.5.7.tar", last modified: Tue Apr 25 08:09:13 2023, max compression, from Unix
```

## Comparing `Nuitka-1.5.6.tar` & `Nuitka-1.5.7.tar`

### file list

```diff
@@ -1,1798 +1,1797 @@
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    91155 2023-04-12 06:01:51.000000 Nuitka-1.5.6/PKG-INFO
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15350 2023-04-12 05:59:07.000000 Nuitka-1.5.6/setup.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/bin/
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1163 2023-04-12 05:59:07.000000 Nuitka-1.5.6/bin/measure-construct-performance
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1136 2023-04-12 05:59:07.000000 Nuitka-1.5.6/bin/check-nuitka-with-pylint
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1685 2023-04-12 05:59:07.000000 Nuitka-1.5.6/bin/nuitka-run
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1135 2023-04-12 05:59:07.000000 Nuitka-1.5.6/bin/autoformat-nuitka-source
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1150 2023-04-12 05:59:07.000000 Nuitka-1.5.6/bin/compare_with_cpython
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3079 2023-04-12 05:59:07.000000 Nuitka-1.5.6/bin/compare_with_xml
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1685 2023-04-12 05:59:07.000000 Nuitka-1.5.6/bin/nuitka
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   336039 2023-04-12 06:00:34.000000 Nuitka-1.5.6/README.pdf
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/doc/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/doc/Logo/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17917 2023-04-12 05:59:07.000000 Nuitka-1.5.6/doc/Logo/Nuitka-Logo-Vertical.svg
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7401 2023-04-12 05:59:07.000000 Nuitka-1.5.6/doc/Logo/Nuitka-Logo-Symbol.svg
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7321 2023-04-12 05:59:07.000000 Nuitka-1.5.6/doc/Logo/Nuitka-Logo-Horizontal.svg
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/doc/images/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7585 2023-04-12 05:59:07.000000 Nuitka-1.5.6/doc/images/Nuitka-Logo-Horizontal.png
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9828 2023-04-12 05:59:07.000000 Nuitka-1.5.6/doc/images/Nuitka-Logo-Vertical.png
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4452 2023-04-12 05:59:07.000000 Nuitka-1.5.6/doc/images/Nuitka-Logo-Symbol.png
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    29732 2023-04-12 06:01:48.000000 Nuitka-1.5.6/doc/nuitka3-run.1
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    29740 2023-04-12 06:01:43.000000 Nuitka-1.5.6/doc/nuitka2.1
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    29716 2023-04-12 06:01:43.000000 Nuitka-1.5.6/doc/nuitka2-run.1
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    29756 2023-04-12 06:01:48.000000 Nuitka-1.5.6/doc/nuitka3.1
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   801878 2023-04-12 05:59:07.000000 Nuitka-1.5.6/Changelog.rst
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       38 2023-04-12 06:01:51.000000 Nuitka-1.5.6/setup.cfg
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   809671 2023-04-12 06:00:49.000000 Nuitka-1.5.6/Developer_Manual.pdf
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    73222 2023-04-12 05:59:07.000000 Nuitka-1.5.6/README.rst
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   152121 2023-04-12 05:59:07.000000 Nuitka-1.5.6/Developer_Manual.rst
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/Nuitka.egg-info/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    91155 2023-04-12 06:01:48.000000 Nuitka-1.5.6/Nuitka.egg-info/PKG-INFO
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        7 2023-04-12 06:01:48.000000 Nuitka-1.5.6/Nuitka.egg-info/top_level.txt
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    76486 2023-04-12 06:01:49.000000 Nuitka-1.5.6/Nuitka.egg-info/SOURCES.txt
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        1 2023-04-12 06:01:48.000000 Nuitka-1.5.6/Nuitka.egg-info/dependency_links.txt
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      394 2023-04-12 06:01:48.000000 Nuitka-1.5.6/Nuitka.egg-info/entry_points.txt
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        1 2023-04-12 06:01:48.000000 Nuitka-1.5.6/Nuitka.egg-info/not-zip-safe
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       31 2023-04-12 06:01:48.000000 Nuitka-1.5.6/Nuitka.egg-info/requires.txt
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)  2697334 2023-04-12 06:01:26.000000 Nuitka-1.5.6/Changelog.pdf
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1741 2023-04-12 05:59:07.000000 Nuitka-1.5.6/MANIFEST.in
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7236 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/Builtins.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2433 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/DataComposerInterface.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/build/static_src/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    47568 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceLshift.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13776 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13057 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersCalling.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   314618 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersComparisonNe.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3805 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersPythonPgo.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    67487 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    77782 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryBitor.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4037 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersTuples.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   315628 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersComparisonLt.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    68748 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    76343 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11945 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/InspectPatcher.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    38320 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersDictionaries.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   136100 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceMod.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18993 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersAllocator.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3033 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersBytes.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26221 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   181243 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryAdd.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17065 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21493 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/CompiledMethodType.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21783 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersBuiltin.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7035 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersExceptions.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    36011 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersConstantsBlob.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    74142 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    60657 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/CompiledGeneratorType.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    82114 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/CompiledAsyncgenType.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    53224 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceBitand.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   107641 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3650 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   313003 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersComparisonGe.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3730 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersSequences.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    53224 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11094 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersSafeStrings.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17742 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    57572 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/CompiledCodeHelpers.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    58321 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/MetaPathBasedLoader.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    66453 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    83405 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryLshift.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6411 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersFiles.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26642 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersStrings.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   183202 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryMod.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    35865 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/CompiledFrameType.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    24294 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersDictionariesGenerated.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   188514 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryMult.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4673 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersComparisonEqUtils.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2991 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersClasses.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   149580 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceAdd.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3513 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersMatching.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13589 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersImportHard.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    45052 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceRshift.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2426 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersFloats.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    30783 2023-04-12 06:00:15.000000 Nuitka-1.5.6/nuitka/build/static_src/OnefileBootstrap.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6274 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    53122 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceBitor.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    93999 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/CompiledFunctionType.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6427 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    76512 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8250 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/CompiledCellType.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16700 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    82842 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceSub.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11199 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersFilesystemPaths.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   316217 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersComparisonLe.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13915 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersListsGenerated.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   460993 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersCallingGenerated.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14561 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersImport.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5578 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersTypes.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    40893 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/MainProgram.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1774 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersHeapStorage.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    78891 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryPow.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   312414 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersComparisonGt.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1236 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    77943 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryBitand.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1640 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersMappings.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4071 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    82669 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplacePow.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    70465 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinarySub.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    77305 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryRshift.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7800 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/OnefileSplashScreen.cpp
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    68005 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1946 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersSlices.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   317872 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersComparisonEq.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1023 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3219 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersProfiling.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    32656 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersAttributes.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18391 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersLists.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1617 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersChecksumTools.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    70973 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/CompiledCoroutineType.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   142211 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceMult.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15369 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersRaising.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3404 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19313 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersDeepcopy.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    77943 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/include/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3144 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/tracing.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14375 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helpers.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1261 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/checksum_tools.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16949 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/compiled_frame.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9136 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/compiled_generator.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12979 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/incbin.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7769 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/allocator.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2002 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/compiled_cell.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1977 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/checkers.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6253 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/freelists.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5972 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/compiled_function.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2830 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/unfreezing.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3840 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/threading.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    33190 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/exceptions.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7408 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/constants.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2119 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/safe_string_ops.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14248 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/prelude.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9571 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/compiled_asyncgen.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1293 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/constants_blob.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3221 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/filesystem_paths.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5363 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/importing.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3423 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/builtins.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1838 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/compiled_method.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1761 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/python_pgo.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2870 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/printing.h
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2941 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/ints.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10616 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/comparisons_ge.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1112 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/sequences.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12685 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_add.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1798 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/indexes.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13140 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/comparisons_le.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5438 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9201 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5422 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10626 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15100 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_builtin_types.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1181 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/bytearrays.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5147 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5824 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_sub.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5791 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8419 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/slices.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1633 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/lists_generated.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4846 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5115 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3397 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/lists.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5641 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10616 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/comparisons_ne.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8670 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_add.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3011 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1206 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/floats.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2663 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/boolean.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4573 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9992 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/iterators.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1242 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/strings.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1025 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/sets.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3767 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3753 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3297 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/raising.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1146 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/richcomparisons.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13139 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/comparisons_lt.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4714 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_pow.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4349 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3275 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/attributes.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1328 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/mappings.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15778 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_mod.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13210 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_mult.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13077 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/dictionaries.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2799 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4975 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10615 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/comparisons_gt.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9335 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/calling_generated.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2727 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4826 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5663 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5460 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5115 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13140 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/comparisons_eq.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1135 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/bytes.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5720 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/tuples.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3011 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3674 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/import_hard.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5663 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2178 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/rangeobjects.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1743 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/complex.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17447 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/subscripts.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3767 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9325 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/compiled_coroutine.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    86326 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/hedley.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4460 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/include/nuitka/calling.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18493 2023-04-12 06:00:15.000000 Nuitka-1.5.6/nuitka/build/Onefile.scons
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5527 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/SconsHacks.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11960 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/SconsSpawn.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    33043 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/Backend.scons
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    29044 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/SconsCompilerSettings.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15210 2023-04-12 06:00:15.000000 Nuitka-1.5.6/nuitka/build/SconsCaching.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8314 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/CCompilerVersion.scons
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/clcache/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/clcache/clcache/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1585 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/clcache/clcache/LICENSE
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       93 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/clcache/clcache/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    65424 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/clcache/clcache/caching.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/glob2/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/glob2/glob2/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8304 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/glob2/glob2/impl.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       82 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/glob2/glob2/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6859 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/glob2/glob2/compat.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4463 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1359 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/glob2/LICENSE
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1101 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/LICENSE
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14184 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/representer.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4165 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/serializer.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6794 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/reader.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2445 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/events.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2061 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/loader.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13170 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    43006 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/emitter.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    25495 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/parser.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1440 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/nodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2573 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/tokens.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    51277 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/scanner.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8999 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/resolver.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    28639 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/constructor.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4883 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/composer.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2533 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/error.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3851 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/cyaml.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2837 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/dumper.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/appdirs/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    24824 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/appdirs/appdirs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1097 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/appdirs/LICENSE.txt
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17474 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    50849 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2616 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    24500 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    20501 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    35875 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    30853 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    36528 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4340 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    28559 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9197 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2685 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1400 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17080 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7308 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12281 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1722 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4214 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3316 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    65386 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    27644 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12719 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1726 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1626 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4428 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       84 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/README.rst
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1466 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17473 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    50849 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/environment.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2423 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    24500 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/ext.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    20501 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/utils.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    35875 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/parser.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    30853 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    36528 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/filters.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4340 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/meta.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    28559 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9197 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2685 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1400 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17080 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7308 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12281 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/debug.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1722 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4214 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/tests.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3316 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    65386 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    27644 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12719 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1726 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1626 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/constants.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4428 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       85 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/README.rst
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1467 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/LICENSE.rst
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/bin/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1331 2023-04-12 06:00:15.000000 Nuitka-1.5.6/nuitka/build/inline_copy/bin/scons.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1101 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/LICENSE
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14097 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/representer.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4165 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6854 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/reader.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2445 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/events.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1138 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/loader.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9607 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    42954 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    25495 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/parser.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1440 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2573 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    51695 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8970 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    25554 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4881 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/composer.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2533 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/error.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3294 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2723 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1101 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/LICENSE
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17711 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/representer.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4171 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6746 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/reader.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2445 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/events.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1132 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/loader.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9776 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    43298 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    25542 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/parser.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1440 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2573 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    52446 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9122 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    25145 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4921 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/composer.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2559 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/error.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3290 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2719 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/atomicwrites/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1069 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/atomicwrites/LICENSE
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6794 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   138334 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/zstd.h
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13662 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/entropy_common.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    20216 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/huf.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15880 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/zstd_internal.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3009 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/error_private.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3763 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/debug.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18198 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/bitstream.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2728 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/zstd_common.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    34422 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/fse.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26976 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/xxhash.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3828 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/zstd_errors.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2497 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/zstd_deps.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2441 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/error_private.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11706 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/xxhash.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4455 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/cpu.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14748 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/fse_decompress.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13930 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/mem.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10157 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/compiler.h
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/decompress/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7906 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2253 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    54982 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    66784 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1321 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9164 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    80283 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1530 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/zstd/LICENSE.txt
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      283 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_main.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3687 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      307 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5943 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/gui.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1591 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      888 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9533 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/utils.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10790 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1376 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/dask.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      287 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_gui.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      857 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      596 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    57572 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/std.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      283 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      333 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/version.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1106 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/auto.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6948 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/tk.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/markupsafe/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1873 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10126 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4690 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      558 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1467 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/markupsafe/LICENSE.rst
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16000 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1950 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2614 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2736 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1965 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1950 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1950 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    40510 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    44500 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2465 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8120 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1742 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1776 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3596 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19253 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1818 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1563 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8467 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7509 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    33996 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8083 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    24133 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14053 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    40719 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14029 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    52665 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    48938 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    49503 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4197 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   121420 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4164 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12950 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1991 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4381 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3730 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2166 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2433 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2256 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2657 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1844 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2333 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3328 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4782 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2945 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2077 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2433 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1902 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1831 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2513 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    72761 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2147 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1804 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2309 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2025 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2168 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2328 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4375 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2639 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    31283 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13881 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5992 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    25816 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2681 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18600 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4224 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3472 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8394 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13016 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2123 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2004 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14869 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2078 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    20832 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19499 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2784 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9248 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2473 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2796 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11380 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2681 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2936 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18084 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2460 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2827 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2290 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2935 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5149 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3428 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1711 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      142 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3579 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3953 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2379 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4695 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2720 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1810 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2618 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2267 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1819 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6841 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1927 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3415 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2349 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3432 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2777 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2502 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4658 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6919 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3763 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2859 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2043 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    29618 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2140 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3785 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14663 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3751 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4810 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2011 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3233 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    34903 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19664 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21540 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7358 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    96183 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2305 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6824 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9589 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    27693 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14948 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1605 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4179 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2483 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3131 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9314 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2170 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1989 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1882 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1718 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17622 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2107 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6938 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    39700 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    47844 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3557 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11034 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3784 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5612 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3007 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4404 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16583 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    41191 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3395 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4307 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1644 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      353 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8183 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9295 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    35213 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15278 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6632 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11061 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26676 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14272 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    42760 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13597 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    53509 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    71693 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    63768 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5126 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   136271 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6167 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14673 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1563 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4577 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3259 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3687 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2122 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1891 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2206 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4879 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2900 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1954 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1851 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1786 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2479 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    84784 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2141 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1752 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2266 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2387 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3296 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4817 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1557 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    32724 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14473 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6412 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    25826 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19180 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4113 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3616 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2588 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12548 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2006 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1943 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15027 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2014 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    22570 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    38783 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2734 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13182 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2429 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7993 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12902 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1544 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1661 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15570 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2437 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2788 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2889 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4368 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3379 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1663 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2377 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3576 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3931 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1578 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1569 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2616 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1772 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2526 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2386 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2677 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2573 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1999 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2228 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1780 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      343 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3534 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6788 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1888 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6064 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4649 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7652 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4076 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2419 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1567 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7461 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2271 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4517 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8622 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1995 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2893 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2096 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3742 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15577 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4357 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7394 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1972 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3546 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    36753 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21614 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21937 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7515 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    97269 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6785 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9430 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    27408 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14831 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1536 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4356 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2630 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3087 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12836 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3860 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2076 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2107 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1805 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1311 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1674 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21423 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2032 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7884 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    41983 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    56578 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3979 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3536 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12708 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3896 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5588 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3134 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4672 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16068 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    42204 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6869 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1784 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1647 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8354 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9002 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    34985 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13596 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26467 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14489 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    39394 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13779 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    53260 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    53803 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    63474 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5239 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   135413 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5758 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13880 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1652 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4956 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3444 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3773 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2211 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1977 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2386 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5335 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2987 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2123 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1944 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1873 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2567 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    82939 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2226 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1847 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2351 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2475 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3389 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4904 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1645 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    50660 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14751 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6756 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26195 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15791 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4808 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3686 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13924 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13982 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2176 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2057 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15165 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2152 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21762 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    33537 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2855 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10674 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2515 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8618 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12588 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1630 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2978 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18207 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2948 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2877 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2977 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4464 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3472 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1753 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2580 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3663 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4041 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1667 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1658 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2840 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1859 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2655 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2475 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2765 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2660 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2088 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2316 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1868 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      313 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3631 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6883 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1976 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3201 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2583 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1653 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8494 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2366 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5235 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7808 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2085 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    29765 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2189 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3827 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15053 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3812 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4853 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2328 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3643 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    35863 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19816 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    22350 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7752 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    96818 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6504 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9565 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    28403 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16962 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1654 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4476 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2739 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3180 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11500 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4003 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2219 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2227 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1931 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1460 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1767 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    20988 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2149 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7533 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    41186 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    53545 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3643 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11655 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3818 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5579 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3064 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4459 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/pkg_resources/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      538 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   107452 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/colorama/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1491 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/colorama/LICENSE.txt
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/nuitka/build/inline_copy/colorama/colorama/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5404 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/colorama/colorama/win32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2522 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/colorama/colorama/ansi.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      243 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/colorama/colorama/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10517 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1915 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/colorama/colorama/initialise.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6438 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/inline_copy/colorama/colorama/winterm.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15532 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/SconsInterface.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2346 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/SconsProgress.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    24258 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/build/SconsUtils.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4086 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/PythonOperators.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    36691 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/MainControl.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5506 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/__main__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/plugins/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/plugins/standard/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9939 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/DataFilesPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5553 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/UpxPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1140 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/TorchPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6554 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/OptionsNannyPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3460 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5027 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/GlfwPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5675 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/DillPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4051 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/DelvewheelPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18092 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/AntiBloatPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2933 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/PywebViewPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1917 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/PbrPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1880 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/GeventPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12180 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/TkinterPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6992 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/PmwPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   124572 2023-04-12 06:00:15.000000 Nuitka-1.5.6/nuitka/plugins/standard/standard.nuitka-package.config.yml
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18758 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/ImplicitImports.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1160 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/TensorflowPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4665 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/PkgResourcesPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3482 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/GiPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2221 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6750 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/MultiprocessingPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3175 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/TrioPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1905 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/EventletPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4948 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/KivyPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7258 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/MatplotlibPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2062 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/EnumPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    49325 2023-04-12 06:00:15.000000 Nuitka-1.5.6/nuitka/plugins/standard/PySidePyQtPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12182 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/DllFilesPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1187 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/NumpyPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8831 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    52710 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/Plugins.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    39068 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/plugins/PluginBase.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3440 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/Bytecodes.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/distutils/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/distutils/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12729 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/distutils/DistutilCommands.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1964 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/distutils/Build.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1884 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/CacheCleanup.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/optimizations/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2272 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/optimizations/Tags.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4038 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/optimizations/FunctionInlining.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2144 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/optimizations/Graphs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/optimizations/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10762 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/optimizations/Optimization.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3279 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/optimizations/BytecodeDemotion.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    52154 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/optimizations/OptimizeBuiltinCalls.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    40896 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/optimizations/TraceCollections.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    23977 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/optimizations/ValueTraces.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    52861 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/OptionParsing.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/importing/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4739 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/importing/PreloadedPackages.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/importing/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10934 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/importing/IgnoreListing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    27820 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/importing/Importing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16375 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/importing/Recursion.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10383 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/importing/StandardLibrary.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6455 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/importing/ImportResolving.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2899 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/importing/ImportCache.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/freezer/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7311 2023-04-12 06:00:15.000000 Nuitka-1.5.6/nuitka/freezer/DependsExe.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    25217 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/freezer/Standalone.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/freezer/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8830 2023-04-12 06:00:15.000000 Nuitka-1.5.6/nuitka/freezer/Onefile.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2380 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/freezer/DllDependenciesCommon.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9146 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/freezer/IncludedEntryPoints.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7211 2023-04-12 06:00:15.000000 Nuitka-1.5.6/nuitka/freezer/DllDependenciesPosix.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10109 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/freezer/DllDependenciesMacOS.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6620 2023-04-12 06:00:15.000000 Nuitka-1.5.6/nuitka/freezer/DllDependenciesWin32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16587 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/freezer/IncludedDataFiles.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/constants/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8524 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/constants/Serialization.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/constants/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/finalizations/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/finalizations/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1224 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/finalizations/Finalization.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6110 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/finalizations/FinalizeMarkups.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4670 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/SourceCodeReferences.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15235 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/Variables.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5022 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/OutputDirectories.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/utils/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4336 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/Jinja2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2224 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/InstanceCounters.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1216 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/Json.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4288 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/ReExecute.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2855 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/Distributions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3248 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/CStrings.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    30973 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/FileOperations.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6207 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/StaticLibraries.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10574 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/WindowsFileUsage.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2362 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/Images.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19540 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/WindowsResources.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5794 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/Download.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10880 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/Utils.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2772 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/Timing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3664 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/Shebang.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5040 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/MemoryUsage.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2602 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/ThreadedExecutor.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3815 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/Rest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21979 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/SharedLibraries.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12216 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/Execution.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6665 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/Importing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5979 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/Yaml.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4173 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/MacOSApp.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2542 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/AppDirs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3653 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/CommandLineOptions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9057 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/ModuleNames.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2507 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/Signing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2885 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/Hashing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7923 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/utils/InstalledPythons.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7472 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/PythonFlavors.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11235 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/Tracing.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/pgo/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/pgo/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4663 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/pgo/PGO.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tree/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14876 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationExecStatements.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15208 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationClasses.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2948 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationBooleanExpressions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2807 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationAssertStatements.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3088 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationYieldExpressions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    20962 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationMatchStatements.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7782 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationForLoopStatements.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14615 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationTryExceptStatements.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8194 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationNamespacePackages.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15371 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationSequenceCreation.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6430 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationComparisonExpressions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1700 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/Extractions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6577 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationLambdaExpressions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1511 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/Operations.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11693 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationCallExpressions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    75578 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ComplexCallHelperFunctions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    46475 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/Building.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11160 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationDictionaryCreation.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    22973 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/TreeHelpers.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26211 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationFunctionStatements.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4658 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationPrintStatements.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13437 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationImportStatements.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14341 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationWithStatements.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    22111 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationContractionExpressions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    30125 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationClasses3.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3757 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/SyntaxErrors.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    20012 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/VariableClosure.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5674 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationWhileLoopStatements.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6982 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationTryFinallyStatements.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4824 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationSubscriptExpressions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9285 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/SourceHandling.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2409 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationMultidist.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    42974 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/ReformulationAssignmentStatements.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2572 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tree/InternalModule.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/specs/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1159 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/specs/BuiltinTypeOperationSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5133 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/specs/HardImportSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/specs/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5911 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/specs/BuiltinBytesOperationSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6065 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/specs/BuiltinStrOperationSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18781 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/specs/ParameterSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4802 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/specs/BuiltinUnicodeOperationSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2786 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/specs/BuiltinDictOperationSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2541 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/specs/BuiltinListOperationSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26455 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/specs/BuiltinParameterSpecs.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/nodes/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/nodes/shapes/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/shapes/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4567 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/shapes/ShapeMixins.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    42374 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/shapes/StandardShapes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4387 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/shapes/ControlFlowDescriptions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   156168 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/shapes/BuiltinTypeShapes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12723 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinIteratorNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18589 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinRangeNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2496 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinComplexNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14922 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/LocalsScopes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    30982 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/VariableRefNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15581 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/LoopNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    39522 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/VariableAssignNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    44996 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ExpressionBases.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6585 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/CodeObjectSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4694 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinDictNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1996 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinLenNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10746 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/VariableDelNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4464 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/PackageResourceNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15128 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/NodeMakingHelpers.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12213 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ContainerMakingNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12501 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/SliceNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26113 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BytesNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9800 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/TypeNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    50665 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/DictionaryNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21683 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ComparisonNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    23094 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/LocalsDictNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4098 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinAnyNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4309 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/SideEffectNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2405 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/TypeMatchNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    74177 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/HardImportNodesGenerated.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1502 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/InjectCNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6478 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/CallNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    34414 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ModuleNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3823 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinAllNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4574 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/VariableNameNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3240 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinOpenNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12442 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/OutlineNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   605501 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ChildrenHavingMixins.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9430 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/StatementNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2834 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ContainerOperationNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6256 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/GeneratorNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4550 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/VariableReleaseNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3902 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/YieldNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3544 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/FunctionAttributeNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2733 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/IndicatorMixins.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4581 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/CoroutineNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5376 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/FutureSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4948 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinFormatNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1698 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinDecodingNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3307 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinSumNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   378745 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/AttributeNodesGenerated.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    45573 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ImportNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3504 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/StringConcatenationNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11228 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/IterationHandles.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6850 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/GlobalsLocalsNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9067 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinRefNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5618 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/NodeMetaClasses.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17853 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/TryNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4082 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/AttributeLookupNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2142 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinHashNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    94880 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/StatementBasesGenerated.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3637 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/AsyncgenNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    46286 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ConstantRefNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7856 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ExceptionNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    24899 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/NodeBases.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11002 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/KeyValuePairNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21278 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ExpressionShapeMixins.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1712 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/MatchNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6772 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ReturnNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1550 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/Checkers.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6534 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ModuleAttributeNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    28658 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/StrNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8448 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ClassNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2727 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinDecoratorNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    39726 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/FunctionNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    30314 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ConditionalNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3407 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/PrintNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8044 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ExecEvalNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3606 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinNextNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16320 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ListOperationNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   245536 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9134 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/OperatorNodesUnary.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8640 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/SubscriptNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12004 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/AttributeNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    31894 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/OperatorNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4202 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/OsSysNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13543 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinTypeNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    31342 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/PackageMetadataNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5491 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ImportHardNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12156 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/FrameNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1714 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/CtypesNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1573 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinVarsNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5334 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/BuiltinIntegerNodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    41307 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/nodes/ExpressionBasesGenerated.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    61976 2023-04-12 06:00:15.000000 Nuitka-1.5.6/nuitka/Options.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14550 2023-04-12 06:00:15.000000 Nuitka-1.5.6/nuitka/PostProcessing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5143 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/__past__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2055 2023-04-12 06:00:15.000000 Nuitka-1.5.6/nuitka/Version.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2447 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/Errors.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3395 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/TreeXML.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4919 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/BytecodeCaching.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11148 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/Constants.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/containers/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      554 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/containers/OrderedSets.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4397 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/containers/OrderedSetsFallback.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/containers/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1435 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/containers/Namedtuples.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6553 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/containers/OrderedDicts.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/reports/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/reports/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15558 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/reports/Reports.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2209 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/reports/LicenseReport.rst.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12083 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/PythonVersions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8064 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/ModuleRegistry.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5770 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/Progress.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/code_generation/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8416 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/CoroutineCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6291 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/ModuleCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2375 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/CodeHelperSelection.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1033 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/InjectCCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1597 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/MatchCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4879 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/CodeObjectCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9809 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/StringCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13095 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/RaisingCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6375 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/LoaderCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4446 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/ComparisonHelperDefinitions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    51024 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/CodeGeneration.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8118 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/Namify.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2612 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/LineNumberCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6911 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/GlobalsLocalsCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1396 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/Indentation.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8099 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/YieldCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14717 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/VariableCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12010 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/IteratorCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    28478 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/DictCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8188 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/SubscriptCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8975 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/ExceptionCodes.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/code_generation/templates/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5747 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesConstants.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6640 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesVariables.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2475 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates/TemplateDebugWrapper.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6339 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesFrames.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3190 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21441 2023-04-12 06:00:15.000000 Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesModules.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2290 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesExceptions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2728 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2805 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2335 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesIterators.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3321 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesFunction.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4217 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesLoader.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1574 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/CtypesCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5879 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/ConstantCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17725 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/FrameCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5721 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/GlobalConstants.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14392 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/CodeHelpers.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15892 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/ListCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2125 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/Emission.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3432 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/IntegerCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4896 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/ClassCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5234 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/ReturnCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9325 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/ErrorCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12304 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/EvalCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1794 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/IdCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12777 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/OperationCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2093 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/ExpressionCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    27345 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/FunctionCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6346 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/AsyncgenCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10153 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/AttributeCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7335 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/ConditionalCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3443 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/Reports.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21864 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/BinaryOperationHelperDefinitions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9121 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/VariableDeclarations.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7350 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    35905 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/CallCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    28479 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/PackageResourceCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13294 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/ImportCodes.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11231 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2557 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1544 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3933 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4292 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2843 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7197 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4288 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12850 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3860 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7407 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15380 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4487 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2984 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19317 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1905 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5904 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3635 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10421 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2979 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2817 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2762 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperLongTools.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2088 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11579 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2044 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperImportHard.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3020 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    23262 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1843 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2118 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11102 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3173 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5238 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12818 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13949 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/SliceCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11176 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/TryCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2339 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/BranchCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3135 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/LoopCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7622 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/GeneratorCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3786 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/TupleCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9951 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/LocalsDictCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5474 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/PythonAPICodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1506 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/IndexCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2022 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/LabelCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16009 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/BuiltinCodes.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/code_generation/c_types/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5128 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1378 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeCLongs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1804 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeCFloats.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/c_types/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19628 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/c_types/CTypePyObjectPointers.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3610 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6069 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeBases.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4017 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5211 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeNuitkaInts.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3399 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeBooleans.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2852 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeVoids.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6517 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/SetCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    31196 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/Contexts.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16827 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/ComparisonCodes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3021 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/code_generation/PrintCodes.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/commercial/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      815 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/commercial/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/general/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/general/find_module/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1238 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/general/find_module/__main__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/general/find_module/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/general/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/general/dll_report/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2366 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/general/dll_report/__main__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/general/dll_report/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/onefile_compressor/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1311 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/onefile_compressor/__main__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/onefile_compressor/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8869 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/onefile_compressor/OnefileCompressor.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1603 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/Basics.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/testing/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3375 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/Valgrind.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/testing/measure_construct_performance/
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8755 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/measure_construct_performance/__main__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/measure_construct_performance/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5371 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/SearchModes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7888 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/RuntimeTracing.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/testing/find_sxs_modules/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1949 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/find_sxs_modules/__main__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/find_sxs_modules/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/testing/check_reference_counts/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3064 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/check_reference_counts/__main__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/check_reference_counts/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    55189 2023-04-12 06:00:15.000000 Nuitka-1.5.6/nuitka/tools/testing/Common.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1483 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/Constructs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1278 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/Pythons.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/testing/compare_with_cpython/
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    29429 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/compare_with_cpython/__main__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/compare_with_cpython/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8940 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/OutputComparison.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/testing/run_nuitka_tests/
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    36321 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/run_nuitka_tests/__main__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/testing/run_nuitka_tests/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/data_composer/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1306 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/data_composer/__main__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/data_composer/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14081 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/data_composer/DataComposer.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/environments/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/environments/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2449 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/environments/CreateEnvironment.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3735 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/environments/Virtualenv.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/profiler/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2529 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/profiler/__main__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/profiler/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/scanning/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/scanning/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2369 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/scanning/DisplayPackageDLLs.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2049 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/scanning/DisplayPackageData.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/nuitka/tools/specialize/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    33585 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/specialize/SpecializePython.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/specialize/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7685 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/specialize/Common.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    51143 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/specialize/CTypeDescriptions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    39625 2023-04-12 05:59:07.000000 Nuitka-1.5.6/nuitka/tools/specialize/SpecializeC.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      834 2023-04-12 05:59:07.000000 Nuitka-1.5.6/pyproject.toml
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/misc/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1038 2023-04-12 05:59:07.000000 Nuitka-1.5.6/misc/nuitka.bat
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      901 2023-04-12 05:59:07.000000 Nuitka-1.5.6/misc/nuitka-run.bat
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11348 2023-04-12 05:59:07.000000 Nuitka-1.5.6/LICENSE.txt
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/lib/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4250 2023-04-12 05:59:07.000000 Nuitka-1.5.6/lib/hints.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/plugins/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/plugins/parameters/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2168 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/plugins/parameters/parameter-using-plugin.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1019 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/plugins/parameters/ParametersMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/plugins/data_files/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1332 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/plugins/data_files/DataFilesMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/plugins/data_files/data_files_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/plugins/data_files/data_files_package/lala.txt
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      924 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/plugins/data_files/data_files_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/plugins/data_files/data_files_package/sub_dir/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      255 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/plugins/data_files/test_case.nuitka-package.config.yml
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3532 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/plugins/run_all.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/optimizations/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      921 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/optimizations/Conditions.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1333 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/optimizations/Subscripts.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1212 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/optimizations/FormatStrings36.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      918 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/optimizations/Iterations.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      958 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/optimizations/ArgumentTypes.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2262 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/optimizations/Operations.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1150 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/optimizations/HardImports.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1260 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/optimizations/Len.py
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8736 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/optimizations/run_all.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1021 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/optimizations/Calls.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      909 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/optimizations/DecodingOperations.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      974 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/optimizations/HardImports_2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1055 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/optimizations/Attributes.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/standalone/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2554 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/CtypesUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1757 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/PySide6Using.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1184 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/GtkUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1431 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/MatplotlibUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3228 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/Urllib3Using.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1136 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/FlaskUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1379 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/PandasUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1151 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/LxmlUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2074 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/PkgResourcesRequiresUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1067 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/PmwUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1086 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/IdnaUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1727 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/NumpyUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      990 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/GlfwUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      973 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/ShlibUsing.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/standalone/zip_importer/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1264 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/zip_importer/ZipImporterMain.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1085 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/PyQt5Plugins.py
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9531 2023-04-12 06:00:15.000000 Nuitka-1.5.6/tests/standalone/run_all.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1105 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/PyQt5SSLSupport.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1025 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/HexEncodingTest_2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1066 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/PasslibUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2538 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/MetadataPackagesUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1504 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/SocketUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1323 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/RsaUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1200 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/Win32ComUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1151 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/PendulumUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1058 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/BrotliUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1941 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/TkInterUsing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2050 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/PyQt6Using.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2050 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/PyQt5Using.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      947 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/standalone/OpenGLUsing.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/basics/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1628 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/DecoratorsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1899 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ParameterErrorsTest32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      890 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/FutureTest32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5934 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/AssignmentsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2305 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/TryExceptFramesTest.py
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2271 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/run_xml.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1988 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/OperatorsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3824 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/GlobalStatementTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1104 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/BuiltinOverload.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      995 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ConstantsTest27.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2899 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ReferencingTest_2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4764 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ClassesTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2923 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ListContractionsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1159 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ThreadedGeneratorsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2095 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/VarargsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14391 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ExceptionRaisingTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2842 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/TryReturnFinallyTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5853 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ParameterErrorsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2469 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ImportingTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      878 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/RecursionTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2212 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/TryExceptContinueTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2317 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/DefaultParametersTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1458 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ExceptionRaisingTest33.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1618 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/InspectionTest_36.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3603 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/FunctionsTest32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4698 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ComparisonChainsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3749 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/BuiltinSuperTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1286 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/HelloWorldTest_2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2275 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/TryExceptFinallyTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1630 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/SlotsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4879 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/WithStatementsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4227 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/InspectionTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2086 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/TryContinueFinallyTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1417 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ExtremeClosureTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      863 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/PrintFutureTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1877 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/UnpackingTest35.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4639 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ConstantsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1041 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/GeneratorExpressionsTest_37.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12335 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/FunctionsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2328 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/TryYieldFinallyTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1406 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ClassesTest34.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1093 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/UnicodeTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1827 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/OrderChecksTest27.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3072 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/YieldFromTest33.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14903 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/OrderChecksTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1127 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/DoubleDeletionsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5809 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/GeneratorExpressionsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5866 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/AssignmentsTest32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1504 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/InspectionTest_35.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      866 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ClassMinimalTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1925 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ModuleAttributesTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1766 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/AssertsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1413 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/PrintingTest_2.py
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3821 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/run_all.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1788 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/TrickAssignmentsTest_2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7819 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ReferencingTest33.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    22965 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/TrickAssignmentsTest32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6745 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ExecEvalTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    23840 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ReferencingTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1536 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/MainProgramsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4055 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/BranchingTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2627 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/FunctionsTest_2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5092 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ReferencingTest36.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1658 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/FunctionObjectsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      961 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ExceptionRaisingTest32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1296 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/InplaceOperationsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2731 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/LateClosureAssignmentTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2076 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ReferencingTest27.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3329 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/LoopingTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      806 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/EmptyModuleTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17079 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/BuiltinsTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3414 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ClassesTest32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1541 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/TrickAssignmentsTest35.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4902 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/ReferencingTest35.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1452 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/OverflowFunctionsTest_2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1671 2023-04-12 05:59:07.000000 Nuitka-1.5.6/tests/basics/LambdasTest.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/onefile/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1307 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/onefile/KeyboardInterruptTest.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      993 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/onefile/HelloWorldTest.py
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5816 2023-04-12 06:00:15.000000 Nuitka-1.5.6/tests/onefile/run_all.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/packages/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/packages/package_import_success_after_failure/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2382 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/packages/package_import_success_after_failure/variable_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1168 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/packages/package_import_success_after_failure/variable_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      942 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/tests/packages/sub_package/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/packages/sub_package/kitty/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1230 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/packages/sub_package/kitty/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/packages/sub_package/kitty/speak/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      966 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/packages/sub_package/kitty/speak/miau.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      929 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/packages/sub_package/kitty/speak/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1053 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/packages/sub_package/kitty/speak/hello.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      968 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/packages/sub_package/kitty/speak/purr.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      910 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/packages/sub_package/kitty/smallkitty.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      908 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/packages/sub_package/kitty/bigkitty.py
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3671 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/packages/run_all.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/tests/packages/top_level_attributes_3/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/packages/top_level_attributes_3/some_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2336 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/packages/top_level_attributes_3/some_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      907 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/packages/top_level_attributes_3/some_package/some_module.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/reflected/
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14085 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/reflected/compile_itself.py
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1243 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/run-tests
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_contains_main/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_contains_main/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      801 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_contains_main/local.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      789 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_contains_main/PackageContainsMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_prevents_submodule/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2972 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_prevents_submodule/some_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1078 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_prevents_submodule/some_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      800 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_prevents_submodule/some_package/some_module.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/case_imports3/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/case_imports3/path2/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/case_imports3/path2/Some_Package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      810 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/case_imports3/path2/Some_Package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      809 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/case_imports3/path2/Some_Module.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1075 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/case_imports3/CasedImportingMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/case_imports3/path1/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/case_imports3/path1/Some_Package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      810 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/case_imports3/path1/Some_Package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      809 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/case_imports3/path1/Some_Module.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_init_import/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      823 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_init_import/PackageInitImportMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_init_import/some_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1169 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_init_import/some_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1008 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_init_import/some_package/PackageLocal.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_missing_init/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      926 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_missing_init/PackageMissingInitMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_missing_init/some_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      965 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_missing_init/some_package/some_module.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_missing_init/some_package/sub_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      977 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/dash_main/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      809 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/dash_main/Dash-Main.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/main_raises2/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1080 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/main_raises2/ErrorInFunctionMain.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      808 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/main_raises2/ErrorRaising.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/resource_reader37/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1169 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/resource_reader37/ResourceReaderMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/resource_reader37/some_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       13 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/resource_reader37/some_package/DATA_FILE.txt
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/resource_reader37/some_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/import_variants/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1005 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/import_variants/ImportVariationsMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/import_variants/some_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      994 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/import_variants/some_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      946 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/import_variants/some_package/Child1.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1098 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/import_variants/some_package/Child2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      822 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/import_variants/some_package/Child3.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/deep/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      898 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/deep/DeepProgramMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/deep/some_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      980 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/deep/some_package/DeepBrother.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/deep/some_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      909 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/deep/some_package/DeepChild.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/deep/some_package/deep_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      952 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/deep/some_package/deep_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      876 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/case_imports2/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/case_imports2/path2/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/case_imports2/path2/Some_Package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      799 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/case_imports2/path2/Some_Package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      798 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/case_imports2/path2/Some_Module.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      808 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/case_imports2/CasedImportingMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/case_imports2/path1/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/case_imports2/path1/some_module.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/case_imports2/path1/some_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/case_imports2/path1/some_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/pkgutil_itermodules/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1728 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/multiprocessing_using/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      990 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/multiprocessing_using/foo/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      836 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/multiprocessing_using/foo/__main__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/multiprocessing_using/foo/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1758 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/multiprocessing_using/foo/entry.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_code/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      800 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_code/PackageInitCodeMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_code/some_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      809 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_code/some_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      810 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_code/some_package/SomeModule.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:50.000000 Nuitka-1.5.6/tests/programs/package_program/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_program/PackageAsMain/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1630 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_program/PackageAsMain/__main__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      888 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_program/PackageAsMain/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/relative_import/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/relative_import/dircache.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      842 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/relative_import/RelativeImportMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/module_object_replacing/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1078 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1359 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/module_object_replacing/SelfReplacingModule.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/stdlib_overload/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1171 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/stdlib_overload/StdlibOverloadMain.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      799 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/stdlib_overload/pyexpat.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/stdlib_overload/some_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      810 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/stdlib_overload/some_package/pyexpat.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/stdlib_overload/some_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1236 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/stdlib_overload/some_package/star_importing.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      909 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/stdlib_overload/some_package/normal_importing.py
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6615 2023-04-12 06:00:15.000000 Nuitka-1.5.6/tests/programs/run_all.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/plugin_import/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      859 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/plugin_import/PluginImportMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/plugin_import/some_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      771 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/plugin_import/some_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      781 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/plugin_import/some_package/some_module.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/main_raises/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      808 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/main_raises/ErrorRaising.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      911 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/main_raises/ErrorMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/absolute_import/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      867 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/absolute_import/AbsoluteImportMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/absolute_import/foobar/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      796 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/absolute_import/foobar/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1043 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/absolute_import/foobar/foobar.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      860 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/absolute_import/foobar/util.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      879 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/absolute_import/foobar/local.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/syntax_errors/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1079 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/syntax_errors/SyntaxErrorsMain.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      800 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/syntax_errors/SyntaxErroring.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      791 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/syntax_errors/IndentationErroring.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/unicode_bom/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      963 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/unicode_bom/UnicodeBomMain.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      846 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/unicode_bom/unicode_bom.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/named_imports/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      846 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/named_imports/NamedImportsMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/named_imports/some_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      824 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/named_imports/some_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/named_imports/some_package/SomeModule.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/named_imports/some_package/sub_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/named_imports/some_package/sub_package/SomeModule.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/with space/
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      826 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/with space/Space Main.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/dash_import/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      888 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/dash_import/DashImportMain.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      817 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/dash_import/dash-module.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      817 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/dash_import/plus+module.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/reimport_main_static/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      898 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/reimport_main_static/ImportItselfStaticMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/pkgutil_usage/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1261 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/pkgutil_usage/package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       13 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/pkgutil_usage/package/DATA_FILE.txt
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1553 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/pkgutil_usage/package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       14 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       14 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/module_exits/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      869 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/module_exits/ErrorExitingModule.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      867 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/module_exits/Main.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/module_attributes/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1529 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/module_attributes/ModuleAttributesMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/module_attributes/package_level1/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/module_attributes/package_level1/package_level2/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1611 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/module_attributes/package_level1/package_level2/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1611 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1744 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1744 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1611 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/module_attributes/package_level1/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1744 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/module_attributes/package_level1/Nearby1.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/dunderinit_imports/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/dunderinit_imports/package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      857 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/dunderinit_imports/package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      797 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/dunderinit_imports/package/SubModule.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      794 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/dunderinit_imports/DunderInitImportsMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_overload/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      852 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_overload/Main.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_overload/foo/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      799 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_overload/foo/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_overload/foo/bar.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_overload/foo/bar2.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/reimport_main_dynamic/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      911 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_module_collision/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      801 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_module_collision/something.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_module_collision/Something/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      810 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_module_collision/Something/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      901 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_init_issue/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      789 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_init_issue/PackageInitIssueMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_init_issue/some_package/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/package_init_issue/some_package/child_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      795 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_init_issue/some_package/child_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      798 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      798 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/package_init_issue/some_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/case_imports1/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/case_imports1/path2/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      798 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/case_imports1/path2/some_module.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/case_imports1/path2/some_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      799 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/case_imports1/path2/some_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      808 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/case_imports1/CasedImportingMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/case_imports1/path1/
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/case_imports1/path1/Some_Package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      799 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/case_imports1/path1/Some_Package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      798 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/case_imports1/path1/Some_Module.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/cyclic_imports/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      801 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/cyclic_imports/CyclicImportsMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/programs/cyclic_imports/cyclic_importing_package/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      842 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      875 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      875 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
-drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-12 06:01:51.000000 Nuitka-1.5.6/tests/syntax/
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      874 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/TryExceptAllNotLast.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      869 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/SyntaxError.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      800 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/ModuleReturn.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      792 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/GlobalForParameter.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      841 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/MisplacedFutureImport.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      793 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/YieldFromInModule.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      791 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/DuplicateArgument.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      868 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/NonlocalNotFound32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      908 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/StarImportExtra.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      915 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/LateFutureImport.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      781 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/YieldInModule.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      799 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/IndentationError.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      811 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/AsyncgenReturn36.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      804 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/YieldInAsync35.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      883 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/NonAsciiWithoutEncoding_2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      849 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/ContinueWithoutLoop.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1041 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/GeneratorExpressions38.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      826 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/FutureBraces.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      995 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/Importing32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      868 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/BreakWithoutLoop.py
--rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2203 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/run_all.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      805 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/FutureUnknown.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1111 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/ExecWithNesting_2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      923 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/YieldInGenexp38.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      809 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/UnpackTwoStars32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      970 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/ClosureDel_2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      879 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/GeneratorReturn_2.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      776 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/UnpackNoTuple.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      794 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/NonlocalForParameter32.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      791 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/ClassReturn.py
--rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      875 2023-04-12 05:59:08.000000 Nuitka-1.5.6/tests/syntax/TryFinallyContinue_37.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    91155 2023-04-25 08:09:05.000000 Nuitka-1.5.7/PKG-INFO
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15284 2023-04-25 06:15:40.000000 Nuitka-1.5.7/setup.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/bin/
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1163 2023-04-25 06:15:40.000000 Nuitka-1.5.7/bin/measure-construct-performance
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1136 2023-04-25 06:15:40.000000 Nuitka-1.5.7/bin/check-nuitka-with-pylint
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1685 2023-04-25 06:15:40.000000 Nuitka-1.5.7/bin/nuitka-run
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1135 2023-04-25 06:15:40.000000 Nuitka-1.5.7/bin/autoformat-nuitka-source
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1150 2023-04-25 06:15:40.000000 Nuitka-1.5.7/bin/compare_with_cpython
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3079 2023-04-25 06:15:40.000000 Nuitka-1.5.7/bin/compare_with_xml
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1685 2023-04-25 06:15:40.000000 Nuitka-1.5.7/bin/nuitka
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   336039 2023-04-25 08:08:00.000000 Nuitka-1.5.7/README.pdf
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/doc/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/doc/Logo/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17917 2023-04-25 06:15:40.000000 Nuitka-1.5.7/doc/Logo/Nuitka-Logo-Vertical.svg
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7401 2023-04-25 06:15:40.000000 Nuitka-1.5.7/doc/Logo/Nuitka-Logo-Symbol.svg
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7321 2023-04-25 06:15:40.000000 Nuitka-1.5.7/doc/Logo/Nuitka-Logo-Horizontal.svg
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/doc/images/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7585 2023-04-25 06:15:40.000000 Nuitka-1.5.7/doc/images/Nuitka-Logo-Horizontal.png
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9828 2023-04-25 06:15:40.000000 Nuitka-1.5.7/doc/images/Nuitka-Logo-Vertical.png
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4452 2023-04-25 06:15:40.000000 Nuitka-1.5.7/doc/images/Nuitka-Logo-Symbol.png
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    29731 2023-04-25 08:09:02.000000 Nuitka-1.5.7/doc/nuitka3-run.1
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    29739 2023-04-25 08:08:57.000000 Nuitka-1.5.7/doc/nuitka2.1
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    29715 2023-04-25 08:08:57.000000 Nuitka-1.5.7/doc/nuitka2-run.1
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    29755 2023-04-25 08:09:02.000000 Nuitka-1.5.7/doc/nuitka3.1
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   801878 2023-04-25 06:15:40.000000 Nuitka-1.5.7/Changelog.rst
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       38 2023-04-25 08:09:05.000000 Nuitka-1.5.7/setup.cfg
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   809671 2023-04-25 08:08:13.000000 Nuitka-1.5.7/Developer_Manual.pdf
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    73222 2023-04-25 06:15:40.000000 Nuitka-1.5.7/README.rst
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   152121 2023-04-25 06:15:40.000000 Nuitka-1.5.7/Developer_Manual.rst
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/Nuitka.egg-info/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    91155 2023-04-25 08:09:04.000000 Nuitka-1.5.7/Nuitka.egg-info/PKG-INFO
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        7 2023-04-25 08:09:04.000000 Nuitka-1.5.7/Nuitka.egg-info/top_level.txt
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    76486 2023-04-25 08:09:04.000000 Nuitka-1.5.7/Nuitka.egg-info/SOURCES.txt
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        1 2023-04-25 08:09:04.000000 Nuitka-1.5.7/Nuitka.egg-info/dependency_links.txt
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      394 2023-04-25 08:09:04.000000 Nuitka-1.5.7/Nuitka.egg-info/entry_points.txt
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        1 2023-04-25 08:09:04.000000 Nuitka-1.5.7/Nuitka.egg-info/not-zip-safe
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)  2697334 2023-04-25 08:08:52.000000 Nuitka-1.5.7/Changelog.pdf
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1741 2023-04-25 06:15:40.000000 Nuitka-1.5.7/MANIFEST.in
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7236 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/Builtins.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2433 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/DataComposerInterface.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/static_src/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    47568 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceLshift.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13776 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13057 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersCalling.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   314618 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersComparisonNe.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3805 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersPythonPgo.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    67487 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    77782 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryBitor.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4037 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersTuples.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   315628 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersComparisonLt.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    68748 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    76343 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11945 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/InspectPatcher.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    38320 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersDictionaries.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   136100 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceMod.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18993 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersAllocator.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3033 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersBytes.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26221 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   181243 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryAdd.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17065 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21493 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/CompiledMethodType.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21783 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersBuiltin.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7035 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersExceptions.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    36011 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersConstantsBlob.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    74142 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    60657 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/CompiledGeneratorType.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    82114 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/CompiledAsyncgenType.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    53224 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceBitand.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   107641 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3650 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   313003 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersComparisonGe.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3730 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersSequences.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    53224 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11094 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersSafeStrings.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17742 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    57572 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/CompiledCodeHelpers.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    58321 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/MetaPathBasedLoader.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    66453 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    83405 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryLshift.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6411 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersFiles.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26642 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersStrings.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   183202 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryMod.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    35865 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/CompiledFrameType.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    24294 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersDictionariesGenerated.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   188514 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryMult.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4673 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersComparisonEqUtils.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2991 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersClasses.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   149580 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceAdd.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3513 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersMatching.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13589 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersImportHard.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    45052 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceRshift.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2426 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersFloats.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    30729 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/OnefileBootstrap.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6274 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    53122 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceBitor.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    93999 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/CompiledFunctionType.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6427 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    76512 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8250 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/CompiledCellType.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16700 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    82842 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceSub.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11199 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersFilesystemPaths.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   316217 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersComparisonLe.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13915 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersListsGenerated.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   460993 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersCallingGenerated.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14561 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersImport.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5578 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersTypes.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    40884 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/MainProgram.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1774 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersHeapStorage.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    78891 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryPow.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   312414 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersComparisonGt.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1236 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    77943 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryBitand.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1640 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersMappings.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4071 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    82669 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplacePow.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    70465 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinarySub.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    77305 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryRshift.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7891 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/OnefileSplashScreen.cpp
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    68005 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1946 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersSlices.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   317872 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersComparisonEq.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1023 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3219 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersProfiling.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    32656 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersAttributes.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18391 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersLists.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1617 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersChecksumTools.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    70973 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/CompiledCoroutineType.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   142211 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceMult.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15369 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersRaising.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3404 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19313 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersDeepcopy.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    77943 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/include/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3144 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/tracing.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14375 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helpers.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1261 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/checksum_tools.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16949 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/compiled_frame.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9136 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/compiled_generator.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12979 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/incbin.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/allocator.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2002 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/compiled_cell.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1977 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/checkers.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6253 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/freelists.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5972 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/compiled_function.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2830 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/unfreezing.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3840 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/threading.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    33190 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/exceptions.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7408 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/constants.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2119 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/safe_string_ops.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14248 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/prelude.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9571 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/compiled_asyncgen.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1293 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/constants_blob.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3221 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/filesystem_paths.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5363 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/importing.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3423 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/builtins.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1838 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/compiled_method.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1761 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/python_pgo.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2870 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/printing.h
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2941 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/ints.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10616 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/comparisons_ge.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1112 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/sequences.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12685 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_add.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1798 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/indexes.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13140 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/comparisons_le.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5438 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9201 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5422 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10626 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15100 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_builtin_types.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1181 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/bytearrays.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5147 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5824 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_sub.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5791 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8419 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/slices.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1633 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/lists_generated.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4846 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5115 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3397 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/lists.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5641 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10616 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/comparisons_ne.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8670 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_add.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3011 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1206 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/floats.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2663 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/boolean.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4573 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9992 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/iterators.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1242 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/strings.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1025 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/sets.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3767 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3753 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3297 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/raising.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1146 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/richcomparisons.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13139 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/comparisons_lt.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4714 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_pow.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4349 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3275 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/attributes.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1328 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/mappings.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15778 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_mod.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13210 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_mult.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13077 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/dictionaries.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2799 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4975 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10615 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/comparisons_gt.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9335 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/calling_generated.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2727 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4826 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5663 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5460 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5115 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13140 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/comparisons_eq.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1135 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/bytes.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5720 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/tuples.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3011 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3674 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/import_hard.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5663 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2178 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/rangeobjects.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1743 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/complex.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17447 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/subscripts.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3767 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9325 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/compiled_coroutine.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    86326 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/hedley.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4460 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/include/nuitka/calling.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18493 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/Onefile.scons
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5527 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/SconsHacks.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11960 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/SconsSpawn.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    33043 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/Backend.scons
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    29044 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/SconsCompilerSettings.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15210 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/SconsCaching.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8314 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/CCompilerVersion.scons
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/clcache/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/clcache/clcache/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1585 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/clcache/clcache/LICENSE
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       93 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/clcache/clcache/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    65424 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/clcache/clcache/caching.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/glob2/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/glob2/glob2/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8304 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/glob2/glob2/impl.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       82 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/glob2/glob2/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6859 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/glob2/glob2/compat.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4463 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1359 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/glob2/LICENSE
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1101 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/LICENSE
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14184 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/representer.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4165 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/serializer.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6794 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/reader.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2445 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/events.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2061 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/loader.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13170 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    43006 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/emitter.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    25495 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/parser.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1440 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/nodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2573 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/tokens.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    51277 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/scanner.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8999 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/resolver.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    28639 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/constructor.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4883 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/composer.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2533 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/error.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3851 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/cyaml.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2837 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/dumper.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/appdirs/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    24824 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/appdirs/appdirs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1097 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/appdirs/LICENSE.txt
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17474 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    50849 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2616 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    24500 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    20501 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    35875 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    30853 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    36528 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4340 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    28559 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9197 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2685 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1400 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17080 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7308 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12281 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1722 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4214 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3316 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    65386 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    27644 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12719 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1726 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1626 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4428 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       84 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/README.rst
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1466 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17473 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    50849 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/environment.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2423 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    24500 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/ext.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    20501 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/utils.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    35875 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/parser.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    30853 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    36528 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/filters.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4340 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/meta.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    28559 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9197 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2685 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1400 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17080 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7308 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12281 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/debug.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1722 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4214 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/tests.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3316 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    65386 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    27644 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12719 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1726 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1626 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/constants.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4428 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       85 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/README.rst
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1467 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/LICENSE.rst
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/bin/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1331 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/bin/scons.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1101 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/LICENSE
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14097 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/representer.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4165 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6854 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/reader.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2445 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/events.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1138 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/loader.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9607 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    42954 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    25495 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/parser.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1440 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2573 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    51695 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8970 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    25554 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4881 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/composer.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2533 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/error.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3294 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2723 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1101 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/LICENSE
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17711 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/representer.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4171 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6746 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/reader.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2445 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/events.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1132 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/loader.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9776 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    43298 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    25542 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/parser.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1440 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2573 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    52446 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9122 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    25145 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4921 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/composer.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2559 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/error.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3290 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2719 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/atomicwrites/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1069 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/atomicwrites/LICENSE
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6794 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   138334 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/zstd.h
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13662 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/entropy_common.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    20216 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/huf.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15880 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/zstd_internal.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3009 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/error_private.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3763 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/debug.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18198 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/bitstream.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2728 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/zstd_common.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    34422 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/fse.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26976 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/xxhash.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3828 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/zstd_errors.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2497 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/zstd_deps.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2441 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/error_private.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11706 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/xxhash.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4455 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/cpu.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14748 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/fse_decompress.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13930 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/mem.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10157 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/compiler.h
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/decompress/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7906 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2253 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    54982 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    66784 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1321 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9164 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    80283 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1530 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/zstd/LICENSE.txt
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      283 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_main.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3687 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      307 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5943 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/gui.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1591 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      888 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9533 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/utils.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10790 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1376 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/dask.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      287 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_gui.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      857 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      596 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    57572 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/std.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      283 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      333 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/version.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1106 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/auto.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6948 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/tk.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/markupsafe/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1873 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10126 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4690 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      558 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1467 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/markupsafe/LICENSE.rst
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16000 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1950 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2614 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2736 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1965 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1950 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1950 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    40510 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    44500 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2465 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8120 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1742 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1776 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3596 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19253 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1818 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1563 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8467 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7509 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    33996 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8083 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    24133 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14053 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    40719 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14029 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    52665 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    48938 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    49503 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4197 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   121420 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4164 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12950 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1991 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4381 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3730 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2166 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2433 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2256 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2657 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1844 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2333 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3328 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4782 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2945 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2077 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2433 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1902 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1831 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2513 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    72761 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2147 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1804 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2309 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2025 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2168 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2328 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4375 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2639 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    31283 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13881 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5992 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    25816 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2681 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18600 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4224 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3472 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8394 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13016 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2123 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2004 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14869 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2078 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    20832 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19499 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2784 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9248 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2473 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2796 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11380 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2681 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2936 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18084 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2460 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2827 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2290 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2935 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5149 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3428 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1711 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      142 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3579 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3953 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2379 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4695 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2720 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1810 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2618 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2267 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1819 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6841 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1927 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3415 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2349 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3432 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2777 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2502 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4658 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6919 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3763 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2859 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2043 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    29618 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2140 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3785 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14663 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3751 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4810 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2011 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3233 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    34903 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19664 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21540 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7358 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    96183 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2305 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6824 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9589 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    27693 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14948 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1605 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4179 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2483 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3131 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9314 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2170 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1989 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1882 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1718 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17622 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2107 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6938 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    39700 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    47844 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3557 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11034 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3784 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5612 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3007 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4404 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16583 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    41191 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3395 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4307 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1644 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      353 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8183 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9295 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    35213 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15278 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6632 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11061 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26676 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14272 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    42760 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13597 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    53509 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    71693 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    63768 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5126 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   136271 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6167 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14673 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1563 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4577 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3259 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3687 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2122 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1891 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2206 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4879 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2900 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1954 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1851 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1786 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2479 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    84784 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2141 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1752 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2266 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2387 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3296 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4817 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1557 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    32724 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14473 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6412 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    25826 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19180 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4113 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3616 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2588 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12548 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2006 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1943 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15027 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2014 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    22570 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    38783 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2734 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13182 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2429 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7993 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12902 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1544 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1661 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15570 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2437 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2788 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2889 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4368 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3379 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1663 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2377 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3576 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3931 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1578 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1569 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2616 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1772 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2526 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2386 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2677 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2573 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1999 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2228 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1780 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      343 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3534 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6788 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1888 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6064 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4649 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7652 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4076 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2419 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1567 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7461 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2271 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4517 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8622 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1995 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2893 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2096 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3742 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15577 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4357 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7394 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1972 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3546 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    36753 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21614 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21937 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7515 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    97269 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6785 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9430 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    27408 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14831 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1536 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4356 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2630 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3087 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12836 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3860 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2076 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2107 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1805 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1311 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1674 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21423 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2032 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7884 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    41983 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    56578 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3979 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3536 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12708 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3896 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5588 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3134 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4672 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16068 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    42204 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6869 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1784 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1647 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8354 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9002 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    34985 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13596 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26467 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14489 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    39394 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13779 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    53260 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    53803 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    63474 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5239 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   135413 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5758 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13880 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1652 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4956 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3444 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3773 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2211 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1977 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2386 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5335 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2987 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2123 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1944 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1873 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2567 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    82939 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2226 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1847 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2351 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2475 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3389 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4904 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1645 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    50660 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14751 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6756 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26195 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15791 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4808 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3686 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13924 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13982 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2176 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2057 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15165 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2152 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21762 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    33537 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2855 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10674 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2515 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8618 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12588 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1630 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2978 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18207 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2948 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2877 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2977 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4464 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3472 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1753 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2580 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3663 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4041 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1667 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1658 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2840 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1859 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2655 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2475 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2765 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2660 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2088 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2316 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1868 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      313 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3631 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6883 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1976 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3201 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2583 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1653 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8494 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2366 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5235 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7808 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2085 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    29765 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2189 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3827 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15053 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3812 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4853 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2328 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3643 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    35863 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19816 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    22350 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7752 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    96818 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6504 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9565 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    28403 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16962 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1654 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4476 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2739 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3180 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11500 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4003 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2219 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2227 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1931 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1460 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1767 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    20988 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2149 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7533 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    41186 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    53545 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3643 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11655 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3818 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5579 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3064 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4459 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/pkg_resources/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/build/inline_copy/pkg_resources/pkg_resources/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      538 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   107452 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/colorama/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1491 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/colorama/LICENSE.txt
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/nuitka/build/inline_copy/colorama/colorama/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5404 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/colorama/colorama/win32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2522 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/colorama/colorama/ansi.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      243 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/colorama/colorama/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10517 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1915 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/colorama/colorama/initialise.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6438 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/inline_copy/colorama/colorama/winterm.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15532 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/SconsInterface.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2346 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/SconsProgress.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    24258 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/build/SconsUtils.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4061 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/PythonOperators.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    36691 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/MainControl.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5506 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/__main__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/plugins/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/plugins/standard/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9939 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/DataFilesPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5553 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/UpxPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1140 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/TorchPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6554 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/OptionsNannyPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3460 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5027 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/GlfwPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5675 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/DillPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4051 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/DelvewheelPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18092 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/AntiBloatPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2933 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/PywebViewPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1917 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/PbrPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1880 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/GeventPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12180 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/TkinterPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6992 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/PmwPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   127647 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/standard.nuitka-package.config.yml
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18758 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/ImplicitImports.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1160 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/TensorflowPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4665 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/PkgResourcesPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3482 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/GiPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2221 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6750 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/MultiprocessingPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3175 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/TrioPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1905 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/EventletPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4948 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/KivyPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7258 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/MatplotlibPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2062 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/EnumPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    49324 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/PySidePyQtPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12182 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/DllFilesPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1187 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/NumpyPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8831 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    52902 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/Plugins.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    39068 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/plugins/PluginBase.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3440 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/Bytecodes.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/distutils/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/distutils/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14107 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/distutils/DistutilCommands.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1964 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/distutils/Build.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1884 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/CacheCleanup.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/optimizations/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2272 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/optimizations/Tags.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4038 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/optimizations/FunctionInlining.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2144 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/optimizations/Graphs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/optimizations/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10762 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/optimizations/Optimization.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3279 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/optimizations/BytecodeDemotion.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    52154 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/optimizations/OptimizeBuiltinCalls.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    40896 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/optimizations/TraceCollections.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    23977 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/optimizations/ValueTraces.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    52861 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/OptionParsing.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/importing/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4739 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/importing/PreloadedPackages.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/importing/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10934 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/importing/IgnoreListing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    28248 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/importing/Importing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16375 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/importing/Recursion.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10383 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/importing/StandardLibrary.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6455 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/importing/ImportResolving.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2899 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/importing/ImportCache.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/freezer/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7311 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/freezer/DependsExe.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    25368 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/freezer/Standalone.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/freezer/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8830 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/freezer/Onefile.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2380 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/freezer/DllDependenciesCommon.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9146 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/freezer/IncludedEntryPoints.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7211 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/freezer/DllDependenciesPosix.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10109 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/freezer/DllDependenciesMacOS.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6620 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/freezer/DllDependenciesWin32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16587 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/freezer/IncludedDataFiles.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/constants/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8524 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/constants/Serialization.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/constants/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/finalizations/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/finalizations/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1224 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/finalizations/Finalization.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6110 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/finalizations/FinalizeMarkups.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4670 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/SourceCodeReferences.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15235 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/Variables.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5022 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/OutputDirectories.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/utils/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4336 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/Jinja2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2224 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/InstanceCounters.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1216 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/Json.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4246 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/ReExecute.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2855 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/Distributions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3248 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/CStrings.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    30973 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/FileOperations.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6207 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/StaticLibraries.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10574 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/WindowsFileUsage.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2362 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/Images.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19540 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/WindowsResources.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5794 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/Download.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10826 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/Utils.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2772 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/Timing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3664 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/Shebang.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5040 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/MemoryUsage.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2602 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/ThreadedExecutor.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3815 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/Rest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21979 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/SharedLibraries.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12216 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/Execution.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6816 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/Importing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6084 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/Yaml.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4173 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/MacOSApp.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2484 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/AppDirs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3653 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/CommandLineOptions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9057 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/ModuleNames.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2507 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/Signing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2885 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/utils/Hashing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7870 2023-04-25 08:00:29.000000 Nuitka-1.5.7/nuitka/utils/InstalledPythons.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7472 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/PythonFlavors.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11235 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/Tracing.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/pgo/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/pgo/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4663 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/pgo/PGO.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tree/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14876 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationExecStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15208 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationClasses.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2948 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationBooleanExpressions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2807 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationAssertStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3088 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationYieldExpressions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    20962 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationMatchStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7782 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationForLoopStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14615 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationTryExceptStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8194 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationNamespacePackages.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15371 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationSequenceCreation.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6430 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationComparisonExpressions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1700 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/Extractions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6577 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationLambdaExpressions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1511 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/Operations.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11693 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationCallExpressions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    75578 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ComplexCallHelperFunctions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    46475 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/Building.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11160 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationDictionaryCreation.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    22973 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/TreeHelpers.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26211 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationFunctionStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4658 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationPrintStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13437 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationImportStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14341 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationWithStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    22111 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationContractionExpressions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    30125 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationClasses3.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3757 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/SyntaxErrors.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    20012 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/VariableClosure.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5674 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationWhileLoopStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6982 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationTryFinallyStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4824 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationSubscriptExpressions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9285 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/SourceHandling.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2409 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationMultidist.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    42974 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/ReformulationAssignmentStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2572 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tree/InternalModule.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/specs/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1159 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/specs/BuiltinTypeOperationSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5133 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/specs/HardImportSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/specs/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5911 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/specs/BuiltinBytesOperationSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6065 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/specs/BuiltinStrOperationSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18740 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/specs/ParameterSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4802 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/specs/BuiltinUnicodeOperationSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2786 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/specs/BuiltinDictOperationSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2541 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/specs/BuiltinListOperationSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26455 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/specs/BuiltinParameterSpecs.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/nodes/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/nodes/shapes/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/shapes/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4567 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/shapes/ShapeMixins.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    42374 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/shapes/StandardShapes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4387 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/shapes/ControlFlowDescriptions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   156243 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/shapes/BuiltinTypeShapes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12723 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinIteratorNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    18589 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinRangeNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2496 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinComplexNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14922 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/LocalsScopes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    30982 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/VariableRefNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15581 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/LoopNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    39522 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/VariableAssignNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    44996 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ExpressionBases.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6585 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/CodeObjectSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4694 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinDictNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1996 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinLenNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10746 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/VariableDelNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4464 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/PackageResourceNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15128 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/NodeMakingHelpers.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12213 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ContainerMakingNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12501 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/SliceNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    26113 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BytesNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9800 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/TypeNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    51021 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/DictionaryNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21683 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ComparisonNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    23094 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/LocalsDictNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4098 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinAnyNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4309 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/SideEffectNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2405 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/TypeMatchNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    74177 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/HardImportNodesGenerated.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1502 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/InjectCNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6478 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/CallNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    34377 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ModuleNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3823 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinAllNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4574 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/VariableNameNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3240 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinOpenNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12442 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/OutlineNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   605501 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ChildrenHavingMixins.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9430 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/StatementNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2834 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ContainerOperationNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6256 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/GeneratorNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4550 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/VariableReleaseNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3902 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/YieldNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3544 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/FunctionAttributeNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2733 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/IndicatorMixins.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4581 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/CoroutineNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5376 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/FutureSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4948 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinFormatNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1698 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinDecodingNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3307 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinSumNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   378745 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/AttributeNodesGenerated.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    45573 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ImportNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3504 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/StringConcatenationNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11228 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/IterationHandles.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6850 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/GlobalsLocalsNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9067 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinRefNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5550 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/NodeMetaClasses.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17853 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/TryNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4082 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/AttributeLookupNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2142 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinHashNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    94880 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/StatementBasesGenerated.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3637 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/AsyncgenNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    46286 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ConstantRefNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7856 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ExceptionNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    24899 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/NodeBases.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11002 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/KeyValuePairNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21278 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ExpressionShapeMixins.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1712 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/MatchNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6772 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ReturnNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1550 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/Checkers.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6534 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ModuleAttributeNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    28658 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/StrNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8448 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ClassNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2727 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinDecoratorNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    39803 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/FunctionNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    30314 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ConditionalNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3407 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/PrintNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8044 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ExecEvalNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3606 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinNextNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16320 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ListOperationNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)   245536 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9134 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/OperatorNodesUnary.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8640 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/SubscriptNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12004 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/AttributeNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    31894 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/OperatorNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4202 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/OsSysNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13543 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinTypeNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    31342 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/PackageMetadataNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5491 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ImportHardNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12156 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/FrameNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1714 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/CtypesNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1573 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinVarsNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5334 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/BuiltinIntegerNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    41307 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/nodes/ExpressionBasesGenerated.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    61976 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/Options.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14550 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/PostProcessing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5143 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/__past__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2055 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/Version.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2447 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/Errors.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3395 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/TreeXML.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5437 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/BytecodeCaching.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11148 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/Constants.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/containers/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      554 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/containers/OrderedSets.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4397 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/containers/OrderedSetsFallback.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/containers/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1435 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/containers/Namedtuples.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6553 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/containers/OrderedDicts.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/reports/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/reports/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15558 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/reports/Reports.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2209 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/reports/LicenseReport.rst.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12083 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/PythonVersions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8064 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/ModuleRegistry.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5770 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/Progress.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/code_generation/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8416 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/CoroutineCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6291 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/ModuleCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2375 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/CodeHelperSelection.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1033 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/InjectCCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1597 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/MatchCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4879 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/CodeObjectCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9809 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/StringCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13095 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/RaisingCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6375 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/LoaderCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4446 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/ComparisonHelperDefinitions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    51024 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/CodeGeneration.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8118 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/Namify.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2612 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/LineNumberCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6911 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/GlobalsLocalsCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1396 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/Indentation.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8099 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/YieldCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14717 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/VariableCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12010 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/IteratorCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    28478 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/DictCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8188 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/SubscriptCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8975 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/ExceptionCodes.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/code_generation/templates/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5747 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesConstants.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6640 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesVariables.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2475 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates/TemplateDebugWrapper.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6339 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesFrames.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3190 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21441 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesModules.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2290 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesExceptions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2728 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2805 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2335 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesIterators.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3321 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesFunction.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4217 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesLoader.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1574 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/CtypesCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5879 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/ConstantCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17725 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/FrameCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5721 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/GlobalConstants.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14392 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/CodeHelpers.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15892 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/ListCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2125 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/Emission.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3432 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/IntegerCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4896 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/ClassCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5234 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/ReturnCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9325 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/ErrorCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12304 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/EvalCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1794 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/IdCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12777 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/OperationCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2093 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/ExpressionCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    27345 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/FunctionCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6346 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/AsyncgenCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10153 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/AttributeCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7335 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/ConditionalCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3443 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/Reports.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    21864 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/BinaryOperationHelperDefinitions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9121 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/VariableDeclarations.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7350 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    35905 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/CallCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    28479 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/PackageResourceCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13294 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/ImportCodes.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11231 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2557 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1544 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3933 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4292 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2843 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7197 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4288 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12850 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3860 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7407 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    15380 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4487 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2984 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19317 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1905 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5904 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3635 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    10421 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2979 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2817 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2762 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperLongTools.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2088 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11579 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2044 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperImportHard.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3020 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    23262 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1843 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2118 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11102 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3173 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5238 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12818 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    13949 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/SliceCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11176 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/TryCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2339 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/BranchCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3135 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/LoopCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7622 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/GeneratorCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3786 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/TupleCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9951 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/LocalsDictCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5474 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/PythonAPICodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1506 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/IndexCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2022 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/LabelCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16009 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/BuiltinCodes.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/code_generation/c_types/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5128 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1378 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeCLongs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1804 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeCFloats.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/c_types/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    19628 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/c_types/CTypePyObjectPointers.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3610 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6069 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeBases.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3955 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5211 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeNuitkaInts.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3399 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeBooleans.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2852 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeVoids.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6517 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/SetCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    31196 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/Contexts.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    16827 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/ComparisonCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3021 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/code_generation/PrintCodes.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/commercial/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      815 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/commercial/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/general/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/general/find_module/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1238 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/general/find_module/__main__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/general/find_module/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/general/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/general/dll_report/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2366 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/general/dll_report/__main__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/general/dll_report/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/onefile_compressor/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1311 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/onefile_compressor/__main__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/onefile_compressor/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8869 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/onefile_compressor/OnefileCompressor.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1603 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/Basics.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/testing/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3375 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/Valgrind.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/testing/measure_construct_performance/
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8755 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/measure_construct_performance/__main__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/measure_construct_performance/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5371 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/SearchModes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7888 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/RuntimeTracing.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/testing/find_sxs_modules/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1949 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/find_sxs_modules/__main__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/find_sxs_modules/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/testing/check_reference_counts/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3064 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/check_reference_counts/__main__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/check_reference_counts/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    55189 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/Common.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1483 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/Constructs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1278 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/Pythons.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/testing/compare_with_cpython/
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    29429 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/compare_with_cpython/__main__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/compare_with_cpython/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8940 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/OutputComparison.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/testing/run_nuitka_tests/
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    36321 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/run_nuitka_tests/__main__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/testing/run_nuitka_tests/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/data_composer/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1306 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/data_composer/__main__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/data_composer/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14081 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/data_composer/DataComposer.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/environments/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/environments/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2449 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/environments/CreateEnvironment.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3735 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/environments/Virtualenv.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/profiler/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2529 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/profiler/__main__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/profiler/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/scanning/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/scanning/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2369 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/scanning/DisplayPackageDLLs.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2049 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/scanning/DisplayPackageData.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/nuitka/tools/specialize/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    33585 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/specialize/SpecializePython.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      833 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/specialize/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7685 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/specialize/Common.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    51143 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/specialize/CTypeDescriptions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    39625 2023-04-25 06:15:40.000000 Nuitka-1.5.7/nuitka/tools/specialize/SpecializeC.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      834 2023-04-25 06:15:40.000000 Nuitka-1.5.7/pyproject.toml
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/misc/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1038 2023-04-25 06:15:40.000000 Nuitka-1.5.7/misc/nuitka.bat
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      901 2023-04-25 06:15:40.000000 Nuitka-1.5.7/misc/nuitka-run.bat
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    11348 2023-04-25 06:15:40.000000 Nuitka-1.5.7/LICENSE.txt
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/lib/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4250 2023-04-25 06:15:40.000000 Nuitka-1.5.7/lib/hints.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/plugins/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/plugins/parameters/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2168 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/plugins/parameters/parameter-using-plugin.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1019 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/plugins/parameters/ParametersMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/plugins/data_files/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1332 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/plugins/data_files/DataFilesMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/plugins/data_files/data_files_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/plugins/data_files/data_files_package/lala.txt
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      924 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/plugins/data_files/data_files_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/plugins/data_files/data_files_package/sub_dir/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      255 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/plugins/data_files/test_case.nuitka-package.config.yml
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3532 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/plugins/run_all.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/optimizations/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      921 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/optimizations/Conditions.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1333 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/optimizations/Subscripts.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1212 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/optimizations/FormatStrings36.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      918 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/optimizations/Iterations.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      958 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/optimizations/ArgumentTypes.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2262 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/optimizations/Operations.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1150 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/optimizations/HardImports.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1260 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/optimizations/Len.py
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     8736 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/optimizations/run_all.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1021 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/optimizations/Calls.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      909 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/optimizations/DecodingOperations.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      974 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/optimizations/HardImports_2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1055 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/optimizations/Attributes.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/standalone/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2554 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/CtypesUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1757 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/PySide6Using.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1184 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/GtkUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1431 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/MatplotlibUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3228 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/Urllib3Using.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1136 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/FlaskUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1379 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/PandasUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1151 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/LxmlUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2074 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/PkgResourcesRequiresUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1067 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/PmwUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1086 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/IdnaUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1727 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/NumpyUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      990 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/GlfwUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      973 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/ShlibUsing.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/standalone/zip_importer/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1264 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/zip_importer/ZipImporterMain.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1085 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/PyQt5Plugins.py
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     9531 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/run_all.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1105 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/PyQt5SSLSupport.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1025 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/HexEncodingTest_2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1066 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/PasslibUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2538 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/MetadataPackagesUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1504 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/SocketUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1323 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/RsaUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1200 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/Win32ComUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1151 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/PendulumUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1058 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/BrotliUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1941 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/TkInterUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2050 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/PyQt6Using.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2050 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/PyQt5Using.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      947 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/standalone/OpenGLUsing.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/basics/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1628 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/DecoratorsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1899 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ParameterErrorsTest32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      890 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/FutureTest32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5934 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/AssignmentsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2305 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/TryExceptFramesTest.py
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2271 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/run_xml.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1988 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/OperatorsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3824 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/GlobalStatementTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1104 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/BuiltinOverload.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      995 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ConstantsTest27.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2899 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ReferencingTest_2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4764 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ClassesTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2923 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ListContractionsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1159 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ThreadedGeneratorsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2095 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/VarargsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14391 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ExceptionRaisingTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2842 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/TryReturnFinallyTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5853 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ParameterErrorsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2469 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ImportingTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      878 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/RecursionTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2212 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/TryExceptContinueTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2317 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/DefaultParametersTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1458 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ExceptionRaisingTest33.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1618 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/InspectionTest_36.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3603 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/FunctionsTest32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4698 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ComparisonChainsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3749 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/BuiltinSuperTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1286 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/HelloWorldTest_2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2275 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/TryExceptFinallyTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1630 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/SlotsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4879 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/WithStatementsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4227 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/InspectionTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2086 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/TryContinueFinallyTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1417 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ExtremeClosureTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      863 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/PrintFutureTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1877 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/UnpackingTest35.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4639 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ConstantsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1041 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/GeneratorExpressionsTest_37.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    12335 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/FunctionsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2328 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/TryYieldFinallyTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1406 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ClassesTest34.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1093 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/UnicodeTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1827 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/OrderChecksTest27.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3072 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/YieldFromTest33.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14903 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/OrderChecksTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1127 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/DoubleDeletionsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5809 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/GeneratorExpressionsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5866 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/AssignmentsTest32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1504 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/InspectionTest_35.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      866 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ClassMinimalTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1925 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ModuleAttributesTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1766 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/AssertsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1413 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/PrintingTest_2.py
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3821 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/run_all.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1788 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/TrickAssignmentsTest_2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     7819 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ReferencingTest33.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    22965 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/TrickAssignmentsTest32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6745 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ExecEvalTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    23840 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ReferencingTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1536 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/MainProgramsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4055 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/BranchingTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2627 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/FunctionsTest_2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5092 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ReferencingTest36.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1658 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/FunctionObjectsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      961 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ExceptionRaisingTest32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1296 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/InplaceOperationsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2731 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/LateClosureAssignmentTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2076 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ReferencingTest27.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3329 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/LoopingTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      806 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/EmptyModuleTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    17079 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/BuiltinsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3414 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ClassesTest32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1541 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/TrickAssignmentsTest35.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     4902 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/ReferencingTest35.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1452 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/OverflowFunctionsTest_2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1671 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/basics/LambdasTest.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/onefile/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1307 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/onefile/KeyboardInterruptTest.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      993 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/onefile/HelloWorldTest.py
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     5816 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/onefile/run_all.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/packages/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/packages/package_import_success_after_failure/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2382 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/packages/package_import_success_after_failure/variable_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1168 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/packages/package_import_success_after_failure/variable_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      942 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/tests/packages/sub_package/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/packages/sub_package/kitty/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1230 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/packages/sub_package/kitty/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/packages/sub_package/kitty/speak/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      966 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/packages/sub_package/kitty/speak/miau.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      929 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/packages/sub_package/kitty/speak/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1053 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/packages/sub_package/kitty/speak/hello.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      968 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/packages/sub_package/kitty/speak/purr.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      910 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/packages/sub_package/kitty/smallkitty.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      908 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/packages/sub_package/kitty/bigkitty.py
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     3671 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/packages/run_all.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/tests/packages/top_level_attributes_3/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/packages/top_level_attributes_3/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2336 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/packages/top_level_attributes_3/some_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      907 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/packages/top_level_attributes_3/some_package/some_module.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/reflected/
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)    14085 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/reflected/compile_itself.py
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1243 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/run-tests
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_contains_main/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_contains_main/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      801 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_contains_main/local.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      789 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_contains_main/PackageContainsMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_prevents_submodule/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2972 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_prevents_submodule/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1078 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_prevents_submodule/some_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      800 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_prevents_submodule/some_package/some_module.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/case_imports3/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/case_imports3/path2/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/case_imports3/path2/Some_Package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      810 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/case_imports3/path2/Some_Package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      809 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/case_imports3/path2/Some_Module.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1075 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/case_imports3/CasedImportingMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/case_imports3/path1/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/case_imports3/path1/Some_Package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      810 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/case_imports3/path1/Some_Package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      809 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/case_imports3/path1/Some_Module.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_init_import/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      823 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_init_import/PackageInitImportMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_init_import/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1169 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_init_import/some_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1008 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_init_import/some_package/PackageLocal.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_missing_init/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      926 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_missing_init/PackageMissingInitMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_missing_init/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      965 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_missing_init/some_package/some_module.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_missing_init/some_package/sub_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      977 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/dash_main/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      809 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/dash_main/Dash-Main.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/main_raises2/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1080 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/main_raises2/ErrorInFunctionMain.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      808 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/main_raises2/ErrorRaising.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/resource_reader37/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1169 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/resource_reader37/ResourceReaderMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/resource_reader37/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       13 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/resource_reader37/some_package/DATA_FILE.txt
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/resource_reader37/some_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/import_variants/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1005 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/import_variants/ImportVariationsMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/import_variants/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      994 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/import_variants/some_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      946 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/import_variants/some_package/Child1.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1098 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/import_variants/some_package/Child2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      822 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/import_variants/some_package/Child3.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/deep/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      898 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/deep/DeepProgramMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/deep/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      980 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/deep/some_package/DeepBrother.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/deep/some_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      909 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/deep/some_package/DeepChild.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/deep/some_package/deep_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      952 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/deep/some_package/deep_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      876 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/case_imports2/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/case_imports2/path2/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/case_imports2/path2/Some_Package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      799 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/case_imports2/path2/Some_Package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      798 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/case_imports2/path2/Some_Module.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      808 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/case_imports2/CasedImportingMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/case_imports2/path1/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/case_imports2/path1/some_module.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/case_imports2/path1/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/case_imports2/path1/some_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/pkgutil_itermodules/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1728 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package2/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package1/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/multiprocessing_using/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      990 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/multiprocessing_using/foo/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      836 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/multiprocessing_using/foo/__main__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/multiprocessing_using/foo/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1758 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/multiprocessing_using/foo/entry.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_code/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      800 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_code/PackageInitCodeMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_code/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      809 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_code/some_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      810 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_code/some_package/SomeModule.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:04.000000 Nuitka-1.5.7/tests/programs/package_program/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_program/PackageAsMain/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1630 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_program/PackageAsMain/__main__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      888 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_program/PackageAsMain/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/relative_import/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/relative_import/dircache.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      842 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/relative_import/RelativeImportMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/module_object_replacing/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1078 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1359 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/module_object_replacing/SelfReplacingModule.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/stdlib_overload/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1171 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/stdlib_overload/StdlibOverloadMain.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      799 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/stdlib_overload/pyexpat.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/stdlib_overload/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      810 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/stdlib_overload/some_package/pyexpat.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/stdlib_overload/some_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1236 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/stdlib_overload/some_package/star_importing.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      909 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/stdlib_overload/some_package/normal_importing.py
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     6615 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/run_all.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/plugin_import/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      859 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/plugin_import/PluginImportMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/plugin_import/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      771 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/plugin_import/some_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      781 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/plugin_import/some_package/some_module.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/main_raises/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      808 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/main_raises/ErrorRaising.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      911 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/main_raises/ErrorMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/absolute_import/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      867 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/absolute_import/AbsoluteImportMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/absolute_import/foobar/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      796 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/absolute_import/foobar/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1043 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/absolute_import/foobar/foobar.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      860 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/absolute_import/foobar/util.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      879 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/absolute_import/foobar/local.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/syntax_errors/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1079 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/syntax_errors/SyntaxErrorsMain.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      800 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/syntax_errors/SyntaxErroring.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      791 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/syntax_errors/IndentationErroring.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/unicode_bom/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      963 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/unicode_bom/UnicodeBomMain.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      846 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/unicode_bom/unicode_bom.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/named_imports/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      846 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/named_imports/NamedImportsMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/named_imports/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      824 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/named_imports/some_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/named_imports/some_package/SomeModule.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/named_imports/some_package/sub_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/named_imports/some_package/sub_package/SomeModule.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/with space/
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      826 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/with space/Space Main.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/dash_import/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      888 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/dash_import/DashImportMain.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      817 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/dash_import/dash-module.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      817 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/dash_import/plus+module.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/reimport_main_static/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      898 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/reimport_main_static/ImportItselfStaticMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/pkgutil_usage/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1261 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/pkgutil_usage/package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       13 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/pkgutil_usage/package/DATA_FILE.txt
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1553 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/pkgutil_usage/package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       14 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)       14 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/module_exits/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      869 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/module_exits/ErrorExitingModule.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      867 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/module_exits/Main.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/module_attributes/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1529 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/module_attributes/ModuleAttributesMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/module_attributes/package_level1/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/module_attributes/package_level1/package_level2/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1611 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/module_attributes/package_level1/package_level2/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/module_attributes/package_level1/package_level2/package_level3/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1611 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1744 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1744 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1611 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/module_attributes/package_level1/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1744 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/module_attributes/package_level1/Nearby1.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/dunderinit_imports/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/dunderinit_imports/package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      857 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/dunderinit_imports/package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      797 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/dunderinit_imports/package/SubModule.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      794 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/dunderinit_imports/DunderInitImportsMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_overload/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      852 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_overload/Main.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_overload/foo/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      799 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_overload/foo/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_overload/foo/bar.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      769 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_overload/foo/bar2.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/reimport_main_dynamic/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      911 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_module_collision/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      801 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_module_collision/something.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_module_collision/Something/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      810 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_module_collision/Something/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      901 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_init_issue/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      789 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_init_issue/PackageInitIssueMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_init_issue/some_package/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/package_init_issue/some_package/child_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      795 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_init_issue/some_package/child_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      798 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      798 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/package_init_issue/some_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/case_imports1/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/case_imports1/path2/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      798 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/case_imports1/path2/some_module.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/case_imports1/path2/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      799 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/case_imports1/path2/some_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      808 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/case_imports1/CasedImportingMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/case_imports1/path1/
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/case_imports1/path1/Some_Package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      799 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/case_imports1/path1/Some_Package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      798 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/case_imports1/path1/Some_Module.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/cyclic_imports/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      801 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/cyclic_imports/CyclicImportsMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/programs/cyclic_imports/cyclic_importing_package/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      842 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      875 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      875 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
+drwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)        0 2023-04-25 08:09:05.000000 Nuitka-1.5.7/tests/syntax/
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      874 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/TryExceptAllNotLast.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      869 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/SyntaxError.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      800 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/ModuleReturn.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      792 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/GlobalForParameter.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      841 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/MisplacedFutureImport.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      793 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/YieldFromInModule.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      791 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/DuplicateArgument.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      868 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/NonlocalNotFound32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      908 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/StarImportExtra.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      915 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/LateFutureImport.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      781 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/YieldInModule.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      799 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/IndentationError.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      811 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/AsyncgenReturn36.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      804 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/YieldInAsync35.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      883 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/NonAsciiWithoutEncoding_2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      849 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/ContinueWithoutLoop.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1041 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/GeneratorExpressions38.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      826 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/FutureBraces.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      995 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/Importing32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      868 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/BreakWithoutLoop.py
+-rwxr-xr-x   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     2203 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/run_all.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      805 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/FutureUnknown.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)     1111 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/ExecWithNesting_2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      923 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/YieldInGenexp38.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      809 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/UnpackTwoStars32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      970 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/ClosureDel_2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      879 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/GeneratorReturn_2.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      776 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/UnpackNoTuple.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      794 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/NonlocalForParameter32.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      791 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/ClassReturn.py
+-rw-r--r--   0 nuitka-buildslave  (2003) nuitka-buildslave  (2003)      875 2023-04-25 06:15:40.000000 Nuitka-1.5.7/tests/syntax/TryFinallyContinue_37.py
```

### Comparing `Nuitka-1.5.6/PKG-INFO` & `Nuitka-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka
-Version: 1.5.6
+Version: 1.5.7
 Summary: Python compiler with full language support and CPython compatibility
 Home-page: https://nuitka.net
 Author: Kay Hayen
 Author-email: Kay.Hayen@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Mastodon, https://fosstodon.org/@kayhayen
 Project-URL: Support, https://nuitka.net/pages/support.html
```

### Comparing `Nuitka-1.5.6/setup.py` & `Nuitka-1.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,17 +248,15 @@
 
     for type_ in "console", "gui":
         group = type_ + "_scripts"
 
         for name, _ep in dist.get_entry_map(group).items():
             script_text = runner_script_template
 
-            args = cls._get_script_args(  # pylint: disable=protected-access
-                type_, name, header, script_text
-            )
+            args = cls._get_script_args(type_, name, header, script_text)
             for res in args:
                 yield res
 
 
 try:
     easy_install.ScriptWriter.get_args = get_args
 except AttributeError:
```

### Comparing `Nuitka-1.5.6/bin/measure-construct-performance` & `Nuitka-1.5.7/bin/measure-construct-performance`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/bin/check-nuitka-with-pylint` & `Nuitka-1.5.7/bin/check-nuitka-with-pylint`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/bin/nuitka-run` & `Nuitka-1.5.7/bin/nuitka-run`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/bin/autoformat-nuitka-source` & `Nuitka-1.5.7/bin/autoformat-nuitka-source`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/bin/compare_with_cpython` & `Nuitka-1.5.7/bin/compare_with_cpython`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/bin/compare_with_xml` & `Nuitka-1.5.7/bin/compare_with_xml`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/bin/nuitka` & `Nuitka-1.5.7/bin/nuitka`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/README.pdf` & `Nuitka-1.5.7/README.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 0% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'331346'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'331346'*

 * *DEBUG:pdfminer.psparser:seek: 331346*

 * *DEBUG:pdfminer.psparser:nexttoken: (331346, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=331346, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 331350, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 331351, b'0 223\n'*

 * *DEBUG:pdfminer.psparser:nextline: 331357, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 331377, b'0000000073 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 331397, b'0000000195 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 331417, b'0000000302 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 331437, b'0000000414 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 331457, b'0000000519 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 331477, b'0000000687 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 331497, b'0000000802 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 331517, b'0000000970 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 331537, b'0000001089 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 331557, b'0000001320 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 331577, b'0000001528 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 331597, b'0000001717 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 331617, b'0000001912 00000 n \n'*

 * *[ truncated after 25 lines; 9701 ignored ]*

```diff
@@ -2350,21 +2350,21 @@
 </object>
 
 <object id="69">
 <dict size="9">
 <key>Author</key>
 <value><string size="0"></string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230412080033+00&#39;00&#39;</string></value>
+<value><string size="23">D:20230425100758+00&#39;00&#39;</string></value>
 <key>Creator</key>
 <value><string size="13">&#40;unspecified&#41;</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230412080033+00&#39;00&#39;</string></value>
+<value><string size="23">D:20230425100758+00&#39;00&#39;</string></value>
 <key>Producer</key>
 <value><string size="41">ReportLab PDF Library - www.reportlab.com</string></value>
 <key>Subject</key>
 <value><string size="13">&#40;unspecified&#41;</string></value>
 <key>Title</key>
 <value><string size="18">Nuitka User Manual</string></value>
 <key>Trapped</key>
@@ -5039,16 +5039,16 @@
 </dict>
 </object>
 
 <trailer>
 <dict size="4">
 <key>ID</key>
 <value><list size="2">
-<string size="16">mr&#175;&#198;&#247;!&#9;NB&#138;&#192;&#162;&#168;&#189;&#200;&#187;</string>
-<string size="16">mr&#175;&#198;&#247;!&#9;NB&#138;&#192;&#162;&#168;&#189;&#200;&#187;</string>
+<string size="16">&#141;2&#247;&#246;&#204;&#24;&#30;&#21;&#164;$&#185;Y&#161;-&#234;-</string>
+<string size="16">&#141;2&#247;&#246;&#204;&#24;&#30;&#21;&#164;$&#185;Y&#161;-&#234;-</string>
 </list></value>
 <key>Info</key>
 <value><ref id="69" /></value>
 <key>Root</key>
 <value><ref id="68" /></value>
 <key>Size</key>
 <value><number>223</number></value>
```

### Comparing `Nuitka-1.5.6/doc/Logo/Nuitka-Logo-Vertical.svg` & `Nuitka-1.5.7/doc/Logo/Nuitka-Logo-Vertical.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/doc/Logo/Nuitka-Logo-Symbol.svg` & `Nuitka-1.5.7/doc/Logo/Nuitka-Logo-Symbol.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/doc/Logo/Nuitka-Logo-Horizontal.svg` & `Nuitka-1.5.7/doc/Logo/Nuitka-Logo-Horizontal.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/doc/images/Nuitka-Logo-Horizontal.png` & `Nuitka-1.5.7/doc/images/Nuitka-Logo-Horizontal.png`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/doc/images/Nuitka-Logo-Vertical.png` & `Nuitka-1.5.7/doc/images/Nuitka-Logo-Vertical.png`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/doc/images/Nuitka-Logo-Symbol.png` & `Nuitka-1.5.7/doc/images/Nuitka-Logo-Symbol.png`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/doc/nuitka3-run.1` & `Nuitka-1.5.7/doc/nuitka3-run.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man 1.48.1.
-.TH NUITKA-RUN "1" "April 2023" "nuitka-run 1.5.6" "User Commands"
+.TH NUITKA-RUN "1" "April 2023" "nuitka-run 1.5.7" "User Commands"
 .SH NAME
 nuitka-run \- the Python compiler
 .SH SYNOPSIS
 .B nuitka-run
 [\fI\,options\/\fR] \fI\,main_module.py\/\fR
 .SH OPTIONS
 .TP
@@ -742,15 +742,15 @@
 Commercial: None
 Python: 3.9.2 (default, Feb 28 2021, 17:03:44)
 Flavor: Debian Python
 Executable: \fI\,/usr/bin/python3\/\fP
 OS: Linux
 Arch: armv7l
 Distribution: Debian 11
-Version C compiler: \fI\,/usr/lib/ccache/gcc\/\fP (gcc).
+Version C compiler: \fI\,/usr/local/bin/gcc\/\fP (gcc).
 .SH EXAMPLES
 
 Compile a Python file "some_module.py" to a module "some_module.so":
 .IP
 \f(CW$ nuitka \-\-module some_module.py\fR
 .PP
 Compile a Python program "some_program.py" to an executable "some_program.exe":
```

### Comparing `Nuitka-1.5.6/doc/nuitka2.1` & `Nuitka-1.5.7/doc/nuitka2.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man 1.48.1.
-.TH NUITKA "1" "April 2023" "nuitka 1.5.6" "User Commands"
+.TH NUITKA "1" "April 2023" "nuitka 1.5.7" "User Commands"
 .SH NAME
 nuitka \- the Python compiler
 .SH SYNOPSIS
 .B nuitka
 [\fI\,--module\/\fR] [\fI\,--run\/\fR] [\fI\,options\/\fR] \fI\,main_module.py\/\fR
 .SH OPTIONS
 .TP
@@ -742,15 +742,15 @@
 Commercial: None
 Python: 2.7.18 (default, Jul 14 2021, 08:11:37)
 Flavor: Debian Python
 Executable: \fI\,/usr/bin/python2\/\fP
 OS: Linux
 Arch: armv7l
 Distribution: Debian 11
-Version C compiler: \fI\,/usr/lib/ccache/gcc\/\fP (gcc).
+Version C compiler: \fI\,/usr/local/bin/gcc\/\fP (gcc).
 .SH EXAMPLES
 
 Compile a Python file "some_module.py" to a module "some_module.so":
 .IP
 \f(CW$ nuitka \-\-module some_module.py\fR
 .PP
 Compile a Python program "some_program.py" to an executable "some_program.exe":
```

### Comparing `Nuitka-1.5.6/doc/nuitka2-run.1` & `Nuitka-1.5.7/doc/nuitka2-run.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man 1.48.1.
-.TH NUITKA-RUN "1" "April 2023" "nuitka-run 1.5.6" "User Commands"
+.TH NUITKA-RUN "1" "April 2023" "nuitka-run 1.5.7" "User Commands"
 .SH NAME
 nuitka-run \- the Python compiler
 .SH SYNOPSIS
 .B nuitka-run
 [\fI\,options\/\fR] \fI\,main_module.py\/\fR
 .SH OPTIONS
 .TP
@@ -742,15 +742,15 @@
 Commercial: None
 Python: 2.7.18 (default, Jul 14 2021, 08:11:37)
 Flavor: Debian Python
 Executable: \fI\,/usr/bin/python2\/\fP
 OS: Linux
 Arch: armv7l
 Distribution: Debian 11
-Version C compiler: \fI\,/usr/lib/ccache/gcc\/\fP (gcc).
+Version C compiler: \fI\,/usr/local/bin/gcc\/\fP (gcc).
 .SH EXAMPLES
 
 Compile a Python file "some_module.py" to a module "some_module.so":
 .IP
 \f(CW$ nuitka \-\-module some_module.py\fR
 .PP
 Compile a Python program "some_program.py" to an executable "some_program.exe":
```

### Comparing `Nuitka-1.5.6/doc/nuitka3.1` & `Nuitka-1.5.7/doc/nuitka3.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man 1.48.1.
-.TH NUITKA "1" "April 2023" "nuitka 1.5.6" "User Commands"
+.TH NUITKA "1" "April 2023" "nuitka 1.5.7" "User Commands"
 .SH NAME
 nuitka \- the Python compiler
 .SH SYNOPSIS
 .B nuitka
 [\fI\,--module\/\fR] [\fI\,--run\/\fR] [\fI\,options\/\fR] \fI\,main_module.py\/\fR
 .SH OPTIONS
 .TP
@@ -742,15 +742,15 @@
 Commercial: None
 Python: 3.9.2 (default, Feb 28 2021, 17:03:44)
 Flavor: Debian Python
 Executable: \fI\,/usr/bin/python3\/\fP
 OS: Linux
 Arch: armv7l
 Distribution: Debian 11
-Version C compiler: \fI\,/usr/lib/ccache/gcc\/\fP (gcc).
+Version C compiler: \fI\,/usr/local/bin/gcc\/\fP (gcc).
 .SH EXAMPLES
 
 Compile a Python file "some_module.py" to a module "some_module.so":
 .IP
 \f(CW$ nuitka \-\-module some_module.py\fR
 .PP
 Compile a Python program "some_program.py" to an executable "some_program.exe":
```

### Comparing `Nuitka-1.5.6/Changelog.rst` & `Nuitka-1.5.7/Changelog.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/Developer_Manual.pdf` & `Nuitka-1.5.7/Developer_Manual.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 0% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'796056'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'796056'*

 * *DEBUG:pdfminer.psparser:seek: 796056*

 * *DEBUG:pdfminer.psparser:nexttoken: (796056, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=796056, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 796060, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 796061, b'0 669\n'*

 * *DEBUG:pdfminer.psparser:nextline: 796067, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 796087, b'0000000073 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 796107, b'0000000204 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 796127, b'0000000311 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 796147, b'0000006874 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 796167, b'0000007598 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 796187, b'0000007868 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 796207, b'0000007980 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 796227, b'0000008149 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 796247, b'0000008318 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 796267, b'0000008487 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 796287, b'0000008657 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 796307, b'0000008827 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 796327, b'0000008997 00000 n \n'*

 * *[ truncated after 25 lines; 31742 ignored ]*

```diff
@@ -12745,21 +12745,21 @@
 </object>
 
 <object id="380">
 <dict size="9">
 <key>Author</key>
 <value><string size="0"></string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230412080045+00&#39;00&#39;</string></value>
+<value><string size="23">D:20230425100809+00&#39;00&#39;</string></value>
 <key>Creator</key>
 <value><string size="13">&#40;unspecified&#41;</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230412080045+00&#39;00&#39;</string></value>
+<value><string size="23">D:20230425100809+00&#39;00&#39;</string></value>
 <key>Producer</key>
 <value><string size="41">ReportLab PDF Library - www.reportlab.com</string></value>
 <key>Subject</key>
 <value><string size="13">&#40;unspecified&#41;</string></value>
 <key>Title</key>
 <value><string size="23">Nuitka Developer Manual</string></value>
 <key>Trapped</key>
@@ -17503,16 +17503,16 @@
 </dict>
 </object>
 
 <trailer>
 <dict size="4">
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#191;&#140;,&#142;&#229;&#230;&#18;&#165;-&#138;iC&#165;&#221;}Y</string>
-<string size="16">&#191;&#140;,&#142;&#229;&#230;&#18;&#165;-&#138;iC&#165;&#221;}Y</string>
+<string size="16">8&#172;l&#149;~J%&#39;~&#171;O&#255;H&#17;v5</string>
+<string size="16">8&#172;l&#149;~J%&#39;~&#171;O&#255;H&#17;v5</string>
 </list></value>
 <key>Info</key>
 <value><ref id="380" /></value>
 <key>Root</key>
 <value><ref id="379" /></value>
 <key>Size</key>
 <value><number>669</number></value>
```

### Comparing `Nuitka-1.5.6/README.rst` & `Nuitka-1.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/Developer_Manual.rst` & `Nuitka-1.5.7/Developer_Manual.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/Nuitka.egg-info/PKG-INFO` & `Nuitka-1.5.7/Nuitka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka
-Version: 1.5.6
+Version: 1.5.7
 Summary: Python compiler with full language support and CPython compatibility
 Home-page: https://nuitka.net
 Author: Kay Hayen
 Author-email: Kay.Hayen@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Mastodon, https://fosstodon.org/@kayhayen
 Project-URL: Support, https://nuitka.net/pages/support.html
```

### Comparing `Nuitka-1.5.6/Nuitka.egg-info/SOURCES.txt` & `Nuitka-1.5.7/Nuitka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/Changelog.pdf` & `Nuitka-1.5.7/Changelog.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 0% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'2664636'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'2664636'*

 * *DEBUG:pdfminer.psparser:seek: 2664636*

 * *DEBUG:pdfminer.psparser:nexttoken: (2664636, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=2664636, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 2664640, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 2664641, b'0 1623\n'*

 * *DEBUG:pdfminer.psparser:nextline: 2664648, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2664668, b'0000000073 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2664688, b'0000000171 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2664708, b'0000000278 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2664728, b'0000000390 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2664748, b'0000000495 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2664768, b'0000000614 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2664788, b'0000000823 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2664808, b'0000001032 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2664828, b'0000001241 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2664848, b'0000001450 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2664868, b'0000001660 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2664888, b'0000001870 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2664908, b'0000002080 00000 n \n'*

 * *[ truncated after 25 lines; 69018 ignored ]*

```diff
@@ -11645,21 +11645,21 @@
 </object>
 
 <object id="333">
 <dict size="9">
 <key>Author</key>
 <value><string size="0"></string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230412080108+00&#39;00&#39;</string></value>
+<value><string size="23">D:20230425100832+00&#39;00&#39;</string></value>
 <key>Creator</key>
 <value><string size="13">&#40;unspecified&#41;</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230412080108+00&#39;00&#39;</string></value>
+<value><string size="23">D:20230425100832+00&#39;00&#39;</string></value>
 <key>Producer</key>
 <value><string size="41">ReportLab PDF Library - www.reportlab.com</string></value>
 <key>Subject</key>
 <value><string size="13">&#40;unspecified&#41;</string></value>
 <key>Title</key>
 <value><string size="16">Nuitka Changelog</string></value>
 <key>Trapped</key>
@@ -34140,16 +34140,16 @@
 </dict>
 </object>
 
 <trailer>
 <dict size="4">
 <key>ID</key>
 <value><list size="2">
-<string size="16">B&#16;&#10;&#40;&#220;&#246;o&#228;b&#210;hY&#24;&#39;Y&#173;</string>
-<string size="16">B&#16;&#10;&#40;&#220;&#246;o&#228;b&#210;hY&#24;&#39;Y&#173;</string>
+<string size="16">&#210;m:.&#14;g&#135;&#134;&#12;hW&#141;&#23;&#168;&#138;&#182;</string>
+<string size="16">&#210;m:.&#14;g&#135;&#134;&#12;hW&#141;&#23;&#168;&#138;&#182;</string>
 </list></value>
 <key>Info</key>
 <value><ref id="333" /></value>
 <key>Root</key>
 <value><ref id="332" /></value>
 <key>Size</key>
 <value><number>1623</number></value>
```

### Comparing `Nuitka-1.5.6/MANIFEST.in` & `Nuitka-1.5.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/Builtins.py` & `Nuitka-1.5.7/nuitka/Builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/DataComposerInterface.py` & `Nuitka-1.5.7/nuitka/build/DataComposerInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceLshift.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryMatmult.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersCalling.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersCalling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersComparisonNe.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersComparisonNe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersPythonPgo.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersPythonPgo.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryDivmod.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryDivmod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryBitor.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersTuples.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersTuples.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersComparisonLt.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersComparisonLt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceTruediv.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/InspectPatcher.c` & `Nuitka-1.5.7/nuitka/build/static_src/InspectPatcher.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersDictionaries.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersDictionaries.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceMod.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersAllocator.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersAllocator.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersBytes.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersBytes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c` & `Nuitka-1.5.7/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryAdd.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c` & `Nuitka-1.5.7/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/CompiledMethodType.c` & `Nuitka-1.5.7/nuitka/build/static_src/CompiledMethodType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersBuiltin.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersBuiltin.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersExceptions.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersExceptions.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersConstantsBlob.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersConstantsBlob.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/CompiledGeneratorType.c` & `Nuitka-1.5.7/nuitka/build/static_src/CompiledGeneratorType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/CompiledAsyncgenType.c` & `Nuitka-1.5.7/nuitka/build/static_src/CompiledAsyncgenType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceBitand.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersBuiltinTypeMethods.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersBuiltinTypeMethods.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c` & `Nuitka-1.5.7/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersComparisonGe.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersComparisonGe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersSequences.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersSequences.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceBitxor.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersSafeStrings.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersSafeStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceMatmult.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/CompiledCodeHelpers.c` & `Nuitka-1.5.7/nuitka/build/static_src/CompiledCodeHelpers.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/MetaPathBasedLoader.c` & `Nuitka-1.5.7/nuitka/build/static_src/MetaPathBasedLoader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryLshift.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersFiles.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersStrings.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryMod.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/CompiledFrameType.c` & `Nuitka-1.5.7/nuitka/build/static_src/CompiledFrameType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersDictionariesGenerated.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersDictionariesGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryMult.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersComparisonEqUtils.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersComparisonEqUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersClasses.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersClasses.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceAdd.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersMatching.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersMatching.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersImportHard.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersImportHard.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceRshift.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersFloats.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersFloats.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/OnefileBootstrap.c` & `Nuitka-1.5.7/nuitka/build/static_src/OnefileBootstrap.c`

 * *Files 1% similar despite different names*

```diff
@@ -289,15 +289,14 @@
 #if _NUITKA_ONEFILE_COMPRESSION_BOOL == 1
 
 static ZSTD_DCtx *dest_ctx = NULL;
 static ZSTD_inBuffer input = {NULL, 0, 0};
 static ZSTD_outBuffer output = {NULL, 0, 0};
 
 static void initZSTD(void) {
-    size_t const input_buffer_size = ZSTD_DStreamInSize();
     input.src = NULL;
 
     size_t const output_buffer_size = ZSTD_DStreamOutSize();
     output.dst = malloc(output_buffer_size);
     if (output.dst == NULL) {
         fatalErrorMemory();
     }
@@ -903,15 +902,15 @@
         fatalErrorHeaderAttachedData();
     }
 #endif
 
     static filename_char_t first_filename[1024] = {0};
 
 #if _NUITKA_ONEFILE_SPLASH_SCREEN
-    NUITKA_PRINT_TIMING("ONEFILE: Splash screen.");
+    NUITKA_PRINT_TIMING("ONEFILE: Init splash screen.");
 
     initSplashScreen();
 #endif
 
     NUITKA_PRINT_TIMING("ONEFILE: Entering decompression.");
 
 #if _NUITKA_ONEFILE_TEMP_BOOL == 1
```

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceBitor.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/CompiledFunctionType.c` & `Nuitka-1.5.7/nuitka/build/static_src/CompiledFunctionType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c` & `Nuitka-1.5.7/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/CompiledCellType.c` & `Nuitka-1.5.7/nuitka/build/static_src/CompiledCellType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceSub.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceSub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersFilesystemPaths.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersFilesystemPaths.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersComparisonLe.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersComparisonLe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersListsGenerated.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersListsGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersCallingGenerated.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersCallingGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersImport.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersImport.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersTypes.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersTypes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/MainProgram.c` & `Nuitka-1.5.7/nuitka/build/static_src/MainProgram.c`

 * *Files 3% similar despite different names*

```diff
@@ -102,70 +102,80 @@
 #endif
 
 #if SYSFLAG_NO_RANDOMIZATION == 1 || SYSFLAG_UNBUFFERED == 1 || defined(_NUITKA_STANDALONE)
 
 #if defined(_WIN32)
 #define environment_char_t wchar_t
 
-static environment_char_t const *getEnvironmentVariable(environment_char_t const *name) {
+static environment_char_t const *getEnvironmentVariable(char const *name) {
     // Max size for environment variables according to docs.
     wchar_t buffer[32768];
     buffer[0] = 0;
 
+    wchar_t name_wide[20];
+    name_wide[0] = 0;
+    appendStringSafeW(name_wide, name, sizeof(name_wide) / sizeof(wchar_t));
+
     // Size must be in bytes apparently, not in characters. Cannot be larger anyway.
-    DWORD res = GetEnvironmentVariableW(name, buffer, 65536);
+    DWORD res = GetEnvironmentVariableW(name_wide, buffer, 65536);
 
     if (res == 0 || res > sizeof(buffer)) {
         return NULL;
     }
 
     return wcsdup(buffer);
 }
 
-static void setEnvironmentVariable(environment_char_t const *name, environment_char_t const *value) {
-    DWORD res = SetEnvironmentVariableW(name, value);
+static void setEnvironmentVariable(char const *name, environment_char_t const *value) {
+    assert(name != NULL);
+    assert(value != NULL);
+
+    wchar_t name_wide[20];
+    name_wide[0] = 0;
+    appendStringSafeW(name_wide, name, sizeof(name_wide) / sizeof(wchar_t));
+
+    DWORD res = SetEnvironmentVariableW(name_wide, value);
+    assert(wcscmp(getEnvironmentVariable(name), value) == 0);
 
     assert(res != 0);
 }
 
-static void unsetEnvironmentVariable(environment_char_t const *name) {
-    DWORD res = SetEnvironmentVariableW(name, NULL);
+static void unsetEnvironmentVariable(char const *name) {
+    wchar_t name_wide[20];
+    name_wide[0] = 0;
+    appendStringSafeW(name_wide, name, sizeof(name_wide) / sizeof(wchar_t));
+
+    DWORD res = SetEnvironmentVariableW(name_wide, NULL);
 
     assert(res != 0);
 }
 
 #define makeEnvironmentLiteral(x) L##x
 
 #else
 #define environment_char_t char
 
 #define makeEnvironmentLiteral(x) x
 
-static environment_char_t const *getEnvironmentVariable(environment_char_t const *name) { return getenv(name); }
+static environment_char_t const *getEnvironmentVariable(char const *name) { return getenv(name); }
 
-static void setEnvironmentVariable(environment_char_t const *name, environment_char_t const *value) {
-    setenv(name, value, 1);
-}
+static void setEnvironmentVariable(char const *name, environment_char_t const *value) { setenv(name, value, 1); }
 
-static void unsetEnvironmentVariable(environment_char_t const *name) { unsetenv(name); }
+static void unsetEnvironmentVariable(char const *name) { unsetenv(name); }
 
 #endif
 
-static void undoEnvironmentVariable(environment_char_t const *variable_name, environment_char_t const *old_value) {
+static void undoEnvironmentVariable(char const *variable_name, environment_char_t const *old_value) {
     PyObject *os_module = IMPORT_HARD_OS();
     CHECK_OBJECT(os_module);
 
     PyObject *os_environ = PyObject_GetAttrString(os_module, "environ");
     CHECK_OBJECT(os_environ);
 
-#ifdef _WIN32
-    PyObject *variable_name_str = NuitkaUnicode_FromWideChar(variable_name, -1);
-#else
     PyObject *variable_name_str = Nuitka_String_FromString(variable_name);
-#endif
     CHECK_OBJECT(variable_name_str);
 
     if (old_value) {
         setEnvironmentVariable(variable_name, old_value);
 
 #ifdef _WIN32
         PyObject *env_value = NuitkaUnicode_FromWideChar(old_value, -1);
@@ -184,16 +194,15 @@
         Py_DECREF(env_value);
     } else {
         unsetEnvironmentVariable(variable_name);
 
         int res = PyObject_DelItem(os_environ, variable_name_str);
 
         if (unlikely(res != 0)) {
-            PyErr_PrintEx(1);
-            Py_Exit(1);
+            DROP_ERROR_OCCURRED();
         }
     }
 
     Py_DECREF(variable_name_str);
     Py_DECREF(os_environ);
 }
 #endif
@@ -206,24 +215,23 @@
 static environment_char_t const *old_env_pythonhome;
 
 static void prepareStandaloneEnvironment(void) {
     /* Setup environment variables to tell CPython that we would like it to use
      * the provided binary directory as the place to look for DLLs and for
      * extension modules.
      */
-    old_env_path = getEnvironmentVariable(makeEnvironmentLiteral("PATH"));
+    old_env_path = getEnvironmentVariable("PATH");
     // Remove the PATH during Python init, so it won't pick up stuff from there.
-    setEnvironmentVariable(makeEnvironmentLiteral("PATH"), makeEnvironmentLiteral("/"));
-
-    old_env_pythonhome = getEnvironmentVariable(makeEnvironmentLiteral("PYTHONHOME"));
+    setEnvironmentVariable("PATH", makeEnvironmentLiteral("/"));
 
+    old_env_pythonhome = getEnvironmentVariable("PYTHONHOME");
 #if defined(_WIN32)
-    setEnvironmentVariable(makeEnvironmentLiteral("PYTHONHOME"), getBinaryDirectoryWideChars());
+    setEnvironmentVariable("PYTHONHOME", getBinaryDirectoryWideChars());
 #else
-    setEnvironmentVariable(makeEnvironmentLiteral("PYTHONHOME"), getBinaryDirectoryHostEncoded());
+    setEnvironmentVariable("PYTHONHOME", getBinaryDirectoryHostEncoded());
 #endif
 
 #if defined(_WIN32)
     SetDllDirectoryW(getBinaryDirectoryWideChars());
 #endif
 
 #if PYTHON_VERSION < 0x300
@@ -926,16 +934,16 @@
 
 #if SYSFLAG_UNBUFFERED == 1
     setbuf(stdin, (char *)NULL);
     setbuf(stdout, (char *)NULL);
     setbuf(stderr, (char *)NULL);
 
 #if PYTHON_VERSION >= 0x300
-    environment_char_t const *old_env_unbuffered = getEnvironmentVariable(makeEnvironmentLiteral("PYTHONUNBUFFERED"));
-    setEnvironmentVariable(makeEnvironmentLiteral("PYTHONUNBUFFERED"), makeEnvironmentLiteral("1"));
+    environment_char_t const *old_env_unbuffered = getEnvironmentVariable("PYTHONUNBUFFERED");
+    setEnvironmentVariable("PYTHONUNBUFFERED", makeEnvironmentLiteral("1"));
 #endif
 #endif
 
 #ifdef __FreeBSD__
     /* FP exceptions run in "no stop" mode by default */
 
     fp_except_t m;
@@ -1035,16 +1043,16 @@
     Py_SetPythonHome(L"" PYTHON_HOME_PATH);
     // Make sure the above Py_SetPythonHome call has effect already.
     Py_GetPath();
 #endif
 #endif
 
 #if PYTHON_VERSION >= 0x300 && SYSFLAG_NO_RANDOMIZATION == 1
-    environment_char_t const *old_env_hash_seed = getEnvironmentVariable(makeEnvironmentLiteral("PYTHONHASHSEED"));
-    setEnvironmentVariable(makeEnvironmentLiteral("PYTHONHASHSEED"), makeEnvironmentLiteral("0"));
+    environment_char_t const *old_env_hash_seed = getEnvironmentVariable("PYTHONHASHSEED");
+    setEnvironmentVariable("PYTHONHASHSEED", makeEnvironmentLiteral("0"));
 #endif
 
     /* Disable CPython warnings if requested to. */
 #if NO_PYTHON_WARNINGS
     NUITKA_PRINT_TRACE("main(): Disabling Python warnings.");
     {
 #if PYTHON_VERSION >= 0x300
@@ -1205,27 +1213,27 @@
 #if PYTHON_VERSION >= 0x300
     NUITKA_PRINT_TRACE("main(): Calling patchInspectModule().");
     patchInspectModule();
 #endif
 
 #if PYTHON_VERSION >= 0x300 && SYSFLAG_NO_RANDOMIZATION == 1
     NUITKA_PRINT_TRACE("main(): Reverting to initial 'PYTHONHASHSEED' value.");
-    undoEnvironmentVariable(makeEnvironmentLiteral("PYTHONHASHSEED"), old_env_hash_seed);
+    undoEnvironmentVariable("PYTHONHASHSEED", old_env_hash_seed);
 #endif
 
 #if PYTHON_VERSION >= 0x300 && SYSFLAG_UNBUFFERED == 1
     NUITKA_PRINT_TRACE("main(): Reverting to initial 'PYTHONUNBUFFERED' value.");
-    undoEnvironmentVariable(makeEnvironmentLiteral("PYTHONUNBUFFERED"), old_env_unbuffered);
+    undoEnvironmentVariable("PYTHONUNBUFFERED", old_env_unbuffered);
 #endif
 
 #ifdef _NUITKA_STANDALONE
     // Restore the PATH, so the program can use it.
     NUITKA_PRINT_TRACE("main(): Reverting to initial 'PATH' value.");
-    undoEnvironmentVariable(makeEnvironmentLiteral("PATH"), old_env_path);
-    // undoEnvironmentVariable("PYTHONHOME", old_env_pythonhome);
+    undoEnvironmentVariable("PATH", old_env_path);
+    undoEnvironmentVariable("PYTHONHOME", old_env_pythonhome);
 #endif
 
 #if _NUITKA_PROFILE
     // Profiling with "vmprof" if enabled.
     startProfiling();
 #endif
```

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersHeapStorage.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersHeapStorage.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryPow.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryPow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersComparisonGt.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersComparisonGt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryBitand.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersMappings.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersMappings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplacePow.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplacePow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinarySub.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinarySub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryRshift.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/OnefileSplashScreen.cpp` & `Nuitka-1.5.7/nuitka/build/static_src/OnefileSplashScreen.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -15,28 +15,29 @@
 //     See the License for the specific language governing permissions and
 //     limitations under the License.
 //
 // Creates a stream object initialized with the data from an executable resource.
 
 #ifdef __IDE_ONLY__
 #include "HelpersSafeStrings.c"
+#include "nuitka/tracing.h"
 #include <windows.h>
 #endif
 
 #include <assert.h>
 #include <wincodec.h>
 
 #ifdef __MINGW32__
 #error "No support for splash screens with MinGW64 yet, only works with MSVC. Somebody please make it portable."
 #endif
 
 IStream *createImageStream(void) {
 
     // Load the resource with image data
-    HRSRC res_handle = FindResource(NULL, MAKEINTRESOURCE(27), RT_RCDATA);
+    HRSRC res_handle = FindResource(NULL, MAKEINTRESOURCE(28), RT_RCDATA);
     if (res_handle == NULL) {
         return NULL;
     }
     DWORD resource_size = SizeofResource(NULL, res_handle);
     HGLOBAL image_handle = LoadResource(NULL, res_handle);
     if (image_handle == NULL) {
         return NULL;
@@ -217,14 +218,16 @@
     }
 
     HANDLE handle_splash_file =
         CreateFileW(splash_indicator_path, GENERIC_WRITE, FILE_SHARE_WRITE, NULL, CREATE_ALWAYS, 0, NULL);
     CloseHandle(handle_splash_file);
 
     splash_active = true;
+
+    NUITKA_PRINT_TIMING("ONEFILE: Done with splash screen.");
 }
 
 static void closeSplashScreen(void) {
     if (splash_window) {
         DestroyWindow(splash_window);
         splash_window = 0;
     }
```

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryTruediv.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersSlices.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersSlices.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersComparisonEq.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersComparisonEq.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersProfiling.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersProfiling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersAttributes.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersAttributes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersLists.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersLists.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersChecksumTools.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersChecksumTools.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/CompiledCoroutineType.c` & `Nuitka-1.5.7/nuitka/build/static_src/CompiledCoroutineType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationInplaceMult.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationInplaceMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersRaising.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersRaising.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersDeepcopy.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersDeepcopy.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/static_src/HelpersOperationBinaryBitxor.c` & `Nuitka-1.5.7/nuitka/build/static_src/HelpersOperationBinaryBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/tracing.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/tracing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helpers.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helpers.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/checksum_tools.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/checksum_tools.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/compiled_frame.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/compiled_frame.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/compiled_generator.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/compiled_generator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/incbin.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/incbin.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/allocator.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/allocator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/compiled_cell.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/compiled_cell.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/checkers.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/checkers.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/freelists.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/freelists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/compiled_function.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/compiled_function.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/unfreezing.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/unfreezing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/threading.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/threading.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/exceptions.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/exceptions.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/constants.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/constants.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/safe_string_ops.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/safe_string_ops.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/prelude.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/prelude.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/compiled_asyncgen.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/compiled_asyncgen.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/constants_blob.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/constants_blob.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/filesystem_paths.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/filesystem_paths.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/importing.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/importing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/builtins.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/builtins.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/compiled_method.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/compiled_method.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/python_pgo.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/python_pgo.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/printing.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/printing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/ints.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/ints.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/comparisons_ge.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/comparisons_ge.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/sequences.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/sequences.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_add.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/indexes.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/indexes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/comparisons_le.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/comparisons_le.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_truediv.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_mult.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_divmod.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_divmod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_mod.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_builtin_types.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_builtin_types.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/bytearrays.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/bytearrays.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_sub.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/slices.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/slices.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/lists_generated.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/lists_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_rshift.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/lists.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/lists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_bitor.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/comparisons_ne.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/comparisons_ne.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_add.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/floats.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/floats.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/boolean.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/boolean.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/iterators.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/iterators.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/strings.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/strings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/sets.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/sets.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/raising.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/raising.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/richcomparisons.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/richcomparisons.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/comparisons_lt.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/comparisons_lt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_pow.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_pow.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/attributes.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/attributes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/mappings.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/mappings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_mod.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_mult.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/dictionaries.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/dictionaries.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_matmult.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_sub.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/comparisons_gt.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/comparisons_gt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/calling_generated.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/calling_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_bitand.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_lshift.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/comparisons_eq.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/comparisons_eq.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/bytes.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/bytes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/tuples.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/tuples.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/import_hard.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/import_hard.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/rangeobjects.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/rangeobjects.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/complex.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/complex.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/subscripts.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/subscripts.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/compiled_coroutine.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/compiled_coroutine.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/hedley.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/hedley.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/include/nuitka/calling.h` & `Nuitka-1.5.7/nuitka/build/include/nuitka/calling.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/Onefile.scons` & `Nuitka-1.5.7/nuitka/build/Onefile.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/SconsHacks.py` & `Nuitka-1.5.7/nuitka/build/SconsHacks.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/__init__.py` & `Nuitka-1.5.7/nuitka/build/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/SconsSpawn.py` & `Nuitka-1.5.7/nuitka/build/SconsSpawn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/Backend.scons` & `Nuitka-1.5.7/nuitka/build/Backend.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/SconsCompilerSettings.py` & `Nuitka-1.5.7/nuitka/build/SconsCompilerSettings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/SconsCaching.py` & `Nuitka-1.5.7/nuitka/build/SconsCaching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/CCompilerVersion.scons` & `Nuitka-1.5.7/nuitka/build/CCompilerVersion.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/clcache/clcache/LICENSE` & `Nuitka-1.5.7/nuitka/build/inline_copy/clcache/clcache/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/clcache/clcache/caching.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/clcache/clcache/caching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/glob2/glob2/impl.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/glob2/glob2/impl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/glob2/glob2/compat.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/glob2/glob2/compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/glob2/glob2/fnmatch.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/glob2/glob2/fnmatch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/glob2/LICENSE` & `Nuitka-1.5.7/nuitka/build/inline_copy/glob2/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/LICENSE` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/representer.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/serializer.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/reader.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/events.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/loader.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/emitter.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/parser.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/nodes.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/tokens.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/scanner.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/resolver.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/constructor.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/composer.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/error.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/cyaml.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml/yaml/dumper.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/appdirs/appdirs.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/appdirs/appdirs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/appdirs/LICENSE.txt` & `Nuitka-1.5.7/nuitka/build/inline_copy/appdirs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2_35/LICENSE.rst` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2_35/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/loaders.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/environment.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/ext.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/utils.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/parser.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/nodes.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/filters.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/meta.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/lexer.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/_compat.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/defaults.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/debug.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/tests.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/visitor.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/compiler.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/runtime.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/bccache.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/constants.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/jinja2/LICENSE.rst` & `Nuitka-1.5.7/nuitka/build/inline_copy/jinja2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/bin/scons.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/bin/scons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/LICENSE` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/representer.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/serializer.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/reader.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/events.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/loader.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/emitter.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/parser.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/nodes.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/tokens.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/scanner.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/resolver.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/constructor.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/composer.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/error.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/dumper.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/LICENSE` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/representer.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/serializer.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/reader.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/events.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/loader.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/emitter.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/parser.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/nodes.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/tokens.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/scanner.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/resolver.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/constructor.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/composer.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/error.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/dumper.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/atomicwrites/LICENSE` & `Nuitka-1.5.7/nuitka/build/inline_copy/atomicwrites/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/atomicwrites/atomicwrites.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/atomicwrites/atomicwrites.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/zstd.h` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/zstd.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/entropy_common.c` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/huf.h` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/huf.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/zstd_internal.h` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/error_private.c` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/error_private.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/debug.h` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/debug.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/bitstream.h` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/zstd_common.c` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/fse.h` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/fse.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/xxhash.c` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/zstd_errors.h` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/zstd_deps.h` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/error_private.h` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/error_private.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/xxhash.h` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/cpu.h` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/cpu.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/fse_decompress.c` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/mem.h` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/mem.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/common/compiler.h` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/common/compiler.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/zstd/LICENSE.txt` & `Nuitka-1.5.7/nuitka/build/inline_copy/zstd/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/gui.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/gui.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/utils.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/notebook.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/notebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/dask.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/dask.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_utils.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/std.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/std.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/auto.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/auto.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/tk.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/tk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/markupsafe/LICENSE.rst` & `Nuitka-1.5.7/nuitka/build/inline_copy/markupsafe/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/colorama/LICENSE.txt` & `Nuitka-1.5.7/nuitka/build/inline_copy/colorama/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/colorama/colorama/win32.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/colorama/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/colorama/colorama/ansi.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/colorama/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/colorama/colorama/initialise.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/colorama/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/inline_copy/colorama/colorama/winterm.py` & `Nuitka-1.5.7/nuitka/build/inline_copy/colorama/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/SconsInterface.py` & `Nuitka-1.5.7/nuitka/build/SconsInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/SconsProgress.py` & `Nuitka-1.5.7/nuitka/build/SconsProgress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/build/SconsUtils.py` & `Nuitka-1.5.7/nuitka/build/SconsUtils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/PythonOperators.py` & `Nuitka-1.5.7/nuitka/PythonOperators.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,29 +118,28 @@
 
 
 all_comparison_functions = dict(rich_comparison_functions)
 all_comparison_functions.update(other_comparison_functions)
 
 
 def matchException(left, right):
+    # This doesn't yet work, make it error exit and silence PyLint for now.
+    # pylint: disable=unused-argument
+
     if python_version >= 0x300:
         if type(right) is tuple:
             for element in right:
                 if not isinstance(BaseException, element):
                     raise TypeError(
                         "catching classes that do not inherit from BaseException is not allowed"
                     )
         elif not isinstance(BaseException, right):
             raise TypeError(
                 "catching classes that do not inherit from BaseException is not allowed"
             )
 
-    # This doesn't yet work, make it error exit. and silence PyLint for now.
-    # pylint: disable=protected-access
     import os
 
     os._exit(16)
 
-    assert False, left
-
 
 all_comparison_functions["exception_match"] = matchException
```

### Comparing `Nuitka-1.5.6/nuitka/MainControl.py` & `Nuitka-1.5.7/nuitka/MainControl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/__main__.py` & `Nuitka-1.5.7/nuitka/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/DataFilesPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/DataFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/UpxPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/UpxPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/TorchPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/TorchPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/OptionsNannyPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/OptionsNannyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/__init__.py` & `Nuitka-1.5.7/nuitka/plugins/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/GlfwPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/GlfwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/DillPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/DillPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/DelvewheelPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/DelvewheelPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/AntiBloatPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/AntiBloatPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/PywebViewPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/PywebViewPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/PbrPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/PbrPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/GeventPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/GeventPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/TkinterPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/TkinterPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/PmwPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/PmwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/standard.nuitka-package.config.yml` & `Nuitka-1.5.7/nuitka/plugins/standard/standard.nuitka-package.config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -199,16 +199,16 @@
         'compile': 'un-callable'
         'distutils_extension': 'un-callable'
       when: 'not use_cffi_recompiler'
 
 - module-name: 'cffi.ffiplatform'
   anti-bloat:
     - description: 'disable distutils hacks'
-      replacements:
-        'import setuptools': "'pass'"
+      replacements_plain:
+        'import setuptools': 'pass'
     - description: 'disable distutils hacks'
       change_function:
         'get_extension': 'un-callable'
         '_build': 'un-callable'
       when: 'not use_cffi_recompiler'
 
 - module-name: 'chainer'
@@ -412,17 +412,17 @@
     patterns:
       - 'distributed.yaml'
 
 - module-name: 'distributed.scheduler'
   anti-bloat:
     - description: 'remove cython support'
       # TODO: We should replace this with a nuitkarize in Cython maybe.
-      replacements:
-        'from cython import compiled': "'raise ImportError'"
-        'if compiled:': "'if False:'"
+      replacements_plain:
+        'from cython import compiled': 'raise ImportError'
+        'if compiled:': 'if False:'
 
 - module-name: 'dns.rdtypes'
   implicit-imports:
     - depends:
         - '.IN.A'
         - '.CH.A'
 
@@ -448,16 +448,16 @@
   data-files:
     patterns:
       - 'eel.js'
 
 - module-name: 'eliot._traceback'
   anti-bloat:
     - description: 'avoid useless duplication of traceback module'
-      replacements:
-        'load_module(str("_traceback_no_io"), traceback)': "'__import__(\"traceback\")'"
+      replacements_plain:
+        'load_module(str("_traceback_no_io"), traceback)': '__import__("traceback")'
 
 - module-name: 'enchant'
   data-files:
     dirs:
       - 'data'
 
 - module-name: 'engineio'
@@ -1125,31 +1125,59 @@
         "imp.find_module('pytest')": "'None'"
 
 - module-name: 'mozilla-ca'
   data-files:
     patterns:
       - '*.pem'
 
+- module-name: 'mpmath'
+  anti-bloat:
+    - description: 'remove pytest reference'
+      change_function:
+        'doctests': 'un-callable'
+        'runtests': 'un-callable'
+      when: 'not use_pytest'
+
 - module-name: 'nacl._sodium'
   implicit-imports:
     - depends:
         - '_cffi_backend'
 
 - module-name: 'networkx'
   anti-bloat:
     - description: 'remove networkx.testing usage'
       replacements_plain:
         'from networkx.testing.test import run as test': 'test = None'
 
+- module-name: 'networkx.classes.backends'
+  anti-bloat:
+    - description: 'remove pytest reference'
+      replacements_plain:
+        'os.environ.get("NETWORKX_GRAPH_CONVERT")': 'None'
+      when: 'not use_pytest'
+
 - module-name: 'networkx.utils.decorators'
   anti-bloat:
     - description: 'required for decorator compatibility'
       replacements_plain:
         'func.__defaults__ = f.__defaults__': ''
         'real_func = func.__argmap__.compile(func.__wrapped__)': 'return func'
+        '    return argmap(_not_implemented_for, 0)': |
+          #
+              import functools
+              def inner(func):
+                  @functools.wraps(func)
+                  def _not_implemented_for(g):
+                      if (mval is None or mval == g.is_multigraph()) and (
+                          dval is None or dval == g.is_directed()
+                      ):
+                          raise nx.NetworkXNotImplemented(errmsg)
+                      return func(g)
+                  return _not_implemented_for
+              return inner
 
 - module-name: 'nose.core'
   data-files:
     patterns:
       - 'usage.txt'
 
 - module-name: 'numba'
@@ -1384,14 +1412,20 @@
         - 'numpy'
 
 - module-name: 'openapi_spec_validator'
   data-files:
     dirs:
       - 'resources/schemas'
 
+- module-name: 'opentele.utils'
+  anti-bloat:
+    - description: 'workaround compiled function decorator issues'
+      replacements_plain:
+        'bases = func.__class__.__bases__': 'bases = func.__class__.__bases__ if bases != (FunctionType,) else (object,)'
+
 - module-name: 'openvino'
   data-files:
     dirs:
       - 'libs'
 
 - module-name: 'openvino.inference_engine'
   dlls:
@@ -1671,14 +1705,15 @@
 
 - module-name: 'patsy.util'
   anti-bloat:
     - description: 'remove pytest reference'
       change_function:
         'test_pandas_friendly_reshape': 'un-callable'
         'test_wide_dtype_for_and_widen': 'un-callable'
+      when: 'not use_pytest'
 
 - module-name: 'pendulum'
   data-files:
     empty_dir_structures:
       - 'locales'
 
 - module-name: 'pendulum.locales'
@@ -1879,14 +1914,19 @@
         'from ._common import NETBSD': "'NETBSD = %r' % + psutil.NETBSD"
         'from ._common import OPENBSD': "'OPENBSD = %r' % + psutil.OPENBSD"
         'from ._common import OSX': "'OSX = %r' % psutil.OSX"
         'from ._common import POSIX': "'POSIX = %r' % psutil.POSIX"
         'from ._common import SUNOS': "'SUNOS = %r' % psutil.SUNOS"
         'from ._common import WINDOWS': "'WINDOWS = %r' % psutil.WINDOWS"
 
+- module-name: 'pyarrow.lib'
+  implicit-imports:
+    - depends:
+        - 'pyarrow.vendored.version'
+
 - module-name: 'pyarrow.vendored.docscrape'
   anti-bloat:
     - description: 'remove sphinx reference'
       replacements_plain:
         "if 'sphinx' in sys.modules:": 'if False:'
     - description: 'workaround for MSVC bug with scipy docscrape 1.8.x'
       replacements_plain:
@@ -2152,15 +2192,32 @@
       - description: 'PySide2 cannot be signed unless onefile'
         macos_bundle_as_onefile: 'yes'
         when: 'macos and plugin("pyside2")'
   import-hacks:
     - find-dlls-near-module:
         - 'shiboken2'
 
-- module-name: 'PySide6'
+- module-name: 'PySide6.QtCore'
+  implicit-imports:
+    - depends:
+        - 'PySide6.support.deprecated'
+    - post-import-code:
+        - |
+          def myconnect(self, func):
+              if hasattr(func, "im_func"):
+                  if hasattr(func.im_func, "__compiled__"):
+                      myconnect._protected = getattr(myconnect, "_protected", set())
+                      myconnect._protected.add(func)
+
+              return orig_connect(self, func)
+
+          from PySide6 import QtCore
+          orig_connect = QtCore.SignalInstance.connect
+          QtCore.SignalInstance.connect = myconnect
+
   options:
     checks:
       - description: 'PySide6 is a GUI framework'
         console: 'recommend'
         when: 'plugin("pyside6")'
   import-hacks:
     - find-dlls-near-module:
@@ -3260,14 +3317,34 @@
       - 'sv.tcl'
 
 - module-name: 'swagger_ui_bundle'
   data-files:
     dirs:
       - 'vendor'
 
+- module-name: 'sympy.interactive.printing'
+  anti-bloat:
+    - description: 'remove IPython reference'
+      replacements_plain:
+        'import IPython': 'raise ImportError'
+        'from IPython import get_ipython': 'raise ImportError'
+        'from IPython.terminal.interactiveshell import TerminalInteractiveShell': 'raise ImportError'
+        'from IPython.frontend.terminal.interactiveshell import TerminalInteractiveShell': 'raise ImportError'
+        'from IPython.lib.latextools import latex_to_png': 'raise ImportError'
+        'from IPython.core.interactiveshell import InteractiveShell': 'raise ImportError'
+      when: 'not use_ipython'
+
+- module-name: 'sympy.interactive.session'
+  anti-bloat:
+    - description: 'remove IPython reference'
+      replacements_plain:
+        'import IPython': 'raise ImportError'
+        'from IPython import get_ipython': 'raise ImportError'
+      when: 'not use_ipython'
+
 - module-name: 'tables'
   anti-bloat:
     - description: 'remove tables.tests usage'
       replacements_plain:
         'from .tests import print_versions, test': ''
 
 - module-name: 'tables.filters'
@@ -3999,14 +4076,21 @@
 - module-name: 'trio._core._multierror'
   anti-bloat:
     - description: 'remove IPython reference'
       replacements_plain:
         '"IPython" in sys.modules': 'False'
       when: 'not use_ipython'
 
+- module-name: 'triton.compiler'
+  anti-bloat:
+    - description: 'remove setuptools usage'
+      replacements_plain:
+        'import setuptools': ''
+      when: 'not use_setuptools'
+
 - module-name: 'tzdata'
   data-files:
     dirs:
       - 'zones'
 
 - module-name: 'tzdata.zoneinfo'
   data-files:
```

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/ImplicitImports.py` & `Nuitka-1.5.7/nuitka/plugins/standard/ImplicitImports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/TensorflowPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/TensorflowPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/PkgResourcesPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/PkgResourcesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/GiPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/GiPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml` & `Nuitka-1.5.7/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/MultiprocessingPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/MultiprocessingPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/TrioPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/TrioPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/EventletPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/EventletPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/KivyPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/KivyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/MatplotlibPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/MatplotlibPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/EnumPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/EnumPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/PySidePyQtPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/PySidePyQtPlugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -607,15 +607,14 @@
     ]
 )
 
 os.environ["QML2_IMPORT_PATH"] = os.path.join(
     os.path.dirname(__file__),
     "qml"
 )
-
 """ % {
                 "package_name": full_name
             }
 
             yield (
                 code,
                 """\
```

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/DllFilesPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/DllFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/NumpyPlugin.py` & `Nuitka-1.5.7/nuitka/plugins/standard/NumpyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml` & `Nuitka-1.5.7/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/Plugins.py` & `Nuitka-1.5.7/nuitka/plugins/Plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -438,15 +438,15 @@
         with withPluginModuleNameProblemReporting(plugin, package_name):
             for path in plugin.getPackageExtraScanPaths(package_name, package_dir):
                 if os.path.isdir(path):
                     yield path
 
     @classmethod
     def getPackageExtraScanPaths(cls, package_name, package_dir):
-        key = package_name
+        key = package_name, package_dir
 
         if key not in cls.extra_scan_paths_cache:
             cls.extra_scan_paths_cache[key] = ()
 
             for plugin in getActivePlugins():
                 cls.extra_scan_paths_cache[key] += tuple(
                     cls._getPackageExtraScanPaths(
@@ -741,28 +741,29 @@
                 source_code=code,
                 is_top=False,
                 is_main=False,
                 is_extension=False,
                 is_fake=module_name,
                 hide_syntax_error=False,
             )
-        except SyntaxError:
+        except SyntaxError as e:
             plugins_logger.sysexit(
-                "SyntaxError in plugin provided source code for '%s'." % module_name
+                "SyntaxError in plugin provided source code for '%s': %s."
+                % (module_name, e)
             )
 
         if trigger_module.getCompilationMode() == "bytecode":
             trigger_module.setSourceCode(code)
 
         return trigger_module
 
     @classmethod
     def onModuleDiscovered(cls, module):
         # We offer plugins many ways to provide extra stuff
-        # pylint: disable=too-many-branches,too-many-locals,too-many-statements
+        # pylint: disable=too-many-locals,too-many-statements
 
         full_name = module.getFullName()
 
         def _untangleLoadDescription(description):
             if description and inspect.isgenerator(description):
                 description = tuple(description)
 
@@ -812,58 +813,64 @@
                     description=plugin.createPostModuleLoadCode(module)
                 )
             )
             fake_module_descriptions.extend(
                 _untangleFakeDesc(description=plugin.createFakeModuleDependency(module))
             )
 
-        if pre_module_load_descriptions:
-            total_code = []
+        def combineLoadCodes(module_load_descriptions, mode):
+            future_imports_code = []
+            normal_code_code = []
             total_flags = OrderedSet()
             reasons = []
 
-            for plugin, pre_code, reason, flags in pre_module_load_descriptions:
-                if pre_code:
+            for plugin, code, reason, flags in module_load_descriptions:
+                if code:
                     plugin.info(
-                        "Injecting pre-module load code for module '%s':" % full_name
+                        "Injecting %s-module load code for module '%s':"
+                        % (mode, full_name)
                     )
                     for line in reason.split("\n"):
                         plugin.info("    " + line)
 
-                    total_code.append(pre_code)
+                    for line in code.splitlines():
+                        line = line + "\n"
+
+                        if line.startswith("from __future__"):
+                            future_imports_code.append(line)
+                        else:
+                            normal_code_code.append(line)
+
                     total_flags.update(flags)
                     reasons.append(reason)
 
+            total_code = future_imports_code + normal_code_code
+
+            return total_code, reasons, total_flags
+
+        if pre_module_load_descriptions:
+            total_code, reasons, total_flags = combineLoadCodes(
+                module_load_descriptions=pre_module_load_descriptions, mode="pre"
+            )
+
             if total_code:
                 assert full_name not in pre_modules
 
                 pre_modules[full_name] = cls._createTriggerLoadedModule(
                     module=module,
                     trigger_name=pre_module_load_trigger_name,
                     code="\n\n".join(total_code),
                     flags=total_flags,
                 )
                 pre_modules_reasons[full_name] = tuple(reasons)
 
         if post_module_load_descriptions:
-            total_code = []
-            total_flags = OrderedSet()
-            reasons = []
-
-            for plugin, post_code, reason, flags in post_module_load_descriptions:
-                if post_code:
-                    plugin.info(
-                        "Injecting post-module load code for module '%s':" % full_name
-                    )
-                    for line in reason.split("\n"):
-                        plugin.info("    " + line)
-
-                    total_code.append(post_code)
-                    total_flags.update(flags)
-                    reasons.append(reason)
+            total_code, reasons, total_flags = combineLoadCodes(
+                module_load_descriptions=post_module_load_descriptions, mode="post"
+            )
 
             if total_code:
                 assert full_name not in post_modules
 
                 post_modules[full_name] = cls._createTriggerLoadedModule(
                     module=module,
                     trigger_name=post_module_load_trigger_name,
@@ -959,15 +966,14 @@
 
             if type(must_recurse) is not tuple and must_recurse not in (True, False):
                 plugin.sysexit(
                     "Error, onModuleEncounter code failed to return a None or tuple(bool, reason) result."
                 )
 
             if result is not None:
-                # false alarm, pylint: disable=unsubscriptable-object
                 if result[0] != must_recurse[0]:
                     plugin.sysexit(
                         "Error, decision %s does not match other plugin '%s' decision."
                         % (must_recurse[0], ".".join(deciding_plugins))
                     )
 
             deciding_plugins.append(plugin.plugin_name)
```

### Comparing `Nuitka-1.5.6/nuitka/plugins/__init__.py` & `Nuitka-1.5.7/nuitka/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/plugins/PluginBase.py` & `Nuitka-1.5.7/nuitka/plugins/PluginBase.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/Bytecodes.py` & `Nuitka-1.5.7/nuitka/Bytecodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/distutils/__init__.py` & `Nuitka-1.5.7/nuitka/distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/distutils/DistutilCommands.py` & `Nuitka-1.5.7/nuitka/distutils/DistutilCommands.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,20 @@
 import wheel.bdist_wheel  # pylint: disable=I0021,import-error,no-name-in-module
 
 from nuitka.__past__ import Iterable, unicode
 from nuitka.containers.OrderedSets import OrderedSet
 from nuitka.importing.Importing import (
     addMainScriptDirectory,
     decideModuleSourceRef,
+    flushImportCache,
     locateModule,
 )
 from nuitka.Tracing import wheel_logger
 from nuitka.utils.Execution import check_call
+from nuitka.utils.FileOperations import deleteFile, renameFile
 from nuitka.utils.ModuleNames import ModuleName
 
 
 def setupNuitkaDistutilsCommands(dist, keyword, value):
     # If the user project setup.py includes the key "build_with_nuitka=True" all
     # build operations (build, bdist_wheel, install etc) will run via Nuitka.
     # pylint: disable=unused-argument
@@ -108,15 +110,15 @@
             )
 
         # Python2 does not allow super on this old style class.
         distutils.command.build.build.run(self)
 
         self._build(os.path.abspath(self.build_lib))
 
-    def _findBuildTasks(self):
+    def _findBuildTasks2(self):
         """
         Helper for _build
         Returns list containing bool (is_package) and module_names
 
         Algorithm for finding distinct packages:
         1) Take minimum package
         2) Find related packages that start with this name
@@ -177,14 +179,50 @@
             py_packages = [
                 p for p in py_packages if not p.hasNamespace(current_package)
             ]
             builds.append((True, current_package))
 
         return builds
 
+    def _findBuildTasks(self):
+        builds = self._findBuildTasks2()
+        result = []
+
+        for _is_package, module_name_orig in builds:
+            _module_name, main_filename, module_kind, finding = locateModule(
+                module_name=module_name_orig,
+                parent_package=None,
+                level=0,
+            )
+
+            # Handle extension modules already compiled. They are either to be replaced, or
+            # they are included as they are, because there is no source, then the task can
+            # be skipped.
+            if module_kind == "extension":
+                main_filename_away = main_filename + ".away"
+                renameFile(main_filename, main_filename_away)
+
+                flushImportCache()
+
+                _module_name, main_filename, module_kind, finding = locateModule(
+                    module_name=module_name_orig,
+                    parent_package=None,
+                    level=0,
+                )
+
+                if finding != "not-found":
+                    deleteFile(main_filename_away, must_exist=True)
+                else:
+                    renameFile(main_filename_away, main_filename)
+                    continue
+
+            result.append((_is_package, module_name_orig))
+
+        return result
+
     @staticmethod
     def _parseOptionsEntry(option, value):
         option = "--" + option.lstrip("-")
 
         if type(value) is tuple and len(value) == 2 and value[0] == "setup.py":
             value = value[1]
```

### Comparing `Nuitka-1.5.6/nuitka/distutils/Build.py` & `Nuitka-1.5.7/nuitka/distutils/Build.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/CacheCleanup.py` & `Nuitka-1.5.7/nuitka/CacheCleanup.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/optimizations/Tags.py` & `Nuitka-1.5.7/nuitka/optimizations/Tags.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/optimizations/FunctionInlining.py` & `Nuitka-1.5.7/nuitka/optimizations/FunctionInlining.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/optimizations/Graphs.py` & `Nuitka-1.5.7/nuitka/optimizations/Graphs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/optimizations/__init__.py` & `Nuitka-1.5.7/nuitka/optimizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/optimizations/Optimization.py` & `Nuitka-1.5.7/nuitka/optimizations/Optimization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/optimizations/BytecodeDemotion.py` & `Nuitka-1.5.7/nuitka/optimizations/BytecodeDemotion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/optimizations/OptimizeBuiltinCalls.py` & `Nuitka-1.5.7/nuitka/optimizations/OptimizeBuiltinCalls.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/optimizations/TraceCollections.py` & `Nuitka-1.5.7/nuitka/optimizations/TraceCollections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/optimizations/ValueTraces.py` & `Nuitka-1.5.7/nuitka/optimizations/ValueTraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/OptionParsing.py` & `Nuitka-1.5.7/nuitka/OptionParsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/importing/PreloadedPackages.py` & `Nuitka-1.5.7/nuitka/importing/PreloadedPackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/importing/__init__.py` & `Nuitka-1.5.7/nuitka/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/importing/IgnoreListing.py` & `Nuitka-1.5.7/nuitka/importing/IgnoreListing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/importing/Importing.py` & `Nuitka-1.5.7/nuitka/importing/Importing.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
 from nuitka import Options, SourceCodeReferences
 from nuitka.__past__ import iter_modules
 from nuitka.containers.Namedtuples import makeNamedtupleClass
 from nuitka.containers.OrderedSets import OrderedSet
 from nuitka.importing import StandardLibrary
 from nuitka.plugins.Plugins import Plugins
+from nuitka.PythonFlavors import isNuitkaPython
 from nuitka.PythonVersions import python_version
 from nuitka.Tracing import my_print, recursion_logger
 from nuitka.tree.ReformulationMultidist import locateMultidistModule
 from nuitka.utils.AppDirs import getCacheDir
 from nuitka.utils.FileOperations import listDir, removeDirectory
 from nuitka.utils.Importing import getSharedLibrarySuffixes
 from nuitka.utils.ModuleNames import ModuleName
@@ -160,14 +161,17 @@
     if os.path.isdir(module_filename):
         return ModuleName(os.path.basename(module_filename)), "py"
 
     return None, None
 
 
 def isIgnoreListedImportMaker(source_ref):
+    if isNuitkaPython():
+        return True
+
     return StandardLibrary.isStandardLibraryPath(source_ref.getFilename())
 
 
 def warnAbout(importing, module_name, level, source_ref):
     # This probably should not be dealt with here
     if module_name == "":
         return
@@ -402,14 +406,25 @@
 
     if path not in _list_dir_cache:
         _list_dir_cache[path] = tuple(listDir(path))
 
     return _list_dir_cache[path]
 
 
+def flushImportCache():
+    """Clear import related caches.
+
+    In some situations, e.g. during package rebuild, we scan and then decide to remove
+    files and scan again. This allows that. Nothing in standard Nuitka should do it,
+    as it throws away so much.
+    """
+    _list_dir_cache.clear()
+    module_search_cache.clear()
+
+
 def _findModuleInPath2(package_name, module_name, search_path):
     """This is out own module finding low level implementation.
 
     Just the full module name and search path are given. This is then
     tasked to raise "ImportError" or return a path if it finds it, or
     None, if it is a built-in.
     """
```

### Comparing `Nuitka-1.5.6/nuitka/importing/Recursion.py` & `Nuitka-1.5.7/nuitka/importing/Recursion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/importing/StandardLibrary.py` & `Nuitka-1.5.7/nuitka/importing/StandardLibrary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/importing/ImportResolving.py` & `Nuitka-1.5.7/nuitka/importing/ImportResolving.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/importing/ImportCache.py` & `Nuitka-1.5.7/nuitka/importing/ImportCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/freezer/DependsExe.py` & `Nuitka-1.5.7/nuitka/freezer/DependsExe.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/freezer/Standalone.py` & `Nuitka-1.5.7/nuitka/freezer/Standalone.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,15 +527,19 @@
                 if package_name is not None:
                     problem_modules.add(package_name)
                 else:
                     problem_modules.add(module_name)
 
     else:
         checkModulePath = None
+        message = None
+        mnemonic = None
 
+    # We intend for other platforms to join, e.g. Fedora, etc. but currently
+    # only Debian is done.
     if checkModulePath is not None:
         for module in ModuleRegistry.getDoneModules():
             checkModulePath(module)
 
     if problem_modules:
         general.info("Using Debian packages for '%s'." % ",".join(problem_modules))
         general.warning(message=message, mnemonic=mnemonic)
```

### Comparing `Nuitka-1.5.6/nuitka/freezer/__init__.py` & `Nuitka-1.5.7/nuitka/freezer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/freezer/Onefile.py` & `Nuitka-1.5.7/nuitka/freezer/Onefile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/freezer/DllDependenciesCommon.py` & `Nuitka-1.5.7/nuitka/freezer/DllDependenciesCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/freezer/IncludedEntryPoints.py` & `Nuitka-1.5.7/nuitka/freezer/IncludedEntryPoints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/freezer/DllDependenciesPosix.py` & `Nuitka-1.5.7/nuitka/freezer/DllDependenciesPosix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/freezer/DllDependenciesMacOS.py` & `Nuitka-1.5.7/nuitka/freezer/DllDependenciesMacOS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/freezer/DllDependenciesWin32.py` & `Nuitka-1.5.7/nuitka/freezer/DllDependenciesWin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/freezer/IncludedDataFiles.py` & `Nuitka-1.5.7/nuitka/freezer/IncludedDataFiles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/constants/Serialization.py` & `Nuitka-1.5.7/nuitka/constants/Serialization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/constants/__init__.py` & `Nuitka-1.5.7/nuitka/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/__init__.py` & `Nuitka-1.5.7/nuitka/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/finalizations/__init__.py` & `Nuitka-1.5.7/nuitka/finalizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/finalizations/Finalization.py` & `Nuitka-1.5.7/nuitka/finalizations/Finalization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/finalizations/FinalizeMarkups.py` & `Nuitka-1.5.7/nuitka/finalizations/FinalizeMarkups.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/SourceCodeReferences.py` & `Nuitka-1.5.7/nuitka/SourceCodeReferences.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/Variables.py` & `Nuitka-1.5.7/nuitka/Variables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/OutputDirectories.py` & `Nuitka-1.5.7/nuitka/OutputDirectories.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/Jinja2.py` & `Nuitka-1.5.7/nuitka/utils/Jinja2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/InstanceCounters.py` & `Nuitka-1.5.7/nuitka/utils/InstanceCounters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/Json.py` & `Nuitka-1.5.7/nuitka/utils/Json.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/ReExecute.py` & `Nuitka-1.5.7/nuitka/utils/ReExecute.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,24 +45,24 @@
         args = list(args)
         del args[1]
 
         try:
             # Context manager is not available on all Python versions, pylint: disable=consider-using-with
             process = subprocess.Popen(args=args)
             process.communicate()
-            # No point in cleaning up, pylint: disable=protected-access
+            # No point in cleaning up, just exit the hard way.
             try:
                 os._exit(process.returncode)
             except OverflowError:
                 # Seems negative values go wrong otherwise,
                 # see https://bugs.python.org/issue28474
                 os._exit(process.returncode - 2**32)
         except KeyboardInterrupt:
             # There was a more relevant stack trace already, so abort this
-            # right here, pylint: disable=protected-access
+            # right here.
             os._exit(2)
     else:
         # The star arguments is the API of execl
         os.execl(*args)
 
 
 def reExecuteNuitka(pgo_filename):
```

### Comparing `Nuitka-1.5.6/nuitka/utils/Distributions.py` & `Nuitka-1.5.7/nuitka/utils/Distributions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/CStrings.py` & `Nuitka-1.5.7/nuitka/utils/CStrings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/FileOperations.py` & `Nuitka-1.5.7/nuitka/utils/FileOperations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/StaticLibraries.py` & `Nuitka-1.5.7/nuitka/utils/StaticLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/__init__.py` & `Nuitka-1.5.7/nuitka/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/WindowsFileUsage.py` & `Nuitka-1.5.7/nuitka/utils/WindowsFileUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/Images.py` & `Nuitka-1.5.7/nuitka/utils/Images.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/WindowsResources.py` & `Nuitka-1.5.7/nuitka/utils/WindowsResources.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/Download.py` & `Nuitka-1.5.7/nuitka/utils/Download.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/Utils.py` & `Nuitka-1.5.7/nuitka/utils/Utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,14 @@
 
     return platform.release()
 
 
 def isDebianBasedLinux():
     dist_name, base, _dist_version = getLinuxDistribution()
 
-    # False alarm, pylint: disable=superfluous-parens
     return (base or dist_name) in ("Debian", "Ubuntu")
 
 
 def isFedoraBasedLinux():
     dist_name, base, _dist_version = getLinuxDistribution()
 
     return (base or dist_name) == "Fedora"
```

### Comparing `Nuitka-1.5.6/nuitka/utils/Timing.py` & `Nuitka-1.5.7/nuitka/utils/Timing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/Shebang.py` & `Nuitka-1.5.7/nuitka/utils/Shebang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/MemoryUsage.py` & `Nuitka-1.5.7/nuitka/utils/MemoryUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/ThreadedExecutor.py` & `Nuitka-1.5.7/nuitka/utils/ThreadedExecutor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/Rest.py` & `Nuitka-1.5.7/nuitka/utils/Rest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/SharedLibraries.py` & `Nuitka-1.5.7/nuitka/utils/SharedLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/Execution.py` & `Nuitka-1.5.7/nuitka/utils/Execution.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/Importing.py` & `Nuitka-1.5.7/nuitka/utils/Importing.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,15 +95,19 @@
 
             for suffix, _mode, module_type in imp.get_suffixes():
                 if module_type == imp.C_EXTENSION:
                     _shared_library_suffixes.append(suffix)
         else:
             import importlib.machinery  # pylint: disable=I0021,import-error,no-name-in-module
 
-            _shared_library_suffixes = importlib.machinery.EXTENSION_SUFFIXES
+            _shared_library_suffixes = list(importlib.machinery.EXTENSION_SUFFIXES)
+
+        # Nuitka-Python on Windows has that
+        if "" in _shared_library_suffixes:
+            _shared_library_suffixes.remove("")
 
         _shared_library_suffixes = tuple(_shared_library_suffixes)
 
     return _shared_library_suffixes
 
 
 def getSharedLibrarySuffix(preferred):
@@ -136,15 +140,15 @@
             del sys.modules[module_name]
 
     # Temporarily add the inline path of the module to the import path.
     sys.path.insert(0, path)
 
     # Handle case without inline copy too.
     try:
-        return __import__(module_name)
+        return __import__(module_name, level=0)
     except (ImportError, SyntaxError, RuntimeError) as e:
         if not must_exist:
             return None
 
         exit_message = (
             "Error, expected inline copy of '%s' to be in '%s', error was: %r."
             % (module_name, path, e)
```

### Comparing `Nuitka-1.5.6/nuitka/utils/Yaml.py` & `Nuitka-1.5.7/nuitka/utils/Yaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 what library to use for what Python. We have an inline copy of PyYAML that
 still does 2.6, on other Pythons, we expect the system to have it installed.
 
 Also we put loading for specific packages in here and a few helpers to work
 with these config files.
 """
 
+# Otherwise "Yaml" and "yaml" collide on case insensitive setups
+from __future__ import absolute_import
+
 import os
 import pkgutil
 
 from nuitka.containers.OrderedDicts import OrderedDict
 from nuitka.Options import getUserProvidedYamlFiles
 from nuitka.Tracing import general
```

### Comparing `Nuitka-1.5.6/nuitka/utils/MacOSApp.py` & `Nuitka-1.5.7/nuitka/utils/MacOSApp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/AppDirs.py` & `Nuitka-1.5.7/nuitka/utils/AppDirs.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,18 @@
 import tempfile
 
 from nuitka.Tracing import general
 
 from .FileOperations import makePath
 from .Importing import importFromInlineCopy
 
-try:
+appdirs = importFromInlineCopy("appdirs", must_exist=False)
+
+if appdirs is None:
     import appdirs  # pylint: disable=I0021,import-error
-except ImportError:
-    # We handle the case without inline copy too.
-    appdirs = importFromInlineCopy("appdirs", must_exist=False)
 
 _cache_dir = None
 
 
 def getCacheDir():
     global _cache_dir  # singleton, pylint: disable=global-statement
```

### Comparing `Nuitka-1.5.6/nuitka/utils/CommandLineOptions.py` & `Nuitka-1.5.7/nuitka/utils/CommandLineOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/ModuleNames.py` & `Nuitka-1.5.7/nuitka/utils/ModuleNames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/Signing.py` & `Nuitka-1.5.7/nuitka/utils/Signing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/Hashing.py` & `Nuitka-1.5.7/nuitka/utils/Hashing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/utils/InstalledPythons.py` & `Nuitka-1.5.7/nuitka/utils/InstalledPythons.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             self.python_version,
         )
 
     def getPythonExe(self):
         return self.python_exe
 
     def getPythonVersion(self):
-        return "%d.%d" % (self.python_version // 256, (self.python_version // 16) % 16)
+        return self.python_version
 
     # Necessary for Python 2.7, otherwise SyntaxError is given on exec.
     @staticmethod
     def _exec(code, context):
         # We can trust our own code there, pylint: disable=exec-used
         exec(code.replace("print", "catch_print"), context)
```

### Comparing `Nuitka-1.5.6/nuitka/PythonFlavors.py` & `Nuitka-1.5.7/nuitka/PythonFlavors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/Tracing.py` & `Nuitka-1.5.7/nuitka/Tracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/pgo/__init__.py` & `Nuitka-1.5.7/nuitka/pgo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/pgo/PGO.py` & `Nuitka-1.5.7/nuitka/pgo/PGO.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationExecStatements.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationExecStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationClasses.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationBooleanExpressions.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationBooleanExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationAssertStatements.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationAssertStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationYieldExpressions.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationYieldExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationMatchStatements.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationMatchStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationForLoopStatements.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationForLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationTryExceptStatements.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationTryExceptStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationNamespacePackages.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationNamespacePackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/__init__.py` & `Nuitka-1.5.7/nuitka/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationSequenceCreation.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationSequenceCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationComparisonExpressions.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationComparisonExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/Extractions.py` & `Nuitka-1.5.7/nuitka/tree/Extractions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationLambdaExpressions.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationLambdaExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/Operations.py` & `Nuitka-1.5.7/nuitka/tree/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationCallExpressions.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationCallExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ComplexCallHelperFunctions.py` & `Nuitka-1.5.7/nuitka/tree/ComplexCallHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/Building.py` & `Nuitka-1.5.7/nuitka/tree/Building.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationDictionaryCreation.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationDictionaryCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/TreeHelpers.py` & `Nuitka-1.5.7/nuitka/tree/TreeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationFunctionStatements.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationFunctionStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationPrintStatements.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationPrintStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationImportStatements.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationImportStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationWithStatements.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationWithStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationContractionExpressions.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationContractionExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationClasses3.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationClasses3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/SyntaxErrors.py` & `Nuitka-1.5.7/nuitka/tree/SyntaxErrors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/VariableClosure.py` & `Nuitka-1.5.7/nuitka/tree/VariableClosure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationWhileLoopStatements.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationWhileLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationTryFinallyStatements.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationTryFinallyStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationSubscriptExpressions.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationSubscriptExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/SourceHandling.py` & `Nuitka-1.5.7/nuitka/tree/SourceHandling.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationMultidist.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationMultidist.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/ReformulationAssignmentStatements.py` & `Nuitka-1.5.7/nuitka/tree/ReformulationAssignmentStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tree/InternalModule.py` & `Nuitka-1.5.7/nuitka/tree/InternalModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/specs/BuiltinTypeOperationSpecs.py` & `Nuitka-1.5.7/nuitka/specs/BuiltinTypeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/specs/HardImportSpecs.py` & `Nuitka-1.5.7/nuitka/specs/HardImportSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/specs/__init__.py` & `Nuitka-1.5.7/nuitka/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/specs/BuiltinBytesOperationSpecs.py` & `Nuitka-1.5.7/nuitka/specs/BuiltinBytesOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/specs/BuiltinStrOperationSpecs.py` & `Nuitka-1.5.7/nuitka/specs/BuiltinStrOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/specs/ParameterSpecs.py` & `Nuitka-1.5.7/nuitka/specs/ParameterSpecs.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,22 +413,22 @@
                 else:
                     message = (
                         "'%s' is an invalid keyword argument for this function"
                         % pair[0]
                     )
 
                 raise TooManyArguments(TypeError(message))
-            else:
-                if arg_index < num_pos_only:
-                    message = "'%s' is an invalid keyword argument for %s()" % (
-                        pair[0],
-                        func_name,
-                    )
 
-                    raise TooManyArguments(TypeError(message))
+            if arg_index < num_pos_only:
+                message = "'%s' is an invalid keyword argument for %s()" % (
+                    pair[0],
+                    func_name,
+                )
+
+                raise TooManyArguments(TypeError(message))
 
     if star_list_arg:
         if num_pos > num_args:
             value = positional[-(num_pos - num_args) :]
             assign(star_list_arg, value)
 
             if star_list_single_arg:
```

### Comparing `Nuitka-1.5.6/nuitka/specs/BuiltinUnicodeOperationSpecs.py` & `Nuitka-1.5.7/nuitka/specs/BuiltinUnicodeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/specs/BuiltinDictOperationSpecs.py` & `Nuitka-1.5.7/nuitka/specs/BuiltinDictOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/specs/BuiltinListOperationSpecs.py` & `Nuitka-1.5.7/nuitka/specs/BuiltinListOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/specs/BuiltinParameterSpecs.py` & `Nuitka-1.5.7/nuitka/specs/BuiltinParameterSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/shapes/__init__.py` & `Nuitka-1.5.7/nuitka/nodes/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/shapes/ShapeMixins.py` & `Nuitka-1.5.7/nuitka/nodes/shapes/ShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/shapes/StandardShapes.py` & `Nuitka-1.5.7/nuitka/nodes/shapes/StandardShapes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/shapes/ControlFlowDescriptions.py` & `Nuitka-1.5.7/nuitka/nodes/shapes/ControlFlowDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/shapes/BuiltinTypeShapes.py` & `Nuitka-1.5.7/nuitka/nodes/shapes/BuiltinTypeShapes.py`

 * *Files 0% similar despite different names*

```diff
@@ -4088,14 +4088,15 @@
         if value is value2:
             r[key] = value
         elif value[0] is tshape_str_or_unicode and value2[0] is tshape_unicode:
             assert value[1] is value2[1]
 
             r[key] = value
         elif value[0] is tshape_str and value2[0] is tshape_unicode:
+            # Actually as intended, pylint: disable=bad-chained-comparison
             assert (
                 value[1]
                 is value2[1]
                 in (
                     operation_result_strorunicode_noescape[1],
                     ControlFlowDescriptionFormatError,
                 )
```

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinIteratorNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinIteratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinRangeNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinRangeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinComplexNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinComplexNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/LocalsScopes.py` & `Nuitka-1.5.7/nuitka/nodes/LocalsScopes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/VariableRefNodes.py` & `Nuitka-1.5.7/nuitka/nodes/VariableRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/LoopNodes.py` & `Nuitka-1.5.7/nuitka/nodes/LoopNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/VariableAssignNodes.py` & `Nuitka-1.5.7/nuitka/nodes/VariableAssignNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/ExpressionBases.py` & `Nuitka-1.5.7/nuitka/nodes/ExpressionBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/CodeObjectSpecs.py` & `Nuitka-1.5.7/nuitka/nodes/CodeObjectSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinDictNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinLenNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinLenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/VariableDelNodes.py` & `Nuitka-1.5.7/nuitka/nodes/VariableDelNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/PackageResourceNodes.py` & `Nuitka-1.5.7/nuitka/nodes/PackageResourceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/NodeMakingHelpers.py` & `Nuitka-1.5.7/nuitka/nodes/NodeMakingHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/ContainerMakingNodes.py` & `Nuitka-1.5.7/nuitka/nodes/ContainerMakingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/SliceNodes.py` & `Nuitka-1.5.7/nuitka/nodes/SliceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BytesNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BytesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/TypeNodes.py` & `Nuitka-1.5.7/nuitka/nodes/TypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/DictionaryNodes.py` & `Nuitka-1.5.7/nuitka/nodes/DictionaryNodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1410,14 +1410,15 @@
     def computeExpression(self, trace_collection):
         if self.mayRaiseExceptionOperation():
             trace_collection.onExceptionRaiseExit(BaseException)
 
         if self.subnode_iterable.isCompileTimeConstant():
             # TODO: Could be assert against it being None with a compile time constant,
             # we will usually be able to tell?
+            # This is actually OK to use like this, pylint: disable=bad-chained-comparison
             if None is not self.subnode_iterable.getIterationLength() < 256:
                 return trace_collection.getCompileTimeComputationResult(
                     node=self,
                     computation=lambda: dict.fromkeys(
                         self.subnode_iterable.getCompileTimeConstant()
                     ),
                     description="Computed 'dict.fromkeys' with constant value.",
@@ -1428,14 +1429,15 @@
     def mayRaiseException(self, exception_type):
         return (
             self.subnode_iterable.mayRaiseException(exception_type)
             or self.mayRaiseExceptionOperation()
         )
 
     def mayRaiseExceptionOperation(self):
+        # This is actually OK to use like this, pylint: disable=bad-chained-comparison
         return None is not self.subnode_iterable.getIterationLength() < 256
 
 
 class ExpressionDictOperationFromkeys3(ExpressionDictOperationFromkeys3Base):
     kind = "EXPRESSION_DICT_OPERATION_FROMKEYS3"
 
     def computeExpression(self, trace_collection):
@@ -1444,14 +1446,15 @@
 
         if (
             self.subnode_iterable.isCompileTimeConstant()
             and self.subnode_value.isCompileTimeConstant()
         ):
             # TODO: Could be assert against it being None with a compile time constant,
             # we will usually be able to tell?
+            # This is actually OK to use like this, pylint: disable=bad-chained-comparison
             if None is not self.subnode_iterable.getIterationLength() < 256:
                 return trace_collection.getCompileTimeComputationResult(
                     node=self,
                     computation=lambda: dict.fromkeys(
                         self.subnode_iterable.getCompileTimeConstant(),
                         self.subnode_value.getCompileTimeConstant(),
                     ),
@@ -1464,14 +1467,15 @@
         return (
             self.subnode_iterable.mayRaiseException(exception_type)
             or self.subnode_value.mayRaiseException(exception_type)
             or self.mayRaiseExceptionOperation()
         )
 
     def mayRaiseExceptionOperation(self):
+        # This is actually OK to use like this, pylint: disable=bad-chained-comparison
         return None is not self.subnode_iterable.getIterationLength() < 256
 
 
 class ExpressionDictOperationFromkeysRef(ExpressionNoSideEffectsMixin, ExpressionBase):
     kind = "EXPRESSION_DICT_OPERATION_FROMKEYS_REF"
 
     def finalize(self):
```

### Comparing `Nuitka-1.5.6/nuitka/nodes/ComparisonNodes.py` & `Nuitka-1.5.7/nuitka/nodes/ComparisonNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/LocalsDictNodes.py` & `Nuitka-1.5.7/nuitka/nodes/LocalsDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinAnyNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinAnyNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/SideEffectNodes.py` & `Nuitka-1.5.7/nuitka/nodes/SideEffectNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/TypeMatchNodes.py` & `Nuitka-1.5.7/nuitka/nodes/TypeMatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/HardImportNodesGenerated.py` & `Nuitka-1.5.7/nuitka/nodes/HardImportNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/InjectCNodes.py` & `Nuitka-1.5.7/nuitka/nodes/InjectCNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/__init__.py` & `Nuitka-1.5.7/nuitka/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/CallNodes.py` & `Nuitka-1.5.7/nuitka/nodes/CallNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/ModuleNodes.py` & `Nuitka-1.5.7/nuitka/nodes/ModuleNodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -827,16 +827,15 @@
             "module_name": self.module_name,
             "main_added": self.main_added,
             "mode": self.mode,
         }
 
     @classmethod
     def fromXML(cls, provider, source_ref, **args):
-        if "code_flags" in args:
-            future_spec = fromFlags(args["code_flags"])
+        future_spec = fromFlags(args["code_flags"])
 
         result = cls(
             main_added=args["main_added"] == "True",
             mode=args["mode"],
             module_name=ModuleName(args["module_name"]),
             future_spec=future_spec,
             source_ref=source_ref,
```

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinAllNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinAllNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/VariableNameNodes.py` & `Nuitka-1.5.7/nuitka/nodes/VariableNameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinOpenNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinOpenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/OutlineNodes.py` & `Nuitka-1.5.7/nuitka/nodes/OutlineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/ChildrenHavingMixins.py` & `Nuitka-1.5.7/nuitka/nodes/ChildrenHavingMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/StatementNodes.py` & `Nuitka-1.5.7/nuitka/nodes/StatementNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/ContainerOperationNodes.py` & `Nuitka-1.5.7/nuitka/nodes/ContainerOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/GeneratorNodes.py` & `Nuitka-1.5.7/nuitka/nodes/GeneratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/VariableReleaseNodes.py` & `Nuitka-1.5.7/nuitka/nodes/VariableReleaseNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/YieldNodes.py` & `Nuitka-1.5.7/nuitka/nodes/YieldNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/FunctionAttributeNodes.py` & `Nuitka-1.5.7/nuitka/nodes/FunctionAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/IndicatorMixins.py` & `Nuitka-1.5.7/nuitka/nodes/IndicatorMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/CoroutineNodes.py` & `Nuitka-1.5.7/nuitka/nodes/CoroutineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/FutureSpecs.py` & `Nuitka-1.5.7/nuitka/nodes/FutureSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinFormatNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinFormatNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinDecodingNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinDecodingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinSumNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinSumNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/AttributeNodesGenerated.py` & `Nuitka-1.5.7/nuitka/nodes/AttributeNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/ImportNodes.py` & `Nuitka-1.5.7/nuitka/nodes/ImportNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/StringConcatenationNodes.py` & `Nuitka-1.5.7/nuitka/nodes/StringConcatenationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/IterationHandles.py` & `Nuitka-1.5.7/nuitka/nodes/IterationHandles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/GlobalsLocalsNodes.py` & `Nuitka-1.5.7/nuitka/nodes/GlobalsLocalsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinRefNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/NodeMetaClasses.py` & `Nuitka-1.5.7/nuitka/nodes/NodeMetaClasses.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         if base is not object and "__slots__" not in base.__dict__:
             raise NuitkaNodeDesignError(name, "All bases must have __slots__.", base)
 
 
 class NodeCheckMetaClass(ABCMeta):
     kinds = {}
 
-    def __new__(cls, name, bases, dictionary):  # pylint: disable=I0021,arguments-differ
+    def __new__(mcs, name, bases, dictionary):  # pylint: disable=I0021,arguments-differ
         _checkBases(name, bases)
 
         if "__slots__" not in dictionary:
             dictionary["__slots__"] = ()
 
         if "named_children" in dictionary:
             assert type(dictionary["named_children"]) is tuple
@@ -99,16 +99,15 @@
 
                 dictionary["__init__"] = __init__
 
         # Not a method:
         if "checker" in dictionary:
             dictionary["checker"] = staticmethod(dictionary["checker"])
 
-        # false alarm, pylint: disable=I0021,too-many-function-args
-        return ABCMeta.__new__(cls, name, bases, dictionary)
+        return ABCMeta.__new__(mcs, name, bases, dictionary)
 
     def __init__(cls, name, bases, dictionary):
 
         if not name.endswith(("Base", "Mixin")):
             if "kind" not in dictionary:
                 raise NuitkaNodeDesignError(name, "Must provide class variable 'kind'")
```

### Comparing `Nuitka-1.5.6/nuitka/nodes/TryNodes.py` & `Nuitka-1.5.7/nuitka/nodes/TryNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/AttributeLookupNodes.py` & `Nuitka-1.5.7/nuitka/nodes/AttributeLookupNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinHashNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinHashNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/StatementBasesGenerated.py` & `Nuitka-1.5.7/nuitka/nodes/StatementBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/AsyncgenNodes.py` & `Nuitka-1.5.7/nuitka/nodes/AsyncgenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/ConstantRefNodes.py` & `Nuitka-1.5.7/nuitka/nodes/ConstantRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/ExceptionNodes.py` & `Nuitka-1.5.7/nuitka/nodes/ExceptionNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/NodeBases.py` & `Nuitka-1.5.7/nuitka/nodes/NodeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/KeyValuePairNodes.py` & `Nuitka-1.5.7/nuitka/nodes/KeyValuePairNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/ExpressionShapeMixins.py` & `Nuitka-1.5.7/nuitka/nodes/ExpressionShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/MatchNodes.py` & `Nuitka-1.5.7/nuitka/nodes/MatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/ReturnNodes.py` & `Nuitka-1.5.7/nuitka/nodes/ReturnNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/Checkers.py` & `Nuitka-1.5.7/nuitka/nodes/Checkers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/ModuleAttributeNodes.py` & `Nuitka-1.5.7/nuitka/nodes/ModuleAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/StrNodes.py` & `Nuitka-1.5.7/nuitka/nodes/StrNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/ClassNodes.py` & `Nuitka-1.5.7/nuitka/nodes/ClassNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinDecoratorNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinDecoratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/FunctionNodes.py` & `Nuitka-1.5.7/nuitka/nodes/FunctionNodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -564,17 +564,19 @@
 
 
 class ExpressionFunctionBody(
     ExpressionNoSideEffectsMixin,
     MarkUnoptimizedFunctionIndicatorMixin,
     ExpressionFunctionEntryPointBase,
 ):
+    # TODO: There should be more special ones than this general type in order to
+    # not cover exec ones in the same object. pylint: disable=too-many-instance-attributes
+
     kind = "EXPRESSION_FUNCTION_BODY"
 
-    # TODO: These should be more special than the general type in order to not cover exec ones.
     __slots__ = (
         "unoptimized_locals",
         "unqualified_exec",
         "doc",
         "return_exception",
         "needs_creation",
         "needs_direct",
```

### Comparing `Nuitka-1.5.6/nuitka/nodes/ConditionalNodes.py` & `Nuitka-1.5.7/nuitka/nodes/ConditionalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/PrintNodes.py` & `Nuitka-1.5.7/nuitka/nodes/PrintNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/ExecEvalNodes.py` & `Nuitka-1.5.7/nuitka/nodes/ExecEvalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinNextNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinNextNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/ListOperationNodes.py` & `Nuitka-1.5.7/nuitka/nodes/ListOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/OperatorNodesUnary.py` & `Nuitka-1.5.7/nuitka/nodes/OperatorNodesUnary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/SubscriptNodes.py` & `Nuitka-1.5.7/nuitka/nodes/SubscriptNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/AttributeNodes.py` & `Nuitka-1.5.7/nuitka/nodes/AttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/OperatorNodes.py` & `Nuitka-1.5.7/nuitka/nodes/OperatorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/OsSysNodes.py` & `Nuitka-1.5.7/nuitka/nodes/OsSysNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinTypeNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinTypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/PackageMetadataNodes.py` & `Nuitka-1.5.7/nuitka/nodes/PackageMetadataNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/ImportHardNodes.py` & `Nuitka-1.5.7/nuitka/nodes/ImportHardNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/FrameNodes.py` & `Nuitka-1.5.7/nuitka/nodes/FrameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/CtypesNodes.py` & `Nuitka-1.5.7/nuitka/nodes/CtypesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinVarsNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinVarsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/BuiltinIntegerNodes.py` & `Nuitka-1.5.7/nuitka/nodes/BuiltinIntegerNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/nodes/ExpressionBasesGenerated.py` & `Nuitka-1.5.7/nuitka/nodes/ExpressionBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/Options.py` & `Nuitka-1.5.7/nuitka/Options.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/PostProcessing.py` & `Nuitka-1.5.7/nuitka/PostProcessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
         splash_data = getFileContents(splash_screen_filename, mode="rb")
 
         addResourceToFile(
             target_filename=result_filename,
             data=splash_data,
             resource_kind=RT_RCDATA,
             lang_id=0,
-            res_name=27,
+            res_name=28,
             logger=postprocessing_logger,
         )
 
 
 def executePostProcessing():
     """Postprocessing of the resulting binary.
```

### Comparing `Nuitka-1.5.6/nuitka/__past__.py` & `Nuitka-1.5.7/nuitka/__past__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/Version.py` & `Nuitka-1.5.7/nuitka/Version.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #     limitations under the License.
 #
 """ Nuitka version related stuff.
 
 """
 
 version_string = """\
-Nuitka V1.5.6
+Nuitka V1.5.7
 Copyright (C) 2022 Kay Hayen."""
 
 
 def getNuitkaVersion():
     """Return Nuitka version as a string.
 
     This should not be used for >= comparisons directly.
```

### Comparing `Nuitka-1.5.6/nuitka/Errors.py` & `Nuitka-1.5.7/nuitka/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/TreeXML.py` & `Nuitka-1.5.7/nuitka/TreeXML.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/BytecodeCaching.py` & `Nuitka-1.5.7/nuitka/BytecodeCaching.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,35 +84,47 @@
         return None
 
     if data["module_name"] != module_name:
         return None
 
     result = OrderedSet()
 
-    for module in data["modules_used"]:
-        module_name = ModuleName(module["module_name"])
+    for module_used in data["modules_used"]:
+        used_module_name = ModuleName(module_used["module_name"])
 
-        # Retry the module scan.
-        _module_name, filename, module_kind, finding = locateModule(
-            module_name=module_name, parent_package=None, level=0
-        )
+        # Retry the module scan to see if it still gives same result
+        if module_used["finding"] == "relative":
+            _used_module_name, filename, module_kind, finding = locateModule(
+                module_name=used_module_name.getBasename(),
+                parent_package=used_module_name.getPackageName(),
+                level=1,
+            )
+        else:
+            _used_module_name, filename, module_kind, finding = locateModule(
+                module_name=used_module_name, parent_package=None, level=0
+            )
+
+        if (
+            finding != module_used["finding"]
+            or module_kind != module_used["module_kind"]
+        ):
+            assert module_name != "email._header_value_parser", finding
 
-        if finding != module["finding"] or module_kind != module["module_kind"]:
             return None
 
         result.add(
             makeModuleUsageAttempt(
-                module_name=module_name,
+                module_name=used_module_name,
                 filename=filename,
-                finding=module["finding"],
-                module_kind=module["module_kind"],
+                finding=module_used["finding"],
+                module_kind=module_used["module_kind"],
                 # TODO: Level might have to be dropped.
                 level=0,
                 # We store only the line number, so this cheats it to at full one.
-                source_ref=source_ref.atLineNumber(module["source_ref_line"]),
+                source_ref=source_ref.atLineNumber(module_used["source_ref_line"]),
             )
         )
 
     return result
 
 
 def writeImportedModulesNamesToCache(module_name, source_code, used_modules):
```

### Comparing `Nuitka-1.5.6/nuitka/Constants.py` & `Nuitka-1.5.7/nuitka/Constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/containers/OrderedSets.py` & `Nuitka-1.5.7/nuitka/containers/OrderedSets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/containers/OrderedSetsFallback.py` & `Nuitka-1.5.7/nuitka/containers/OrderedSetsFallback.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/containers/__init__.py` & `Nuitka-1.5.7/nuitka/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/containers/Namedtuples.py` & `Nuitka-1.5.7/nuitka/containers/Namedtuples.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/containers/OrderedDicts.py` & `Nuitka-1.5.7/nuitka/containers/OrderedDicts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/reports/__init__.py` & `Nuitka-1.5.7/nuitka/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/reports/Reports.py` & `Nuitka-1.5.7/nuitka/reports/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/reports/LicenseReport.rst.j2` & `Nuitka-1.5.7/nuitka/reports/LicenseReport.rst.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/PythonVersions.py` & `Nuitka-1.5.7/nuitka/PythonVersions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/ModuleRegistry.py` & `Nuitka-1.5.7/nuitka/ModuleRegistry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/Progress.py` & `Nuitka-1.5.7/nuitka/Progress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/CoroutineCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/CoroutineCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/ModuleCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/ModuleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/CodeHelperSelection.py` & `Nuitka-1.5.7/nuitka/code_generation/CodeHelperSelection.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/InjectCCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/InjectCCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/MatchCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/MatchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/CodeObjectCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/CodeObjectCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/StringCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/StringCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/RaisingCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/RaisingCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/LoaderCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/LoaderCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/ComparisonHelperDefinitions.py` & `Nuitka-1.5.7/nuitka/code_generation/ComparisonHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/CodeGeneration.py` & `Nuitka-1.5.7/nuitka/code_generation/CodeGeneration.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/Namify.py` & `Nuitka-1.5.7/nuitka/code_generation/Namify.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/LineNumberCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/LineNumberCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/GlobalsLocalsCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/GlobalsLocalsCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/__init__.py` & `Nuitka-1.5.7/nuitka/code_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/Indentation.py` & `Nuitka-1.5.7/nuitka/code_generation/Indentation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/YieldCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/YieldCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/VariableCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/VariableCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/IteratorCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/IteratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/DictCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/DictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/SubscriptCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/SubscriptCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/ExceptionCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/ExceptionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesConstants.py` & `Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesConstants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesVariables.py` & `Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates/TemplateDebugWrapper.py` & `Nuitka-1.5.7/nuitka/code_generation/templates/TemplateDebugWrapper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesFrames.py` & `Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesFrames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py` & `Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates/__init__.py` & `Nuitka-1.5.7/nuitka/code_generation/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesModules.py` & `Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesModules.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesExceptions.py` & `Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesExceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py` & `Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesCoroutines.py` & `Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesCoroutines.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesIterators.py` & `Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesIterators.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesFunction.py` & `Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates/CodeTemplatesLoader.py` & `Nuitka-1.5.7/nuitka/code_generation/templates/CodeTemplatesLoader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/CtypesCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/CtypesCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/ConstantCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/ConstantCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/FrameCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/FrameCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/GlobalConstants.py` & `Nuitka-1.5.7/nuitka/code_generation/GlobalConstants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/CodeHelpers.py` & `Nuitka-1.5.7/nuitka/code_generation/CodeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/ListCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/ListCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/Emission.py` & `Nuitka-1.5.7/nuitka/code_generation/Emission.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/IntegerCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/IntegerCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/ClassCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/ClassCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/ReturnCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/ReturnCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/ErrorCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/ErrorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/EvalCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/EvalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/IdCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/IdCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/OperationCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/OperationCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/ExpressionCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/ExpressionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/FunctionCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/FunctionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/AsyncgenCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/AsyncgenCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/AttributeCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/AttributeCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/ConditionalCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/ConditionalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/Reports.py` & `Nuitka-1.5.7/nuitka/code_generation/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/BinaryOperationHelperDefinitions.py` & `Nuitka-1.5.7/nuitka/code_generation/BinaryOperationHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/VariableDeclarations.py` & `Nuitka-1.5.7/nuitka/code_generation/VariableDeclarations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py` & `Nuitka-1.5.7/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/CallCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/CallCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/PackageResourceCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/PackageResourceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/ImportCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/ImportCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperObjectTools.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperObjectTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsList.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperLongTools.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperLongTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperImportHard.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperImportHard.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2` & `Nuitka-1.5.7/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/SliceCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/SliceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/TryCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/TryCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/BranchCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/BranchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/LoopCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/LoopCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/GeneratorCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/GeneratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/TupleCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/TupleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/LocalsDictCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/LocalsDictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/PythonAPICodes.py` & `Nuitka-1.5.7/nuitka/code_generation/PythonAPICodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/IndexCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/IndexCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/LabelCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/LabelCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/BuiltinCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/BuiltinCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py` & `Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeCLongs.py` & `Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeCLongs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeCFloats.py` & `Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeCFloats.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/c_types/__init__.py` & `Nuitka-1.5.7/nuitka/code_generation/c_types/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/c_types/CTypePyObjectPointers.py` & `Nuitka-1.5.7/nuitka/code_generation/c_types/CTypePyObjectPointers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeModuleDictVariables.py` & `Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeModuleDictVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeBases.py` & `Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeNuitkaVoids.py` & `Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeNuitkaVoids.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,14 @@
         if Options.is_debug:
             emit("%s = NUITKA_VOID_OK;" % to_name)
 
     @classmethod
     def emitAssignmentCodeFromConstant(
         cls, to_name, constant, may_escape, emit, context
     ):
-        # No context needed, pylint: disable=unused-argument
-
         # Everything else expresses missed compiled time optimization.
         assert constant is None
 
         # The only possible value, and in this case never read, but the compiler hates
         # it being defined which is hard for us to know ahead of time.
         if Options.is_debug:
             emit("%s = NUITKA_VOID_OK;" % to_name)
```

### Comparing `Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeNuitkaInts.py` & `Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeNuitkaInts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeBooleans.py` & `Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/c_types/CTypeVoids.py` & `Nuitka-1.5.7/nuitka/code_generation/c_types/CTypeVoids.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/SetCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/SetCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/Contexts.py` & `Nuitka-1.5.7/nuitka/code_generation/Contexts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/ComparisonCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/ComparisonCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/code_generation/PrintCodes.py` & `Nuitka-1.5.7/nuitka/code_generation/PrintCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/commercial/__init__.py` & `Nuitka-1.5.7/nuitka/tools/commercial/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/general/find_module/__main__.py` & `Nuitka-1.5.7/nuitka/tools/general/find_module/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/general/find_module/__init__.py` & `Nuitka-1.5.7/nuitka/tools/general/find_module/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/general/__init__.py` & `Nuitka-1.5.7/nuitka/tools/general/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/general/dll_report/__main__.py` & `Nuitka-1.5.7/nuitka/tools/general/dll_report/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/general/dll_report/__init__.py` & `Nuitka-1.5.7/nuitka/tools/general/dll_report/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/__init__.py` & `Nuitka-1.5.7/nuitka/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/onefile_compressor/__main__.py` & `Nuitka-1.5.7/nuitka/tools/onefile_compressor/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/onefile_compressor/__init__.py` & `Nuitka-1.5.7/nuitka/tools/onefile_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/onefile_compressor/OnefileCompressor.py` & `Nuitka-1.5.7/nuitka/tools/onefile_compressor/OnefileCompressor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/Basics.py` & `Nuitka-1.5.7/nuitka/tools/Basics.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/Valgrind.py` & `Nuitka-1.5.7/nuitka/tools/testing/Valgrind.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/measure_construct_performance/__main__.py` & `Nuitka-1.5.7/nuitka/tools/testing/measure_construct_performance/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/measure_construct_performance/__init__.py` & `Nuitka-1.5.7/nuitka/tools/testing/measure_construct_performance/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/SearchModes.py` & `Nuitka-1.5.7/nuitka/tools/testing/SearchModes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/__init__.py` & `Nuitka-1.5.7/nuitka/tools/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/RuntimeTracing.py` & `Nuitka-1.5.7/nuitka/tools/testing/RuntimeTracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/find_sxs_modules/__main__.py` & `Nuitka-1.5.7/nuitka/tools/testing/find_sxs_modules/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/find_sxs_modules/__init__.py` & `Nuitka-1.5.7/nuitka/tools/testing/find_sxs_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/check_reference_counts/__main__.py` & `Nuitka-1.5.7/nuitka/tools/testing/check_reference_counts/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/check_reference_counts/__init__.py` & `Nuitka-1.5.7/nuitka/tools/testing/check_reference_counts/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/Common.py` & `Nuitka-1.5.7/nuitka/tools/testing/Common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/Constructs.py` & `Nuitka-1.5.7/nuitka/tools/testing/Constructs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/Pythons.py` & `Nuitka-1.5.7/nuitka/tools/testing/Pythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/compare_with_cpython/__main__.py` & `Nuitka-1.5.7/nuitka/tools/testing/compare_with_cpython/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/compare_with_cpython/__init__.py` & `Nuitka-1.5.7/nuitka/tools/testing/compare_with_cpython/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/OutputComparison.py` & `Nuitka-1.5.7/nuitka/tools/testing/OutputComparison.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/run_nuitka_tests/__main__.py` & `Nuitka-1.5.7/nuitka/tools/testing/run_nuitka_tests/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/testing/run_nuitka_tests/__init__.py` & `Nuitka-1.5.7/nuitka/tools/testing/run_nuitka_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/data_composer/__main__.py` & `Nuitka-1.5.7/nuitka/tools/data_composer/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/data_composer/__init__.py` & `Nuitka-1.5.7/nuitka/tools/data_composer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/data_composer/DataComposer.py` & `Nuitka-1.5.7/nuitka/tools/data_composer/DataComposer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/environments/__init__.py` & `Nuitka-1.5.7/nuitka/tools/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/environments/CreateEnvironment.py` & `Nuitka-1.5.7/nuitka/tools/environments/CreateEnvironment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/environments/Virtualenv.py` & `Nuitka-1.5.7/nuitka/tools/environments/Virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/profiler/__main__.py` & `Nuitka-1.5.7/nuitka/tools/profiler/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/profiler/__init__.py` & `Nuitka-1.5.7/nuitka/tools/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/scanning/__init__.py` & `Nuitka-1.5.7/nuitka/tools/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/scanning/DisplayPackageDLLs.py` & `Nuitka-1.5.7/nuitka/tools/scanning/DisplayPackageDLLs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/scanning/DisplayPackageData.py` & `Nuitka-1.5.7/nuitka/tools/scanning/DisplayPackageData.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/specialize/SpecializePython.py` & `Nuitka-1.5.7/nuitka/tools/specialize/SpecializePython.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/specialize/__init__.py` & `Nuitka-1.5.7/nuitka/tools/specialize/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/specialize/Common.py` & `Nuitka-1.5.7/nuitka/tools/specialize/Common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/specialize/CTypeDescriptions.py` & `Nuitka-1.5.7/nuitka/tools/specialize/CTypeDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/nuitka/tools/specialize/SpecializeC.py` & `Nuitka-1.5.7/nuitka/tools/specialize/SpecializeC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/pyproject.toml` & `Nuitka-1.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/misc/nuitka.bat` & `Nuitka-1.5.7/misc/nuitka.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/misc/nuitka-run.bat` & `Nuitka-1.5.7/misc/nuitka-run.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/LICENSE.txt` & `Nuitka-1.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/lib/hints.py` & `Nuitka-1.5.7/lib/hints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/plugins/parameters/parameter-using-plugin.py` & `Nuitka-1.5.7/tests/plugins/parameters/parameter-using-plugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/plugins/parameters/ParametersMain.py` & `Nuitka-1.5.7/tests/plugins/parameters/ParametersMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/plugins/data_files/DataFilesMain.py` & `Nuitka-1.5.7/tests/plugins/data_files/DataFilesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/plugins/data_files/data_files_package/__init__.py` & `Nuitka-1.5.7/tests/plugins/data_files/data_files_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/plugins/run_all.py` & `Nuitka-1.5.7/tests/plugins/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/optimizations/Conditions.py` & `Nuitka-1.5.7/tests/optimizations/Conditions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/optimizations/Subscripts.py` & `Nuitka-1.5.7/tests/optimizations/Subscripts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/optimizations/FormatStrings36.py` & `Nuitka-1.5.7/tests/optimizations/FormatStrings36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/optimizations/Iterations.py` & `Nuitka-1.5.7/tests/optimizations/Iterations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/optimizations/ArgumentTypes.py` & `Nuitka-1.5.7/tests/optimizations/ArgumentTypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/optimizations/Operations.py` & `Nuitka-1.5.7/tests/optimizations/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/optimizations/HardImports.py` & `Nuitka-1.5.7/tests/optimizations/HardImports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/optimizations/Len.py` & `Nuitka-1.5.7/tests/optimizations/Len.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/optimizations/run_all.py` & `Nuitka-1.5.7/tests/optimizations/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/optimizations/Calls.py` & `Nuitka-1.5.7/tests/optimizations/Calls.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/optimizations/DecodingOperations.py` & `Nuitka-1.5.7/tests/optimizations/DecodingOperations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/optimizations/HardImports_2.py` & `Nuitka-1.5.7/tests/optimizations/HardImports_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/optimizations/Attributes.py` & `Nuitka-1.5.7/tests/optimizations/Attributes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/CtypesUsing.py` & `Nuitka-1.5.7/tests/standalone/CtypesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/PySide6Using.py` & `Nuitka-1.5.7/tests/standalone/PySide6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/GtkUsing.py` & `Nuitka-1.5.7/tests/standalone/GtkUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/MatplotlibUsing.py` & `Nuitka-1.5.7/tests/standalone/MatplotlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/Urllib3Using.py` & `Nuitka-1.5.7/tests/standalone/Urllib3Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/FlaskUsing.py` & `Nuitka-1.5.7/tests/standalone/FlaskUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/PandasUsing.py` & `Nuitka-1.5.7/tests/standalone/PandasUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/LxmlUsing.py` & `Nuitka-1.5.7/tests/standalone/LxmlUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/PkgResourcesRequiresUsing.py` & `Nuitka-1.5.7/tests/standalone/PkgResourcesRequiresUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/PmwUsing.py` & `Nuitka-1.5.7/tests/standalone/PmwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/IdnaUsing.py` & `Nuitka-1.5.7/tests/standalone/IdnaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/NumpyUsing.py` & `Nuitka-1.5.7/tests/standalone/NumpyUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/GlfwUsing.py` & `Nuitka-1.5.7/tests/standalone/GlfwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/ShlibUsing.py` & `Nuitka-1.5.7/tests/standalone/ShlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/zip_importer/ZipImporterMain.py` & `Nuitka-1.5.7/tests/standalone/zip_importer/ZipImporterMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/PyQt5Plugins.py` & `Nuitka-1.5.7/tests/standalone/PyQt5Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/run_all.py` & `Nuitka-1.5.7/tests/standalone/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/PyQt5SSLSupport.py` & `Nuitka-1.5.7/tests/standalone/PyQt5SSLSupport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/HexEncodingTest_2.py` & `Nuitka-1.5.7/tests/standalone/HexEncodingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/PasslibUsing.py` & `Nuitka-1.5.7/tests/standalone/PasslibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/MetadataPackagesUsing.py` & `Nuitka-1.5.7/tests/standalone/MetadataPackagesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/SocketUsing.py` & `Nuitka-1.5.7/tests/standalone/SocketUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/RsaUsing.py` & `Nuitka-1.5.7/tests/standalone/RsaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/Win32ComUsing.py` & `Nuitka-1.5.7/tests/standalone/Win32ComUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/PendulumUsing.py` & `Nuitka-1.5.7/tests/standalone/PendulumUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/BrotliUsing.py` & `Nuitka-1.5.7/tests/standalone/BrotliUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/TkInterUsing.py` & `Nuitka-1.5.7/tests/standalone/TkInterUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/PyQt6Using.py` & `Nuitka-1.5.7/tests/standalone/PyQt6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/PyQt5Using.py` & `Nuitka-1.5.7/tests/standalone/PyQt5Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/standalone/OpenGLUsing.py` & `Nuitka-1.5.7/tests/standalone/OpenGLUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/DecoratorsTest.py` & `Nuitka-1.5.7/tests/basics/DecoratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ParameterErrorsTest32.py` & `Nuitka-1.5.7/tests/basics/ParameterErrorsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/FutureTest32.py` & `Nuitka-1.5.7/tests/basics/FutureTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/AssignmentsTest.py` & `Nuitka-1.5.7/tests/basics/AssignmentsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/TryExceptFramesTest.py` & `Nuitka-1.5.7/tests/basics/TryExceptFramesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/run_xml.py` & `Nuitka-1.5.7/tests/basics/run_xml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/OperatorsTest.py` & `Nuitka-1.5.7/tests/basics/OperatorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/GlobalStatementTest.py` & `Nuitka-1.5.7/tests/basics/GlobalStatementTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/BuiltinOverload.py` & `Nuitka-1.5.7/tests/basics/BuiltinOverload.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ConstantsTest27.py` & `Nuitka-1.5.7/tests/basics/ConstantsTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ReferencingTest_2.py` & `Nuitka-1.5.7/tests/basics/ReferencingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ClassesTest.py` & `Nuitka-1.5.7/tests/basics/ClassesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ListContractionsTest.py` & `Nuitka-1.5.7/tests/basics/ListContractionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ThreadedGeneratorsTest.py` & `Nuitka-1.5.7/tests/basics/ThreadedGeneratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/VarargsTest.py` & `Nuitka-1.5.7/tests/basics/VarargsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ExceptionRaisingTest.py` & `Nuitka-1.5.7/tests/basics/ExceptionRaisingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/TryReturnFinallyTest.py` & `Nuitka-1.5.7/tests/basics/TryReturnFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ParameterErrorsTest.py` & `Nuitka-1.5.7/tests/basics/ParameterErrorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ImportingTest.py` & `Nuitka-1.5.7/tests/basics/ImportingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/RecursionTest.py` & `Nuitka-1.5.7/tests/basics/RecursionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/TryExceptContinueTest.py` & `Nuitka-1.5.7/tests/basics/TryExceptContinueTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/DefaultParametersTest.py` & `Nuitka-1.5.7/tests/basics/DefaultParametersTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ExceptionRaisingTest33.py` & `Nuitka-1.5.7/tests/basics/ExceptionRaisingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/InspectionTest_36.py` & `Nuitka-1.5.7/tests/basics/InspectionTest_36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/FunctionsTest32.py` & `Nuitka-1.5.7/tests/basics/FunctionsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ComparisonChainsTest.py` & `Nuitka-1.5.7/tests/basics/ComparisonChainsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/BuiltinSuperTest.py` & `Nuitka-1.5.7/tests/basics/BuiltinSuperTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/HelloWorldTest_2.py` & `Nuitka-1.5.7/tests/basics/HelloWorldTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/TryExceptFinallyTest.py` & `Nuitka-1.5.7/tests/basics/TryExceptFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/SlotsTest.py` & `Nuitka-1.5.7/tests/basics/SlotsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/WithStatementsTest.py` & `Nuitka-1.5.7/tests/basics/WithStatementsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/InspectionTest.py` & `Nuitka-1.5.7/tests/basics/InspectionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/TryContinueFinallyTest.py` & `Nuitka-1.5.7/tests/basics/TryContinueFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ExtremeClosureTest.py` & `Nuitka-1.5.7/tests/basics/ExtremeClosureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/PrintFutureTest.py` & `Nuitka-1.5.7/tests/basics/PrintFutureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/UnpackingTest35.py` & `Nuitka-1.5.7/tests/basics/UnpackingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ConstantsTest.py` & `Nuitka-1.5.7/tests/basics/ConstantsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/GeneratorExpressionsTest_37.py` & `Nuitka-1.5.7/tests/basics/GeneratorExpressionsTest_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/FunctionsTest.py` & `Nuitka-1.5.7/tests/basics/FunctionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/TryYieldFinallyTest.py` & `Nuitka-1.5.7/tests/basics/TryYieldFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ClassesTest34.py` & `Nuitka-1.5.7/tests/basics/ClassesTest34.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/UnicodeTest.py` & `Nuitka-1.5.7/tests/basics/UnicodeTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/OrderChecksTest27.py` & `Nuitka-1.5.7/tests/basics/OrderChecksTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/YieldFromTest33.py` & `Nuitka-1.5.7/tests/basics/YieldFromTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/OrderChecksTest.py` & `Nuitka-1.5.7/tests/basics/OrderChecksTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/DoubleDeletionsTest.py` & `Nuitka-1.5.7/tests/basics/DoubleDeletionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/GeneratorExpressionsTest.py` & `Nuitka-1.5.7/tests/basics/GeneratorExpressionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/AssignmentsTest32.py` & `Nuitka-1.5.7/tests/basics/AssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/InspectionTest_35.py` & `Nuitka-1.5.7/tests/basics/InspectionTest_35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ClassMinimalTest.py` & `Nuitka-1.5.7/tests/basics/ClassMinimalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ModuleAttributesTest.py` & `Nuitka-1.5.7/tests/basics/ModuleAttributesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/AssertsTest.py` & `Nuitka-1.5.7/tests/basics/AssertsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/PrintingTest_2.py` & `Nuitka-1.5.7/tests/basics/PrintingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/run_all.py` & `Nuitka-1.5.7/tests/basics/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/TrickAssignmentsTest_2.py` & `Nuitka-1.5.7/tests/basics/TrickAssignmentsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ReferencingTest33.py` & `Nuitka-1.5.7/tests/basics/ReferencingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/TrickAssignmentsTest32.py` & `Nuitka-1.5.7/tests/basics/TrickAssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ExecEvalTest.py` & `Nuitka-1.5.7/tests/basics/ExecEvalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ReferencingTest.py` & `Nuitka-1.5.7/tests/basics/ReferencingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/MainProgramsTest.py` & `Nuitka-1.5.7/tests/basics/MainProgramsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/BranchingTest.py` & `Nuitka-1.5.7/tests/basics/BranchingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/FunctionsTest_2.py` & `Nuitka-1.5.7/tests/basics/FunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ReferencingTest36.py` & `Nuitka-1.5.7/tests/basics/ReferencingTest36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/FunctionObjectsTest.py` & `Nuitka-1.5.7/tests/basics/FunctionObjectsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ExceptionRaisingTest32.py` & `Nuitka-1.5.7/tests/basics/ExceptionRaisingTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/InplaceOperationsTest.py` & `Nuitka-1.5.7/tests/basics/InplaceOperationsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/LateClosureAssignmentTest.py` & `Nuitka-1.5.7/tests/basics/LateClosureAssignmentTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ReferencingTest27.py` & `Nuitka-1.5.7/tests/basics/ReferencingTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/LoopingTest.py` & `Nuitka-1.5.7/tests/basics/LoopingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/EmptyModuleTest.py` & `Nuitka-1.5.7/tests/basics/EmptyModuleTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/BuiltinsTest.py` & `Nuitka-1.5.7/tests/basics/BuiltinsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ClassesTest32.py` & `Nuitka-1.5.7/tests/basics/ClassesTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/TrickAssignmentsTest35.py` & `Nuitka-1.5.7/tests/basics/TrickAssignmentsTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/ReferencingTest35.py` & `Nuitka-1.5.7/tests/basics/ReferencingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/OverflowFunctionsTest_2.py` & `Nuitka-1.5.7/tests/basics/OverflowFunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/basics/LambdasTest.py` & `Nuitka-1.5.7/tests/basics/LambdasTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/onefile/KeyboardInterruptTest.py` & `Nuitka-1.5.7/tests/onefile/KeyboardInterruptTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/onefile/HelloWorldTest.py` & `Nuitka-1.5.7/tests/onefile/HelloWorldTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/onefile/run_all.py` & `Nuitka-1.5.7/tests/onefile/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py` & `Nuitka-1.5.7/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/packages/package_import_success_after_failure/variable_package/__init__.py` & `Nuitka-1.5.7/tests/packages/package_import_success_after_failure/variable_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py` & `Nuitka-1.5.7/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/packages/sub_package/kitty/__init__.py` & `Nuitka-1.5.7/tests/packages/sub_package/kitty/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/packages/sub_package/kitty/speak/miau.py` & `Nuitka-1.5.7/tests/packages/sub_package/kitty/speak/miau.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/packages/sub_package/kitty/speak/__init__.py` & `Nuitka-1.5.7/tests/packages/sub_package/kitty/speak/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/packages/sub_package/kitty/speak/hello.py` & `Nuitka-1.5.7/tests/packages/sub_package/kitty/speak/hello.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/packages/sub_package/kitty/speak/purr.py` & `Nuitka-1.5.7/tests/packages/sub_package/kitty/speak/purr.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/packages/sub_package/kitty/smallkitty.py` & `Nuitka-1.5.7/tests/packages/sub_package/kitty/smallkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/packages/sub_package/kitty/bigkitty.py` & `Nuitka-1.5.7/tests/packages/sub_package/kitty/bigkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/packages/run_all.py` & `Nuitka-1.5.7/tests/packages/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/packages/top_level_attributes_3/some_package/__init__.py` & `Nuitka-1.5.7/tests/packages/top_level_attributes_3/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/packages/top_level_attributes_3/some_package/some_module.py` & `Nuitka-1.5.7/tests/packages/top_level_attributes_3/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/reflected/compile_itself.py` & `Nuitka-1.5.7/tests/reflected/compile_itself.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/run-tests` & `Nuitka-1.5.7/tests/run-tests`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_contains_main/__init__.py` & `Nuitka-1.5.7/tests/programs/package_contains_main/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_contains_main/local.py` & `Nuitka-1.5.7/tests/programs/package_contains_main/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_contains_main/PackageContainsMain.py` & `Nuitka-1.5.7/tests/programs/package_contains_main/PackageContainsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py` & `Nuitka-1.5.7/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_prevents_submodule/some_package/__init__.py` & `Nuitka-1.5.7/tests/programs/package_prevents_submodule/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_prevents_submodule/some_package/some_module.py` & `Nuitka-1.5.7/tests/programs/package_prevents_submodule/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/case_imports3/path2/Some_Package/__init__.py` & `Nuitka-1.5.7/tests/programs/case_imports3/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/case_imports3/path2/Some_Module.py` & `Nuitka-1.5.7/tests/programs/case_imports3/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/case_imports3/CasedImportingMain.py` & `Nuitka-1.5.7/tests/programs/case_imports3/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/case_imports3/path1/Some_Package/__init__.py` & `Nuitka-1.5.7/tests/programs/case_imports3/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/case_imports3/path1/Some_Module.py` & `Nuitka-1.5.7/tests/programs/case_imports3/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_init_import/PackageInitImportMain.py` & `Nuitka-1.5.7/tests/programs/package_init_import/PackageInitImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_init_import/some_package/__init__.py` & `Nuitka-1.5.7/tests/programs/package_init_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_init_import/some_package/PackageLocal.py` & `Nuitka-1.5.7/tests/programs/package_init_import/some_package/PackageLocal.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_missing_init/PackageMissingInitMain.py` & `Nuitka-1.5.7/tests/programs/package_missing_init/PackageMissingInitMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_missing_init/some_package/some_module.py` & `Nuitka-1.5.7/tests/programs/package_missing_init/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py` & `Nuitka-1.5.7/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/dash_main/Dash-Main.py` & `Nuitka-1.5.7/tests/programs/dash_main/Dash-Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/main_raises2/ErrorInFunctionMain.py` & `Nuitka-1.5.7/tests/programs/main_raises2/ErrorInFunctionMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/main_raises2/ErrorRaising.py` & `Nuitka-1.5.7/tests/programs/main_raises2/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/resource_reader37/ResourceReaderMain.py` & `Nuitka-1.5.7/tests/programs/resource_reader37/ResourceReaderMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/resource_reader37/some_package/__init__.py` & `Nuitka-1.5.7/tests/programs/resource_reader37/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/import_variants/ImportVariationsMain.py` & `Nuitka-1.5.7/tests/programs/import_variants/ImportVariationsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/import_variants/some_package/__init__.py` & `Nuitka-1.5.7/tests/programs/import_variants/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/import_variants/some_package/Child1.py` & `Nuitka-1.5.7/tests/programs/import_variants/some_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/import_variants/some_package/Child2.py` & `Nuitka-1.5.7/tests/programs/import_variants/some_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/import_variants/some_package/Child3.py` & `Nuitka-1.5.7/tests/programs/import_variants/some_package/Child3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/deep/DeepProgramMain.py` & `Nuitka-1.5.7/tests/programs/deep/DeepProgramMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/deep/some_package/DeepBrother.py` & `Nuitka-1.5.7/tests/programs/deep/some_package/DeepBrother.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/deep/some_package/__init__.py` & `Nuitka-1.5.7/tests/programs/deep/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/deep/some_package/DeepChild.py` & `Nuitka-1.5.7/tests/programs/deep/some_package/DeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/deep/some_package/deep_package/__init__.py` & `Nuitka-1.5.7/tests/programs/deep/some_package/deep_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/deep/some_package/deep_package/DeepDeepChild.py` & `Nuitka-1.5.7/tests/programs/deep/some_package/deep_package/DeepDeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/case_imports2/path2/Some_Package/__init__.py` & `Nuitka-1.5.7/tests/programs/case_imports2/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/case_imports2/path2/Some_Module.py` & `Nuitka-1.5.7/tests/programs/case_imports2/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/case_imports2/CasedImportingMain.py` & `Nuitka-1.5.7/tests/programs/case_imports2/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/case_imports2/path1/some_module.py` & `Nuitka-1.5.7/tests/programs/case_imports2/path1/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/case_imports2/path1/some_package/__init__.py` & `Nuitka-1.5.7/tests/programs/case_imports2/path1/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py` & `Nuitka-1.5.7/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/__init__.py` & `Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py` & `Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py` & `Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py` & `Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py` & `Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py` & `Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py` & `Nuitka-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py` & `Nuitka-1.5.7/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/multiprocessing_using/foo/__main__.py` & `Nuitka-1.5.7/tests/programs/multiprocessing_using/foo/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/multiprocessing_using/foo/__init__.py` & `Nuitka-1.5.7/tests/programs/multiprocessing_using/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/multiprocessing_using/foo/entry.py` & `Nuitka-1.5.7/tests/programs/multiprocessing_using/foo/entry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_code/PackageInitCodeMain.py` & `Nuitka-1.5.7/tests/programs/package_code/PackageInitCodeMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_code/some_package/__init__.py` & `Nuitka-1.5.7/tests/programs/package_code/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_code/some_package/SomeModule.py` & `Nuitka-1.5.7/tests/programs/package_code/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_program/PackageAsMain/__main__.py` & `Nuitka-1.5.7/tests/programs/package_program/PackageAsMain/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_program/PackageAsMain/__init__.py` & `Nuitka-1.5.7/tests/programs/package_program/PackageAsMain/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/relative_import/dircache.py` & `Nuitka-1.5.7/tests/programs/relative_import/dircache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/relative_import/RelativeImportMain.py` & `Nuitka-1.5.7/tests/programs/relative_import/RelativeImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py` & `Nuitka-1.5.7/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/module_object_replacing/SelfReplacingModule.py` & `Nuitka-1.5.7/tests/programs/module_object_replacing/SelfReplacingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/stdlib_overload/StdlibOverloadMain.py` & `Nuitka-1.5.7/tests/programs/stdlib_overload/StdlibOverloadMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/stdlib_overload/pyexpat.py` & `Nuitka-1.5.7/tests/programs/stdlib_overload/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/stdlib_overload/some_package/pyexpat.py` & `Nuitka-1.5.7/tests/programs/stdlib_overload/some_package/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/stdlib_overload/some_package/__init__.py` & `Nuitka-1.5.7/tests/programs/stdlib_overload/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/stdlib_overload/some_package/star_importing.py` & `Nuitka-1.5.7/tests/programs/stdlib_overload/some_package/star_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/stdlib_overload/some_package/normal_importing.py` & `Nuitka-1.5.7/tests/programs/stdlib_overload/some_package/normal_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/run_all.py` & `Nuitka-1.5.7/tests/programs/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/plugin_import/PluginImportMain.py` & `Nuitka-1.5.7/tests/programs/plugin_import/PluginImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/plugin_import/some_package/__init__.py` & `Nuitka-1.5.7/tests/programs/plugin_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/plugin_import/some_package/some_module.py` & `Nuitka-1.5.7/tests/programs/plugin_import/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/main_raises/ErrorRaising.py` & `Nuitka-1.5.7/tests/programs/main_raises/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/main_raises/ErrorMain.py` & `Nuitka-1.5.7/tests/programs/main_raises/ErrorMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/absolute_import/AbsoluteImportMain.py` & `Nuitka-1.5.7/tests/programs/absolute_import/AbsoluteImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/absolute_import/foobar/__init__.py` & `Nuitka-1.5.7/tests/programs/absolute_import/foobar/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/absolute_import/foobar/foobar.py` & `Nuitka-1.5.7/tests/programs/absolute_import/foobar/foobar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/absolute_import/foobar/util.py` & `Nuitka-1.5.7/tests/programs/absolute_import/foobar/util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/absolute_import/foobar/local.py` & `Nuitka-1.5.7/tests/programs/absolute_import/foobar/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/syntax_errors/SyntaxErrorsMain.py` & `Nuitka-1.5.7/tests/programs/syntax_errors/SyntaxErrorsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/syntax_errors/SyntaxErroring.py` & `Nuitka-1.5.7/tests/programs/syntax_errors/SyntaxErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/syntax_errors/IndentationErroring.py` & `Nuitka-1.5.7/tests/programs/syntax_errors/IndentationErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/unicode_bom/UnicodeBomMain.py` & `Nuitka-1.5.7/tests/programs/unicode_bom/UnicodeBomMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/unicode_bom/unicode_bom.py` & `Nuitka-1.5.7/tests/programs/unicode_bom/unicode_bom.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/named_imports/NamedImportsMain.py` & `Nuitka-1.5.7/tests/programs/named_imports/NamedImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/named_imports/some_package/__init__.py` & `Nuitka-1.5.7/tests/programs/named_imports/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/named_imports/some_package/SomeModule.py` & `Nuitka-1.5.7/tests/programs/named_imports/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/named_imports/some_package/sub_package/SomeModule.py` & `Nuitka-1.5.7/tests/programs/named_imports/some_package/sub_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/with space/Space Main.py` & `Nuitka-1.5.7/tests/programs/with space/Space Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/dash_import/DashImportMain.py` & `Nuitka-1.5.7/tests/programs/dash_import/DashImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/dash_import/dash-module.py` & `Nuitka-1.5.7/tests/programs/dash_import/dash-module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/dash_import/plus+module.py` & `Nuitka-1.5.7/tests/programs/dash_import/plus+module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/reimport_main_static/ImportItselfStaticMain.py` & `Nuitka-1.5.7/tests/programs/reimport_main_static/ImportItselfStaticMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/pkgutil_usage/PkgUtilUsageMain.py` & `Nuitka-1.5.7/tests/programs/pkgutil_usage/PkgUtilUsageMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/pkgutil_usage/package/__init__.py` & `Nuitka-1.5.7/tests/programs/pkgutil_usage/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/module_exits/ErrorExitingModule.py` & `Nuitka-1.5.7/tests/programs/module_exits/ErrorExitingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/module_exits/Main.py` & `Nuitka-1.5.7/tests/programs/module_exits/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/module_attributes/ModuleAttributesMain.py` & `Nuitka-1.5.7/tests/programs/module_attributes/ModuleAttributesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/module_attributes/package_level1/package_level2/__init__.py` & `Nuitka-1.5.7/tests/programs/module_attributes/package_level1/package_level2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py` & `Nuitka-1.5.7/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py` & `Nuitka-1.5.7/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py` & `Nuitka-1.5.7/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/module_attributes/package_level1/__init__.py` & `Nuitka-1.5.7/tests/programs/module_attributes/package_level1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/module_attributes/package_level1/Nearby1.py` & `Nuitka-1.5.7/tests/programs/module_attributes/package_level1/Nearby1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/dunderinit_imports/package/__init__.py` & `Nuitka-1.5.7/tests/programs/dunderinit_imports/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/dunderinit_imports/package/SubModule.py` & `Nuitka-1.5.7/tests/programs/dunderinit_imports/package/SubModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/dunderinit_imports/DunderInitImportsMain.py` & `Nuitka-1.5.7/tests/programs/dunderinit_imports/DunderInitImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_overload/Main.py` & `Nuitka-1.5.7/tests/programs/package_overload/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_overload/foo/__init__.py` & `Nuitka-1.5.7/tests/programs/package_overload/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_overload/foo/bar.py` & `Nuitka-1.5.7/tests/programs/package_overload/foo/bar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_overload/foo/bar2.py` & `Nuitka-1.5.7/tests/programs/package_overload/foo/bar2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py` & `Nuitka-1.5.7/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_module_collision/something.py` & `Nuitka-1.5.7/tests/programs/package_module_collision/something.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_module_collision/Something/__init__.py` & `Nuitka-1.5.7/tests/programs/package_module_collision/Something/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py` & `Nuitka-1.5.7/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_init_issue/PackageInitIssueMain.py` & `Nuitka-1.5.7/tests/programs/package_init_issue/PackageInitIssueMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_init_issue/some_package/child_package/__init__.py` & `Nuitka-1.5.7/tests/programs/package_init_issue/some_package/child_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_init_issue/some_package/child_package/SomeModule.py` & `Nuitka-1.5.7/tests/programs/package_init_issue/some_package/child_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/package_init_issue/some_package/__init__.py` & `Nuitka-1.5.7/tests/programs/package_init_issue/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/case_imports1/path2/some_module.py` & `Nuitka-1.5.7/tests/programs/case_imports1/path2/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/case_imports1/path2/some_package/__init__.py` & `Nuitka-1.5.7/tests/programs/case_imports1/path2/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/case_imports1/CasedImportingMain.py` & `Nuitka-1.5.7/tests/programs/case_imports1/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/case_imports1/path1/Some_Package/__init__.py` & `Nuitka-1.5.7/tests/programs/case_imports1/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/case_imports1/path1/Some_Module.py` & `Nuitka-1.5.7/tests/programs/case_imports1/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/cyclic_imports/CyclicImportsMain.py` & `Nuitka-1.5.7/tests/programs/cyclic_imports/CyclicImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py` & `Nuitka-1.5.7/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py` & `Nuitka-1.5.7/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py` & `Nuitka-1.5.7/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/TryExceptAllNotLast.py` & `Nuitka-1.5.7/tests/syntax/TryExceptAllNotLast.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/SyntaxError.py` & `Nuitka-1.5.7/tests/syntax/SyntaxError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/ModuleReturn.py` & `Nuitka-1.5.7/tests/syntax/ModuleReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/GlobalForParameter.py` & `Nuitka-1.5.7/tests/syntax/GlobalForParameter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/MisplacedFutureImport.py` & `Nuitka-1.5.7/tests/syntax/MisplacedFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/YieldFromInModule.py` & `Nuitka-1.5.7/tests/syntax/YieldFromInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/DuplicateArgument.py` & `Nuitka-1.5.7/tests/syntax/DuplicateArgument.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/NonlocalNotFound32.py` & `Nuitka-1.5.7/tests/syntax/NonlocalNotFound32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/StarImportExtra.py` & `Nuitka-1.5.7/tests/syntax/StarImportExtra.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/LateFutureImport.py` & `Nuitka-1.5.7/tests/syntax/LateFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/YieldInModule.py` & `Nuitka-1.5.7/tests/syntax/YieldInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/IndentationError.py` & `Nuitka-1.5.7/tests/syntax/IndentationError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/AsyncgenReturn36.py` & `Nuitka-1.5.7/tests/syntax/AsyncgenReturn36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/YieldInAsync35.py` & `Nuitka-1.5.7/tests/syntax/YieldInAsync35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/NonAsciiWithoutEncoding_2.py` & `Nuitka-1.5.7/tests/syntax/NonAsciiWithoutEncoding_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/ContinueWithoutLoop.py` & `Nuitka-1.5.7/tests/syntax/ContinueWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/GeneratorExpressions38.py` & `Nuitka-1.5.7/tests/syntax/GeneratorExpressions38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/FutureBraces.py` & `Nuitka-1.5.7/tests/syntax/FutureBraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/Importing32.py` & `Nuitka-1.5.7/tests/syntax/Importing32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/BreakWithoutLoop.py` & `Nuitka-1.5.7/tests/syntax/BreakWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/run_all.py` & `Nuitka-1.5.7/tests/syntax/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/FutureUnknown.py` & `Nuitka-1.5.7/tests/syntax/FutureUnknown.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/ExecWithNesting_2.py` & `Nuitka-1.5.7/tests/syntax/ExecWithNesting_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/YieldInGenexp38.py` & `Nuitka-1.5.7/tests/syntax/YieldInGenexp38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/UnpackTwoStars32.py` & `Nuitka-1.5.7/tests/syntax/UnpackTwoStars32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/ClosureDel_2.py` & `Nuitka-1.5.7/tests/syntax/ClosureDel_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/GeneratorReturn_2.py` & `Nuitka-1.5.7/tests/syntax/GeneratorReturn_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/UnpackNoTuple.py` & `Nuitka-1.5.7/tests/syntax/UnpackNoTuple.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/NonlocalForParameter32.py` & `Nuitka-1.5.7/tests/syntax/NonlocalForParameter32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/ClassReturn.py` & `Nuitka-1.5.7/tests/syntax/ClassReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.5.6/tests/syntax/TryFinallyContinue_37.py` & `Nuitka-1.5.7/tests/syntax/TryFinallyContinue_37.py`

 * *Files identical despite different names*

