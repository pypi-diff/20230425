# Comparing `tmp/edwh-0.8.0.tar.gz` & `tmp/edwh-0.9.0.tar.gz`

## Comparing `edwh-0.8.0.tar` & `edwh-0.9.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 edwh-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh-0.8.0/config.toml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh-0.8.0/requirements-dev.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 edwh-0.8.0/requirements.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0   193690 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    57310 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0    22378 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    66395 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0  1141227 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   134231 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   113689 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0    63269 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0    66858 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    24418 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    93277 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    31524 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    96592 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    48558 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    82126 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   182939 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    15221 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    30275 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    53725 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0   173191 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   152168 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0   248525 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   444970 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73973 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    96993 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   446284 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   140957 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/edwh/__about__.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/edwh/__about__.meta.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/edwh/__init__.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/edwh/__init__.meta.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/edwh/cli.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/edwh/cli.meta.json
--rw-r--r--   0        0        0     8144 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    27009 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0    10010 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    86512 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    33595 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    75549 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    69950 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    97916 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12954 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   382607 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/tests/__init__.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 edwh-0.8.0/.mypy_cache/3.10/tests/__init__.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 edwh-0.8.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 edwh-0.8.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 edwh-0.8.0/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh-0.8.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh-0.8.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.8.0/src/edwh/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.8.0/src/edwh/__init__.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 edwh-0.8.0/src/edwh/cli.py
--rw-r--r--   0        0        0    26913 2020-02-02 00:00:00.000000 edwh-0.8.0/src/edwh/tasks.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 edwh-0.8.0/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 edwh-0.8.0/README.md
--rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 edwh-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 edwh-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 edwh-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh-0.9.0/config.toml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh-0.9.0/requirements-dev.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 edwh-0.9.0/requirements.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0   193690 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    57310 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0    22378 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0    66395 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0  1141227 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0   134231 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   113689 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0    63269 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0    66858 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    24418 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0    93277 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0    31524 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0    96592 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    48558 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    82126 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0   182939 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    15221 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    30275 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    53725 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0   173191 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   152168 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0   248525 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   444970 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    73973 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    96993 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   446284 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0   140957 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/edwh/__about__.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/edwh/__about__.meta.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/edwh/__init__.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/edwh/__init__.meta.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/edwh/cli.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/edwh/cli.meta.json
+-rw-r--r--   0        0        0     8144 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    27009 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0    10010 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    86512 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    33595 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    75549 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    69950 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    97916 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12954 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   382607 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/tests/__init__.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 edwh-0.9.0/.mypy_cache/3.10/tests/__init__.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 edwh-0.9.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 edwh-0.9.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 edwh-0.9.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh-0.9.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh-0.9.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.9.0/src/edwh/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.9.0/src/edwh/__init__.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 edwh-0.9.0/src/edwh/cli.py
+-rw-r--r--   0        0        0    27507 2020-02-02 00:00:00.000000 edwh-0.9.0/src/edwh/tasks.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 edwh-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 edwh-0.9.0/README.md
+-rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 edwh-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 edwh-0.9.0/PKG-INFO
```

### Comparing `edwh-0.8.0/CHANGELOG.md` & `edwh-0.9.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.9.0 (2023-04-24)
+### Feature
+* -n will remove the config file so that you can reconfigure it. NOTE IT WILL REMOVE THE EXISTING CONFIG.TOML ([`33a8f5c`](https://github.com/educationwarehouse/edwh/commit/33a8f5ca59f9227233996828fc4c36da764cfb12))
+* -n will remove the config file so that you can reconfigure it. NOTE IT WILL REMOVE THE EXISTING CONFIG.TOML ([`9e2dc42`](https://github.com/educationwarehouse/edwh/commit/9e2dc4236827de74291a69fdfcb352ccca0a2fe0))
+* Fixed color coding ([`4e1c7ca`](https://github.com/educationwarehouse/edwh/commit/4e1c7ca16907fe7e1adc8b3ba468b7147b01e1fe))
+
+### Fix
+* Celeries will only be included in minimal when include_celeries_in_minimal == "true". ([`b12b997`](https://github.com/educationwarehouse/edwh/commit/b12b99764f317d47c35d8a9a8a1cba15cf595200))
+* When a key is not found en config.toml it will run edwh setup ([`742902a`](https://github.com/educationwarehouse/edwh/commit/742902ad42c5c26a73d3791aef948912be618ab2))
+* Wrong indexing of services ([`1e8a601`](https://github.com/educationwarehouse/edwh/commit/1e8a6012549fbd9eabde265e58fd5d76a31928cc))
+* Color codes and type ([`8d0674c`](https://github.com/educationwarehouse/edwh/commit/8d0674caed03c561b2c38e15654b5eb135144a17))
+
 ## v0.8.0 (2023-04-21)
 
 
 ## v0.7.1 (2023-04-21)
 ### Fix
 * Copy/paste error ([`197975f`](https://github.com/educationwarehouse/edwh/commit/197975f23ab6598289cb4dd2131bdeed7dec2918))
```

### Comparing `edwh-0.8.0/.mypy_cache/3.10/_ast.data.json` & `edwh-0.9.0/.mypy_cache/3.10/_ast.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/_ast.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/_codecs.data.json` & `edwh-0.9.0/.mypy_cache/3.10/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/_codecs.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/_collections_abc.data.json` & `edwh-0.9.0/.mypy_cache/3.10/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/_collections_abc.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/_ctypes.data.json` & `edwh-0.9.0/.mypy_cache/3.10/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/_ctypes.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/abc.data.json` & `edwh-0.9.0/.mypy_cache/3.10/abc.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/abc.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/abc.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/array.data.json` & `edwh-0.9.0/.mypy_cache/3.10/array.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/array.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/array.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/builtins.data.json` & `edwh-0.9.0/.mypy_cache/3.10/builtins.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/builtins.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/codecs.data.json` & `edwh-0.9.0/.mypy_cache/3.10/codecs.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/codecs.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/contextlib.data.json` & `edwh-0.9.0/.mypy_cache/3.10/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/contextlib.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/dataclasses.data.json` & `edwh-0.9.0/.mypy_cache/3.10/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/dataclasses.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/enum.data.json` & `edwh-0.9.0/.mypy_cache/3.10/enum.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/enum.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/enum.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/genericpath.data.json` & `edwh-0.9.0/.mypy_cache/3.10/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/genericpath.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/io.data.json` & `edwh-0.9.0/.mypy_cache/3.10/io.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/io.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/io.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/mmap.data.json` & `edwh-0.9.0/.mypy_cache/3.10/mmap.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/mmap.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/pathlib.data.json` & `edwh-0.9.0/.mypy_cache/3.10/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/pathlib.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/pickle.data.json` & `edwh-0.9.0/.mypy_cache/3.10/pickle.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/pickle.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/posixpath.data.json` & `edwh-0.9.0/.mypy_cache/3.10/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/posixpath.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/re.data.json` & `edwh-0.9.0/.mypy_cache/3.10/re.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/re.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/re.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/sre_compile.data.json` & `edwh-0.9.0/.mypy_cache/3.10/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/sre_compile.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/sre_constants.data.json` & `edwh-0.9.0/.mypy_cache/3.10/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/sre_constants.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/sre_parse.data.json` & `edwh-0.9.0/.mypy_cache/3.10/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/sre_parse.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/subprocess.data.json` & `edwh-0.9.0/.mypy_cache/3.10/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/subprocess.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/sys.data.json` & `edwh-0.9.0/.mypy_cache/3.10/sys.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/sys.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/sys.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/types.data.json` & `edwh-0.9.0/.mypy_cache/3.10/types.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/types.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/types.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/typing.data.json` & `edwh-0.9.0/.mypy_cache/3.10/typing.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/typing.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/typing.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/typing_extensions.data.json` & `edwh-0.9.0/.mypy_cache/3.10/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/typing_extensions.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/_typeshed/__init__.data.json` & `edwh-0.9.0/.mypy_cache/3.10/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/_typeshed/__init__.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/collections/__init__.data.json` & `edwh-0.9.0/.mypy_cache/3.10/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/collections/__init__.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/collections/abc.data.json` & `edwh-0.9.0/.mypy_cache/3.10/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/collections/abc.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/ctypes/__init__.data.json` & `edwh-0.9.0/.mypy_cache/3.10/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/ctypes/__init__.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/edwh/__about__.data.json` & `edwh-0.9.0/.mypy_cache/3.10/edwh/__about__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/edwh/__about__.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/edwh/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/edwh/__init__.data.json` & `edwh-0.9.0/.mypy_cache/3.10/edwh/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/edwh/__init__.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/edwh/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/edwh/cli.data.json` & `edwh-0.9.0/.mypy_cache/3.10/edwh/cli.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/edwh/cli.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/edwh/cli.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/email/__init__.data.json` & `edwh-0.9.0/.mypy_cache/3.10/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/email/__init__.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/email/charset.data.json` & `edwh-0.9.0/.mypy_cache/3.10/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/email/charset.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/email/contentmanager.data.json` & `edwh-0.9.0/.mypy_cache/3.10/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/email/contentmanager.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/email/errors.data.json` & `edwh-0.9.0/.mypy_cache/3.10/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/email/errors.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/email/header.data.json` & `edwh-0.9.0/.mypy_cache/3.10/email/header.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/email/header.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/email/message.data.json` & `edwh-0.9.0/.mypy_cache/3.10/email/message.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/email/message.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/email/policy.data.json` & `edwh-0.9.0/.mypy_cache/3.10/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/email/policy.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/importlib/__init__.data.json` & `edwh-0.9.0/.mypy_cache/3.10/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/importlib/__init__.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/importlib/abc.data.json` & `edwh-0.9.0/.mypy_cache/3.10/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/importlib/abc.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/importlib/machinery.data.json` & `edwh-0.9.0/.mypy_cache/3.10/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/importlib/machinery.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/importlib/metadata/__init__.data.json` & `edwh-0.9.0/.mypy_cache/3.10/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/importlib/metadata/__init__.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/importlib/metadata/_meta.data.json` & `edwh-0.9.0/.mypy_cache/3.10/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/importlib/metadata/_meta.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/os/__init__.data.json` & `edwh-0.9.0/.mypy_cache/3.10/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/os/__init__.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/os/path.data.json` & `edwh-0.9.0/.mypy_cache/3.10/os/path.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/os/path.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/tests/__init__.data.json` & `edwh-0.9.0/.mypy_cache/3.10/tests/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/.mypy_cache/3.10/tests/__init__.meta.json` & `edwh-0.9.0/.mypy_cache/3.10/tests/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/src/edwh/cli.py` & `edwh-0.9.0/src/edwh/cli.py`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/src/edwh/tasks.py` & `edwh-0.9.0/src/edwh/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     import random
     import re
     import sys
     import time
     import typing
     import json
     import importlib.util
+    from termcolor import colored
     from collections import defaultdict, OrderedDict
     from dataclasses import dataclass, field
     from pathlib import Path
     from statistics import median
 
     import tabulate
     import warnings
@@ -58,16 +59,17 @@
         allowed.add(" ")
 
     answer = input(prompt).lower().strip()
     answer += " "
 
     return answer[0] in allowed
 
+
 # used for treafik config
-def apply_dotenv_vars_to_yaml_templates(yaml_path: Path, dotenv_path:Path):
+def apply_dotenv_vars_to_yaml_templates(yaml_path: Path, dotenv_path: Path):
     """Indention preserving templating of yaml files, uses dotenv_path for variables.
 
     Pythong formatting is used with a dictionary of environment variables used from os environment variables
     updated by the dotenv_path parsed .dotenv entries.
     Templating is found using `# template:`
     indention is saved, everything after the above indicator is python string formatted and written back.
 
@@ -91,30 +93,29 @@
         new_lines = []
         for line in source_lines:
             if len(needle.findall(line)):
                 # split on template definition:
                 old, template = needle.split(line)
                 template = template.strip()
                 # save the indention part, add an addition if no indention was found
-                indention = (re.findall(r'^[\s]*',old)+[''])[0]
+                indention = (re.findall(r'^[\s]*', old) + [''])[0]
                 if not old.lstrip().startswith('#'):
                     # skip comment only lines
                     new = template.format(**env)
                     # reconstruct the line for the yaml file
                     line = f'{indention}{new} # template: {template}'
             new_lines.append(line)
         # move filepointer to the start of the file
-        yaml_file.seek(0,0)
+        yaml_file.seek(0, 0)
         # write all lines and newlines to the file
         yaml_file.write('\n'.join(new_lines))
         # and remove any part that might be left over (when the new file is shorter than the old one)
         yaml_file.truncate()
 
 
-
 @dataclass
 class TomlConfig:
     config: dict
     all_services: list[str]
     celeries: list[str]
     services_minimal: list[str]
     services_log: list[str]
@@ -137,29 +138,29 @@
         config_path = Path(fname)
         if not pathlib.Path.exists(config_path):
             setup(invoke.Context())
         config = load_toml(config_path)
 
         if "services" not in config:
             setup(invoke.Context())
-        for key in config["services"].keys():
-            if key not in ["minimal", "services", "include_celeries_in_minimal", "log"]:
+        for service_name in ["minimal", "services", "include_celeries_in_minimal", "log"]:
+            if service_name not in config["services"].keys():
                 setup(invoke.Context())
 
         if config["services"]["services"] == "discover":
             with open("docker-compose.yml", "r") as compose:
                 compose = yaml.load(compose, yaml.SafeLoader)
                 all_services = compose["services"].keys()
         else:
             all_services = config["services"]["services"]
 
         celeries = [s for s in all_services if "celery" in s.lower()]
 
-        minimal_services = config["services"]["minimal"] + celeries
-        if config["services"]["include_celeries_in_minimal"]:
+        minimal_services = config["services"]["minimal"]
+        if config["services"]["include_celeries_in_minimal"] == "true":
             minimal_services += celeries
         cls.__loaded = TomlConfig(
             config=config,
             all_services=all_services,
             celeries=celeries,
             services_minimal=minimal_services,
             services_log=config["services"]["log"],
@@ -238,19 +239,19 @@
             items[k.strip()] = v.strip()
 
     _dotenv_settings[cache_key] = items
     return items
 
 
 def check_env(
-    key: str,
-    default: typing.Optional[str],
-    comment: str,
-    prefix: str | None = None,
-    postfix: str | None = None,
+        key: str,
+        default: typing.Optional[str],
+        comment: str,
+        prefix: str | None = None,
+        postfix: str | None = None,
 ):
     """
     Test if key is in .env file path, appends prompted or default value if missing.
     """
     config = TomlConfig.load()
     env = read_dotenv()
     if key not in env:
@@ -431,25 +432,28 @@
     :rtype: Any
     """
 
     if "services" in toml_file and content_key in toml_file["services"]:
         return ""
 
     print_services(services)
-
+    print(colored("NOTE: To select multiple services please use single spaces or ',' inbetween numbers\n"
+          "For example '1, 2, 3, 4'", 'green'))
+    if content_key == "services":
+        print(colored("discover will include all services.\n", "green"))
     chosen_services_ids = input(content)
     if "," not in chosen_services_ids:
         chosen_services_ids = chosen_services_ids.split(" ")
     else:
         chosen_services_ids = chosen_services_ids.replace(" ", "").split(",")
 
     if chosen_services_ids[0] in default or len(chosen_services_ids[0]) == 0:
         return default
 
-    return [services[int(service_id)] for service_id in chosen_services_ids]
+    return [services[int(service_id)-1] for service_id in chosen_services_ids]
 
 
 def setup_config_file():
     """
     sets up config.toml for use
     """
     config_toml_file = tomlkit.loads(Path("config.toml").read_text())
@@ -467,20 +471,14 @@
     :param services: list of all docker services that are in the docker-compose.yml
     :return:
 
     """
     setup_config_file()
     config_toml_file = tomlkit.loads(Path("config.toml").read_text())
 
-    print("\033[91mNOTE: \033[00m")
-    print(
-        "To input multiple services please use singel spaces or ',' inbetween numbers"
-    )
-    print("For example '1, 2, 3, 4'")
-
     # services
     services_list = get_content_from_toml_file(
         all_services,
         config_toml_file,
         "services",
         "select a service by number(default is 'discover'): ",
         "discover",
@@ -504,49 +502,55 @@
         "select minimal services by number: ",
         [],
     )
     write_content_to_toml_file("minimal", content)
 
     # check if minimal exists if yes add celeries to services
     if (
-        "services" not in config_toml_file
-        or "include_celeries_in_minimal" not in config_toml_file["services"]
+            "services" not in config_toml_file
+            or "include_celeries_in_minimal" not in config_toml_file["services"]
     ):
         # check if user wants to include celeries
         include_celeries = (
             "true"
             if input("do you want to include celeries in minimal(Y/n): ").replace(
                 " ", ""
             )
-            in ["", "y", "Y"]
+               in ["", "y", "Y"]
             else "false"
         )
         write_content_to_toml_file("include_celeries_in_minimal", include_celeries)
 
     content = get_content_from_toml_file(
         minimal_services,
         config_toml_file,
         "log",
         "select services to be logged by number: ",
         [],
     )
     write_content_to_toml_file("log", content)
 
 
-@task(help={"run_local_setup": "executes local_tasks setup(default is True)"})
-def setup(c, run_local_setup=True):
+@task(help={"run_local_setup": "executes local_tasks setup(default is True)",
+            "new_config_toml": "will REMOVE and create a new config.toml file"})
+def setup(c, run_local_setup=True, new_config_toml=False):
     """
     sets up config.toml and tries to run setup in local tasks.py if it exists
 
     while configuring the config.toml the program will ask you to select a service by id.
     All service can be found by the print that is done above.
     While giving up id's please only give 1 id at the time, this goes for the services and the minimal services
 
     """
 
+    if new_config_toml and Path.is_file(Path("config.toml")):
+        remove_config = input(colored("are you sure you want to remove the config.toml(y/N): ", "red"))
+        if remove_config.replace(" ", "") in ["y", "Y"]:
+            os.remove("config.toml")
+
     if not Path.is_file(Path("config.toml")):
         with open("config.toml", "x") as config_toml:
             config_toml.close()
 
     print("getting services...")
 
     # get and print all found docker compose services
@@ -603,15 +607,15 @@
     """
     Show container and volume names.
 
     Based on `docker-compose ps -q` ids and `docker inspect` output.
     """
     lines = []
     for container_id in (
-        ctx.run("docker-compose ps -q", hide=True, warn=True).stdout.strip().split("\n")
+            ctx.run("docker-compose ps -q", hide=True, warn=True).stdout.strip().split("\n")
     ):
         ran = ctx.run(f"docker inspect {container_id}", hide=True, warn=True)
         if ran.ok:
             info = json.loads(ran.stdout)
             container = info[0]["Name"]
             for volume in [
                 _["Name"] for _ in info[0]["Mounts"] if _["Type"] == "volume"
@@ -623,31 +627,31 @@
     print(tabulate.tabulate(lines, headers="keys"))
 
 
 # noinspection PyShadowingNames
 @task(
     help=dict(
         service="Service to up, defaults to config.toml's [services].minimal. "
-        "Can be used multiple times, handles wildcards.",
+                "Can be used multiple times, handles wildcards.",
         build="request a build be performed first",
         quickest="restart only, no down;up",
         stop_timeout="timeout for stopping services, defaults to 2 seconds",
         tail="tails the log of restart services, defaults to False",
         clean="adds `--renew-anon-volumes --build` to `docker-compose up` command ",
     ),
     iterable=["service"],
 )
 def up(
-    ctx,
-    service=None,
-    build=False,
-    quickest=False,
-    stop_timeout=2,
-    tail=False,
-    clean=False,
+        ctx,
+        service=None,
+        build=False,
+        quickest=False,
+        stop_timeout=2,
+        tail=False,
+        clean=False,
 ):
     """Restart (or down;up) some or all services, after an optional rebuild."""
     ctx: Context = ctx
     config = TomlConfig.load()
     # recalculate the hash and save it, so with the next up, migrate will see differences and start migration
     set_env_value(config.dotenv_path, "SCHEMA_VERSION", calculate_schema_hash())
     # test for --service arguments, if none given: use defaults
@@ -737,15 +741,15 @@
     service = service_names(service or [])
     ctx.run(f"docker-compose down {' '.join(service)}")
 
 
 @task(
     help=dict(
         yes="Don't ask for confirmation, just do it. "
-        "(unless requirements.in files are found and the `edwh-pipcompile-plugin` is not installed)",
+            "(unless requirements.in files are found and the `edwh-pipcompile-plugin` is not installed)",
     )
 )
 def build(ctx, yes=False):
     """
     Build all services.
 
     Will test for the presence of `edwh-pipcompile-plugin` and use it to compile
@@ -782,30 +786,30 @@
                 if yes or confirm(f"recompile {req}? [Yn]", default=True):
                     pcl.compile(ctx, str(req.parent))
             else:
                 print("still current")
     else:
         print("Compilation of requirements.in files skipped.")
     if yes or (
-        not with_compile and confirm("Build docker images? [yN]", default=False)
+            not with_compile and confirm("Build docker images? [yN]", default=False)
     ):
         ctx.run("docker-compose build")
 
 
 @task(
     help=dict(
         service="Service to rebuild, can be used multiple times, handles wildcards.",
         force_rebuild="uses --no-cache option for docker-compose build",
     ),
     iterable=["service"],
 )
 def rebuild(
-    ctx,
-    service=None,
-    force_rebuild=False,
+        ctx,
+        service=None,
+        force_rebuild=False,
 ):
     """
     Downs ALL services, then rebuilds services using docker-compose build.
     """
     if service is None:
         service = []
     ctx.run("docker-compose down")
```

### Comparing `edwh-0.8.0/LICENSE.txt` & `edwh-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/README.md` & `edwh-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `edwh-0.8.0/pyproject.toml` & `edwh-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 ]
 dependencies = [
   'invoke >= 2.0',
   'fabric >= 3.0',
   'importlib_metadata >=3.6 ; python_version < "3.10"',
   'tabulate',
   'pyyaml',
+  'termcolor',
   'tomlkit ; python_version < "3.11"',
   'diceware',
 ]
 [project.optional-dependencies]
 dev = [
   "hatch",
   # "python-semantic-release >= 8.0.0a5",
```

### Comparing `edwh-0.8.0/PKG-INFO` & `edwh-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh
-Version: 0.8.0
+Version: 0.9.0
 Summary: Education Warehouse maintenance tools
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -18,14 +18,15 @@
 Requires-Python: >=3.10
 Requires-Dist: diceware
 Requires-Dist: fabric>=3.0
 Requires-Dist: importlib-metadata>=3.6; python_version < '3.10'
 Requires-Dist: invoke>=2.0
 Requires-Dist: pyyaml
 Requires-Dist: tabulate
+Requires-Dist: termcolor
 Requires-Dist: tomlkit; python_version < '3.11'
 Provides-Extra: bundle
 Requires-Dist: edwh-bundler-plugin; extra == 'bundle'
 Provides-Extra: bundler
 Requires-Dist: edwh-bundler-plugin; extra == 'bundler'
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
```

