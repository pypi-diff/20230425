# Comparing `tmp/mkdocs-glightbox-0.3.3.tar.gz` & `tmp/mkdocs-glightbox-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-glightbox-0.3.3.tar", last modified: Thu Apr 20 14:43:58 2023, max compression
+gzip compressed data, was "mkdocs-glightbox-0.3.4.tar", last modified: Tue Apr 25 12:09:29 2023, max compression
```

## Comparing `mkdocs-glightbox-0.3.3.tar` & `mkdocs-glightbox-0.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-04-20 14:43:58.579763 mkdocs-glightbox-0.3.3/
--rw-r--r--   0 blueswen   (501) staff       (20)     1065 2022-06-10 06:58:58.000000 mkdocs-glightbox-0.3.3/LICENSE
--rw-r--r--   0 blueswen   (501) staff       (20)       37 2022-07-15 16:30:44.000000 mkdocs-glightbox-0.3.3/MANIFEST.in
--rw-r--r--   0 blueswen   (501) staff       (20)     5205 2023-04-20 14:43:58.579565 mkdocs-glightbox-0.3.3/PKG-INFO
--rw-r--r--   0 blueswen   (501) staff       (20)     4779 2023-04-20 14:30:58.000000 mkdocs-glightbox-0.3.3/README.md
-drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-04-20 14:43:58.577083 mkdocs-glightbox-0.3.3/mkdocs_glightbox/
--rw-r--r--   0 blueswen   (501) staff       (20)        0 2022-06-12 06:19:32.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox/__init__.py
-drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-04-20 14:43:58.578438 mkdocs-glightbox-0.3.3/mkdocs_glightbox/__pycache__/
--rw-r--r--   0 blueswen   (501) staff       (20)      165 2022-11-15 14:31:20.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 blueswen   (501) staff       (20)     6248 2023-04-20 14:34:14.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox/__pycache__/plugin.cpython-39.pyc
-drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-04-20 14:43:58.579110 mkdocs-glightbox-0.3.3/mkdocs_glightbox/glightbox/
--rw-r--r--   0 blueswen   (501) staff       (20)     1096 2022-06-10 06:42:44.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox/glightbox/LICENSE.md
--rw-r--r--   0 blueswen   (501) staff       (20)    13749 2022-06-07 11:18:17.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox/glightbox/glightbox.min.css
--rw-r--r--   0 blueswen   (501) staff       (20)    56280 2022-06-07 11:18:23.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox/glightbox/glightbox.min.js
--rw-r--r--   0 blueswen   (501) staff       (20)     8184 2023-04-20 14:27:45.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox/plugin.py
-drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-04-20 14:43:58.577937 mkdocs-glightbox-0.3.3/mkdocs_glightbox.egg-info/
--rw-r--r--   0 blueswen   (501) staff       (20)     5205 2023-04-20 14:43:58.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox.egg-info/PKG-INFO
--rw-r--r--   0 blueswen   (501) staff       (20)      528 2023-04-20 14:43:58.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox.egg-info/SOURCES.txt
--rw-r--r--   0 blueswen   (501) staff       (20)        1 2023-04-20 14:43:58.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox.egg-info/dependency_links.txt
--rw-r--r--   0 blueswen   (501) staff       (20)       69 2023-04-20 14:43:58.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox.egg-info/entry_points.txt
--rw-r--r--   0 blueswen   (501) staff       (20)       17 2023-04-20 14:43:58.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox.egg-info/top_level.txt
--rw-r--r--   0 blueswen   (501) staff       (20)       38 2023-04-20 14:43:58.579810 mkdocs-glightbox-0.3.3/setup.cfg
--rw-rw-r--   0 blueswen   (501) staff       (20)      816 2023-04-20 14:30:38.000000 mkdocs-glightbox-0.3.3/setup.py
+drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-04-25 12:09:29.194431 mkdocs-glightbox-0.3.4/
+-rw-r--r--   0 blueswen   (501) staff       (20)     1065 2022-06-10 06:58:58.000000 mkdocs-glightbox-0.3.4/LICENSE
+-rw-r--r--   0 blueswen   (501) staff       (20)       37 2022-07-15 16:30:44.000000 mkdocs-glightbox-0.3.4/MANIFEST.in
+-rw-r--r--   0 blueswen   (501) staff       (20)     5205 2023-04-25 12:09:29.194282 mkdocs-glightbox-0.3.4/PKG-INFO
+-rw-r--r--   0 blueswen   (501) staff       (20)     4779 2023-04-20 14:30:58.000000 mkdocs-glightbox-0.3.4/README.md
+drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-04-25 12:09:29.190701 mkdocs-glightbox-0.3.4/mkdocs_glightbox/
+-rw-r--r--   0 blueswen   (501) staff       (20)        0 2022-06-12 06:19:32.000000 mkdocs-glightbox-0.3.4/mkdocs_glightbox/__init__.py
+drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-04-25 12:09:29.192679 mkdocs-glightbox-0.3.4/mkdocs_glightbox/__pycache__/
+-rw-r--r--   0 blueswen   (501) staff       (20)      165 2022-11-15 14:31:20.000000 mkdocs-glightbox-0.3.4/mkdocs_glightbox/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 blueswen   (501) staff       (20)     6426 2023-04-25 12:05:45.000000 mkdocs-glightbox-0.3.4/mkdocs_glightbox/__pycache__/plugin.cpython-39.pyc
+drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-04-25 12:09:29.193741 mkdocs-glightbox-0.3.4/mkdocs_glightbox/glightbox/
+-rw-r--r--   0 blueswen   (501) staff       (20)     1096 2022-06-10 06:42:44.000000 mkdocs-glightbox-0.3.4/mkdocs_glightbox/glightbox/LICENSE.md
+-rw-r--r--   0 blueswen   (501) staff       (20)    13749 2022-06-07 11:18:17.000000 mkdocs-glightbox-0.3.4/mkdocs_glightbox/glightbox/glightbox.min.css
+-rw-r--r--   0 blueswen   (501) staff       (20)    56280 2022-06-07 11:18:23.000000 mkdocs-glightbox-0.3.4/mkdocs_glightbox/glightbox/glightbox.min.js
+-rw-r--r--   0 blueswen   (501) staff       (20)     8597 2023-04-25 12:02:00.000000 mkdocs-glightbox-0.3.4/mkdocs_glightbox/plugin.py
+drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-04-25 12:09:29.192119 mkdocs-glightbox-0.3.4/mkdocs_glightbox.egg-info/
+-rw-r--r--   0 blueswen   (501) staff       (20)     5205 2023-04-25 12:09:29.000000 mkdocs-glightbox-0.3.4/mkdocs_glightbox.egg-info/PKG-INFO
+-rw-r--r--   0 blueswen   (501) staff       (20)      528 2023-04-25 12:09:29.000000 mkdocs-glightbox-0.3.4/mkdocs_glightbox.egg-info/SOURCES.txt
+-rw-r--r--   0 blueswen   (501) staff       (20)        1 2023-04-25 12:09:29.000000 mkdocs-glightbox-0.3.4/mkdocs_glightbox.egg-info/dependency_links.txt
+-rw-r--r--   0 blueswen   (501) staff       (20)       69 2023-04-25 12:09:29.000000 mkdocs-glightbox-0.3.4/mkdocs_glightbox.egg-info/entry_points.txt
+-rw-r--r--   0 blueswen   (501) staff       (20)       17 2023-04-25 12:09:29.000000 mkdocs-glightbox-0.3.4/mkdocs_glightbox.egg-info/top_level.txt
+-rw-r--r--   0 blueswen   (501) staff       (20)       38 2023-04-25 12:09:29.194479 mkdocs-glightbox-0.3.4/setup.cfg
+-rw-rw-r--   0 blueswen   (501) staff       (20)      816 2023-04-25 12:02:46.000000 mkdocs-glightbox-0.3.4/setup.py
```

### Comparing `mkdocs-glightbox-0.3.3/LICENSE` & `mkdocs-glightbox-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-glightbox-0.3.3/PKG-INFO` & `mkdocs-glightbox-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-glightbox
-Version: 0.3.3
+Version: 0.3.4
 Summary: MkDocs plugin supports image lightbox with GLightbox.
 Home-page: https://blueswen.github.io/mkdocs-glightbox
 Author: Blueswen
 Author-email: blueswen.tw@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/Blueswen/mkdocs-glightbox
 Keywords: mkdocs,plugin,lightbox
```

### Comparing `mkdocs-glightbox-0.3.3/README.md` & `mkdocs-glightbox-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-glightbox-0.3.3/mkdocs_glightbox/__pycache__/plugin.cpython-39.pyc` & `mkdocs-glightbox-0.3.4/mkdocs_glightbox/__pycache__/plugin.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 20 14:27:45 2023 UTC, .py size: 8184 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 e14b 4164 f81f 0000  a........KAd....
+00000000: 610d 0d0a 0000 0000 38c1 4764 9521 0000  a.......8.Gd.!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 6400 6403 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6400 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6501 a00a 650b a101 5a0c 6502 6a0d  ..e...e...Z.e.j.
@@ -97,15 +97,15 @@
 00000600: 2020 2020 202e 6773 6c69 6465 2d64 6573       .gslide-des
 00000610: 6320 7b20 636f 6c6f 723a 2023 3636 363b  c { color: #666;
 00000620: 2075 7365 722d 7365 6c65 6374 3a20 7465   user-select: te
 00000630: 7874 3b20 7d0a 2020 2020 2020 2020 2e67  xt; }.        .g
 00000640: 736c 6964 652d 696d 6167 6520 696d 6720  slide-image img 
 00000650: 7b20 6261 636b 6772 6f75 6e64 3a20 7768  { background: wh
 00000660: 6974 653b 207d 0a20 2020 2020 2020 20da  ite; }.        .
-00000670: 0574 6865 6d65 5a08 6d61 7465 7269 616c  .themeZ.material
+00000670: 0574 6865 6d65 da08 6d61 7465 7269 616c  .theme..material
 00000680: 61a1 0100 000a 2020 2020 2020 2020 2020  a.....          
 00000690: 2020 2e67 7363 726f 6c6c 6261 722d 6669    .gscrollbar-fi
 000006a0: 7865 7220 7b20 7061 6464 696e 672d 7269  xer { padding-ri
 000006b0: 6768 743a 2031 3570 783b 207d 0a20 2020  ght: 15px; }.   
 000006c0: 2020 2020 2020 2020 202e 6764 6573 632d           .gdesc-
 000006d0: 696e 6e65 7220 7b20 666f 6e74 2d73 697a  inner { font-siz
 000006e0: 653a 2030 2e37 3572 656d 3b20 7d0a 2020  e: 0.75rem; }.  
@@ -134,16 +134,16 @@
 00000850: 7420 7372 633d 227a 2361 7373 6574 732f  t src="z#assets/
 00000860: 6a61 7661 7363 7269 7074 732f 676c 6967  javascripts/glig
 00000870: 6874 626f 782e 6d69 6e2e 6a73 7a0b 223e  htbox.min.jsz.">
 00000880: 3c2f 7363 7269 7074 3e63 0100 0000 0000  </script>c......
 00000890: 0000 0000 0000 0200 0000 0500 0000 1300  ................
 000008a0: 0000 7316 0000 0069 007c 005d 0e7d 017c  ..s....i.|.].}.|
 000008b0: 0188 007c 0119 0093 0271 0453 00a9 0072  ...|.....q.S...r
-000008c0: 1e00 0000 a902 da02 2e30 da01 6ba9 01da  .........0..k...
-000008d0: 0d70 6c75 6769 6e5f 636f 6e66 6967 721e  .plugin_configr.
+000008c0: 1f00 0000 a902 da02 2e30 da01 6ba9 01da  .........0..k...
+000008d0: 0d70 6c75 6769 6e5f 636f 6e66 6967 721f  .plugin_configr.
 000008e0: 0000 00fa 482f 5573 6572 732f 626c 7565  ....H/Users/blue
 000008f0: 7377 656e 2f70 726f 6a65 6374 732f 6c61  swen/projects/la
 00000900: 622f 6d6b 646f 6373 2d67 6c69 6768 7462  b/mkdocs-glightb
 00000910: 6f78 2f6d 6b64 6f63 735f 676c 6967 6874  ox/mkdocs_glight
 00000920: 626f 782f 706c 7567 696e 2e70 79da 0a3c  box/plugin.py..<
 00000930: 6469 6374 636f 6d70 3e4a 0000 0073 0400  dictcomp>J...s..
 00000940: 0000 0602 02ff 7a2f 4c69 6768 7462 6f78  ......z/Lightbox
@@ -167,21 +167,21 @@
 00000a60: 7069 6c65 da06 444f 5441 4c4c 7202 0000  pile..DOTALLr...
 00000a70: 00da 1067 6574 5f72 656c 6174 6976 655f  ...get_relative_
 00000a80: 7572 6cda 0d6e 6f72 6d61 6c69 7a65 5f75  url..normalize_u
 00000a90: 726c da03 7572 6cda 0373 7562 da04 6e61  rl..url..sub..na
 00000aa0: 6d65 da04 6469 6374 da06 636f 6e66 6967  me..dict..config
 00000ab0: da04 6a73 6f6e da05 6475 6d70 73da 055f  ..json..dumps.._
 00000ac0: 7661 7273 290c da04 7365 6c66 da06 6f75  vars)...self..ou
-00000ad0: 7470 7574 da04 7061 6765 7232 0000 00da  tput..pager2....
+00000ad0: 7470 7574 da04 7061 6765 7233 0000 00da  tput..pager3....
 00000ae0: 066b 7761 7267 735a 0a68 6561 645f 7265  .kwargsZ.head_re
 00000af0: 6765 785a 0a62 6f64 795f 7265 6765 785a  gexZ.body_regexZ
 00000b00: 0863 7373 5f6c 696e 6b5a 0963 7373 5f70  .css_linkZ.css_p
 00000b10: 6174 6368 5a09 6a73 5f73 6372 6970 745a  atchZ.js_scriptZ
 00000b20: 096c 625f 636f 6e66 6967 5a07 6a73 5f63  .lb_configZ.js_c
-00000b30: 6f64 6572 1e00 0000 7222 0000 0072 2400  oder....r"...r$.
+00000b30: 6f64 6572 1f00 0000 7223 0000 0072 2500  oder....r#...r%.
 00000b40: 0000 da0c 6f6e 5f70 6f73 745f 7061 6765  ....on_post_page
 00000b50: 2500 0000 7338 0000 0000 031c 0104 0310  %...s8..........
 00000b60: 0110 031c 0114 0304 060e 0108 0714 031c  ................
 00000b70: 0114 030a 010a 0202 fe06 0410 0110 0110  ................
 00000b80: 0112 0114 0102 ff06 0204 fe08 040c 0114  ................
 00000b90: 027a 1b4c 6967 6874 626f 7850 6c75 6769  .z.LightboxPlugi
 00000ba0: 6e2e 6f6e 5f70 6f73 745f 7061 6765 6304  n.on_post_pagec.
@@ -199,193 +199,204 @@
 00000c60: 6167 2077 6974 6820 676c 6967 6874 626f  ag with glightbo
 00000c70: 7820 636c 6173 7320 616e 6420 6174 7472  x class and attr
 00000c80: 6962 7574 6573 2066 726f 6d20 636f 6e66  ibutes from conf
 00000c90: 6967 721b 0000 0054 4663 0100 0000 0000  igr....TFc......
 00000ca0: 0000 0000 0000 0200 0000 0500 0000 1300  ................
 00000cb0: 0000 731c 0000 0069 007c 005d 147d 017c  ..s....i.|.].}.|
 00000cc0: 0174 0088 006a 0183 017c 0119 0093 0271  .t...j...|.....q
-00000cd0: 0453 0072 1e00 0000 2902 7231 0000 0072  .S.r....).r1...r
-00000ce0: 3200 0000 721f 0000 0029 0172 3600 0000  2...r....).r6...
-00000cf0: 721e 0000 0072 2400 0000 7225 0000 0060  r....r$...r%...`
+00000cd0: 0453 0072 1f00 0000 2902 7232 0000 0072  .S.r....).r2...r
+00000ce0: 3300 0000 7220 0000 0029 0172 3700 0000  3...r ...).r7...
+00000cf0: 721f 0000 0072 2500 0000 7226 0000 0060  r....r%...r&...`
 00000d00: 0000 00f3 0000 0000 7a32 4c69 6768 7462  ........z2Lightb
 00000d10: 6f78 506c 7567 696e 2e6f 6e5f 7061 6765  oxPlugin.on_page
 00000d20: 5f63 6f6e 7465 6e74 2e3c 6c6f 6361 6c73  _content.<locals
 00000d30: 3e2e 3c64 6963 7463 6f6d 703e 2902 720f  >.<dictcomp>).r.
-00000d40: 0000 0072 1000 0000 2903 da08 656d 6f6a  ...r....)...emoj
-00000d50: 696f 6e65 da07 7477 656d 6f6a 69da 0667  ione..twemoji..g
+00000d40: 0000 0072 1000 0000 2903 5a08 656d 6f6a  ...r....).Z.emoj
+00000d50: 696f 6e65 5a07 7477 656d 6f6a 695a 0667  ioneZ.twemojiZ.g
 00000d60: 656d 6f6a 697a 076f 6666 2d67 6c62 7214  emojiz.off-glbr.
 00000d70: 0000 007a 513c 615c 625b 5e3e 5d2a 3e28  ...zQ<a\b[^>]*>(
 00000d80: 3f3a 5c73 2a3c 5b5e 3e5d 2b3e 5c73 2a29  ?:\s*<[^>]+>\s*)
 00000d90: 2a3c 696d 675c 625b 5e3e 5d2a 3e28 3f3a  *<img\b[^>]*>(?:
 00000da0: 5c73 2a3c 5b5e 3e5d 2b3e 5c73 2a29 2a3c  \s*<[^>]+>\s*)*<
 00000db0: 2f61 3e7c 3c69 6d67 283f 503c 6174 7472  /a>|<img(?P<attr
 00000dc0: 3e2e 2a3f 293e 6301 0000 0000 0000 0000  >.*?)>c.........
 00000dd0: 0000 0001 0000 0006 0000 0013 0000 0073  ...............s
 00000de0: 1200 0000 8802 a000 7c00 8801 8803 8800  ........|.......
 00000df0: 6a01 a104 5300 2901 4e29 02da 1477 7261  j...S.).N)...wra
 00000e00: 705f 696d 675f 7769 7468 5f61 6e63 686f  p_img_with_ancho
-00000e10: 7272 2700 0000 2901 da05 6d61 7463 68a9  rr'...)...match.
-00000e20: 0472 3800 0000 7223 0000 0072 3600 0000  .r8...r#...r6...
-00000e30: da0a 736b 6970 5f63 6c61 7373 721e 0000  ..skip_classr...
-00000e40: 0072 2400 0000 da08 3c6c 616d 6264 613e  .r$.....<lambda>
+00000e10: 7272 2800 0000 2901 da05 6d61 7463 68a9  rr(...)...match.
+00000e20: 0472 3900 0000 7224 0000 0072 3700 0000  .r9...r$...r7...
+00000e30: da0a 736b 6970 5f63 6c61 7373 721f 0000  ..skip_classr...
+00000e40: 0072 2500 0000 da08 3c6c 616d 6264 613e  .r%.....<lambda>
 00000e50: 6b00 0000 7304 0000 0004 010a ff7a 304c  k...s........z0L
 00000e60: 6967 6874 626f 7850 6c75 6769 6e2e 6f6e  ightboxPlugin.on
 00000e70: 5f70 6167 655f 636f 6e74 656e 742e 3c6c  _page_content.<l
 00000e80: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e29  ocals>.<lambda>)
-00000e90: 0672 2700 0000 7228 0000 0072 3200 0000  .r'...r(...r2...
-00000ea0: 7229 0000 0072 2a00 0000 722f 0000 0029  r)...r*...r/...)
-00000eb0: 0672 3600 0000 da04 6874 6d6c 7238 0000  .r6.....htmlr8..
-00000ec0: 0072 3200 0000 7239 0000 00da 0770 6174  .r2...r9.....pat
-00000ed0: 7465 726e 721e 0000 0072 4100 0000 7224  ternr....rA...r$
+00000e90: 0672 2800 0000 7229 0000 0072 3300 0000  .r(...r)...r3...
+00000ea0: 722a 0000 0072 2b00 0000 7230 0000 0029  r*...r+...r0...)
+00000eb0: 0672 3700 0000 da04 6874 6d6c 7239 0000  .r7.....htmlr9..
+00000ec0: 0072 3300 0000 723a 0000 00da 0770 6174  .r3...r:.....pat
+00000ed0: 7465 726e 721f 0000 0072 3f00 0000 7225  ternr....r?...r%
 00000ee0: 0000 00da 0f6f 6e5f 7061 6765 5f63 6f6e  .....on_page_con
 00000ef0: 7465 6e74 5b00 0000 731a 0000 0000 031c  tent[...s.......
 00000f00: 0104 0112 0208 0214 0304 0102 ff04 0304  ................
 00000f10: 0110 0302 fc04 077a 1e4c 6967 6874 626f  .......z.Lightbo
 00000f20: 7850 6c75 6769 6e2e 6f6e 5f70 6167 655f  xPlugin.on_page_
 00000f30: 636f 6e74 656e 7463 0500 0000 0000 0000  contentc........
-00000f40: 0000 0000 1100 0000 0700 0000 4300 0000  ............C...
-00000f50: 73e8 0100 0074 00a0 0164 01a1 017d 057c  s....t...d...}.|
-00000f60: 05a0 027c 01a0 0364 02a1 01a1 0172 247c  ...|...d.....r$|
-00000f70: 01a0 0364 02a1 0153 007c 01a0 0364 02a1  ...d...S.|...d..
-00000f80: 017d 067c 01a0 0364 03a1 017d 0774 00a0  .}.|...d...}.t..
-00000f90: 0464 047c 07a1 027d 0864 0564 0684 007c  .d.|...}.d.d...|
-00000fa0: 0844 0083 017d 0874 057c 0383 0174 057c  .D...}.t.|...t.|
-00000fb0: 0883 0140 0072 667c 0653 0074 00a0 0664  ...@.rf|.S.t...d
-00000fc0: 077c 07a1 02a0 0364 08a1 017d 0964 097c  .|.....d...}.d.|
-00000fd0: 099b 0064 0a9d 037d 0a7c 02a0 07a1 0044  ...d...}.|.....D
-00000fe0: 005d 1e5c 027d 0b7d 0c7c 0a64 0b7c 0b9b  .].\.}.}.|.d.|..
-00000ff0: 0064 0c7c 0c9b 0064 0d9d 0537 007d 0a71  .d.|...d...7.}.q
-00001000: 8c67 0064 0ea2 017d 0d7c 0d44 0090 015d  .g.d...}.|.D...]
-00001010: 187d 0e64 0f7c 0e9b 009d 027d 0f7c 0f64  .}.d.|.....}.|.d
-00001020: 106b 0290 0172 4074 00a0 0664 117c 07a1  .k...r@t...d.|..
-00001030: 027d 107c 006a 0864 1219 0090 0173 0664  .}.|.j.d.....s.d
-00001040: 137c 0476 0090 0172 2a7c 04a0 0964 1364  .|.v...r*|...d.d
-00001050: 14a1 0264 1575 0090 0172 2a7c 1090 0172  ...d.u...r*|...r
-00001060: 167c 10a0 0364 08a1 016e 1074 00a0 0664  .|...d...n.t...d
-00001070: 167c 07a1 02a0 0364 08a1 017d 106e 147c  .|.....d...}.n.|
-00001080: 1090 0172 3a7c 10a0 0364 08a1 016e 0264  ...r:|...d...n.d
-00001090: 177d 106e 587c 0f64 186b 0290 0172 7274  .}.nX|.d.k...rrt
-000010a0: 00a0 0664 197c 07a1 027d 107c 1090 0172  ...d.|...}.|...r
-000010b0: 667c 10a0 0364 08a1 016e 087c 006a 0864  f|...d...n.|.j.d
-000010c0: 1a19 007d 106e 2674 00a0 067c 0f9b 0064  ...}.n&t...|...d
-000010d0: 1b9d 027c 07a1 027d 107c 1090 0172 947c  ...|...}.|...r.|
-000010e0: 10a0 0364 08a1 016e 0264 177d 107c 1064  ...d...n.d.}.|.d
-000010f0: 176b 0372 b87c 0f64 186b 0290 0172 bc7c  .k.r.|.d.k...r.|
-00001100: 0a64 1c7c 109b 0064 0d9d 0337 007d 0a71  .d.|...d...7.}.q
-00001110: b87c 0a64 1d7c 0f9b 0064 0c7c 109b 0064  .|.d.|...d.|...d
-00001120: 0d9d 0537 007d 0a71 b87c 0a64 1e7c 069b  ...7.}.q.|.d.|..
-00001130: 0064 1f9d 0337 007d 0a7c 0a53 0029 207a  .d...7.}.|.S.) z
-00001140: 2057 7261 7020 696d 6167 6520 7461 6773   Wrap image tags
-00001150: 2077 6974 6820 616e 6368 6f72 2074 6167   with anchor tag
-00001160: 737a 103c 6128 3f50 3c61 7474 723e 2e2a  sz.<a(?P<attr>.*
-00001170: 3f29 3e72 0100 0000 da04 6174 7472 7a0f  ?)>r......attrz.
-00001180: 636c 6173 733d 2228 5b5e 225d 2b29 2263  class="([^"]+)"c
-00001190: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-000011a0: 0400 0000 5300 0000 731e 0000 0067 007c  ....S...s....g.|
-000011b0: 005d 167d 017c 01a0 00a1 0044 005d 087d  .].}.|.....D.].}
-000011c0: 027c 0291 0371 1071 0453 0072 1e00 0000  .|...q.q.S.r....
-000011d0: 2901 da05 7370 6c69 7429 0372 2000 0000  )...split).r ...
-000011e0: 7240 0000 00da 0163 721e 0000 0072 1e00  r@.....cr....r..
-000011f0: 0000 7224 0000 00da 0a3c 6c69 7374 636f  ..r$.....<listco
-00001200: 6d70 3e7c 0000 0072 3b00 0000 7a37 4c69  mp>|...r;...z7Li
-00001210: 6768 7462 6f78 506c 7567 696e 2e77 7261  ghtboxPlugin.wra
-00001220: 705f 696d 675f 7769 7468 5f61 6e63 686f  p_img_with_ancho
-00001230: 722e 3c6c 6f63 616c 733e 2e3c 6c69 7374  r.<locals>.<list
-00001240: 636f 6d70 3e7a 1473 7263 3d5b 5c22 5c27  comp>z.src=[\"\'
-00001250: 5d28 5b5e 5c22 5c27 5d2b 29e9 0100 0000  ]([^\"\']+).....
-00001260: 7a1b 3c61 2063 6c61 7373 3d22 676c 6967  z.<a class="glig
-00001270: 6874 626f 7822 2068 7265 663d 227a 1322  htbox" href="z."
-00001280: 2064 6174 612d 7479 7065 3d22 696d 6167   data-type="imag
-00001290: 6522 7a06 2064 6174 612d 7a02 3d22 fa01  e"z. data-z.="..
-000012a0: 2229 04da 0574 6974 6c65 da0b 6465 7363  ")...title..desc
-000012b0: 7269 7074 696f 6e7a 1063 6170 7469 6f6e  riptionz.caption
-000012c0: 2d70 6f73 6974 696f 6eda 0767 616c 6c65  -position..galle
-000012d0: 7279 7a05 6461 7461 2d7a 0a64 6174 612d  ryz.data-z.data-
-000012e0: 7469 746c 657a 1b64 6174 612d 7469 746c  titlez.data-titl
-000012f0: 653d 5b5c 225c 275d 285b 5e5c 225c 275d  e=[\"\']([^\"\']
-00001300: 2b29 7215 0000 007a 1667 6c69 6768 7462  +)r....z.glightb
-00001310: 6f78 2e61 7574 6f5f 6361 7074 696f 6e46  ox.auto_captionF
-00001320: 547a 1461 6c74 3d5b 5c22 5c27 5d28 5b5e  Tz.alt=[\"\']([^
-00001330: 5c22 5c27 5d2b 29da 007a 1564 6174 612d  \"\']+)..z.data-
-00001340: 6361 7074 696f 6e2d 706f 7369 7469 6f6e  caption-position
-00001350: 7a26 6461 7461 2d63 6170 7469 6f6e 2d70  z&data-caption-p
-00001360: 6f73 6974 696f 6e3d 5b5c 225c 275d 285b  osition=[\"\']([
-00001370: 5e5c 225c 275d 2b29 7216 0000 007a 0d3d  ^\"\']+)r....z.=
-00001380: 5b22 275d 285b 5e22 275d 2b29 7a15 2064  ["']([^"']+)z. d
-00001390: 6174 612d 6465 7363 2d70 6f73 6974 696f  ata-desc-positio
-000013a0: 6e3d 22fa 0120 fa01 3e7a 043c 2f61 3e29  n=".. ..>z.</a>)
-000013b0: 0a72 2900 0000 722a 0000 0072 4000 0000  .r)...r*...r@...
-000013c0: da05 6772 6f75 70da 0766 696e 6461 6c6c  ..group..findall
-000013d0: da03 7365 74da 0673 6561 7263 68da 0569  ..set..search..i
-000013e0: 7465 6d73 7232 0000 0072 2800 0000 2911  temsr2...r(...).
-000013f0: 7236 0000 0072 4000 0000 7223 0000 0072  r6...r@...r#...r
-00001400: 4200 0000 7227 0000 005a 0961 5f70 6174  B...r'...Z.a_pat
-00001410: 7465 726e 5a07 696d 675f 7461 675a 0869  ternZ.img_tagZ.i
-00001420: 6d67 5f61 7474 72da 0763 6c61 7373 6573  mg_attr..classes
-00001430: da03 7372 635a 0561 5f74 6167 7221 0000  ..srcZ.a_tagr!..
-00001440: 00da 0176 5a0d 736c 6964 655f 6f70 7469  ...vZ.slide_opti
-00001450: 6f6e 73da 066f 7074 696f 6e72 4700 0000  ons..optionrG...
-00001460: da03 7661 6c72 1e00 0000 721e 0000 0072  ..valr....r....r
-00001470: 2400 0000 723f 0000 0073 0000 0073 4e00  $...r?...s...sN.
-00001480: 0000 0002 0a01 1001 0a02 0a01 0a01 0c01  ................
-00001490: 0e02 1001 0402 1201 0c02 1001 1801 0806  ................
-000014a0: 0a01 0a01 0a01 0c01 0c01 06ff 0402 0efe  ................
-000014b0: 0406 02ff 0e02 10fd 0406 1601 0a01 0c01  ................
-000014c0: 1c02 1201 1403 0802 0a01 1202 1801 1001  ................
-000014d0: 7a23 4c69 6768 7462 6f78 506c 7567 696e  z#LightboxPlugin
-000014e0: 2e77 7261 705f 696d 675f 7769 7468 5f61  .wrap_img_with_a
-000014f0: 6e63 686f 7263 0200 0000 0000 0000 0000  nchorc..........
-00001500: 0000 0600 0000 0700 0000 4b00 0000 7376  ..........K...sv
-00001510: 0000 0074 006a 01a0 027c 0164 0119 0064  ...t.j...|.d...d
-00001520: 02a1 027d 0374 006a 01a0 027c 0364 03a1  ...}.t.j...|.d..
-00001530: 027d 0474 03a0 0474 006a 01a0 0274 0564  .}.t...t.j...t.d
-00001540: 0464 05a1 0374 006a 01a0 027c 0464 05a1  .d...t.j...|.d..
-00001550: 02a1 0201 0074 006a 01a0 027c 0364 06a1  .....t.j...|.d..
-00001560: 027d 0574 03a0 0474 006a 01a0 0274 0564  .}.t...t.j...t.d
-00001570: 0464 07a1 0374 006a 01a0 027c 0564 07a1  .d...t.j...|.d..
-00001580: 02a1 0201 0064 0853 0029 097a 3543 6f70  .....d.S.).z5Cop
-00001590: 7920 676c 6967 6874 626f 7822 7320 6373  y glightbox"s cs
-000015a0: 7320 616e 6420 6a73 2066 696c 6573 2074  s and js files t
-000015b0: 6f20 6173 7365 7473 2064 6972 6563 746f  o assets directo
-000015c0: 7279 da08 7369 7465 5f64 6972 da06 6173  ry..site_dir..as
-000015d0: 7365 7473 da0b 7374 796c 6573 6865 6574  sets..stylesheet
-000015e0: 7372 1b00 0000 7a11 676c 6967 6874 626f  sr....z.glightbo
-000015f0: 782e 6d69 6e2e 6373 73da 0b6a 6176 6173  x.min.css..javas
-00001600: 6372 6970 7473 7a10 676c 6967 6874 626f  criptsz.glightbo
-00001610: 782e 6d69 6e2e 6a73 4e29 06da 026f 73da  x.min.jsN)...os.
-00001620: 0470 6174 68da 046a 6f69 6e72 0200 0000  .path..joinr....
-00001630: da09 636f 7079 5f66 696c 65da 0962 6173  ..copy_file..bas
-00001640: 655f 7061 7468 2906 7236 0000 0072 3200  e_path).r6...r2.
-00001650: 0000 7239 0000 005a 106f 7574 7075 745f  ..r9...Z.output_
-00001660: 6261 7365 5f70 6174 68da 0863 7373 5f70  base_path..css_p
-00001670: 6174 685a 076a 735f 7061 7468 721e 0000  athZ.js_pathr...
-00001680: 0072 1e00 0000 7224 0000 00da 0d6f 6e5f  .r....r$.....on_
-00001690: 706f 7374 5f62 7569 6c64 ac00 0000 7316  post_build....s.
-000016a0: 0000 0000 0312 010e 0104 010e 010c fe04  ................
-000016b0: 040e 0104 010e 010c fe7a 1c4c 6967 6874  .........z.Light
-000016c0: 626f 7850 6c75 6769 6e2e 6f6e 5f70 6f73  boxPlugin.on_pos
-000016d0: 745f 6275 696c 644e 290f da08 5f5f 6e61  t_buildN)...__na
-000016e0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000016f0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00001700: 5f5f 646f 635f 5f72 0300 0000 da04 5479  __doc__r......Ty
-00001710: 7065 da04 626f 6f6c da06 4368 6f69 6365  pe..bool..Choice
-00001720: da03 7374 72da 046c 6973 74da 0d63 6f6e  ..str..list..con
-00001730: 6669 675f 7363 6865 6d65 723a 0000 0072  fig_schemer:...r
-00001740: 4600 0000 723f 0000 0072 6700 0000 721e  F...r?...rg...r.
-00001750: 0000 0072 1e00 0000 721e 0000 0072 2400  ...r....r....r$.
-00001760: 0000 7205 0000 000e 0000 0073 2a00 0000  ..r........s*...
-00001770: 0801 0403 1001 1001 1002 0201 0cfe 0204  ................
-00001780: 1001 1001 1001 1001 1001 1002 0201 0cfe  ................
-00001790: 02f2 0414 0836 0818 0839 7205 0000 0029  .....6...9r....)
-000017a0: 1372 3300 0000 da07 6c6f 6767 696e 6772  .r3.....loggingr
-000017b0: 6100 0000 7229 0000 00da 066d 6b64 6f63  a...r).....mkdoc
-000017c0: 7372 0200 0000 da0d 6d6b 646f 6373 2e63  sr......mkdocs.c
-000017d0: 6f6e 6669 6772 0300 0000 5a0e 6d6b 646f  onfigr....Z.mkdo
-000017e0: 6373 2e70 6c75 6769 6e73 7204 0000 00da  cs.pluginsr.....
-000017f0: 0967 6574 4c6f 6767 6572 7268 0000 00da  .getLoggerrh....
-00001800: 036c 6f67 7262 0000 00da 0764 6972 6e61  .logrb.....dirna
-00001810: 6d65 da07 6162 7370 6174 68da 085f 5f66  me..abspath..__f
-00001820: 696c 655f 5f72 6500 0000 7205 0000 0072  ile__re...r....r
-00001830: 1e00 0000 721e 0000 0072 1e00 0000 7224  ....r....r....r$
-00001840: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00001850: 0073 1200 0000 0801 0801 0801 0802 0c01  .s..............
-00001860: 0c01 0c02 0a01 1403                      ........
+00000f40: 0000 0000 1200 0000 0b00 0000 4300 0000  ............C...
+00000f50: 7352 0200 0090 017a fe74 00a0 0164 01a1  sR.....z.t...d..
+00000f60: 017d 057c 05a0 027c 01a0 0364 02a1 01a1  .}.|...|...d....
+00000f70: 0172 2a7c 01a0 0364 02a1 0157 0053 007c  .r*|...d...W.S.|
+00000f80: 01a0 0364 02a1 017d 067c 01a0 0364 03a1  ...d...}.|...d..
+00000f90: 017d 0774 00a0 0464 047c 07a1 027d 0864  .}.t...d.|...}.d
+00000fa0: 0564 0684 007c 0844 0083 017d 0874 057c  .d...|.D...}.t.|
+00000fb0: 0383 0174 057c 0883 0140 0072 6e7c 0657  ...t.|...@.rn|.W
+00000fc0: 0053 0074 00a0 0664 077c 07a1 02a0 0364  .S.t...d.|.....d
+00000fd0: 08a1 017d 0964 097c 099b 0064 0a9d 037d  ...}.d.|...d...}
+00000fe0: 0a7c 02a0 07a1 0044 005d 1e5c 027d 0b7d  .|.....D.].\.}.}
+00000ff0: 0c7c 0a64 0b7c 0b9b 0064 0c7c 0c9b 0064  .|.d.|...d.|...d
+00001000: 0d9d 0537 007d 0a71 9467 0064 0ea2 017d  ...7.}.q.g.d...}
+00001010: 0d7c 0d44 0090 015d 287d 0e64 0f7c 0e9b  .|.D...](}.d.|..
+00001020: 009d 027d 0f7c 0f64 106b 0290 0172 5874  ...}.|.d.k...rXt
+00001030: 00a0 0664 117c 07a1 027d 107c 006a 0864  ...d.|...}.|.j.d
+00001040: 1219 0090 0173 0e64 137c 0476 0090 0172  .....s.d.|.v...r
+00001050: 427c 04a0 0964 1364 14a1 0264 1575 0090  B|...d.d...d.u..
+00001060: 0172 427c 1090 0172 207c 10a0 0364 08a1  .rB|...r |...d..
+00001070: 017d 106e 2074 00a0 0664 167c 07a1 027d  .}.n t...d.|...}
+00001080: 107c 1090 0172 3c7c 10a0 0364 08a1 016e  .|...r<|...d...n
+00001090: 0264 177d 106e 147c 1090 0172 527c 10a0  .d.}.n.|...rR|..
+000010a0: 0364 08a1 016e 0264 177d 106e 587c 0f64  .d...n.d.}.nX|.d
+000010b0: 186b 0290 0172 8a74 00a0 0664 197c 07a1  .k...r.t...d.|..
+000010c0: 027d 107c 1090 0172 7e7c 10a0 0364 08a1  .}.|...r~|...d..
+000010d0: 016e 087c 006a 0864 1a19 007d 106e 2674  .n.|.j.d...}.n&t
+000010e0: 00a0 067c 0f9b 0064 1b9d 027c 07a1 027d  ...|...d...|...}
+000010f0: 107c 1090 0172 ac7c 10a0 0364 08a1 016e  .|...r.|...d...n
+00001100: 0264 177d 107c 1064 176b 0372 c07c 0f64  .d.}.|.d.k.r.|.d
+00001110: 186b 0290 0172 d47c 0a64 1c7c 109b 0064  .k...r.|.d.|...d
+00001120: 0d9d 0337 007d 0a71 c07c 0a64 1d7c 0f9b  ...7.}.q.|.d.|..
+00001130: 0064 0c7c 109b 0064 0d9d 0537 007d 0a71  .d.|...d...7.}.q
+00001140: c07c 0a64 1e7c 069b 0064 1f9d 0337 007d  .|.d.|...d...7.}
+00001150: 0a7c 0a57 0053 0004 0074 0a90 0279 4c01  .|.W.S...t...yL.
+00001160: 007d 1101 007a 3274 0ba0 0c64 207c 119b  .}...z2t...d |..
+00001170: 0064 1d7c 01a0 0364 02a1 019b 009d 04a1  .d.|...d........
+00001180: 0101 007c 01a0 0364 02a1 0157 0006 0059  ...|...d...W...Y
+00001190: 0064 217d 117e 1153 0064 217d 117e 1130  .d!}.~.S.d!}.~.0
+000011a0: 0030 0064 2153 0029 227a 2057 7261 7020  .0.d!S.)"z Wrap 
+000011b0: 696d 6167 6520 7461 6773 2077 6974 6820  image tags with 
+000011c0: 616e 6368 6f72 2074 6167 737a 103c 6128  anchor tagsz.<a(
+000011d0: 3f50 3c61 7474 723e 2e2a 3f29 3e72 0100  ?P<attr>.*?)>r..
+000011e0: 0000 da04 6174 7472 7a0f 636c 6173 733d  ....attrz.class=
+000011f0: 2228 5b5e 225d 2b29 2263 0100 0000 0000  "([^"]+)"c......
+00001200: 0000 0000 0000 0300 0000 0400 0000 5300  ..............S.
+00001210: 0000 731e 0000 0067 007c 005d 167d 017c  ..s....g.|.].}.|
+00001220: 01a0 00a1 0044 005d 087d 027c 0291 0371  .....D.].}.|...q
+00001230: 1071 0453 0072 1f00 0000 2901 da05 7370  .q.S.r....)...sp
+00001240: 6c69 7429 0372 2100 0000 723e 0000 00da  lit).r!...r>....
+00001250: 0163 721f 0000 0072 1f00 0000 7225 0000  .cr....r....r%..
+00001260: 00da 0a3c 6c69 7374 636f 6d70 3e7d 0000  ...<listcomp>}..
+00001270: 0072 3c00 0000 7a37 4c69 6768 7462 6f78  .r<...z7Lightbox
+00001280: 506c 7567 696e 2e77 7261 705f 696d 675f  Plugin.wrap_img_
+00001290: 7769 7468 5f61 6e63 686f 722e 3c6c 6f63  with_anchor.<loc
+000012a0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e7a  als>.<listcomp>z
+000012b0: 1473 7263 3d5b 5c22 5c27 5d28 5b5e 5c22  .src=[\"\']([^\"
+000012c0: 5c27 5d2b 29e9 0100 0000 7a1b 3c61 2063  \']+).....z.<a c
+000012d0: 6c61 7373 3d22 676c 6967 6874 626f 7822  lass="glightbox"
+000012e0: 2068 7265 663d 227a 1322 2064 6174 612d   href="z." data-
+000012f0: 7479 7065 3d22 696d 6167 6522 7a06 2064  type="image"z. d
+00001300: 6174 612d 7a02 3d22 fa01 2229 04da 0574  ata-z.="..")...t
+00001310: 6974 6c65 da0b 6465 7363 7269 7074 696f  itle..descriptio
+00001320: 6e7a 1063 6170 7469 6f6e 2d70 6f73 6974  nz.caption-posit
+00001330: 696f 6e5a 0767 616c 6c65 7279 7a05 6461  ionZ.galleryz.da
+00001340: 7461 2d7a 0a64 6174 612d 7469 746c 657a  ta-z.data-titlez
+00001350: 1764 6174 612d 7469 746c 653d 5b5c 225d  .data-title=[\"]
+00001360: 285b 5e5c 225d 2b29 7215 0000 007a 1667  ([^\"]+)r....z.g
+00001370: 6c69 6768 7462 6f78 2e61 7574 6f5f 6361  lightbox.auto_ca
+00001380: 7074 696f 6e46 547a 1061 6c74 3d5b 5c22  ptionFTz.alt=[\"
+00001390: 5d28 5b5e 5c22 5d2b 29da 007a 1564 6174  ]([^\"]+)..z.dat
+000013a0: 612d 6361 7074 696f 6e2d 706f 7369 7469  a-caption-positi
+000013b0: 6f6e 7a22 6461 7461 2d63 6170 7469 6f6e  onz"data-caption
+000013c0: 2d70 6f73 6974 696f 6e3d 5b5c 225d 285b  -position=[\"]([
+000013d0: 5e5c 225d 2b29 7216 0000 007a 0b3d 5b22  ^\"]+)r....z.=["
+000013e0: 5d28 5b5e 225d 2b29 7a15 2064 6174 612d  ]([^"]+)z. data-
+000013f0: 6465 7363 2d70 6f73 6974 696f 6e3d 22fa  desc-position=".
+00001400: 0120 fa01 3e7a 043c 2f61 3e7a 2b45 7272  . ..>z.</a>z+Err
+00001410: 6f72 2069 6e20 7772 6170 7069 6e67 2069  or in wrapping i
+00001420: 6d67 2074 6167 2077 6974 6820 616e 6368  mg tag with anch
+00001430: 6f72 2074 6167 3a20 4e29 0d72 2a00 0000  or tag: N).r*...
+00001440: 722b 0000 0072 3e00 0000 da05 6772 6f75  r+...r>.....grou
+00001450: 70da 0766 696e 6461 6c6c da03 7365 74da  p..findall..set.
+00001460: 0673 6561 7263 68da 0569 7465 6d73 7233  .search..itemsr3
+00001470: 0000 0072 2900 0000 da09 4578 6365 7074  ...r).....Except
+00001480: 696f 6eda 036c 6f67 da07 7761 726e 696e  ion..log..warnin
+00001490: 6729 1272 3700 0000 723e 0000 0072 2400  g).r7...r>...r$.
+000014a0: 0000 7240 0000 0072 2800 0000 5a09 615f  ..r@...r(...Z.a_
+000014b0: 7061 7474 6572 6e5a 0769 6d67 5f74 6167  patternZ.img_tag
+000014c0: 5a08 696d 675f 6174 7472 da07 636c 6173  Z.img_attr..clas
+000014d0: 7365 73da 0373 7263 5a05 615f 7461 6772  ses..srcZ.a_tagr
+000014e0: 2200 0000 da01 765a 0d73 6c69 6465 5f6f  ".....vZ.slide_o
+000014f0: 7074 696f 6e73 da06 6f70 7469 6f6e 7245  ptions..optionrE
+00001500: 0000 00da 0376 616c da01 6572 1f00 0000  .....val..er....
+00001510: 721f 0000 0072 2500 0000 723d 0000 0073  r....r%...r=...s
+00001520: 0000 0073 5a00 0000 0002 0401 0a01 1001  ...sZ...........
+00001530: 0c02 0a01 0a01 0c01 0e02 1001 0602 1201  ................
+00001540: 0c02 1001 1801 0806 0a01 0a01 0a01 0c01  ................
+00001550: 0c01 06ff 0402 0efe 0404 0601 0c02 0c01  ................
+00001560: 1602 1601 0a01 0c01 1c02 1201 1403 0802  ................
+00001570: 0a01 1202 1801 1001 0601 1001 0401 14ff  ................
+00001580: 0403 7a23 4c69 6768 7462 6f78 506c 7567  ..z#LightboxPlug
+00001590: 696e 2e77 7261 705f 696d 675f 7769 7468  in.wrap_img_with
+000015a0: 5f61 6e63 686f 7263 0200 0000 0000 0000  _anchorc........
+000015b0: 0000 0000 0600 0000 0700 0000 4b00 0000  ............K...
+000015c0: 7376 0000 0074 006a 01a0 027c 0164 0119  sv...t.j...|.d..
+000015d0: 0064 02a1 027d 0374 006a 01a0 027c 0364  .d...}.t.j...|.d
+000015e0: 03a1 027d 0474 03a0 0474 006a 01a0 0274  ...}.t...t.j...t
+000015f0: 0564 0464 05a1 0374 006a 01a0 027c 0464  .d.d...t.j...|.d
+00001600: 05a1 02a1 0201 0074 006a 01a0 027c 0364  .......t.j...|.d
+00001610: 06a1 027d 0574 03a0 0474 006a 01a0 0274  ...}.t...t.j...t
+00001620: 0564 0464 07a1 0374 006a 01a0 027c 0564  .d.d...t.j...|.d
+00001630: 07a1 02a1 0201 0064 0853 0029 097a 3543  .......d.S.).z5C
+00001640: 6f70 7920 676c 6967 6874 626f 7822 7320  opy glightbox"s 
+00001650: 6373 7320 616e 6420 6a73 2066 696c 6573  css and js files
+00001660: 2074 6f20 6173 7365 7473 2064 6972 6563   to assets direc
+00001670: 746f 7279 da08 7369 7465 5f64 6972 5a06  tory..site_dirZ.
+00001680: 6173 7365 7473 5a0b 7374 796c 6573 6865  assetsZ.styleshe
+00001690: 6574 7372 1b00 0000 7a11 676c 6967 6874  etsr....z.glight
+000016a0: 626f 782e 6d69 6e2e 6373 735a 0b6a 6176  box.min.cssZ.jav
+000016b0: 6173 6372 6970 7473 7a10 676c 6967 6874  ascriptsz.glight
+000016c0: 626f 782e 6d69 6e2e 6a73 4e29 06da 026f  box.min.jsN)...o
+000016d0: 73da 0470 6174 68da 046a 6f69 6e72 0200  s..path..joinr..
+000016e0: 0000 da09 636f 7079 5f66 696c 65da 0962  ....copy_file..b
+000016f0: 6173 655f 7061 7468 2906 7237 0000 0072  ase_path).r7...r
+00001700: 3300 0000 723a 0000 005a 106f 7574 7075  3...r:...Z.outpu
+00001710: 745f 6261 7365 5f70 6174 685a 0863 7373  t_base_pathZ.css
+00001720: 5f70 6174 685a 076a 735f 7061 7468 721f  _pathZ.js_pathr.
+00001730: 0000 0072 1f00 0000 7225 0000 00da 0d6f  ...r....r%.....o
+00001740: 6e5f 706f 7374 5f62 7569 6c64 b200 0000  n_post_build....
+00001750: 7316 0000 0000 0312 010e 0104 010e 010c  s...............
+00001760: fe04 040e 0104 010e 010c fe7a 1c4c 6967  ...........z.Lig
+00001770: 6874 626f 7850 6c75 6769 6e2e 6f6e 5f70  htboxPlugin.on_p
+00001780: 6f73 745f 6275 696c 644e 290f da08 5f5f  ost_buildN)...__
+00001790: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+000017a0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+000017b0: da07 5f5f 646f 635f 5f72 0300 0000 da04  ..__doc__r......
+000017c0: 5479 7065 da04 626f 6f6c da06 4368 6f69  Type..bool..Choi
+000017d0: 6365 da03 7374 72da 046c 6973 74da 0d63  ce..str..list..c
+000017e0: 6f6e 6669 675f 7363 6865 6d65 723b 0000  onfig_schemer;..
+000017f0: 0072 4400 0000 723d 0000 0072 6400 0000  .rD...r=...rd...
+00001800: 721f 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
+00001810: 2500 0000 7205 0000 000e 0000 0073 2a00  %...r........s*.
+00001820: 0000 0801 0403 1001 1001 1002 0201 0cfe  ................
+00001830: 0204 1001 1001 1001 1001 1001 1002 0201  ................
+00001840: 0cfe 02f2 0414 0836 0818 083f 7205 0000  .......6...?r...
+00001850: 0029 1372 3400 0000 da07 6c6f 6767 696e  .).r4.....loggin
+00001860: 6772 5f00 0000 722a 0000 00da 066d 6b64  gr_...r*.....mkd
+00001870: 6f63 7372 0200 0000 5a0d 6d6b 646f 6373  ocsr....Z.mkdocs
+00001880: 2e63 6f6e 6669 6772 0300 0000 5a0e 6d6b  .configr....Z.mk
+00001890: 646f 6373 2e70 6c75 6769 6e73 7204 0000  docs.pluginsr...
+000018a0: 00da 0967 6574 4c6f 6767 6572 7265 0000  ...getLoggerre..
+000018b0: 0072 5600 0000 7260 0000 00da 0764 6972  .rV...r`.....dir
+000018c0: 6e61 6d65 da07 6162 7370 6174 68da 085f  name..abspath.._
+000018d0: 5f66 696c 655f 5f72 6300 0000 7205 0000  _file__rc...r...
+000018e0: 0072 1f00 0000 721f 0000 0072 1f00 0000  .r....r....r....
+000018f0: 7225 0000 00da 083c 6d6f 6475 6c65 3e01  r%.....<module>.
+00001900: 0000 0073 1200 0000 0801 0801 0801 0802  ...s............
+00001910: 0c01 0c01 0c02 0a01 1403                 ..........
```

### Comparing `mkdocs-glightbox-0.3.3/mkdocs_glightbox/glightbox/LICENSE.md` & `mkdocs-glightbox-0.3.4/mkdocs_glightbox/glightbox/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-glightbox-0.3.3/mkdocs_glightbox/glightbox/glightbox.min.css` & `mkdocs-glightbox-0.3.4/mkdocs_glightbox/glightbox/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-glightbox-0.3.3/mkdocs_glightbox/glightbox/glightbox.min.js` & `mkdocs-glightbox-0.3.4/mkdocs_glightbox/glightbox/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-glightbox-0.3.3/mkdocs_glightbox/plugin.py` & `mkdocs-glightbox-0.3.4/mkdocs_glightbox/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,68 +110,74 @@
             html,
         )
 
         return html
 
     def wrap_img_with_anchor(self, match, plugin_config, skip_class, meta):
         """Wrap image tags with anchor tags"""
-        a_pattern = re.compile(r"<a(?P<attr>.*?)>")
-        if a_pattern.match(match.group(0)):
-            return match.group(0)
-
-        img_tag = match.group(0)
-        img_attr = match.group("attr")
-        classes = re.findall(r'class="([^"]+)"', img_attr)
-        classes = [c for match in classes for c in match.split()]
-
-        if set(skip_class) & set(classes):
-            return img_tag
-
-        src = re.search(r"src=[\"\']([^\"\']+)", img_attr).group(1)
-        a_tag = f'<a class="glightbox" href="{src}" data-type="image"'
-        # setting data-width and data-height with plugin options
-        for k, v in plugin_config.items():
-            a_tag += f' data-{k}="{v}"'
-        slide_options = [
-            "title",
-            "description",
-            "caption-position",
-            "gallery",
-        ]
-        for option in slide_options:
-            attr = f"data-{option}"
-            if attr == "data-title":
-                val = re.search(r"data-title=[\"\']([^\"\']+)", img_attr)
-                if self.config["auto_caption"] or (
-                    "glightbox.auto_caption" in meta
-                    and meta.get("glightbox.auto_caption", False) is True
-                ):
-                    val = (
-                        val.group(1)
-                        if val
-                        else re.search(r"alt=[\"\']([^\"\']+)", img_attr).group(1)
-                    )
+        try:
+            a_pattern = re.compile(r"<a(?P<attr>.*?)>")
+            if a_pattern.match(match.group(0)):
+                return match.group(0)
+
+            img_tag = match.group(0)
+            img_attr = match.group("attr")
+            classes = re.findall(r'class="([^"]+)"', img_attr)
+            classes = [c for match in classes for c in match.split()]
+
+            if set(skip_class) & set(classes):
+                return img_tag
+
+            src = re.search(r"src=[\"\']([^\"\']+)", img_attr).group(1)
+            a_tag = f'<a class="glightbox" href="{src}" data-type="image"'
+            # setting data-width and data-height with plugin options
+            for k, v in plugin_config.items():
+                a_tag += f' data-{k}="{v}"'
+            slide_options = [
+                "title",
+                "description",
+                "caption-position",
+                "gallery",
+            ]
+            for option in slide_options:
+                attr = f"data-{option}"
+                if attr == "data-title":
+                    val = re.search(r"data-title=[\"]([^\"]+)", img_attr)
+                    if self.config["auto_caption"] or (
+                        "glightbox.auto_caption" in meta
+                        and meta.get("glightbox.auto_caption", False) is True
+                    ):
+                        if val:
+                            val = val.group(1)
+                        else:
+                            val = re.search(r"alt=[\"]([^\"]+)", img_attr)
+                            val = val.group(1) if val else ""
+                    else:
+                        val = val.group(1) if val else ""
+                elif attr == "data-caption-position":
+                    val = re.search(r"data-caption-position=[\"]([^\"]+)", img_attr)
+                    val = val.group(1) if val else self.config["caption_position"]
                 else:
+                    val = re.search(f'{attr}=["]([^"]+)', img_attr)
                     val = val.group(1) if val else ""
-            elif attr == "data-caption-position":
-                val = re.search(r"data-caption-position=[\"\']([^\"\']+)", img_attr)
-                val = val.group(1) if val else self.config["caption_position"]
-            else:
-                val = re.search(f"{attr}=[\"']([^\"']+)", img_attr)
-                val = val.group(1) if val else ""
-
-            # skip val is empty
-            if val != "":
-                # convert data-caption-position to data-desc-position
-                if attr == "data-caption-position":
-                    a_tag += f' data-desc-position="{val}"'
-                else:
-                    a_tag += f' {attr}="{val}"'
-        a_tag += f">{img_tag}</a>"
-        return a_tag
+
+                # skip val is empty
+                if val != "":
+                    # convert data-caption-position to data-desc-position
+                    if attr == "data-caption-position":
+                        a_tag += f' data-desc-position="{val}"'
+                    else:
+                        a_tag += f' {attr}="{val}"'
+            a_tag += f">{img_tag}</a>"
+            return a_tag
+        except Exception as e:
+            log.warning(
+                f"Error in wrapping img tag with anchor tag: {e} {match.group(0)}"
+            )
+            return match.group(0)
 
     def on_post_build(self, config, **kwargs):
         """Copy glightbox"s css and js files to assets directory"""
 
         output_base_path = os.path.join(config["site_dir"], "assets")
         css_path = os.path.join(output_base_path, "stylesheets")
         utils.copy_file(
```

### Comparing `mkdocs-glightbox-0.3.3/mkdocs_glightbox.egg-info/PKG-INFO` & `mkdocs-glightbox-0.3.4/mkdocs_glightbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-glightbox
-Version: 0.3.3
+Version: 0.3.4
 Summary: MkDocs plugin supports image lightbox with GLightbox.
 Home-page: https://blueswen.github.io/mkdocs-glightbox
 Author: Blueswen
 Author-email: blueswen.tw@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/Blueswen/mkdocs-glightbox
 Keywords: mkdocs,plugin,lightbox
```

### Comparing `mkdocs-glightbox-0.3.3/mkdocs_glightbox.egg-info/SOURCES.txt` & `mkdocs-glightbox-0.3.4/mkdocs_glightbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-glightbox-0.3.3/setup.py` & `mkdocs-glightbox-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mkdocs-glightbox",
-    version="0.3.3",
+    version="0.3.4",
     author="Blueswen",
     author_email="blueswen.tw@gmail.com",
     url="https://blueswen.github.io/mkdocs-glightbox",
     project_urls={
         "Source": "https://github.com/Blueswen/mkdocs-glightbox",
     },
     keywords=["mkdocs", "plugin", "lightbox"],
```

