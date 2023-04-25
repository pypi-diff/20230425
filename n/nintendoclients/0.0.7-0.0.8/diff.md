# Comparing `tmp/nintendoclients-0.0.7.tar.gz` & `tmp/nintendoclients-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nintendoclients-0.0.7.tar", last modified: Tue Mar 28 12:34:25 2023, max compression
+gzip compressed data, was "nintendoclients-0.0.8.tar", last modified: Tue Apr 25 07:20:32 2023, max compression
```

## Comparing `nintendoclients-0.0.7.tar` & `nintendoclients-0.0.8.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2023-03-28 12:34:25.192833 nintendoclients-0.0.7/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1072 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/LICENSE
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      324 2023-03-28 12:34:25.192833 nintendoclients-0.0.7/PKG-INFO
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2118 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/README.md
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2023-03-28 12:34:25.188833 nintendoclients-0.0.7/nintendo/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)        2 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/__init__.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     9734 2023-03-28 12:30:03.000000 nintendoclients-0.0.7/nintendo/aauth.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     7353 2023-03-28 12:31:00.000000 nintendoclients-0.0.7/nintendo/baas.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    10858 2023-03-28 12:32:38.000000 nintendoclients-0.0.7/nintendo/dauth.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     6107 2023-03-28 12:31:43.000000 nintendoclients-0.0.7/nintendo/dragons.py
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2023-03-28 12:34:25.188833 nintendoclients-0.0.7/nintendo/files/
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2023-03-28 12:34:25.192833 nintendoclients-0.0.7/nintendo/files/cert/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1060 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/files/cert/CACERT_NINTENDO_CA_G3.der
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1200 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/files/cert/CACERT_NINTENDO_CLASS2_CA_G3.der
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1224 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/files/cert/WIIU_COMMON_1_CERT.der
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1200 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/files/cert/WIIU_COMMON_1_RSA_KEY.der
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1223 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/files/cert/ctr-common-1-cert.der
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1194 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/files/cert/ctr-common-1-key.der
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2023-03-28 12:34:25.192833 nintendoclients-0.0.7/nintendo/files/config/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       45 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/files/config/3ds.cfg
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      533 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/files/config/default.cfg
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      101 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/files/config/friends.cfg
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      185 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/files/config/switch.cfg
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     7906 2023-03-28 12:31:58.000000 nintendoclients-0.0.7/nintendo/five.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     7406 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/miis.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     7226 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nasc.py
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2023-03-28 12:34:25.192833 nintendoclients-0.0.7/nintendo/nex/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)        2 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/__init__.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     5836 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/aauser.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    43193 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/account.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    24107 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/authentication.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     4362 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/backend.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     6737 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/common.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)   104615 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/datastore.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)   107915 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/datastore_smm.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)   191023 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/datastore_smm2.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     6941 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/debug.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    12134 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/errors.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    82735 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/friends.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     5299 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/health.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2877 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/hpp.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3791 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/kerberos.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)   190057 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/matchmaking.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)   192342 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/matchmaking_eagle.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)   209565 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/matchmaking_mk8d.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    15122 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/messaging.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3131 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/monitoring.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      480 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/natcheck.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     9997 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/nattraversal.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     8617 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/nintendonotification.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3099 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/notification.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    50589 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/prudp.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    26271 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/ranking.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    24689 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/ranking2.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    26774 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/ranking2_eagle.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    38970 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/ranking_mk8d.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1703 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/remotelog.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     9104 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/rmc.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      775 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/screening.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    12459 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/secure.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2257 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/settings.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3439 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/streams.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     4802 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/subscriber.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    12343 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nex/utility.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    12217 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/nnas.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2112 2023-03-26 20:14:25.000000 nintendoclients-0.0.7/nintendo/switch.py
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2023-03-28 12:34:25.192833 nintendoclients-0.0.7/nintendoclients.egg-info/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      324 2023-03-28 12:34:25.000000 nintendoclients-0.0.7/nintendoclients.egg-info/PKG-INFO
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1771 2023-03-28 12:34:25.000000 nintendoclients-0.0.7/nintendoclients.egg-info/SOURCES.txt
--rw-rw-r--   0 yannik    (1000) yannik    (1000)        1 2023-03-28 12:34:25.000000 nintendoclients-0.0.7/nintendoclients.egg-info/dependency_links.txt
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       28 2023-03-28 12:34:25.000000 nintendoclients-0.0.7/nintendoclients.egg-info/requires.txt
--rw-rw-r--   0 yannik    (1000) yannik    (1000)        9 2023-03-28 12:34:25.000000 nintendoclients-0.0.7/nintendoclients.egg-info/top_level.txt
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       38 2023-03-28 12:34:25.192833 nintendoclients-0.0.7/setup.cfg
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      578 2023-03-28 12:34:20.000000 nintendoclients-0.0.7/setup.py
+drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2023-04-25 07:20:32.849922 nintendoclients-0.0.8/
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     1072 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/LICENSE
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)      324 2023-04-25 07:20:32.849922 nintendoclients-0.0.8/PKG-INFO
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     2118 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/README.md
+drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2023-04-25 07:20:32.841922 nintendoclients-0.0.8/nintendo/
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)        2 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/__init__.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     9840 2023-04-25 07:17:10.000000 nintendoclients-0.0.8/nintendo/aauth.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     7445 2023-04-25 07:17:24.000000 nintendoclients-0.0.8/nintendo/baas.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)    11029 2023-04-25 07:16:27.000000 nintendoclients-0.0.8/nintendo/dauth.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     6128 2023-04-25 07:17:41.000000 nintendoclients-0.0.8/nintendo/dragons.py
+drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2023-04-25 07:20:32.841922 nintendoclients-0.0.8/nintendo/files/
+drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2023-04-25 07:20:32.841922 nintendoclients-0.0.8/nintendo/files/cert/
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     1060 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/files/cert/CACERT_NINTENDO_CA_G3.der
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     1200 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/files/cert/CACERT_NINTENDO_CLASS2_CA_G3.der
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     1224 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/files/cert/WIIU_COMMON_1_CERT.der
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     1200 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/files/cert/WIIU_COMMON_1_RSA_KEY.der
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     1223 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/files/cert/ctr-common-1-cert.der
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     1194 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/files/cert/ctr-common-1-key.der
+drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2023-04-25 07:20:32.845922 nintendoclients-0.0.8/nintendo/files/config/
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)       45 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/files/config/3ds.cfg
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)      533 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/files/config/default.cfg
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)      101 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/files/config/friends.cfg
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)      185 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/files/config/switch.cfg
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     8005 2023-04-25 07:17:57.000000 nintendoclients-0.0.8/nintendo/five.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     7406 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/miis.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     7226 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nasc.py
+drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2023-04-25 07:20:32.849922 nintendoclients-0.0.8/nintendo/nex/
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)        2 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/__init__.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     5836 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/aauser.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)    43193 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/account.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)    24107 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/authentication.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     4362 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/backend.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     6737 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/common.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)   104615 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/datastore.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)   107915 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/datastore_smm.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)   191023 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/datastore_smm2.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     6941 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/debug.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)    12134 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/errors.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)    82735 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/friends.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     5299 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/health.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     2877 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/hpp.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     3791 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/kerberos.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)   190996 2023-04-25 07:14:25.000000 nintendoclients-0.0.8/nintendo/nex/matchmaking.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)   193281 2023-04-25 07:14:25.000000 nintendoclients-0.0.8/nintendo/nex/matchmaking_eagle.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)   212264 2023-04-25 07:14:25.000000 nintendoclients-0.0.8/nintendo/nex/matchmaking_mk8d.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)    15122 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/messaging.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     3131 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/monitoring.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)      480 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/natcheck.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     9997 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/nattraversal.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     8617 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/nintendonotification.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     3099 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/notification.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)    50589 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/prudp.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)    26271 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/ranking.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)    24689 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/ranking2.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)    26774 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/ranking2_eagle.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)    39274 2023-04-25 07:14:25.000000 nintendoclients-0.0.8/nintendo/nex/ranking_mk8d.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     1703 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/remotelog.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     9104 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/rmc.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)      775 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/screening.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)    12459 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/secure.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     2257 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/settings.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     3439 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/streams.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     4802 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/subscriber.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)    12343 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nex/utility.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)    12217 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/nnas.py
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     2112 2023-03-26 20:14:25.000000 nintendoclients-0.0.8/nintendo/switch.py
+drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2023-04-25 07:20:32.849922 nintendoclients-0.0.8/nintendoclients.egg-info/
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)      324 2023-04-25 07:20:32.000000 nintendoclients-0.0.8/nintendoclients.egg-info/PKG-INFO
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)     1771 2023-04-25 07:20:32.000000 nintendoclients-0.0.8/nintendoclients.egg-info/SOURCES.txt
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)        1 2023-04-25 07:20:32.000000 nintendoclients-0.0.8/nintendoclients.egg-info/dependency_links.txt
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)       28 2023-04-25 07:20:32.000000 nintendoclients-0.0.8/nintendoclients.egg-info/requires.txt
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)        9 2023-04-25 07:20:32.000000 nintendoclients-0.0.8/nintendoclients.egg-info/top_level.txt
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)       38 2023-04-25 07:20:32.849922 nintendoclients-0.0.8/setup.cfg
+-rw-rw-r--   0 yannik    (1000) yannik    (1000)      578 2023-04-25 07:14:46.000000 nintendoclients-0.0.8/setup.py
```

### Comparing `nintendoclients-0.0.7/LICENSE` & `nintendoclients-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/README.md` & `nintendoclients-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/aauth.py` & `nintendoclients-0.0.8/nintendo/aauth.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 	1410: "libcurl (nnHttp; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 14.3.0.0; Add-on 14.3.0.0)",
 	1411: "libcurl (nnHttp; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 14.3.0.0; Add-on 14.3.0.0)",
 	1412: "libcurl (nnHttp; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 14.3.0.0; Add-on 14.3.0.0)",
 	1500: "libcurl (nnHttp; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 15.3.0.0; Add-on 15.3.0.0)",
 	1501: "libcurl (nnHttp; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 15.3.0.0; Add-on 15.3.0.0)",
 	1600: "libcurl (nnHttp; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 16.2.0.0; Add-on 16.2.0.0)",
 	1601: "libcurl (nnHttp; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 16.2.0.0; Add-on 16.2.0.0)",
+	1602: "libcurl (nnHttp; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 16.2.0.0; Add-on 16.2.0.0)",
 }
 
 API_VERSION = {
 	 900: 3,
 	 901: 3,
 	 910: 3,
 	 920: 3,
@@ -94,17 +95,18 @@
 	1410: 3,
 	1411: 3,
 	1412: 3,
 	1500: 4,
 	1501: 4,
 	1600: 4,
 	1601: 4,
+	1602: 4,
 }
 
-LATEST_VERSION = 1601
+LATEST_VERSION = 1602
 
 
 class AAuthError(Exception):
 	DEVICE_TOKEN_EXPIRED = 103
 	ROMID_BANNED = 105
 	UNAUTHORIZED_APPLICATION = 106
 	SERVICE_CLOSED = 109
```

### Comparing `nintendoclients-0.0.7/nintendo/baas.py` & `nintendoclients-0.0.8/nintendo/baas.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,18 @@
 	1410: "libcurl (%s; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 14.3.0.0; Add-on 14.3.0.0)",
 	1411: "libcurl (%s; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 14.3.0.0; Add-on 14.3.0.0)",
 	1412: "libcurl (%s; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 14.3.0.0; Add-on 14.3.0.0)",
 	1500: "libcurl (%s; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 15.3.0.0; Add-on 15.3.0.0)",
 	1501: "libcurl (%s; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 15.3.0.0; Add-on 15.3.0.0)",
 	1600: "libcurl (%s; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 16.2.0.0; Add-on 16.2.0.0)",
 	1601: "libcurl (%s; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 16.2.0.0; Add-on 16.2.0.0)",
+	1602: "libcurl (%s; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 16.2.0.0; Add-on 16.2.0.0)",
 }
 
-LATEST_VERSION = 1601
+LATEST_VERSION = 1602
 
 
 class PresenceState:
 	INACTIVE = "INACTIVE"
 	ONLINE = "ONLINE"
 	PLAYING = "PLAYING"
```

### Comparing `nintendoclients-0.0.7/nintendo/dauth.py` & `nintendoclients-0.0.8/nintendo/dauth.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 	1400: "CusHY#000e0000#35hWb15SBXTnbUfTMLBz9sCnfheuRGis0OTZqa7l8yw=",
 	1410: "CusHY#000e0100#ctIxSPR4jenzQNGc6y4zXIvzvF75ty53jN0T15Rjtmk=",
 	1411: "CusHY#000e0101#uTt4IVydkYqwYArOFR3BzOCmw0MkEeF_tZxHENYDh4E=",
 	1412: "CusHY#000e0102#jHk6_VwXVPPl3ijRZ5jRy5MIAcUW_Q2uFdfJ0vrjhCA=",
 	1500: "CusHY#000f0000#MJE7we0zvVhAnXN9uCU7fQAM7GiqGHpR5ECuC9G_nuU=",
 	1501: "CusHY#000f0001#TMqizZGvUaBZApmHHQE0Uo7vQ6xWuQxZ8JH87_HnnqI=",
 	1600: "CusHY#00100000#k_VrW8iX7QgupPlYZYhg3dLEVDhqGN_iXW5Mm0VYEvQ=",
-	1601: "CusHY#00100001#qHay53MkzVLOUU_Iy7_kyPlUMnaoi7HXCAmESYTft_c=",
+	1601: "CusHY#00100001#qHay53MkzVLOUU_Iy7_kyPlUMnaoi7HXCAmESYTft_c=",
+	1602: "CusHY#00100002#qjeCnaxVt5NjGjxosJOMVw-ZyR219B3qgAB3YtSil6g=",
 }
 
 USER_AGENT = {
 	900:  "libcurl (nnDauth; 16f4553f-9eee-4e39-9b61-59bc7c99b7c8; SDK 9.3.0.0)",
 	901:  "libcurl (nnDauth; 16f4553f-9eee-4e39-9b61-59bc7c99b7c8; SDK 9.3.0.0)",
 	910:  "libcurl (nnDauth; 16f4553f-9eee-4e39-9b61-59bc7c99b7c8; SDK 9.3.0.0)",
 	920:  "libcurl (nnDauth; 16f4553f-9eee-4e39-9b61-59bc7c99b7c8; SDK 9.3.0.0)",
@@ -75,15 +76,16 @@
 	1400: "libcurl (nnDauth; 16f4553f-9eee-4e39-9b61-59bc7c99b7c8; SDK 14.3.0.0)",
 	1410: "libcurl (nnDauth; 16f4553f-9eee-4e39-9b61-59bc7c99b7c8; SDK 14.3.0.0)",
 	1411: "libcurl (nnDauth; 16f4553f-9eee-4e39-9b61-59bc7c99b7c8; SDK 14.3.0.0)",
 	1412: "libcurl (nnDauth; 16f4553f-9eee-4e39-9b61-59bc7c99b7c8; SDK 14.3.0.0)",
 	1500: "libcurl (nnDauth; 16f4553f-9eee-4e39-9b61-59bc7c99b7c8; SDK 15.3.0.0)",
 	1501: "libcurl (nnDauth; 16f4553f-9eee-4e39-9b61-59bc7c99b7c8; SDK 15.3.0.0)",
 	1600: "libcurl (nnDauth; 16f4553f-9eee-4e39-9b61-59bc7c99b7c8; SDK 16.2.0.0)",
-	1601: "libcurl (nnDauth; 16f4553f-9eee-4e39-9b61-59bc7c99b7c8; SDK 16.2.0.0)",
+	1601: "libcurl (nnDauth; 16f4553f-9eee-4e39-9b61-59bc7c99b7c8; SDK 16.2.0.0)",
+	1602: "libcurl (nnDauth; 16f4553f-9eee-4e39-9b61-59bc7c99b7c8; SDK 16.2.0.0)",
 }
 
 KEY_GENERATION = {
 	900:  10,
 	901:  10,
 	910:  11,
 	920:  11,
@@ -109,15 +111,16 @@
 	1400: 14,
 	1410: 14,
 	1411: 14,
 	1412: 14,
 	1500: 15,
 	1501: 15,
 	1600: 16,
-	1601: 16,
+	1601: 16,
+	1602: 16,
 }
 
 API_VERSION = {
 	900: 6,
 	901: 6,
 	910: 6,
 	920: 6,
@@ -143,18 +146,19 @@
 	1400: 7,
 	1410: 7,
 	1411: 7,
 	1412: 7,
 	1500: 7,
 	1501: 7,
 	1600: 7,
-	1601: 7,
+	1601: 7,
+	1602: 7,
 }
 
-LATEST_VERSION = 1601
+LATEST_VERSION = 1602
 
 
 class DAuthError(Exception):
 	UNAUTHORIZED_DEVICE = 4
 	SYSTEM_UPDATE_REQUIRED = 7
 	BANNED_DEIVCE = 8
 	INTERNAL_SERVER_ERROR = 9
```

### Comparing `nintendoclients-0.0.7/nintendo/dragons.py` & `nintendoclients-0.0.8/nintendo/dragons.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,18 @@
 	1410: "14.1.0-1.0",
 	1411: "14.1.1-1.0",
 	1412: "14.1.2-1.0",
 	1500: "15.0.0-4.0",
 	1501: "15.0.1-1.0",
 	1600: "16.0.0-3.0",
 	1601: "16.0.1-1.0",
+	1602: "16.0.2-1.0",
 }
 
-LATEST_VERSION = 1601
+LATEST_VERSION = 1602
 
 
 class DragonsError(Exception):
 	def __init__(self, response):
 		self.response = response
 		
 		self.type = response.json["type"]
```

### Comparing `nintendoclients-0.0.7/nintendo/files/cert/CACERT_NINTENDO_CA_G3.der` & `nintendoclients-0.0.8/nintendo/files/cert/CACERT_NINTENDO_CA_G3.der`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/files/cert/CACERT_NINTENDO_CLASS2_CA_G3.der` & `nintendoclients-0.0.8/nintendo/files/cert/CACERT_NINTENDO_CLASS2_CA_G3.der`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/files/cert/WIIU_COMMON_1_CERT.der` & `nintendoclients-0.0.8/nintendo/files/cert/WIIU_COMMON_1_CERT.der`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/files/cert/WIIU_COMMON_1_RSA_KEY.der` & `nintendoclients-0.0.8/nintendo/files/cert/WIIU_COMMON_1_RSA_KEY.der`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/files/cert/ctr-common-1-cert.der` & `nintendoclients-0.0.8/nintendo/files/cert/ctr-common-1-cert.der`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/files/cert/ctr-common-1-key.der` & `nintendoclients-0.0.8/nintendo/files/cert/ctr-common-1-key.der`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/files/config/default.cfg` & `nintendoclients-0.0.8/nintendo/files/config/default.cfg`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/five.py` & `nintendoclients-0.0.8/nintendo/five.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,18 @@
 	1410: "libcurl (nnFriends; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 14.3.0.0; Add-on 14.3.0.0)",
 	1411: "libcurl (nnFriends; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 14.3.0.0; Add-on 14.3.0.0)",
 	1412: "libcurl (nnFriends; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 14.3.0.0; Add-on 14.3.0.0)",
 	1500: "libcurl (nnFriends; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 15.3.0.0; Add-on 15.3.0.0)",
 	1501: "libcurl (nnFriends; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 15.3.0.0; Add-on 15.3.0.0)",
 	1600: "libcurl (nnFriends; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 16.2.0.0; Add-on 16.2.0.0)",
 	1601: "libcurl (nnFriends; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 16.2.0.0; Add-on 16.2.0.0)",
+	1602: "libcurl (nnFriends; 789f928b-138e-4b2f-afeb-1acae821d897; SDK 16.2.0.0; Add-on 16.2.0.0)",
 }
 
-LATEST_VERSION = 1601
+LATEST_VERSION = 1602
 
 LANGUAGES = [
 	"en-US", "en-GB", "ja", "fr", "de", "es-419", "es", "it", "nl"
 	"fr-CA", "pt", "ru", "zh-Hans", "zh-Hant", "ko", "pt-BR", "dummy"
 ]
```

### Comparing `nintendoclients-0.0.7/nintendo/miis.py` & `nintendoclients-0.0.8/nintendo/miis.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nasc.py` & `nintendoclients-0.0.8/nintendo/nasc.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/aauser.py` & `nintendoclients-0.0.8/nintendo/nex/aauser.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/account.py` & `nintendoclients-0.0.8/nintendo/nex/account.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/authentication.py` & `nintendoclients-0.0.8/nintendo/nex/authentication.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/backend.py` & `nintendoclients-0.0.8/nintendo/nex/backend.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/common.py` & `nintendoclients-0.0.8/nintendo/nex/common.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/datastore.py` & `nintendoclients-0.0.8/nintendo/nex/datastore.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/datastore_smm.py` & `nintendoclients-0.0.8/nintendo/nex/datastore_smm.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/datastore_smm2.py` & `nintendoclients-0.0.8/nintendo/nex/datastore_smm2.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/debug.py` & `nintendoclients-0.0.8/nintendo/nex/debug.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/errors.py` & `nintendoclients-0.0.8/nintendo/nex/errors.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/friends.py` & `nintendoclients-0.0.8/nintendo/nex/friends.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/health.py` & `nintendoclients-0.0.8/nintendo/nex/health.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/hpp.py` & `nintendoclients-0.0.8/nintendo/nex/hpp.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/kerberos.py` & `nintendoclients-0.0.8/nintendo/nex/kerberos.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/matchmaking.py` & `nintendoclients-0.0.8/nintendo/nex/matchmaking_eagle.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,45 +275,74 @@
 		self.started_time = common.DateTime(0)
 		self.user_password = ""
 		self.refer_gid = 0
 		self.user_password_enabled = False
 		self.system_password_enabled = False
 		self.codeword = ""
 	
+	def max_version(self, settings):
+		version = 0
+		if settings["nex.version"] >= 30600:
+			version = 1
+		if settings["nex.version"] >= 30700:
+			version = 2
+		if settings["nex.version"] >= 30800:
+			version = 3
+		if settings["nex.version"] >= 40000:
+			version = 0
+		return version
+	
 	def check_required(self, settings, version):
 		if settings["nex.version"] >= 30500:
 			pass
 		if settings["nex.version"] >= 30000:
 			pass
 		if settings["nex.version"] >= 30500:
 			pass
+		if settings["nex.version"] >= 30600:
+			if version >= 1:
+				pass
+		if settings["nex.version"] >= 30700:
+			if version >= 2:
+				pass
+		if settings["nex.version"] >= 30800:
+			if version >= 3:
+				pass
 		if settings["nex.version"] >= 40000:
-			pass
+			if version >= 0:
+				pass
 	
 	def load(self, stream, version):
 		self.game_mode = stream.u32()
 		self.attribs = stream.list(stream.u32)
 		self.open_participation = stream.bool()
 		self.matchmake_system = stream.u32()
 		self.application_data = stream.buffer()
 		self.num_participants = stream.u32()
 		if stream.settings["nex.version"] >= 30500:
 			self.progress_score = stream.u8()
 		if stream.settings["nex.version"] >= 30000:
 			self.session_key = stream.buffer()
 		if stream.settings["nex.version"] >= 30500:
 			self.option = stream.u32()
+		if stream.settings["nex.version"] >= 30600:
+			if version >= 1:
+				self.param = stream.extract(MatchmakeParam)
+				self.started_time = stream.datetime()
+		if stream.settings["nex.version"] >= 30700:
+			if version >= 2:
+				self.user_password = stream.string()
+		if stream.settings["nex.version"] >= 30800:
+			if version >= 3:
+				self.refer_gid = stream.u32()
+				self.user_password_enabled = stream.bool()
+				self.system_password_enabled = stream.bool()
 		if stream.settings["nex.version"] >= 40000:
-			self.param = stream.extract(MatchmakeParam)
-			self.started_time = stream.datetime()
-			self.user_password = stream.string()
-			self.refer_gid = stream.u32()
-			self.user_password_enabled = stream.bool()
-			self.system_password_enabled = stream.bool()
-			self.codeword = stream.string()
+			if version >= 0:
+				self.codeword = stream.string()
 	
 	def save(self, stream, version):
 		self.check_required(stream.settings, version)
 		stream.u32(self.game_mode)
 		stream.list(self.attribs, stream.u32)
 		stream.bool(self.open_participation)
 		stream.u32(self.matchmake_system)
@@ -321,22 +350,29 @@
 		stream.u32(self.num_participants)
 		if stream.settings["nex.version"] >= 30500:
 			stream.u8(self.progress_score)
 		if stream.settings["nex.version"] >= 30000:
 			stream.buffer(self.session_key)
 		if stream.settings["nex.version"] >= 30500:
 			stream.u32(self.option)
+		if stream.settings["nex.version"] >= 30600:
+			if version >= 1:
+				stream.add(self.param)
+				stream.datetime(self.started_time)
+		if stream.settings["nex.version"] >= 30700:
+			if version >= 2:
+				stream.string(self.user_password)
+		if stream.settings["nex.version"] >= 30800:
+			if version >= 3:
+				stream.u32(self.refer_gid)
+				stream.bool(self.user_password_enabled)
+				stream.bool(self.system_password_enabled)
 		if stream.settings["nex.version"] >= 40000:
-			stream.add(self.param)
-			stream.datetime(self.started_time)
-			stream.string(self.user_password)
-			stream.u32(self.refer_gid)
-			stream.bool(self.user_password_enabled)
-			stream.bool(self.system_password_enabled)
-			stream.string(self.codeword)
+			if version >= 0:
+				stream.string(self.codeword)
 common.DataHolder.register(MatchmakeSession, "MatchmakeSession")
 
 
 class MatchmakeBlockListParam(common.Structure):
 	def __init__(self):
 		super().__init__()
 		self.options = 0
@@ -727,30 +763,36 @@
 
 class MatchmakeRefereeStartRoundParam(common.Structure):
 	def __init__(self):
 		super().__init__()
 		self.personal_data_category = None
 		self.gid = None
 		self.pids = None
+		self.report_summary_mode = None
+		self.event_id = None
 	
 	def check_required(self, settings, version):
-		for field in ['personal_data_category', 'gid', 'pids']:
+		for field in ['personal_data_category', 'gid', 'pids', 'report_summary_mode', 'event_id']:
 			if getattr(self, field) is None:
 				raise ValueError("No value assigned to required field: %s" %field)
 	
 	def load(self, stream, version):
 		self.personal_data_category = stream.u32()
 		self.gid = stream.u32()
 		self.pids = stream.list(stream.pid)
+		self.report_summary_mode = stream.u8()
+		self.event_id = stream.u32()
 	
 	def save(self, stream, version):
 		self.check_required(stream.settings, version)
 		stream.u32(self.personal_data_category)
 		stream.u32(self.gid)
 		stream.list(self.pids, stream.pid)
+		stream.u8(self.report_summary_mode)
+		stream.u32(self.event_id)
 
 
 class MatchmakeRefereeEndRoundParam(common.Structure):
 	def __init__(self):
 		super().__init__()
 		self.round_id = None
 		self.results = None
@@ -772,36 +814,42 @@
 
 class MatchmakeRefereePersonalRoundResult(common.Structure):
 	def __init__(self):
 		super().__init__()
 		self.pid = None
 		self.personal_round_result_flag = None
 		self.round_win_loss = None
-		self.rating_change = None
+		self.rating_value_change = None
 		self.buffer = None
+		self.report_summary_mode = None
+		self.event_id = None
 	
 	def check_required(self, settings, version):
-		for field in ['pid', 'personal_round_result_flag', 'round_win_loss', 'rating_change', 'buffer']:
+		for field in ['pid', 'personal_round_result_flag', 'round_win_loss', 'rating_value_change', 'buffer', 'report_summary_mode', 'event_id']:
 			if getattr(self, field) is None:
 				raise ValueError("No value assigned to required field: %s" %field)
 	
 	def load(self, stream, version):
 		self.pid = stream.pid()
 		self.personal_round_result_flag = stream.u32()
 		self.round_win_loss = stream.u32()
-		self.rating_change = stream.s32()
+		self.rating_value_change = stream.s32()
 		self.buffer = stream.qbuffer()
+		self.report_summary_mode = stream.u8()
+		self.event_id = stream.u32()
 	
 	def save(self, stream, version):
 		self.check_required(stream.settings, version)
 		stream.pid(self.pid)
 		stream.u32(self.personal_round_result_flag)
 		stream.u32(self.round_win_loss)
-		stream.s32(self.rating_change)
+		stream.s32(self.rating_value_change)
 		stream.qbuffer(self.buffer)
+		stream.u8(self.report_summary_mode)
+		stream.u32(self.event_id)
 
 
 class MatchmakeRefereeStats(common.Structure):
 	def __init__(self):
 		super().__init__()
 		self.unique_id = None
 		self.category = None
@@ -1023,24 +1071,27 @@
 	PROTOCOL_ID = 0x6D
 
 
 class MatchmakeRefereeProtocol:
 	METHOD_START_ROUND = 1
 	METHOD_GET_START_ROUND_PARAM = 2
 	METHOD_END_ROUND = 3
-	METHOD_END_ROUND_WITHOUT_REPORT = 4
-	METHOD_GET_ROUND_PARTICIPANTS = 5
-	METHOD_GET_NOT_SUMMARIZED_ROUND = 6
-	METHOD_GET_ROUND = 7
-	METHOD_GET_STATS_PRIMARY = 8
-	METHOD_GET_STATS_PRIMARIES = 9
-	METHOD_GET_STATS_ALL = 10
-	METHOD_CREATE_STATS = 11
-	METHOD_GET_OR_CREATE_STATS = 12
-	METHOD_RESET_STATS = 13
+	METHOD_END_ROUND_WITH_PARTIAL_REPORT = 4
+	METHOD_END_ROUND_WITHOUT_REPORT = 5
+	METHOD_GET_ROUND_PARTICIPANTS = 6
+	METHOD_GET_NOT_SUMMARIZED_ROUND = 7
+	METHOD_GET_ROUND = 8
+	METHOD_GET_STATS_PRIMARY = 9
+	METHOD_GET_STATS_PRIMARIES = 10
+	METHOD_GET_STATS_ALL = 11
+	METHOD_CREATE_STATS = 12
+	METHOD_GET_OR_CREATE_STATS = 13
+	METHOD_RESET_STATS = 14
+	METHOD_GET_EVENT_POINT = 15
+	METHOD_RESET_EVENT_POINT = 16
 	
 	PROTOCOL_ID = 0x78
 
 
 class MatchMakingClient(MatchMakingProtocol):
 	def __init__(self, client):
 		self.settings = client.settings
@@ -1354,19 +1405,19 @@
 		stream = streams.StreamIn(data, self.settings)
 		gatherings = stream.list(stream.anydata)
 		if not stream.eof():
 			raise ValueError("Response is bigger than expected (got %i bytes, but only %i were read)" %(stream.size(), stream.tell()))
 		logger.info("MatchMakingClient.find_by_id -> done")
 		return gatherings
 	
-	async def find_by_single_id(self, id):
+	async def find_by_single_id(self, gid):
 		logger.info("MatchMakingClient.find_by_single_id()")
 		#--- request ---
 		stream = streams.StreamOut(self.settings)
-		stream.list(id, stream.u32)
+		stream.u32(gid)
 		data = await self.client.request(self.PROTOCOL_ID, self.METHOD_FIND_BY_SINGLE_ID, stream.get())
 		
 		#--- response ---
 		stream = streams.StreamIn(data, self.settings)
 		obj = rmc.RMCResponse()
 		obj.result = stream.bool()
 		obj.gathering = stream.anydata()
@@ -2684,14 +2735,27 @@
 		
 		#--- response ---
 		stream = streams.StreamIn(data, self.settings)
 		if not stream.eof():
 			raise ValueError("Response is bigger than expected (got %i bytes, but only %i were read)" %(stream.size(), stream.tell()))
 		logger.info("MatchmakeRefereeClient.end_round -> done")
 	
+	async def end_round_with_partial_report(self, param):
+		logger.info("MatchmakeRefereeClient.end_round_with_partial_report()")
+		#--- request ---
+		stream = streams.StreamOut(self.settings)
+		stream.add(param)
+		data = await self.client.request(self.PROTOCOL_ID, self.METHOD_END_ROUND_WITH_PARTIAL_REPORT, stream.get())
+		
+		#--- response ---
+		stream = streams.StreamIn(data, self.settings)
+		if not stream.eof():
+			raise ValueError("Response is bigger than expected (got %i bytes, but only %i were read)" %(stream.size(), stream.tell()))
+		logger.info("MatchmakeRefereeClient.end_round_with_partial_report -> done")
+	
 	async def end_round_without_report(self, round_id):
 		logger.info("MatchmakeRefereeClient.end_round_without_report()")
 		#--- request ---
 		stream = streams.StreamOut(self.settings)
 		stream.u64(round_id)
 		data = await self.client.request(self.PROTOCOL_ID, self.METHOD_END_ROUND_WITHOUT_REPORT, stream.get())
 		
@@ -3125,16 +3189,16 @@
 		if not isinstance(response, list):
 			raise RuntimeError("Expected list, got %s" %response.__class__.__name__)
 		output.list(response, output.anydata)
 	
 	async def handle_find_by_single_id(self, client, input, output):
 		logger.info("MatchMakingServer.find_by_single_id()")
 		#--- request ---
-		id = input.list(input.u32)
-		response = await self.find_by_single_id(client, id)
+		gid = input.u32()
+		response = await self.find_by_single_id(client, gid)
 		
 		#--- response ---
 		if not isinstance(response, rmc.RMCResponse):
 			raise RuntimeError("Expected RMCResponse, got %s" %response.__class__.__name__)
 		for field in ['result', 'gathering']:
 			if not hasattr(response, field):
 				raise RuntimeError("Missing field in RMCResponse: %s" %field)
@@ -4511,24 +4575,27 @@
 
 class MatchmakeRefereeServer(MatchmakeRefereeProtocol):
 	def __init__(self):
 		self.methods = {
 			self.METHOD_START_ROUND: self.handle_start_round,
 			self.METHOD_GET_START_ROUND_PARAM: self.handle_get_start_round_param,
 			self.METHOD_END_ROUND: self.handle_end_round,
+			self.METHOD_END_ROUND_WITH_PARTIAL_REPORT: self.handle_end_round_with_partial_report,
 			self.METHOD_END_ROUND_WITHOUT_REPORT: self.handle_end_round_without_report,
 			self.METHOD_GET_ROUND_PARTICIPANTS: self.handle_get_round_participants,
 			self.METHOD_GET_NOT_SUMMARIZED_ROUND: self.handle_get_not_summarized_round,
 			self.METHOD_GET_ROUND: self.handle_get_round,
 			self.METHOD_GET_STATS_PRIMARY: self.handle_get_stats_primary,
 			self.METHOD_GET_STATS_PRIMARIES: self.handle_get_stats_primaries,
 			self.METHOD_GET_STATS_ALL: self.handle_get_stats_all,
 			self.METHOD_CREATE_STATS: self.handle_create_stats,
 			self.METHOD_GET_OR_CREATE_STATS: self.handle_get_or_create_stats,
 			self.METHOD_RESET_STATS: self.handle_reset_stats,
+			self.METHOD_GET_EVENT_POINT: self.handle_get_event_point,
+			self.METHOD_RESET_EVENT_POINT: self.handle_reset_event_point,
 		}
 	
 	async def logout(self, client):
 		pass
 	
 	async def handle(self, client, method_id, input, output):
 		if method_id in self.methods:
@@ -4561,14 +4628,20 @@
 	
 	async def handle_end_round(self, client, input, output):
 		logger.info("MatchmakeRefereeServer.end_round()")
 		#--- request ---
 		param = input.extract(MatchmakeRefereeEndRoundParam)
 		await self.end_round(client, param)
 	
+	async def handle_end_round_with_partial_report(self, client, input, output):
+		logger.info("MatchmakeRefereeServer.end_round_with_partial_report()")
+		#--- request ---
+		param = input.extract(MatchmakeRefereeEndRoundParam)
+		await self.end_round_with_partial_report(client, param)
+	
 	async def handle_end_round_without_report(self, client, input, output):
 		logger.info("MatchmakeRefereeServer.end_round_without_report()")
 		#--- request ---
 		round_id = input.u64()
 		await self.end_round_without_report(client, round_id)
 	
 	async def handle_get_round_participants(self, client, input, output):
@@ -4663,26 +4736,38 @@
 		output.add(response)
 	
 	async def handle_reset_stats(self, client, input, output):
 		logger.info("MatchmakeRefereeServer.reset_stats()")
 		#--- request ---
 		await self.reset_stats(client)
 	
+	async def handle_get_event_point(self, client, input, output):
+		logger.warning("MatchmakeRefereeServer.get_event_point is not supported")
+		raise common.RMCError("Core::NotImplemented")
+	
+	async def handle_reset_event_point(self, client, input, output):
+		logger.warning("MatchmakeRefereeServer.reset_event_point is not supported")
+		raise common.RMCError("Core::NotImplemented")
+	
 	async def start_round(self, *args):
 		logger.warning("MatchmakeRefereeServer.start_round not implemented")
 		raise common.RMCError("Core::NotImplemented")
 	
 	async def get_start_round_param(self, *args):
 		logger.warning("MatchmakeRefereeServer.get_start_round_param not implemented")
 		raise common.RMCError("Core::NotImplemented")
 	
 	async def end_round(self, *args):
 		logger.warning("MatchmakeRefereeServer.end_round not implemented")
 		raise common.RMCError("Core::NotImplemented")
 	
+	async def end_round_with_partial_report(self, *args):
+		logger.warning("MatchmakeRefereeServer.end_round_with_partial_report not implemented")
+		raise common.RMCError("Core::NotImplemented")
+	
 	async def end_round_without_report(self, *args):
 		logger.warning("MatchmakeRefereeServer.end_round_without_report not implemented")
 		raise common.RMCError("Core::NotImplemented")
 	
 	async def get_round_participants(self, *args):
 		logger.warning("MatchmakeRefereeServer.get_round_participants not implemented")
 		raise common.RMCError("Core::NotImplemented")
```

### Comparing `nintendoclients-0.0.7/nintendo/nex/matchmaking_eagle.py` & `nintendoclients-0.0.8/nintendo/nex/matchmaking.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,45 +275,74 @@
 		self.started_time = common.DateTime(0)
 		self.user_password = ""
 		self.refer_gid = 0
 		self.user_password_enabled = False
 		self.system_password_enabled = False
 		self.codeword = ""
 	
+	def max_version(self, settings):
+		version = 0
+		if settings["nex.version"] >= 30600:
+			version = 1
+		if settings["nex.version"] >= 30700:
+			version = 2
+		if settings["nex.version"] >= 30800:
+			version = 3
+		if settings["nex.version"] >= 40000:
+			version = 0
+		return version
+	
 	def check_required(self, settings, version):
 		if settings["nex.version"] >= 30500:
 			pass
 		if settings["nex.version"] >= 30000:
 			pass
 		if settings["nex.version"] >= 30500:
 			pass
+		if settings["nex.version"] >= 30600:
+			if version >= 1:
+				pass
+		if settings["nex.version"] >= 30700:
+			if version >= 2:
+				pass
+		if settings["nex.version"] >= 30800:
+			if version >= 3:
+				pass
 		if settings["nex.version"] >= 40000:
-			pass
+			if version >= 0:
+				pass
 	
 	def load(self, stream, version):
 		self.game_mode = stream.u32()
 		self.attribs = stream.list(stream.u32)
 		self.open_participation = stream.bool()
 		self.matchmake_system = stream.u32()
 		self.application_data = stream.buffer()
 		self.num_participants = stream.u32()
 		if stream.settings["nex.version"] >= 30500:
 			self.progress_score = stream.u8()
 		if stream.settings["nex.version"] >= 30000:
 			self.session_key = stream.buffer()
 		if stream.settings["nex.version"] >= 30500:
 			self.option = stream.u32()
+		if stream.settings["nex.version"] >= 30600:
+			if version >= 1:
+				self.param = stream.extract(MatchmakeParam)
+				self.started_time = stream.datetime()
+		if stream.settings["nex.version"] >= 30700:
+			if version >= 2:
+				self.user_password = stream.string()
+		if stream.settings["nex.version"] >= 30800:
+			if version >= 3:
+				self.refer_gid = stream.u32()
+				self.user_password_enabled = stream.bool()
+				self.system_password_enabled = stream.bool()
 		if stream.settings["nex.version"] >= 40000:
-			self.param = stream.extract(MatchmakeParam)
-			self.started_time = stream.datetime()
-			self.user_password = stream.string()
-			self.refer_gid = stream.u32()
-			self.user_password_enabled = stream.bool()
-			self.system_password_enabled = stream.bool()
-			self.codeword = stream.string()
+			if version >= 0:
+				self.codeword = stream.string()
 	
 	def save(self, stream, version):
 		self.check_required(stream.settings, version)
 		stream.u32(self.game_mode)
 		stream.list(self.attribs, stream.u32)
 		stream.bool(self.open_participation)
 		stream.u32(self.matchmake_system)
@@ -321,22 +350,29 @@
 		stream.u32(self.num_participants)
 		if stream.settings["nex.version"] >= 30500:
 			stream.u8(self.progress_score)
 		if stream.settings["nex.version"] >= 30000:
 			stream.buffer(self.session_key)
 		if stream.settings["nex.version"] >= 30500:
 			stream.u32(self.option)
+		if stream.settings["nex.version"] >= 30600:
+			if version >= 1:
+				stream.add(self.param)
+				stream.datetime(self.started_time)
+		if stream.settings["nex.version"] >= 30700:
+			if version >= 2:
+				stream.string(self.user_password)
+		if stream.settings["nex.version"] >= 30800:
+			if version >= 3:
+				stream.u32(self.refer_gid)
+				stream.bool(self.user_password_enabled)
+				stream.bool(self.system_password_enabled)
 		if stream.settings["nex.version"] >= 40000:
-			stream.add(self.param)
-			stream.datetime(self.started_time)
-			stream.string(self.user_password)
-			stream.u32(self.refer_gid)
-			stream.bool(self.user_password_enabled)
-			stream.bool(self.system_password_enabled)
-			stream.string(self.codeword)
+			if version >= 0:
+				stream.string(self.codeword)
 common.DataHolder.register(MatchmakeSession, "MatchmakeSession")
 
 
 class MatchmakeBlockListParam(common.Structure):
 	def __init__(self):
 		super().__init__()
 		self.options = 0
@@ -727,36 +763,30 @@
 
 class MatchmakeRefereeStartRoundParam(common.Structure):
 	def __init__(self):
 		super().__init__()
 		self.personal_data_category = None
 		self.gid = None
 		self.pids = None
-		self.report_summary_mode = None
-		self.event_id = None
 	
 	def check_required(self, settings, version):
-		for field in ['personal_data_category', 'gid', 'pids', 'report_summary_mode', 'event_id']:
+		for field in ['personal_data_category', 'gid', 'pids']:
 			if getattr(self, field) is None:
 				raise ValueError("No value assigned to required field: %s" %field)
 	
 	def load(self, stream, version):
 		self.personal_data_category = stream.u32()
 		self.gid = stream.u32()
 		self.pids = stream.list(stream.pid)
-		self.report_summary_mode = stream.u8()
-		self.event_id = stream.u32()
 	
 	def save(self, stream, version):
 		self.check_required(stream.settings, version)
 		stream.u32(self.personal_data_category)
 		stream.u32(self.gid)
 		stream.list(self.pids, stream.pid)
-		stream.u8(self.report_summary_mode)
-		stream.u32(self.event_id)
 
 
 class MatchmakeRefereeEndRoundParam(common.Structure):
 	def __init__(self):
 		super().__init__()
 		self.round_id = None
 		self.results = None
@@ -778,42 +808,36 @@
 
 class MatchmakeRefereePersonalRoundResult(common.Structure):
 	def __init__(self):
 		super().__init__()
 		self.pid = None
 		self.personal_round_result_flag = None
 		self.round_win_loss = None
-		self.rating_value_change = None
+		self.rating_change = None
 		self.buffer = None
-		self.report_summary_mode = None
-		self.event_id = None
 	
 	def check_required(self, settings, version):
-		for field in ['pid', 'personal_round_result_flag', 'round_win_loss', 'rating_value_change', 'buffer', 'report_summary_mode', 'event_id']:
+		for field in ['pid', 'personal_round_result_flag', 'round_win_loss', 'rating_change', 'buffer']:
 			if getattr(self, field) is None:
 				raise ValueError("No value assigned to required field: %s" %field)
 	
 	def load(self, stream, version):
 		self.pid = stream.pid()
 		self.personal_round_result_flag = stream.u32()
 		self.round_win_loss = stream.u32()
-		self.rating_value_change = stream.s32()
+		self.rating_change = stream.s32()
 		self.buffer = stream.qbuffer()
-		self.report_summary_mode = stream.u8()
-		self.event_id = stream.u32()
 	
 	def save(self, stream, version):
 		self.check_required(stream.settings, version)
 		stream.pid(self.pid)
 		stream.u32(self.personal_round_result_flag)
 		stream.u32(self.round_win_loss)
-		stream.s32(self.rating_value_change)
+		stream.s32(self.rating_change)
 		stream.qbuffer(self.buffer)
-		stream.u8(self.report_summary_mode)
-		stream.u32(self.event_id)
 
 
 class MatchmakeRefereeStats(common.Structure):
 	def __init__(self):
 		super().__init__()
 		self.unique_id = None
 		self.category = None
@@ -1035,27 +1059,24 @@
 	PROTOCOL_ID = 0x6D
 
 
 class MatchmakeRefereeProtocol:
 	METHOD_START_ROUND = 1
 	METHOD_GET_START_ROUND_PARAM = 2
 	METHOD_END_ROUND = 3
-	METHOD_END_ROUND_WITH_PARTIAL_REPORT = 4
-	METHOD_END_ROUND_WITHOUT_REPORT = 5
-	METHOD_GET_ROUND_PARTICIPANTS = 6
-	METHOD_GET_NOT_SUMMARIZED_ROUND = 7
-	METHOD_GET_ROUND = 8
-	METHOD_GET_STATS_PRIMARY = 9
-	METHOD_GET_STATS_PRIMARIES = 10
-	METHOD_GET_STATS_ALL = 11
-	METHOD_CREATE_STATS = 12
-	METHOD_GET_OR_CREATE_STATS = 13
-	METHOD_RESET_STATS = 14
-	METHOD_GET_EVENT_POINT = 15
-	METHOD_RESET_EVENT_POINT = 16
+	METHOD_END_ROUND_WITHOUT_REPORT = 4
+	METHOD_GET_ROUND_PARTICIPANTS = 5
+	METHOD_GET_NOT_SUMMARIZED_ROUND = 6
+	METHOD_GET_ROUND = 7
+	METHOD_GET_STATS_PRIMARY = 8
+	METHOD_GET_STATS_PRIMARIES = 9
+	METHOD_GET_STATS_ALL = 10
+	METHOD_CREATE_STATS = 11
+	METHOD_GET_OR_CREATE_STATS = 12
+	METHOD_RESET_STATS = 13
 	
 	PROTOCOL_ID = 0x78
 
 
 class MatchMakingClient(MatchMakingProtocol):
 	def __init__(self, client):
 		self.settings = client.settings
@@ -1369,19 +1390,19 @@
 		stream = streams.StreamIn(data, self.settings)
 		gatherings = stream.list(stream.anydata)
 		if not stream.eof():
 			raise ValueError("Response is bigger than expected (got %i bytes, but only %i were read)" %(stream.size(), stream.tell()))
 		logger.info("MatchMakingClient.find_by_id -> done")
 		return gatherings
 	
-	async def find_by_single_id(self, id):
+	async def find_by_single_id(self, gid):
 		logger.info("MatchMakingClient.find_by_single_id()")
 		#--- request ---
 		stream = streams.StreamOut(self.settings)
-		stream.list(id, stream.u32)
+		stream.u32(gid)
 		data = await self.client.request(self.PROTOCOL_ID, self.METHOD_FIND_BY_SINGLE_ID, stream.get())
 		
 		#--- response ---
 		stream = streams.StreamIn(data, self.settings)
 		obj = rmc.RMCResponse()
 		obj.result = stream.bool()
 		obj.gathering = stream.anydata()
@@ -2699,27 +2720,14 @@
 		
 		#--- response ---
 		stream = streams.StreamIn(data, self.settings)
 		if not stream.eof():
 			raise ValueError("Response is bigger than expected (got %i bytes, but only %i were read)" %(stream.size(), stream.tell()))
 		logger.info("MatchmakeRefereeClient.end_round -> done")
 	
-	async def end_round_with_partial_report(self, param):
-		logger.info("MatchmakeRefereeClient.end_round_with_partial_report()")
-		#--- request ---
-		stream = streams.StreamOut(self.settings)
-		stream.add(param)
-		data = await self.client.request(self.PROTOCOL_ID, self.METHOD_END_ROUND_WITH_PARTIAL_REPORT, stream.get())
-		
-		#--- response ---
-		stream = streams.StreamIn(data, self.settings)
-		if not stream.eof():
-			raise ValueError("Response is bigger than expected (got %i bytes, but only %i were read)" %(stream.size(), stream.tell()))
-		logger.info("MatchmakeRefereeClient.end_round_with_partial_report -> done")
-	
 	async def end_round_without_report(self, round_id):
 		logger.info("MatchmakeRefereeClient.end_round_without_report()")
 		#--- request ---
 		stream = streams.StreamOut(self.settings)
 		stream.u64(round_id)
 		data = await self.client.request(self.PROTOCOL_ID, self.METHOD_END_ROUND_WITHOUT_REPORT, stream.get())
 		
@@ -3153,16 +3161,16 @@
 		if not isinstance(response, list):
 			raise RuntimeError("Expected list, got %s" %response.__class__.__name__)
 		output.list(response, output.anydata)
 	
 	async def handle_find_by_single_id(self, client, input, output):
 		logger.info("MatchMakingServer.find_by_single_id()")
 		#--- request ---
-		id = input.list(input.u32)
-		response = await self.find_by_single_id(client, id)
+		gid = input.u32()
+		response = await self.find_by_single_id(client, gid)
 		
 		#--- response ---
 		if not isinstance(response, rmc.RMCResponse):
 			raise RuntimeError("Expected RMCResponse, got %s" %response.__class__.__name__)
 		for field in ['result', 'gathering']:
 			if not hasattr(response, field):
 				raise RuntimeError("Missing field in RMCResponse: %s" %field)
@@ -4539,27 +4547,24 @@
 
 class MatchmakeRefereeServer(MatchmakeRefereeProtocol):
 	def __init__(self):
 		self.methods = {
 			self.METHOD_START_ROUND: self.handle_start_round,
 			self.METHOD_GET_START_ROUND_PARAM: self.handle_get_start_round_param,
 			self.METHOD_END_ROUND: self.handle_end_round,
-			self.METHOD_END_ROUND_WITH_PARTIAL_REPORT: self.handle_end_round_with_partial_report,
 			self.METHOD_END_ROUND_WITHOUT_REPORT: self.handle_end_round_without_report,
 			self.METHOD_GET_ROUND_PARTICIPANTS: self.handle_get_round_participants,
 			self.METHOD_GET_NOT_SUMMARIZED_ROUND: self.handle_get_not_summarized_round,
 			self.METHOD_GET_ROUND: self.handle_get_round,
 			self.METHOD_GET_STATS_PRIMARY: self.handle_get_stats_primary,
 			self.METHOD_GET_STATS_PRIMARIES: self.handle_get_stats_primaries,
 			self.METHOD_GET_STATS_ALL: self.handle_get_stats_all,
 			self.METHOD_CREATE_STATS: self.handle_create_stats,
 			self.METHOD_GET_OR_CREATE_STATS: self.handle_get_or_create_stats,
 			self.METHOD_RESET_STATS: self.handle_reset_stats,
-			self.METHOD_GET_EVENT_POINT: self.handle_get_event_point,
-			self.METHOD_RESET_EVENT_POINT: self.handle_reset_event_point,
 		}
 	
 	async def logout(self, client):
 		pass
 	
 	async def handle(self, client, method_id, input, output):
 		if method_id in self.methods:
@@ -4592,20 +4597,14 @@
 	
 	async def handle_end_round(self, client, input, output):
 		logger.info("MatchmakeRefereeServer.end_round()")
 		#--- request ---
 		param = input.extract(MatchmakeRefereeEndRoundParam)
 		await self.end_round(client, param)
 	
-	async def handle_end_round_with_partial_report(self, client, input, output):
-		logger.info("MatchmakeRefereeServer.end_round_with_partial_report()")
-		#--- request ---
-		param = input.extract(MatchmakeRefereeEndRoundParam)
-		await self.end_round_with_partial_report(client, param)
-	
 	async def handle_end_round_without_report(self, client, input, output):
 		logger.info("MatchmakeRefereeServer.end_round_without_report()")
 		#--- request ---
 		round_id = input.u64()
 		await self.end_round_without_report(client, round_id)
 	
 	async def handle_get_round_participants(self, client, input, output):
@@ -4700,38 +4699,26 @@
 		output.add(response)
 	
 	async def handle_reset_stats(self, client, input, output):
 		logger.info("MatchmakeRefereeServer.reset_stats()")
 		#--- request ---
 		await self.reset_stats(client)
 	
-	async def handle_get_event_point(self, client, input, output):
-		logger.warning("MatchmakeRefereeServer.get_event_point is not supported")
-		raise common.RMCError("Core::NotImplemented")
-	
-	async def handle_reset_event_point(self, client, input, output):
-		logger.warning("MatchmakeRefereeServer.reset_event_point is not supported")
-		raise common.RMCError("Core::NotImplemented")
-	
 	async def start_round(self, *args):
 		logger.warning("MatchmakeRefereeServer.start_round not implemented")
 		raise common.RMCError("Core::NotImplemented")
 	
 	async def get_start_round_param(self, *args):
 		logger.warning("MatchmakeRefereeServer.get_start_round_param not implemented")
 		raise common.RMCError("Core::NotImplemented")
 	
 	async def end_round(self, *args):
 		logger.warning("MatchmakeRefereeServer.end_round not implemented")
 		raise common.RMCError("Core::NotImplemented")
 	
-	async def end_round_with_partial_report(self, *args):
-		logger.warning("MatchmakeRefereeServer.end_round_with_partial_report not implemented")
-		raise common.RMCError("Core::NotImplemented")
-	
 	async def end_round_without_report(self, *args):
 		logger.warning("MatchmakeRefereeServer.end_round_without_report not implemented")
 		raise common.RMCError("Core::NotImplemented")
 	
 	async def get_round_participants(self, *args):
 		logger.warning("MatchmakeRefereeServer.get_round_participants not implemented")
 		raise common.RMCError("Core::NotImplemented")
```

### Comparing `nintendoclients-0.0.7/nintendo/nex/matchmaking_mk8d.py` & `nintendoclients-0.0.8/nintendo/nex/matchmaking_mk8d.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,23 @@
 
 
 class MatchmakeSystem:
 	GLOBAL = 1
 	FRIENDS = 2
 
 
+class SimpleSearchConditionOperator:
+	ANY = 0
+	EQUAL = 1
+	GREATER_THAN = 2
+	LESS_THAN = 3
+	GREATER_THAN_OR_EQUAL = 4
+	LESS_THAN_OR_EQUAL = 5
+
+
 class Gathering(common.Structure):
 	def __init__(self):
 		super().__init__()
 		self.id = 0
 		self.owner = 0
 		self.host = 0
 		self.min_participants = 0
@@ -275,45 +284,74 @@
 		self.started_time = common.DateTime(0)
 		self.user_password = ""
 		self.refer_gid = 0
 		self.user_password_enabled = False
 		self.system_password_enabled = False
 		self.codeword = ""
 	
+	def max_version(self, settings):
+		version = 0
+		if settings["nex.version"] >= 30600:
+			version = 1
+		if settings["nex.version"] >= 30700:
+			version = 2
+		if settings["nex.version"] >= 30800:
+			version = 3
+		if settings["nex.version"] >= 40000:
+			version = 0
+		return version
+	
 	def check_required(self, settings, version):
 		if settings["nex.version"] >= 30500:
 			pass
 		if settings["nex.version"] >= 30000:
 			pass
 		if settings["nex.version"] >= 30500:
 			pass
+		if settings["nex.version"] >= 30600:
+			if version >= 1:
+				pass
+		if settings["nex.version"] >= 30700:
+			if version >= 2:
+				pass
+		if settings["nex.version"] >= 30800:
+			if version >= 3:
+				pass
 		if settings["nex.version"] >= 40000:
-			pass
+			if version >= 0:
+				pass
 	
 	def load(self, stream, version):
 		self.game_mode = stream.u32()
 		self.attribs = stream.list(stream.u32)
 		self.open_participation = stream.bool()
 		self.matchmake_system = stream.u32()
 		self.application_data = stream.buffer()
 		self.num_participants = stream.u32()
 		if stream.settings["nex.version"] >= 30500:
 			self.progress_score = stream.u8()
 		if stream.settings["nex.version"] >= 30000:
 			self.session_key = stream.buffer()
 		if stream.settings["nex.version"] >= 30500:
 			self.option = stream.u32()
+		if stream.settings["nex.version"] >= 30600:
+			if version >= 1:
+				self.param = stream.extract(MatchmakeParam)
+				self.started_time = stream.datetime()
+		if stream.settings["nex.version"] >= 30700:
+			if version >= 2:
+				self.user_password = stream.string()
+		if stream.settings["nex.version"] >= 30800:
+			if version >= 3:
+				self.refer_gid = stream.u32()
+				self.user_password_enabled = stream.bool()
+				self.system_password_enabled = stream.bool()
 		if stream.settings["nex.version"] >= 40000:
-			self.param = stream.extract(MatchmakeParam)
-			self.started_time = stream.datetime()
-			self.user_password = stream.string()
-			self.refer_gid = stream.u32()
-			self.user_password_enabled = stream.bool()
-			self.system_password_enabled = stream.bool()
-			self.codeword = stream.string()
+			if version >= 0:
+				self.codeword = stream.string()
 	
 	def save(self, stream, version):
 		self.check_required(stream.settings, version)
 		stream.u32(self.game_mode)
 		stream.list(self.attribs, stream.u32)
 		stream.bool(self.open_participation)
 		stream.u32(self.matchmake_system)
@@ -321,22 +359,29 @@
 		stream.u32(self.num_participants)
 		if stream.settings["nex.version"] >= 30500:
 			stream.u8(self.progress_score)
 		if stream.settings["nex.version"] >= 30000:
 			stream.buffer(self.session_key)
 		if stream.settings["nex.version"] >= 30500:
 			stream.u32(self.option)
+		if stream.settings["nex.version"] >= 30600:
+			if version >= 1:
+				stream.add(self.param)
+				stream.datetime(self.started_time)
+		if stream.settings["nex.version"] >= 30700:
+			if version >= 2:
+				stream.string(self.user_password)
+		if stream.settings["nex.version"] >= 30800:
+			if version >= 3:
+				stream.u32(self.refer_gid)
+				stream.bool(self.user_password_enabled)
+				stream.bool(self.system_password_enabled)
 		if stream.settings["nex.version"] >= 40000:
-			stream.add(self.param)
-			stream.datetime(self.started_time)
-			stream.string(self.user_password)
-			stream.u32(self.refer_gid)
-			stream.bool(self.user_password_enabled)
-			stream.bool(self.system_password_enabled)
-			stream.string(self.codeword)
+			if version >= 0:
+				stream.string(self.codeword)
 common.DataHolder.register(MatchmakeSession, "MatchmakeSession")
 
 
 class MatchmakeBlockListParam(common.Structure):
 	def __init__(self):
 		super().__init__()
 		self.options = 0
@@ -1510,19 +1555,19 @@
 		stream = streams.StreamIn(data, self.settings)
 		gatherings = stream.list(stream.anydata)
 		if not stream.eof():
 			raise ValueError("Response is bigger than expected (got %i bytes, but only %i were read)" %(stream.size(), stream.tell()))
 		logger.info("MatchMakingClient.find_by_id -> done")
 		return gatherings
 	
-	async def find_by_single_id(self, id):
+	async def find_by_single_id(self, gid):
 		logger.info("MatchMakingClient.find_by_single_id()")
 		#--- request ---
 		stream = streams.StreamOut(self.settings)
-		stream.list(id, stream.u32)
+		stream.u32(gid)
 		data = await self.client.request(self.PROTOCOL_ID, self.METHOD_FIND_BY_SINGLE_ID, stream.get())
 		
 		#--- response ---
 		stream = streams.StreamIn(data, self.settings)
 		obj = rmc.RMCResponse()
 		obj.result = stream.bool()
 		obj.gathering = stream.anydata()
@@ -3058,14 +3103,33 @@
 		stream = streams.StreamIn(data, self.settings)
 		objects = stream.list(SimpleSearchObject)
 		if not stream.eof():
 			raise ValueError("Response is bigger than expected (got %i bytes, but only %i were read)" %(stream.size(), stream.tell()))
 		logger.info("MatchmakeExtensionClientMK8D.search_simple_search_object_by_object_ids -> done")
 		return objects
 	
+	async def join_matchmake_session_with_extra_participants(self, gid, join_message, ignore_blacklist, participation_count, extra_participants):
+		logger.info("MatchmakeExtensionClientMK8D.join_matchmake_session_with_extra_participants()")
+		#--- request ---
+		stream = streams.StreamOut(self.settings)
+		stream.u32(gid)
+		stream.string(join_message)
+		stream.bool(ignore_blacklist)
+		stream.u16(participation_count)
+		stream.u32(extra_participants)
+		data = await self.client.request(self.PROTOCOL_ID, self.METHOD_JOIN_MATCHMAKE_SESSION_WITH_EXTRA_PARTICIPANTS, stream.get())
+		
+		#--- response ---
+		stream = streams.StreamIn(data, self.settings)
+		session_key = stream.buffer()
+		if not stream.eof():
+			raise ValueError("Response is bigger than expected (got %i bytes, but only %i were read)" %(stream.size(), stream.tell()))
+		logger.info("MatchmakeExtensionClientMK8D.join_matchmake_session_with_extra_participants -> done")
+		return session_key
+	
 	async def create_competition(self, competition):
 		logger.info("MatchmakeExtensionClientMK8D.create_competition()")
 		#--- request ---
 		stream = streams.StreamOut(self.settings)
 		stream.add(competition)
 		data = await self.client.request(self.PROTOCOL_ID, self.METHOD_CREATE_COMPETITION, stream.get())
 		
@@ -3421,16 +3485,16 @@
 		if not isinstance(response, list):
 			raise RuntimeError("Expected list, got %s" %response.__class__.__name__)
 		output.list(response, output.anydata)
 	
 	async def handle_find_by_single_id(self, client, input, output):
 		logger.info("MatchMakingServer.find_by_single_id()")
 		#--- request ---
-		id = input.list(input.u32)
-		response = await self.find_by_single_id(client, id)
+		gid = input.u32()
+		response = await self.find_by_single_id(client, gid)
 		
 		#--- response ---
 		if not isinstance(response, rmc.RMCResponse):
 			raise RuntimeError("Expected RMCResponse, got %s" %response.__class__.__name__)
 		for field in ['result', 'gathering']:
 			if not hasattr(response, field):
 				raise RuntimeError("Missing field in RMCResponse: %s" %field)
@@ -4860,16 +4924,27 @@
 		
 		#--- response ---
 		if not isinstance(response, list):
 			raise RuntimeError("Expected list, got %s" %response.__class__.__name__)
 		output.list(response, output.add)
 	
 	async def handle_join_matchmake_session_with_extra_participants(self, client, input, output):
-		logger.warning("MatchmakeExtensionServerMK8D.join_matchmake_session_with_extra_participants is not supported")
-		raise common.RMCError("Core::NotImplemented")
+		logger.info("MatchmakeExtensionServerMK8D.join_matchmake_session_with_extra_participants()")
+		#--- request ---
+		gid = input.u32()
+		join_message = input.string()
+		ignore_blacklist = input.bool()
+		participation_count = input.u16()
+		extra_participants = input.u32()
+		response = await self.join_matchmake_session_with_extra_participants(client, gid, join_message, ignore_blacklist, participation_count, extra_participants)
+		
+		#--- response ---
+		if not isinstance(response, bytes):
+			raise RuntimeError("Expected bytes, got %s" %response.__class__.__name__)
+		output.buffer(response)
 	
 	async def handle_custom_get_simple_playing_session(self, client, input, output):
 		logger.warning("MatchmakeExtensionServerMK8D.custom_get_simple_playing_session is not supported")
 		raise common.RMCError("Core::NotImplemented")
 	
 	async def handle_create_competition(self, client, input, output):
 		logger.info("MatchmakeExtensionServerMK8D.create_competition()")
@@ -5146,14 +5221,18 @@
 		logger.warning("MatchmakeExtensionServerMK8D.search_simple_search_object not implemented")
 		raise common.RMCError("Core::NotImplemented")
 	
 	async def search_simple_search_object_by_object_ids(self, *args):
 		logger.warning("MatchmakeExtensionServerMK8D.search_simple_search_object_by_object_ids not implemented")
 		raise common.RMCError("Core::NotImplemented")
 	
+	async def join_matchmake_session_with_extra_participants(self, *args):
+		logger.warning("MatchmakeExtensionServerMK8D.join_matchmake_session_with_extra_participants not implemented")
+		raise common.RMCError("Core::NotImplemented")
+	
 	async def create_competition(self, *args):
 		logger.warning("MatchmakeExtensionServerMK8D.create_competition not implemented")
 		raise common.RMCError("Core::NotImplemented")
 	
 	async def delete_competition(self, *args):
 		logger.warning("MatchmakeExtensionServerMK8D.delete_competition not implemented")
 		raise common.RMCError("Core::NotImplemented")
```

### Comparing `nintendoclients-0.0.7/nintendo/nex/messaging.py` & `nintendoclients-0.0.8/nintendo/nex/messaging.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/monitoring.py` & `nintendoclients-0.0.8/nintendo/nex/monitoring.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/nattraversal.py` & `nintendoclients-0.0.8/nintendo/nex/nattraversal.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/nintendonotification.py` & `nintendoclients-0.0.8/nintendo/nex/nintendonotification.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/notification.py` & `nintendoclients-0.0.8/nintendo/nex/notification.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/prudp.py` & `nintendoclients-0.0.8/nintendo/nex/prudp.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/ranking.py` & `nintendoclients-0.0.8/nintendo/nex/ranking.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/ranking2.py` & `nintendoclients-0.0.8/nintendo/nex/ranking2.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/ranking2_eagle.py` & `nintendoclients-0.0.8/nintendo/nex/ranking2_eagle.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/ranking_mk8d.py` & `nintendoclients-0.0.8/nintendo/nex/ranking_mk8d.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,152 +270,152 @@
 		stream.u32(self.id)
 		stream.add(self.range)
 
 
 class CompetitionRankingInfo(common.Structure):
 	def __init__(self):
 		super().__init__()
-		self.unk1 = None
-		self.unk2 = None
-		self.unk3 = None
+		self.id = None
+		self.num_participants = None
+		self.team_scores = None
 	
 	def check_required(self, settings, version):
-		for field in ['unk1', 'unk2', 'unk3']:
+		for field in ['id', 'num_participants', 'team_scores']:
 			if getattr(self, field) is None:
 				raise ValueError("No value assigned to required field: %s" %field)
 	
 	def load(self, stream, version):
-		self.unk1 = stream.u32()
-		self.unk2 = stream.u32()
-		self.unk3 = stream.list(stream.u32)
+		self.id = stream.u32()
+		self.num_participants = stream.u32()
+		self.team_scores = stream.list(stream.u32)
 	
 	def save(self, stream, version):
 		self.check_required(stream.settings, version)
-		stream.u32(self.unk1)
-		stream.u32(self.unk2)
-		stream.list(self.unk3, stream.u32)
+		stream.u32(self.id)
+		stream.u32(self.num_participants)
+		stream.list(self.team_scores, stream.u32)
 
 
 class CompetitionRankingInfoGetParam(common.Structure):
 	def __init__(self):
 		super().__init__()
-		self.unk = None
+		self.rank_order = None
 		self.range = common.ResultRange()
 	
 	def check_required(self, settings, version):
-		for field in ['unk']:
+		for field in ['rank_order']:
 			if getattr(self, field) is None:
 				raise ValueError("No value assigned to required field: %s" %field)
 	
 	def load(self, stream, version):
-		self.unk = stream.u8()
+		self.rank_order = stream.u8()
 		self.range = stream.extract(common.ResultRange)
 	
 	def save(self, stream, version):
 		self.check_required(stream.settings, version)
-		stream.u8(self.unk)
+		stream.u8(self.rank_order)
 		stream.add(self.range)
 
 
 class CompetitionRankingScoreData(common.Structure):
 	def __init__(self):
 		super().__init__()
-		self.unk1 = None
+		self.rank = None
 		self.pid = None
-		self.unk2 = None
-		self.datetime = None
-		self.unk3 = None
+		self.score = None
+		self.last_update = None
+		self.team_id = 255
 		self.metadata = None
 	
 	def check_required(self, settings, version):
-		for field in ['unk1', 'pid', 'unk2', 'datetime', 'unk3', 'metadata']:
+		for field in ['rank', 'pid', 'score', 'last_update', 'metadata']:
 			if getattr(self, field) is None:
 				raise ValueError("No value assigned to required field: %s" %field)
 	
 	def load(self, stream, version):
-		self.unk1 = stream.u32()
+		self.rank = stream.u32()
 		self.pid = stream.pid()
-		self.unk2 = stream.u32()
-		self.datetime = stream.datetime()
-		self.unk3 = stream.u8()
+		self.score = stream.u32()
+		self.last_update = stream.datetime()
+		self.team_id = stream.u8()
 		self.metadata = stream.qbuffer()
 	
 	def save(self, stream, version):
 		self.check_required(stream.settings, version)
-		stream.u32(self.unk1)
+		stream.u32(self.rank)
 		stream.pid(self.pid)
-		stream.u32(self.unk2)
-		stream.datetime(self.datetime)
-		stream.u8(self.unk3)
+		stream.u32(self.score)
+		stream.datetime(self.last_update)
+		stream.u8(self.team_id)
 		stream.qbuffer(self.metadata)
 
 
 class CompetitionRankingScoreInfo(common.Structure):
 	def __init__(self):
 		super().__init__()
-		self.unk1 = None
+		self.season_id = None
 		self.scores = None
-		self.unk2 = None
-		self.unk3 = None
+		self.num_participants = None
+		self.team_scores = None
 	
 	def check_required(self, settings, version):
-		for field in ['unk1', 'scores', 'unk2', 'unk3']:
+		for field in ['season_id', 'scores', 'num_participants', 'team_scores']:
 			if getattr(self, field) is None:
 				raise ValueError("No value assigned to required field: %s" %field)
 	
 	def load(self, stream, version):
-		self.unk1 = stream.u32()
+		self.season_id = stream.u32()
 		self.scores = stream.list(CompetitionRankingScoreData)
-		self.unk2 = stream.u32()
-		self.unk3 = stream.list(stream.u32)
+		self.num_participants = stream.u32()
+		self.team_scores = stream.list(stream.u32)
 	
 	def save(self, stream, version):
 		self.check_required(stream.settings, version)
-		stream.u32(self.unk1)
+		stream.u32(self.season_id)
 		stream.list(self.scores, stream.add)
-		stream.u32(self.unk2)
-		stream.list(self.unk3, stream.u32)
+		stream.u32(self.num_participants)
+		stream.list(self.team_scores, stream.u32)
 
 
 class CompetitionRankingUploadScoreParam(common.Structure):
 	def __init__(self):
 		super().__init__()
-		self.unk1 = None
-		self.unk2 = None
+		self.id = None
+		self.season_id = None
 		self.unk3 = None
-		self.unk4 = None
-		self.unk5 = None
-		self.unk6 = None
-		self.unk7 = None
+		self.score = None
+		self.team_id = None
+		self.team_score = None
+		self.is_first_upload = None
 		self.metadata = None
 	
 	def check_required(self, settings, version):
-		for field in ['unk1', 'unk2', 'unk3', 'unk4', 'unk5', 'unk6', 'unk7', 'metadata']:
+		for field in ['id', 'season_id', 'unk3', 'score', 'team_id', 'team_score', 'is_first_upload', 'metadata']:
 			if getattr(self, field) is None:
 				raise ValueError("No value assigned to required field: %s" %field)
 	
 	def load(self, stream, version):
-		self.unk1 = stream.u32()
-		self.unk2 = stream.u32()
+		self.id = stream.u32()
+		self.season_id = stream.u32()
 		self.unk3 = stream.u32()
-		self.unk4 = stream.u32()
-		self.unk5 = stream.u8()
-		self.unk6 = stream.u32()
-		self.unk7 = stream.bool()
+		self.score = stream.u32()
+		self.team_id = stream.u8()
+		self.team_score = stream.u32()
+		self.is_first_upload = stream.bool()
 		self.metadata = stream.qbuffer()
 	
 	def save(self, stream, version):
 		self.check_required(stream.settings, version)
-		stream.u32(self.unk1)
-		stream.u32(self.unk2)
+		stream.u32(self.id)
+		stream.u32(self.season_id)
 		stream.u32(self.unk3)
-		stream.u32(self.unk4)
-		stream.u8(self.unk5)
-		stream.u32(self.unk6)
-		stream.bool(self.unk7)
+		stream.u32(self.score)
+		stream.u8(self.team_id)
+		stream.u32(self.team_score)
+		stream.bool(self.is_first_upload)
 		stream.qbuffer(self.metadata)
 
 
 class RankingProtocolMK8D:
 	METHOD_UPLOAD_SCORE = 1
 	METHOD_DELETE_SCORE = 2
 	METHOD_DELETE_ALL_SCORES = 3
```

### Comparing `nintendoclients-0.0.7/nintendo/nex/remotelog.py` & `nintendoclients-0.0.8/nintendo/nex/remotelog.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/rmc.py` & `nintendoclients-0.0.8/nintendo/nex/rmc.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/screening.py` & `nintendoclients-0.0.8/nintendo/nex/screening.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/secure.py` & `nintendoclients-0.0.8/nintendo/nex/secure.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/settings.py` & `nintendoclients-0.0.8/nintendo/nex/settings.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/streams.py` & `nintendoclients-0.0.8/nintendo/nex/streams.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/subscriber.py` & `nintendoclients-0.0.8/nintendo/nex/subscriber.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nex/utility.py` & `nintendoclients-0.0.8/nintendo/nex/utility.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/nnas.py` & `nintendoclients-0.0.8/nintendo/nnas.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendo/switch.py` & `nintendoclients-0.0.8/nintendo/switch.py`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/nintendoclients.egg-info/SOURCES.txt` & `nintendoclients-0.0.8/nintendoclients.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nintendoclients-0.0.7/setup.py` & `nintendoclients-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 long_description = \
 	"This library implements various network protocols made by Nintendo."
 
 setuptools.setup(
 	name = "nintendoclients",
-	version = "0.0.7",
+	version = "0.0.8",
 	description = "Nintendo network library",
 	long_description = long_description,
 	author = "Yannik Marchand",
 	author_email = "ymarchand@me.com",
 	url = "https://github.com/kinnay/NintendoClients",
 	license = "MIT",
 	packages = [
```

