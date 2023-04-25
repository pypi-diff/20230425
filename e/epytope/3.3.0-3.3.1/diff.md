# Comparing `tmp/epytope-3.3.0-1669976442.tar.gz` & `tmp/epytope-3.3.1-1682423381.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/epytope/epytope/dist/.tmp-v33flq0f/epytope-3.3.0.tar", last modified: Fri Dec  2 10:20:33 2022, max compression
+gzip compressed data, was "/home/runner/work/epytope/epytope/dist/.tmp-rqdw6xvk/epytope-3.3.1.tar", last modified: Tue Apr 25 11:49:30 2023, max compression
```

## Comparing `epytope-3.3.0-1669976442.tar` & `epytope-3.3.1-1682423381.tar`

### file list

```diff
@@ -1,1708 +1,1708 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (116)     4174 2022-12-02 10:20:19.000000 epytope-3.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)     1566 2022-12-02 10:20:19.000000 epytope-3.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)     5594 2022-12-02 10:20:33.000000 epytope-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4711 2022-12-02 10:20:19.000000 epytope-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/CleavagePrediction/
--rw-r--r--   0 runner    (1001) docker     (116)    12708 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/CleavagePrediction/External.py
--rw-r--r--   0 runner    (1001) docker     (116)    18011 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/CleavagePrediction/PSSM.py
--rw-r--r--   0 runner    (1001) docker     (116)     3794 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/CleavagePrediction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Core/
--rw-r--r--   0 runner    (1001) docker     (116)     4029 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Core/Allele.py
--rw-r--r--   0 runner    (1001) docker     (116)    13566 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Core/Base.py
--rw-r--r--   0 runner    (1001) docker     (116)    23014 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Core/Generator.py
--rw-r--r--   0 runner    (1001) docker     (116)    11225 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Core/Peptide.py
--rw-r--r--   0 runner    (1001) docker     (116)     4995 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Core/Protein.py
--rw-r--r--   0 runner    (1001) docker     (116)    17004 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Core/Result.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     4437 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Core/Transcript.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6408 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Core/Variant.py
--rw-r--r--   0 runner    (1001) docker     (116)      567 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Data/
--rw-r--r--   0 runner    (1001) docker     (116)    20018 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/DistanceMatrices.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Data/examples/
--rw-r--r--   0 runner    (1001) docker     (116)    61427 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/examples/Homo_sapiens.GRCh38.cds.test_stub.fa
--rw-r--r--   0 runner    (1001) docker     (116)    24260 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/examples/Homo_sapiens.GRCh38.pep.test_stub.fa
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/examples/alleles.txt
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/examples/alleles_defect.txt
--rw-r--r--   0 runner    (1001) docker     (116)      865 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/examples/testSequences.fasta
--rw-r--r--   0 runner    (1001) docker     (116)    59052 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/examples/testSequences_d2s.fasta
--rw-r--r--   0 runner    (1001) docker     (116)     1061 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/examples/test_annovar.out
--rw-r--r--   0 runner    (1001) docker     (116)    13343 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/examples/vcftestfile1.vcf
--rw-r--r--   0 runner    (1001) docker     (116)     1749 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/examples/vcftestfile2.vcf
--rw-r--r--   0 runner    (1001) docker     (116)     7631 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/examples/vcftestfile3.vcf
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Data/pssms/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Data/pssms/arb/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/
--rw-r--r--   0 runner    (1001) docker     (116)     5197 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0101_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4866 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5238 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0201_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     5300 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0201_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     4071 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0201_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     4829 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0201_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5242 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0202_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4864 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0202_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     3939 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0202_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     4752 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0202_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5262 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0203_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4847 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0203_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     3943 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0203_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     4837 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0203_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5237 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0206_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4838 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0206_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     3967 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0206_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     4785 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0206_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4760 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0211_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4795 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0212_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4779 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0216_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4797 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0219_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4384 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0250_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5223 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0301_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4853 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0301_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5234 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_1101_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4832 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_1101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2301_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4804 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2301_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2402_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4854 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2402_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4811 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2403_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4820 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2501_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5197 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2601_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4892 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2601_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4572 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2602_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4618 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2603_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5199 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2902_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4817 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2902_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4610 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3001_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4805 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3001_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5180 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3002_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4742 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3002_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5205 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3101_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4838 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4310 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3201_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4575 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3201_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5217 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3301_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4768 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3301_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5188 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_6801_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4735 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_6801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5252 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_6802_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4603 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_6802_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     3966 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_6802_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     4836 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_6802_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4877 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_6901_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4809 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/A_8001_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5150 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_0702_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     3238 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_0702_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     4865 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_0702_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5063 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_0801_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4825 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_0801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4832 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_0802_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4681 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_0803_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4840 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_1501_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4428 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_1502_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4539 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_1503_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4710 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_1509_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4776 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_1517_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5211 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_1801_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4902 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_1801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5351 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_2703_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5278 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_2705_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     5790 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_2705_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     4237 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_2705_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     4875 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_2705_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5176 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_3501_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     3205 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_3501_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     4830 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_3501_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4508 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_3801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4827 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_3901_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5215 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4001_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4863 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4001_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5191 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4002_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4670 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4002_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5244 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4402_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4909 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4402_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5246 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4403_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4694 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4403_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5266 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4501_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4689 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4501_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4903 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4601_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4859 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5134 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5101_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4832 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5126 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5301_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4683 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5301_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     5115 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5401_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4706 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5401_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4816 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5701_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4872 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5701_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4536 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5801_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     4856 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     4242 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/B_7301_9.py
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/arb/mat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Data/pssms/bimas/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/
--rw-r--r--   0 runner    (1001) docker     (116)     2299 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_0101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2710 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_0201_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2640 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_0205_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2583 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_0301_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2391 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_1101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2330 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_2402_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2427 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_3101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2140 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_3302_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2311 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_6801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2346 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_0401_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2271 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_0702_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_0801_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2377 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_0801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2459 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_1501_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2276 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_2702_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2046 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_2705_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2251 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_2705_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2071 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_3501_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2276 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_3501_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2116 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_3701_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2277 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_3801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2081 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_3901_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2286 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_3901_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2155 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_3902_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2402 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_4001_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_4006_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2365 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_4006_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2339 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_40_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2398 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_4403_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2349 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_5101_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2566 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_5101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2347 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_5102_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2596 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_5102_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2483 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_5103_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2309 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_5201_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2554 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_5201_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2510 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_5801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2331 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/C_0301_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2363 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/C_0401_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2280 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/C_0602_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2340 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/C_0702_9.py
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/bimas/mat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A0101.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A0201.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A0202.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A0203.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A0206.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A0211.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A0301.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A1101.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A2301.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A2402.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A2601.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A2902.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A3001.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A3002.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A3101.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A3201.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A3301.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A6801.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A6802.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/A6901.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B0702.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B0801.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B1501.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B1502.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B1801.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B2705.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B3501.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B3901.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B4001.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B4002.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B4402.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B4403.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B4501.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B4601.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B5101.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B5301.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B5401.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B5701.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/B5801.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/calisimm/mat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/
--rw-r--r--   0 runner    (1001) docker     (116)     2272 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/A_0201_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2265 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/A_3001_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2241 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/A_3201_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2260 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/A_6802_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2275 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_0702_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2272 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_0801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2237 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_1501_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2260 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_1503_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2245 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_2705_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2270 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_3501_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2250 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_5101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2288 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_5301_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2312 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_5401_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2255 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_5801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2266 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_5802_9.py
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Data/pssms/doytchinova/
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/doytchinova/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Data/pssms/doytchinova/mat/
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/doytchinova/mat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2267 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/doytchinova/mat/doytchinova_9.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/
--rw-r--r--   0 runner    (1001) docker     (116)     1969 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_0201_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2408 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_0201_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1948 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_0201_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2183 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_03_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1963 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2192 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_1101_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1964 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_1101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1956 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_2402_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1965 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_24_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2187 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_25_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1979 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_25_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1960 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_07_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1759 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_08_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1960 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_08_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1746 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_1801_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1962 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_1801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1965 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_2705_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2190 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_27_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1959 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_27_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1964 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_3701_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1968 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_44_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1764 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_5101_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1967 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_5101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/epidemix/mat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope/Data/pssms/ginodi/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/ginodi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/ginodi/mat/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/ginodi/mat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1599 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/ginodi/mat/ginodi_11.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/hammer/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/
--rw-r--r--   0 runner    (1001) docker     (116)     1967 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1965 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0102_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1950 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0301_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1956 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0305_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1954 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0306_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1954 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0307_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1954 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0308_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1951 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0309_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1954 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0311_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1957 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0401_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1953 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0402_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1963 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0404_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1956 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0405_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1964 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0408_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1955 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0410_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1952 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0421_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1963 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0423_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1957 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0426_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1949 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0701_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1949 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0703_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1953 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1961 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0802_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1960 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0804_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1952 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0806_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1957 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0813_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1951 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0817_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1963 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1952 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1102_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1962 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1104_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1962 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1106_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1955 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1107_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1953 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1114_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1948 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1120_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1952 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1121_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1958 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1128_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1947 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1301_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1948 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1302_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1944 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1304_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1958 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1305_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1965 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1307_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1962 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1311_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1955 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1321_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1952 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1322_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1953 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1323_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1947 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1327_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1947 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1328_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1947 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1501_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1948 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1502_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1947 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1506_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1949 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB5_0101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1949 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB5_0105_9.py
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/hammer/mat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/pcm/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/pcm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/pcm/mat/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/pcm/mat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1407 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/pcm/mat/pcm_6.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/proteasmm_c/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/proteasmm_c/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/proteasmm_c/mat/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/proteasmm_c/mat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3364 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/proteasmm_c/mat/proteasmm_c_10.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/proteasmm_i/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/proteasmm_i/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/proteasmm_i/mat/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/proteasmm_i/mat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3341 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/proteasmm_i/mat/proteasmm_i_10.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/smm/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/
--rw-r--r--   0 runner    (1001) docker     (116)     2517 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_01_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2737 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_01_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1963 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_01_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2303 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_01_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2568 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2727 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1981 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2306 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2574 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_02_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2648 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_02_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1973 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_02_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2302 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2567 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_03_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2663 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_03_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1991 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_03_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2310 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2561 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_06_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2729 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_06_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1992 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_06_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2315 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_06_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2312 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_11_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2305 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_12_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2303 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_16_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2422 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_17_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2226 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_17_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2303 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_19_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_50_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2562 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_03_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2761 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_03_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1818 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_03_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2306 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_03_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2569 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_11_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2718 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_11_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1985 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_11_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2299 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_11_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2503 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_23_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2639 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_23_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1990 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_23_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2292 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_23_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2557 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_24_02_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2686 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_24_02_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1996 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_24_02_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2308 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_24_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2308 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_24_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2278 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_25_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2565 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_26_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2488 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_26_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1864 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_26_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2308 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_26_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2297 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_26_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2291 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_26_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2538 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_29_02_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2686 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_29_02_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1880 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_29_02_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2308 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_29_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2556 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_30_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2303 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_30_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2509 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_30_02_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2649 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_30_02_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1844 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_30_02_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2260 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_30_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2562 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_31_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2671 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_31_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2312 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_31_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2545 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_32_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2307 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_32_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2145 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_32_07_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2118 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_32_15_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2541 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_33_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2301 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_33_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2154 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_66_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2554 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_68_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2299 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_68_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2565 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_68_02_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2526 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_68_02_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2011 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_68_02_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2311 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_68_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2155 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_68_23_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2299 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_69_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2296 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/A_80_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2553 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_07_02_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2674 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_07_02_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2014 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_07_02_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2293 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_07_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2535 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_08_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2548 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_08_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1979 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_08_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2312 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_08_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2280 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_08_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2231 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_08_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2276 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_14_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2526 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_15_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2289 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_15_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2204 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_15_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2485 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_15_03_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2308 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_15_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2259 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_15_09_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2303 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_15_17_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2054 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_15_42_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2539 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_18_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2716 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_18_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1917 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_18_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2307 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_18_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2558 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_27_05_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2804 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_27_05_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2044 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_27_05_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2314 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_27_05_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_27_20_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2539 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_35_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2620 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_35_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1995 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_35_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2307 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_35_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2469 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_35_03_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2259 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_35_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2300 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_38_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2311 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_39_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2537 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_40_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1906 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_40_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2310 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_40_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2506 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_40_02_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2579 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_40_02_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1917 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_40_02_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2281 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_40_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2101 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_40_13_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2465 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_42_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2259 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_42_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2529 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_44_02_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1865 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_44_02_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2287 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_44_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2477 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_44_03_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2678 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_44_03_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1890 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_44_03_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2296 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_44_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2527 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_45_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2630 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_45_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1952 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_45_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2251 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_45_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2297 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_46_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2278 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_48_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2556 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_51_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2589 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_51_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1997 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_51_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2293 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_51_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2548 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_53_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2636 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_53_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1934 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_53_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2302 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_53_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2530 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_54_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1971 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_54_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2290 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_54_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2513 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_57_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2672 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_57_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2298 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_57_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2529 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_58_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2640 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_58_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2314 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_58_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2184 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_58_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2225 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_73_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/B_83_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2235 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/C_03_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/C_04_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2221 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/C_05_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2272 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/C_06_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2248 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/C_07_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2238 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/C_07_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2187 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/C_08_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2154 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/C_12_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/C_14_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2215 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/C_15_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2188 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/E_01_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2102 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/E_01_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smm/mat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/
--rw-r--r--   0 runner    (1001) docker     (116)     2557 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_01_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2808 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_01_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2049 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_01_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2311 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_01_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2558 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2802 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2049 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2294 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2562 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_02_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2819 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_02_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2049 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_02_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2306 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2557 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_03_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2811 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_03_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2045 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_03_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2305 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2571 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_06_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2803 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_06_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2055 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_06_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2315 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_06_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2305 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_11_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2312 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_12_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2307 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_16_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2569 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_17_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2301 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_17_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2312 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_19_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2312 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_50_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2562 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_03_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2801 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_03_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1940 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_03_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2321 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_03_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2556 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_11_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2816 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_11_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2048 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_11_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2303 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_11_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2544 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_23_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2815 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_23_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2048 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_23_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2296 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_23_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2551 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_24_02_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2811 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_24_02_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2044 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_24_02_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2294 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_24_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2297 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_24_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2298 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_25_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2567 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_26_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2809 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_26_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2049 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_26_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2307 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_26_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2298 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_26_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2294 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_26_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2558 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_29_02_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2807 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_29_02_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2048 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_29_02_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2303 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_29_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2548 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_30_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2312 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_30_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2557 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_30_02_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2802 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_30_02_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2048 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_30_02_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2298 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_30_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2554 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_31_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2802 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_31_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2307 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_31_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2563 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_32_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2305 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_32_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2285 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_32_07_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2317 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_32_15_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2547 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_33_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2304 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_33_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2295 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_66_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2559 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_68_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2308 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_68_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2563 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_68_02_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2783 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_68_02_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2033 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_68_02_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2307 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_68_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2300 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_68_23_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2303 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_69_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2298 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_80_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2549 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_07_02_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2816 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_07_02_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2056 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_07_02_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2309 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_07_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2554 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_08_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2807 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_08_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2042 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_08_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2305 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_08_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2306 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_08_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2300 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_08_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2302 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_14_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2547 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_15_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2308 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_15_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2289 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_15_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2544 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_15_03_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2303 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_15_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2313 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_15_09_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2307 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_15_17_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2270 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_15_42_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2562 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_18_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2804 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_18_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2058 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_18_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2300 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_18_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2562 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_27_05_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2818 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_27_05_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2060 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_27_05_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2301 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_27_05_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2326 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_27_20_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2555 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_35_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2802 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_35_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2051 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_35_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2308 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_35_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2552 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_35_03_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2317 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_35_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2303 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_38_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2306 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_39_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2568 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_40_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2035 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_40_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2301 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_40_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2566 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_40_02_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2807 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_40_02_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2049 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_40_02_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2296 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_40_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2274 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_40_13_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2558 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_42_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2310 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_42_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2559 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_44_02_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2044 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_44_02_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2299 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_44_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2552 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_44_03_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2811 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_44_03_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2047 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_44_03_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2308 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_44_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2558 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_45_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2791 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_45_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2050 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_45_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2299 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_45_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2298 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_46_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2310 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_48_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2562 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_51_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2812 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_51_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2046 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_51_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2304 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_51_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2551 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_53_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2810 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_53_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2047 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_53_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2315 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_53_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2548 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_54_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2051 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_54_01_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     2306 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_54_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2552 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_57_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2805 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_57_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2297 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_57_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2558 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_58_01_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     2812 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_58_01_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2314 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_58_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2296 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_58_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2305 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_73_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2309 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_83_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2306 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_03_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2304 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_04_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2318 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_05_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2319 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_06_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2313 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_07_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2309 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_07_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2302 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_08_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2286 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_12_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2301 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_14_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2300 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_15_02_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2305 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/E_01_01_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2312 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/E_01_03_9.py
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/smmtap/
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmtap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/smmtap/mat/
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmtap/mat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2110 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/smmtap/mat/smmtap_9.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/
--rw-r--r--   0 runner    (1001) docker     (116)     1744 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0101_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1918 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0101_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     2093 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0101_12.py
--rw-r--r--   0 runner    (1001) docker     (116)     2267 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0101_13.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1754 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0201_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1928 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0201_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1580 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0201_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1747 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0301_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1921 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0301_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1573 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0301_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1746 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_1101_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1920 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_1101_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1572 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_1101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1749 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_2402_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1923 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_2402_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1575 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_2402_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1745 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_2601_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1919 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_2601_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1571 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_2601_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1743 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3101_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1917 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3101_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1569 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1761 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3201_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1933 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3201_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1579 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3201_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1743 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3303_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1917 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3303_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1569 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3303_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1745 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_6601_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1573 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_6601_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1754 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_6801_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1928 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_6801_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1580 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_6801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1744 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_0702_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1918 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_0702_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_0702_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1398 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_0801_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1571 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_0801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1746 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1302_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1572 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1302_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1397 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1402_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1402_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1750 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1501_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1576 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1501_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1510_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1575 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1516_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1398 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1801_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1578 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1747 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_2705_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1573 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_2705_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_2709_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1745 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3501_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1571 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3501_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1748 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3701_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1401 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3701_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1576 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3701_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1747 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3801_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1576 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1745 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3901_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1571 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3901_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1749 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3902_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1575 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3902_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1744 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4001_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4001_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4002_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1744 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4101_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1747 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4402_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1921 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4402_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1573 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4402_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1745 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4501_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1571 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4501_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1744 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4701_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4701_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1757 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4901_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1583 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4901_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1744 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5001_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5001_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1398 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5101_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1571 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1746 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5301_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1572 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5301_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1745 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5701_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1571 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5701_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1747 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5801_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1921 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5801_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1403 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5801_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1578 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1750 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5802_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1923 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5802_11.py
--rw-r--r--   0 runner    (1001) docker     (116)     1402 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5802_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1577 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5802_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1744 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0102_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1397 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0102_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0102_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1745 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0202_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1398 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0202_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1572 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0202_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1744 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0303_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1398 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0303_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0303_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1744 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0304_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1399 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0304_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0304_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1745 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0401_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1397 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0401_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1571 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0401_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1745 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0501_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1397 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0501_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0501_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1572 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0601_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1746 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0602_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1398 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0602_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1571 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0602_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1745 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0701_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1399 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0701_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1572 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0701_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1746 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0702_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1399 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0702_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1573 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0702_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1744 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0802_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1397 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0802_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0802_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1746 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1203_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1399 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1203_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1572 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1203_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1746 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1402_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1399 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1402_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1572 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1402_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1746 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1502_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1399 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1502_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1573 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1502_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1746 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1601_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1400 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1601_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1572 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1601_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1748 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1701_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1397 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1701_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1701_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1574 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/DRB1_0101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1576 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/DRB1_0301_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1574 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/DRB1_0701_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1574 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/DRB1_1101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1578 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/DRB1_1501_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1744 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/G_0101_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1397 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/G_0101_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1571 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/G_0101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1757 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/H2_Db_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1583 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/H2_Db_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1397 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/H2_Kb_8.py
--rw-r--r--   0 runner    (1001) docker     (116)     1744 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/H2_Kd_10.py
--rw-r--r--   0 runner    (1001) docker     (116)     1576 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/H2_Kd_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/H2_Ld_9.py
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0102_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2144 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0103_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0104_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0105_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2153 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0106_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0107_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0108_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2152 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0109_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0110_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0111_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0112_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0113_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2155 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0114_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2154 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0115_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2153 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0116_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2150 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0117_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0118_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0119_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0120_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2153 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0121_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0122_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0123_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0124_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0125_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0126_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0127_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0128_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2155 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0129_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0130_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0131_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0132_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0134_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0135_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0136_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0301_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0302_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0303_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2175 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0304_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0305_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2178 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0306_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0307_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0308_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0309_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0310_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0311_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2180 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0312_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0313_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0314_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0315_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2180 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0316_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0317_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0318_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2175 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0319_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0320_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0321_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0322_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0323_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0324_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0325_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2178 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0326_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0327_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0328_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0329_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0330_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2176 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0331_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0332_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0333_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0334_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0335_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0336_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0337_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0338_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0339_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0340_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0341_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0342_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0343_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0344_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0345_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0346_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0347_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0348_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0349_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0350_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0351_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0352_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0353_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0354_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0355_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2176 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0356_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0357_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0358_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0359_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2178 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0360_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0361_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0362_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0363_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0364_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2153 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0401_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2149 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0402_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0403_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0404_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0405_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0406_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2155 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0407_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0408_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0409_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0410_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0411_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0412_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2154 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0413_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2148 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0414_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0415_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2153 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0416_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0417_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0418_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0419_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0420_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0421_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0422_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0423_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0424_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0425_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2153 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0426_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0427_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0428_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0429_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0430_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0431_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0432_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2153 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0433_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2154 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0434_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2155 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0435_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0436_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0437_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2154 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0438_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0439_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0440_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0441_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0442_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0443_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0444_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0445_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0446_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0447_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0448_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0449_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0450_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0451_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0452_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0453_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0454_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0455_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0456_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0457_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0458_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0459_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0460_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0461_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2155 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0462_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2153 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0463_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2154 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0464_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0465_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0466_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0467_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0468_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0469_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0470_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0471_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2153 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0472_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0473_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2155 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0474_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0475_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2153 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0476_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0477_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0478_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0479_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0480_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0482_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0483_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0484_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0485_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0486_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0487_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0488_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0489_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0490_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0491_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2155 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0492_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0493_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0495_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0496_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0497_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2155 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0498_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2111 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0701_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2111 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0703_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2112 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0704_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2111 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0705_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2132 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0706_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2111 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0707_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2133 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0708_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2134 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0709_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2112 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0711_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2128 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0712_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2111 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0713_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2111 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0714_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2111 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0715_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2111 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0716_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2111 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0717_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2111 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0718_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2111 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0719_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2108 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0720_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2111 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0721_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0801_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0802_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0803_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0804_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0805_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0806_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0807_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0808_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0809_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0810_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0811_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0812_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0813_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0814_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0815_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0816_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0817_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0818_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0819_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0820_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0821_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0822_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0823_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0824_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0825_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0826_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0827_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0828_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0829_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0830_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0831_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0832_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0833_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0834_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0835_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0836_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0837_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0838_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0839_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0840_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0841_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0842_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0843_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0844_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0845_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2137 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0901_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2139 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0902_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2140 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0903_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2140 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0904_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2138 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0905_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2138 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0906_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2138 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0907_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2141 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0908_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2137 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0909_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2117 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0910_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2137 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0911_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2137 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0912_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1001_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1002_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1003_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1102_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1103_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1104_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1105_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1106_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1107_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1108_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1109_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1110_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1111_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1112_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1113_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1114_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1115_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1116_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1117_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1118_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1119_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1120_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1121_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2149 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1122_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1123_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1124_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1125_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1126_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1127_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1128_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1129_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1130_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1131_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1132_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1133_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1134_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1135_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1136_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1137_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1138_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1139_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1140_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1141_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1142_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1143_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1144_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1145_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1146_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1147_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1148_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1149_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1150_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1151_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1152_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1153_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1154_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1155_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1156_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1157_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1158_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1159_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1160_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1161_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1162_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1163_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1164_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1165_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1166_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1167_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1168_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1169_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1170_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1172_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1173_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1174_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1175_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1176_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1177_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1178_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1179_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1180_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1181_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1182_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1183_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1184_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1185_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2153 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1186_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1187_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1188_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1189_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1190_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1191_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1192_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1193_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1194_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1195_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1196_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1197_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1198_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1199_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1201_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1202_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1203_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1204_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1205_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1206_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1207_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1208_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1209_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1210_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1211_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1212_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1213_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1214_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1215_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1216_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1217_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1218_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1219_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1220_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1221_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1222_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1223_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1225_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1226_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1227_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1301_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1302_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1303_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1304_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1305_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1306_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1307_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1308_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1309_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1310_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1311_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1312_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1313_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1314_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1315_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2155 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1316_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2153 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1317_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1318_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1319_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1320_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1321_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1322_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1323_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1324_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2152 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1325_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1326_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1327_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1328_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1329_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1330_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1331_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1332_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1333_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1334_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1335_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1336_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1337_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1338_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1339_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1340_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1341_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1342_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1343_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1344_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2148 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1345_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1346_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1347_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1348_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1349_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1350_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1351_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1352_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1353_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1354_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1355_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1356_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1357_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1358_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1359_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1360_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1361_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1362_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1363_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1364_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1365_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1366_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1367_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1368_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1369_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1370_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1371_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1372_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1373_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1374_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1375_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1376_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1377_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1378_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1379_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1380_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1381_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1382_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1383_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1384_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1385_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1386_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1387_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1388_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1389_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1390_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1391_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1392_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1393_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1394_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1395_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1396_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1397_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1398_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1399_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1401_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1402_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1403_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1404_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1405_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1406_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1407_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1408_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1409_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1410_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1411_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1412_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1413_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1414_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1415_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1416_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1417_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1418_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2175 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1419_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1420_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1421_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1422_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1423_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1424_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1425_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1426_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1427_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1428_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1429_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1430_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1431_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1432_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1433_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1434_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1435_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1436_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1437_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1438_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1439_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1440_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1441_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1442_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1443_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1444_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1445_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1446_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1447_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1448_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1449_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1450_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1451_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1452_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1453_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1454_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1455_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1456_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1457_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1458_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1459_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1460_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1461_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1462_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1463_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1464_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1465_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1467_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1468_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1469_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2177 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1470_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1471_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1472_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1473_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1474_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1475_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2177 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1476_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1477_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1478_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1479_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1480_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1481_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1482_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1483_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1484_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1485_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1486_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1487_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1488_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1489_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1490_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2175 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1491_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1493_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1494_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1495_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1496_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1497_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1498_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1499_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1501_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2150 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1502_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1503_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2153 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1504_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1505_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1506_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2154 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1507_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2150 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1508_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1509_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1510_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2153 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1511_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2154 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1512_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1513_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2150 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1514_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2152 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1515_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1516_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2155 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1518_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2150 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1519_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1520_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1521_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1522_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2155 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1523_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1524_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1525_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2150 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1526_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1527_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2154 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1528_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2153 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1529_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2149 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1530_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2155 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1531_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1532_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1533_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1534_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1535_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1536_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1537_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2152 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1538_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2150 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1539_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1540_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1541_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1542_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1543_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2150 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1544_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1545_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1546_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2150 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1547_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2154 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1548_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2154 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1549_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1551_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1552_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1553_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1554_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1555_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1556_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1557_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1601_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1602_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1603_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1604_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1605_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1607_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1608_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1609_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1610_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1611_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1612_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1614_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1615_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1616_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1617_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1618_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0102_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0103_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0104_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2179 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0105_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0106_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0107_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0108_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0109_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0110_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0111_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0112_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2176 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0113_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2178 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0114_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2175 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0115_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0201_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0202_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0203_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0204_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0205_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2155 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0206_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0207_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0208_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0209_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0210_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0211_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0212_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0213_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0214_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0215_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0216_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0217_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0218_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0219_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0220_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0221_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0222_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0223_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2166 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0224_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0225_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0226_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0227_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0228_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0301_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2169 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0302_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0303_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB4_0101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB4_0103_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB4_0104_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB4_0105_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB4_0106_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB4_0107_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB4_0108_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2134 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0101_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2138 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0102_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2134 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0104_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2134 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0105_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2096 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0106_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2124 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0107_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2138 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0108_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2122 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0109_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2095 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0111_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2136 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0112_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2134 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0113_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2140 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0114_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2134 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0202_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2133 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0203_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2140 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0204_9.py
--rw-r--r--   0 runner    (1001) docker     (116)     2138 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0205_9.py
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/supportedAlleles/
--rw-r--r--   0 runner    (1001) docker     (116)       28 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/supportedAlleles/ann/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/ann/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1289 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/ann/mhcflurry_1_2_2.py
--rw-r--r--   0 runner    (1001) docker     (116)     1289 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/ann/mhcflurry_1_4_3.py
--rw-r--r--   0 runner    (1001) docker     (116)     1961 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/ann/mhcnuggets_class_1_2_0.py
--rw-r--r--   0 runner    (1001) docker     (116)     1643 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/ann/mhcnuggets_class_1_2_3_2.py
--rw-r--r--   0 runner    (1001) docker     (116)     3090 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/ann/mhcnuggets_class_2_2_0.py
--rw-r--r--   0 runner    (1001) docker     (116)     2395 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/ann/mhcnuggets_class_2_2_3_2.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    44431 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/netMHCstabpan_1_0.py
--rw-r--r--   0 runner    (1001) docker     (116)    44375 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/netctlpan_1_1.py
--rw-r--r--   0 runner    (1001) docker     (116)      647 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcII_2_2.py
--rw-r--r--   0 runner    (1001) docker     (116)     1394 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcII_2_3.py
--rw-r--r--   0 runner    (1001) docker     (116)   156318 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcIIpan_3_0.py
--rw-r--r--   0 runner    (1001) docker     (116)   156318 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcIIpan_3_1.py
--rw-r--r--   0 runner    (1001) docker     (116)   156384 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcIIpan_4_0.py
--rw-r--r--   0 runner    (1001) docker     (116)      864 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhc_3_0.py
--rw-r--r--   0 runner    (1001) docker     (116)     1524 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhc_3_4.py
--rw-r--r--   0 runner    (1001) docker     (116)     1420 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhc_4_0.py
--rw-r--r--   0 runner    (1001) docker     (116)    44405 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcpan_2_4.py
--rw-r--r--   0 runner    (1001) docker     (116)    44405 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcpan_2_8.py
--rw-r--r--   0 runner    (1001) docker     (116)    44427 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcpan_3_0.py
--rw-r--r--   0 runner    (1001) docker     (116)    66517 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcpan_4_0.py
--rw-r--r--   0 runner    (1001) docker     (116)   161708 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcpan_4_1.py
--rw-r--r--   0 runner    (1001) docker     (116)    44406 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/external/pickpocket_1_1.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/Data/supportedAlleles/pssm/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/pssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      876 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/pssm/arb_1_0.py
--rw-r--r--   0 runner    (1001) docker     (116)      638 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/pssm/bimas_1_0.py
--rw-r--r--   0 runner    (1001) docker     (116)      611 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/pssm/calisimm_1_0.py
--rw-r--r--   0 runner    (1001) docker     (116)      256 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/pssm/comblibsidney_1_0.py
--rw-r--r--   0 runner    (1001) docker     (116)      350 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/pssm/epidemix_1_0.py
--rw-r--r--   0 runner    (1001) docker     (116)      943 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/pssm/hammer_1_0.py
--rw-r--r--   0 runner    (1001) docker     (116)     1228 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/pssm/smm_1_0.py
--rw-r--r--   0 runner    (1001) docker     (116)     1271 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/pssm/smmpmbec_1_0.py
--rw-r--r--   0 runner    (1001) docker     (116)     1251 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/pssm/syfpeithi_1_0.py
--rw-r--r--   0 runner    (1001) docker     (116)    13241 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/Data/supportedAlleles/pssm/tepitopepan_1_0.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/EpitopeAssembly/
--rw-r--r--   0 runner    (1001) docker     (116)    47830 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/EpitopeAssembly/EpitopeAssembly.py
--rw-r--r--   0 runner    (1001) docker     (116)       78 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/EpitopeAssembly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/EpitopePrediction/
--rw-r--r--   0 runner    (1001) docker     (116)    36337 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/EpitopePrediction/ANN.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    77738 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/EpitopePrediction/External.py
--rw-r--r--   0 runner    (1001) docker     (116)    31229 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/EpitopePrediction/PSSM.py
--rw-r--r--   0 runner    (1001) docker     (116)     2202 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/EpitopePrediction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/EpitopeSelection/
--rw-r--r--   0 runner    (1001) docker     (116)    17795 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/EpitopeSelection/OptiTope.py
--rw-r--r--   0 runner    (1001) docker     (116)       48 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/EpitopeSelection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/HLAtyping/
--rw-r--r--   0 runner    (1001) docker     (116)    18107 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/HLAtyping/External.py
--rw-r--r--   0 runner    (1001) docker     (116)     1627 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/HLAtyping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/IO/
--rw-r--r--   0 runner    (1001) docker     (116)     2619 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/IO/ADBAdapter.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    12575 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/IO/EnsemblAdapter.py
--rw-r--r--   0 runner    (1001) docker     (116)    13806 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/IO/FileReader.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    47054 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/IO/MartsAdapter.py
--rw-r--r--   0 runner    (1001) docker     (116)     3596 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/IO/RefSeqAdapter.py
--rw-r--r--   0 runner    (1001) docker     (116)     6703 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/IO/UniProtAdapter.py
--rw-r--r--   0 runner    (1001) docker     (116)      531 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/IO/Utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      561 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/IO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/TAPPrediction/
--rw-r--r--   0 runner    (1001) docker     (116)     6262 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/TAPPrediction/PSSM.py
--rw-r--r--   0 runner    (1001) docker     (116)     1963 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/TAPPrediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      136 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/test/
--rw-r--r--   0 runner    (1001) docker     (116)     1607 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/DummyAdapter.py
--rw-r--r--   0 runner    (1001) docker     (116)      761 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/DummyEpitopePredictor.py
--rw-r--r--   0 runner    (1001) docker     (116)     1393 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/TestAllele.py
--rw-r--r--   0 runner    (1001) docker     (116)     1574 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/TestCleavagePrediction.py
--rw-r--r--   0 runner    (1001) docker     (116)     1993 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/TestEpitopeAssembly.py
--rw-r--r--   0 runner    (1001) docker     (116)     2360 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/TestEpitopePrediction.py
--rw-r--r--   0 runner    (1001) docker     (116)    12430 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/TestGenerator.py
--rw-r--r--   0 runner    (1001) docker     (116)    22469 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/TestIO.py
--rw-r--r--   0 runner    (1001) docker     (116)     2593 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/TestOptiTope.py
--rw-r--r--   0 runner    (1001) docker     (116)     3985 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/TestPeptide.py
--rw-r--r--   0 runner    (1001) docker     (116)     3641 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/TestPredictionVersioning.py
--rw-r--r--   0 runner    (1001) docker     (116)     8563 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/TestProtein.py
--rw-r--r--   0 runner    (1001) docker     (116)     2231 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/TestSpacerDesign.py
--rw-r--r--   0 runner    (1001) docker     (116)     1341 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/TestTAPPrediction.py
--rw-r--r--   0 runner    (1001) docker     (116)     5416 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/TestTranscript.py
--rw-r--r--   0 runner    (1001) docker     (116)     1140 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/TestVariant.py
--rw-r--r--   0 runner    (1001) docker     (116)    12323 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/VariantsForTesting.py
--rw-r--r--   0 runner    (1001) docker     (116)       85 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:33.000000 epytope-3.3.0/epytope/test/external/
--rw-r--r--   0 runner    (1001) docker     (116)     1551 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/external/TestExternalCleavagePrediction.py
--rw-r--r--   0 runner    (1001) docker     (116)     7178 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/external/TestExternalEpitopePrediction.py
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-02 10:20:19.000000 epytope-3.3.0/epytope/test/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5594 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    75760 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      139 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2022-12-02 10:20:32.000000 epytope-3.3.0/epytope.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-12-02 10:20:33.000000 epytope-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     4213 2022-12-02 10:20:19.000000 epytope-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-25 11:49:15.000000 epytope-3.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-25 11:49:15.000000 epytope-3.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-04-25 11:49:30.000000 epytope-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-04-25 11:49:15.000000 epytope-3.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/CleavagePrediction/
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/CleavagePrediction/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/CleavagePrediction/PSSM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/CleavagePrediction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Core/Allele.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Core/Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Core/Generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11225 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Core/Peptide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Core/Protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17004 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Core/Result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4437 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Core/Transcript.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6408 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Core/Variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20018 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/DistanceMatrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    61427 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/examples/Homo_sapiens.GRCh38.cds.test_stub.fa
+-rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/examples/Homo_sapiens.GRCh38.pep.test_stub.fa
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/examples/alleles.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/examples/alleles_defect.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/examples/testSequences.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    59052 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/examples/testSequences_d2s.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/examples/test_annovar.out
+-rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/examples/vcftestfile1.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/examples/vcftestfile2.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/examples/vcftestfile3.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/arb/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0101_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0201_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0201_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0201_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0201_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0202_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0202_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0202_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0202_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0203_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0203_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0203_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0203_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0206_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0206_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0206_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0206_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0211_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0212_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0216_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0219_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0250_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0301_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0301_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_1101_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_1101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2301_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2301_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2402_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2402_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2403_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2501_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2601_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2601_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2602_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2603_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2902_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2902_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3001_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3001_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3002_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3002_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3101_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3201_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3201_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3301_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3301_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_6801_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_6801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_6802_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_6802_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_6802_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_6802_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_6901_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/A_8001_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_0702_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_0702_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_0702_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_0801_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_0801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_0802_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_0803_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_1501_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_1502_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_1503_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_1509_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_1517_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_1801_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_1801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_2703_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_2705_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_2705_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_2705_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_2705_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_3501_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_3501_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_3501_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_3801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_3901_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4001_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4001_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4002_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4002_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4402_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4402_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4403_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4403_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4501_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4501_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4601_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5101_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5301_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5301_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5401_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5401_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5701_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5701_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5801_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/B_7301_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/arb/mat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/bimas/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_0101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_0201_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_0205_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_0301_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_1101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_2402_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_3101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_3302_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_6801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_0401_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_0702_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_0801_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_0801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_1501_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_2702_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_2705_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_2705_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_3501_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_3501_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_3701_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_3801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_3901_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_3901_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_3902_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_4001_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_4006_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_4006_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_40_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_4403_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_5101_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_5101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_5102_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_5102_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_5103_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_5201_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_5201_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_5801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/C_0301_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/C_0401_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/C_0602_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/C_0702_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/bimas/mat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A0101.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A0201.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A0202.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A0203.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A0206.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A0211.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A0301.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A1101.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A2301.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A2402.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A2601.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A2902.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A3001.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A3002.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A3101.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A3201.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A3301.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A6801.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A6802.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/A6901.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B0702.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B0801.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B1501.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B1502.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B1801.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B2705.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B3501.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B3901.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B4001.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B4002.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B4402.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B4403.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B4501.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B4601.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B5101.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B5301.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B5401.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B5701.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/B5801.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/calisimm/mat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/A_0201_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/A_3001_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/A_3201_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/A_6802_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_0702_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_0801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_1501_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_1503_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_2705_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_3501_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_5101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_5301_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_5401_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_5801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_5802_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/doytchinova/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/doytchinova/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/doytchinova/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/doytchinova/mat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/doytchinova/mat/doytchinova_9.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_0201_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_0201_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_0201_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_03_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_1101_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_1101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_2402_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_24_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_25_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_25_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_07_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_08_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_08_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_1801_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_1801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_2705_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_27_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_27_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_3701_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_44_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_5101_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_5101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/epidemix/mat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/ginodi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/ginodi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/ginodi/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/ginodi/mat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/ginodi/mat/ginodi_11.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/hammer/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0102_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0301_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0305_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0306_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0307_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0308_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0309_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0311_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0401_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0402_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0404_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0405_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0408_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0410_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0421_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0423_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0426_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0701_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0703_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0802_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0804_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0806_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0813_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0817_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1102_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1104_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1106_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1107_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1114_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1120_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1121_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1128_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1301_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1302_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1304_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1305_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1307_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1311_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1321_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1322_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1323_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1327_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1328_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1501_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1502_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1506_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB5_0101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB5_0105_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/hammer/mat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/pcm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/pcm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/pcm/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/pcm/mat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/pcm/mat/pcm_6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/proteasmm_c/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/proteasmm_c/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/proteasmm_c/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/proteasmm_c/mat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/proteasmm_c/mat/proteasmm_c_10.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/proteasmm_i/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/proteasmm_i/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/proteasmm_i/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/proteasmm_i/mat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/proteasmm_i/mat/proteasmm_i_10.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/smm/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_01_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_01_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_01_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_01_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_02_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_02_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_02_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_03_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_03_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_03_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_06_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_06_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_06_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_06_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_11_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_12_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_16_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_17_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_17_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_19_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_50_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_03_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_03_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_03_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_03_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_11_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_11_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_11_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_11_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_23_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_23_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_23_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_23_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_24_02_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_24_02_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_24_02_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_24_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_24_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_25_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_26_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_26_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_26_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_26_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_26_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_26_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_29_02_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_29_02_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_29_02_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_29_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_30_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_30_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_30_02_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_30_02_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_30_02_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_30_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_31_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_31_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_31_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_32_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_32_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_32_07_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_32_15_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_33_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_33_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_66_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_68_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_68_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_68_02_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_68_02_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_68_02_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_68_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_68_23_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_69_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/A_80_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_07_02_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_07_02_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_07_02_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_07_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_08_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_08_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_08_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_08_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_08_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_08_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_14_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_15_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_15_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_15_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_15_03_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_15_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_15_09_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_15_17_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_15_42_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_18_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_18_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_18_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_18_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_27_05_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_27_05_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_27_05_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_27_05_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_27_20_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_35_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_35_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_35_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_35_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_35_03_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_35_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_38_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_39_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_40_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_40_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_40_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_40_02_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_40_02_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_40_02_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_40_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_40_13_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_42_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_42_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_44_02_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_44_02_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_44_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_44_03_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_44_03_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_44_03_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_44_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_45_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_45_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_45_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_45_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_46_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_48_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_51_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_51_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_51_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_51_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_53_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_53_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_53_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_53_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_54_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_54_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_54_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_57_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_57_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_57_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_58_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_58_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_58_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_58_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_73_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/B_83_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/C_03_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/C_04_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/C_05_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/C_06_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/C_07_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/C_07_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/C_08_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/C_12_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/C_14_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/C_15_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/E_01_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/E_01_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smm/mat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_01_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_01_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_01_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_01_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_02_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_02_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_02_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_03_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_03_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_03_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_06_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_06_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_06_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_06_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_11_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_12_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_16_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_17_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_17_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_19_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_50_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_03_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_03_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_03_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_03_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_11_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_11_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_11_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_11_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_23_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_23_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_23_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_23_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_24_02_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_24_02_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_24_02_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_24_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_24_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_25_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_26_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_26_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_26_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_26_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_26_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_26_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_29_02_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_29_02_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_29_02_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_29_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_30_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_30_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_30_02_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_30_02_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_30_02_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_30_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_31_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_31_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_31_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_32_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_32_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_32_07_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_32_15_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_33_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_33_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_66_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_68_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_68_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_68_02_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_68_02_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_68_02_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_68_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_68_23_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_69_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_80_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_07_02_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_07_02_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_07_02_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_07_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_08_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_08_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_08_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_08_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_08_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_08_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_14_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_15_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_15_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_15_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_15_03_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_15_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_15_09_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_15_17_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_15_42_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_18_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_18_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_18_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_18_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_27_05_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_27_05_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_27_05_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_27_05_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_27_20_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_35_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_35_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_35_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_35_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_35_03_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_35_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_38_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_39_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_40_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_40_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_40_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_40_02_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_40_02_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_40_02_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_40_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_40_13_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_42_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_42_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_44_02_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_44_02_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_44_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_44_03_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_44_03_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_44_03_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_44_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_45_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_45_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_45_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_45_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_46_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_48_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_51_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_51_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_51_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_51_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_53_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_53_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_53_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_53_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_54_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_54_01_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_54_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_57_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_57_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_57_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_58_01_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_58_01_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_58_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_58_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_73_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_83_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_03_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_04_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_05_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_06_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_07_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_07_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_08_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_12_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_14_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_15_02_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/E_01_01_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/E_01_03_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/smmtap/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmtap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/smmtap/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmtap/mat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/smmtap/mat/smmtap_9.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0101_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0101_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0101_12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0101_13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0201_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0201_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0201_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0301_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0301_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0301_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_1101_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_1101_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_1101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_2402_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_2402_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_2402_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_2601_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_2601_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_2601_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3101_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3101_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3201_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3201_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3201_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3303_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3303_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3303_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_6601_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_6601_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_6801_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_6801_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_6801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_0702_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_0702_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_0702_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_0801_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_0801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1302_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1302_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1402_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1402_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1501_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1501_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1510_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1516_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1801_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_2705_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_2705_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_2709_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3501_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3501_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3701_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3701_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3701_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3801_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3901_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3901_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3902_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3902_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4001_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4001_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4002_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4101_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4402_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4402_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4402_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4501_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4501_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4701_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4701_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4901_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4901_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5001_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5001_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5101_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5301_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5301_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5701_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5701_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5801_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5801_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5801_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5802_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5802_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5802_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5802_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0102_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0102_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0102_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0202_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0202_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0202_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0303_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0303_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0303_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0304_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0304_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0304_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0401_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0401_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0401_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0501_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0501_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0501_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0601_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0602_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0602_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0602_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0701_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0701_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0701_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0702_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0702_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0702_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0802_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0802_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0802_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1203_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1203_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1203_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1402_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1402_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1402_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1502_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1502_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1502_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1601_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1601_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1601_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1701_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1701_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1701_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/DRB1_0101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/DRB1_0301_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/DRB1_0701_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/DRB1_1101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/DRB1_1501_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/D_b_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/D_b_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/G_0101_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/G_0101_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/G_0101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/K_b_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/K_d_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/K_d_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/L_d_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0102_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0103_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0104_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0105_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0106_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0107_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0108_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0109_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0110_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0111_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0112_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0113_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0114_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0115_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0116_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0117_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0118_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0119_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0120_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0121_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0122_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0123_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0124_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0125_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0126_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0127_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0128_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0129_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0130_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0131_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0132_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0134_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0135_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0136_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0301_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0302_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0303_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0304_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0305_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0306_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0307_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0308_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0309_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0310_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0311_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0312_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0313_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0314_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0315_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0316_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0317_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0318_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0319_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0320_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0321_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0322_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0323_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0324_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0325_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0326_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0327_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0328_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0329_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0330_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0331_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0332_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0333_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0334_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0335_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0336_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0337_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0338_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0339_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0340_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0341_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0342_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0343_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0344_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0345_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0346_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0347_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0348_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0349_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0350_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0351_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0352_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0353_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0354_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0355_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0356_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0357_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0358_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0359_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0360_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0361_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0362_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0363_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0364_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0401_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0402_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0403_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0404_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0405_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0406_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0407_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0408_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0409_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0410_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0411_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0412_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0413_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0414_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0415_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0416_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0417_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0418_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0419_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0420_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0421_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0422_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0423_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0424_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0425_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0426_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0427_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0428_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0429_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0430_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0431_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0432_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0433_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0434_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0435_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0436_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0437_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0438_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0439_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0440_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0441_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0442_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0443_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0444_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0445_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0446_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0447_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0448_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0449_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0450_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0451_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0452_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0453_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0454_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0455_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0456_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0457_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0458_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0459_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0460_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0461_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0462_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0463_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0464_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0465_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0466_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0467_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0468_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0469_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0470_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0471_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0472_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0473_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0474_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0475_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0476_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0477_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0478_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0479_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0480_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0482_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0483_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0484_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0485_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0486_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0487_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0488_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0489_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0490_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0491_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0492_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0493_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0495_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0496_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0497_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0498_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0701_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0703_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0704_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0705_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0706_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0707_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0708_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0709_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0711_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0712_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0713_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0714_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0715_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0716_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0717_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0718_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0719_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0720_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0721_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0801_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0802_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0803_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0804_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0805_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0806_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0807_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0808_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0809_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0810_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0811_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0812_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0813_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0814_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0815_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0816_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0817_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0818_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0819_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0820_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0821_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0822_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0823_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0824_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0825_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0826_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0827_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0828_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0829_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0830_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0831_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0832_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0833_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0834_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0835_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0836_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0837_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0838_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0839_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0840_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0841_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0842_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0843_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0844_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0845_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0901_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0902_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0903_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0904_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0905_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0906_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0907_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0908_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0909_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0910_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0911_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0912_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1001_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1002_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1003_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1102_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1103_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1104_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1105_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1106_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1107_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1108_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1109_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1110_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1111_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1112_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1113_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1114_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1115_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1116_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1117_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1118_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1119_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1120_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1121_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1122_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1123_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1124_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1125_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1126_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1127_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1128_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1129_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1130_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1131_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1132_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1133_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1134_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1135_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1136_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1137_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1138_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1139_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1140_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1141_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1142_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1143_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1144_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1145_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1146_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1147_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1148_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1149_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1150_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1151_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1152_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1153_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1154_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1155_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1156_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1157_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1158_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1159_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1160_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1161_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1162_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1163_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1164_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1165_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1166_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1167_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1168_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1169_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1170_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1172_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1173_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1174_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1175_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1176_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1177_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1178_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1179_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1180_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1181_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1182_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1183_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1184_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1185_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1186_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1187_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1188_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1189_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1190_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1191_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1192_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1193_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1194_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1195_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1196_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1197_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1198_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1199_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1201_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1202_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1203_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1204_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1205_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1206_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1207_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1208_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1209_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1210_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1211_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1212_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1213_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1214_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1215_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1216_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1217_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1218_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1219_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1220_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1221_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1222_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1223_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1225_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1226_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1227_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1301_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1302_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1303_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1304_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1305_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1306_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1307_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1308_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1309_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1310_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1311_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1312_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1313_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1314_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1315_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1316_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1317_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1318_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1319_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1320_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1321_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1322_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1323_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1324_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1325_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1326_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1327_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1328_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1329_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1330_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1331_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1332_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1333_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1334_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1335_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1336_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1337_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1338_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1339_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1340_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1341_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1342_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1343_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1344_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1345_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1346_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1347_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1348_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1349_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1350_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1351_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1352_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1353_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1354_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1355_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1356_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1357_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1358_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1359_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1360_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1361_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1362_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1363_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1364_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1365_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1366_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1367_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1368_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1369_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1370_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1371_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1372_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1373_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1374_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1375_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1376_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1377_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1378_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1379_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1380_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1381_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1382_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1383_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1384_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1385_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1386_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1387_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1388_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1389_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1390_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1391_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1392_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1393_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1394_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1395_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1396_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1397_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1398_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1399_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1401_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1402_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1403_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1404_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1405_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1406_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1407_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1408_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1409_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1410_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1411_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1412_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1413_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1414_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1415_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1416_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1417_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1418_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1419_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1420_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1421_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1422_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1423_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1424_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1425_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1426_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1427_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1428_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1429_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1430_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1431_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1432_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1433_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1434_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1435_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1436_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1437_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1438_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1439_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1440_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1441_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1442_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1443_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1444_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1445_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1446_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1447_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1448_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1449_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1450_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1451_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1452_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1453_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1454_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1455_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1456_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1457_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1458_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1459_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1460_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1461_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1462_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1463_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1464_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1465_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1467_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1468_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1469_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1470_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1471_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1472_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1473_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1474_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1475_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1476_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1477_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1478_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1479_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1480_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1481_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1482_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1483_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1484_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1485_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1486_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1487_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1488_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1489_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1490_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1491_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1493_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1494_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1495_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1496_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1497_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1498_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1499_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1501_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1502_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1503_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1504_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1505_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1506_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1507_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1508_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1509_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1510_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1511_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1512_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1513_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1514_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1515_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1516_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1518_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1519_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1520_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1521_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1522_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1523_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1524_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1525_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1526_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1527_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1528_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1529_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1530_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1531_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1532_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1533_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1534_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1535_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1536_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1537_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1538_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1539_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1540_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1541_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1542_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1543_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1544_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1545_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1546_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1547_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1548_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1549_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1551_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1552_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1553_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1554_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1555_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1556_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1557_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1601_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1602_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1603_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1604_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1605_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1607_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1608_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1609_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1610_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1611_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1612_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1614_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1615_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1616_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1617_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1618_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0102_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0103_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0104_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0105_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0106_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0107_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0108_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0109_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0110_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0111_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0112_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0113_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0114_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0115_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0201_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0202_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0203_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0204_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0205_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0206_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0207_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0208_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0209_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0210_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0211_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0212_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0213_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0214_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0215_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0216_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0217_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0218_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0219_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0220_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0221_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0222_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0223_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0224_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0225_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0226_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0227_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0228_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0301_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0302_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0303_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB4_0101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB4_0103_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB4_0104_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB4_0105_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB4_0106_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB4_0107_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB4_0108_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0101_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0102_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0104_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0105_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0106_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0107_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0108_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0109_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0111_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0112_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0113_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0114_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0202_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0203_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0204_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0205_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/supportedAlleles/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/supportedAlleles/ann/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/ann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/ann/mhcflurry_1_2_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/ann/mhcflurry_1_4_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/ann/mhcnuggets_class_1_2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/ann/mhcnuggets_class_1_2_3_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/ann/mhcnuggets_class_2_2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/ann/mhcnuggets_class_2_2_3_2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44431 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/netMHCstabpan_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44375 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/netctlpan_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcII_2_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcII_2_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)   156318 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcIIpan_3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)   156318 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcIIpan_3_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)   156384 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcIIpan_4_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhc_3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhc_3_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhc_4_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44405 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcpan_2_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44405 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcpan_2_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44427 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcpan_3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66517 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcpan_4_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)   161708 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcpan_4_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44406 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/external/pickpocket_1_1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/Data/supportedAlleles/pssm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/pssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/pssm/arb_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/pssm/bimas_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/pssm/calisimm_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/pssm/comblibsidney_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/pssm/epidemix_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/pssm/hammer_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/pssm/smm_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/pssm/smmpmbec_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/pssm/syfpeithi_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/Data/supportedAlleles/pssm/tepitopepan_1_0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/EpitopeAssembly/
+-rw-r--r--   0 runner    (1001) docker     (123)    47830 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/EpitopeAssembly/EpitopeAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/EpitopeAssembly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/EpitopePrediction/
+-rw-r--r--   0 runner    (1001) docker     (123)    36337 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/EpitopePrediction/ANN.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    77738 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/EpitopePrediction/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31229 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/EpitopePrediction/PSSM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/EpitopePrediction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/EpitopeSelection/
+-rw-r--r--   0 runner    (1001) docker     (123)    17795 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/EpitopeSelection/OptiTope.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/EpitopeSelection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/HLAtyping/
+-rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/HLAtyping/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/HLAtyping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/IO/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/IO/ADBAdapter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12575 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/IO/EnsemblAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/IO/FileReader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47054 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/IO/MartsAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/IO/RefSeqAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/IO/UniProtAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/IO/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/IO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/TAPPrediction/
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/TAPPrediction/PSSM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/TAPPrediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/DummyAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/DummyEpitopePredictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/TestAllele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/TestCleavagePrediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/TestEpitopeAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/TestEpitopePrediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/TestGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22469 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/TestIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/TestOptiTope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/TestPeptide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/TestPredictionVersioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/TestProtein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/TestSpacerDesign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/TestTAPPrediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/TestTranscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/TestVariant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12323 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/VariantsForTesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope/test/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/external/TestExternalCleavagePrediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/external/TestExternalEpitopePrediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:49:15.000000 epytope-3.3.1/epytope/test/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    75748 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 11:49:30.000000 epytope-3.3.1/epytope.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:49:30.000000 epytope-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-04-25 11:49:15.000000 epytope-3.3.1/setup.py
```

### Comparing `epytope-3.3.0/CHANGELOG.md` & `epytope-3.3.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 # epytope: Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## v3.3.1 - 2023-04-25
+
+### `Added`
+
+### `Changed`
+
+- [#85](https://github.com/KohlbacherLab/epytope/pull/85) Pinned pandas version >= 1.3.5 as requested by @e-dorigatti [#84](https://github.com/KohlbacherLab/epytope/issues/84).
+
+### `Fixed`
+
+- [#83](https://github.com/KohlbacherLab/epytope/pull/83) Fixed erroneous mouse allele parsing for PSSM predictors [#82](https://github.com/KohlbacherLab/epytope/issues/82)
+
 ## v3.3.0 - 2022-12-01
 
 ### `Added`
 
 ### `Changed`
 
 - Switch from [PyVCF](https://github.com/jamescasbon/PyVCF) to [PyVCF3](https://github.com/dridk/PyVCF3) as dependency
```

### Comparing `epytope-3.3.0/LICENSE.txt` & `epytope-3.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/PKG-INFO` & `epytope-3.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epytope
-Version: 3.3.0
+Version: 3.3.1
 Summary: A Framework for Epitope Detection and Vaccine Design
 Home-page: https://github.com/KohlbacherLab/epytope
 Author: Benjamin Schubert, Mathias Walzer, Christopher Mohr, Leon Kuchenbecker
 Author-email: benjamin.schubert@helmholtz-muenchen.de, walzer@ebi.ac.uk, christopher.mohr@uni-tuebingen.de, leon.kuchenbecker@uni-tuebingen.de 
 Maintainer: Christopher Mohr
 Maintainer-email: christopher.mohr@uni-tuebingen.de
 License: BSD
@@ -21,15 +21,16 @@
 
 ![PyPi](https://github.com/KohlbacherLab/epytope/actions/workflows/pypi-publish.yml/badge.svg)
 ![Tests](https://github.com/KohlbacherLab/epytope/actions/workflows/python-test-conda.yml/badge.svg)
 ![Tests external](https://github.com/KohlbacherLab/epytope/actions/workflows/python-test-conda-external.yml/badge.svg)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/epytope/badges/version.svg)](https://anaconda.org/bioconda/epytope)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/epytope/badges/latest_release_date.svg)](https://anaconda.org/bioconda/epytope)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![Anaconda-Server Badge](https://anaconda.org/bioconda/epytope/badges/installer/conda.svg)](https://conda.anaconda.org/bioconda)
+[![Anaconda-Server Badge](https://anaconda.org/bioconda/epytope/badges/platforms.svg
+)](https://anaconda.org/bioconda/epytope)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/epytope/badges/downloads.svg)](https://anaconda.org/bioconda/epytope)
 
 Copyright 2014 by Benjamin Schuber, Mathias Walzer, Philipp Brachvogel, Andras Szolek, Christopher Mohr, and Oliver Kohlbacher
 
 **epytope** is a framework for T-cell epitope detection, and vaccine design. It offers consistent, easy, and simultaneous access to well established prediction methods of computational immunology. **epytope** can handle polymorphic proteins and offers analysis tools to select, assemble, and design linker sequences for string-of-beads epitope-based vaccines. It is implemented in Python in a modular way and can easily be extended by user defined methods.
 
 ## Copyright
```

### Comparing `epytope-3.3.0/README.md` & `epytope-3.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 ![PyPi](https://github.com/KohlbacherLab/epytope/actions/workflows/pypi-publish.yml/badge.svg)
 ![Tests](https://github.com/KohlbacherLab/epytope/actions/workflows/python-test-conda.yml/badge.svg)
 ![Tests external](https://github.com/KohlbacherLab/epytope/actions/workflows/python-test-conda-external.yml/badge.svg)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/epytope/badges/version.svg)](https://anaconda.org/bioconda/epytope)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/epytope/badges/latest_release_date.svg)](https://anaconda.org/bioconda/epytope)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![Anaconda-Server Badge](https://anaconda.org/bioconda/epytope/badges/installer/conda.svg)](https://conda.anaconda.org/bioconda)
+[![Anaconda-Server Badge](https://anaconda.org/bioconda/epytope/badges/platforms.svg
+)](https://anaconda.org/bioconda/epytope)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/epytope/badges/downloads.svg)](https://anaconda.org/bioconda/epytope)
 
 Copyright 2014 by Benjamin Schuber, Mathias Walzer, Philipp Brachvogel, Andras Szolek, Christopher Mohr, and Oliver Kohlbacher
 
 **epytope** is a framework for T-cell epitope detection, and vaccine design. It offers consistent, easy, and simultaneous access to well established prediction methods of computational immunology. **epytope** can handle polymorphic proteins and offers analysis tools to select, assemble, and design linker sequences for string-of-beads epitope-based vaccines. It is implemented in Python in a modular way and can easily be extended by user defined methods.
 
 ## Copyright
```

### Comparing `epytope-3.3.0/epytope/CleavagePrediction/External.py` & `epytope-3.3.1/epytope/CleavagePrediction/External.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/CleavagePrediction/PSSM.py` & `epytope-3.3.1/epytope/CleavagePrediction/PSSM.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/CleavagePrediction/__init__.py` & `epytope-3.3.1/epytope/CleavagePrediction/__init__.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Core/Allele.py` & `epytope-3.3.1/epytope/Core/Allele.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Core/Base.py` & `epytope-3.3.1/epytope/Core/Base.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Core/Generator.py` & `epytope-3.3.1/epytope/Core/Generator.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Core/Peptide.py` & `epytope-3.3.1/epytope/Core/Peptide.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Core/Protein.py` & `epytope-3.3.1/epytope/Core/Protein.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Core/Result.py` & `epytope-3.3.1/epytope/Core/Result.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Core/Transcript.py` & `epytope-3.3.1/epytope/Core/Transcript.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Core/Variant.py` & `epytope-3.3.1/epytope/Core/Variant.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Core/__init__.py` & `epytope-3.3.1/epytope/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/DistanceMatrices.py` & `epytope-3.3.1/epytope/Data/DistanceMatrices.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/examples/Homo_sapiens.GRCh38.cds.test_stub.fa` & `epytope-3.3.1/epytope/Data/examples/Homo_sapiens.GRCh38.cds.test_stub.fa`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/examples/Homo_sapiens.GRCh38.pep.test_stub.fa` & `epytope-3.3.1/epytope/Data/examples/Homo_sapiens.GRCh38.pep.test_stub.fa`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/examples/testSequences.fasta` & `epytope-3.3.1/epytope/Data/examples/testSequences.fasta`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/examples/testSequences_d2s.fasta` & `epytope-3.3.1/epytope/Data/examples/testSequences_d2s.fasta`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/examples/test_annovar.out` & `epytope-3.3.1/epytope/Data/examples/test_annovar.out`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/examples/vcftestfile1.vcf` & `epytope-3.3.1/epytope/Data/examples/vcftestfile1.vcf`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/examples/vcftestfile2.vcf` & `epytope-3.3.1/epytope/Data/examples/vcftestfile2.vcf`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/examples/vcftestfile3.vcf` & `epytope-3.3.1/epytope/Data/examples/vcftestfile3.vcf`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0101_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0101_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0101_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0201_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0201_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0201_11.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0201_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0201_8.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0201_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0201_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0201_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0202_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0202_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0202_11.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0202_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0202_8.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0202_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0202_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0202_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0203_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0203_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0203_11.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0203_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0203_8.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0203_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0203_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0203_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0206_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0206_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0206_11.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0206_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0206_8.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0206_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0206_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0206_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0211_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0211_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0212_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0212_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0216_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0216_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0219_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0219_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0250_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0250_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0301_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0301_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_0301_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_0301_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_1101_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_1101_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_1101_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_1101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2301_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2301_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2301_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2301_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2402_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2402_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2402_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2402_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2403_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2403_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2501_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2501_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2601_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2601_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2601_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2601_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2602_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2602_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2603_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2603_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2902_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2902_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_2902_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_2902_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3001_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3001_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3001_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3001_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3002_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3002_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3002_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3002_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3101_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3101_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3101_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3201_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3201_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3201_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3201_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3301_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3301_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_3301_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_3301_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_6801_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_6801_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_6801_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_6801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_6802_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_6802_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_6802_11.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_6802_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_6802_8.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_6802_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_6802_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_6802_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_6901_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_6901_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/A_8001_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/A_8001_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_0702_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_0702_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_0702_8.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_0702_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_0702_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_0702_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_0801_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_0801_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_0801_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_0801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_0802_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_0802_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_0803_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_0803_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_1501_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_1501_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_1502_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_1502_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_1503_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_1503_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_1509_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_1509_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_1517_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_1517_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_1801_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_1801_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_1801_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_1801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_2703_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_2703_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_2705_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_2705_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_2705_11.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_2705_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_2705_8.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_2705_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_2705_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_2705_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_3501_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_3501_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_3501_8.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_3501_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_3501_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_3501_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_3801_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_3801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_3901_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_3901_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4001_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4001_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4001_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4001_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4002_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4002_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4002_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4002_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4402_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4402_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4402_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4402_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4403_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4403_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4403_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4403_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4501_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4501_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4501_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4501_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4601_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4601_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_4801_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_4801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5101_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5101_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5101_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5301_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5301_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5301_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5301_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5401_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5401_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5401_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5401_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5701_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5701_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5701_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5701_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5801_10.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5801_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_5801_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_5801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/arb/mat/B_7301_9.py` & `epytope-3.3.1/epytope/Data/pssms/arb/mat/B_7301_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_0101_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_0101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_0201_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_0201_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_0205_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_0205_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_0301_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_0301_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_1101_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_1101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_2402_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_2402_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_3101_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_3101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_3302_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_3302_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/A_6801_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/A_6801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_0401_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_0401_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_0702_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_0702_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_0801_8.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_0801_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_0801_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_0801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_1501_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_1501_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_2702_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_2702_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_2705_8.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_2705_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_2705_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_2705_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_3501_8.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_3501_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_3501_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_3501_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_3701_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_3701_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_3801_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_3801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_3901_8.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_3901_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_3901_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_3901_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_3902_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_3902_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_4001_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_4001_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_4006_8.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_4006_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_4006_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_4006_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_40_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_40_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_4403_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_4403_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_5101_8.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_5101_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_5101_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_5101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_5102_8.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_5102_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_5102_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_5102_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_5103_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_5103_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_5201_8.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_5201_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_5201_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_5201_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/B_5801_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/B_5801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/C_0301_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/C_0301_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/C_0401_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/C_0401_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/C_0602_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/C_0602_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/bimas/mat/C_0702_9.py` & `epytope-3.3.1/epytope/Data/pssms/bimas/mat/C_0702_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/A_0201_9.py` & `epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/A_0201_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/A_3001_9.py` & `epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/A_3001_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/A_3201_9.py` & `epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/A_3201_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/A_6802_9.py` & `epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/A_6802_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_0702_9.py` & `epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_0702_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_0801_9.py` & `epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_0801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_1501_9.py` & `epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_1501_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_1503_9.py` & `epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_1503_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_2705_9.py` & `epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_2705_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_3501_9.py` & `epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_3501_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_5101_9.py` & `epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_5101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_5301_9.py` & `epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_5301_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_5401_9.py` & `epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_5401_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_5801_9.py` & `epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_5801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/comblibsidney/mat/B_5802_9.py` & `epytope-3.3.1/epytope/Data/pssms/comblibsidney/mat/B_5802_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/doytchinova/mat/doytchinova_9.py` & `epytope-3.3.1/epytope/Data/pssms/doytchinova/mat/doytchinova_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_0201_10.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_0201_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_0201_11.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_0201_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_0201_9.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_0201_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_03_10.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_03_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_1101_10.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_1101_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_1101_9.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_1101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_2402_9.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_2402_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_24_9.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_24_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_25_10.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_25_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/A_25_9.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/A_25_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_07_9.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_07_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_08_8.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_08_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_08_9.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_08_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_1801_8.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_1801_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_1801_9.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_1801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_2705_9.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_2705_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_27_10.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_27_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_27_9.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_27_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_3701_9.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_3701_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_44_9.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_44_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_5101_8.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_5101_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/epidemix/mat/B_5101_9.py` & `epytope-3.3.1/epytope/Data/pssms/epidemix/mat/B_5101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/ginodi/mat/ginodi_11.py` & `epytope-3.3.1/epytope/Data/pssms/ginodi/mat/ginodi_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0101_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0102_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0102_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0301_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0301_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0305_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0305_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0306_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0306_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0307_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0307_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0308_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0308_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0309_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0309_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0311_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0311_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0401_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0401_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0402_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0402_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0404_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0404_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0405_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0405_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0408_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0408_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0410_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0410_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0421_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0421_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0423_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0423_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0426_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0426_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0701_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0701_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0703_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0703_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0801_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0802_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0802_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0804_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0804_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0806_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0806_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0813_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0813_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_0817_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_0817_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1101_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1102_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1102_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1104_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1104_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1106_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1106_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1107_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1107_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1114_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1114_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1120_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1120_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1121_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1121_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1128_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1128_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1301_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1301_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1302_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1302_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1304_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1304_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1305_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1305_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1307_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1307_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1311_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1311_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1321_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1321_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1322_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1322_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1323_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1323_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1327_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1327_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1328_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1328_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1501_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1501_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1502_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1502_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB1_1506_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB1_1506_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB5_0101_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB5_0101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/hammer/mat/DRB5_0105_9.py` & `epytope-3.3.1/epytope/Data/pssms/hammer/mat/DRB5_0105_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/pcm/mat/pcm_6.py` & `epytope-3.3.1/epytope/Data/pssms/pcm/mat/pcm_6.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/proteasmm_c/mat/proteasmm_c_10.py` & `epytope-3.3.1/epytope/Data/pssms/proteasmm_c/mat/proteasmm_c_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/proteasmm_i/mat/proteasmm_i_10.py` & `epytope-3.3.1/epytope/Data/pssms/proteasmm_i/mat/proteasmm_i_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_01_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_01_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_01_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_01_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_01_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_01_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_01_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_01_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_02_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_02_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_02_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_02_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_02_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_02_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_03_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_03_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_03_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_03_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_03_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_03_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_06_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_06_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_06_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_06_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_06_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_06_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_06_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_06_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_11_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_11_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_12_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_12_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_16_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_16_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_17_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_17_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_17_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_17_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_19_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_19_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_02_50_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_02_50_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_03_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_03_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_03_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_03_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_03_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_03_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_03_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_03_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_11_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_11_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_11_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_11_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_11_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_11_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_11_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_11_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_23_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_23_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_23_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_23_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_23_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_23_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_23_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_23_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_24_02_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_24_02_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_24_02_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_24_02_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_24_02_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_24_02_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_24_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_24_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_24_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_24_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_25_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_25_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_26_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_26_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_26_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_26_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_26_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_26_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_26_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_26_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_26_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_26_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_26_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_26_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_29_02_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_29_02_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_29_02_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_29_02_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_29_02_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_29_02_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_29_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_29_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_30_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_30_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_30_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_30_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_30_02_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_30_02_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_30_02_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_30_02_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_30_02_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_30_02_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_30_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_30_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_31_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_31_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_31_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_31_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_31_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_31_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_32_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_32_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_32_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_32_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_32_07_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_32_07_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_32_15_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_32_15_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_33_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_33_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_33_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_33_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_66_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_66_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_68_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_68_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_68_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_68_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_68_02_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_68_02_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_68_02_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_68_02_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_68_02_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_68_02_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_68_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_68_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_68_23_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_68_23_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_69_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_69_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/A_80_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/A_80_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_07_02_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_07_02_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_07_02_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_07_02_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_07_02_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_07_02_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_07_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_07_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_08_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_08_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_08_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_08_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_08_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_08_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_08_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_08_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_08_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_08_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_08_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_08_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_14_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_14_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_15_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_15_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_15_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_15_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_15_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_15_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_15_03_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_15_03_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_15_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_15_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_15_09_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_15_09_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_15_17_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_15_17_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_15_42_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_15_42_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_18_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_18_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_18_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_18_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_18_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_18_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_18_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_18_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_27_05_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_27_05_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_27_05_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_27_05_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_27_05_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_27_05_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_27_05_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_27_05_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_27_20_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_27_20_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_35_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_35_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_35_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_35_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_35_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_35_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_35_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_35_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_35_03_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_35_03_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_35_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_35_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_38_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_38_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_39_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_39_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_40_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_40_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_40_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_40_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_40_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_40_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_40_02_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_40_02_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_40_02_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_40_02_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_40_02_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_40_02_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_40_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_40_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_40_13_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_40_13_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_42_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_42_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_42_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_42_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_44_02_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_44_02_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_44_02_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_44_02_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_44_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_44_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_44_03_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_44_03_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_44_03_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_44_03_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_44_03_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_44_03_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_44_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_44_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_45_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_45_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_45_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_45_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_45_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_45_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_45_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_45_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_46_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_46_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_48_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_48_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_51_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_51_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_51_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_51_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_51_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_51_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_51_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_51_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_53_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_53_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_53_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_53_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_53_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_53_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_53_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_53_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_54_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_54_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_54_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_54_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_54_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_54_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_57_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_57_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_57_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_57_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_57_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_57_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_58_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_58_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_58_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_58_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_58_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_58_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_58_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_58_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_73_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_73_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/B_83_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/B_83_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/C_03_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/C_03_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/C_04_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/C_04_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/C_05_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/C_05_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/C_06_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/C_06_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/C_07_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/C_07_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/C_07_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/C_07_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/C_08_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/C_08_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/C_12_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/C_12_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/C_14_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/C_14_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/C_15_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/C_15_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/E_01_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/E_01_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smm/mat/E_01_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smm/mat/E_01_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_01_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_01_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_01_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_01_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_01_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_01_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_01_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_01_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_02_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_02_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_02_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_02_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_02_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_02_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_03_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_03_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_03_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_03_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_03_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_03_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_06_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_06_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_06_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_06_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_06_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_06_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_06_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_06_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_11_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_11_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_12_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_12_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_16_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_16_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_17_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_17_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_17_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_17_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_19_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_19_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_02_50_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_02_50_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_03_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_03_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_03_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_03_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_03_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_03_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_03_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_03_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_11_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_11_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_11_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_11_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_11_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_11_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_11_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_11_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_23_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_23_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_23_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_23_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_23_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_23_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_23_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_23_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_24_02_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_24_02_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_24_02_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_24_02_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_24_02_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_24_02_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_24_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_24_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_24_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_24_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_25_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_25_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_26_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_26_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_26_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_26_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_26_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_26_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_26_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_26_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_26_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_26_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_26_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_26_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_29_02_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_29_02_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_29_02_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_29_02_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_29_02_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_29_02_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_29_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_29_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_30_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_30_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_30_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_30_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_30_02_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_30_02_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_30_02_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_30_02_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_30_02_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_30_02_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_30_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_30_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_31_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_31_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_31_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_31_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_31_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_31_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_32_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_32_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_32_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_32_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_32_07_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_32_07_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_32_15_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_32_15_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_33_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_33_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_33_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_33_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_66_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_66_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_68_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_68_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_68_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_68_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_68_02_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_68_02_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_68_02_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_68_02_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_68_02_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_68_02_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_68_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_68_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_68_23_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_68_23_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_69_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_69_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/A_80_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/A_80_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_07_02_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_07_02_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_07_02_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_07_02_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_07_02_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_07_02_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_07_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_07_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_08_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_08_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_08_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_08_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_08_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_08_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_08_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_08_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_08_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_08_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_08_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_08_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_14_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_14_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_15_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_15_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_15_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_15_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_15_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_15_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_15_03_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_15_03_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_15_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_15_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_15_09_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_15_09_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_15_17_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_15_17_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_15_42_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_15_42_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_18_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_18_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_18_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_18_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_18_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_18_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_18_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_18_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_27_05_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_27_05_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_27_05_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_27_05_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_27_05_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_27_05_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_27_05_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_27_05_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_27_20_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_27_20_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_35_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_35_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_35_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_35_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_35_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_35_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_35_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_35_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_35_03_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_35_03_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_35_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_35_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_38_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_38_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_39_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_39_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_40_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_40_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_40_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_40_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_40_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_40_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_40_02_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_40_02_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_40_02_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_40_02_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_40_02_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_40_02_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_40_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_40_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_40_13_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_40_13_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_42_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_42_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_42_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_42_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_44_02_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_44_02_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_44_02_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_44_02_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_44_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_44_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_44_03_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_44_03_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_44_03_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_44_03_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_44_03_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_44_03_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_44_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_44_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_45_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_45_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_45_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_45_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_45_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_45_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_45_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_45_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_46_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_46_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_48_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_48_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_51_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_51_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_51_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_51_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_51_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_51_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_51_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_51_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_53_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_53_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_53_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_53_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_53_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_53_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_53_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_53_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_54_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_54_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_54_01_8.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_54_01_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_54_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_54_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_57_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_57_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_57_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_57_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_57_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_57_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_58_01_10.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_58_01_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_58_01_11.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_58_01_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_58_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_58_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_58_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_58_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_73_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_73_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/B_83_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/B_83_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_03_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_03_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_04_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_04_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_05_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_05_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_06_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_06_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_07_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_07_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_07_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_07_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_08_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_08_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_12_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_12_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_14_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_14_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/C_15_02_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/C_15_02_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/E_01_01_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/E_01_01_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmpmbec/mat/E_01_03_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmpmbec/mat/E_01_03_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/smmtap/mat/smmtap_9.py` & `epytope-3.3.1/epytope/Data/pssms/smmtap/mat/smmtap_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0101_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0101_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0101_11.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0101_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0101_12.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0101_12.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0101_13.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0101_13.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0101_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0201_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0201_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0201_11.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0201_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0201_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0201_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0301_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0301_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0301_11.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0301_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_0301_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_0301_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_1101_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_1101_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_1101_11.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_1101_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_1101_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_1101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_2402_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_2402_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_2402_11.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_2402_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_2402_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_2402_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_2601_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_2601_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_2601_11.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_2601_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_2601_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_2601_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3101_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3101_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3101_11.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3101_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3101_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3201_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3201_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3201_11.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3201_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3201_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3201_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3303_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3303_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3303_11.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3303_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_3303_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_3303_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_6601_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_6601_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_6601_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_6601_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_6801_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_6801_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_6801_11.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_6801_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/A_6801_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/A_6801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_0702_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_0702_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_0702_11.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_0702_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_0702_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_0702_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_0801_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_0801_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_0801_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_0801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1302_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1302_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1302_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1302_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1402_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1402_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1402_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1402_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1501_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1501_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1501_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1501_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1510_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1510_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1516_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1516_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1801_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1801_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_1801_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_1801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_2705_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_2705_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_2705_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_2705_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_2709_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_2709_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3501_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3501_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3501_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3501_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3701_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3701_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3701_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3701_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3701_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3701_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3801_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3801_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3801_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3901_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3901_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3901_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3901_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3902_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3902_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_3902_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_3902_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4001_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4001_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4001_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4001_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4002_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4002_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4101_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4101_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4101_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4402_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4402_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4402_11.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4402_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4402_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4402_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4501_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4501_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4501_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4501_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4701_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4701_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4701_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4701_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4901_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4901_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_4901_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_4901_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5001_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5001_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5001_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5001_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5101_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5101_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5101_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5301_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5301_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5301_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5301_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5701_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5701_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5701_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5701_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5801_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5801_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5801_11.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5801_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5801_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5801_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5801_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5802_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5802_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5802_11.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5802_11.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5802_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5802_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/B_5802_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/B_5802_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0102_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0102_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0102_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0102_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0102_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0102_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0202_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0202_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0202_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0202_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0202_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0202_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0303_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0303_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0303_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0303_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0303_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0303_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0304_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0304_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0304_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0304_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0304_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0304_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0401_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0401_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0401_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0401_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0401_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0401_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0501_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0501_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0501_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0501_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0501_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0501_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0601_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0601_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0602_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0602_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0602_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0602_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0602_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0602_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0701_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0701_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0701_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0701_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0701_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0701_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0702_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0702_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0702_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0702_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0702_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0702_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0802_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0802_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0802_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0802_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_0802_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_0802_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1203_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1203_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1203_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1203_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1203_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1203_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1402_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1402_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1402_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1402_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1402_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1402_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1502_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1502_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1502_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1502_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1502_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1502_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1601_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1601_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1601_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1601_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1601_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1601_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1701_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1701_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1701_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1701_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/C_1701_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/C_1701_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/DRB1_0101_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/DRB1_0101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/DRB1_0301_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/DRB1_0301_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/DRB1_0701_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/DRB1_0701_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/DRB1_1101_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/DRB1_1101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/DRB1_1501_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/DRB1_1501_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/G_0101_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/G_0101_10.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/G_0101_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/G_0101_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/G_0101_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/G_0101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/H2_Db_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/D_b_9.py`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-H2_Db_10 = {0: {'A': 2, 'C': 0, 'D': 0, 'E': -1, 'F': 2, 'G': 0, 'H': 0, 'I': 0, 'K': 1, 'L': 0, 'M': 0, 'N': 0, 'P': -1, 'Q': 0, 'R': -1, 'S': 2, 'T': 1, 'V': 1, 'W': 0, 'X': 0, 'Y': 0}, 1: {'A': 3, 'C': 0, 'D': 0, 'E': 0, 'F': -1, 'G': 2, 'H': 0, 'I': -1, 'K': 0, 'L': 0, 'M': 2, 'N': 0, 'P': 0, 'Q': 1, 'R': 0, 'S': 2, 'T': 0, 'V': -1, 'W': 0, 'X': 0, 'Y': 0}, 2: {'A': 0, 'C': 0, 'D': 0, 'E': -1, 'F': 0, 'G': 1, 'H': 0, 'I': 2, 'K': -1, 'L': 2, 'M': 0, 'N': 0, 'P': 3, 'Q': 0, 'R': -1, 'S': 0, 'T': -1, 'V': 2, 'W': 0, 'X': 0, 'Y': 0}, 3: {'A': 0, 'C': 0, 'D': 1, 'E': 2, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 1, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 1, 'R': 1, 'S': 1, 'T': 1, 'V': 2, 'W': 0, 'X': 0, 'Y': 0}, 4: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 10, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 5: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 1, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 2, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 6: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 7: {'A': 0, 'C': 0, 'D': 2, 'E': 2, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 1, 'R': 0, 'S': 1, 'T': 2, 'V': 1, 'W': 0, 'X': 0, 'Y': 0}, 8: {'A': 0, 'C': 0, 'D': 0, 'E': 2, 'F': 1, 'G': 0, 'H': 1, 'I': -1, 'K': 0, 'L': 1, 'M': -1, 'N': 0, 'P': 0, 'Q': 0, 'R': 1, 'S': 1, 'T': 2, 'V': 0, 'W': 0, 'X': 0, 'Y': 2}, 9: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 8, 'G': 0, 'H': 0, 'I': 10, 'K': 0, 'L': 10, 'M': 10, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 6, 'W': 0, 'X': 0, 'Y': 0}}
+D_b_9 = {0: {'A': 2, 'C': 0, 'D': 0, 'E': -1, 'F': 2, 'G': 0, 'H': 0, 'I': 0, 'K': 1, 'L': 0, 'M': 0, 'N': 0, 'P': -1, 'Q': 0, 'R': -1, 'S': 2, 'T': 1, 'V': 1, 'W': 0, 'X': 0, 'Y': 0}, 1: {'A': 3, 'C': 0, 'D': 0, 'E': 0, 'F': -1, 'G': 2, 'H': 0, 'I': -1, 'K': 0, 'L': 0, 'M': 2, 'N': 0, 'P': 0, 'Q': 1, 'R': 0, 'S': 2, 'T': 0, 'V': -1, 'W': 0, 'X': 0, 'Y': 0}, 2: {'A': 0, 'C': 0, 'D': 0, 'E': -1, 'F': 0, 'G': 1, 'H': 0, 'I': 2, 'K': -1, 'L': 2, 'M': 0, 'N': 0, 'P': 3, 'Q': 0, 'R': -1, 'S': 0, 'T': -1, 'V': 2, 'W': 0, 'X': 0, 'Y': 0}, 3: {'A': 0, 'C': 0, 'D': 1, 'E': 2, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 1, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 1, 'R': 1, 'S': 1, 'T': 1, 'V': 2, 'W': 0, 'X': 0, 'Y': 0}, 4: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 10, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 5: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 1, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 2, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 6: {'A': 0, 'C': 0, 'D': 2, 'E': 2, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 1, 'R': 0, 'S': 1, 'T': 2, 'V': 1, 'W': 0, 'X': 0, 'Y': 0}, 7: {'A': 0, 'C': 0, 'D': 0, 'E': 2, 'F': 1, 'G': 0, 'H': 1, 'I': -1, 'K': 0, 'L': 1, 'M': -1, 'N': 0, 'P': 0, 'Q': 0, 'R': 1, 'S': 1, 'T': 2, 'V': 0, 'W': 0, 'X': 0, 'Y': 2}, 8: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 8, 'G': 0, 'H': 0, 'I': 10, 'K': 0, 'L': 10, 'M': 10, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 6, 'W': 0, 'X': 0, 'Y': 0}}
```

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/H2_Db_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/D_b_10.py`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-H2_Db_9 = {0: {'A': 2, 'C': 0, 'D': 0, 'E': -1, 'F': 2, 'G': 0, 'H': 0, 'I': 0, 'K': 1, 'L': 0, 'M': 0, 'N': 0, 'P': -1, 'Q': 0, 'R': -1, 'S': 2, 'T': 1, 'V': 1, 'W': 0, 'X': 0, 'Y': 0}, 1: {'A': 3, 'C': 0, 'D': 0, 'E': 0, 'F': -1, 'G': 2, 'H': 0, 'I': -1, 'K': 0, 'L': 0, 'M': 2, 'N': 0, 'P': 0, 'Q': 1, 'R': 0, 'S': 2, 'T': 0, 'V': -1, 'W': 0, 'X': 0, 'Y': 0}, 2: {'A': 0, 'C': 0, 'D': 0, 'E': -1, 'F': 0, 'G': 1, 'H': 0, 'I': 2, 'K': -1, 'L': 2, 'M': 0, 'N': 0, 'P': 3, 'Q': 0, 'R': -1, 'S': 0, 'T': -1, 'V': 2, 'W': 0, 'X': 0, 'Y': 0}, 3: {'A': 0, 'C': 0, 'D': 1, 'E': 2, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 1, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 1, 'R': 1, 'S': 1, 'T': 1, 'V': 2, 'W': 0, 'X': 0, 'Y': 0}, 4: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 10, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 5: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 1, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 2, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 6: {'A': 0, 'C': 0, 'D': 2, 'E': 2, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 1, 'R': 0, 'S': 1, 'T': 2, 'V': 1, 'W': 0, 'X': 0, 'Y': 0}, 7: {'A': 0, 'C': 0, 'D': 0, 'E': 2, 'F': 1, 'G': 0, 'H': 1, 'I': -1, 'K': 0, 'L': 1, 'M': -1, 'N': 0, 'P': 0, 'Q': 0, 'R': 1, 'S': 1, 'T': 2, 'V': 0, 'W': 0, 'X': 0, 'Y': 2}, 8: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 8, 'G': 0, 'H': 0, 'I': 10, 'K': 0, 'L': 10, 'M': 10, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 6, 'W': 0, 'X': 0, 'Y': 0}}
+D_b_10 = {0: {'A': 2, 'C': 0, 'D': 0, 'E': -1, 'F': 2, 'G': 0, 'H': 0, 'I': 0, 'K': 1, 'L': 0, 'M': 0, 'N': 0, 'P': -1, 'Q': 0, 'R': -1, 'S': 2, 'T': 1, 'V': 1, 'W': 0, 'X': 0, 'Y': 0}, 1: {'A': 3, 'C': 0, 'D': 0, 'E': 0, 'F': -1, 'G': 2, 'H': 0, 'I': -1, 'K': 0, 'L': 0, 'M': 2, 'N': 0, 'P': 0, 'Q': 1, 'R': 0, 'S': 2, 'T': 0, 'V': -1, 'W': 0, 'X': 0, 'Y': 0}, 2: {'A': 0, 'C': 0, 'D': 0, 'E': -1, 'F': 0, 'G': 1, 'H': 0, 'I': 2, 'K': -1, 'L': 2, 'M': 0, 'N': 0, 'P': 3, 'Q': 0, 'R': -1, 'S': 0, 'T': -1, 'V': 2, 'W': 0, 'X': 0, 'Y': 0}, 3: {'A': 0, 'C': 0, 'D': 1, 'E': 2, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 1, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 1, 'R': 1, 'S': 1, 'T': 1, 'V': 2, 'W': 0, 'X': 0, 'Y': 0}, 4: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 10, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 5: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 1, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 2, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 6: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 7: {'A': 0, 'C': 0, 'D': 2, 'E': 2, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 1, 'R': 0, 'S': 1, 'T': 2, 'V': 1, 'W': 0, 'X': 0, 'Y': 0}, 8: {'A': 0, 'C': 0, 'D': 0, 'E': 2, 'F': 1, 'G': 0, 'H': 1, 'I': -1, 'K': 0, 'L': 1, 'M': -1, 'N': 0, 'P': 0, 'Q': 0, 'R': 1, 'S': 1, 'T': 2, 'V': 0, 'W': 0, 'X': 0, 'Y': 2}, 9: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 8, 'G': 0, 'H': 0, 'I': 10, 'K': 0, 'L': 10, 'M': 10, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 6, 'W': 0, 'X': 0, 'Y': 0}}
```

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/H2_Kb_8.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/K_b_8.py`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-H2_Kb_8 = {0: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 1, 'K': 0, 'L': 1, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 1, 'S': 1, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 1: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 1, 'H': 0, 'I': 1, 'K': 0, 'L': 0, 'M': 0, 'N': 1, 'P': 0, 'Q': 0, 'R': 0, 'S': 1, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 2: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 1, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 1, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 6}, 3: {'A': 0, 'C': 0, 'D': 1, 'E': 1, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 1, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 1, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 4: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 10, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 10}, 5: {'A': 0, 'C': 0, 'D': 0, 'E': 1, 'F': 0, 'G': 0, 'H': 0, 'I': 1, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 1, 'S': 1, 'T': 1, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 6: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 1, 'L': 0, 'M': 0, 'N': 1, 'P': 0, 'Q': 1, 'R': 0, 'S': 0, 'T': 1, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 7: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 6, 'K': 0, 'L': 10, 'M': 6, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 6, 'W': 0, 'X': 0, 'Y': 0}}
+K_b_8 = {0: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 1, 'K': 0, 'L': 1, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 1, 'S': 1, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 1: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 1, 'H': 0, 'I': 1, 'K': 0, 'L': 0, 'M': 0, 'N': 1, 'P': 0, 'Q': 0, 'R': 0, 'S': 1, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 2: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 1, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 1, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 6}, 3: {'A': 0, 'C': 0, 'D': 1, 'E': 1, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 1, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 1, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 4: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 10, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 10}, 5: {'A': 0, 'C': 0, 'D': 0, 'E': 1, 'F': 0, 'G': 0, 'H': 0, 'I': 1, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 1, 'S': 1, 'T': 1, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 6: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 1, 'L': 0, 'M': 0, 'N': 1, 'P': 0, 'Q': 1, 'R': 0, 'S': 0, 'T': 1, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 7: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 6, 'K': 0, 'L': 10, 'M': 6, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 6, 'W': 0, 'X': 0, 'Y': 0}}
```

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/H2_Kd_10.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/K_d_10.py`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-H2_Kd_10 = {0: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 1, 'K': 2, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 1, 'S': 3, 'T': 2, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 1: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 6, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 10}, 2: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 1, 'K': 1, 'L': 3, 'M': 0, 'N': 0, 'P': 0, 'Q': 2, 'R': 0, 'S': 0, 'T': 0, 'V': 2, 'W': 0, 'X': 0, 'Y': 0}, 3: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 4: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 5: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 6: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 7: {'A': 0, 'C': 0, 'D': 0, 'E': 1, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 2, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 1, 'R': 0, 'S': 1, 'T': 4, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 8: {'A': 0, 'C': 0, 'D': 0, 'E': 1, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 1, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 2, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 1}, 9: {'A': 6, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 10, 'K': 0, 'L': 10, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 8, 'W': 0, 'X': 0, 'Y': 0}}
+K_d_10 = {0: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 1, 'K': 2, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 1, 'S': 3, 'T': 2, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 1: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 6, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 10}, 2: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 1, 'K': 1, 'L': 3, 'M': 0, 'N': 0, 'P': 0, 'Q': 2, 'R': 0, 'S': 0, 'T': 0, 'V': 2, 'W': 0, 'X': 0, 'Y': 0}, 3: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 4: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 5: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 6: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 7: {'A': 0, 'C': 0, 'D': 0, 'E': 1, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 2, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 1, 'R': 0, 'S': 1, 'T': 4, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 8: {'A': 0, 'C': 0, 'D': 0, 'E': 1, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 1, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 2, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 1}, 9: {'A': 6, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 10, 'K': 0, 'L': 10, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 8, 'W': 0, 'X': 0, 'Y': 0}}
```

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/H2_Kd_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/K_d_9.py`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-H2_Kd_9 = {0: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 1, 'K': 2, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 1, 'S': 3, 'T': 2, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 1: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 6, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 10}, 2: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 1, 'K': 1, 'L': 3, 'M': 0, 'N': 0, 'P': 0, 'Q': 2, 'R': 0, 'S': 0, 'T': 0, 'V': 2, 'W': 0, 'X': 0, 'Y': 0}, 3: {'A': 0, 'C': 0, 'D': 1, 'E': 0, 'F': -1, 'G': 2, 'H': 0, 'I': -1, 'K': 0, 'L': -1, 'M': -1, 'N': 0, 'P': 3, 'Q': 0, 'R': 0, 'S': 2, 'T': 2, 'V': 1, 'W': 0, 'X': 0, 'Y': 0}, 4: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': -1, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 1, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 2, 'T': 1, 'V': 2, 'W': 0, 'X': 0, 'Y': 0}, 5: {'A': 2, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 2, 'H': 0, 'I': 1, 'K': 2, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': -1, 'T': 0, 'V': 1, 'W': 0, 'X': 0, 'Y': 0}, 6: {'A': 0, 'C': 0, 'D': 0, 'E': 1, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 2, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 1, 'R': 0, 'S': 1, 'T': 4, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 7: {'A': 0, 'C': 0, 'D': 0, 'E': 1, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 1, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 2, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 1}, 8: {'A': 6, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 10, 'K': 0, 'L': 10, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 8, 'W': 0, 'X': 0, 'Y': 0}}
+K_d_9 = {0: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 1, 'K': 2, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 1, 'S': 3, 'T': 2, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 1: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 6, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 10}, 2: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 1, 'K': 1, 'L': 3, 'M': 0, 'N': 0, 'P': 0, 'Q': 2, 'R': 0, 'S': 0, 'T': 0, 'V': 2, 'W': 0, 'X': 0, 'Y': 0}, 3: {'A': 0, 'C': 0, 'D': 1, 'E': 0, 'F': -1, 'G': 2, 'H': 0, 'I': -1, 'K': 0, 'L': -1, 'M': -1, 'N': 0, 'P': 3, 'Q': 0, 'R': 0, 'S': 2, 'T': 2, 'V': 1, 'W': 0, 'X': 0, 'Y': 0}, 4: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': -1, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 1, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 2, 'T': 1, 'V': 2, 'W': 0, 'X': 0, 'Y': 0}, 5: {'A': 2, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 2, 'H': 0, 'I': 1, 'K': 2, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': -1, 'T': 0, 'V': 1, 'W': 0, 'X': 0, 'Y': 0}, 6: {'A': 0, 'C': 0, 'D': 0, 'E': 1, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 2, 'L': 0, 'M': 0, 'N': 0, 'P': 0, 'Q': 1, 'R': 0, 'S': 1, 'T': 4, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 7: {'A': 0, 'C': 0, 'D': 0, 'E': 1, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 1, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 2, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 1}, 8: {'A': 6, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 10, 'K': 0, 'L': 10, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 8, 'W': 0, 'X': 0, 'Y': 0}}
```

### Comparing `epytope-3.3.0/epytope/Data/pssms/syfpeithi/mat/H2_Ld_9.py` & `epytope-3.3.1/epytope/Data/pssms/syfpeithi/mat/L_d_9.py`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-H2_Ld_9 = {0: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 1, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 1}, 1: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 10, 'Q': 0, 'R': 0, 'S': 8, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 2: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 1, 'H': 1, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 1, 'Q': 2, 'R': 0, 'S': 1, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 1}, 3: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 1, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 1, 'M': 0, 'N': 0, 'P': 2, 'Q': 0, 'R': 1, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 4: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 2, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 1, 'P': 0, 'Q': 0, 'R': 0, 'S': 1, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 5: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 1, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 1, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 1, 'S': 0, 'T': 0, 'V': 0, 'W': 1, 'X': 0, 'Y': 0}, 6: {'A': 0, 'C': 0, 'D': 0, 'E': 1, 'F': 1, 'G': 0, 'H': 1, 'I': 0, 'K': 0, 'L': 1, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 1, 'V': 1, 'W': 0, 'X': 0, 'Y': 0}, 7: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 2, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 1, 'W': 0, 'X': 0, 'Y': 1}, 8: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 10, 'G': 0, 'H': 0, 'I': 6, 'K': 0, 'L': 10, 'M': 6, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}}
+L_d_9 = {0: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 1, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 1}, 1: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 10, 'Q': 0, 'R': 0, 'S': 8, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 2: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 1, 'H': 1, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 0, 'P': 1, 'Q': 2, 'R': 0, 'S': 1, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 1}, 3: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 1, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 1, 'M': 0, 'N': 0, 'P': 2, 'Q': 0, 'R': 1, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 4: {'A': 1, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 2, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 1, 'P': 0, 'Q': 0, 'R': 0, 'S': 1, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}, 5: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 1, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 1, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 1, 'S': 0, 'T': 0, 'V': 0, 'W': 1, 'X': 0, 'Y': 0}, 6: {'A': 0, 'C': 0, 'D': 0, 'E': 1, 'F': 1, 'G': 0, 'H': 1, 'I': 0, 'K': 0, 'L': 1, 'M': 0, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 1, 'V': 1, 'W': 0, 'X': 0, 'Y': 0}, 7: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 0, 'G': 0, 'H': 0, 'I': 0, 'K': 0, 'L': 0, 'M': 0, 'N': 2, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 1, 'W': 0, 'X': 0, 'Y': 1}, 8: {'A': 0, 'C': 0, 'D': 0, 'E': 0, 'F': 10, 'G': 0, 'H': 0, 'I': 6, 'K': 0, 'L': 10, 'M': 6, 'N': 0, 'P': 0, 'Q': 0, 'R': 0, 'S': 0, 'T': 0, 'V': 0, 'W': 0, 'X': 0, 'Y': 0}}
```

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0101_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0102_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0102_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0103_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0103_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0104_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0104_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0105_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0105_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0106_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0106_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0107_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0107_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0108_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0108_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0109_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0109_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0110_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0110_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0111_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0111_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0112_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0112_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0113_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0113_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0114_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0114_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0115_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0115_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0116_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0116_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0117_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0117_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0118_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0118_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0119_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0119_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0120_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0120_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0121_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0121_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0122_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0122_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0123_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0123_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0124_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0124_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0125_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0125_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0126_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0126_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0127_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0127_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0128_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0128_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0129_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0129_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0130_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0130_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0131_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0131_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0132_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0132_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0134_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0134_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0135_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0135_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0136_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0136_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0301_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0301_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0302_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0302_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0303_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0303_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0304_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0304_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0305_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0305_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0306_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0306_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0307_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0307_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0308_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0308_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0309_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0309_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0310_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0310_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0311_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0311_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0312_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0312_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0313_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0313_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0314_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0314_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0315_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0315_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0316_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0316_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0317_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0317_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0318_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0318_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0319_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0319_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0320_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0320_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0321_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0321_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0322_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0322_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0323_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0323_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0324_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0324_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0325_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0325_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0326_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0326_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0327_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0327_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0328_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0328_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0329_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0329_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0330_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0330_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0331_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0331_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0332_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0332_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0333_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0333_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0334_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0334_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0335_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0335_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0336_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0336_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0337_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0337_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0338_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0338_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0339_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0339_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0340_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0340_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0341_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0341_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0342_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0342_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0343_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0343_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0344_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0344_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0345_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0345_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0346_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0346_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0347_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0347_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0348_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0348_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0349_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0349_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0350_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0350_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0351_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0351_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0352_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0352_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0353_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0353_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0354_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0354_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0355_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0355_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0356_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0356_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0357_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0357_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0358_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0358_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0359_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0359_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0360_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0360_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0361_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0361_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0362_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0362_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0363_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0363_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0364_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0364_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0401_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0401_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0402_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0402_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0403_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0403_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0404_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0404_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0405_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0405_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0406_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0406_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0407_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0407_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0408_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0408_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0409_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0409_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0410_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0410_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0411_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0411_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0412_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0412_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0413_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0413_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0414_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0414_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0415_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0415_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0416_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0416_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0417_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0417_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0418_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0418_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0419_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0419_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0420_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0420_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0421_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0421_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0422_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0422_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0423_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0423_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0424_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0424_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0425_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0425_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0426_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0426_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0427_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0427_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0428_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0428_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0429_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0429_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0430_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0430_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0431_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0431_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0432_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0432_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0433_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0433_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0434_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0434_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0435_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0435_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0436_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0436_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0437_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0437_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0438_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0438_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0439_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0439_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0440_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0440_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0441_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0441_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0442_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0442_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0443_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0443_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0444_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0444_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0445_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0445_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0446_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0446_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0447_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0447_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0448_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0448_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0449_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0449_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0450_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0450_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0451_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0451_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0452_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0452_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0453_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0453_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0454_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0454_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0455_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0455_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0456_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0456_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0457_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0457_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0458_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0458_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0459_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0459_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0460_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0460_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0461_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0461_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0462_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0462_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0463_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0463_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0464_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0464_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0465_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0465_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0466_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0466_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0467_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0467_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0468_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0468_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0469_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0469_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0470_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0470_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0471_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0471_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0472_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0472_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0473_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0473_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0474_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0474_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0475_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0475_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0476_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0476_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0477_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0477_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0478_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0478_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0479_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0479_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0480_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0480_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0482_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0482_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0483_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0483_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0484_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0484_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0485_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0485_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0486_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0486_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0487_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0487_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0488_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0488_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0489_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0489_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0490_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0490_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0491_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0491_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0492_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0492_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0493_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0493_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0495_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0495_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0496_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0496_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0497_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0497_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0498_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0498_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0701_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0701_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0703_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0703_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0704_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0704_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0705_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0705_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0706_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0706_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0707_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0707_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0708_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0708_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0709_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0709_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0711_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0711_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0712_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0712_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0713_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0713_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0714_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0714_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0715_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0715_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0716_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0716_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0717_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0717_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0718_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0718_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0719_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0719_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0720_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0720_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0721_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0721_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0801_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0801_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0802_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0802_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0803_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0803_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0804_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0804_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0805_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0805_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0806_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0806_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0807_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0807_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0808_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0808_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0809_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0809_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0810_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0810_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0811_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0811_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0812_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0812_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0813_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0813_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0814_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0814_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0815_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0815_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0816_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0816_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0817_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0817_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0818_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0818_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0819_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0819_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0820_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0820_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0821_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0821_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0822_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0822_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0823_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0823_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0824_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0824_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0825_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0825_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0826_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0826_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0827_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0827_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0828_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0828_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0829_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0829_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0830_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0830_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0831_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0831_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0832_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0832_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0833_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0833_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0834_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0834_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0835_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0835_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0836_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0836_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0837_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0837_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0838_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0838_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0839_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0839_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0840_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0840_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0841_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0841_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0842_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0842_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0843_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0843_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0844_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0844_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0845_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0845_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0901_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0901_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0902_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0902_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0903_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0903_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0904_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0904_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0905_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0905_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0906_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0906_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0907_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0907_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0908_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0908_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0909_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0909_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0910_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0910_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0911_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0911_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_0912_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_0912_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1001_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1001_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1002_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1002_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1003_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1003_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1101_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1102_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1102_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1103_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1103_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1104_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1104_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1105_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1105_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1106_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1106_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1107_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1107_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1108_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1108_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1109_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1109_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1110_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1110_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1111_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1111_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1112_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1112_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1113_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1113_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1114_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1114_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1115_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1115_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1116_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1116_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1117_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1117_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1118_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1118_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1119_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1119_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1120_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1120_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1121_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1121_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1122_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1122_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1123_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1123_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1124_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1124_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1125_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1125_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1126_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1126_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1127_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1127_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1128_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1128_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1129_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1129_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1130_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1130_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1131_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1131_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1132_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1132_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1133_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1133_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1134_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1134_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1135_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1135_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1136_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1136_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1137_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1137_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1138_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1138_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1139_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1139_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1140_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1140_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1141_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1141_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1142_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1142_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1143_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1143_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1144_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1144_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1145_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1145_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1146_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1146_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1147_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1147_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1148_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1148_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1149_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1149_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1150_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1150_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1151_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1151_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1152_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1152_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1153_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1153_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1154_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1154_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1155_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1155_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1156_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1156_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1157_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1157_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1158_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1158_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1159_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1159_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1160_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1160_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1161_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1161_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1162_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1162_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1163_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1163_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1164_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1164_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1165_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1165_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1166_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1166_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1167_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1167_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1168_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1168_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1169_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1169_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1170_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1170_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1172_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1172_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1173_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1173_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1174_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1174_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1175_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1175_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1176_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1176_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1177_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1177_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1178_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1178_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1179_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1179_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1180_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1180_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1181_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1181_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1182_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1182_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1183_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1183_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1184_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1184_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1185_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1185_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1186_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1186_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1187_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1187_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1188_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1188_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1189_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1189_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1190_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1190_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1191_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1191_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1192_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1192_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1193_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1193_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1194_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1194_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1195_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1195_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1196_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1196_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1197_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1197_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1198_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1198_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1199_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1199_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1201_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1201_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1202_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1202_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1203_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1203_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1204_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1204_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1205_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1205_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1206_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1206_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1207_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1207_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1208_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1208_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1209_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1209_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1210_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1210_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1211_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1211_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1212_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1212_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1213_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1213_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1214_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1214_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1215_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1215_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1216_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1216_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1217_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1217_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1218_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1218_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1219_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1219_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1220_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1220_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1221_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1221_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1222_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1222_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1223_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1223_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1225_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1225_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1226_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1226_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1227_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1227_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1301_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1301_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1302_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1302_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1303_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1303_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1304_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1304_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1305_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1305_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1306_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1306_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1307_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1307_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1308_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1308_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1309_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1309_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1310_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1310_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1311_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1311_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1312_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1312_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1313_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1313_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1314_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1314_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1315_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1315_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1316_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1316_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1317_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1317_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1318_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1318_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1319_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1319_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1320_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1320_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1321_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1321_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1322_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1322_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1323_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1323_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1324_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1324_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1325_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1325_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1326_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1326_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1327_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1327_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1328_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1328_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1329_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1329_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1330_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1330_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1331_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1331_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1332_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1332_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1333_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1333_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1334_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1334_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1335_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1335_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1336_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1336_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1337_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1337_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1338_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1338_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1339_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1339_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1340_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1340_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1341_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1341_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1342_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1342_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1343_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1343_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1344_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1344_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1345_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1345_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1346_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1346_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1347_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1347_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1348_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1348_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1349_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1349_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1350_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1350_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1351_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1351_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1352_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1352_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1353_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1353_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1354_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1354_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1355_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1355_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1356_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1356_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1357_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1357_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1358_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1358_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1359_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1359_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1360_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1360_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1361_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1361_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1362_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1362_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1363_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1363_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1364_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1364_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1365_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1365_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1366_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1366_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1367_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1367_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1368_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1368_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1369_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1369_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1370_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1370_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1371_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1371_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1372_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1372_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1373_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1373_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1374_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1374_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1375_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1375_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1376_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1376_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1377_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1377_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1378_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1378_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1379_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1379_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1380_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1380_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1381_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1381_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1382_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1382_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1383_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1383_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1384_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1384_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1385_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1385_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1386_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1386_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1387_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1387_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1388_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1388_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1389_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1389_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1390_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1390_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1391_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1391_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1392_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1392_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1393_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1393_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1394_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1394_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1395_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1395_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1396_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1396_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1397_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1397_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1398_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1398_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1399_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1399_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1401_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1401_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1402_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1402_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1403_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1403_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1404_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1404_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1405_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1405_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1406_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1406_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1407_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1407_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1408_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1408_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1409_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1409_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1410_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1410_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1411_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1411_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1412_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1412_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1413_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1413_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1414_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1414_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1415_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1415_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1416_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1416_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1417_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1417_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1418_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1418_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1419_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1419_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1420_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1420_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1421_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1421_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1422_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1422_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1423_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1423_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1424_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1424_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1425_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1425_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1426_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1426_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1427_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1427_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1428_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1428_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1429_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1429_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1430_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1430_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1431_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1431_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1432_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1432_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1433_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1433_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1434_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1434_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1435_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1435_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1436_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1436_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1437_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1437_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1438_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1438_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1439_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1439_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1440_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1440_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1441_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1441_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1442_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1442_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1443_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1443_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1444_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1444_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1445_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1445_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1446_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1446_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1447_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1447_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1448_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1448_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1449_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1449_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1450_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1450_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1451_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1451_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1452_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1452_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1453_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1453_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1454_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1454_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1455_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1455_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1456_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1456_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1457_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1457_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1458_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1458_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1459_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1459_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1460_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1460_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1461_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1461_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1462_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1462_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1463_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1463_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1464_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1464_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1465_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1465_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1467_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1467_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1468_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1468_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1469_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1469_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1470_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1470_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1471_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1471_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1472_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1472_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1473_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1473_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1474_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1474_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1475_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1475_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1476_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1476_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1477_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1477_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1478_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1478_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1479_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1479_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1480_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1480_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1481_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1481_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1482_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1482_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1483_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1483_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1484_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1484_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1485_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1485_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1486_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1486_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1487_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1487_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1488_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1488_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1489_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1489_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1490_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1490_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1491_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1491_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1493_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1493_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1494_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1494_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1495_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1495_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1496_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1496_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1497_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1497_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1498_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1498_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1499_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1499_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1501_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1501_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1502_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1502_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1503_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1503_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1504_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1504_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1505_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1505_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1506_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1506_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1507_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1507_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1508_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1508_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1509_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1509_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1510_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1510_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1511_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1511_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1512_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1512_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1513_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1513_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1514_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1514_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1515_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1515_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1516_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1516_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1518_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1518_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1519_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1519_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1520_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1520_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1521_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1521_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1522_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1522_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1523_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1523_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1524_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1524_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1525_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1525_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1526_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1526_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1527_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1527_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1528_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1528_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1529_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1529_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1530_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1530_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1531_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1531_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1532_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1532_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1533_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1533_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1534_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1534_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1535_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1535_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1536_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1536_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1537_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1537_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1538_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1538_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1539_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1539_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1540_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1540_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1541_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1541_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1542_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1542_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1543_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1543_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1544_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1544_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1545_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1545_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1546_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1546_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1547_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1547_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1548_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1548_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1549_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1549_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1551_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1551_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1552_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1552_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1553_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1553_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1554_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1554_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1555_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1555_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1556_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1556_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1557_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1557_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1601_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1601_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1602_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1602_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1603_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1603_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1604_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1604_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1605_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1605_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1607_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1607_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1608_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1608_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1609_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1609_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1610_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1610_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1611_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1611_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1612_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1612_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1614_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1614_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1615_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1615_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1616_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1616_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1617_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1617_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB1_1618_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB1_1618_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0101_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0102_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0102_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0103_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0103_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0104_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0104_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0105_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0105_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0106_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0106_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0107_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0107_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0108_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0108_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0109_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0109_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0110_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0110_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0111_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0111_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0112_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0112_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0113_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0113_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0114_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0114_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0115_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0115_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0201_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0201_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0202_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0202_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0203_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0203_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0204_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0204_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0205_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0205_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0206_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0206_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0207_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0207_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0208_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0208_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0209_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0209_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0210_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0210_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0211_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0211_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0212_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0212_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0213_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0213_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0214_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0214_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0215_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0215_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0216_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0216_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0217_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0217_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0218_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0218_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0219_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0219_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0220_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0220_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0221_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0221_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0222_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0222_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0223_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0223_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0224_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0224_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0225_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0225_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0226_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0226_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0227_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0227_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0228_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0228_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0301_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0301_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0302_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0302_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB3_0303_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB3_0303_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB4_0101_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB4_0101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB4_0103_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB4_0103_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB4_0104_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB4_0104_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB4_0105_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB4_0105_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB4_0106_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB4_0106_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB4_0107_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB4_0107_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB4_0108_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB4_0108_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0101_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0101_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0102_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0102_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0104_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0104_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0105_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0105_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0106_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0106_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0107_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0107_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0108_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0108_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0109_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0109_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0111_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0111_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0112_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0112_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0113_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0113_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0114_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0114_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0202_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0202_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0203_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0203_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0204_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0204_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/pssms/tepitopepan/mat/DRB5_0205_9.py` & `epytope-3.3.1/epytope/Data/pssms/tepitopepan/mat/DRB5_0205_9.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/ann/mhcflurry_1_2_2.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/ann/mhcflurry_1_2_2.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/ann/mhcflurry_1_4_3.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/ann/mhcflurry_1_4_3.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/ann/mhcnuggets_class_1_2_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/ann/mhcnuggets_class_1_2_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/ann/mhcnuggets_class_1_2_3_2.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/ann/mhcnuggets_class_1_2_3_2.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/ann/mhcnuggets_class_2_2_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/ann/mhcnuggets_class_2_2_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/ann/mhcnuggets_class_2_2_3_2.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/ann/mhcnuggets_class_2_2_3_2.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/external/netMHCstabpan_1_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/external/netMHCstabpan_1_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/external/netctlpan_1_1.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/external/netctlpan_1_1.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcII_2_2.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcII_2_2.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcII_2_3.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcII_2_3.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcIIpan_3_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcIIpan_3_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcIIpan_3_1.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcIIpan_3_1.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcIIpan_4_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcIIpan_4_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhc_3_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhc_3_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhc_3_4.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhc_3_4.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhc_4_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhc_4_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcpan_2_4.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcpan_2_4.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcpan_2_8.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcpan_2_8.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcpan_3_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcpan_3_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcpan_4_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcpan_4_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/external/netmhcpan_4_1.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/external/netmhcpan_4_1.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/external/pickpocket_1_1.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/external/pickpocket_1_1.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/pssm/arb_1_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/pssm/arb_1_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/pssm/bimas_1_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/pssm/bimas_1_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/pssm/calisimm_1_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/pssm/calisimm_1_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/pssm/hammer_1_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/pssm/hammer_1_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/pssm/smm_1_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/pssm/smm_1_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/pssm/smmpmbec_1_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/pssm/smmpmbec_1_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/pssm/syfpeithi_1_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/pssm/syfpeithi_1_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/Data/supportedAlleles/pssm/tepitopepan_1_0.py` & `epytope-3.3.1/epytope/Data/supportedAlleles/pssm/tepitopepan_1_0.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/EpitopeAssembly/EpitopeAssembly.py` & `epytope-3.3.1/epytope/EpitopeAssembly/EpitopeAssembly.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/EpitopePrediction/ANN.py` & `epytope-3.3.1/epytope/EpitopePrediction/ANN.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/EpitopePrediction/External.py` & `epytope-3.3.1/epytope/EpitopePrediction/External.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/EpitopePrediction/PSSM.py` & `epytope-3.3.1/epytope/EpitopePrediction/PSSM.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/EpitopePrediction/__init__.py` & `epytope-3.3.1/epytope/EpitopePrediction/__init__.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/EpitopeSelection/OptiTope.py` & `epytope-3.3.1/epytope/EpitopeSelection/OptiTope.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/HLAtyping/External.py` & `epytope-3.3.1/epytope/HLAtyping/External.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/HLAtyping/__init__.py` & `epytope-3.3.1/epytope/HLAtyping/__init__.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/IO/ADBAdapter.py` & `epytope-3.3.1/epytope/IO/ADBAdapter.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/IO/EnsemblAdapter.py` & `epytope-3.3.1/epytope/IO/EnsemblAdapter.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/IO/FileReader.py` & `epytope-3.3.1/epytope/IO/FileReader.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/IO/MartsAdapter.py` & `epytope-3.3.1/epytope/IO/MartsAdapter.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/IO/RefSeqAdapter.py` & `epytope-3.3.1/epytope/IO/RefSeqAdapter.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/IO/UniProtAdapter.py` & `epytope-3.3.1/epytope/IO/UniProtAdapter.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/IO/Utils.py` & `epytope-3.3.1/epytope/IO/Utils.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/IO/__init__.py` & `epytope-3.3.1/epytope/IO/__init__.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/TAPPrediction/PSSM.py` & `epytope-3.3.1/epytope/TAPPrediction/PSSM.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/TAPPrediction/__init__.py` & `epytope-3.3.1/epytope/TAPPrediction/__init__.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/DummyAdapter.py` & `epytope-3.3.1/epytope/test/DummyAdapter.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/DummyEpitopePredictor.py` & `epytope-3.3.1/epytope/test/DummyEpitopePredictor.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/TestAllele.py` & `epytope-3.3.1/epytope/test/TestAllele.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/TestCleavagePrediction.py` & `epytope-3.3.1/epytope/test/TestCleavagePrediction.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/TestEpitopeAssembly.py` & `epytope-3.3.1/epytope/test/TestEpitopeAssembly.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/TestEpitopePrediction.py` & `epytope-3.3.1/epytope/test/TestEpitopePrediction.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     def setUp(self):
         #Peptides of different length 9,10,11,12,13,14,15
         self.peptides_mhcI = [Peptide("SYFPEITHI"), Peptide("IHTIEPFYS")]
         self.peptides_mhcII = [Peptide("SYFPEITHI"), Peptide("IHTIEPFYSAAAAAA")]
         self.mhcI = [Allele("HLA-B*15:01"), Allele("HLA-A*02:01")]
         self.mhcII = [Allele("HLA-DRB1*07:01"), Allele("HLA-DRB1*15:01")]
+        self.mouse = [Allele("H2-Kd"), Allele("H2-Kb")]
 
     def test_multiple_peptide_input_mhcI(self):
             for m in EpitopePredictorFactory.available_methods():
                 model = EpitopePredictorFactory(m)
                 if not isinstance(model, AExternalEpitopePrediction):
                     if all(a in model.supportedAlleles for a in self.mhcI):
                         res = model.predict(self.peptides_mhcI, alleles=self.mhcI)
@@ -46,11 +47,23 @@
 
     def test_single_peptide_input_mhcII(self):
             for m in EpitopePredictorFactory.available_methods():
                 model = EpitopePredictorFactory(m)
                 if not isinstance(model, AExternalEpitopePrediction):
                     if all(a in model.supportedAlleles for a in self.mhcII):
                         res = model.predict(self.peptides_mhcII, alleles=self.mhcII)
-
+    
+    def test_prediction_for_mouse(self):
+        syfpeithi = EpitopePredictorFactory("Syfpeithi")
+        res = syfpeithi.predict(self.peptides_mhcI, alleles=self.mouse)
+
+        mhcflurry = EpitopePredictorFactory("mhcflurry")
+        mhcnuggets = EpitopePredictorFactory("mhcnuggets-class-1")
+        netmhc = EpitopePredictorFactory("netmhc")
+        netmhcpan = EpitopePredictorFactory("netmhcpan")
+
+        for allele in self.mouse:
+            for m in [mhcflurry, mhcnuggets, netmhc, netmhcpan]:
+                self.assertTrue(allele in m.supportedAlleles)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `epytope-3.3.0/epytope/test/TestGenerator.py` & `epytope-3.3.1/epytope/test/TestGenerator.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/TestIO.py` & `epytope-3.3.1/epytope/test/TestIO.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/TestOptiTope.py` & `epytope-3.3.1/epytope/test/TestOptiTope.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/TestPeptide.py` & `epytope-3.3.1/epytope/test/TestPeptide.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/TestPredictionVersioning.py` & `epytope-3.3.1/epytope/test/TestPredictionVersioning.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/TestProtein.py` & `epytope-3.3.1/epytope/test/TestProtein.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/TestSpacerDesign.py` & `epytope-3.3.1/epytope/test/TestSpacerDesign.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/TestTAPPrediction.py` & `epytope-3.3.1/epytope/test/TestTAPPrediction.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/TestTranscript.py` & `epytope-3.3.1/epytope/test/TestTranscript.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/TestVariant.py` & `epytope-3.3.1/epytope/test/TestVariant.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/VariantsForTesting.py` & `epytope-3.3.1/epytope/test/VariantsForTesting.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/external/TestExternalCleavagePrediction.py` & `epytope-3.3.1/epytope/test/external/TestExternalCleavagePrediction.py`

 * *Files identical despite different names*

### Comparing `epytope-3.3.0/epytope/test/external/TestExternalEpitopePrediction.py` & `epytope-3.3.1/epytope/test/external/TestExternalEpitopePrediction.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
     def setUp(self):
         self.peptides_mhcI = [Peptide("SYFPEITHI"), Peptide("IHTIEPFYS")]
         self.peptides_mhcII = [Peptide("AAAAAASYFPEITHI"), Peptide("IHTIEPFYSAAAAAA")]
         self.mhcI = [Allele("HLA-B*07:02"), Allele("HLA-A*02:01")]
         self.mhcII = [Allele("HLA-DRB1*07:01"), Allele("HLA-DRB1*15:01")]
         self.mhcII_combined_alleles = [CombinedAllele("DPA1*01:03-DPB1*01:01"), CombinedAllele("DQA1*06:02-DQB1*06:31")]
+        self.mouse = [Allele("H2-Kd"), Allele("H2-Kb")]
         self.transcript = Transcript("")
 
     def test_multiple_inputs(self):
         for m in EpitopePredictorFactory.available_methods():
             for v in EpitopePredictorFactory.available_methods()[m]:
                 mo = EpitopePredictorFactory(m, version=v)
                 if isinstance(mo, AExternalEpitopePrediction) and not (mo.version=="0.1" and mo.name=="netmhc"):
@@ -102,27 +103,29 @@
         with self.assertRaises(ValueError):
             EpitopePredictorFactory("NetMHC").predict(self.mhcI, alleles=self.transcript)
 
     def test_wrong_internal_to_external_version(self):
         with self.assertRaises(RuntimeError):
             EpitopePredictorFactory("NetMHC", version="0.1").predict(self.peptides_mhcI, alleles=self.mhcI)
 
-#--sort flag not supported by newer versions
-
-    # def test_path_option_and_optional_parameters_netmhc(self):
-    #     netmhc = EpitopePredictorFactory("NetMHC")
-    #     exe = netmhc.command.split()[0]
-    #     for try_path in os.environ["PATH"].split(os.pathsep):
-    #         try_path = try_path.strip('"')
-    #         exe_try = os.path.join(try_path, exe).strip()
-    #         if os.path.isfile(exe_try) and os.access(exe_try, os.X_OK):
-    #             r = netmhc.predict(self.peptides_mhcI, alleles=self.mhcI, command=exe_try, options="--sort", chunksize=1)
-    #             self.assertTrue(len(r) == len(self.peptides_mhcI))
-    #             self.assertAlmostEqual(r["A*02:01"]["SYFPEITHI"]["netmhc"], 0.150579105869, places=7, msg=None, delta=None)
-    #             self.assertAlmostEqual(r["A*02:01"]["IHTIEPFYS"]["netmhc"], 0.0619540879359, places=7, msg=None, delta=None)
+    def test_mouse_allele_prediction(self):
+        for m in EpitopePredictorFactory.available_methods():
+            for v in EpitopePredictorFactory.available_methods()[m]:
+                mo = EpitopePredictorFactory(m, version=v)
+                if isinstance(mo, AExternalEpitopePrediction) and not (mo.version=="0.1" and mo.name=="netmhc"):
+                    print("Testing", mo.name, "version", mo.version)
+                    try:
+                        if any(a.name in mo.supportedAlleles for a in self.mouse):
+                            mo.predict(self.peptides_mhcI[0], alleles=self.mouse)
+                        print("Success")
+                    except RuntimeError as e: #catch only those stemming from binary unavailability
+                        if "could not be found in PATH" not in e.message:
+                            raise e #all others do not except
+                        else:
+                            print(mo.name, "not available")
 
     def test_path_and_optional_parameters_netctl(self):
         netctlpan = EpitopePredictorFactory("NetCTLpan")
         exe = netctlpan.command.split()[0]
         for try_path in os.environ["PATH"].split(os.pathsep):
             try_path = try_path.strip('"')
             exe_try = os.path.join(try_path, exe).strip()
```

### Comparing `epytope-3.3.0/epytope.egg-info/PKG-INFO` & `epytope-3.3.1/epytope.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epytope
-Version: 3.3.0
+Version: 3.3.1
 Summary: A Framework for Epitope Detection and Vaccine Design
 Home-page: https://github.com/KohlbacherLab/epytope
 Author: Benjamin Schubert, Mathias Walzer, Christopher Mohr, Leon Kuchenbecker
 Author-email: benjamin.schubert@helmholtz-muenchen.de, walzer@ebi.ac.uk, christopher.mohr@uni-tuebingen.de, leon.kuchenbecker@uni-tuebingen.de 
 Maintainer: Christopher Mohr
 Maintainer-email: christopher.mohr@uni-tuebingen.de
 License: BSD
@@ -21,15 +21,16 @@
 
 ![PyPi](https://github.com/KohlbacherLab/epytope/actions/workflows/pypi-publish.yml/badge.svg)
 ![Tests](https://github.com/KohlbacherLab/epytope/actions/workflows/python-test-conda.yml/badge.svg)
 ![Tests external](https://github.com/KohlbacherLab/epytope/actions/workflows/python-test-conda-external.yml/badge.svg)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/epytope/badges/version.svg)](https://anaconda.org/bioconda/epytope)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/epytope/badges/latest_release_date.svg)](https://anaconda.org/bioconda/epytope)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![Anaconda-Server Badge](https://anaconda.org/bioconda/epytope/badges/installer/conda.svg)](https://conda.anaconda.org/bioconda)
+[![Anaconda-Server Badge](https://anaconda.org/bioconda/epytope/badges/platforms.svg
+)](https://anaconda.org/bioconda/epytope)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/epytope/badges/downloads.svg)](https://anaconda.org/bioconda/epytope)
 
 Copyright 2014 by Benjamin Schuber, Mathias Walzer, Philipp Brachvogel, Andras Szolek, Christopher Mohr, and Oliver Kohlbacher
 
 **epytope** is a framework for T-cell epitope detection, and vaccine design. It offers consistent, easy, and simultaneous access to well established prediction methods of computational immunology. **epytope** can handle polymorphic proteins and offers analysis tools to select, assemble, and design linker sequences for string-of-beads epitope-based vaccines. It is implemented in Python in a modular way and can easily be extended by user defined methods.
 
 ## Copyright
```

### Comparing `epytope-3.3.0/epytope.egg-info/SOURCES.txt` & `epytope-3.3.1/epytope.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -825,23 +825,23 @@
 epytope/Data/pssms/syfpeithi/mat/C_1701_8.py
 epytope/Data/pssms/syfpeithi/mat/C_1701_9.py
 epytope/Data/pssms/syfpeithi/mat/DRB1_0101_9.py
 epytope/Data/pssms/syfpeithi/mat/DRB1_0301_9.py
 epytope/Data/pssms/syfpeithi/mat/DRB1_0701_9.py
 epytope/Data/pssms/syfpeithi/mat/DRB1_1101_9.py
 epytope/Data/pssms/syfpeithi/mat/DRB1_1501_9.py
+epytope/Data/pssms/syfpeithi/mat/D_b_10.py
+epytope/Data/pssms/syfpeithi/mat/D_b_9.py
 epytope/Data/pssms/syfpeithi/mat/G_0101_10.py
 epytope/Data/pssms/syfpeithi/mat/G_0101_8.py
 epytope/Data/pssms/syfpeithi/mat/G_0101_9.py
-epytope/Data/pssms/syfpeithi/mat/H2_Db_10.py
-epytope/Data/pssms/syfpeithi/mat/H2_Db_9.py
-epytope/Data/pssms/syfpeithi/mat/H2_Kb_8.py
-epytope/Data/pssms/syfpeithi/mat/H2_Kd_10.py
-epytope/Data/pssms/syfpeithi/mat/H2_Kd_9.py
-epytope/Data/pssms/syfpeithi/mat/H2_Ld_9.py
+epytope/Data/pssms/syfpeithi/mat/K_b_8.py
+epytope/Data/pssms/syfpeithi/mat/K_d_10.py
+epytope/Data/pssms/syfpeithi/mat/K_d_9.py
+epytope/Data/pssms/syfpeithi/mat/L_d_9.py
 epytope/Data/pssms/syfpeithi/mat/__init__.py
 epytope/Data/pssms/tepitopepan/__init__.py
 epytope/Data/pssms/tepitopepan/mat/DRB1_0101_9.py
 epytope/Data/pssms/tepitopepan/mat/DRB1_0102_9.py
 epytope/Data/pssms/tepitopepan/mat/DRB1_0103_9.py
 epytope/Data/pssms/tepitopepan/mat/DRB1_0104_9.py
 epytope/Data/pssms/tepitopepan/mat/DRB1_0105_9.py
```

### Comparing `epytope-3.3.0/setup.py` & `epytope-3.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='epytope',
 
     # Version:
-    version='3.3.0',
+    version='3.3.1',
 
     description='A Framework for Epitope Detection and Vaccine Design',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     # The project's main homepage.
     url='https://github.com/KohlbacherLab/epytope',
@@ -98,15 +98,15 @@
     #    ],
     #},
 
     # Run-time dependencies. (will be installed by pip when epytope is installed)
     # TODO: find alternative for SMVlight scikitlearn
     install_requires=[
             'setuptools',
-            'pandas',
+            'pandas>=1.3.5',        # See issue #84
             'pyomo>=4.0',
             'PyMySQL',
             'biopython',
             'PyVCF3',
             'mhcflurry<=1.4.3',
             'mhcnuggets==2.3.2',
             'keras<=2.3.1',         # legacy tensorflow required by mhcnuggets resolves to incompatible keras version
```

