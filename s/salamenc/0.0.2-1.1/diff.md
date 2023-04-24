# Comparing `tmp/SalamEnc-0.0.2.tar.gz` & `tmp/salamenc-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SalamEnc-0.0.2.tar", last modified: Sun Aug 28 22:12:41 2022, max compression
+gzip compressed data, was "salamenc-1.1.tar", last modified: Mon Apr 24 23:40:59 2023, max compression
```

## Comparing `SalamEnc-0.0.2.tar` & `salamenc-1.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwx---   0 root         (0)     9997        0 2022-08-28 22:12:41.005287 SalamEnc-0.0.2/
--rw-rw----   0 root         (0)     9997     1068 2022-04-08 08:09:49.000000 SalamEnc-0.0.2/LICENSE
--rw-rw----   0 root         (0)     9997     1377 2022-08-28 22:12:40.985287 SalamEnc-0.0.2/PKG-INFO
--rw-rw----   0 root         (0)     9997      825 2022-08-28 21:53:03.000000 SalamEnc-0.0.2/README.md
--rw-rw----   0 root         (0)     9997       38 2022-08-28 22:12:41.005287 SalamEnc-0.0.2/setup.cfg
--rw-rw----   0 root         (0)     9997     1134 2022-08-28 22:10:31.000000 SalamEnc-0.0.2/setup.py
-drwxrwx---   0 root         (0)     9997        0 2022-08-28 22:12:40.675287 SalamEnc-0.0.2/src/
-drwxrwx---   0 root         (0)     9997        0 2022-08-28 22:12:40.855287 SalamEnc-0.0.2/src/SalamEnc/
--rw-rw----   0 root         (0)     9997     2815 2022-04-08 08:49:58.000000 SalamEnc-0.0.2/src/SalamEnc/SalamEnc.py
--rw-rw----   0 root         (0)     9997       59 2022-08-28 21:51:19.000000 SalamEnc-0.0.2/src/SalamEnc/__init__.py
-drwxrwx---   0 root         (0)     9997        0 2022-08-28 22:12:40.965287 SalamEnc-0.0.2/src/SalamEnc.egg-info/
--rw-rw----   0 root         (0)     9997     1377 2022-08-28 22:12:40.000000 SalamEnc-0.0.2/src/SalamEnc.egg-info/PKG-INFO
--rw-rw----   0 root         (0)     9997      220 2022-08-28 22:12:40.000000 SalamEnc-0.0.2/src/SalamEnc.egg-info/SOURCES.txt
--rw-rw----   0 root         (0)     9997        1 2022-08-28 22:12:40.000000 SalamEnc-0.0.2/src/SalamEnc.egg-info/dependency_links.txt
--rw-rw----   0 root         (0)     9997        9 2022-08-28 22:12:40.000000 SalamEnc-0.0.2/src/SalamEnc.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-24 23:40:59.659005 salamenc-1.1/
+-rw-rw----   0 root         (0) everybody  (9997)     1061 2022-07-07 15:21:40.000000 salamenc-1.1/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     2053 2023-04-24 23:40:59.639005 salamenc-1.1/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     1446 2023-04-24 23:38:49.000000 salamenc-1.1/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-24 23:40:59.499004 salamenc-1.1/salamenc/
+-rw-rw----   0 root         (0) everybody  (9997)       23 2023-04-24 23:39:13.000000 salamenc-1.1/salamenc/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    23109 2023-04-24 23:27:59.000000 salamenc-1.1/salamenc/salamenc.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-24 23:40:59.619005 salamenc-1.1/salamenc.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     2053 2023-04-24 23:40:59.000000 salamenc-1.1/salamenc.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      196 2023-04-24 23:40:59.000000 salamenc-1.1/salamenc.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-24 23:40:59.000000 salamenc-1.1/salamenc.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        9 2023-04-24 23:40:59.000000 salamenc-1.1/salamenc.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-24 23:40:59.659005 salamenc-1.1/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1162 2023-04-24 23:38:30.000000 salamenc-1.1/setup.py
```

### Comparing `SalamEnc-0.0.2/LICENSE` & `salamenc-1.1/LICENSE`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 keegang6705
+Copyright (c) 2021 NOVA
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

