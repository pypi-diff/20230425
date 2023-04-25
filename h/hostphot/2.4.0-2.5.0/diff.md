# Comparing `tmp/hostphot-2.4.0.tar.gz` & `tmp/hostphot-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hostphot-2.4.0.tar", last modified: Thu Mar 23 14:37:45 2023, max compression
+gzip compressed data, was "hostphot-2.5.0.tar", last modified: Tue Apr 25 09:48:32 2023, max compression
```

## Comparing `hostphot-2.4.0.tar` & `hostphot-2.5.0.tar`

### file list

```diff
@@ -1,324 +1,325 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.396258 hostphot-2.4.0/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1065 2022-05-31 09:22:42.000000 hostphot-2.4.0/LICENSE
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.4.0/MANIFEST.in
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7767 2023-03-23 14:37:45.396258 hostphot-2.4.0/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7228 2023-02-23 11:18:32.000000 hostphot-2.4.0/README.md
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      187 2022-05-31 09:22:42.000000 hostphot-2.4.0/pyproject.toml
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      158 2023-03-23 14:36:04.000000 hostphot-2.4.0/requirements.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-03-23 14:37:45.396258 hostphot-2.4.0/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1257 2023-02-22 10:47:46.000000 hostphot-2.4.0/setup.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.328259 hostphot-2.4.0/src/
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.332259 hostphot-2.4.0/src/hostphot/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      412 2022-08-30 07:45:59.000000 hostphot-2.4.0/src/hostphot/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      123 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/_constants.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       47 2023-03-23 14:36:34.000000 hostphot-2.4.0/src/hostphot/_version.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1762 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/coadd.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    38665 2023-03-23 14:36:04.000000 hostphot-2.4.0/src/hostphot/cutouts.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6150 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/dust.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.332259 hostphot-2.4.0/src/hostphot/filters/
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.332259 hostphot-2.4.0/src/hostphot/filters/2MASS/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1218 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/2MASS/2MASS_H.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2247 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/2MASS/2MASS_J.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1596 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/2MASS/2MASS_Ks.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/2MASS/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1549 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/AAA_README
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.336259 hostphot-2.4.0/src/hostphot/filters/DES/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.4.0/src/hostphot/filters/DES/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3387 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/DES/DES_Y.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4281 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/DES/DES_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4515 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/DES/DES_i.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4516 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/DES/DES_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4338 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/DES/DES_z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.336259 hostphot-2.4.0/src/hostphot/filters/GALEX/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/GALEX/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6777 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/GALEX/GALEX_FUV.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18911 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/GALEX/GALEX_NUV.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.328259 hostphot-2.4.0/src/hostphot/filters/HST/
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.344259 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    23838 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    32416 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4110 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15624 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    31966 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    43735 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    29858 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5234 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    37258 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   103143 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    53451 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7990 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21666 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9107 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9858 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    36616 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10646 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11519 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12578 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13680 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    53850 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    14675 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15873 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    17289 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18750 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    61170 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19635 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.348259 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9747 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2486 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2874 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3264 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12445 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24500 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3077 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    33411 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13978 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21021 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4877 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11680 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5199 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12148 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6879 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7831 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.352259 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24275 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20849 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12018 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18588 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    17947 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6506 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    41358 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5506 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21662 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30947 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20965 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11516 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7894 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7479 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30813 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26323 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.352259 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3240 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24427 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3363 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    35249 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20994 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4858 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4820 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    43711 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6876 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5510 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7212 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9291 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11541 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7906 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30812 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13019 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.356258 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8959 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9826 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21512 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22426 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4121 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5064 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6580 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3261 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3792 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5421 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13977 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6752 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10046 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4738 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6887 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.372258 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   156254 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21978 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    29976 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21591 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7558 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    56436 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15547 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19356 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   146819 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4504 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9638 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26406 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7035 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9314 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18697 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9833 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3637 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    32782 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    72677 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5098 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5804 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    38578 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    63538 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    97333 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    51442 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21890 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    34917 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4204 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3675 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2150 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11299 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11865 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13792 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20007 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19898 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    36590 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    54378 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    33733 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    57316 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12497 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.388258 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   156503 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20752 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    29190 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21479 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7566 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    55542 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15542 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19332 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   147032 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4495 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9640 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26441 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7031 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9300 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18727 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9871 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    32751 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    72732 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5104 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5798 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    38608 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    63493 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    97494 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    51384 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21858 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    34960 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4209 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3686 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2154 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11309 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3233 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11857 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13805 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20019 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19919 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    36600 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    54473 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    33739 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    57507 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12507 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.388258 hostphot-2.4.0/src/hostphot/filters/LegacySurvey/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2281 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/LegacySurvey/BASS_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3180 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/LegacySurvey/BASS_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21743 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/LegacySurvey/DECAM_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/LegacySurvey/DECAM_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/LegacySurvey/DECAM_z.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7028 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/LegacySurvey/MzLS_z.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      300 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/LegacySurvey/README.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4275 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/LegacySurvey/init_BASS_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5840 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/LegacySurvey/init_BASS_r.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.388258 hostphot-2.4.0/src/hostphot/filters/PS1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      136 2022-05-31 09:22:42.000000 hostphot-2.4.0/src/hostphot/filters/PS1/AAA_README.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3717 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/PS1/PS1_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3759 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/PS1/PS1_i.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3885 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/PS1/PS1_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4385 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/PS1/PS1_y.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3486 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/PS1/PS1_z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.388258 hostphot-2.4.0/src/hostphot/filters/SDSS/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       72 2022-05-31 09:22:42.000000 hostphot-2.4.0/src/hostphot/filters/SDSS/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1414 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/SDSS/SDSS_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1260 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/SDSS/SDSS_i.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1176 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/SDSS/SDSS_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4718 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/SDSS/SDSS_u.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2509 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/SDSS/SDSS_z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.392258 hostphot-2.4.0/src/hostphot/filters/Spitzer/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      189 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/Spitzer/README.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8211 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8421 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6531 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7375 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2816 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.392258 hostphot-2.4.0/src/hostphot/filters/VISTA/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       84 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/VISTA/README.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    39168 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/VISTA/VISTA_H.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    50048 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/VISTA/VISTA_J.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    41344 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/VISTA/VISTA_Ks.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    46341 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/VISTA/VISTA_Y.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   176418 2022-11-14 14:06:00.000000 hostphot-2.4.0/src/hostphot/filters/VISTA/VISTA_Z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.392258 hostphot-2.4.0/src/hostphot/filters/WISE/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/filters/WISE/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2961 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/WISE/WISE_W1.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3528 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/WISE/WISE_W2.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24404 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/WISE/WISE_W3.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19734 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/filters/WISE/WISE_W4.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      739 2023-03-13 12:52:42.000000 hostphot-2.4.0/src/hostphot/filters/config.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18615 2023-03-23 14:36:04.000000 hostphot-2.4.0/src/hostphot/global_photometry.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2494 2022-07-28 14:32:41.000000 hostphot-2.4.0/src/hostphot/image_cleaning.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10939 2023-03-23 14:36:04.000000 hostphot-2.4.0/src/hostphot/image_masking.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12343 2023-02-15 13:45:13.000000 hostphot-2.4.0/src/hostphot/interactive_aperture.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12429 2023-03-23 14:36:04.000000 hostphot-2.4.0/src/hostphot/local_photometry.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7869 2023-03-23 14:36:04.000000 hostphot-2.4.0/src/hostphot/objects_detect.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10706 2022-08-15 08:03:30.000000 hostphot-2.4.0/src/hostphot/rgb_images.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22677 2023-03-13 12:52:42.000000 hostphot-2.4.0/src/hostphot/utils.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.332259 hostphot-2.4.0/src/hostphot.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7767 2023-03-23 14:37:45.000000 hostphot-2.4.0/src/hostphot.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    14675 2023-03-23 14:37:45.000000 hostphot-2.4.0/src/hostphot.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-03-23 14:37:45.000000 hostphot-2.4.0/src/hostphot.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      158 2023-03-23 14:37:45.000000 hostphot-2.4.0/src/hostphot.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        9 2023-03-23 14:37:45.000000 hostphot-2.4.0/src/hostphot.egg-info/top_level.txt
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-03-23 14:37:45.392258 hostphot-2.4.0/tests/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2609 2023-03-13 12:52:42.000000 hostphot-2.4.0/tests/test_cutouts.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1040 2022-08-15 08:03:30.000000 hostphot-2.4.0/tests/test_global_phot.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      460 2022-07-28 14:32:41.000000 hostphot-2.4.0/tests/test_interactivity.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1051 2022-08-15 08:03:30.000000 hostphot-2.4.0/tests/test_local_phot.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1095 2022-07-28 14:32:41.000000 hostphot-2.4.0/tests/test_preprocessing.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      857 2022-08-15 08:03:30.000000 hostphot-2.4.0/tests/test_rgb_images.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.966889 hostphot-2.5.0/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1065 2022-05-31 09:22:42.000000 hostphot-2.5.0/LICENSE
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.5.0/MANIFEST.in
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8755 2023-04-25 09:48:32.966889 hostphot-2.5.0/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8216 2023-04-25 09:34:42.000000 hostphot-2.5.0/README.md
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      187 2022-05-31 09:22:42.000000 hostphot-2.5.0/pyproject.toml
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      190 2023-04-25 09:34:42.000000 hostphot-2.5.0/requirements.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-04-25 09:48:32.966889 hostphot-2.5.0/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1257 2023-02-22 10:47:46.000000 hostphot-2.5.0/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.910889 hostphot-2.5.0/src/
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.914889 hostphot-2.5.0/src/hostphot/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      412 2022-08-30 07:45:59.000000 hostphot-2.5.0/src/hostphot/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      123 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/_constants.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       47 2023-04-25 09:34:42.000000 hostphot-2.5.0/src/hostphot/_version.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1762 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/coadd.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    39841 2023-04-25 09:34:42.000000 hostphot-2.5.0/src/hostphot/cutouts.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6150 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/dust.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.914889 hostphot-2.5.0/src/hostphot/filters/
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.914889 hostphot-2.5.0/src/hostphot/filters/2MASS/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1218 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/2MASS/2MASS_H.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2247 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/2MASS/2MASS_J.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1596 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/2MASS/2MASS_Ks.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/2MASS/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1549 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/AAA_README
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.918889 hostphot-2.5.0/src/hostphot/filters/DES/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.5.0/src/hostphot/filters/DES/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3387 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/DES/DES_Y.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4281 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/DES/DES_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4515 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/DES/DES_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4516 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/DES/DES_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4338 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/DES/DES_z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.918889 hostphot-2.5.0/src/hostphot/filters/GALEX/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/GALEX/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6777 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/GALEX/GALEX_FUV.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18911 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/GALEX/GALEX_NUV.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.918889 hostphot-2.5.0/src/hostphot/filters/HST/
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.922889 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    23838 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    32416 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4110 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15624 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    31966 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    43735 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    29858 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5234 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    37258 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   103143 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    53451 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7990 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21666 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9107 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9858 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    36616 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10646 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11519 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12578 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13680 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    53850 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    14675 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15873 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    17289 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18750 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    61170 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19635 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11835 2023-04-25 09:34:42.000000 hostphot-2.5.0/src/hostphot/filters/HST/HST_filters.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.926889 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9747 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2486 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2874 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3264 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12445 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24500 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3077 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    33411 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13978 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21021 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4877 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11680 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5199 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12148 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6879 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7831 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.930889 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24275 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20849 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12018 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18588 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    17947 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6506 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    41358 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5506 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21662 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30947 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20965 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11516 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7894 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7479 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30813 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26323 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.930889 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3240 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24427 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3363 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    35249 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20994 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4858 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4820 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    43711 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6876 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5510 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7212 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9291 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11541 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7906 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30812 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13019 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.934889 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8959 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9826 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21512 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22426 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4121 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5064 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6580 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3261 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3792 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5421 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13977 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6752 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10046 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4738 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6887 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.946889 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   156254 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21978 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    29976 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21591 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7558 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    56436 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15547 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19356 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   146819 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4504 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9638 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26406 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7035 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9314 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18697 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9833 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3637 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    32782 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    72677 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5098 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5804 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    38578 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    63538 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    97333 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    51442 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21890 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    34917 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4204 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3675 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2150 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11299 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11865 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13792 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20007 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19898 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    36590 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    54378 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    33733 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    57316 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12497 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.962889 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   156503 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20752 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    29190 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21479 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7566 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    55542 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15542 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19332 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   147032 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4495 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9640 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26441 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7031 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9300 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18727 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9871 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    32751 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    72732 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5104 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5798 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    38608 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    63493 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    97494 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    51384 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21858 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    34960 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4209 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3686 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2154 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11309 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3233 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11857 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13805 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20019 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19919 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    36600 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    54473 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    33739 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    57507 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12507 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.962889 hostphot-2.5.0/src/hostphot/filters/LegacySurvey/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2281 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/LegacySurvey/BASS_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3180 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/LegacySurvey/BASS_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21743 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/LegacySurvey/DECAM_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/LegacySurvey/DECAM_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/LegacySurvey/DECAM_z.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7028 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/LegacySurvey/MzLS_z.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      300 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/LegacySurvey/README.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4275 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/LegacySurvey/init_BASS_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5840 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/LegacySurvey/init_BASS_r.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.962889 hostphot-2.5.0/src/hostphot/filters/PS1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      136 2022-05-31 09:22:42.000000 hostphot-2.5.0/src/hostphot/filters/PS1/AAA_README.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3717 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/PS1/PS1_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3759 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/PS1/PS1_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3885 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/PS1/PS1_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4385 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/PS1/PS1_y.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3486 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/PS1/PS1_z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.962889 hostphot-2.5.0/src/hostphot/filters/SDSS/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       72 2022-05-31 09:22:42.000000 hostphot-2.5.0/src/hostphot/filters/SDSS/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1414 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/SDSS/SDSS_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1260 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/SDSS/SDSS_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1176 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/SDSS/SDSS_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4718 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/SDSS/SDSS_u.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2509 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/SDSS/SDSS_z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.966889 hostphot-2.5.0/src/hostphot/filters/Spitzer/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      189 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/Spitzer/README.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8211 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8421 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6531 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7375 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2816 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.966889 hostphot-2.5.0/src/hostphot/filters/VISTA/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       84 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/VISTA/README.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    39168 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/VISTA/VISTA_H.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    50048 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/VISTA/VISTA_J.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    41344 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/VISTA/VISTA_Ks.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    46341 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/VISTA/VISTA_Y.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   176418 2022-11-14 14:06:00.000000 hostphot-2.5.0/src/hostphot/filters/VISTA/VISTA_Z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.966889 hostphot-2.5.0/src/hostphot/filters/WISE/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/filters/WISE/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2961 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/WISE/WISE_W1.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3528 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/WISE/WISE_W2.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24404 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/WISE/WISE_W3.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19734 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/filters/WISE/WISE_W4.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      739 2023-04-24 13:20:08.000000 hostphot-2.5.0/src/hostphot/filters/config.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22688 2023-04-25 09:34:42.000000 hostphot-2.5.0/src/hostphot/global_photometry.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2494 2022-07-28 14:32:41.000000 hostphot-2.5.0/src/hostphot/image_cleaning.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12319 2023-04-25 09:34:42.000000 hostphot-2.5.0/src/hostphot/image_masking.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12493 2023-04-25 09:34:42.000000 hostphot-2.5.0/src/hostphot/interactive_aperture.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13116 2023-04-25 09:34:42.000000 hostphot-2.5.0/src/hostphot/local_photometry.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8326 2023-04-25 09:34:42.000000 hostphot-2.5.0/src/hostphot/objects_detect.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10706 2022-08-15 08:03:30.000000 hostphot-2.5.0/src/hostphot/rgb_images.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    27890 2023-04-25 09:34:42.000000 hostphot-2.5.0/src/hostphot/utils.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.914889 hostphot-2.5.0/src/hostphot.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8755 2023-04-25 09:48:32.000000 hostphot-2.5.0/src/hostphot.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    14716 2023-04-25 09:48:32.000000 hostphot-2.5.0/src/hostphot.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-04-25 09:48:32.000000 hostphot-2.5.0/src/hostphot.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      193 2023-04-25 09:48:32.000000 hostphot-2.5.0/src/hostphot.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        9 2023-04-25 09:48:32.000000 hostphot-2.5.0/src/hostphot.egg-info/top_level.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-25 09:48:32.966889 hostphot-2.5.0/tests/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2771 2023-04-25 09:34:42.000000 hostphot-2.5.0/tests/test_cutouts.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1040 2022-08-15 08:03:30.000000 hostphot-2.5.0/tests/test_global_phot.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      460 2022-07-28 14:32:41.000000 hostphot-2.5.0/tests/test_interactivity.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1055 2023-04-25 09:34:42.000000 hostphot-2.5.0/tests/test_local_phot.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1095 2022-07-28 14:32:41.000000 hostphot-2.5.0/tests/test_preprocessing.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      860 2023-04-25 09:34:42.000000 hostphot-2.5.0/tests/test_rgb_images.py
```

### Comparing `hostphot-2.4.0/LICENSE` & `hostphot-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/PKG-INFO` & `hostphot-2.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hostphot
-Version: 2.4.0
+Version: 2.5.0
 Summary: Global and local photometry of galaxies hosting supernovae or other transients
 Home-page: https://github.com/temuller/hostphot
 Author: Tomás Enrique Müller-Bravo and Lluís Galbany
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -192,14 +192,32 @@
   number = {76}, 
   pages = {4508},  
   journal = {Journal of Open Source Software} 
 } 
 ```
 
 ## What's new!
+v2.5.0:
+* Systematic error floor added to PS1 photometry
+* Added missing uncertainties in the error budget of DES (~5 mmag) 
+* Flux/counts have been added to output photometry
+* GALEX now downloads images with largest exposure time by default
+* Fixed image realignment/orientation between different surveys when using common apertures (for masking and global photometry)
+* Added option to output mask parameters, and also aperture parameters for global photometry
+* Option added to set a distant threshold to identify the host galaxy in the image (by default use the nearest object)
+* Slight change in the column names of the local photometry output file
+* Offsets in SDSS zeropoints to place it in the AB system
+* overwrite set to True by default when downloading image cutouts
+* Other minor bugs fixed
+
+v2.4.0:
+* Fixed and improved GALEX cutouts
+* Better galaxy identification
+* Better output plots for masked images
+* Option to return NaN or raise an exception when getting photometry
 
 v2.3.2:
 * Improved download of GALEX images (download even if they seem to be just background noise)
 
 
 ## Acknowledgements
```

### Comparing `hostphot-2.4.0/README.md` & `hostphot-2.5.0/src/hostphot.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: hostphot
+Version: 2.5.0
+Summary: Global and local photometry of galaxies hosting supernovae or other transients
+Home-page: https://github.com/temuller/hostphot
+Author: Tomás Enrique Müller-Bravo and Lluís Galbany
+Author-email: t.e.muller-bravo@ice.csic.es
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8, <3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
 	<img src="docs/hostphot_logo.png" alt="drawing" width="300"/>
 </p>
 
 Global and local photometry of galaxies hosting supernovae or other transients
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fhostphot-blue.svg?style=flat)](https://github.com/temuller/hostphot)
@@ -177,14 +192,32 @@
   number = {76}, 
   pages = {4508},  
   journal = {Journal of Open Source Software} 
 } 
 ```
 
 ## What's new!
+v2.5.0:
+* Systematic error floor added to PS1 photometry
+* Added missing uncertainties in the error budget of DES (~5 mmag) 
+* Flux/counts have been added to output photometry
+* GALEX now downloads images with largest exposure time by default
+* Fixed image realignment/orientation between different surveys when using common apertures (for masking and global photometry)
+* Added option to output mask parameters, and also aperture parameters for global photometry
+* Option added to set a distant threshold to identify the host galaxy in the image (by default use the nearest object)
+* Slight change in the column names of the local photometry output file
+* Offsets in SDSS zeropoints to place it in the AB system
+* overwrite set to True by default when downloading image cutouts
+* Other minor bugs fixed
+
+v2.4.0:
+* Fixed and improved GALEX cutouts
+* Better galaxy identification
+* Better output plots for masked images
+* Option to return NaN or raise an exception when getting photometry
 
 v2.3.2:
 * Improved download of GALEX images (download even if they seem to be just background noise)
 
 
 ## Acknowledgements
```

### Comparing `hostphot-2.4.0/setup.py` & `hostphot-2.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/coadd.py` & `hostphot-2.5.0/src/hostphot/coadd.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/cutouts.py` & `hostphot-2.5.0/src/hostphot/cutouts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import copy
-import gzip
 import shutil
 import tarfile
 import requests  # for several surveys
 import numpy as np
 import pandas as pd
 
 # for VISTA
@@ -19,24 +18,24 @@
 
 import pyvo  # 2MASS
 from pyvo.dal import sia  # DES, DELVE
 from astroquery.sdss import SDSS
 from astroquery.skyview import SkyView  # other surveys
 from astroquery.mast import Observations  # for GALEX
 
-from reproject import reproject_interp, reproject_exact
-from reproject.mosaicking import find_optimal_celestial_wcs
+from reproject import reproject_interp
 
 from hostphot._constants import workdir
 from hostphot.utils import (
     get_survey_filters,
     clean_dir,
     check_work_dir,
     check_survey_validity,
     check_filters_validity,
+    check_HST_inputs,
     survey_pixel_scale,
 )
 
 import warnings
 from astropy.utils.exceptions import AstropyWarning
 
 
@@ -217,22 +216,25 @@
     for filt in filters:
         cond_filt = imgs_df["obs_bandpass"] == filt
 
         selected_images = imgs_df[cond_filt & (cond_stack & cond_image)]
         selected_weights = imgs_df[cond_filt & (cond_stack & cond_weight)]
 
         if len(selected_images) > 0:
-            # pick image with longest exposure time
+            # pick image with the longest exposure time
             max_exptime = np.argmax(selected_images["exptime"])
             row = selected_images.iloc[max_exptime]
             url = row["access_url"]  # get the download URL
 
-            max_exptime = np.argmax(selected_weights["exptime"])
-            row_w = selected_weights.iloc[max_exptime]
-            url_w = row_w["access_url"]
+            if len(selected_weights) == 0:
+                url_w = None
+            else:
+                max_exptime = np.argmax(selected_weights["exptime"])
+                row_w = selected_weights.iloc[max_exptime]
+                url_w = row_w["access_url"]
         else:
             url = url_w = None
         url_list.append(url)
         url_w_list.append(url_w)
 
     return url_list, url_w_list
 
@@ -285,71 +287,89 @@
         hdu_list.append(hdu_sublist)
 
     return hdu_list
 
 
 # SDSS
 # ----------------------------------------
-def get_SDSS_images(ra, dec, size=3, filters=None):
+def get_SDSS_images(ra, dec, size=3, filters=None, version=None):
     """Downloads a set of SDSS fits images for a given set
     of coordinates and filters using SkyView.
 
     Parameters
     ----------
     ra: str or float
         Right ascension in degrees.
     dec: str or float
         Declination in degrees.
     size: float or ~astropy.units.Quantity, default ``3``
         Image size. If a float is given, the units are assumed to be arcmin.
     filters: str, default ``None``
         Filters to use. If ``None``, uses ``ugriz``.
+    version: str, default ``None``
+        Data release version to use. If not given, use the latest one (``dr17``).
 
     Return
     ------
     hdu_list: list
         List with fits images for the given filters.
         `None` is returned if no image is found.
     """
     survey = "SDSS"
     if filters is None:
         filters = get_survey_filters(survey)
     check_filters_validity(filters, survey)
+    # check data release version
+    if version is None:
+        version = "dr17"
+
+    versions = [f"dr{i}" for i in range(12, 17 + 1)]
+    assert (
+        version in versions
+    ), f"The given version ({version}) is not a valid data release: {versions}"
+    dr = int(version.replace("dr", ""))
 
     if isinstance(size, (float, int)):
         size_arcsec = (size * u.arcmin).to(u.arcsec)
     else:
         size_arcsec = size.to(u.arcsec)
 
     pixel_scale = survey_pixel_scale(survey)
     size_pixels = int(size_arcsec.value / pixel_scale)
 
     pos = SkyCoord(ra=ra * u.degree, dec=dec * u.degree)
-    for radius in np.arange(1, 30):
-        ids = SDSS.query_region(pos, radius=radius * u.arcsec)
+    for radius in np.arange(1, 60, 1):
+        ids = SDSS.query_region(pos, radius=radius * u.arcsec, data_release=dr)
         if ids is not None:
             break
 
     if ids is None:
         return None
 
-    # get images
-    hdu_id = len(ids) // 2
-    if hdu_id == 0:
-        hdu_list = SDSS.get_images(matches=ids, band=filters)
-    else:
-        sub_id = ids[hdu_id - 1 : hdu_id]  # get the one in the middle
-        hdu_list = SDSS.get_images(matches=sub_id, band=filters)
+    pointings_ra = ids["ra"].value
+    pointings_dec = ids["dec"].value
+    dist = np.sqrt(
+        (pointings_ra - ra) ** 2 * (np.cos(pointings_dec * np.pi / 180) ** 2)
+        + (pointings_dec - dec) ** 2
+    )
+
+    # get the pointing closest to the given coordinates
+    pointing_id = np.argmin(dist)
+    ids2remove = list(np.arange(len(dist)))
+    del ids2remove[pointing_id]
+    ids.remove_rows(ids2remove)
+
+    # download images here
+    hdu_list = SDSS.get_images(matches=ids, band=filters, data_release=dr)
 
     # SDSS images are large so need to be trimmed
     for hdu in hdu_list:
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", AstropyWarning)
             img_wcs = wcs.WCS(hdu[0].header)
-        pos = SkyCoord(ra=ra * u.degree, dec=dec * u.degree)
 
         trimmed_data = Cutout2D(hdu[0].data, pos, size_pixels, img_wcs)
         hdu[0].data = trimmed_data.data
         hdu[0].header.update(trimmed_data.wcs.to_header())
 
     return hdu_list
 
@@ -372,31 +392,25 @@
     Returns
     -------
     dist_from_center: float
         Distance of from the image center to the galaxy
         position in pixel units.
     """
     # coordinates of the image center
-    img_wcs = wcs.WCS(header)
-    img_ra, img_dec = header['RA_CENT'], header['DEC_CENT']
-    img_coord = SkyCoord(
-        ra=img_ra, dec=img_dec, unit=(u.degree, u.degree), frame="icrs"
-    )
-    img_x, img_y = img_wcs.world_to_pixel(img_coord)
+    img_ra, img_dec = float(header["RA_CENT"]), float(header["DEC_CENT"])
 
-    # coordinates of the galaxy
-    host_coord = SkyCoord(
-        ra=host_ra, dec=host_dec, unit=(u.degree, u.degree), frame="icrs"
+    # distance to the galaxy
+    dist_from_center = np.sqrt(
+        (img_ra - host_ra) ** 2 * (np.cos(img_dec * np.pi / 180) ** 2)
+        + (img_dec - host_dec) ** 2
     )
-    host_x, host_y = img_wcs.world_to_pixel(host_coord)
-
-    dist_from_center = np.sqrt((img_x - host_x) ** 2 + (img_y - host_y) ** 2)
 
     return dist_from_center
 
+
 def get_GALEX_images(ra, dec, size=3, filters=None, version=None):
     """Downloads a set of GALEX fits images for a given set
     of coordinates and filters.
 
     Parameters
     ----------
     ra: str or float
@@ -406,27 +420,28 @@
     size: float or ~astropy.units.Quantity, default ``3``
         Image size. If a float is given, the units are assumed to be arcmin.
     filters: str, default ``None``
         Filters to use. If ``None``, uses ``FUV, NUV``.
     version: str, default ``None``
         Version of GALEX images. Either Deep (``DIS``), Medium (``MIS``) or
         All-Sky Imaging Survey (``AIS``), or Nearby Galaxy Survey (``NGS``) or
-        Guest Investigator Survey (``GII``). By default, ``AIS`` is used.
+        Guest Investigator Survey (``GII``). If ``None``, take the image with the
+        longest exposure time.
 
     Return
     ------
     hdu_list: list
         List with fits images for the given filters.
         ``None`` is returned if no image is found.
     """
     survey = "GALEX"
-    if version is None:
-        version = 'AIS'
     if filters is None:
         filters = get_survey_filters(survey)
+    if isinstance(filters, str):
+        filters = [filters]
     check_filters_validity(filters, survey)
 
     if isinstance(size, (float, int)):
         size_arcsec = (size * u.arcmin).to(u.arcsec)
     else:
         size_arcsec = size.to(u.arcsec)
 
@@ -438,70 +453,74 @@
         coords = SkyCoord(
             ra=ra, dec=dec, unit=(u.degree, u.degree), frame="icrs"
         )
 
     obs_table = Observations.query_criteria(
         coordinates=coords, radius=size_arcsec, obs_collection=["GALEX"]
     )
-    obs_df = obs_table.to_pandas()
-    print(obs_df.jpegURL.values)
-    print(obs_df.dataURL.values)
-    print(obs_df.project.values)
-    obs_df = obs_df[obs_df.project == version]  # only all sky survey
-
-    # get unique image sectors
-    nuv_files, fuv_files = [], []
-    for file in obs_df.dataURL.values:
-        nuv_file = '-'.join(string for string in file.split('-')[:-2]) + '-nd-int.fits.gz'
-        if nuv_file not in nuv_files:
-            nuv_files.append(nuv_file)
-            fuv_file = nuv_file.replace('-nd-', '-fd-')
-            fuv_files.append(fuv_file)
-
-    # download the FITS images
-    nuv_hdu_list, fuv_hdu_list = [], []
-    for nuv_file, fuv_file in zip(nuv_files, fuv_files):
-        try:
-            nuv_hdu = fits.open(nuv_file)
-            nuv_hdu_list.append(nuv_hdu)
-        except:
-            pass
-        try:
-            fuv_hdu = fits.open(fuv_file)
-            fuv_hdu_list.append(fuv_hdu)
-        except:
-            pass
-
-    # calculate the distance of the galaxy to the image center
-    nuv_distances = []
-    for hdu in nuv_hdu_list:
-        header = hdu[0].header
-        dist_from_center = get_img_dist(ra, dec, header)
-        nuv_distances.append(dist_from_center)
-
-    fuv_distances = []
-    for hdu in fuv_hdu_list:
-        header = hdu[0].header
-        dist_from_center = get_img_dist(ra, dec, header)
-        fuv_distances.append(dist_from_center)
-
-    # get the image with the galaxy closest to the center
-    if len(nuv_distances)!=0:
-        id_nuv_file = np.argmin(np.array(nuv_distances))
-        nuv_hdu = nuv_hdu_list[id_nuv_file]
-    else:
-        nuv_hdu = None
+    obs_df_ = obs_table.to_pandas()
 
-    if len(fuv_distances)!=0:
-        id_fuv_file = np.argmin(np.array(fuv_distances))
-        fuv_hdu = fuv_hdu_list[id_fuv_file]
+    if version is None:
+        # starts from the survey with the deepest images first
+        obs_df_ = obs_df_.sort_values("t_exptime", ascending=False)
+        projects = obs_df_.project.unique()
     else:
-        fuv_hdu = None
+        # only use the survey requested by the user
+        projects = [version]
+
+    hdu_dict = {"NUV": None, "FUV": None}
+    for project in projects:
+        obs_df = obs_df_[obs_df_.project == project]
+
+        for filt in filters:
+            if hdu_dict[filt] is not None:
+                # if the image was already found, skip this filter
+                continue
+
+            # get only "intensity" images
+            filt_extension = {
+                "NUV": "-nd-int.fits.gz",
+                "FUV": "-fd-int.fits.gz",
+            }
+            # get unique image sectors
+            files = []
+            for file in obs_df.dataURL.values:
+                sector_info = file.split("-")[:-2]
+                file = (
+                    "-".join(string for string in sector_info)
+                    + filt_extension[filt]
+                )
+                if file not in files:
+                    files.append(file)
+
+            # download the FITS images
+            hdu_list = []
+            for file in files:
+                try:
+                    hdu = fits.open(file)
+                    hdu_list.append(hdu)
+                except:
+                    pass
+
+            # calculate the distance of the galaxy to the image center
+            distances = []
+            for hdu in hdu_list:
+                header = hdu[0].header
+                dist_from_center = get_img_dist(ra, dec, header)
+                distances.append(dist_from_center)
+
+            # get the image with the galaxy closest to the center
+            if len(distances) != 0:
+                id_file = np.argmin(np.array(distances))
+                hdu = hdu_list[id_file]
+            else:
+                hdu = None
+
+            hdu_dict[filt] = hdu
 
-    hdu_dict = {'NUV': nuv_hdu, 'FUV': fuv_hdu}
     hdu_list = []
     for filt in filters:
         hdu = hdu_dict[filt]
         if hdu is None:
             continue  # no image in this filter
         # trim data to requested size
         img_wcs = wcs.WCS(hdu[0].header)
@@ -564,29 +583,27 @@
 
     if isinstance(size, (float, int)):
         size_arcsec = (size * u.arcmin).to(u.arcsec)
     else:
         size_arcsec = size.to(u.arcsec)
 
     pixel_scale = survey_pixel_scale(survey)
-    size_pixels = int(size_arcsec.value / pixel_scale)
+    # size_pixels = int(size_arcsec.value / pixel_scale)
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", AstropyWarning)
         coords = SkyCoord(
             ra=ra, dec=dec, unit=(u.degree, u.degree), frame="icrs"
         )
-
+        # just to get the original image used
         skyview_fits = SkyView.get_images(
             position=coords,
             coordinates="icrs",
-            pixels=str(size_pixels),
+            pixels="100",
             survey="WISE 3.4",
-            #width=size_arcsec,
-            #height=size_arcsec,
         )
         header = skyview_fits[0][0].header
 
         coadd_id = get_used_image(header)
         coadd_id1 = coadd_id[:4]
         coadd_id2 = coadd_id1[:2]
 
@@ -621,30 +638,38 @@
     dec: str or float
         Declination in degrees.
     size: float or ~astropy.units.Quantity, default ``3``
         Image size. If a float is given, the units are assumed to be arcmin.
     filters: str, default ``None``
         Filters to use. If ``None``, uses all WISE filters.
     version: str, default ``allwise``
-        Version of the unWISE images. Either ``allwise``, ``neo1`` or ``neo2``.
+        Version of the unWISE images. Either ``allwise`` or ``neo{i}`` for
+        {i} = 1 to 7.
 
     Return
     ------
     hdu_list: list
         List with fits images for the given filters.
         `None` is returned if no image is found.
     """
     survey = "unWISE"
     if version is None:
-        version = 'allwise'
+        version = "allwise"
+    else:
+        # check validity of the version used
+        neo_versions = [f"neo{i}" for i in range(1, 8)]
+        all_versions = ["allwise"] + neo_versions
+        assert (
+            version in all_versions
+        ), f"Not a valid version ({version}): {all_versions}"
     if filters is None:
         filters = get_survey_filters(survey)
     check_filters_validity(filters, survey)
 
-    if version in ["neo1", "neo2"]:
+    if "neo" in version:
         # these only have W1 and W2 data
         if "W3" in filters:
             filters.remove("W3")
         if "W4" in filters:
             filters.remove("W4")
 
     if isinstance(size, (float, int)):
@@ -737,138 +762,152 @@
         # for more info: https://irsa.ipac.caltech.edu/ibe/docs/twomass/allsky/allsky/#main
         base_url = (
             "https://irsa.ipac.caltech.edu/ibe/data/twomass/allsky/allsky"
         )
 
         hdu_list = []
         for i, filt in enumerate(filters):
-            if filt=='Ks':
-                filt = 'K'
+            if filt == "Ks":
+                filt = "K"
             band_df = twomass_df[twomass_df.band == filt]
             if len(band_df) == 0:
                 # no data for this band:
                 hdu_list.append(None)
                 continue
 
             fname = band_df.download.values[0].split("=")[-1]
             hemisphere = band_df.hem.values[0]
             ordate = band_df.date.values[0]
             scanno = band_df.scan.values[0]
             # add leading zeros for scanno bellow 100
             n_zeros = 3 - len(str(scanno))
-            scanno = n_zeros * '0' + str(scanno)
+            scanno = n_zeros * "0" + str(scanno)
 
             tile_url = os.path.join(f"{ordate}{hemisphere}", f"s{scanno}")
             fits_url = os.path.join("image", f"{fname}.gz")
             params_url = f"center={ra},{dec}&size={size_degree}degree&gzip=0"  # center and size of the image
 
             url = os.path.join(base_url, tile_url, fits_url + "?" + params_url)
             hdu = fits.open(url)
             hdu_list.append(hdu)
 
     return hdu_list
 
-
+'''
 # HST
 # ----------------------------------------
-def get_HST_images(ra, dec, size=3, filters=None):
+def get_HST_images(ra, dec, size=3, filt=None, instrument=None):
     """Downloads a set of HST fits images for a given set
     of coordinates and filters using SkyView.
 
     Parameters
     ----------
     ra: str or float
         Right ascension in degrees.
     dec: str or float
         Declination in degrees.
     size: float or ~astropy.units.Quantity, default ``3``
         Image size. If a float is given, the units are assumed to be arcmin.
-    filters: str, default ``None``
-        Filters to use.
+    filt: str, default ``None``
+        Filter to use.
+    instrument: str, default ``None``
+        Instrument to use.
 
     Return
     ------
     hdu_list: list
-        List with fits images for the given filters.
+        List with fits image for the given filter.
         `None` is returned if no image is found.
     """
-    survey = "HST"
-    if filters is None:
-        filters = get_survey_filters(survey)
-    check_filters_validity(filters, survey)
+    check_HST_inputs(filt, instrument)
 
     if isinstance(size, (float, int)):
-        size_degree = (size * u.arcmin).to(u.degree)
+        size_arcsec = (size * u.arcmin).to(u.arcsec)
     else:
-        size_degree = size.to(u.degree)
-    size_degree = size_degree.value
+        size_arcsec = size.to(u.arcsec)
+    size_arcsec = size_arcsec.value
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", AstropyWarning)
         coords = SkyCoord(
             ra=ra, dec=dec, unit=(u.degree, u.degree), frame="icrs"
         )
 
-    obs_table = Observations.query_criteria(
-        coordinates=coords, radius=size_degree, obs_collection=["HST"]
-    )
+    obs_table = Observations.query_region(coords, radius=size)
+    obs_table = obs_table.filled()  # remove masked rows
     obs_df = obs_table.to_pandas()
 
-    df_list = []
-    for inst in obs_df.instrument_name.unique():
-        inst_df = obs_df[obs_df.instrument_name == inst]
-
-        for filt in inst_df.filters.unique():
-            if not filt.startswith("F") or ";" in filt:
-                continue  # skip these odd filters
-            filt_df = inst_df[inst_df.filters == filt]
-
-            dist = np.sqrt(
-                (filt_df.s_dec.values - dec) ** 2
-                + (filt_df.s_ra.values - ra) ** 2
-            )
-            filt_df = filt_df[
-                dist == dist.min()
-            ]  # take the most centred image
-            filt_df = filt_df[:1]  # take first image
-            df_list.append(filt_df)
-    obs_df = pd.concat(df_list)
+    obs_df = obs_df[
+        (obs_df.obs_collection == "HST") | (obs_df.obs_collection == "HLA")
+    ]
+    obs_df = obs_df[obs_df.dataproduct_type == "image"]
+    obs_df = obs_df[obs_df.t_exptime > 15]  # remove short exposures
+
+    # filter by instrument+filter
+    inst = instrument.split("/")[0]
+    # inst_df = obs_df[obs_df.instrument_name==instrument]
+    inst_df = obs_df[obs_df.instrument_name.str.contains(inst)]
+    filt_df = inst_df[inst_df.filters == filt]
+    # just use one image
+    filt_df = filt_df[filt_df.t_exptime == filt_df.t_exptime.max()]
 
-    # identify products to download
-    data_products = Observations.get_product_list(Table.from_pandas(obs_df))
+    # get data products
+    data_products = Observations.get_product_list(Table.from_pandas(filt_df))
     dp_df = data_products.to_pandas()
-    dp_df = dp_df[dp_df.productType == "SCIENCE"]
+    dp_df = dp_df[dp_df.type == "S"]
+    dp_df = dp_df[dp_df.productSubGroupDescription == "FLT"]  # only images
+    # choose first image
+    single_dp_df = dp_df[dp_df.obs_id == dp_df.obs_id.values[0]]
 
-    df_list = []
-    for filt in obs_df.filters.unique():
-        if filt.lower() in dp_df.dataURI.values:
-            filt_df = dp_df[dp_df.dataURI.contains(filt.lower())]
-        elif filt.upper() in dp_df.dataURI.values:
-            filt_df = dp_df[dp_df.dataURI.contains(filt.upper())]
-        else:
-            continue
+    Observations.download_products(
+        Table.from_pandas(single_dp_df),
+        download_dir=None,
+        cache=False,
+        productType="SCIENCE",
+        extension=["fits"],
+    )
 
-        if "HLA" in filt_df.obs_collection:
-            # choose images from the legacy archive
-            filt_df = filt_df[filt_df.obs_collection == "HLA"]
+    for path, subdirs, files in os.walk("mastDownload"):
+        for file in files:
+            fits_file = os.path.join(path, file)
+
+    hdu = fits.open(fits_file)
+    hdu[0].data = hdu[1].data
+
+    # add zeropoints
+    # https://www.stsci.edu/hst/instrumentation/acs/data-analysis/zeropoints
+    photflam = hdu[0].header["PHOTFLAM"]
+    photplam = hdu[0].header["PHOTFLAM"]
+    hdu[0].header["MAGZP"] = (
+        -2.5 * np.log10(photflam) - 5 * np.log10(photplam) - 2.408
+    )
+    hdu_list = [hdu]
 
-        filt_df = filt_df[:1]  # take first image
-        df_list.append(filt_df)
-    dp_df = pd.concat(df_list)
+    # remove directory created by MAST download
+    shutil.rmtree("mastDownload", ignore_errors=True)
 
-    # download images
-    Observations.download_products(
-        Table.from_pandas(dp_df), productType="SCIENCE", extension="fits"
-    )
+    # HST images can be large so need to be trimmed
+    pixel_scale = survey_pixel_scale('HST')
+    size_pixels = int(size_arcsec / pixel_scale)
+    pos = SkyCoord(ra=ra * u.degree, dec=dec * u.degree)
 
-    # return hdu_list
+    for hdu in hdu_list:
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", AstropyWarning)
+            img_wcs = wcs.WCS(hdu[0].header)
 
+        trimmed_data = Cutout2D(hdu[0].data, pos, size_pixels, img_wcs)
+        hdu[0].data = trimmed_data.data
+        hdu[0].header.update(trimmed_data.wcs.to_header())
+
+    return hdu_list
+'''
 
 # Legacy Survey
-def get_LegacySurvey_images(ra, dec, size=3, filters=None, version='dr10'):
+def get_LegacySurvey_images(ra, dec, size=3, filters=None, version="dr10"):
     """Gets Legacy Survey fits images for the given coordinates and
     filters.
 
     Parameters
     ----------
     ra: float
         Right Ascension in degrees.
@@ -895,15 +934,15 @@
     if isinstance(size, (float, int)):
         size_arcsec = (size * u.arcmin).to(u.arcsec).value
     else:
         size_arcsec = size.to(u.arcsec).value
     size_pixels = int(size_arcsec / pixel_scale)
 
     if version is None:
-        version = 'dr10'  # latest data release
+        version = "dr10"  # latest data release
 
     base_url = "https://www.legacysurvey.org/viewer/fits-cutout?"
     params = f"ra={ra}&dec={dec}&layer=ls-{version}&pixscale={pixel_scale}&bands={filters}&size={size_pixels}"
     url = base_url + params
     master_hdu = fits.open(url)
     header = master_hdu[0].header
 
@@ -911,15 +950,15 @@
     # assuming order grz of the filters
     for i, filt in enumerate(filters):
         data = master_hdu[0].data[i]
         hdu = fits.PrimaryHDU(data=data, header=header)
         hdu_list.append(hdu)
 
     return hdu_list
-
+    
 
 # Spitzer
 def get_Spitzer_images(ra, dec, size=3, filters=None):
     """Gets Spitzer fits images for the given coordinates and
     filters.
 
     Parameters
@@ -1037,15 +1076,15 @@
         filters = get_survey_filters(survey)
     check_filters_validity(filters, survey)
 
     if not isinstance(size, (float, int)):
         size = size.to(u.arcmin).value
 
     if version is None:
-        version = 'VHS'
+        version = "VHS"
     # These are final data releases except for VHS(?):
     # VHSDR5: https://www.eso.org/sci/publications/announcements/sciann17290.html
     # VHSDR6: https://b2find.eudat.eu/dataset/0b10d3a0-1cfe-5e67-8a5c-0949db9d19cb
     # VIDEODR5: https://www.eso.org/sci/publications/announcements/sciann17491.html
     # VIKINGDR4: https://www.eso.org/sci/publications/announcements/sciann17289.html
     database_dict = {
         "VHS": "VHSDR6",
@@ -1132,39 +1171,39 @@
 # ----------------------------------------
 def download_images(
     name,
     ra,
     dec,
     size=3,
     filters=None,
-    overwrite=False,
+    overwrite=True,
     survey="PS1",
     version=None,
 ):
     """Download images for a given object in the given filters of a
     given survey.
 
     The surveys that use the ``version`` parameter are: GALEX (``AIS``, ``MIS``,
-    ``DIS``, ``NGS`` and ``GII``),  unWISE (``allwise``, ``neo1`` and ``neo2``)
-    and VISTA (``VHS``, ``VIDEO`` and ``VIKING``).
+    ``DIS``, ``NGS`` and ``GII``),  unWISE (``allwise`` and ``neo{i}`` for {i}=1-7),
+    VISTA (``VHS``, ``VIDEO`` and ``VIKING``) and SDSS (``dr{i}`` for {i}=12-17).
 
     Parameters
     ----------
     name: str
         Name used for tracking the object in your local
         directory.
     ra: float
         Right ascension in degrees.
     dec: float
         Declination in degrees.
     size: float or ~astropy.units.Quantity, default ``3``
         Image size. If a float is given, the units are assumed to be arcmin.
     filters: str, default ``None``
         Filters for the images.
-    overwrite: bool, default ``False``
+    overwrite: bool, default ``True``
         If ``True``, the images are overwritten if they already
         exist.
     survey: str, default ``PS1``
         Survey used to download the images.
     version: str, default ``None``
         Version used by some surveys including multiple surveys. E.g. ``VHS`` for VISTA.
 
@@ -1173,70 +1212,64 @@
     >>> from hostphot.cutouts import download_images
     >>> name = 'SN2004eo'
     >>> host_ra, host_dec = 308.2092, 9.92755  # coords of host galaxy of SN2004eo
     >>> survey = 'PS1'
     >>> download_images(name, host_ra, host_dec, survey=survey)
     """
     check_survey_validity(survey)
-    check_filters_validity(filters, survey)
-    if filters is None:
-        filters = get_survey_filters(survey)
 
     check_work_dir(workdir)
     obj_dir = os.path.join(workdir, name)
     if not os.path.isdir(obj_dir):
         os.mkdir(obj_dir)
 
     # download fits files
     if survey == "PS1":
         hdu_list = get_PS1_images(ra, dec, size, filters)
     elif survey == "DES":
         hdu_list = get_DES_images(ra, dec, size, filters)
     elif survey == "SDSS":
-        hdu_list = get_SDSS_images(ra, dec, size, filters)
+        hdu_list = get_SDSS_images(ra, dec, size, filters, version)
     elif survey == "GALEX":
         hdu_list = get_GALEX_images(ra, dec, size, filters, version)
     elif survey == "WISE":
         hdu_list = get_WISE_images(ra, dec, size, filters)
     elif survey == "unWISE":
         hdu_list = get_unWISE_images(ra, dec, size, filters, version)
     elif survey == "2MASS":
         hdu_list = get_2MASS_images(ra, dec, size, filters)
+    #elif survey == "HST":
+    #    hdu_list = get_HST_images(ra, dec, size, filters, version)
     elif survey == "LegacySurvey":
         hdu_list = get_LegacySurvey_images(ra, dec, size, filters, version)
     elif survey == "Spitzer":
         hdu_list = get_Spitzer_images(ra, dec, size, filters)
     elif survey == "VISTA":
         hdu_list = get_VISTA_images(ra, dec, size, filters, version)
+    else:
+        raise ValueError(
+            "The given survey is not properly added to HostPhot..."
+        )
+    
+    if filters is None and survey != 'HST':
+        filters = get_survey_filters(survey)
 
     if hdu_list:
-        # NOT WORKING: this corrects any possible shifts between the images
-        # fits_files = match_wcs(fits_files)
-        # fix wcs (some have rotated wcs)
-        """
-        if survey in ["XXX"]:
-            for hdu in hdu_list:
-                fits_file = hdu[0]
-                wcs_out, shape_out = find_optimal_celestial_wcs(
-                    [fits_file], auto_rotate=True
-                )
-                fixed_data, footprint = reproject_exact(
-                    fits_file, wcs_out, shape_out=shape_out
-                )
-                fits_file.header.update(wcs_out.to_header())
-                fits_file.data = fixed_data
-        """
-
         for hdu, filt in zip(hdu_list, filters):
             if hdu is None:
                 continue  # skip missing filter/image
-            outfile = os.path.join(obj_dir, f"{survey}_{filt}.fits")
-            if not os.path.isfile(outfile):
-                hdu.writeto(outfile)
+
+            if survey == "HST":
+                inst = version.replace("/", "-")
+                outfile = os.path.join(
+                    obj_dir, f"{survey}_{inst}-{filters}.fits"
+                )
+            else:
+                outfile = os.path.join(obj_dir, f"{survey}_{filt}.fits")
+
+            if overwrite is True or os.path.isfile(outfile) is False:
+                hdu.writeto(outfile, overwrite=overwrite)
             else:
-                if overwrite:
-                    hdu.writeto(outfile, overwrite=overwrite)
-                else:
-                    continue
+                continue
 
     # remove directory if it ends up empty
-    clean_dir(obj_dir)
+    clean_dir(obj_dir)
```

### Comparing `hostphot-2.4.0/src/hostphot/dust.py` & `hostphot-2.5.0/src/hostphot/dust.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/2MASS/2MASS_H.dat` & `hostphot-2.5.0/src/hostphot/filters/2MASS/2MASS_H.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/2MASS/2MASS_J.dat` & `hostphot-2.5.0/src/hostphot/filters/2MASS/2MASS_J.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/2MASS/2MASS_Ks.dat` & `hostphot-2.5.0/src/hostphot/filters/2MASS/2MASS_Ks.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/AAA_README` & `hostphot-2.5.0/src/hostphot/filters/AAA_README`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/DES/DES_Y.dat` & `hostphot-2.5.0/src/hostphot/filters/DES/DES_Y.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/DES/DES_g.dat` & `hostphot-2.5.0/src/hostphot/filters/DES/DES_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/DES/DES_i.dat` & `hostphot-2.5.0/src/hostphot/filters/DES/DES_i.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/DES/DES_r.dat` & `hostphot-2.5.0/src/hostphot/filters/DES/DES_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/DES/DES_z.dat` & `hostphot-2.5.0/src/hostphot/filters/DES/DES_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/GALEX/GALEX_FUV.dat` & `hostphot-2.5.0/src/hostphot/filters/GALEX/GALEX_FUV.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/GALEX/GALEX_NUV.dat` & `hostphot-2.5.0/src/hostphot/filters/GALEX/GALEX_NUV.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat` & `hostphot-2.5.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/LegacySurvey/BASS_g.dat` & `hostphot-2.5.0/src/hostphot/filters/LegacySurvey/BASS_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/LegacySurvey/BASS_r.dat` & `hostphot-2.5.0/src/hostphot/filters/LegacySurvey/BASS_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/LegacySurvey/DECAM_g.dat` & `hostphot-2.5.0/src/hostphot/filters/LegacySurvey/DECAM_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/LegacySurvey/DECAM_r.dat` & `hostphot-2.5.0/src/hostphot/filters/LegacySurvey/DECAM_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/LegacySurvey/DECAM_z.dat` & `hostphot-2.5.0/src/hostphot/filters/LegacySurvey/DECAM_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/LegacySurvey/MzLS_z.dat` & `hostphot-2.5.0/src/hostphot/filters/LegacySurvey/MzLS_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/LegacySurvey/init_BASS_g.dat` & `hostphot-2.5.0/src/hostphot/filters/LegacySurvey/init_BASS_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/LegacySurvey/init_BASS_r.dat` & `hostphot-2.5.0/src/hostphot/filters/LegacySurvey/init_BASS_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/PS1/PS1_g.dat` & `hostphot-2.5.0/src/hostphot/filters/PS1/PS1_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/PS1/PS1_i.dat` & `hostphot-2.5.0/src/hostphot/filters/PS1/PS1_i.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/PS1/PS1_r.dat` & `hostphot-2.5.0/src/hostphot/filters/PS1/PS1_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/PS1/PS1_y.dat` & `hostphot-2.5.0/src/hostphot/filters/PS1/PS1_y.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/PS1/PS1_z.dat` & `hostphot-2.5.0/src/hostphot/filters/PS1/PS1_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/SDSS/SDSS_g.dat` & `hostphot-2.5.0/src/hostphot/filters/SDSS/SDSS_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/SDSS/SDSS_i.dat` & `hostphot-2.5.0/src/hostphot/filters/SDSS/SDSS_i.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/SDSS/SDSS_r.dat` & `hostphot-2.5.0/src/hostphot/filters/SDSS/SDSS_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/SDSS/SDSS_u.dat` & `hostphot-2.5.0/src/hostphot/filters/SDSS/SDSS_u.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/SDSS/SDSS_z.dat` & `hostphot-2.5.0/src/hostphot/filters/SDSS/SDSS_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat` & `hostphot-2.5.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat` & `hostphot-2.5.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat` & `hostphot-2.5.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat` & `hostphot-2.5.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat` & `hostphot-2.5.0/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/VISTA/VISTA_H.dat` & `hostphot-2.5.0/src/hostphot/filters/VISTA/VISTA_H.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/VISTA/VISTA_J.dat` & `hostphot-2.5.0/src/hostphot/filters/VISTA/VISTA_J.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/VISTA/VISTA_Ks.dat` & `hostphot-2.5.0/src/hostphot/filters/VISTA/VISTA_Ks.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/VISTA/VISTA_Y.dat` & `hostphot-2.5.0/src/hostphot/filters/VISTA/VISTA_Y.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/VISTA/VISTA_Z.dat` & `hostphot-2.5.0/src/hostphot/filters/VISTA/VISTA_Z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/WISE/WISE_W1.dat` & `hostphot-2.5.0/src/hostphot/filters/WISE/WISE_W1.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/WISE/WISE_W2.dat` & `hostphot-2.5.0/src/hostphot/filters/WISE/WISE_W2.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/WISE/WISE_W3.dat` & `hostphot-2.5.0/src/hostphot/filters/WISE/WISE_W3.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/WISE/WISE_W4.dat` & `hostphot-2.5.0/src/hostphot/filters/WISE/WISE_W4.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/filters/config.txt` & `hostphot-2.5.0/src/hostphot/filters/config.txt`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/global_photometry.py` & `hostphot-2.5.0/src/hostphot/global_photometry.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #
 #     https://www.sdss.org/dr12/algorithms/fluxcal/#SDSStoAB
 #     https://data.sdss.org/datamodel/files/BOSS_PHOTOOBJ/frames/RERUN/RUN/CAMCOL/frame.html
 #
 # Some parts of this notebook are based on https://github.com/djones1040/PS1_surface_brightness/blob/master/Surface%20Brightness%20Tutorial.ipynb and codes from Lluís Galbany
 
 import os
+import pickle
 import numpy as np
 import pandas as pd
 
 import sep
 from astropy import wcs
 from astropy.io import fits
 
@@ -26,17 +27,18 @@
 from hostphot.utils import (
     get_survey_filters,
     check_survey_validity,
     check_filters_validity,
     get_image_gain,
     pixel2pixel,
     check_work_dir,
-    magnitude_calc,
+    magnitude_calculation,
     survey_pixel_scale,
-    bkg_surveys
+    adapt_aperture,
+    bkg_surveys,
 )
 from hostphot.objects_detect import extract_objects, plot_detected_objects
 from hostphot.image_cleaning import remove_nan
 from hostphot.dust import calc_extinction
 
 import warnings
 from astropy.utils.exceptions import AstropyWarning
@@ -70,25 +72,31 @@
     flux_err: array
         Kron flux error.
     """
     r_min = 1.75  # minimum diameter = 3.5
 
     if kronrad * np.sqrt(objects["a"] * objects["b"]) < r_min:
         print(f"Warning: using circular photometry")
-        flux, flux_err, flag = sep.sum_circle(
+        flux, flux_err, _ = sep.sum_circle(
             data,
             objects["x"],
             objects["y"],
             r_min,
             err=err,
             subpix=5,
             gain=1.0,
         )
     else:
-        flux, flux_err, flag = sep.sum_ellipse(
+        # theta must be in the range [-pi/2, pi/2] for sep.sum_ellipse()
+        if objects["theta"] > np.pi / 2:
+            objects["theta"] -= np.pi
+        elif objects["theta"] < -np.pi / 2:
+            objects["theta"] += np.pi
+
+        flux, flux_err, _ = sep.sum_ellipse(
             data,
             objects["x"],
             objects["y"],
             objects["a"],
             objects["b"],
             objects["theta"],
             scale * kronrad,
@@ -126,15 +134,15 @@
     opt_kronrad: float
         Optimized Kron radius.
     opt_scale: float
         Optimized scale of the Kron radius.
     """
     # iterate over kron radii
     for r in np.arange(1, 6.05, 0.05)[::-1]:
-        kronrad, krflag = sep.kron_radius(
+        kronrad, _ = sep.kron_radius(
             data,
             objects["x"],
             objects["y"],
             objects["a"],
             objects["b"],
             objects["theta"],
             r,
@@ -164,15 +172,15 @@
             opt_scale = scale
             break
         elif np.isnan(calc_eps):
             opt_scale = scales[-2]
             warnings.warn("Warning: the aperture might not fit in the image!")
             break
 
-    return opt_flux, opt_flux_err, opt_kronrad, opt_scale
+    return opt_flux, opt_flux_err, opt_kronrad[0], opt_scale
 
 
 def extract_kronparams(
     name,
     host_ra,
     host_dec,
     filt,
@@ -180,15 +188,17 @@
     ra=None,
     dec=None,
     bkg_sub=False,
     threshold=10,
     use_mask=True,
     optimize_kronrad=True,
     eps=0.0001,
+    gal_dist_thresh=-1,
     save_plots=True,
+    save_aperture_params=True,
 ):
     """Calculates the aperture parameters for common aperture.
 
     Parameters
     ----------
     name: str
         Name of the object to find the path of the fits file.
@@ -210,30 +220,42 @@
         Threshold used by `sep.extract()` to extract objects.
     use_mask: bool, default `True`
         If `True`, the masked fits files are used. These must have
         been created beforehand.
     optimize_kronrad: bool, default `True`
         If `True`, the Kron radius is optimized, increasing the
         aperture size until the flux does not increase.
-    eps: float, default ``0.0001`` (0.1%)
-        Minimum percent change in flux allowed between iterations
-        when optimizing the Kron radius.
-    save_plots: bool, default `False`
+    eps: float, default ``0.0001``
+        The Kron radius is increased until the change in flux is lower than ``eps``.
+        A value of 0.0001 means 0.01% change in flux.
+    gal_dist_thresh: float, default ``-1``.
+        Distance in arcsec to crossmatch the galaxy coordinates with a detected object,
+        where the object nearest to the galaxy position is considered as the galaxy (within
+        the given threshold). If no objects are found within the given distance threshold,
+        the galaxy is considered as not found and a warning is printed. If a non-positive value
+        is given, the threshold is considered as infinite, i.e. the closest detected object is
+        considered as the galaxy (default option).
+    save_plots: bool, default `True`
         If `True`, the mask and galaxy aperture figures are saved.
+    save_aperture_params: bool, default `True`
+        If `True`, the extracted mask parameters are saved into a pickle file.
 
     Returns
     -------
     gal_obj: array
         Galaxy object.
     img_wcs: WCS
         Image's WCS.
     kronrad: float
         Kron radius.
     scale: float
         Scale for the Kron radius.
+    flip: bool
+        Whether to flip the orientation of the
+        aperture. Only used for DES images.
     """
     check_survey_validity(survey)
     check_work_dir(workdir)
     obj_dir = os.path.join(workdir, name)
     if use_mask:
         suffix = "masked_"
     else:
@@ -250,47 +272,65 @@
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", AstropyWarning)
         img_wcs = wcs.WCS(header, naxis=2)
 
     data = data.astype(np.float64)
     bkg = sep.Background(data)
     bkg_rms = bkg.globalrms
-    if bkg_sub:
+    if (bkg_sub is None and survey in bkg_surveys) or bkg_sub is True:
         data_sub = np.copy(data - bkg)
     else:
         data_sub = np.copy(data)
 
-    pixel_scale = survey_pixel_scale(survey, filt)
-    # extract objects
-    gal_obj, nogal_objs = extract_objects(
-        data_sub, bkg_rms, host_ra, host_dec, threshold, img_wcs, pixel_scale
+    # extract galaxy
+    gal_obj, _ = extract_objects(
+        data_sub,
+        bkg_rms,
+        host_ra,
+        host_dec,
+        threshold,
+        img_wcs,
+        gal_dist_thresh,
     )
     if optimize_kronrad:
         gain = 1  # doesn't matter here
         opt_res = optimize_kron_flux(data_sub, bkg_rms, gain, gal_obj, eps)
-        flux, flux_err, kronrad, scale = opt_res
+        _, _, kronrad, scale = opt_res
     else:
         scale = 2.5
-        kronrad, krflag = sep.kron_radius(
+        kronrad, _ = sep.kron_radius(
             data_sub,
             gal_obj["x"],
             gal_obj["y"],
             gal_obj["a"],
             gal_obj["b"],
             gal_obj["theta"],
             6.0,
         )
 
-    if save_plots:
+    if save_plots is True:
         outfile = os.path.join(obj_dir, f"global_{survey}_{filt}.jpg")
         plot_detected_objects(
             data_sub, gal_obj, scale * kronrad, img_wcs, ra, dec, outfile
         )
 
-    return gal_obj, img_wcs, kronrad, scale
+    if survey == "DES":
+        flip = True
+    else:
+        flip = False
+
+    if save_aperture_params is True:
+        outfile = os.path.join(
+            obj_dir, f"{survey}_{filt}_aperture_parameters.pickle"
+        )
+        with open(outfile, "wb") as fp:
+            aperture_parameters = gal_obj, img_wcs, kronrad, scale, flip
+            pickle.dump(aperture_parameters, fp, protocol=4)
+
+    return gal_obj, img_wcs, kronrad, scale, flip
 
 
 def photometry(
     name,
     host_ra,
     host_dec,
     filt,
@@ -300,14 +340,15 @@
     bkg_sub=None,
     threshold=10,
     use_mask=True,
     correct_extinction=True,
     aperture_params=None,
     optimize_kronrad=True,
     eps=0.0001,
+    gal_dist_thresh=-1,
     save_plots=True,
 ):
     """Calculates the global aperture photometry of a galaxy using
     the Kron flux.
 
     **Note:** the galaxy must be ideally centred in the image.
 
@@ -342,26 +383,37 @@
     aperture_params: tuple, default `None`
         Tuple with objects info and Kron parameters. Used for
         common aperture. If given, the Kron parameters are not
         re-calculated
     optimize_kronrad: bool, default `True`
         If `True`, the Kron radius is optimized, increasing the
         aperture size until the flux does not increase.
-    eps: float, default ``0.0001`` (0.1%)
-        Minimum percent change in flux allowed between iterations
-        when optimizing the Kron radius.
+    eps: float, default ``0.0001``
+        The Kron radius is increased until the change in flux is lower than ``eps``.
+        A value of 0.0001 means 0.01% change in flux.
+    gal_dist_thresh: float, default ``-1``.
+        Distance in arcsec to crossmatch the galaxy coordinates with a detected object,
+        where the object nearest to the galaxy position is considered as the galaxy (within
+        the given threshold). If no objects are found within the given distance threshold,
+        the galaxy is considered as not found and a warning is printed. If a non-positive value
+        is given, the threshold is considered as infinite, i.e. the closest detected object is
+        considered as the galaxy (default option).
     save_plots: bool, default `True`
         If `True`, the mask and galaxy aperture figures are saved.
 
     Returns
     -------
     mag: float
         Aperture magnitude.
     mag_err: float
         Error on the aperture magnitude.
+    flux: float
+        Aperture flux.
+    total_flux_err: float
+        Total flux error on the aperture flux.
     """
     check_survey_validity(survey)
     check_work_dir(workdir)
     obj_dir = os.path.join(workdir, name)
     if use_mask:
         suffix = "masked_"
     else:
@@ -384,39 +436,54 @@
     bkg_rms = bkg.globalrms
     if (bkg_sub is None and survey in bkg_surveys) or bkg_sub is True:
         data_sub = np.copy(data - bkg)
     else:
         data_sub = np.copy(data)
 
     if aperture_params is not None:
-        gal_obj, img_wcs0, kronrad, scale = aperture_params
+        gal_obj, master_img_wcs, kronrad, scale, flip2 = aperture_params
 
-        gal_obj["x"], gal_obj["y"] = pixel2pixel(
-            gal_obj["x"], gal_obj["y"], img_wcs0, img_wcs
-        )
+        if survey == "DES":
+            flip = True
+        else:
+            flip = False
+        if flip == flip2:
+            flip_ = False
+        else:
+            flip_ = True
+
+        a0 = gal_obj["a"]
+        gal_obj = adapt_aperture(gal_obj, master_img_wcs, img_wcs, flip_)
+        # factor used for scaling the Kron radius between different pixel scales
+        conv_factor = gal_obj["a"] / a0
 
         flux, flux_err = kron_flux(
-            data_sub, bkg_rms, gain, gal_obj, kronrad, scale
+            data_sub, bkg_rms, gain, gal_obj, kronrad * conv_factor, scale
         )
         flux, flux_err = flux[0], flux_err[0]
     else:
-        pixel_scale = survey_pixel_scale(survey, filt)
-        # extract objects
-        gal_obj, nogal_objs = extract_objects(
-            data_sub, bkg_rms, host_ra, host_dec, threshold, img_wcs, pixel_scale
+        # extract galaxy
+        gal_obj, _ = extract_objects(
+            data_sub,
+            bkg_rms,
+            host_ra,
+            host_dec,
+            threshold,
+            img_wcs,
+            gal_dist_thresh,
         )
 
         # aperture photometry
         # This uses what would be the default SExtractor parameters.
         # See https://sep.readthedocs.io/en/v1.1.x/apertures.html
         if optimize_kronrad:
             opt_res = optimize_kron_flux(data_sub, bkg_rms, gain, gal_obj, eps)
             flux, flux_err, kronrad, scale = opt_res
         else:
-            kronrad, krflag = sep.kron_radius(
+            kronrad, _ = sep.kron_radius(
                 data_sub,
                 gal_obj["x"],
                 gal_obj["y"],
                 gal_obj["a"],
                 gal_obj["b"],
                 gal_obj["theta"],
                 6.0,
@@ -424,57 +491,59 @@
             scale = 2.5
             flux, flux_err = kron_flux(
                 data_sub, bkg_rms, gain, gal_obj, kronrad, scale
             )
             flux, flux_err = flux[0], flux_err[0]
 
     ap_area = np.pi * gal_obj["a"][0] * gal_obj["b"][0]
-    mag, mag_err = magnitude_calc(
+
+    mag, mag_err, total_flux_err = magnitude_calculation(
         flux,
         flux_err,
         survey,
         filt,
         ap_area,
         header,
         bkg_rms,
     )
 
-    # extinction correction is optional
-    if correct_extinction:
+    if correct_extinction is True:
         A_ext = calc_extinction(filt, survey, host_ra, host_dec)
         mag -= A_ext
 
-    if save_plots:
+    if save_plots is True:
         outfile = os.path.join(obj_dir, f"global_{survey}_{filt}.jpg")
         plot_detected_objects(
             data_sub, gal_obj, scale * kronrad, img_wcs, ra, dec, outfile
         )
 
-    return mag, mag_err
+    return mag, mag_err, flux, total_flux_err
 
 
 def multi_band_phot(
     name,
     host_ra,
     host_dec,
     filters=None,
     survey="PS1",
     ra=None,
     dec=None,
     bkg_sub=None,
     threshold=10,
     use_mask=True,
     correct_extinction=True,
+    aperture_params=None,
     common_aperture=True,
     coadd_filters="riz",
     optimize_kronrad=True,
     eps=0.0001,
+    gal_dist_thresh=-1,
     save_plots=True,
     save_results=True,
-    raise_exception = False,
+    raise_exception=False,
 ):
     """Calculates multi-band aperture photometry of the host galaxy
     for an object.
 
     Parameters
     ----------
     name: str
@@ -499,24 +568,37 @@
     threshold: float, default ``10``
         Threshold used by :func:`sep.extract()` to extract objects.
     use_mask: bool, default ``True``
         If ``True``, the masked fits files are used. These must have
         been created beforehand.
     correct_extinction: bool, default ``True``
         If ``True``, the magnitudes are corrected for extinction.
+    aperture_params: tuple, default `None`
+        Tuple with objects info and Kron parameters. Used for common aperture. If given,
+        the Kron parameters are not re-calculated. If given, this supersedes the use of
+        coadds for common aperture (``common_aperture`` parameter).
     common_aperture: bool, default ``True``
-        If ``True``, use a coadd image for common aperture photometry.
+        If ``True``, use a coadd image for common aperture photometry. This is not used
+        if ``aperture_params`` is given.
     coadd_filters: str, default ``riz``
         Filters of the coadd image. Used for common aperture photometry.
     optimize_kronrad: bool, default ``True``
         If ``True``, the Kron radius is optimized, increasing the
         aperture size until the flux does not increase.
-    eps: float, default ``0.0001`` (0.1%)
-        Minimum percent change in flux allowed between iterations
+    eps: float, default ``0.0001``
+        The Kron radius is increased until the change in flux is lower than ``eps``.
+        A value of 0.0001 means 0.01% change in flux.
         when optimizing the Kron radius.
+    gal_dist_thresh: float, default ``-1``.
+        Distance in arcsec to crossmatch the galaxy coordinates with a detected object,
+        where the object nearest to the galaxy position is considered as the galaxy (within
+        the given threshold). If no objects are found within the given distance threshold,
+        the galaxy is considered as not found and a warning is printed. If a non-positive value
+        is given, the threshold is considered as infinite, i.e. the closest detected object is
+        considered as the galaxy (default option).
     save_plots: bool, default ``True``
         If ``True``, the mask and galaxy aperture figures are saved.
     save_results: bool, default ``True``
         If ``True``, the magnitudes are saved into a csv file.
     raise_exception: bool, default ``False``
         If ``True``, an exception is raised if the photometry fails for any filter.
 
@@ -545,60 +627,64 @@
     results_dict = {
         "name": name,
         "host_ra": host_ra,
         "host_dec": host_dec,
         "survey": survey,
     }
 
-    if common_aperture:
+    if common_aperture is True and aperture_params is None:
         aperture_params = extract_kronparams(
             name,
             host_ra,
             host_dec,
             coadd_filters,
             survey,
-            ra,
-            dec,
-            bkg_sub,
-            threshold,
-            use_mask,
-            optimize_kronrad,
-            eps,
-            save_plots,
+            ra=ra,
+            dec=dec,
+            bkg_sub=bkg_sub,
+            threshold=threshold,
+            use_mask=use_mask,
+            optimize_kronrad=optimize_kronrad,
+            eps=eps,
+            gal_dist_thresh=gal_dist_thresh,
+            save_plots=save_plots,
         )
-    else:
-        aperture_params = None
 
     for filt in filters:
         try:
-            mag, mag_err = photometry(
+            mag, mag_err, flux, flux_err = photometry(
                 name,
                 host_ra,
                 host_dec,
                 filt,
                 survey,
-                ra,
-                dec,
-                bkg_sub,
-                threshold,
-                use_mask,
-                correct_extinction,
-                aperture_params,
-                optimize_kronrad,
-                eps,
-                save_plots,
+                ra=ra,
+                dec=dec,
+                bkg_sub=bkg_sub,
+                threshold=threshold,
+                use_mask=use_mask,
+                correct_extinction=correct_extinction,
+                aperture_params=aperture_params,
+                optimize_kronrad=optimize_kronrad,
+                eps=eps,
+                gal_dist_thresh=gal_dist_thresh,
+                save_plots=save_plots,
             )
             results_dict[filt] = mag
             results_dict[f"{filt}_err"] = mag_err
+            results_dict[f"{filt}_flux"] = flux
+            results_dict[f"{filt}_flux_err"] = flux_err
         except Exception as exc:
             if raise_exception is True:
-                raise Exception(exc)
+                raise Exception(f"{filt}-band: {exc}")
             else:
                 results_dict[filt] = np.nan
                 results_dict[f"{filt}_err"] = np.nan
 
     if save_results is True:
-        outfile = os.path.join(workdir, name, f'{survey}_global.csv')
-        phot_df = pd.DataFrame({key: [val] for key, val in results_dict.items()})
+        outfile = os.path.join(workdir, name, f"{survey}_global.csv")
+        phot_df = pd.DataFrame(
+            {key: [val] for key, val in results_dict.items()}
+        )
         phot_df.to_csv(outfile, index=False)
 
     return results_dict
```

### Comparing `hostphot-2.4.0/src/hostphot/image_cleaning.py` & `hostphot-2.5.0/src/hostphot/image_cleaning.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/image_masking.py` & `hostphot-2.5.0/src/hostphot/image_masking.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import pickle
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.patches import Ellipse
 
 import sep
 from astropy.io import fits
 from astropy import wcs, units as u
@@ -22,15 +23,16 @@
     cross_match,
 )
 from hostphot.utils import (
     check_survey_validity,
     pixel2pixel,
     update_axislabels,
     survey_pixel_scale,
-    bkg_surveys
+    bkg_surveys,
+    adapt_aperture,
 )
 
 import warnings
 from astropy.utils.exceptions import AstropyWarning
 
 
 # ----------------------------------------
@@ -85,17 +87,19 @@
     survey,
     ra=None,
     dec=None,
     bkg_sub=None,
     threshold=15,
     sigma=8,
     crossmatch=False,
+    gal_dist_thresh=-1,
     extract_params=False,
     common_params=None,
     save_plots=True,
+    save_mask_params=True,
 ):
     """Calculates the aperture parameters for common aperture.
 
     Parameters
     ----------
     name: str
         Name of the object to find the path of the fits file.
@@ -119,33 +123,43 @@
         Threshold used by :func:`sep.extract()` to extract objects.
     sigma: float, default ``8``
         Standard deviation in pixel units of the 2D Gaussian kernel
         used to convolve the image.
     crossmatch: bool, default ``False``
         If ``True``, the detected objects are cross-matched with a
         Gaia catalog.
+    gal_dist_thresh: float, default ``-1``.
+        Distance in arcsec to crossmatch the galaxy coordinates with a detected object,
+        where the object nearest to the galaxy position is considered as the galaxy (within
+        the given threshold). If no objects are found within the given distance threshold,
+        the galaxy is considered as not found and a warning is printed. If a non-positive value
+        is given, the threshold is considered as infinite, i.e. the closest detected object is
+        considered as the galaxy (default option).
     extract_params: bool, default ``False``
         If ``True``, returns the parameters listed below.
     common_params: tuple, default ``None``
         Parameters to use for common masking of different filters.
         These are the same as the outputs of this function.
     save_plots: bool, default ``True``
         If ``True``, the mask and galaxy aperture figures are saved.
+    save_mask_params: bool, default `True`
+        If `True`, the extracted mask parameters are saved into a pickle file.
 
     Returns
     -------
     **This are only returned if ``extract_params==True``.**
     gal_obj: array
         Galaxy object.
     nogal_obj: array
         Non-galaxy objects.
     img_wcs: WCS
         Image's WCS.
-    pixel_scale: float
-        Pixel scale for the survey.
+    flip: bool
+        Whether to flip the orientation of the
+        aperture. Only used for DES images.
     """
     check_survey_validity(survey)
     if isinstance(filt, list):
         filt = "".join(f for f in filt)
 
     obj_dir = os.path.join(workdir, name)
     fits_file = os.path.join(obj_dir, f"{survey}_{filt}.fits")
@@ -162,71 +176,98 @@
     bkg = sep.Background(data)
     bkg_rms = bkg.globalrms
     if (bkg_sub is None and survey in bkg_surveys) or bkg_sub is True:
         data_sub = np.copy(data - bkg)
     else:
         data_sub = np.copy(data)
 
-    pixel_scale = survey_pixel_scale(survey, filt)
-
     if common_params is None:
         # extract objects
         gal_obj, nogal_objs = extract_objects(
-            data_sub, bkg_rms, host_ra, host_dec, threshold, img_wcs,
-            pixel_scale
+            data_sub,
+            bkg_rms,
+            host_ra,
+            host_dec,
+            threshold,
+            img_wcs,
+            gal_dist_thresh,
         )
         # preprocessing: cross-match extracted objects with a catalog
         # using two Gaia catalogs as they do not always include the
         # same objects.
         if crossmatch:
             cat_coord1 = find_gaia_objects(host_ra, host_dec)
             cat_coord2 = find_catalog_objects(host_ra, host_dec)
             cat_coord = concatenate([cat_coord1, cat_coord2])
             nogal_objs = cross_match(nogal_objs, img_wcs, cat_coord)
     else:
         # use objects previously extracted
-        # the pixels coordinates are updated accordingly
-        gal_obj, nogal_objs, img_wcs0, pixel_scale0 = common_params
-        scale = pixel_scale0 / pixel_scale
-
-        # make copies to prevent altering the initial values
-        if gal_obj is not None:
-            gal_obj = gal_obj.copy()
-            gal_obj["x"], gal_obj["y"] = pixel2pixel(
-                gal_obj["x"], gal_obj["y"], img_wcs0, img_wcs
-            )
-            gal_obj["a"] *= scale
-            gal_obj["b"] *= scale
+        # the aperture/ellipse parameters are updated accordingly
+        gal_obj, nogal_objs, master_img_wcs, flip2 = common_params
 
-        nogal_objs = nogal_objs.copy()
-        nogal_objs["x"], nogal_objs["y"] = pixel2pixel(
-            nogal_objs["x"], nogal_objs["y"], img_wcs0, img_wcs
-        )
-        nogal_objs["a"] *= scale
-        nogal_objs["b"] *= scale
+        if survey == "DES":
+            flip = True
+        else:
+            flip = False
+        if flip == flip2:
+            flip_ = False
+        else:
+            flip_ = True
+
+        gal_obj = adapt_aperture(gal_obj, master_img_wcs, img_wcs, flip_)
+        nogal_objs = adapt_aperture(nogal_objs, master_img_wcs, img_wcs, flip_)
 
     masked_data = mask_image(data_sub, nogal_objs, sigma=sigma)
     img[0].data = masked_data
     outfile = os.path.join(obj_dir, f"masked_{survey}_{filt}.fits")
     img.writeto(outfile, overwrite=True)
 
     if save_plots:
         outfile = os.path.join(obj_dir, f"masked_{survey}_{filt}.jpg")
         plot_masked_image(
-            data_sub, masked_data, nogal_objs, img_wcs, gal_obj,
-            host_ra, host_dec, ra, dec, outfile
+            data_sub,
+            masked_data,
+            nogal_objs,
+            img_wcs,
+            gal_obj,
+            host_ra,
+            host_dec,
+            ra,
+            dec,
+            outfile,
         )
 
+    if survey == "DES":
+        flip = True
+    else:
+        flip = False
+
+    if save_mask_params is True:
+        outfile = os.path.join(
+            obj_dir, f"{survey}_{filt}_mask_parameters.pickle"
+        )
+        with open(outfile, "wb") as fp:
+            mask_parameters = gal_obj, nogal_objs, img_wcs, flip
+            pickle.dump(mask_parameters, fp, protocol=4)
+
     if extract_params:
-        return gal_obj, nogal_objs, img_wcs, pixel_scale
+        return gal_obj, nogal_objs, img_wcs, flip
 
 
 def plot_masked_image(
-    data, masked_data, objects, img_wcs, gal_obj=None,
-    host_ra=None, host_dec=None, ra=None, dec=None, outfile=None
+    data,
+    masked_data,
+    objects,
+    img_wcs,
+    gal_obj=None,
+    host_ra=None,
+    host_dec=None,
+    ra=None,
+    dec=None,
+    outfile=None,
 ):
     """Plots the masked image together with the original image and
     the detected objects.
 
     Parameters
     ----------
     data: ndarray
@@ -295,16 +336,22 @@
         )
         e.set_facecolor("none")
         e.set_edgecolor("red")
         e.set_linestyle("dotted")
         e.set_linewidth(3)
         ax1.add_artist(e)
 
-        ax1.scatter(gal_obj["x"][0], gal_obj["y"][0], marker="x", s=140, c="r",
-                    label='Identified galaxy center')
+        ax1.scatter(
+            gal_obj["x"][0],
+            gal_obj["y"][0],
+            marker="x",
+            s=140,
+            c="r",
+            label="Identified galaxy center",
+        )
 
     ax2.imshow(
         masked_data,
         interpolation="nearest",
         cmap="gray",
         vmin=m - s,
         vmax=m + s,
@@ -318,29 +365,45 @@
     # plot SN position
     if (host_ra is not None) and (host_dec is not None):
         coord = SkyCoord(
             ra=host_ra, dec=host_dec, unit=(u.degree, u.degree), frame="icrs"
         )
         x, y = img_wcs.world_to_pixel(coord)
         for ax in axes[1:]:
-            ax.scatter(x, y, marker="P", s=140, c="r", edgecolor="gold", label='Galaxy position')
+            ax.scatter(
+                x,
+                y,
+                marker="P",
+                s=140,
+                c="r",
+                edgecolor="gold",
+                label="Galaxy position",
+            )
 
     # plot SN position
     if (ra is not None) and (dec is not None):
         coord = SkyCoord(
             ra=ra, dec=dec, unit=(u.degree, u.degree), frame="icrs"
         )
         x, y = img_wcs.world_to_pixel(coord)
         for ax in axes[1:]:
-            ax.scatter(x, y, marker="*", s=200, c="g", edgecolor="gold", label='SN position')
+            ax.scatter(
+                x,
+                y,
+                marker="*",
+                s=200,
+                c="g",
+                edgecolor="gold",
+                label="SN position",
+            )
 
     axes[1].legend(ncol=2, fontsize=14)
     if outfile:
         basename = os.path.basename(outfile)
         title = os.path.splitext(basename)[0]
-        title = '-'.join(part for part in title.split('_'))
+        title = "-".join(part for part in title.split("_"))
         fig.suptitle(title, fontsize=28)
         plt.tight_layout()
         plt.savefig(outfile, bbox_inches="tight")
         plt.close(fig)
     else:
         plt.show()
```

### Comparing `hostphot-2.4.0/src/hostphot/interactive_aperture.py` & `hostphot-2.5.0/src/hostphot/interactive_aperture.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 from astropy.io import fits
 
 from hostphot._constants import workdir
 from hostphot.utils import (
     get_image_exptime,
     get_image_gain,
     get_image_readnoise,
-    magnitude_calc,
+    magnitude_calculation,
     get_survey_filters,
     check_filters_validity,
-    bkg_surveys
+    bkg_surveys,
 )
 from hostphot.dust import calc_extinction
 
 import warnings
 from astropy.utils.exceptions import AstropyWarning
 
 # ----------------------------------------
@@ -61,22 +61,22 @@
         filters=None,
         masked=True,
         bkg_sub=None,
         correct_extinction=True,
     ):
         self.name = name
         self.survey = survey
-        if not filters:
+        if filters is None:
             self.filters = get_survey_filters(survey)
         else:
             check_filters_validity(filters, survey)
             self.filters = filters
         self.filt = self.filters[0]
 
-        if masked:
+        if masked is True:
             self.masked = "masked_"
         else:
             self.masked = ""
         self.bkg_sub = bkg_sub
 
         self.correct_extinction = correct_extinction
 
@@ -122,15 +122,17 @@
         self.header = img[0].header
         self.data = img[0].data
         self.data = self.data.astype(np.float64)
 
         self.bkg = sep.Background(self.data)
         self.bkg_rms = self.bkg.globalrms
 
-        if (self.bkg_sub is None and self.survey in bkg_surveys) or self.bkg_sub is True:
+        if (
+            self.bkg_sub is None and self.survey in bkg_surveys
+        ) or self.bkg_sub is True:
             self.data = np.copy(self.data - self.bkg)
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", AstropyWarning)
             self.img_wcs = wcs.WCS(self.header, naxis=2)
 
         self.exptime = get_image_exptime(self.header, self.survey)
@@ -300,15 +302,15 @@
         theta = [self.eparams["angle"]["value"] * (np.pi / 180)]  # in radians
 
         coords = self.img_wcs.pixel_to_world(x, y)
         self.ra = coords.ra.value[0]
         self.dec = coords.dec.value[0]
 
         scale = 1  # fixed
-        flux, flux_err, flag = sep.sum_ellipse(
+        flux, flux_err, _ = sep.sum_ellipse(
             self.data,
             x,
             y,
             a,
             b,
             theta,
             scale,
@@ -326,15 +328,15 @@
         flux_err = self.flux_phot[f"{self.filt}_err"]
 
         ap_area = (
             np.pi
             * self.eparams["width"]["value"]
             * self.eparams["height"]["value"]
         )
-        mag, mag_err = magnitude_calc(
+        mag, mag_err, total_flux_error = magnitude_calculation(
             flux,
             flux_err,
             self.survey,
             self.filt,
             ap_area,
             self.header,
             self.bkg_rms,
@@ -363,15 +365,16 @@
             f"Magnitude (${self.filt}$-band): {mag:.5f} +/- {mag_err:.5f}"
         )
 
     # Export Photometry
     def export_photometry(self, outfile=None):
         """Exports the photometry (magnitudes) into a csv file."""
         if not outfile:
-            outfile = f"{self.name}_phot.csv"
+            basename = f"{self.survey}_interactive_photometry.csv"
+            outfile = os.path.join(workdir, self.name, basename)
 
         mag_phot = self.mag_phot.copy()
         for key in mag_phot.keys():
             mag_phot[key] = [mag_phot[key]]
 
         mag_phot["name"] = self.name
         self.phot_df = pd.DataFrame(mag_phot)
```

### Comparing `hostphot-2.4.0/src/hostphot/local_photometry.py` & `hostphot-2.5.0/src/hostphot/local_photometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     check_survey_validity,
     check_filters_validity,
     calc_sky_unc,
     get_image_exptime,
     survey_pixel_scale,
     check_work_dir,
     update_axislabels,
-    magnitude_calc,
-    bkg_surveys
+    magnitude_calculation,
+    bkg_surveys,
 )
 from hostphot.image_cleaning import remove_nan
 from hostphot.dust import calc_extinction
 
 import warnings
 from astropy.utils.exceptions import AstropyWarning
 
@@ -160,15 +160,15 @@
         (px, py), radius_pix, color="r", fill=False, linewidth=1.5
     )
     ax.add_patch(circle)
 
     if outfile:
         basename = os.path.basename(outfile)
         title = os.path.splitext(basename)[0]
-        title = '-'.join(part for part in title.split('_'))
+        title = "-".join(part for part in title.split("_"))
         fig.suptitle(title, fontsize=28)
         plt.tight_layout()
         plt.savefig(outfile, bbox_inches="tight")
         plt.close(fig)
     else:
         plt.show()
 
@@ -220,14 +220,18 @@
 
     Returns
     -------
     mags: list
         Aperture magnitudes for the given aperture radii.
     mags_err: list
         Aperture magnitude errors for the given aperture radii.
+    fluxes: list
+        Aperture flux for the given aperture radii.
+    fluxes_err: list
+        Aperture flux errors for the given aperture radii.
     """
     check_survey_validity(survey)
     check_work_dir(workdir)
     obj_dir = os.path.join(workdir, name)
     if use_mask:
         suffix = "masked_"
     else:
@@ -254,29 +258,30 @@
         data_sub = np.copy(data)
 
     # turn float into a list
     if isinstance(ap_radii, (float, int)):
         ap_radii = [ap_radii]
 
     mags, mags_err = [], []
+    fluxes, fluxes_err = [], []
     px, py = img_wcs.wcs_world2pix(ra, dec, 1)
     pixel_scale = survey_pixel_scale(survey, filt)
     error = calc_sky_unc(data_sub, exptime)
 
     for ap_radius in ap_radii:
         # aperture photometry
         radius_arcsec = calc_aperture_size(z, ap_radius)
         radius_pix = radius_arcsec / pixel_scale
 
         flux, flux_err = extract_aperture_flux(
             data_sub, error, px, py, radius_pix
         )
 
         ap_area = 2 * np.pi * (radius_pix**2)
-        mag, mag_err = magnitude_calc(
+        mag, mag_err, total_flux_error = magnitude_calculation(
             flux,
             flux_err,
             survey,
             filt,
             ap_area,
             header,
             bkg_rms,
@@ -285,22 +290,24 @@
         # extinction correction is optional
         if correct_extinction:
             A_ext = calc_extinction(filt, survey, ra, dec)
             mag -= A_ext
 
         mags.append(mag)
         mags_err.append(mag_err)
+        fluxes.append(flux)
+        fluxes_err.append(total_flux_error)
 
         if save_plots:
             outfile = os.path.join(
                 obj_dir, f"local_{survey}_{filt}_{ap_radius}kpc.jpg"
             )
             plot_aperture(data_sub, px, py, radius_pix, img_wcs, outfile)
 
-    return mags, mags_err
+    return mags, mags_err, fluxes, fluxes_err
 
 
 def multi_band_phot(
     name,
     ra,
     dec,
     z,
@@ -377,43 +384,51 @@
     if isinstance(ap_radii, (float, int)):
         ap_radii = [ap_radii]
 
     results_dict = {
         "name": name,
         "ra": ra,
         "dec": dec,
-        "zspec": z,
+        "redshift": z,
         "survey": survey,
     }
 
     for filt in filters:
         try:
-            mags, mags_err = photometry(
+            mags, mags_err, fluxes, fluxes_err = photometry(
                 name,
                 ra,
                 dec,
                 z,
                 filt,
                 survey,
                 ap_radii,
                 bkg_sub,
                 use_mask,
                 correct_extinction,
                 save_plots,
             )
-            for radius, mag, mag_err in zip(ap_radii, mags, mags_err):
-                results_dict[f"{filt}{radius}"] = mag
-                results_dict[f"{filt}{radius}_err"] = mag_err
+            for radius, mag, mag_err, flux, flux_err in zip(
+                ap_radii, mags, mags_err, fluxes, fluxes_err
+            ):
+                results_dict[f"{filt}_{radius}"] = mag
+                results_dict[f"{filt}_{radius}_err"] = mag_err
+                results_dict[f"{filt}_{radius}_flux"] = flux
+                results_dict[f"{filt}_{radius}_flux_err"] = flux_err
         except Exception as exc:
             if raise_exception is True:
                 raise Exception(exc)
             else:
                 for radius in ap_radii:
                     results_dict[f"{filt}_{radius}"] = np.nan
                     results_dict[f"{filt}_{radius}_err"] = np.nan
+                    results_dict[f"{filt}_{radius}_flux"] = np.nan
+                    results_dict[f"{filt}_{radius}_flux_err"] = np.nan
 
     if save_results is True:
-        outfile = os.path.join(workdir, name, f'{survey}_local.csv')
-        phot_df = pd.DataFrame({key: [val] for key, val in results_dict.items()})
+        outfile = os.path.join(workdir, name, f"{survey}_local.csv")
+        phot_df = pd.DataFrame(
+            {key: [val] for key, val in results_dict.items()}
+        )
         phot_df.to_csv(outfile, index=False)
 
     return results_dict
```

### Comparing `hostphot-2.4.0/src/hostphot/objects_detect.py` & `hostphot-2.5.0/src/hostphot/objects_detect.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from astroquery.mast import Catalogs
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 
 from hostphot.utils import update_axislabels
 
 
-def extract_objects(data, err, host_ra, host_dec, threshold, img_wcs, pixel_scale, dist_thresh=5.0):
+def extract_objects(
+    data, err, host_ra, host_dec, threshold, img_wcs, dist_thresh=-1
+):
     """Extracts objects and their ellipse parameters. The function :func:`sep.extract()`
     is used.
 
     If there is no detected object within a distance of ``dist_thresh`` from the galaxy
     coordinates, it means that the galaxy was not correctly identified.
 
     Parameters
@@ -32,47 +34,51 @@
     threshold: float
         Source with flux above ``threshold*bkg_rms`` are extracted.
         See :func:`sep.extract()` for more information.
     img_wcs: WCS
         Image's WCS.
     pixel_scale: float
         Pixel scale, in units of arcsec/pixel, used to convert from pixel units
-         to arcseconds.
-    dist_thresh: float, default ``5.0``.
-        Distance in arcsec to crossmatch the galaxy coordinates with
-        an object.
+        to arcseconds.
+    dist_thresh: float, default ``-1``.
+        Distance in arcsec to crossmatch the galaxy coordinates with a detected object,
+        where the object nearest to the galaxy position is considered as the galaxy (within
+        the given threshold). If no objects are found within the given distance threshold,
+        the galaxy is considered as not found and a warning is printed. If a non-positive value
+        is given, the threshold is considered as infinite, i.e. the closest detected object is
+        considered as the galaxy (default option).
 
     Returns
     -------
     gal_obj: numpy array
         Galaxy object extracted.
     nogal_objs: numpy array
         All objects extracted except for the galaxy.
     """
     # extract objects with Source Extractor
     objects = sep.extract(data, threshold, err=err)
 
-    gal_coords = SkyCoord(
-        ra=host_ra * u.degree, dec=host_dec * u.degree, frame="icrs"
-    )
-    gal_x, gal_y = img_wcs.world_to_pixel(gal_coords)
+    objs_coords = img_wcs.pixel_to_world(objects["x"], objects["y"])
+    objs_ra, objs_dec = objs_coords.ra.value, objs_coords.dec.value
+    dist = np.sqrt(
+        (objs_ra - host_ra) ** 2 * (np.cos(host_dec * np.pi / 180) ** 2)
+        + (objs_dec - host_dec) ** 2
+    )  # in degrees
+    dist_arcsec = dist * 3600
 
-    # find the galaxy
-    x_diff = np.abs(objects["x"] - gal_x)
-    y_diff = np.abs(objects["y"] - gal_y)
-    dist = np.sqrt(x_diff**2 + y_diff**2)
-    dist_arcsec = dist*pixel_scale
+    if dist_thresh <= 0.0:
+        dist_thresh = np.inf
 
     if any(dist_arcsec <= dist_thresh):
-        gal_id = np.argmin(dist)
-        gal_obj = objects[gal_id: gal_id + 1]
+        gal_id = np.argmin(dist_arcsec)
+        gal_obj = objects[gal_id : gal_id + 1]
     else:
         gal_obj = None
         gal_id = -99
-        print('WARNING: the galaxy was no detected')
+        print("WARNING: the galaxy was no detected")
 
     objs_id = [i for i in range(len(objects)) if i != gal_id]
     nogal_objs = objects.take(objs_id)
 
     return gal_obj, nogal_objs
 
 
@@ -248,14 +254,14 @@
         )
         px, py = img_wcs.world_to_pixel(coord)
         ax.scatter(px, py, marker="*", s=200, c="g", edgecolor="gold")
 
     if outfile:
         basename = os.path.basename(outfile)
         title = os.path.splitext(basename)[0]
-        title = '-'.join(part for part in title.split('_'))
+        title = "-".join(part for part in title.split("_"))
         fig.suptitle(title, fontsize=28)
         plt.tight_layout()
         plt.savefig(outfile, bbox_inches="tight")
         plt.close(fig)
     else:
         plt.show()
```

### Comparing `hostphot-2.4.0/src/hostphot/rgb_images.py` & `hostphot-2.5.0/src/hostphot/rgb_images.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/src/hostphot/utils.py` & `hostphot-2.5.0/src/hostphot/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 
 from astropy import wcs
 from astropy.io import fits
 from astropy.stats import sigma_clipped_stats
 from photutils.utils import calc_total_error
+from photutils.aperture import EllipticalAperture
 
 import warnings
 from astropy.utils.exceptions import AstropyWarning
 
 import hostphot
 
 hostphot_path = hostphot.__path__[0]
 config_file = os.path.join(hostphot_path, "filters", "config.txt")
 config_df = pd.read_csv(config_file, delim_whitespace=True)
 
 # surveys that need background subtraction
-bkg_surveys = ['2MASS', 'WISE', 'VISTA']
+bkg_surveys = ["2MASS", "WISE", "VISTA"]
+
 
 def calc_sky_unc(image, exptime):
     """Calculates the uncertainty of the image from the
     sky standard deviation, sigma-clipped STD.
 
     Parameters
     ----------
@@ -116,14 +118,20 @@
 
     if zps == "header":
         return zps
 
     if "," in zps:
         zps = zps.split(",")
         zp_dict = {filt: float(zp) for filt, zp in zip(filters, zps)}
+    elif survey == "SDSS":
+        # SDSS zero-points are not exactly in AB:
+        # https://www.sdss4.org/dr12/algorithms/fluxcal/#SDSStoAB
+        zp_dict = {filt: float(zps) for filt in filters}
+        zp_dict["u"] -= 0.04
+        zp_dict["z"] += 0.02
     else:
         zp_dict = {filt: float(zps) for filt in filters}
 
     return zp_dict
 
 
 def get_image_gain(header, survey):
@@ -261,15 +269,15 @@
         exptime = 900.0  # assumed similar to DES
     else:
         exptime = 1.0
 
     return exptime
 
 
-def magnitude_calc(
+def magnitude_calculation(
     flux,
     flux_err,
     survey,
     filt=None,
     ap_area=0.0,
     header=None,
     bkg_rms=0.0,
@@ -293,14 +301,16 @@
 
     Returns
     -------
     mag: float
         Apparent magnitude.
     mag_err: float
         Apparent magnitude uncertainty.
+    total_flux_error: float
+        Total uncertainty in flux units.
     """
     zp_dict = survey_zp(survey)
     if zp_dict == "header":
         zp = header["MAGZP"]
     else:
         zp = zp_dict[filt]
 
@@ -308,37 +318,39 @@
         exptime = get_image_exptime(header, survey)
         zp += 2.5 * np.log10(exptime)
 
     mag = -2.5 * np.log10(flux) + zp
     mag_err = 2.5 / np.log(10) * flux_err / flux
 
     # error propagation
-    extra_err = uncertainty_calc(
+    extra_err, total_flux_error = uncertainty_calculation(
         flux,
         flux_err,
         survey,
         filt,
         ap_area,
         header,
         bkg_rms,
     )
     mag_err = np.sqrt(mag_err**2 + extra_err**2)
 
-    return mag, mag_err
+    return mag, mag_err, total_flux_error
 
 
-def uncertainty_calc(
+def uncertainty_calculation(
     flux, flux_err, survey, filt=None, ap_area=0.0, header=None, bkg_rms=0.0
 ):
     """Calculates the uncertainty propagation.
 
     Parameters
     ----------
     flux: float
         Aperture flux.
+    flux_err: float
+        Aperture flux error.
     survey: str
         Survey name. E.g. ``PS1``, ``DES``, ``SDSS``, ``GALEX``, ``WISE``, etc.
     filt: str, default ``None``
         Survey-specific filter.
     ap_area: float, default ``0.0``
         Aperture area.
     header: fits header, default ``None``
@@ -346,45 +358,77 @@
     bkg_rms: float, default ``0.0``
         Background noise.
 
     Returns
     -------
     mag_err: float
         Extra uncertainty in magnitudes.
+    total_flux_err: float
+        Total uncertainty in flux units.
     """
     exptime = get_image_exptime(header, survey)
     gain = get_image_gain(header, survey)
     readnoise = get_image_readnoise(header, survey)
 
     mag_err = 0.0
+    total_flux_err = np.copy(flux_err)
     if survey in ["PS1", "DES", "LegacySurvey", "Spitzer", "VISTA"]:
         if survey == "Spitzer":
             flux /= header["EFCONV"]  # conv. factor (MJy/sr)/(DN/s)
         # 1.0857 = 2.5/ln(10)
         extra_err = (
             1.0857 * np.sqrt(ap_area * (readnoise**2) + flux / gain) / flux
         )
         mag_err = np.sqrt(mag_err**2 + extra_err**2)
 
+        extra_flux_err = np.sqrt(ap_area * (readnoise**2) + flux / gain)
+        total_flux_err = np.sqrt(total_flux_err**2 + extra_flux_err**2)
+
     if survey == "DES":
-        # see https://des.ncsa.illinois.edu/releases/dr1/dr1-docs/quality
-        # Photometry section
+        # see the photometry section in https://des.ncsa.illinois.edu/releases/dr1/dr1-docs/quality
+        # statistical uncertainties on the AB magnitud system zeropoints
         unc_dict = {
             "g": 2.6e-3,
             "r": 2.9e-3,
             "i": 3.4e-3,
             "z": 2.5e-3,
             "Y": 4.5e-3,
         }
         extra_err = unc_dict[filt]
         mag_err = np.sqrt(mag_err**2 + extra_err**2)
 
+        # median coadd zeropoint statistical uncertainty
+        unc_dict = {
+            "g": 5e-3,
+            "r": 4e-3,
+            "i": 5e-3,
+            "z": 6e-3,
+            "Y": 5e-3,
+        }
+        extra_err = unc_dict[filt]
+        mag_err = np.sqrt(mag_err**2 + extra_err**2)
+
+        extra_flux_err = np.abs(flux * 0.4 * np.log(10) * extra_err)
+        total_flux_err = np.sqrt(total_flux_err**2 + extra_flux_err**2)
+
     elif survey == "PS1":
-        # just as a check to make sure all surveys are included
-        pass
+        # add floor systematic error from:
+        # https://iopscience.iop.org/article/10.3847/1538-4365/abb82a/pdf
+        unc_dict = {
+            "g": 14e-3,
+            "r": 14e-3,
+            "i": 15e-3,
+            "z": 15e-3,
+            "y": 18e-3,
+        }
+        floor_err = unc_dict[filt]
+        mag_err = np.sqrt(mag_err**2 + floor_err**2)
+
+        extra_flux_err = np.abs(flux * 0.4 * np.log(10) * floor_err)
+        total_flux_err = np.sqrt(total_flux_err**2 + extra_flux_err**2)
 
     elif survey == "SDSS":
         # https://data.sdss.org/datamodel/files/BOSS_PHOTOOBJ/frames/RERUN/RUN/CAMCOL/frame.html
         camcol = header["CAMCOL"]
         run = header["RUN"]
 
         gain_dict = {
@@ -437,54 +481,70 @@
             if camcol == 4:
                 dark_variance = 12.6025
             if camcol == 5:
                 dark_variance = 2.1025
 
         extra_err = 1.0857 * np.sqrt(dark_variance + flux / gain) / flux
         mag_err = np.sqrt(mag_err**2 + extra_err**2)
-        mag_err = np.sqrt(mag_err**2 + extra_err**2)
+
+        extra_flux_err = np.sqrt(dark_variance + flux / gain)
+        total_flux_err = np.sqrt(total_flux_err**2 + extra_flux_err**2)
 
     elif survey == "GALEX":
+        # https://asd.gsfc.nasa.gov/archive/galex/FAQ/counts_background.html
         CPS = flux
         if filt == "FUV":
             uv_err = -2.5 * (
                 np.log10(CPS)
                 - np.log10(
                     CPS
                     + (CPS * exptime + (0.050 * CPS * exptime) ** 2) ** 0.5
                     / exptime
                 )
             )
+            flux_uv_err = (
+                np.sqrt(CPS * exptime + (0.050 * CPS * exptime) ** 2) / exptime
+            )
         elif filt == "NUV":
             uv_err = -2.5 * (
                 np.log10(CPS)
                 - np.log10(
                     CPS
                     + (CPS * exptime + (0.027 * CPS * exptime) ** 2) ** 0.5
                     / exptime
                 )
             )
+            flux_uv_err = (
+                np.sqrt(CPS * exptime + (0.027 * CPS * exptime) ** 2) / exptime
+            )
+
         mag_err = np.sqrt(mag_err**2 + uv_err**2)
 
+        total_flux_err = np.sqrt(total_flux_err**2 + flux_uv_err**2)
+
     elif survey == "2MASS":
         # see: https://wise2.ipac.caltech.edu/staff/jarrett/2mass/3chan/noise/
         S = flux
         N_c = 6  # number of coadd pixels
         k_z = 1.7  # kernel smoothing factor
         n_f = ap_area  # number of frame pixels in the aperture; aprox. as aperture area
         n_c = 4 * n_f  # number of coadd pixels in the aperture
         sigma_c = bkg_rms  # coadd noise; assumed to be ~background noise
 
         SNR = S / np.sqrt(
             S / (gain * N_c)
             + n_c * (2 * k_z * sigma_c) ** 2
             + (n_c * 0.024 * sigma_c) ** 2
         )
+
         mag_err = 1.0857 / SNR
 
+        extra_flux_err = flux / SNR
+        total_flux_err = np.sqrt(total_flux_err**2 + extra_flux_err**2)
+
     elif "WISE" in survey:
         # see: https://wise2.ipac.caltech.edu/docs/release/allsky/expsup/sec2_3f.html
         # see Table 5 of
         # https://wise2.ipac.caltech.edu/docs/release/allsky/expsup/sec4_4c.html#wpro
         # correction assumed to be 0 mags as PSF fitting is not used.
         m_apcor = 0.0
         f_apcor = 10 ** (-0.4 * m_apcor)
@@ -506,41 +566,50 @@
             * F_corr
             * (flux_err**2 + k * (N_A**2) / N_B * bkg_rms**2)
             + sigma_conf**2
         )
 
         mag_err = np.sqrt(1.179 * sigma_src**2 / F_src**2)
 
+        total_flux_err = f_apcor**2
+
         # add uncertainty from the ZP
-        if survey=="unWISE":
+        if survey == "unWISE":
             # These values are the same for all Atlas Images of a given band...
             # see: https://wise2.ipac.caltech.edu/docs/release/allsky/expsup/sec2_3f.html
-            unc_dict = {'W1':0.006, 'W2':0.007, 'W3':0.012, 'W4':0.012}
+            unc_dict = {"W1": 0.006, "W2": 0.007, "W3": 0.012, "W4": 0.012}
             zp_unc = unc_dict[filt]
-        elif survey=="WISE":
+        elif survey == "WISE":
             zp_unc = header["MAGZPUNC"]
+
         mag_err = np.sqrt(mag_err**2 + zp_unc**2)
 
+        extra_flux_err = np.abs(flux * 0.4 * np.log(10) * zp_unc)
+        total_flux_err = np.sqrt(total_flux_err**2 + extra_flux_err**2)
+
     elif survey == "LegacySurvey":
         # already added at the beginning
         pass
     elif survey == "Spitzer":
         # already added at the beginning
         pass
     elif survey == "VISTA":
         # add uncertainty from the ZP
         zp_unc = header["MAGZRR"]
         mag_err = np.sqrt(mag_err**2 + zp_unc**2)
 
+        extra_flux_err = np.abs(flux * 0.4 * np.log(10) * zp_unc)
+        total_flux_err = np.sqrt(total_flux_err**2 + extra_flux_err**2)
+
     else:
         raise Exception(
             f"Survey {survey} has not been added for error propagation."
         )
 
-    return mag_err
+    return mag_err, total_flux_err
 
 
 def survey_pixel_scale(survey, filt=None):
     """Returns the pixel scale for a given survey.
 
     Parameters
     ----------
@@ -582,30 +651,58 @@
 
 def check_filters_validity(filters, survey):
     """Check whether the given filters are whithin the valid
     options for the given survey.
 
     Parameters
     ----------
-    filters: str
+    filters: str or list
         Filters to use, e,g, ``griz``.
     survey: str
-        Survey name: ``PS1``, ``DES``, ``SDSS``, ``GALEX``, ``WISE``, ``2MASS``.
+        Survey name, e.g. ``PS1``, ``DES`` and ``GALEX``.
     """
     if filters is not None:
         valid_filters = get_survey_filters(survey)
 
         for filt in filters:
             message = (
                 f"filter '{filt}' is not a valid option for "
                 f"'{survey}' survey ({valid_filters})"
             )
             assert filt in valid_filters, message
 
 
+def check_HST_inputs(filt, instrument):
+    """Check whether the given filter and instrument are whithin the valid
+    options for HST.
+
+    Parameters
+    ----------
+    filt: str
+        Filter to use, e,g, ``F225W``.
+    instrument: str
+        Instrument name, e.g. ``WFC3/UVIS1``.
+    """
+    hst_file = os.path.join(hostphot_path, "filters/HST", "HST_filters.txt")
+    valid_instruments, valid_filters = np.loadtxt(hst_file, dtype=str).T
+
+    assert (
+        instrument in valid_instruments
+    ), f"Not a valid HST instrument ({instrument}): {valid_instruments}"
+    assert (
+        filt in valid_filters
+    ), f"Not a valid HST filter ({filt}): {valid_filters}"
+
+    indexes_inst = [i for i, f in enumerate(valid_filters) if f == filt]
+    matched_instruments = valid_instruments[indexes_inst]
+    assert (
+        instrument in matched_instruments
+    ), f"Not a valid HST instrument-filter combination -> {instrument}-{filt}"
+
+
 def extract_filters(filters, survey, version=None):
     """Extracts transmission functions.
 
     Parameters
     ----------
     filters: str
         Filters to extract.
@@ -704,14 +801,61 @@
     )
     int2 = np.trapz(filter_response * filter_wave, filter_wave)
     flux_filter = int1 / int2
 
     return flux_filter
 
 
+def adapt_aperture(objects, img_wcs, img_wcs2, flip=False):
+    """Changes the aperture parameters to consider differences
+    in WCS between surveys.
+
+    The values of ``center``, ``a`` and ``b`` should in pixel
+    units. DES images are flipped, so these need to be corrected
+    with ``theta -> -theta``, i.e. using ``flip=True``.
+
+    Parameters
+    ----------
+    objects: ndarray
+        Objects with apertures.
+    img_wcs: ~wcs.WCS
+        WCS of the image from where the objects were extracted.
+    img_wcs2: ~wcs.WCS
+        WCS used to adapt the apertures.
+    flip: bool, default ``False``
+        Whether to flip the orientation of the aperture. Only
+        used for DES images.
+
+    Returns
+    -------
+    objects_: ndarray
+        Objects with adapted apertures.
+    """
+    objects_ = objects.copy()  # avoid modifying the intial objects
+    for obj in objects_:
+        center = (obj["x"], obj["y"])
+        apertures = EllipticalAperture(
+            center, obj["a"], obj["b"], obj["theta"]
+        )
+        sky_apertures = apertures.to_sky(img_wcs)
+
+        new_apertures = sky_apertures.to_pixel(img_wcs2)
+        new_center = new_apertures.positions
+        obj["x"], obj["y"] = new_center
+        obj["a"] = new_apertures.a
+        obj["b"] = new_apertures.b
+        obj["theta"] = new_apertures.theta
+
+        if flip is True:
+            # flip aperture orientation
+            obj["theta"] *= -1
+
+    return objects_
+
+
 def check_work_dir(wokrdir):
     """Checks if the working directory exists. If it
     does not, one is created.
 
     Parameters
     ----------
     wokrdir: str
@@ -731,34 +875,42 @@
     """
     try:
         os.rmdir(directory)
     except:
         pass
 
 
-def plot_fits(fits_file):
+def plot_fits(fits_file, ext=0):
     """Plots a fits file.
 
     Parameters
     ----------
-    fits_file: str
+    fits_file: str or HDU.
         Path to fits file.
+    ext: int
+        Extension index.
     """
-    img = fits.open(fits_file)
-    header = img[0].header
-    data = img[0].data
+    if isinstance(fits_file, str):
+        hdu = fits.open(fits_file)
+        title = os.path.splitext(os.path.basename(fits_file))[0]
+    else:
+        hdu = fits_file
+        title = None
+    header = hdu[ext].header
+    data = hdu[ext].data
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", AstropyWarning)
         img_wcs = wcs.WCS(header, naxis=2)
 
     m, s = np.nanmean(data), np.nanstd(data)
 
     fig = plt.figure(figsize=(10, 10))
     ax = plt.subplot(projection=img_wcs)
+    ax.set_title(title, fontsize=18)
     update_axislabels(ax)
 
     im = ax.imshow(
         data,
         interpolation="nearest",
         cmap="gray",
         vmin=m - s,
```

### Comparing `hostphot-2.4.0/src/hostphot.egg-info/PKG-INFO` & `hostphot-2.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: hostphot
-Version: 2.4.0
-Summary: Global and local photometry of galaxies hosting supernovae or other transients
-Home-page: https://github.com/temuller/hostphot
-Author: Tomás Enrique Müller-Bravo and Lluís Galbany
-Author-email: t.e.muller-bravo@ice.csic.es
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8, <3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
 	<img src="docs/hostphot_logo.png" alt="drawing" width="300"/>
 </p>
 
 Global and local photometry of galaxies hosting supernovae or other transients
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fhostphot-blue.svg?style=flat)](https://github.com/temuller/hostphot)
@@ -192,14 +177,32 @@
   number = {76}, 
   pages = {4508},  
   journal = {Journal of Open Source Software} 
 } 
 ```
 
 ## What's new!
+v2.5.0:
+* Systematic error floor added to PS1 photometry
+* Added missing uncertainties in the error budget of DES (~5 mmag) 
+* Flux/counts have been added to output photometry
+* GALEX now downloads images with largest exposure time by default
+* Fixed image realignment/orientation between different surveys when using common apertures (for masking and global photometry)
+* Added option to output mask parameters, and also aperture parameters for global photometry
+* Option added to set a distant threshold to identify the host galaxy in the image (by default use the nearest object)
+* Slight change in the column names of the local photometry output file
+* Offsets in SDSS zeropoints to place it in the AB system
+* overwrite set to True by default when downloading image cutouts
+* Other minor bugs fixed
+
+v2.4.0:
+* Fixed and improved GALEX cutouts
+* Better galaxy identification
+* Better output plots for masked images
+* Option to return NaN or raise an exception when getting photometry
 
 v2.3.2:
 * Improved download of GALEX images (download even if they seem to be just background noise)
 
 
 ## Acknowledgements
```

### Comparing `hostphot-2.4.0/src/hostphot.egg-info/SOURCES.txt` & `hostphot-2.5.0/src/hostphot.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 src/hostphot/filters/DES/DES_g.dat
 src/hostphot/filters/DES/DES_i.dat
 src/hostphot/filters/DES/DES_r.dat
 src/hostphot/filters/DES/DES_z.dat
 src/hostphot/filters/GALEX/AAA_README
 src/hostphot/filters/GALEX/GALEX_FUV.dat
 src/hostphot/filters/GALEX/GALEX_NUV.dat
+src/hostphot/filters/HST/HST_filters.txt
 src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat
 src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat
 src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat
 src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat
 src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat
 src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat
 src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat
```

### Comparing `hostphot-2.4.0/tests/test_cutouts.py` & `hostphot-2.5.0/tests/test_cutouts.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,20 +36,24 @@
             self.sn_name, self.ra, self.dec, overwrite=True, survey="WISE"
         )
 
     def test_cutouts_2MASS(self):
         download_images(
             self.sn_name, self.ra, self.dec, overwrite=True, survey="2MASS"
         )
-    
+
     def test_cutouts_unWISE(self):
         for version in ["neo1", "neo2", "allwise"]:
             download_images(
-                self.sn_name, self.ra, self.dec, overwrite=True, survey="unWISE",
-                version=version
+                self.sn_name,
+                self.ra,
+                self.dec,
+                overwrite=True,
+                survey="unWISE",
+                version=version,
             )
 
     def test_cutouts_LegacySurvey(self):
         download_images(
             self.sn_name,
             self.ra,
             self.dec,
@@ -61,26 +65,34 @@
         name = "Spitzer_test"
         ra, dec = 52.158591, -27.891113
         download_images(name, ra, dec, overwrite=True, survey="Spitzer")
 
     def test_cutouts_VISTA(self):
         name = "VISTA_test"
         # use different coordinates for each survey as they don't overlap
-        surveys = {"VHS": [120, -60],
-                   "VIDEO": [36.1, -5],
-                   "VIKING": [220.5, 0.0]}
+        surveys = {
+            "VHS": [120, -60],
+            "VIDEO": [36.1, -5],
+            "VIKING": [220.5, 0.0],
+        }
 
         try:
             for version, coords in surveys.items():
                 ra, dec = coords
                 download_images(
-                    name, ra, dec,
-                    overwrite=True, survey="VISTA",
-                    version=version
+                    name,
+                    ra,
+                    dec,
+                    overwrite=True,
+                    survey="VISTA",
+                    version=version,
                 )
         except Exception as exc:
-            warnings.warn("The VISTA SCIENCE ARCHIVE might be having issues...")
-            print('Skipping this test...')
+            warnings.warn(
+                "The VISTA SCIENCE ARCHIVE might be having issues..."
+            )
+            print("Skipping this test...")
             print(exc)
 
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `hostphot-2.4.0/tests/test_global_phot.py` & `hostphot-2.5.0/tests/test_global_phot.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/tests/test_local_phot.py` & `hostphot-2.5.0/tests/test_local_phot.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             z,
             survey="PS1",
             filters="grizy",
             ap_radii=ap_radii,
             use_mask=False,
             save_plots=True,
         )
-        mags = [phot[filt] for filt in ["g4", "r4", "i4", "z4"]]
+        mags = [phot[filt] for filt in ["g_4", "r_4", "i_4", "z_4"]]
         # pre-calculated magnitudes
         ref_mags = [12.26, 11.89, 11.72, 11.57]
 
         err_msg = (
             "Large difference between calculated and reference magnitudes"
         )
         np.testing.assert_allclose(mags, ref_mags, rtol=0.03, err_msg=err_msg)
```

### Comparing `hostphot-2.4.0/tests/test_preprocessing.py` & `hostphot-2.5.0/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.4.0/tests/test_rgb_images.py` & `hostphot-2.5.0/tests/test_rgb_images.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,14 @@
         for scaling in ["linear", "sqrt", "log", "asinh"]:
             create_RGB_image(images_dir=images_dir, scaling=scaling)
 
     def test_get_PS1_RGB_image(self):
         ra, dec = 50.527333, -15.400056
         get_PS1_RGB_image("PS1.jpg", ra=ra, dec=dec)
 
-    def test_get_SDSS_RGB_image(self):
-        ra, dec = 50.527333, -15.400056
-        get_SDSS_RGB_image("SDSS.jpg", ra=ra, dec=dec)
+    #def test_get_SDSS_RGB_image(self):
+    #    ra, dec = 50.527333, -15.400056
+    #    get_SDSS_RGB_image("SDSS.jpg", ra=ra, dec=dec)
 
 
 if __name__ == "__main__":
     unittest.main()
```

