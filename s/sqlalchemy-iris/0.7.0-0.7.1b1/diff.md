# Comparing `tmp/sqlalchemy-iris-0.7.0.tar.gz` & `tmp/sqlalchemy-iris-0.7.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-iris-0.7.0.tar", last modified: Sun Apr 16 12:13:13 2023, max compression
+gzip compressed data, was "sqlalchemy-iris-0.7.1b1.tar", last modified: Tue Apr 25 11:44:09 2023, max compression
```

## Comparing `sqlalchemy-iris-0.7.0.tar` & `sqlalchemy-iris-0.7.1b1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:13:13.690688 sqlalchemy-iris-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-16 12:12:47.000000 sqlalchemy-iris-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-16 12:13:13.690688 sqlalchemy-iris-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-16 12:12:47.000000 sqlalchemy-iris-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:13:13.682688 sqlalchemy-iris-0.7.0/intersystems_iris/
--rw-rw-rw-   0 runner    (1001) docker     (123)      299 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_BufferReader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1337 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_BufferWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1896 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_ConnectionInformation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      578 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_ConnectionParameters.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1483 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_Constant.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    20104 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_DBList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2311 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_Device.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      618 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_GatewayContext.py
--rw-rw-rw-   0 runner    (1001) docker     (123)       96 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_GatewayException.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2735 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_GatewayUtility.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    49548 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_IRIS.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    21467 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_IRISConnection.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2614 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_IRISEmbedded.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    12049 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_IRISGlobalNode.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      797 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_IRISGlobalNodeView.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6906 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_IRISIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10247 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_IRISList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6756 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (123)       82 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_IRISOREF.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    14456 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_IRISObject.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4905 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_IRISReference.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6643 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_InStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4130 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_LegacyIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      354 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_ListItem.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2966 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_ListReader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5515 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_ListWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     3797 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_LogFileStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1662 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_MessageHeader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1327 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_OutStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1963 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_PrintStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    41638 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_PythonGateway.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4330 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/_SharedMemorySocket.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1773 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      218 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:13:13.686688 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2535 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_Column.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    95424 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_DBAPI.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1391 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_Descriptor.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2113 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_IRISStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4076 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4776 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_Parameter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5151 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_ParameterCollection.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    12810 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_ResultSetRow.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      557 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_SQLType.py
--rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:13:13.686688 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/preparser/
--rw-rw-rw-   0 runner    (1001) docker     (123)    78828 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/preparser/_PreParser.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    16163 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/preparser/_Scanner.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2304 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/preparser/_Token.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6770 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/preparser/_TokenList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/preparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:13:13.686688 sqlalchemy-iris-0.7.0/intersystems_iris/pex/
--rw-rw-rw-   0 runner    (1001) docker     (123)     4370 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/pex/_BusinessHost.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5241 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/pex/_BusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10774 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/pex/_BusinessProcess.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5441 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/pex/_BusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10509 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/pex/_Common.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1203 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/pex/_Director.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      172 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/pex/_IRISBusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      585 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/pex/_IRISBusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      171 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/pex/_IRISInboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      522 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/pex/_IRISOutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2296 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/pex/_InboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      320 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/pex/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1628 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/pex/_OutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1379 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/intersystems_iris/pex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:13:13.686688 sqlalchemy-iris-0.7.0/iris/
--rw-rw-rw-   0 runner    (1001) docker     (123)      922 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      501 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/iris/iris_site.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2687 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/iris/irisbuiltins.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4808 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/iris/irisloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:13:13.686688 sqlalchemy-iris-0.7.0/irisnative/
--rw-rw-rw-   0 runner    (1001) docker     (123)      665 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/irisnative/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      341 2023-04-16 12:13:09.000000 sqlalchemy-iris-0.7.0/irisnative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-16 12:13:13.690688 sqlalchemy-iris-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-16 12:12:47.000000 sqlalchemy-iris-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:13:13.690688 sqlalchemy-iris-0.7.0/sqlalchemy_iris/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-16 12:12:47.000000 sqlalchemy-iris-0.7.0/sqlalchemy_iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40355 2023-04-16 12:12:47.000000 sqlalchemy-iris-0.7.0/sqlalchemy_iris/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-16 12:12:47.000000 sqlalchemy-iris-0.7.0/sqlalchemy_iris/embedded.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-16 12:12:47.000000 sqlalchemy-iris-0.7.0/sqlalchemy_iris/information_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-16 12:12:47.000000 sqlalchemy-iris-0.7.0/sqlalchemy_iris/iris.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-16 12:12:47.000000 sqlalchemy-iris-0.7.0/sqlalchemy_iris/provision.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-16 12:12:47.000000 sqlalchemy-iris-0.7.0/sqlalchemy_iris/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-16 12:12:47.000000 sqlalchemy-iris-0.7.0/sqlalchemy_iris/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:13:13.690688 sqlalchemy-iris-0.7.0/sqlalchemy_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-16 12:13:13.000000 sqlalchemy-iris-0.7.0/sqlalchemy_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-16 12:13:13.000000 sqlalchemy-iris-0.7.0/sqlalchemy_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 12:13:13.000000 sqlalchemy-iris-0.7.0/sqlalchemy_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-16 12:13:13.000000 sqlalchemy-iris-0.7.0/sqlalchemy_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-16 12:13:13.000000 sqlalchemy-iris-0.7.0/sqlalchemy_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-16 12:13:13.000000 sqlalchemy-iris-0.7.0/sqlalchemy_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:13:13.690688 sqlalchemy-iris-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-16 12:12:47.000000 sqlalchemy-iris-0.7.0/tests/test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:44:09.976089 sqlalchemy-iris-0.7.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-25 11:43:50.000000 sqlalchemy-iris-0.7.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-25 11:44:09.976089 sqlalchemy-iris-0.7.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-25 11:43:50.000000 sqlalchemy-iris-0.7.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:44:09.968089 sqlalchemy-iris-0.7.1b1/intersystems_iris/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      299 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_BufferReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1337 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_BufferWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1896 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_ConnectionInformation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      578 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_ConnectionParameters.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1483 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_Constant.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    20104 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_DBList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2311 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_Device.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      618 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_GatewayContext.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)       96 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_GatewayException.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2735 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_GatewayUtility.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    49548 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRIS.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    21467 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISConnection.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2614 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISEmbedded.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    12049 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISGlobalNode.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      797 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISGlobalNodeView.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6906 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10247 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6756 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)       82 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISOREF.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14456 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISObject.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4905 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISReference.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6643 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_InStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4130 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_LegacyIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      354 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_ListItem.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2966 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_ListReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5515 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_ListWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3797 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_LogFileStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1662 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_MessageHeader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1327 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_OutStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1963 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_PrintStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    41638 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_PythonGateway.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4330 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/_SharedMemorySocket.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1773 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      218 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:44:09.968089 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2535 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_Column.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    95424 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_DBAPI.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1391 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_Descriptor.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2113 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_IRISStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4076 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4776 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_Parameter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5151 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_ParameterCollection.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    12810 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_ResultSetRow.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      557 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_SQLType.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:44:09.972089 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/preparser/
+-rw-rw-rw-   0 runner    (1001) docker     (123)    78828 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/preparser/_PreParser.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    16163 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/preparser/_Scanner.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2304 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/preparser/_Token.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6770 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/preparser/_TokenList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/preparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:44:09.972089 sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4370 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_BusinessHost.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5241 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_BusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10774 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_BusinessProcess.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5441 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_BusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10509 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_Common.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1203 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_Director.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      172 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_IRISBusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      585 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_IRISBusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      171 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_IRISInboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      522 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_IRISOutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2296 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_InboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      320 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1628 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_OutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1379 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:44:09.972089 sqlalchemy-iris-0.7.1b1/iris/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      922 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      501 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/iris/iris_site.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2687 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/iris/irisbuiltins.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4808 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/iris/irisloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:44:09.972089 sqlalchemy-iris-0.7.1b1/irisnative/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      665 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/irisnative/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      341 2023-04-25 11:44:05.000000 sqlalchemy-iris-0.7.1b1/irisnative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-25 11:44:09.976089 sqlalchemy-iris-0.7.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-25 11:43:50.000000 sqlalchemy-iris-0.7.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:44:09.976089 sqlalchemy-iris-0.7.1b1/sqlalchemy_iris/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-25 11:43:50.000000 sqlalchemy-iris-0.7.1b1/sqlalchemy_iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40685 2023-04-25 11:43:50.000000 sqlalchemy-iris-0.7.1b1/sqlalchemy_iris/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-25 11:43:50.000000 sqlalchemy-iris-0.7.1b1/sqlalchemy_iris/embedded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-25 11:43:50.000000 sqlalchemy-iris-0.7.1b1/sqlalchemy_iris/information_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-25 11:43:50.000000 sqlalchemy-iris-0.7.1b1/sqlalchemy_iris/iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-25 11:43:50.000000 sqlalchemy-iris-0.7.1b1/sqlalchemy_iris/provision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-25 11:43:50.000000 sqlalchemy-iris-0.7.1b1/sqlalchemy_iris/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-25 11:43:50.000000 sqlalchemy-iris-0.7.1b1/sqlalchemy_iris/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:44:09.976089 sqlalchemy-iris-0.7.1b1/sqlalchemy_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-25 11:44:09.000000 sqlalchemy-iris-0.7.1b1/sqlalchemy_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-25 11:44:09.000000 sqlalchemy-iris-0.7.1b1/sqlalchemy_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:44:09.000000 sqlalchemy-iris-0.7.1b1/sqlalchemy_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 11:44:09.000000 sqlalchemy-iris-0.7.1b1/sqlalchemy_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 11:44:09.000000 sqlalchemy-iris-0.7.1b1/sqlalchemy_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-25 11:44:09.000000 sqlalchemy-iris-0.7.1b1/sqlalchemy_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:44:09.976089 sqlalchemy-iris-0.7.1b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-25 11:43:50.000000 sqlalchemy-iris-0.7.1b1/tests/test_suite.py
```

### Comparing `sqlalchemy-iris-0.7.0/LICENSE` & `sqlalchemy-iris-0.7.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/PKG-INFO` & `sqlalchemy-iris-0.7.1b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-iris
-Version: 0.7.0
+Version: 0.7.1b1
 Summary: InterSystems IRIS for SQLAlchemy
 Home-page: https://github.com/caretdev/sqlalchemy-iris
 Maintainer: CaretDev
 Maintainer-email: dmitry@caretdev.com
 License: MIT
 Project-URL: Source, https://github.com/caretdev/sqlalchemy-iris
 Project-URL: Tracker, https://github.com/caretdev/sqlalchemy-iris/issues
```

### Comparing `sqlalchemy-iris-0.7.0/README.md` & `sqlalchemy-iris-0.7.1b1/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_BufferWriter.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_BufferWriter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_ConnectionInformation.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_ConnectionInformation.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_ConnectionParameters.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_ConnectionParameters.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_Constant.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_Constant.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_DBList.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_DBList.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_Device.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_Device.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_GatewayContext.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_GatewayContext.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_GatewayUtility.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_GatewayUtility.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_IRIS.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRIS.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_IRISConnection.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISConnection.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_IRISEmbedded.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISEmbedded.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_IRISGlobalNode.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISGlobalNode.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_IRISGlobalNodeView.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISGlobalNodeView.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_IRISIterator.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISIterator.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_IRISList.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISList.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_IRISNative.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_IRISObject.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISObject.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_IRISReference.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_IRISReference.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_InStream.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_InStream.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_LegacyIterator.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_LegacyIterator.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_ListReader.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_ListReader.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_ListWriter.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_ListWriter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_LogFileStream.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_LogFileStream.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_MessageHeader.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_MessageHeader.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_OutStream.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_OutStream.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_PrintStream.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_PrintStream.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_PythonGateway.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_PythonGateway.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/_SharedMemorySocket.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/_SharedMemorySocket.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/__init__.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_Column.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_Column.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_DBAPI.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_DBAPI.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_Descriptor.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_Descriptor.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_IRISStream.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_IRISStream.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_Message.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_Message.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_Parameter.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_Parameter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_ParameterCollection.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_ParameterCollection.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_ResultSetRow.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_ResultSetRow.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/_SQLType.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/_SQLType.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/preparser/_PreParser.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/preparser/_PreParser.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/preparser/_Scanner.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/preparser/_Scanner.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/preparser/_Token.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/preparser/_Token.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/dbapi/preparser/_TokenList.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/dbapi/preparser/_TokenList.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/pex/_BusinessHost.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_BusinessHost.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/pex/_BusinessOperation.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_BusinessOperation.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/pex/_BusinessProcess.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_BusinessProcess.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/pex/_BusinessService.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_BusinessService.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/pex/_Common.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_Common.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/pex/_Director.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_Director.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/pex/_IRISBusinessService.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_IRISBusinessService.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/pex/_IRISOutboundAdapter.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_IRISOutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/pex/_InboundAdapter.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_InboundAdapter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/pex/_OutboundAdapter.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/_OutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/intersystems_iris/pex/__init__.py` & `sqlalchemy-iris-0.7.1b1/intersystems_iris/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/iris/__init__.py` & `sqlalchemy-iris-0.7.1b1/iris/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/iris/irisbuiltins.py` & `sqlalchemy-iris-0.7.1b1/iris/irisbuiltins.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/iris/irisloader.py` & `sqlalchemy-iris-0.7.1b1/iris/irisloader.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/irisnative/_IRISNative.py` & `sqlalchemy-iris-0.7.1b1/irisnative/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/setup.cfg` & `sqlalchemy-iris-0.7.1b1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlalchemy-iris
-version = 0.7.0
+version = 0.7.1b1
 description = InterSystems IRIS for SQLAlchemy
 long_description = file: README.md
 url = https://github.com/caretdev/sqlalchemy-iris
 maintainer = CaretDev
 maintainer_email = dmitry@caretdev.com
 license = MIT
 long_description_content_type = text/markdown
```

### Comparing `sqlalchemy-iris-0.7.0/sqlalchemy_iris/base.py` & `sqlalchemy-iris-0.7.1b1/sqlalchemy_iris/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
 import intersystems_iris.dbapi._DBAPI as dbapi
 from . import information_schema as ischema
-from . import types
 from sqlalchemy import exc
 from sqlalchemy.orm import aliased
 from sqlalchemy.engine import default
 from sqlalchemy.engine import reflection
 from sqlalchemy.sql import compiler
 from sqlalchemy.sql import util as sql_util
 from sqlalchemy.sql import between
@@ -16,40 +15,50 @@
 from sqlalchemy import sql, text
 from sqlalchemy import util
 from sqlalchemy import types as sqltypes
 
 from sqlalchemy.types import BIGINT
 from sqlalchemy.types import VARCHAR
 from sqlalchemy.types import INTEGER
-from sqlalchemy.types import BOOLEAN
 from sqlalchemy.types import DATE
 from sqlalchemy.types import TIMESTAMP
 from sqlalchemy.types import TIME
 from sqlalchemy.types import NUMERIC
-from sqlalchemy.types import FLOAT
 from sqlalchemy.types import BINARY
 from sqlalchemy.types import VARBINARY
 from sqlalchemy.types import TEXT
 from sqlalchemy.types import SMALLINT
 
+from .types import BIT
+from .types import DOUBLE
+from .types import LONGVARCHAR
+from .types import LONGVARBINARY
+from .types import TINYINT
+
+from .types import IRISBoolean
+from .types import IRISTime
+from .types import IRISTimeStamp
+from .types import IRISDate
+from .types import IRISDateTime
+
 ischema_names = {
     "BIGINT": BIGINT,
-    "VARCHAR": VARCHAR,
-    "INTEGER": INTEGER,
-    "BIT": BOOLEAN,
+    "BIT": BIT,
     "DATE": DATE,
-    "TIMESTAMP": TIMESTAMP,
+    "DOUBLE": DOUBLE,
+    "INTEGER": INTEGER,
+    "LONGVARBINARY": LONGVARBINARY,
+    "LONGVARCHAR": LONGVARCHAR,
     "NUMERIC": NUMERIC,
-    "DOUBLE": FLOAT,
-    "VARBINARY": BINARY,
-    "LONGVARCHAR": TEXT,
-    "LONGVARBINARY": VARBINARY,
-    "TIME": TIME,
     "SMALLINT": SMALLINT,
-    "TINYINT": SMALLINT,
+    "TIME": TIME,
+    "TIMESTAMP": TIMESTAMP,
+    "TINYINT": TINYINT,
+    "VARBINARY": VARBINARY,
+    "VARCHAR": VARCHAR,
 }
 
 RESERVED_WORDS = set(
     [
         "%afterhaving",
         "%allindex",
         "%alphaup",
@@ -642,16 +651,22 @@
             )
 
         return text
 
 
 class IRISTypeCompiler(compiler.GenericTypeCompiler):
     def visit_boolean(self, type_, **kw):
+        return self.visit_BIT(type_)
+
+    def visit_BIT(self, type_, **kw):
         return "BIT"
 
+    def visit_TEXT(self, type_, **kw):
+        return "VARCHAR(65535)"
+
 
 class IRISIdentifierPreparer(sql.compiler.IdentifierPreparer):
     """Install IRIS specific reserved words."""
 
     reserved_words = compiler.RESERVED_WORDS.copy()
     reserved_words.update(RESERVED_WORDS)
     illegal_initial_characters = compiler.ILLEGAL_INITIAL_CHARACTERS.union(["_"])
@@ -695,19 +710,19 @@
 
     def create_cursor(self):
         cursor = self._dbapi_connection.cursor()
         return cursor
 
 
 colspecs = {
-    sqltypes.Boolean: types.IRISBoolean,
-    sqltypes.Date: types.IRISDate,
-    sqltypes.DateTime: types.IRISDateTime,
-    sqltypes.TIMESTAMP: types.IRISTimeStamp,
-    sqltypes.Time: types.IRISTime,
+    sqltypes.Boolean: IRISBoolean,
+    sqltypes.Date: IRISDate,
+    sqltypes.DateTime: IRISDateTime,
+    sqltypes.TIMESTAMP: IRISTimeStamp,
+    sqltypes.Time: IRISTime,
 }
 
 
 class IRISExact(ReturnTypeFromArgs):
     """The IRIS SQL %EXACT() function."""
 
     inherit_cache = True
```

### Comparing `sqlalchemy-iris-0.7.0/sqlalchemy_iris/embedded.py` & `sqlalchemy-iris-0.7.1b1/sqlalchemy_iris/embedded.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/sqlalchemy_iris/information_schema.py` & `sqlalchemy-iris-0.7.1b1/sqlalchemy_iris/information_schema.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/sqlalchemy_iris/requirements.py` & `sqlalchemy-iris-0.7.1b1/sqlalchemy_iris/requirements.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/sqlalchemy_iris/types.py` & `sqlalchemy-iris-0.7.1b1/sqlalchemy_iris/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -116,7 +116,27 @@
                 minute = int(horolog // 60)
                 second = int(horolog % 60)
                 micro = int(value % 1 * 1000000)
                 return datetime.time(hour, minute, second, micro)
             return value
 
         return process
+
+
+class BIT(sqltypes.TypeEngine):
+    __visit_name__ = "BIT"
+
+
+class TINYINT(sqltypes.Integer):
+    __visit_name__ = "TINYINT"
+
+
+class DOUBLE(sqltypes.Float):
+    __visit_name__ = "DOUBLE"
+
+
+class LONGVARCHAR(sqltypes.VARCHAR):
+    __visit_name__ = "LONGVARCHAR"
+
+
+class LONGVARBINARY(sqltypes.VARBINARY):
+    __visit_name__ = "LONGVARBINARY"
```

### Comparing `sqlalchemy-iris-0.7.0/sqlalchemy_iris.egg-info/PKG-INFO` & `sqlalchemy-iris-0.7.1b1/sqlalchemy_iris.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-iris
-Version: 0.7.0
+Version: 0.7.1b1
 Summary: InterSystems IRIS for SQLAlchemy
 Home-page: https://github.com/caretdev/sqlalchemy-iris
 Maintainer: CaretDev
 Maintainer-email: dmitry@caretdev.com
 License: MIT
 Project-URL: Source, https://github.com/caretdev/sqlalchemy-iris
 Project-URL: Tracker, https://github.com/caretdev/sqlalchemy-iris/issues
```

### Comparing `sqlalchemy-iris-0.7.0/sqlalchemy_iris.egg-info/SOURCES.txt` & `sqlalchemy-iris-0.7.1b1/sqlalchemy_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.7.0/tests/test_suite.py` & `sqlalchemy-iris-0.7.1b1/tests/test_suite.py`

 * *Files identical despite different names*

