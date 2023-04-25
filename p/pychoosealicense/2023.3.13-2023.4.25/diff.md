# Comparing `tmp/pychoosealicense-2023.3.13.tar.gz` & `tmp/pychoosealicense-2023.4.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychoosealicense-2023.3.13.tar", last modified: Mon Mar 13 16:49:19 2023, max compression
+gzip compressed data, was "pychoosealicense-2023.4.25.tar", last modified: Tue Apr 25 07:34:18 2023, max compression
```

## Comparing `pychoosealicense-2023.3.13.tar` & `pychoosealicense-2023.4.25.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0 runner    (1001) docker     (122)     4692 2023-03-13 16:49:19.275640 pychoosealicense-2023.3.13/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6524 2023-03-13 16:49:19.275640 pychoosealicense-2023.3.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5020 2023-03-13 16:49:19.271640 pychoosealicense-2023.3.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-03-13 16:49:19.267640 pychoosealicense-2023.3.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-03-13 16:49:19.271640 pychoosealicense-2023.3.13/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     5084 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5778 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3104 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/description.py
--rw-r--r--   0 runner    (1001) docker     (122)    14871 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/eupl-1.2.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3868 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/ms-rl.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/bsd-4-clause.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/bsd-2-clause.txt
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/wtfpl.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1989 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/mit.txt
--rw-r--r--   0 runner    (1001) docker     (122)    14163 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/eupl-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (122)    15123 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/epl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    12624 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8437 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/cc0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6117 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/vim.txt
--rw-r--r--   0 runner    (1001) docker     (122)    15986 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/cern-ohl-w-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)      468 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2001 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2505 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/bsd-3-clause.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3295 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/upl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    19759 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/cc-by-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    11142 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/afl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    14802 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/cern-ohl-s-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    11580 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/osl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    12457 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/epl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9152 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/lgpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2348 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/bsd-3-clause-clear.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/postgresql.txt
--rw-r--r--   0 runner    (1001) docker     (122)    36394 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/gpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    23872 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/cecill-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/0bsd.txt
--rw-r--r--   0 runner    (1001) docker     (122)    21474 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/cc-by-sa-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/zlib.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5824 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/ofl-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (122)    10202 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/cern-ohl-p-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    19293 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/gpl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    26174 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/odbl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2939 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/ncsa.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9649 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/artistic-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/isc.txt
--rw-r--r--   0 runner    (1001) docker     (122)    19902 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/lppl-1.3c.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3226 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/ms-pl.txt
--rw-r--r--   0 runner    (1001) docker     (122)    10377 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/mulanpsl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2423 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/bsl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/mit-0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    18103 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/mpl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    23958 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/gfdl-1.3.txt
--rw-r--r--   0 runner    (1001) docker     (122)    27491 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/lgpl-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (122)    35944 2023-03-13 16:48:48.922787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/agpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    12156 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/_licenses/ecl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2830 2023-03-13 16:48:48.926787 pychoosealicense-2023.3.13/pychoosealicense/rules/rules.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     6524 2023-04-25 07:34:18.062186 pychoosealicense-2023.4.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4975 2023-04-25 07:34:18.058186 pychoosealicense-2023.4.25/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-04-25 07:34:18.050186 pychoosealicense-2023.4.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4692 2023-04-25 07:34:18.058186 pychoosealicense-2023.4.25/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-04-25 07:34:18.058186 pychoosealicense-2023.4.25/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5084 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     2037 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3104 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/description.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5809 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2830 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/rules/rules.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    12624 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    35944 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/agpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    19759 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/cc-by-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15123 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/epl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3868 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/ms-rl.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2939 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/ncsa.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/mit-0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/bsd-4-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    12156 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/ecl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    11580 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/osl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14802 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/cern-ohl-s-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    10202 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/cern-ohl-p-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9152 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/lgpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    18103 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/mpl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/0bsd.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2001 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2423 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/bsl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    11142 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/afl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2505 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/bsd-3-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/upl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/isc.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5824 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/ofl-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/zlib.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    21474 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/cc-by-sa-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/postgresql.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    12457 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/epl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14163 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/eupl-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    26174 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/odbl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14871 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/eupl-1.2.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6117 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/vim.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    23958 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/gfdl-1.3.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    36394 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/gpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9649 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/artistic-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    19902 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/lppl-1.3c.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    23872 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/cecill-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3226 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/ms-pl.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    27491 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/lgpl-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/bsd-2-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    19293 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/gpl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/wtfpl.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    15986 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/cern-ohl-w-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2348 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/bsd-3-clause-clear.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8437 2023-04-25 07:33:44.693920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/cc0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    10377 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/mulanpsl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1989 2023-04-25 07:33:44.697920 pychoosealicense-2023.4.25/pychoosealicense/_licenses/mit.txt
```

### Comparing `pychoosealicense-2023.3.13/README.rst` & `pychoosealicense-2023.4.25/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/PyChooseALicense
 	:target: https://github.com/repo-helper/PyChooseALicense/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/PyChooseALicense
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/PyChooseALicense/v2023.3.13
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/PyChooseALicense/v2023.4.25
 	:target: https://github.com/repo-helper/PyChooseALicense/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/PyChooseALicense
 	:target: https://github.com/repo-helper/PyChooseALicense/commit/master
 	:alt: GitHub last commit
```

### Comparing `pychoosealicense-2023.3.13/PKG-INFO` & `pychoosealicense-2023.4.25/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychoosealicense
-Version: 2023.3.13
+Version: 2023.4.25
 Summary: Provides license metadata from choosealicense.com
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: license
 Home-page: https://github.com/repo-helper/PyChooseALicense
 Project-URL: Issue Tracker, https://github.com/repo-helper/PyChooseALicense/issues
 Project-URL: Source Code, https://github.com/repo-helper/PyChooseALicense
@@ -131,15 +131,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/PyChooseALicense
 	:target: https://github.com/repo-helper/PyChooseALicense/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/PyChooseALicense
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/PyChooseALicense/v2023.3.13
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/PyChooseALicense/v2023.4.25
 	:target: https://github.com/repo-helper/PyChooseALicense/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/PyChooseALicense
 	:target: https://github.com/repo-helper/PyChooseALicense/commit/master
 	:alt: GitHub last commit
```

### Comparing `pychoosealicense-2023.3.13/pyproject.toml` & `pychoosealicense-2023.4.25/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "PyChooseALicense"
-version = "2023.3.13"
+version = "2023.4.25"
 description = "Provides license metadata from choosealicense.com"
 readme = "README.rst"
 keywords = [ "license",]
 dynamic = []
 dependencies = [
     "domdf-python-tools>=3.2.0",
     "python-frontmatter>=1.0.0",
@@ -96,15 +96,14 @@
     "sphinx_copybutton",
     "sphinxcontrib.default_values",
     "sphinx_debuginfo",
     "sphinx_licenseinfo",
     "seed_intersphinx_mapping",
     "html_section",
     "sphinx_toolbox_experimental.autosummary_widths",
-    "sphinx_toolbox_experimental.needspace",
     "sphinx_click",
 ]
 sphinxemoji_style = "twemoji"
 gitstamp_fmt = "%d %b %Y"
 templates_path = [ "_templates",]
 html_static_path = [ "_static",]
 source_suffix = ".rst"
```

### Comparing `pychoosealicense-2023.3.13/LICENSE` & `pychoosealicense-2023.4.25/LICENSE`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/__init__.py` & `pychoosealicense-2023.4.25/pychoosealicense/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 # this package
 from pychoosealicense import rules
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "2023.3.13"
+__version__: str = "2023.4.25"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["License", "get_license"]
 
 _yaml_handler = frontmatter.YAMLHandler()
 _field_convert_re = re.compile(r"\[(fullname|login|email|project|description|year|projecturl)]")
 _brace_map = {ord('{'): "{{", ord('}'): "}}"}
```

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_cli.py` & `pychoosealicense-2023.4.25/pychoosealicense/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 	def _verbose_rules(self) -> None:
 		# TODO: handle really narrow terminals (less than longest label)
 		#  Perhaps put description in wrapped paragraph on the next line
 
 		indent = 4
 
-		def print_rule(rule: Rule):
+		def print_rule(rule: Rule) -> None:
 			label = f"{rule.label} \u2013 "
 			max_desc_width = self.term_size - indent
 			first_line_extra_indent = (len(label) - indent) * ' '
 			wrapped_description = textwrap.wrap(first_line_extra_indent + rule.description, width=max_desc_width)
 			self._echo(f"{label}{wrapped_description[0].lstrip()}")
 			for line in wrapped_description[1:]:
 				self._echo(f"{' ' * indent}{line}")
@@ -122,15 +122,15 @@
 
 		data = [
 				self.the_license.permissions,
 				self.the_license.conditions,
 				self.the_license.limitations,
 				]
 
-		def get_rule_length(rule: Rule):
+		def get_rule_length(rule: Rule) -> int:
 			return len(rule.label) + 2
 
 		rule_lengths = (tuple(map(get_rule_length, row)) for row in data)
 		min_col_widths = []
 
 		for row, label_width in zip(rule_lengths, (12, 11, 12)):
 			if row:
@@ -157,28 +157,28 @@
 			self._echo(' ' * (column_widths[0] - len(permission.label)), nl=False)
 			self._echo(condition.label, nl=False)
 			self._echo(' ' * (column_widths[1] - len(condition.label)), nl=False)
 			self._echo(limitation.label)
 
 		self._echo()
 
-	def print_header(self):
+	def print_header(self) -> None:
 		"""
 		Print a header giving the name of the license and a short description.
 		"""
 
 		self._echo(Style.BRIGHT(self.the_license.title))
 		self._echo(Style.BRIGHT('=' * len(self.the_license.title)))
 		self._echo()
 
 		the_description = description.as_plaintext(self.the_license.description)
 		self._echo('\n'.join(textwrap.wrap(the_description, width=self.term_size)))
 		self._echo()
 
-	def print_info(self, verbose: bool = False):
+	def print_info(self, verbose: bool = False) -> None:
 		"""
 		Print information about the license.
 
 		:param verbose: Whether to show a description of each rule (permission, limitation etc.)
 		"""
 
 		self.print_header()
```

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/__main__.py` & `pychoosealicense-2023.4.25/pychoosealicense/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 @colour_option()
 @click.argument("license")
 @click_command()
 def main(
 		license: str,  # noqa: A002  # pylint: disable=redefined-builtin
 		colour: "ColourTrilean" = None,
 		verbose: bool = False,
-		):
+		) -> None:
 	"""
 	Show information about the given license.
 	"""
 
 	# this package
 	from pychoosealicense._cli import CLI
```

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/description.py` & `pychoosealicense-2023.4.25/pychoosealicense/description.py`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/eupl-1.2.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/eupl-1.2.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/ms-rl.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/ms-rl.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/bsd-4-clause.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/bsd-4-clause.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/bsd-2-clause.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/bsd-2-clause.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/wtfpl.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/wtfpl.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/mit.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/mit.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/eupl-1.1.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/eupl-1.1.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/epl-2.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/epl-2.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/apache-2.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/cc0-1.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/cc0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/vim.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/vim.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/cern-ohl-w-2.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/cern-ohl-w-2.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/unlicense.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/unlicense.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/bsd-3-clause.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/bsd-3-clause.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/upl-1.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/upl-1.0.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 description: A permissive, OSI and FSF approved, GPL compatible license, expressly allowing attribution with just a copyright notice and a short form link rather than the full text of the license.  Includes an express grant of patent rights.  Licensed works and modifications may be distributed under different terms and without source code, and the patent grant may also optionally be expanded to larger works to permit use as a contributor license agreement.
 
 how: Insert the license or a link to it along with a copyright notice into your source file(s), and/or create a text file (typically named LICENSE or LICENSE.txt) in the root of your source code and copy the text of the license into the file, replacing [year] with the current year and [fullname] with the name (or names) of the copyright holders.
 
 note: It is recommended to add a link to the license and copyright notice at the top of each source file, example text can be found at https://oss.oracle.com/licenses/upl/.
 
 using:
-  Oracle Product Images for Docker: https://github.com/oracle/docker-images/blob/main/LICENSE.txt
-  Skater: https://github.com/oracle/Skater/blob/master/LICENSE
+  Roc: https://github.com/roc-lang/roc/blob/main/LICENSE
+  Skater: https://github.com/oracle/skater/blob/main/LICENSE.txt
   Soufflé: https://github.com/souffle-lang/souffle/blob/master/LICENSE
 
 permissions:
   - commercial-use
   - modifications
   - distribution
   - patent-use
@@ -39,15 +39,15 @@
 rights in the Software, and any and all patent rights owned or freely
 licensable by each licensor hereunder covering either (i) the unmodified
 Software as contributed to or provided by such licensor, or (ii) the Larger
 Works (as defined below), to deal in both
 
 (a) the Software, and
 (b) any piece of software and/or hardware listed in the lrgrwrks.txt file if
-one is included with the Software (each a “Larger Work” to which the Software
+one is included with the Software (each a "Larger Work" to which the Software
 is contributed by such licensors),
 
 without restriction, including without limitation the rights to copy, create
 derivative works of, display, perform, and distribute the Software and make,
 use, sell, offer for sale, import, export, have made, and have sold the
 Software and the Larger Work(s), and to sublicense the foregoing rights on
 either these or other terms.
```

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/cc-by-4.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/cc-by-4.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/afl-3.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/afl-3.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/cern-ohl-s-2.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/cern-ohl-s-2.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/osl-3.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/osl-3.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/epl-1.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/epl-1.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/lgpl-3.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/lgpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/bsd-3-clause-clear.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/bsd-3-clause-clear.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/postgresql.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/postgresql.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/gpl-3.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/gpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/cecill-2.1.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/cecill-2.1.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/0bsd.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/0bsd.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/cc-by-sa-4.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/cc-by-sa-4.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/zlib.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/zlib.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/ofl-1.1.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/ofl-1.1.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/cern-ohl-p-2.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/cern-ohl-p-2.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/gpl-2.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/odbl-1.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/odbl-1.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/ncsa.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/ncsa.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/artistic-2.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/artistic-2.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/isc.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/isc.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/lppl-1.3c.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/lppl-1.3c.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/ms-pl.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/ms-pl.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/mulanpsl-2.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/mulanpsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/bsl-1.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/bsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/mit-0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/mit-0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/mpl-2.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/mpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/gfdl-1.3.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/gfdl-1.3.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/lgpl-2.1.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/lgpl-2.1.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/agpl-3.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/_licenses/ecl-2.0.txt` & `pychoosealicense-2023.4.25/pychoosealicense/_licenses/ecl-2.0.txt`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/rules/__init__.py` & `pychoosealicense-2023.4.25/pychoosealicense/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `pychoosealicense-2023.3.13/pychoosealicense/rules/rules.yml` & `pychoosealicense-2023.4.25/pychoosealicense/rules/rules.yml`

 * *Files identical despite different names*

