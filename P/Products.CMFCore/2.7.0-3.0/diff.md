# Comparing `tmp/Products.CMFCore-2.7.0.tar.gz` & `tmp/Products.CMFCore-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Products.CMFCore-2.7.0.tar", last modified: Fri Dec 16 13:02:53 2022, max compression
+gzip compressed data, was "Products.CMFCore-3.0.tar", last modified: Tue Apr 25 06:20:47 2023, max compression
```

## Comparing `Products.CMFCore-2.7.0.tar` & `Products.CMFCore-3.0.tar`

### file list

```diff
@@ -1,329 +1,319 @@
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/
--rw-r--r--   0 jens       (501) staff       (20)    32864 2022-12-16 12:56:17.000000 Products.CMFCore-2.7.0/CHANGES.rst
--rw-r--r--   0 jens       (501) staff       (20)      805 2022-12-16 12:53:25.000000 Products.CMFCore-2.7.0/CONTRIBUTING.md
--rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/COPYRIGHT.txt
--rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/LICENSE.txt
--rw-r--r--   0 jens       (501) staff       (20)      710 2022-12-16 12:53:25.000000 Products.CMFCore-2.7.0/MANIFEST.in
--rw-r--r--   0 jens       (501) staff       (20)    35520 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     1001 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/README.rst
--rw-r--r--   0 jens       (501) staff       (20)      402 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/buildout.cfg
--rw-r--r--   0 jens       (501) staff       (20)      136 2022-12-16 12:51:08.000000 Products.CMFCore-2.7.0/buildout4.cfg
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/docs/
--rw-r--r--   0 jens       (501) staff       (20)     3135 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/docs/Makefile
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/docs/_build/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/docs/_build/html/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/docs/_build/html/_sources/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/docs/_build/html/_sources/api/
--rw-r--r--   0 jens       (501) staff       (20)     2841 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/docs/_build/html/_sources/api/content.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     5496 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/docs/_build/html/_sources/api/tools.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)       28 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/docs/_build/html/_sources/changes.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      306 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/docs/_build/html/_sources/index.rst.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/docs/api/
--rw-r--r--   0 jens       (501) staff       (20)     2841 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/docs/api/content.rst
--rw-r--r--   0 jens       (501) staff       (20)     5496 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/docs/api/tools.rst
--rw-r--r--   0 jens       (501) staff       (20)       28 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/docs/changes.rst
--rw-r--r--   0 jens       (501) staff       (20)     6940 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/docs/conf.py
--rw-r--r--   0 jens       (501) staff       (20)      306 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/docs/index.rst
--rw-r--r--   0 jens       (501) staff       (20)       36 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/rtd.txt
--rw-r--r--   0 jens       (501) staff       (20)      735 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/setup.cfg
--rw-r--r--   0 jens       (501) staff       (20)     3088 2022-12-16 12:56:25.000000 Products.CMFCore-2.7.0/setup.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/
--rw-r--r--   0 jens       (501) staff       (20)    20473 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/ActionInformation.py
--rw-r--r--   0 jens       (501) staff       (20)    12251 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/ActionProviderBase.py
--rw-r--r--   0 jens       (501) staff       (20)     6607 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/ActionsTool.py
--rw-r--r--   0 jens       (501) staff       (20)     2306 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/CMFBTreeFolder.py
--rw-r--r--   0 jens       (501) staff       (20)    11363 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/CMFCatalogAware.py
--rw-r--r--   0 jens       (501) staff       (20)    31347 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/CachingPolicyManager.py
--rw-r--r--   0 jens       (501) staff       (20)    12812 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/CatalogTool.py
--rw-r--r--   0 jens       (501) staff       (20)    16869 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/ContentTypeRegistry.py
--rw-r--r--   0 jens       (501) staff       (20)    13717 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/CookieCrumbler.py
--rw-r--r--   0 jens       (501) staff       (20)    19062 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/DirectoryView.py
--rw-r--r--   0 jens       (501) staff       (20)     5432 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/DiscussionTool.py
--rw-r--r--   0 jens       (501) staff       (20)     5713 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/DynamicType.py
--rw-r--r--   0 jens       (501) staff       (20)     4137 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/Expression.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/Extensions/
--rw-r--r--   0 jens       (501) staff       (20)      154 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/Extensions/TestRecord.py
--rw-r--r--   0 jens       (501) staff       (20)     7622 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/FSDTMLMethod.py
--rw-r--r--   0 jens       (501) staff       (20)     7490 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/FSFile.py
--rw-r--r--   0 jens       (501) staff       (20)     5658 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/FSImage.py
--rw-r--r--   0 jens       (501) staff       (20)     4948 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/FSMetadata.py
--rw-r--r--   0 jens       (501) staff       (20)     9473 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/FSObject.py
--rw-r--r--   0 jens       (501) staff       (20)    11019 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/FSPageTemplate.py
--rw-r--r--   0 jens       (501) staff       (20)     5496 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/FSPropertiesObject.py
--rw-r--r--   0 jens       (501) staff       (20)     8158 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/FSPythonScript.py
--rw-r--r--   0 jens       (501) staff       (20)     6256 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/FSReSTMethod.py
--rw-r--r--   0 jens       (501) staff       (20)     6300 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/FSSTXMethod.py
--rw-r--r--   0 jens       (501) staff       (20)     5537 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/FSZSQLMethod.py
--rw-r--r--   0 jens       (501) staff       (20)    12284 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/MemberDataTool.py
--rw-r--r--   0 jens       (501) staff       (20)    21029 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/MembershipTool.py
--rw-r--r--   0 jens       (501) staff       (20)     3015 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/PortalContent.py
--rw-r--r--   0 jens       (501) staff       (20)    20280 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/PortalFolder.py
--rw-r--r--   0 jens       (501) staff       (20)     2826 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/PortalObject.py
--rw-r--r--   0 jens       (501) staff       (20)     7214 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/RegistrationTool.py
--rw-r--r--   0 jens       (501) staff       (20)     6706 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/Skinnable.py
--rw-r--r--   0 jens       (501) staff       (20)     3309 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/SkinsContainer.py
--rw-r--r--   0 jens       (501) staff       (20)    13575 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/SkinsTool.py
--rw-r--r--   0 jens       (501) staff       (20)    28843 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/TypesTool.py
--rw-r--r--   0 jens       (501) staff       (20)     3534 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/URLTool.py
--rw-r--r--   0 jens       (501) staff       (20)     3918 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/UndoTool.py
--rw-r--r--   0 jens       (501) staff       (20)     2528 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/WorkflowCore.py
--rw-r--r--   0 jens       (501) staff       (20)    21894 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/WorkflowTool.py
--rw-r--r--   0 jens       (501) staff       (20)     5055 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/browser/
--rw-r--r--   0 jens       (501) staff       (20)       14 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/browser/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     4067 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/browser/actions.py
--rw-r--r--   0 jens       (501) staff       (20)     1306 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/browser/configure.zcml
--rw-r--r--   0 jens       (501) staff       (20)     3661 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/browser/typeinfo.py
--rw-r--r--   0 jens       (501) staff       (20)      322 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/configure.zcml
--rw-r--r--   0 jens       (501) staff       (20)     1235 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/content.zcml
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/
--rw-r--r--   0 jens       (501) staff       (20)     1083 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/addCC.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1558 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/addFSDirView.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1383 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/addInstance.dtml
--rw-r--r--   0 jens       (501) staff       (20)    10284 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/cachingPolicies.dtml
--rw-r--r--   0 jens       (501) staff       (20)     3876 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/catalogFind.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1888 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/compareResults.dtml
--rw-r--r--   0 jens       (501) staff       (20)     2135 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/configureRegistrationTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1827 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/custdtml.dtml
--rw-r--r--   0 jens       (501) staff       (20)     2824 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/custfile.dtml
--rw-r--r--   0 jens       (501) staff       (20)     2761 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/custimage.dtml
--rw-r--r--   0 jens       (501) staff       (20)     2520 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/custprops.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1825 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/custpt.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1827 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/custpy.dtml
--rw-r--r--   0 jens       (501) staff       (20)     2092 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/custstx.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1808 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/custzsql.dtml
--rw-r--r--   0 jens       (501) staff       (20)      626 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/dirview_properties.dtml
--rw-r--r--   0 jens       (501) staff       (20)     6207 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/editToolsActions.dtml
--rw-r--r--   0 jens       (501) staff       (20)      844 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/explainActionsTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      346 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/explainCatalogTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      314 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/explainDiscussionTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      303 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/explainMemberDataTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      410 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/explainMembershipTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      294 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/explainRegistrationTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      443 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/explainSkinsTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      622 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/explainTypesTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      331 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/explainURLTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      310 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/explainUndoTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      465 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/explainWorkflowTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      433 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/extensionWidget.dtml
--rw-r--r--   0 jens       (501) staff       (20)     2802 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/findForm.dtml
--rw-r--r--   0 jens       (501) staff       (20)     8133 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/findResult.dtml
--rw-r--r--   0 jens       (501) staff       (20)      596 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/majorMinorWidget.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1694 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/manageActionProviders.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1355 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/memberdataContents.dtml
--rw-r--r--   0 jens       (501) staff       (20)     2110 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/membershipRolemapping.dtml
--rw-r--r--   0 jens       (501) staff       (20)      465 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/mimetypePredEdit.dtml
--rw-r--r--   0 jens       (501) staff       (20)      428 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/patternWidget.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1816 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/registryPredList.dtml
--rw-r--r--   0 jens       (501) staff       (20)      750 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/registryTest.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1941 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/selectWorkflows.dtml
--rw-r--r--   0 jens       (501) staff       (20)     3810 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/skinProps.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1023 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/zmi_workflows.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1132 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/event.zcml
--rw-r--r--   0 jens       (501) staff       (20)     1516 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exceptions.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/
--rw-r--r--   0 jens       (501) staff       (20)      752 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)    10072 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/actions.py
--rw-r--r--   0 jens       (501) staff       (20)     7625 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/cachingpolicymgr.py
--rw-r--r--   0 jens       (501) staff       (20)     1474 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/catalog.py
--rw-r--r--   0 jens       (501) staff       (20)     7132 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/configure.zcml
--rw-r--r--   0 jens       (501) staff       (20)    12455 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/content.py
--rw-r--r--   0 jens       (501) staff       (20)     5673 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/contenttyperegistry.py
--rw-r--r--   0 jens       (501) staff       (20)     3033 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/cookieauth.py
--rw-r--r--   0 jens       (501) staff       (20)     1514 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/mailhost.py
--rw-r--r--   0 jens       (501) staff       (20)     2535 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/memberdata.py
--rw-r--r--   0 jens       (501) staff       (20)     3017 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/properties.py
--rw-r--r--   0 jens       (501) staff       (20)     9014 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/skins.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/
--rw-r--r--   0 jens       (501) staff       (20)      664 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     2083 2022-12-16 12:51:22.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/conformance.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/four/
--rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/four/placeholder.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/one/
--rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/one/placeholder.txt
--rw-r--r--   0 jens       (501) staff       (20)    20983 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_actions.py
--rw-r--r--   0 jens       (501) staff       (20)     8397 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_cachingpolicymgr.py
--rw-r--r--   0 jens       (501) staff       (20)     7314 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_catalog.py
--rw-r--r--   0 jens       (501) staff       (20)    41376 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_content.py
--rw-r--r--   0 jens       (501) staff       (20)    11183 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_contenttyperegistry.py
--rw-r--r--   0 jens       (501) staff       (20)     7049 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_cookieauth.py
--rw-r--r--   0 jens       (501) staff       (20)     4592 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_mailhost.py
--rw-r--r--   0 jens       (501) staff       (20)     5594 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_memberdata.py
--rw-r--r--   0 jens       (501) staff       (20)     8832 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_properties.py
--rw-r--r--   0 jens       (501) staff       (20)    22804 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_skins.py
--rw-r--r--   0 jens       (501) staff       (20)    27115 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_typeinfo.py
--rw-r--r--   0 jens       (501) staff       (20)    12268 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_workflow.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/three/
--rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/three/placeholder.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/two/
--rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/two/placeholder.txt
--rw-r--r--   0 jens       (501) staff       (20)     8767 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/typeinfo.py
--rw-r--r--   0 jens       (501) staff       (20)     5125 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/workflow.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/help/
--rw-r--r--   0 jens       (501) staff       (20)     2049 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/help/Actions.stx
--rw-r--r--   0 jens       (501) staff       (20)     2007 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/help/CPMPolicies.stx
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/images/
--rw-r--r--   0 jens       (501) staff       (20)      148 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/images/cmf_action.gif
--rw-r--r--   0 jens       (501) staff       (20)      139 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/images/cmf_action_category.gif
--rw-r--r--   0 jens       (501) staff       (20)      270 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/images/cookie.gif
--rw-r--r--   0 jens       (501) staff       (20)      171 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/images/dirview.gif
--rw-r--r--   0 jens       (501) staff       (20)      126 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/images/fsdtml.gif
--rw-r--r--   0 jens       (501) staff       (20)      143 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/images/fsfile.gif
--rw-r--r--   0 jens       (501) staff       (20)      174 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/images/fsimage.gif
--rw-r--r--   0 jens       (501) staff       (20)      205 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/images/fsprops.gif
--rw-r--r--   0 jens       (501) staff       (20)      181 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/images/fspt.gif
--rw-r--r--   0 jens       (501) staff       (20)      272 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/images/fspy.gif
--rw-r--r--   0 jens       (501) staff       (20)      165 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/images/fssqlmethod.gif
--rw-r--r--   0 jens       (501) staff       (20)      124 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/images/registry.gif
--rw-r--r--   0 jens       (501) staff       (20)      118 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/images/typeinfo.gif
--rw-r--r--   0 jens       (501) staff       (20)    10457 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/indexing.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/interfaces/
--rw-r--r--   0 jens       (501) staff       (20)      743 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/interfaces/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)    18918 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/interfaces/_content.py
--rw-r--r--   0 jens       (501) staff       (20)     2391 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/interfaces/_cookieCrumbler.py
--rw-r--r--   0 jens       (501) staff       (20)     1677 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/interfaces/_events.py
--rw-r--r--   0 jens       (501) staff       (20)    64829 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/interfaces/_tools.py
--rw-r--r--   0 jens       (501) staff       (20)      316 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/meta.zcml
--rw-r--r--   0 jens       (501) staff       (20)     1816 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/namespace.py
--rw-r--r--   0 jens       (501) staff       (20)      139 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/overrides.zcml
--rw-r--r--   0 jens       (501) staff       (20)     5082 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/permissions.py
--rw-r--r--   0 jens       (501) staff       (20)     1763 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/permissions.zcml
--rw-r--r--   0 jens       (501) staff       (20)     3160 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/subscribers.py
--rw-r--r--   0 jens       (501) staff       (20)     1512 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/subscribers.zcml
--rw-r--r--   0 jens       (501) staff       (20)     7026 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/testing.py
--rw-r--r--   0 jens       (501) staff       (20)      712 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/testing.zcml
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/
--rw-r--r--   0 jens       (501) staff       (20)      171 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/base/
--rw-r--r--   0 jens       (501) staff       (20)       48 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/base/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     5270 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/base/content.py
--rw-r--r--   0 jens       (501) staff       (20)    12212 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/base/dummy.py
--rw-r--r--   0 jens       (501) staff       (20)     2922 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/base/security.py
--rw-r--r--   0 jens       (501) staff       (20)     8162 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/base/testcase.py
--rw-r--r--   0 jens       (501) staff       (20)     4363 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/base/tidata.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/
--rw-r--r--   0 jens       (501) staff       (20)       27 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/#test1.py
--rw-r--r--   0 jens       (501) staff       (20)       27 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/.test1.py
--rw-r--r--   0 jens       (501) staff       (20)      405 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/nested_view.zpt
--rw-r--r--   0 jens       (501) staff       (20)      195 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/nested_view_1.zpt
--rw-r--r--   0 jens       (501) staff       (20)       26 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/nested_view_2.dtml
--rw-r--r--   0 jens       (501) staff       (20)       62 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/nested_view_2.zpt
--rw-r--r--   0 jens       (501) staff       (20)      139 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/output_page_1.zpt
--rw-r--r--   0 jens       (501) staff       (20)       46 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/output_page_2.zpt
--rw-r--r--   0 jens       (501) staff       (20)       52 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/output_page_3.dtml
--rw-r--r--   0 jens       (501) staff       (20)       28 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/output_page_4.dtml
--rw-r--r--   0 jens       (501) staff       (20)       23 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test1.py
--rw-r--r--   0 jens       (501) staff       (20)       23 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test4.py
--rw-r--r--   0 jens       (501) staff       (20)       34 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test4.py.metadata
--rw-r--r--   0 jens       (501) staff       (20)       23 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test5.py
--rw-r--r--   0 jens       (501) staff       (20)       23 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test6.py
--rw-r--r--   0 jens       (501) staff       (20)      180 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test6.py.metadata
--rw-r--r--   0 jens       (501) staff       (20)       45 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testDTML.dtml
--rw-r--r--   0 jens       (501) staff       (20)       47 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testDTML.dtml.metadata
--rw-r--r--   0 jens       (501) staff       (20)       26 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testDTML_CPM3.dtml
--rw-r--r--   0 jens       (501) staff       (20)       41 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT.pt
--rw-r--r--   0 jens       (501) staff       (20)       26 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT.pt.metadata
--rw-r--r--   0 jens       (501) staff       (20)       92 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT2.pt
--rw-r--r--   0 jens       (501) staff       (20)       34 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT2.pt.metadata
--rw-r--r--   0 jens       (501) staff       (20)      140 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT3.pt
--rw-r--r--   0 jens       (501) staff       (20)       25 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT3.pt.metadata
--rw-r--r--   0 jens       (501) staff       (20)       73 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT4.pt
--rw-r--r--   0 jens       (501) staff       (20)       24 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT4.pt.metadata
--rw-r--r--   0 jens       (501) staff       (20)      140 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT5.pt
--rw-r--r--   0 jens       (501) staff       (20)       49 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT5.pt.metadata
--rw-r--r--   0 jens       (501) staff       (20)      397 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_CPM1.zpt
--rw-r--r--   0 jens       (501) staff       (20)      191 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_CPM2.zpt
--rw-r--r--   0 jens       (501) staff       (20)      183 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_multiline_python_dos.pt
--rw-r--r--   0 jens       (501) staff       (20)      179 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_multiline_python_mac.pt
--rw-r--r--   0 jens       (501) staff       (20)      179 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_multiline_python_unix.pt
--rw-r--r--   0 jens       (501) staff       (20)      169 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_utf8.pt
--rw-r--r--   0 jens       (501) staff       (20)       36 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPTbad.pt
--rw-r--r--   0 jens       (501) staff       (20)      107 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testReST.rst
--rw-r--r--   0 jens       (501) staff       (20)       28 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testReST.rst.metadata
--rw-r--r--   0 jens       (501) staff       (20)       87 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testSTX.stx
--rw-r--r--   0 jens       (501) staff       (20)       27 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testSTX.stx.metadata
--rw-r--r--   0 jens       (501) staff       (20)       84 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testUtf8.js
--rw-r--r--   0 jens       (501) staff       (20)      133 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testXMLPT.pt
--rw-r--r--   0 jens       (501) staff       (20)      151 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testXMLPT_with_encoding.pt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_directory/
--rw-r--r--   0 jens       (501) staff       (20)      179 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_directory/README.txt
--rw-r--r--   0 jens       (501) staff       (20)       39 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_directory.metadata
--rw-r--r--   0 jens       (501) staff       (20)       74 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_dos.py
--rw-r--r--   0 jens       (501) staff       (20)       22 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_dtml.dtml
--rw-r--r--   0 jens       (501) staff       (20)       36 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_dtml.dtml.metadata
--rw-r--r--   0 jens       (501) staff       (20)    11218 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file.swf
--rw-r--r--   0 jens       (501) staff       (20)       74 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file.swf.metadata
--rw-r--r--   0 jens       (501) staff       (20)    11218 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file_two.swf
--rw-r--r--   0 jens       (501) staff       (20)       55 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file_two.swf.metadata
--rw-r--r--   0 jens       (501) staff       (20)      209 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_image.gif
--rw-r--r--   0 jens       (501) staff       (20)       75 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_image.gif.metadata
--rw-r--r--   0 jens       (501) staff       (20)       77 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_mac.py
--rw-r--r--   0 jens       (501) staff       (20)       27 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_manual_ignore.py
--rw-r--r--   0 jens       (501) staff       (20)      207 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_props.props
--rw-r--r--   0 jens       (501) staff       (20)       25 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_text.metadata
--rw-r--r--   0 jens       (501) staff       (20)       23 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_text.txt
--rw-r--r--   0 jens       (501) staff       (20)       18 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_text_latin1.txt
--rw-r--r--   0 jens       (501) staff       (20)       30 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_text_latin1.txt.metadata
--rw-r--r--   0 jens       (501) staff       (20)       72 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_unix.py
--rw-r--r--   0 jens       (501) staff       (20)       26 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_warn.py
--rw-r--r--   0 jens       (501) staff       (20)      326 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testsql.zsql
--rw-r--r--   0 jens       (501) staff       (20)    19752 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_ActionInformation.py
--rw-r--r--   0 jens       (501) staff       (20)    10227 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_ActionProviderBase.py
--rw-r--r--   0 jens       (501) staff       (20)     7645 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_ActionsTool.py
--rw-r--r--   0 jens       (501) staff       (20)     1215 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_CMFBTreeFolder.py
--rw-r--r--   0 jens       (501) staff       (20)    11089 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_CMFCatalogAware.py
--rw-r--r--   0 jens       (501) staff       (20)    51856 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_CachingPolicyManager.py
--rw-r--r--   0 jens       (501) staff       (20)    17482 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_CatalogIndexing.py
--rw-r--r--   0 jens       (501) staff       (20)    23000 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_CatalogTool.py
--rw-r--r--   0 jens       (501) staff       (20)     9351 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_ContentTypeRegistry.py
--rw-r--r--   0 jens       (501) staff       (20)     9312 2022-06-21 13:27:27.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_CookieCrumbler.py
--rw-r--r--   0 jens       (501) staff       (20)    12040 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_DirectoryView.py
--rw-r--r--   0 jens       (501) staff       (20)     1482 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_DiscussionTool.py
--rw-r--r--   0 jens       (501) staff       (20)     7319 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_DynamicType.py
--rw-r--r--   0 jens       (501) staff       (20)     3228 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_Expression.py
--rw-r--r--   0 jens       (501) staff       (20)     6620 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSDTMLMethod.py
--rw-r--r--   0 jens       (501) staff       (20)    11259 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSFile.py
--rw-r--r--   0 jens       (501) staff       (20)     8834 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSImage.py
--rw-r--r--   0 jens       (501) staff       (20)     2463 2022-12-16 12:51:22.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSMetadata.py
--rw-r--r--   0 jens       (501) staff       (20)     8965 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSPageTemplate.py
--rw-r--r--   0 jens       (501) staff       (20)     4485 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSPropertiesObject.py
--rw-r--r--   0 jens       (501) staff       (20)    10414 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSPythonScript.py
--rw-r--r--   0 jens       (501) staff       (20)     7757 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSReSTMethod.py
--rw-r--r--   0 jens       (501) staff       (20)     9837 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSSTXMethod.py
--rw-r--r--   0 jens       (501) staff       (20)     7515 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSSecurity.py
--rw-r--r--   0 jens       (501) staff       (20)     4725 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSZSQLMethod.py
--rw-r--r--   0 jens       (501) staff       (20)     7936 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_MemberDataTool.py
--rw-r--r--   0 jens       (501) staff       (20)    13458 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_MembershipTool.py
--rw-r--r--   0 jens       (501) staff       (20)     8807 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_OpaqueItems.py
--rw-r--r--   0 jens       (501) staff       (20)     4809 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_PortalContent.py
--rw-r--r--   0 jens       (501) staff       (20)    47934 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_PortalFolder.py
--rw-r--r--   0 jens       (501) staff       (20)     1332 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_RegistrationTool.py
--rw-r--r--   0 jens       (501) staff       (20)     4857 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_SkinsTool.py
--rw-r--r--   0 jens       (501) staff       (20)    32807 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_TypesTool.py
--rw-r--r--   0 jens       (501) staff       (20)     2428 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_URLTool.py
--rw-r--r--   0 jens       (501) staff       (20)     1619 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_UndoTool.py
--rw-r--r--   0 jens       (501) staff       (20)    14705 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_WorkflowTool.py
--rw-r--r--   0 jens       (501) staff       (20)    10154 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_utils.py
--rw-r--r--   0 jens       (501) staff       (20)     2150 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_zcml.py
--rw-r--r--   0 jens       (501) staff       (20)      166 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tool.gif
--rw-r--r--   0 jens       (501) staff       (20)     1209 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/tool.zcml
--rw-r--r--   0 jens       (501) staff       (20)    28434 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/utils.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/www/
--rw-r--r--   0 jens       (501) staff       (20)      624 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/www/cpsDiff.pt
--rw-r--r--   0 jens       (501) staff       (20)     2075 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/www/typeinfoAliases.zpt
--rw-r--r--   0 jens       (501) staff       (20)     2638 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/www/typesAliases.zpt
--rw-r--r--   0 jens       (501) staff       (20)     2953 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/CMFCore/zcml.py
--rw-r--r--   0 jens       (501) staff       (20)      244 2021-11-02 08:51:13.000000 Products.CMFCore-2.7.0/src/Products/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products.CMFCore.egg-info/
--rw-r--r--   0 jens       (501) staff       (20)    35520 2022-12-16 13:02:52.000000 Products.CMFCore-2.7.0/src/Products.CMFCore.egg-info/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)    13998 2022-12-16 13:02:53.000000 Products.CMFCore-2.7.0/src/Products.CMFCore.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2022-12-16 13:02:52.000000 Products.CMFCore-2.7.0/src/Products.CMFCore.egg-info/dependency_links.txt
--rw-r--r--   0 jens       (501) staff       (20)       66 2022-12-16 13:02:52.000000 Products.CMFCore-2.7.0/src/Products.CMFCore.egg-info/entry_points.txt
--rw-r--r--   0 jens       (501) staff       (20)        9 2022-12-16 13:02:52.000000 Products.CMFCore-2.7.0/src/Products.CMFCore.egg-info/namespace_packages.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2022-12-16 12:53:25.000000 Products.CMFCore-2.7.0/src/Products.CMFCore.egg-info/not-zip-safe
--rw-r--r--   0 jens       (501) staff       (20)      378 2022-12-16 13:02:52.000000 Products.CMFCore-2.7.0/src/Products.CMFCore.egg-info/requires.txt
--rw-r--r--   0 jens       (501) staff       (20)        9 2022-12-16 13:02:52.000000 Products.CMFCore-2.7.0/src/Products.CMFCore.egg-info/top_level.txt
--rw-r--r--   0 jens       (501) staff       (20)     2148 2022-12-16 12:53:25.000000 Products.CMFCore-2.7.0/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.688586 Products.CMFCore-3.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    33142 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      805 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      688 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)    35523 2023-04-25 06:20:47.688981 Products.CMFCore-3.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1001 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      402 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/buildout.cfg
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.540149 Products.CMFCore-3.0/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3135 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/docs/Makefile
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.540486 Products.CMFCore-3.0/docs/api/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2841 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/docs/api/content.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5496 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/docs/api/tools.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/docs/changes.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6940 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      306 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       36 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/rtd.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      735 2023-04-25 06:20:47.690601 Products.CMFCore-3.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2796 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.535284 Products.CMFCore-3.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.540664 Products.CMFCore-3.0/src/Products/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.552225 Products.CMFCore-3.0/src/Products/CMFCore/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    20365 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/ActionInformation.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12217 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/ActionProviderBase.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6607 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/ActionsTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2306 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/CMFBTreeFolder.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11373 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/CMFCatalogAware.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    31340 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/CachingPolicyManager.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12804 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/CatalogTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    16841 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/ContentTypeRegistry.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    13312 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/CookieCrumbler.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    19042 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/DirectoryView.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5417 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/DiscussionTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5711 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/DynamicType.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4137 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/Expression.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.552379 Products.CMFCore-3.0/src/Products/CMFCore/Extensions/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      154 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/Extensions/TestRecord.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7316 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/FSDTMLMethod.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7396 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/FSFile.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5576 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/FSImage.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4937 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/FSMetadata.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9420 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/FSObject.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10454 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/FSPageTemplate.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5502 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/FSPropertiesObject.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8037 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/FSPythonScript.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6243 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/FSReSTMethod.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6295 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/FSSTXMethod.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5532 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/FSZSQLMethod.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12275 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/MemberDataTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    20936 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/MembershipTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3007 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/PortalContent.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    20141 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/PortalFolder.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2768 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/PortalObject.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7212 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/RegistrationTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6695 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/Skinnable.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3309 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/SkinsContainer.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    13340 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/SkinsTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    28718 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/TypesTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3534 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/URLTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3918 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/UndoTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2528 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/WorkflowCore.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    21841 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/WorkflowTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5055 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.552980 Products.CMFCore-3.0/src/Products/CMFCore/browser/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       14 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/browser/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4057 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/browser/actions.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1306 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/browser/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3660 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/browser/typeinfo.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      322 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1235 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/content.zcml
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.559181 Products.CMFCore-3.0/src/Products/CMFCore/dtml/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1083 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/addCC.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1558 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/addFSDirView.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1383 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/addInstance.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10284 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/cachingPolicies.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3876 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/catalogFind.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1888 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/compareResults.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2135 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/configureRegistrationTool.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1827 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/custdtml.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2824 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/custfile.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2761 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/custimage.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2520 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/custprops.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1825 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/custpt.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1827 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/custpy.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2092 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/custstx.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1808 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/custzsql.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      626 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/dirview_properties.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6207 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/editToolsActions.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      844 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/explainActionsTool.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      346 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/explainCatalogTool.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      314 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/explainDiscussionTool.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      303 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/explainMemberDataTool.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      410 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/explainMembershipTool.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      294 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/explainRegistrationTool.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      443 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/explainSkinsTool.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      622 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/explainTypesTool.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      331 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/explainURLTool.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      310 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/explainUndoTool.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      465 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/explainWorkflowTool.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      433 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/extensionWidget.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9219 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/findForm.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      596 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/majorMinorWidget.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1694 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/manageActionProviders.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1355 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/memberdataContents.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2110 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/membershipRolemapping.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      465 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/mimetypePredEdit.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      428 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/patternWidget.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1816 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/registryPredList.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      750 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/registryTest.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1941 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/selectWorkflows.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3810 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/skinProps.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1023 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/dtml/zmi_workflows.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1132 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/event.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1433 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exceptions.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.561351 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      752 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10072 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/actions.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7625 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/cachingpolicymgr.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1474 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/catalog.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7132 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12158 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/content.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5673 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/contenttyperegistry.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3033 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/cookieauth.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1514 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/mailhost.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2535 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/memberdata.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3017 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/properties.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9014 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/skins.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.563544 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      664 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2083 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/conformance.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.563703 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/four/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/four/placeholder.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.563841 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/one/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/one/placeholder.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)    21071 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_actions.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8482 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_cachingpolicymgr.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7400 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_catalog.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    40943 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_content.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11181 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_contenttyperegistry.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7131 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_cookieauth.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4652 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_mailhost.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5676 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_memberdata.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8751 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_properties.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    22889 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_skins.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    27200 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_typeinfo.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12350 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_workflow.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.563969 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/three/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/three/placeholder.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.564103 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/two/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/two/placeholder.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8767 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/typeinfo.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5125 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/exportimport/workflow.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.564373 Products.CMFCore-3.0/src/Products/CMFCore/help/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2049 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/help/Actions.stx
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2007 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/help/CPMPolicies.stx
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.566591 Products.CMFCore-3.0/src/Products/CMFCore/images/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      148 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/images/cmf_action.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)      139 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/images/cmf_action_category.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)      270 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/images/cookie.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)      171 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/images/dirview.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)      126 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/images/fsdtml.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)      143 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/images/fsfile.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)      174 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/images/fsimage.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)      205 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/images/fsprops.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)      181 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/images/fspt.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)      272 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/images/fspy.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)      165 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/images/fssqlmethod.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)      124 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/images/registry.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)      118 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/images/typeinfo.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10417 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/indexing.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.568280 Products.CMFCore-3.0/src/Products/CMFCore/interfaces/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      743 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/interfaces/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    18918 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/interfaces/_content.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2391 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/interfaces/_cookieCrumbler.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1677 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/interfaces/_events.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    64829 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/interfaces/_tools.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      316 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/meta.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1808 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/namespace.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      139 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/overrides.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5082 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/permissions.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1763 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/permissions.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3160 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/subscribers.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1512 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/subscribers.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6920 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/testing.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      712 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/testing.zcml
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.603421 Products.CMFCore-3.0/src/Products/CMFCore/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      171 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.608782 Products.CMFCore-3.0/src/Products/CMFCore/tests/base/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       48 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/base/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5270 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/base/content.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12202 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/base/dummy.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2897 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/base/security.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8156 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/base/testcase.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4363 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/base/tidata.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.537152 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.680943 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       27 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/#test1.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       27 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/.test1.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      405 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/nested_view.zpt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      195 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/nested_view_1.zpt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       26 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/nested_view_2.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)       62 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/nested_view_2.zpt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      139 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/output_page_1.zpt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       46 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/output_page_2.zpt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       52 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/output_page_3.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/output_page_4.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)       23 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test1.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       23 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test4.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       34 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test4.py.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)       23 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test5.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       23 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test6.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      180 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test6.py.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)       45 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testDTML.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)       47 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testDTML.dtml.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)       26 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testDTML_CPM3.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)       41 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       26 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT.pt.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)       92 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT2.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       34 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT2.pt.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)      140 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT3.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       25 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT3.pt.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)       73 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT4.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       24 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT4.pt.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)      140 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT5.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       49 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT5.pt.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)      397 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_CPM1.zpt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      191 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_CPM2.zpt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      183 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_multiline_python_dos.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      179 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_multiline_python_mac.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      179 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_multiline_python_unix.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      169 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_utf8.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       36 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testPTbad.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      107 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testReST.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testReST.rst.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)       87 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testSTX.stx
+-rw-r--r--   0 m.howitz   (502) staff       (20)       27 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testSTX.stx.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)       84 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testUtf8.js
+-rw-r--r--   0 m.howitz   (502) staff       (20)      133 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testXMLPT.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      151 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testXMLPT_with_encoding.pt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.682526 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_directory/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      179 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_directory/README.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       39 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_directory.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)       74 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_dos.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       22 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_dtml.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)       36 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_dtml.dtml.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11218 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file.swf
+-rw-r--r--   0 m.howitz   (502) staff       (20)       74 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file.swf.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11218 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file_two.swf
+-rw-r--r--   0 m.howitz   (502) staff       (20)       55 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file_two.swf.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)      209 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_image.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)       75 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_image.gif.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)       77 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_mac.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       27 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_manual_ignore.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      207 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_props.props
+-rw-r--r--   0 m.howitz   (502) staff       (20)       25 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_text.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)       23 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_text.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       18 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_text_latin1.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       30 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_text_latin1.txt.metadata
+-rw-r--r--   0 m.howitz   (502) staff       (20)       72 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_unix.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       26 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_warn.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      326 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/testsql.zsql
+-rw-r--r--   0 m.howitz   (502) staff       (20)    19603 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_ActionInformation.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10026 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_ActionProviderBase.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7718 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_ActionsTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1245 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_CMFBTreeFolder.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11162 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_CMFCatalogAware.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    52032 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_CachingPolicyManager.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    17423 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_CatalogIndexing.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    23073 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_CatalogTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9439 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_ContentTypeRegistry.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9183 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_CookieCrumbler.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12132 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_DirectoryView.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1542 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_DiscussionTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7290 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_DynamicType.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3258 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_Expression.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6693 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSDTMLMethod.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10397 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSFile.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8864 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSImage.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2493 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSMetadata.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9035 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSPageTemplate.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4515 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSPropertiesObject.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10488 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSPythonScript.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7830 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSReSTMethod.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9910 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSSTXMethod.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7585 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSSecurity.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4798 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSZSQLMethod.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7996 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_MemberDataTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    13574 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_MembershipTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8825 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_OpaqueItems.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4875 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_PortalContent.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    47604 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_PortalFolder.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1218 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_RegistrationTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4947 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_SkinsTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    32890 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_TypesTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2342 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_URLTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1641 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_UndoTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    14729 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_WorkflowTool.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10219 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_utils.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2150 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tests/test_zcml.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      166 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tool.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1209 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/tool.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)    28111 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/utils.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.687284 Products.CMFCore-3.0/src/Products/CMFCore/www/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      624 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/www/cpsDiff.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2075 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/www/typeinfoAliases.zpt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2638 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/www/typesAliases.zpt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2942 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/CMFCore/zcml.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/src/Products/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-25 06:20:47.542111 Products.CMFCore-3.0/src/Products.CMFCore.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    35523 2023-04-25 06:20:47.000000 Products.CMFCore-3.0/src/Products.CMFCore.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)    13770 2023-04-25 06:20:47.000000 Products.CMFCore-3.0/src/Products.CMFCore.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-04-25 06:20:47.000000 Products.CMFCore-3.0/src/Products.CMFCore.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       66 2023-04-25 06:20:47.000000 Products.CMFCore-3.0/src/Products.CMFCore.egg-info/entry_points.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-04-25 06:20:47.000000 Products.CMFCore-3.0/src/Products.CMFCore.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-04-25 06:20:47.000000 Products.CMFCore-3.0/src/Products.CMFCore.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      370 2023-04-25 06:20:47.000000 Products.CMFCore-3.0/src/Products.CMFCore.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-04-25 06:20:47.000000 Products.CMFCore-3.0/src/Products.CMFCore.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1860 2023-04-25 06:20:46.000000 Products.CMFCore-3.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Products.CMFCore-2.7.0/CHANGES.rst` & `Products.CMFCore-3.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 Products.CMFCore Changelog
 ==========================
 
+3.0 (2023-04-25)
+----------------
+
+- SkinsTool: fix Find form with Zope ZMI
+  (`#127 <https://github.com/zopefoundation/Products.CMFCore/pull/127>`_).
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop support for ``Zope 4.x``.
+
+- Make tests compatible with ``Zope >= 5.7.1``.
+
+
 2.7.0 (2022-12-16)
 ------------------
 
 - Fix insidious buildout configuration bug for tests against Zope 4.
 
 - Add support for Python 3.11.
```

### Comparing `Products.CMFCore-2.7.0/CONTRIBUTING.md` & `Products.CMFCore-3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/LICENSE.txt` & `Products.CMFCore-3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/MANIFEST.in` & `Products.CMFCore-3.0/MANIFEST.in`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs *.txt
 recursive-include docs Makefile
 
 recursive-include src *.py
-include buildout4.cfg
 recursive-include src *.dtml
 recursive-include src *.gif
 recursive-include src *.js
 recursive-include src *.metadata
 recursive-include src *.props
 recursive-include src *.pt
 recursive-include src *.rst
```

### Comparing `Products.CMFCore-2.7.0/PKG-INFO` & `Products.CMFCore-3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 Metadata-Version: 2.1
 Name: Products.CMFCore
-Version: 2.7.0
+Version: 3.0
 Summary: Zope Content Management Framework core components
 Home-page: https://github.com/zopefoundation/Products.CMFCore
 Author: Zope Foundation and Contributors
 Author-email: zope-cmf@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://zope.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/zopefoundation/Products.CMFCore/issues
 Project-URL: Sources, https://github.com/zopefoundation/Products.CMFCore
 Keywords: web application server zope cmf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
-Classifier: Framework :: Zope :: 4
 Classifier: Framework :: Zope :: 5
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: zsql
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 .. image:: https://github.com/zopefoundation/Products.CMFCore/actions/workflows/tests.yml/badge.svg
         :target: https://github.com/zopefoundation/Products.CMFCore/actions/workflows/tests.yml
@@ -62,14 +57,27 @@
 
 
 ------------------------------------------------------------
 
 Products.CMFCore Changelog
 ==========================
 
+3.0 (2023-04-25)
+----------------
+
+- SkinsTool: fix Find form with Zope ZMI
+  (`#127 <https://github.com/zopefoundation/Products.CMFCore/pull/127>`_).
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop support for ``Zope 4.x``.
+
+- Make tests compatible with ``Zope >= 5.7.1``.
+
+
 2.7.0 (2022-12-16)
 ------------------
 
 - Fix insidious buildout configuration bug for tests against Zope 4.
 
 - Add support for Python 3.11.
```

### Comparing `Products.CMFCore-2.7.0/README.rst` & `Products.CMFCore-3.0/README.rst`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/docs/Makefile` & `Products.CMFCore-3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/docs/_build/html/_sources/api/content.rst.txt` & `Products.CMFCore-3.0/docs/api/content.rst`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/docs/_build/html/_sources/api/tools.rst.txt` & `Products.CMFCore-3.0/docs/api/tools.rst`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/docs/conf.py` & `Products.CMFCore-3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/setup.cfg` & `Products.CMFCore-3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bdist_wheel]
-universal = 1
+universal = 0
 
 [flake8]
 doctests = 1
 no-accept-encodings = True
 htmldir = parts/flake8
 
 [check-manifest]
```

### Comparing `Products.CMFCore-2.7.0/setup.py` & `Products.CMFCore-3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,36 +17,32 @@
 _boundary = '\n' + ('-' * 60) + '\n\n'
 README = _boundary.join([
     _package_doc('README.rst'),
     _package_doc('CHANGES.rst'),
 ])
 
 setup(name='Products.%s' % NAME,
-      version='2.7.0',
+      version='3.0',
       description='Zope Content Management Framework core components',
       long_description=README,
       classifiers=[
           'Development Status :: 5 - Production/Stable',
           'Framework :: Plone',
-          'Framework :: Zope :: 4',
           'Framework :: Zope :: 5',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: Zope Public License',
-          'Programming Language :: Python :: 2',
-          'Programming Language :: Python :: 2.7',
           'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.5',
-          'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
           'Programming Language :: Python :: 3.11',
           'Programming Language :: Python :: Implementation :: CPython',
-          'Topic :: Software Development :: Libraries :: Application Frameworks',  # noqa
+          'Topic :: Software Development :: Libraries'
+          ' :: Application Frameworks',
       ],
       keywords='web application server zope cmf',
       author='Zope Foundation and Contributors',
       author_email='zope-cmf@zope.org',
       url='https://github.com/zopefoundation/Products.CMFCore',
       project_urls={
           'Documentation': 'https://zope.readthedocs.io',
@@ -56,33 +52,32 @@
       },
       license='ZPL 2.1',
       packages=find_packages('src'),
       package_dir={'': 'src'},
       include_package_data=True,
       namespace_packages=['Products'],
       zip_safe=False,
-      python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*',
+      python_requires='>=3.7',
       install_requires=[
           'setuptools',
-          'Zope >= 4.0b8',
+          'Zope >= 5',
           'docutils > 0.15',
           'five.localsitemanager',
           'Products.BTreeFolder2',
           'Products.GenericSetup >= 2.1.2',
           'Products.MailHost >= 4.0',
           'Products.PythonScripts',
           'Products.StandardCacheManagers',
           'Products.ZCatalog >= 4.0a2',  # Products.ZCTextIndex lives there now
-          'six',
           'zope.datetime',
           'zope.interface >= 3.8',
           ],
       extras_require={
           'test': ['Products.StandardCacheManagers'],
           'zsql': ['Products.ZSQLMethods >= 3.0.0b1'],
           'docs': ['Sphinx', 'repoze.sphinx.autointerface', 'pkginfo'],
           },
       entry_points="""
       [zope2.initialize]
-      Products.%s = Products.%s:initialize
-      """ % (NAME, NAME),
+      Products.{} = Products.{}:initialize
+      """.format(NAME, NAME),
       )
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/ActionInformation.py` & `Products.CMFCore-3.0/src/Products/CMFCore/ActionInformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """ Information about customizable actions.
 """
 
-import six
-from six.moves import UserDict
+from collections import UserDict
 
 from AccessControl.class_init import InitializeClass
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from Acquisition import aq_base
 from Acquisition import aq_inner
 from Acquisition import aq_parent
 from OFS.ObjectManager import IFAwareObjectManager
@@ -343,31 +342,31 @@
         if title is not _unchanged:
             self.title = title
         if description is not _unchanged:
             self.description = description
         if category is not _unchanged:
             self.category = category
         if condition is not _unchanged:
-            if condition and isinstance(condition, six.string_types):
+            if condition and isinstance(condition, str):
                 condition = Expression(condition)
             self.condition = condition
         if permissions is not _unchanged:
             if permissions == ('',):
                 permissions = ()
             self.permissions = permissions
         if priority is not _unchanged:
             self.priority = priority
         if visible is not _unchanged:
             self.visible = visible
         if action is not _unchanged:
-            if action and isinstance(action, six.string_types):
+            if action and isinstance(action, str):
                 action = Expression(action)
             self.setActionExpression(action)
         if icon_expr is not _unchanged:
-            if icon_expr and isinstance(icon_expr, six.string_types):
+            if icon_expr and isinstance(icon_expr, str):
                 icon_expr = Expression(icon_expr)
             self.setIconExpression(icon_expr)
         if link_target is not _unchanged:
             self.link_target = link_target
 
     @security.protected(View)
     def Title(self):
@@ -413,24 +412,24 @@
 
     @security.public
     def getActionExpression(self):
         """ Return the text of the TALES expression for our URL.
         """
         action = self._getActionObject()
         expr = action and action.text or ''
-        if expr and isinstance(expr, six.string_types):
+        if expr and isinstance(expr, str):
             if not expr.startswith('string:') and \
                not expr.startswith('python:'):
                 expr = 'string:${object_url}/%s' % expr
                 self.action = Expression(expr)
         return expr
 
     @security.private
     def setActionExpression(self, action):
-        if action and isinstance(action, six.string_types):
+        if action and isinstance(action, str):
             if not action.startswith('string:') and \
                not action.startswith('python:'):
                 action = 'string:${object_url}/%s' % action
             action = Expression(action)
         self.action = action
 
     @security.private
@@ -441,24 +440,24 @@
 
     @security.public
     def getIconExpression(self):
         """ Return the text of the TALES expression for our icon URL.
         """
         icon_expr = self._getIconExpressionObject()
         expr = icon_expr and icon_expr.text or ''
-        if expr and isinstance(expr, six.string_types):
+        if expr and isinstance(expr, str):
             if not expr.startswith('string:') and \
                not expr.startswith('python:'):
                 expr = 'string:${object_url}/%s' % expr
                 self.icon_expr = Expression(expr)
         return expr
 
     @security.private
     def setIconExpression(self, icon_expr):
-        if icon_expr and isinstance(icon_expr, six.string_types):
+        if icon_expr and isinstance(icon_expr, str):
             if not icon_expr.startswith('string:') and \
                not icon_expr.startswith('python:'):
                 icon_expr = 'string:${object_url}/%s' % icon_expr
             icon_expr = Expression(icon_expr)
         self.icon_expr = icon_expr
 
     @security.public
@@ -576,15 +575,15 @@
                     folder = aq_parent(aq_inner(folder))
         info = oai(context, folder, object)
         if request:
             cache[id(object)] = info
     return info
 
 
-class oai(object):
+class oai:
 
     # Provided for backward compatibility
     # Provides information that may be needed when constructing the list of
     # available actions.
     __allow_access_to_unprotected_subobjects__ = 1
 
     def __init__(self, tool, folder, object=None):
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/ActionProviderBase.py` & `Products.CMFCore-3.0/src/Products/CMFCore/ActionProviderBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 #
 ##############################################################################
 """ Implement a shared base for tools which provide actions.
 """
 
 from warnings import warn
 
-import six
-
 from AccessControl.class_init import InitializeClass
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from App.special_dtml import DTMLFile
 from zope.interface import implementer
 
 from .ActionInformation import ActionInfo
 from .ActionInformation import ActionInformation
@@ -90,15 +88,15 @@
         #
         ec = self._getExprContext(object)
         actions = self.listActions(object=object)
         actions = [ActionInfo(action, ec) for action in actions]
 
         if action_chain:
             filtered_actions = []
-            if isinstance(action_chain, six.string_types):
+            if isinstance(action_chain, str):
                 action_chain = (action_chain,)
             for action_ident in action_chain:
                 sep = action_ident.rfind('/')
                 category, id = action_ident[:sep], action_ident[sep+1:]
                 for ai in actions:
                     if id == ai['id'] and category == ai['category']:
                         filtered_actions.append(ai)
@@ -127,15 +125,15 @@
                                             check_permissions=False,
                                             check_condition=check_condition)
         if not action_infos:
             if object is None:
                 provider = self
             else:
                 provider = object
-            msg = 'Action "%s" not available for %s' % (
+            msg = 'Action "{}" not available for {}'.format(
                         action_chain, '/'.join(provider.getPhysicalPath()))
             raise ValueError(msg)
         for ai in action_infos:
             if ai['allowed']:
                 return ai
         raise AccessControl_Unauthorized('You are not allowed to access any '
                                          'of the specified Actions.')
@@ -315,15 +313,15 @@
 
         if not title:
             raise ValueError('A title is required.')
 
         if category == '':
             category = 'object'
 
-        if isinstance(permissions, six.string_types):
+        if isinstance(permissions, str):
             permissions = (permissions,)
 
         return ActionInformation(id=id, title=title, action=action,
                                  condition=condition,
                                  permissions=permissions,
                                  category=category,
                                  visible=visible,
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/ActionsTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/ActionsTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/CMFBTreeFolder.py` & `Products.CMFCore-3.0/src/Products/CMFCore/CMFBTreeFolder.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/CMFCatalogAware.py` & `Products.CMFCore-3.0/src/Products/CMFCore/CMFCatalogAware.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 from Acquisition import aq_base
 from App.special_dtml import DTMLFile
 from ExtensionClass import Base
 from OFS.interfaces import IObjectClonedEvent
 from OFS.interfaces import IObjectWillBeMovedEvent
 from zope.component import queryUtility
 from zope.component import subscribers
-from zope.container.interfaces import IObjectAddedEvent
-from zope.container.interfaces import IObjectMovedEvent
 from zope.interface import implementer
+from zope.lifecycleevent.interfaces import IObjectAddedEvent
 from zope.lifecycleevent.interfaces import IObjectCopiedEvent
 from zope.lifecycleevent.interfaces import IObjectCreatedEvent
+from zope.lifecycleevent.interfaces import IObjectMovedEvent
 
 from .interfaces import ICallableOpaqueItem
 from .interfaces import ICatalogAware
 from .interfaces import ICatalogTool
 from .interfaces import IOpaqueItemManager
 from .interfaces import IWorkflowAware
 from .interfaces import IWorkflowTool
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/CachingPolicyManager.py` & `Products.CMFCore-3.0/src/Products/CMFCore/CachingPolicyManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 from OFS.Cache import getVerifiedManagerIds
 from OFS.interfaces import IObjectWillBeMovedEvent
 from OFS.SimpleItem import SimpleItem
 from Persistence import PersistentMapping
 from Products.PageTemplates.Expressions import SecureModuleImporter
 from Products.PageTemplates.Expressions import getEngine
 from zope.component import getUtility
-from zope.container.interfaces import IObjectMovedEvent
 from zope.datetime import rfc1123_date
 from zope.interface import implementer
+from zope.lifecycleevent.interfaces import IObjectMovedEvent
 
 from .Expression import Expression
 from .interfaces import ICachingPolicy
 from .interfaces import ICachingPolicyManager
 from .interfaces import IMembershipTool
 from .permissions import ManagePortal
 from .permissions import View
@@ -657,15 +657,15 @@
     def removePolicy(self, policy_id, REQUEST=None):
         """
             Remove a caching policy.
         """
         self._removePolicy(policy_id)
         if REQUEST is not None:
             pth = '/manage_cachingPolicies?manage_tabs_message=Policy+removed.'
-            REQUEST['RESPONSE'].redirect('%s%s' % (self.absolute_url(), pth))
+            REQUEST['RESPONSE'].redirect(f'{self.absolute_url()}{pth}')
 
     #
     #   Policy manipulation methods.
     #
     @security.private
     def _addPolicy(self,
                    policy_id,
@@ -882,8 +882,8 @@
     """
     id = CachingPolicyManager.id
     mgr = CachingPolicyManager()
     self._setObject(id, mgr)
 
     if REQUEST is not None:
         pth = '/manage_main?manage_tabs_message=Caching+Policy+Manager+added.'
-        REQUEST['RESPONSE'].redirect('%s%s' % (self.absolute_url(), pth))
+        REQUEST['RESPONSE'].redirect(f'{self.absolute_url()}{pth}')
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/CatalogTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/CatalogTool.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         else:
             provided = providedBy(inst._IndexableObjectWrapper__ob)
             cls = type(inst)
             return ObjectSpecification(provided, cls)
 
 
 @implementer(IIndexableObjectWrapper, IIndexableObject)
-class IndexableObjectWrapper(object):
+class IndexableObjectWrapper:
 
     adapts(IContentish, ICatalogTool)
     __providedBy__ = IndexableObjectSpecification()
 
     def __init__(self, ob, catalog):
         # look up the workflow variables for the object
         wtool = queryUtility(IWorkflowTool)
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/ContentTypeRegistry.py` & `Products.CMFCore-3.0/src/Products/CMFCore/ContentTypeRegistry.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 #
 ##############################################################################
 """ Basic Site content type registry
 """
 
 import os
 import re
-
-from six.moves import urllib
+import urllib
 
 from AccessControl.class_init import InitializeClass
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from App.special_dtml import DTMLFile
 from OFS.SimpleItem import SimpleItem
 from Persistence import PersistentMapping
 from zope.component import getUtility
@@ -378,15 +377,15 @@
     @security.protected(ManagePortal)
     def doUpdatePredicate(self, predicate_id, predicate, typeObjectName,
                           REQUEST):
         """
         """
         self.updatePredicate(predicate_id, predicate, typeObjectName)
         pth = '/manage_predicates?manage_tabs_message=Predicate+updated.'
-        REQUEST['RESPONSE'].redirect('%s%s' % (self.absolute_url(), pth))
+        REQUEST['RESPONSE'].redirect(f'{self.absolute_url()}{pth}')
 
     @security.protected(ManagePortal)
     def doMovePredicateUp(self, predicate_id, REQUEST):
         """
         """
         predicate_ids = list(self.predicate_ids)
         ndx = predicate_ids.index(predicate_id)
@@ -416,15 +415,15 @@
 
     @security.protected(ManagePortal)
     def doRemovePredicate(self, predicate_id, REQUEST):
         """
         """
         self.removePredicate(predicate_id)
         pth = '/manage_predicates?manage_tabs_message=Predicate+removed.'
-        REQUEST['RESPONSE'].redirect('%s%s' % (self.absolute_url(), pth))
+        REQUEST['RESPONSE'].redirect(f'{self.absolute_url()}{pth}')
 
     security.declareProtected(ManagePortal,  # NOQA: flake8: D001
                               'manage_testRegistry')
     manage_testRegistry = DTMLFile('registryTest', _dtmldir)
 
     @security.protected(ManagePortal)
     def doTestRegistry(self, name, content_type, body, REQUEST):
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/CookieCrumbler.py` & `Products.CMFCore-3.0/src/Products/CMFCore/CookieCrumbler.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,33 +10,31 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """ Cookie Crumbler: Enable cookies for non-cookie user folders.
 """
 
 import base64
-
-import six
-from six.moves.urllib.parse import quote
-from six.moves.urllib.parse import unquote
+from urllib.parse import quote
+from urllib.parse import unquote
 
 from AccessControl.class_init import InitializeClass
 from AccessControl.Permissions import view_management_screens
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from Acquisition import aq_inner
 from Acquisition import aq_parent
 from App.special_dtml import HTMLFile
 from DateTime.DateTime import DateTime
 from OFS.interfaces import IObjectWillBeMovedEvent
 from OFS.PropertyManager import PropertyManager
 from OFS.SimpleItem import SimpleItem
 from zope.component import getUtility
-from zope.container.interfaces import IObjectMovedEvent
 from zope.globalrequest import getRequest
 from zope.interface import implementer
+from zope.lifecycleevent.interfaces import IObjectMovedEvent
 from ZPublisher import BeforeTraverse
 from ZPublisher.HTTPRequest import HTTPRequest
 
 from .interfaces import IActionsTool
 from .interfaces import ICookieCrumbler
 from .utils import UniqueObject
 from .utils import registerToolInterface
@@ -202,19 +200,16 @@
                 raise CookieCrumblerDisabled
 
             if self.pw_cookie in req and self.name_cookie in req:
                 # Attempt to log in and set cookies.
                 attempt = ATTEMPT_LOGIN
                 name = req[self.name_cookie]
                 pw = req[self.pw_cookie]
-                if six.PY2:
-                    ac = base64.encodestring('%s:%s' % (name, pw)).rstrip()
-                else:
-                    ac = base64.encodebytes(
-                        ('%s:%s' % (name, pw)).encode()).rstrip().decode()
+                ac = base64.encodebytes(
+                    (f'{name}:{pw}').encode()).rstrip().decode()
                 self._setAuthHeader(ac, req, resp)
                 if req.get(self.persist_cookie, 0):
                     # Persist the user name (but not the pw or session)
                     expires = (DateTime() + 365).toZone('GMT').rfc822()
                     resp.setCookie(self.name_cookie, name,
                                    path=self.getCookiePath(),
                                    expires=expires)
@@ -230,18 +225,15 @@
 
             elif self.auth_cookie in req:
                 # Attempt to resume a session if the cookie is valid.
                 # Copy __ac to the auth header.
                 ac = unquote(req[self.auth_cookie])
                 if ac and ac != 'deleted':
                     try:
-                        if six.PY2:
-                            base64.decodestring(ac)
-                        else:
-                            base64.decodebytes(ac.encode())
+                        base64.decodebytes(ac.encode())
                     except Exception:
                         # Not a valid auth header.
                         pass
                     else:
                         attempt = ATTEMPT_RESUME
                         self._setAuthHeader(ac, req, resp)
                         self.delRequestVar(req, self.auth_cookie)
@@ -277,19 +269,16 @@
     def credentialsChanged(self, user, name, pw, request=None):
         """
         Updates cookie credentials if user details are changed.
         """
         if request is None:
             request = getRequest()  # BBB for Membershiptool
         reponse = request['RESPONSE']
-        if six.PY2:
-            ac = base64.encodestring('%s:%s' % (name, pw)).rstrip()
-        else:
-            ac = base64.encodebytes(
-                ('%s:%s' % (name, pw)).encode()).rstrip().decode()
+        ac = base64.encodebytes(
+            (f'{name}:{pw}').encode()).rstrip().decode()
         method = self.getCookieMethod('setAuthCookie',
                                       self.defaultSetAuthCookie)
         method(reponse, self.auth_cookie, quote(ac))
 
     @security.public
     def logout(self, response=None):
         """
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/DirectoryView.py` & `Products.CMFCore-3.0/src/Products/CMFCore/DirectoryView.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     return [name for name in os.listdir(path)
             if name not in ignore and not ignore_re.match(name)]
 
 
 class _walker:
     def __init__(self, ignore):
         # make a dict for faster lookup
-        self.ignore = dict([(x, None) for x in ignore])
+        self.ignore = {x: None for x in ignore}
 
     def __call__(self, dirlist, dirname, names):
         # filter names inplace, so filtered directories don't get visited
         names[:] = [name for name in names
                     if name not in self.ignore and not ignore_re.match(name)]
         # append with stat info
         results = [(name, os.stat(os.path.join(dirname, name)).st_mtime)
@@ -142,16 +142,16 @@
         self.data = None
 
     def _readTypesFile(self):
         """ Read the .objects file produced by FSDump.
         """
         types = {}
         try:
-            f = open(os.path.join(self._filepath, '.objects'), 'rt')
-        except IOError:
+            f = open(os.path.join(self._filepath, '.objects'))
+        except OSError:
             pass
         else:
             lines = f.readlines()
             f.close()
             for line in lines:
                 try:
                     obname, meta_type = line.split(':')
@@ -381,15 +381,15 @@
 
             if path:
                 subpath = path + '/' + subob.getId()
             else:
                 subpath = subob.getId()
             title = getattr(subob, 'title', None)
             if title:
-                name = '%s (%s)' % (subpath, title)
+                name = f'{subpath} ({title})'
             else:
                 name = subpath
             rval.append((subpath, name))
             listFolderHierarchy(subob, subpath, rval, adding_meta_type)
 
 
 @implementer(IDirectoryView)
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/DiscussionTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/DiscussionTool.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """ Basic portal discussion access tool.
 """
 
-from six.moves import urllib
+import urllib
 
 from AccessControl.class_init import InitializeClass
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from Acquisition import Implicit
 from App.special_dtml import DTMLFile
 from DateTime.DateTime import DateTime
 from OFS.SimpleItem import SimpleItem
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/DynamicType.py` & `Products.CMFCore-3.0/src/Products/CMFCore/DynamicType.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         """ Get an Action info mapping specified by a chain of actions.
         """
         ti = self.getTypeInfo()
         if ti:
             return ti.getActionInfo(action_chain, self, check_visibility,
                                     check_condition)
         else:
-            msg = 'Action "%s" not available for %s' % (
+            msg = 'Action "{}" not available for {}'.format(
                         action_chain, '/'.join(self.getPhysicalPath()))
             raise ValueError(msg)
 
     @security.public
     def getIconURL(self):
         """ Get the absolute URL of the icon for the object.
         """
@@ -122,15 +122,15 @@
             utool = aq_get(self, 'portal_url')
         portal_url = utool()
         icon = self.getIconURL()
         if icon.startswith(portal_url):
             icon = icon[len(portal_url)+1:]
             if not relative_to_portal:
                 # Relative to REQUEST['BASEPATH1']
-                icon = '%s/%s' % (utool(relative=1), icon)
+                icon = f'{utool(relative=1)}/{icon}'
         try:
             utool.getPortalObject().unrestrictedTraverse(icon)
         except (AttributeError, KeyError):
             icon = ''
         return icon
 
     # deprecated alias
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/Expression.py` & `Products.CMFCore-3.0/src/Products/CMFCore/Expression.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/FSDTMLMethod.py` & `Products.CMFCore-3.0/src/Products/CMFCore/FSDTMLMethod.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """ Customizable DTML methods that come from the filesystem.
 """
 
-import six
-from six import get_unbound_function
-
 from AccessControl.class_init import InitializeClass
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from AccessControl.SecurityManagement import getSecurityManager
 from App.special_dtml import HTML
 from App.special_dtml import DTMLFile
 from DocumentTemplate.security import RestrictedDTML
 from OFS.DTMLMethod import DTMLMethod
@@ -79,15 +76,15 @@
     def _createZODBClone(self):
         """Create a ZODB (editable) equivalent of this object."""
         return DTMLMethod(self.read(), __name__=self.getId())
 
     def _readFile(self, reparse):
         """Read the data from the filesystem.
         """
-        file = open(self._filepath, 'r')  # not 'rb', as this is a text file!
+        file = open(self._filepath)  # not 'rb', as this is a text file!
         try:
             data = file.read()
         finally:
             file.close()
         self.raw = data
 
         if reparse:
@@ -147,31 +144,28 @@
                     result = r
                 else:
                     result = decapitate(r, RESPONSE)
                 if not self._cache_namespace_keys:
                     self.ZCacheable_set(result)
                 return result
 
-            if not isinstance(r, six.string_types) or RESPONSE is None:
+            if not isinstance(r, str) or RESPONSE is None:
                 if not self._cache_namespace_keys:
                     self.ZCacheable_set(r)
                 return r
 
         finally:
             security.removeContext(self)
 
         headers = RESPONSE.headers
         if not ('content-type' in headers or 'Content-Type' in headers):
             if 'content_type' in self.__dict__:
                 c = self.content_type
             else:
-                if six.PY2:
-                    c, _e = guess_content_type(self.getId(), r)
-                else:
-                    c, _e = guess_content_type(self.getId(), r.encode())
+                c, _e = guess_content_type(self.getId(), r.encode())
 
             RESPONSE.setHeader('Content-Type', c)
         if RESPONSE is not None:
             # caching policy manager hook
             _setCacheHeaders(self, {})
         result = decapitate(r, RESPONSE)
         if not self._cache_namespace_keys:
@@ -200,24 +194,23 @@
 
     # Zope 2.3.x way:
     def validate(self, inst, parent, name, value, md=None):
         return getSecurityManager().validate(inst, parent, name, value)
 
     if HAS_ZSERVER:
         security.declareProtected(FTPAccess, 'manage_FTPget')
-        manage_FTPget = get_unbound_function(DTMLMethod.manage_FTPget)
+        manage_FTPget = DTMLMethod.manage_FTPget
 
     security.declareProtected(ViewManagementScreens, 'PrincipiaSearchSource')
-    PrincipiaSearchSource = get_unbound_function(
-                                DTMLMethod.PrincipiaSearchSource)
+    PrincipiaSearchSource = DTMLMethod.PrincipiaSearchSource
 
     security.declareProtected(ViewManagementScreens, 'document_src')
-    document_src = get_unbound_function(DTMLMethod.document_src)
+    document_src = DTMLMethod.document_src
 
     security.declareProtected(ViewManagementScreens, 'manage_haveProxy')
-    manage_haveProxy = get_unbound_function(DTMLMethod.manage_haveProxy)
+    manage_haveProxy = DTMLMethod.manage_haveProxy
 
 
 InitializeClass(FSDTMLMethod)
 
 registerFileExtension('dtml', FSDTMLMethod)
 registerMetaType('DTML Method', FSDTMLMethod)
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/FSFile.py` & `Products.CMFCore-3.0/src/Products/CMFCore/FSFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 """ Customizable image objects that come from the filesystem.
 """
 
 import codecs
 import os
 from warnings import warn
 
-import six
-
 from AccessControl.class_init import InitializeClass
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from App.special_dtml import DTMLFile
 from OFS.Image import File
 from zope.contenttype import guess_content_type
 from ZPublisher.HTTPRequest import default_encoding
 
@@ -76,15 +74,15 @@
         headers = getattr(file, 'headers', None)
         if headers and 'content-type' in headers:
             content_type = headers['content-type']
         else:
             # Last resort: Use the (imperfect) content type guessing
             # mechanism from OFS.Image, which ultimately uses the
             # Python mimetypes module.
-            if not isinstance(body, (six.string_types, six.binary_type)):
+            if not isinstance(body, ((str,), bytes)):
                 body = body.data
             content_type, enc = guess_content_type(
                 getattr(file, 'filename', id), body, content_type)
             if (enc is None
                 and (content_type.startswith('text/') or
                      content_type.startswith('application/'))
                     and body.startswith(codecs.BOM_UTF8)):
@@ -112,16 +110,14 @@
             self.content_type = self._get_content_type(file, data, self.id)
         return data
 
     # The following is mainly taken from OFS/File.py
 
     def __str__(self):
         self._updateFromFS()
-        if six.PY2:
-            return str(self._readFile(0))
 
         data = self._readFile(0)
         ct = self.content_type
         encoding = None
 
         if 'charset=' in ct:
             encoding = ct[ct.find('charset=')+8:]
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/FSImage.py` & `Products.CMFCore-3.0/src/Products/CMFCore/FSImage.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 #
 ##############################################################################
 """ Customizable image objects that come from the filesystem.
 """
 
 import os
 
-from six import get_unbound_function
-
 from AccessControl.class_init import InitializeClass
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from App.special_dtml import DTMLFile
 from OFS.Image import Image
 from OFS.Image import getImageInfo
 
 from .DirectoryView import registerFileExtension
@@ -86,17 +84,17 @@
             self.content_type = ct
             self.width = width
             self.height = height
         return data
 
     # The following is mainly taken from OFS/Image.py
 
-    __str__ = get_unbound_function(Image.__str__)
+    __str__ = Image.__str__
 
-    _image_tag = get_unbound_function(Image.tag)
+    _image_tag = Image.tag
 
     @security.protected(View)
     def tag(self, *args, **kw):
         # Hook into an opportunity to reload metadata.
         self._updateFromFS()
         return self._image_tag(*args, **kw)
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/FSMetadata.py` & `Products.CMFCore-3.0/src/Products/CMFCore/FSMetadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 #
 ##############################################################################
 """Handles reading the properties for an object that comes from the filesystem.
 """
 
 import logging
 import re
+from configparser import ConfigParser
 from os.path import exists
 
-from six.moves.configparser import ConfigParser
-
 
 logger = logging.getLogger('CMFCore.FSMetadata')
 
 
 class CMFConfigParser(ConfigParser):
     """ This our wrapper around ConfigParser to
     solve a few minor niggles with the code """
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/FSObject.py` & `Products.CMFCore-3.0/src/Products/CMFCore/FSObject.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,28 +127,27 @@
             fpath = ()
         folder = portal_skins.restrictedTraverse(fpath)
         if id in folder.objectIds():
             # we cant catch the badrequest so
             # we'll that to check before hand
             obj = folder._getOb(id)
             if RESPONSE is not None:
-                RESPONSE.redirect('%s/manage_main?manage_tabs_message=%s' % (
-                    obj.absolute_url(),
-                    html_quote('An object with this id already exists')))
+                RESPONSE.redirect(
+                    '{}/manage_main?manage_tabs_message={}'.format(
+                        obj.absolute_url(),
+                        html_quote('An object with this id already exists')))
         else:
             folder._verifyObjectPaste(obj, validate_src=0)
             folder._setObject(id, obj)
 
             if RESPONSE is not None:
-                RESPONSE.redirect('%s/%s/manage_main' % (folder.absolute_url(),
-                                                         id))
+                RESPONSE.redirect(f'{folder.absolute_url()}/{id}/manage_main')
 
         if RESPONSE is not None:
-            RESPONSE.redirect('%s/%s/manage_main' % (
-                folder.absolute_url(), id))
+            RESPONSE.redirect(f'{folder.absolute_url()}/{id}/manage_main')
 
     def _createZODBClone(self):
         """Create a ZODB (editable) equivalent of this object."""
         raise NotImplementedError('This should be implemented in a subclass.')
 
     def _readFile(self, reparse):
         """Read the data from the filesystem.
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/FSPageTemplate.py` & `Products.CMFCore-3.0/src/Products/CMFCore/FSPageTemplate.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,14 @@
 #
 ##############################################################################
 """ Customizable page templates that come from the filesystem.
 """
 
 import re
 
-import six
-from six import get_unbound_function
-
 from AccessControl.class_init import InitializeClass
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from AccessControl.SecurityManagement import getSecurityManager
 from App.special_dtml import DTMLFile
 from Products.PageTemplates.PageTemplate import PageTemplate
 from Products.PageTemplates.utils import charsetFromMetaEquiv
 from Products.PageTemplates.utils import encodingFromXMLPreamble
@@ -85,23 +82,18 @@
 #    def ZCacheable_isCachingEnabled(self):
 #        return 0
 
     def _readFile(self, reparse):
         """Read the data from the filesystem.
         """
         if reparse:
-            if six.PY2:
-                # not 'rb', as this is a text file!
-                file = open(self._filepath, 'rU')
-            else:
-                file = open(self._filepath, 'br')
+            file = open(self._filepath, 'br')
             try:
                 data = file.read()
-                if not six.PY2:
-                    data = data.replace(b'\r\n', b'\n').replace(b'\r', b'\n')
+                data = data.replace(b'\r\n', b'\n').replace(b'\r', b'\n')
             finally:
                 file.close()
 
             # If we already have a content_type set it must come from a
             # .metadata file and we should always honor that. The content
             # type is initialized as text/html by default, so we only
             # attempt further detection if the default is encountered.
@@ -112,23 +104,20 @@
 
             if getattr(self, 'content_type', 'text/html') == 'text/html':
                 xml_info = xml_detect_re.match(data)
                 if xml_info:
                     # Smells like xml
                     # set "content_type" from the XML declaration
                     if xml_info.group(1):
-                        if six.PY3:
-                            encoding = xml_info.group(1).decode('ascii')
-                        else:
-                            encoding = xml_info.group(1)
+                        encoding = xml_info.group(1).decode('ascii')
                     else:
                         encoding = 'utf-8'
                     self.content_type = 'text/xml; charset=%s' % encoding
 
-            if not isinstance(data, six.text_type):
+            if not isinstance(data, str):
                 if encoding is None:
                     charset = getattr(self, 'charset', None)
 
                     if charset is None:
                         if self.content_type.startswith('text/html'):
                             mo = charset_re.search(self.content_type)
                             if mo:
@@ -148,21 +137,21 @@
                         preferred.insert(0, charset)
 
                 else:
                     preferred.insert(0, encoding)
 
                 for enc in preferred:
                     try:
-                        data = six.text_type(data, enc)
-                        if isinstance(data, six.text_type):
+                        data = str(data, enc)
+                        if isinstance(data, str):
                             break
                     except UnicodeDecodeError:
                         continue
                 else:
-                    data = six.text_type(data)
+                    data = str(data)
 
             self.write(data)
 
     @security.private
     def read(self):
         # Tie in on an opportunity to auto-update
         self._updateFromFS()
@@ -204,15 +193,15 @@
     def pt_source_file(self):
 
         """ Return a file name to be compiled into the TAL code.
         """
         return 'file:%s' % self._filepath
 
     security.declarePrivate('_ZPT_exec')  # NOQA: flake8: D001
-    _ZPT_exec = get_unbound_function(ZopePageTemplate._exec)
+    _ZPT_exec = ZopePageTemplate._exec
 
     @security.private
     def _exec(self, bound_names, args, kw):
         """Call a FSPageTemplate"""
         try:
             response = self.REQUEST.RESPONSE
         except AttributeError:
@@ -264,30 +253,29 @@
 
         return result
 
     # Copy over more methods
     if HAS_ZSERVER:
         security.declareProtected(FTPAccess,  # NOQA: flake8: D001
                                   'manage_FTPget')
-        manage_FTPget = get_unbound_function(ZopePageTemplate.manage_FTPget)
+        manage_FTPget = ZopePageTemplate.manage_FTPget
 
     security.declareProtected(View, 'get_size')  # NOQA: flake8: D001
-    get_size = get_unbound_function(ZopePageTemplate.get_size)
+    get_size = ZopePageTemplate.get_size
     getSize = get_size
 
     security.declareProtected(ViewManagementScreens,  # NOQA: flake8: D001
                               'PrincipiaSearchSource')
-    PrincipiaSearchSource = get_unbound_function(
-                                ZopePageTemplate.PrincipiaSearchSource)
+    PrincipiaSearchSource = ZopePageTemplate.PrincipiaSearchSource
 
     security.declareProtected(ViewManagementScreens,  # NOQA: flake8: D001
                               'document_src')
-    document_src = get_unbound_function(ZopePageTemplate.document_src)
+    document_src = ZopePageTemplate.document_src
 
-    pt_getContext = get_unbound_function(ZopePageTemplate.pt_getContext)
+    pt_getContext = ZopePageTemplate.pt_getContext
 
     source_dot_xml = Src()
 
 
 setattr(FSPageTemplate, 'source.xml', FSPageTemplate.source_dot_xml)
 setattr(FSPageTemplate, 'source.html', FSPageTemplate.source_dot_xml)
 InitializeClass(FSPageTemplate)
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/FSPropertiesObject.py` & `Products.CMFCore-3.0/src/Products/CMFCore/FSPropertiesObject.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,17 @@
 
         if RESPONSE is not None:
             if folder_path == '.':
                 fpath = ()
             else:
                 fpath = tuple(folder_path.split('/'))
             folder = self.restrictedTraverse(fpath)
-            RESPONSE.redirect('%s/%s/manage_propertiesForm' % (
-                folder.absolute_url(), self.getId()))
+            RESPONSE.redirect(
+                f'{folder.absolute_url()}/{self.getId()}/manage_propertiesForm'
+                )
 
     def _createZODBClone(self):
         """Create a ZODB (editable) equivalent of this object."""
         # Create a Folder to hold the properties.
         obj = Folder()
         obj.id = self.getId()
         map = []
@@ -89,15 +90,15 @@
         obj._properties = tuple(map)
 
         return obj
 
     def _readFile(self, reparse):
         """Read the data from the filesystem.
         """
-        file = open(self._filepath, 'r')  # not 'rb', as this is a text file!
+        file = open(self._filepath)  # not 'rb', as this is a text file!
         try:
             lines = file.readlines()
         finally:
             file.close()
 
         map = []
         lino = 0
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/FSPythonScript.py` & `Products.CMFCore-3.0/src/Products/CMFCore/FSPythonScript.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 #
 ##############################################################################
 """ Customizable Python scripts that come from the filesystem.
 """
 
 from difflib import unified_diff
 
-from six import get_unbound_function
-
 from AccessControl.class_init import InitializeClass
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from App.special_dtml import DTMLFile
 from ComputedAttribute import ComputedAttribute
 from Products.PageTemplates.PageTemplateFile import PageTemplateFile
 from Shared.DC.Scripts.Script import Script
 
@@ -44,15 +42,15 @@
     """
 
     # meta_type = 'Customized Python Script'  #(need permissions here)
 
     security = ClassSecurityInfo()
 
     def __init__(self, id, text):
-        super(CustomizedPythonScript, self).__init__(id)
+        super().__init__(id)
         self.write(text)
         self.original_source = text
 
     @security.protected(ViewManagementScreens)
     def getDiff(self):
         """ Return a diff of the current source with the original source.
         """
@@ -107,15 +105,15 @@
     def _createZODBClone(self):
         """Create a ZODB (editable) equivalent of this object."""
         return CustomizedPythonScript(self.getId(), self.read())
 
     def _readFile(self, reparse):
         """Read the data from the filesystem.
         """
-        file = open(self._filepath, 'r')
+        file = open(self._filepath)
         try:
             data = file.read()
         finally:
             file.close()
 
         if reparse:
             self._write(data, reparse)
@@ -129,15 +127,15 @@
         return Script.__render_with_namespace__(self, namespace)
 
     def __call__(self, *args, **kw):
         """Calls the script."""
         self._updateFromFS()
         return Script.__call__(self, *args, **kw)
 
-    _exec = get_unbound_function(PythonScript._exec)
+    _exec = PythonScript._exec
 
     security.declareProtected(ViewManagementScreens,  # NOQA: flake8: D001
                               'getModTime')
     # getModTime defined in FSObject
 
     def ZScriptHTML_tryParams(self):
         """Parameters to test the script with."""
@@ -160,23 +158,23 @@
         if RESPONSE is not None:
             RESPONSE.setHeader('Content-Type', 'text/plain')
         return self._source
 
     @security.protected(ViewManagementScreens)
     def PrincipiaSearchSource(self):
         """Support for searching - the document's contents are searched."""
-        return '%s\n%s' % (self._params, self._body)
+        return f'{self._params}\n{self._body}'
 
     @security.protected(ViewManagementScreens)
     def params(self):
         return self._params
 
     security.declareProtected(ViewManagementScreens,  # NOQA: flake8: D001
                               'manage_haveProxy')
-    manage_haveProxy = get_unbound_function(PythonScript.manage_haveProxy)
+    manage_haveProxy = PythonScript.manage_haveProxy
 
     @security.protected(ViewManagementScreens)
     def body(self):
         return self._body
 
     @security.protected(ViewManagementScreens)
     def get_size(self):
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/FSReSTMethod.py` & `Products.CMFCore-3.0/src/Products/CMFCore/FSReSTMethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 </metal:block>
 
 </body>
 </html>
 """
 
 
-class Warnings(object):
+class Warnings:
 
     def __init__(self):
         self.messages = []
 
     def write(self, message):
         self.messages.append(message)
 
@@ -102,15 +102,15 @@
         target = ZopePageTemplate(self.getId(), _CUSTOMIZED_TEMPLATE_ZPT)
         target._setProperty('rest', self.raw, 'text')
         return target
 
     def _readFile(self, reparse):
         """Read the data from the filesystem.
         """
-        file = open(self._filepath, 'r')  # not 'rb', as this is a text file!
+        file = open(self._filepath)  # not 'rb', as this is a text file!
         try:
             data = file.read()
         finally:
             file.close()
         self.raw = data
 
         if reparse:
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/FSSTXMethod.py` & `Products.CMFCore-3.0/src/Products/CMFCore/FSSTXMethod.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
         target._setProperty('stx', self.raw, 'text')
         return target
 
     def _readFile(self, reparse):
         """Read the data from the filesystem.
         """
-        file = open(self._filepath, 'r')  # not 'rb', as this is a text file!
+        file = open(self._filepath)  # not 'rb', as this is a text file!
         try:
             data = file.read()
         finally:
             file.close()
         self.raw = data
 
         if reparse:
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/FSZSQLMethod.py` & `Products.CMFCore-3.0/src/Products/CMFCore/FSZSQLMethod.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                           connection_hook=self.connection_hook,
                           direct=self.allow_simple_one_argument_traversal)
         return s
 
     def _readFile(self, reparse):
         """Read the data from the filesystem.
         """
-        file = open(self._filepath, 'r')  # not 'rb', as this is a text file!
+        file = open(self._filepath)  # not 'rb', as this is a text file!
         try:
             data = file.read()
         finally:
             file.close()
 
         # parse parameters
         parameters = {}
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/MemberDataTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/MemberDataTool.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
 class MemberData(Persistent):
 
     def __init__(self, id):
         self.id = id
 
 
 @implementer(IMember)
-class MemberAdapter(object):
+class MemberAdapter:
 
     """Member data adapter.
     """
 
     adapts(IUser, IMemberDataTool)
 
     security = ClassSecurityInfo()
@@ -257,15 +257,15 @@
     def setProperties(self, properties=None, **kw):
         """Allows the authenticated member to set his/her own properties.
         Accepts either keyword arguments or a mapping for the "properties"
         argument.
         """
         mtool = getUtility(IMembershipTool)
         if not mtool.isMemberAccessAllowed(self._user.getId()):
-            raise BadRequest(u'Only own properties can be set.')
+            raise BadRequest('Only own properties can be set.')
         if properties is None:
             properties = kw
         rtool = queryUtility(IRegistrationTool)
         if rtool is not None:
             failMessage = rtool.testPropertiesValidity(properties, self)
             if failMessage is not None:
                 raise BadRequest(failMessage)
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/MembershipTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/MembershipTool.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 ##############################################################################
 """ Basic membership tool.
 """
 
 import logging
 from warnings import warn
 
-import six
-
 from AccessControl.class_init import InitializeClass
 from AccessControl.requestmethod import postonly
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from AccessControl.SecurityManagement import getSecurityManager
 from AccessControl.users import nobody
 from Acquisition import aq_base
 from Acquisition import aq_inner
@@ -490,15 +488,15 @@
     def deleteMembers(self, member_ids, delete_memberareas=1,
                       delete_localroles=1, REQUEST=None):
         """ Delete members specified by member_ids.
         """
         # Delete members in acl_users.
         acl_users = self.acl_users
         if _checkPermission(ManageUsers, acl_users):
-            if isinstance(member_ids, six.string_types):
+            if isinstance(member_ids, str):
                 member_ids = (member_ids,)
             member_ids = list(member_ids)
             for member_id in member_ids[:]:
                 if not acl_users.getUserById(member_id, None):
                     member_ids.remove(member_id)
             try:
                 acl_users.userFolderDelUsers(member_ids)
@@ -546,43 +544,42 @@
 
 
 InitializeClass(MembershipTool)
 registerToolInterface('portal_membership', IMembershipTool)
 
 
 @implementer(IFactory)
-class HomeFolderFactoryBase(object):
+class HomeFolderFactoryBase:
 
     """Creates a home folder.
     """
 
-    title = _(u'Home Folder')
-    description = _(u'A home folder for portal members.')
+    title = _('Home Folder')
+    description = _('A home folder for portal members.')
 
     def __call__(self, id, title=None, *args, **kw):
         if title is None:
-            title = "{0}'s Home".format(id)
+            title = f"{id}'s Home"
         item = PortalFolder(id, title, *args, **kw)
         item.manage_setLocalRoles(id, ['Owner'])
         return item
 
     def getInterfaces(self):
         return implementedBy(PortalFolder)
 
 
 class _BBBHomeFolderFactory(HomeFolderFactoryBase):
 
     """Creates a home folder.
     """
 
-    description = _(u'Classic CMFCore home folder for portal members.')
+    description = _('Classic CMFCore home folder for portal members.')
 
     def __call__(self, id, title=None, *args, **kw):
-        item = super(_BBBHomeFolderFactory,
-                     self).__call__(id, title=title, *args, **kw)
+        item = super().__call__(id, title=title, *args, **kw)
 
         item.manage_permission(View,
                                ['Owner', 'Manager', 'Reviewer'], 0)
         item.manage_permission(AccessContentsInformation,
                                ['Owner', 'Manager', 'Reviewer'], 0)
         return item
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/PortalContent.py` & `Products.CMFCore-3.0/src/Products/CMFCore/PortalContent.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,28 +49,28 @@
 
     security.declareObjectProtected(View)
 
     def failIfLocked(self):
         """ Check if isLocked via webDav.
         """
         if self.wl_isLocked():
-            raise ResourceLockedError(_(u'This resource is locked via '
-                                        u'webDAV.'))
+            raise ResourceLockedError(_('This resource is locked via '
+                                        'webDAV.'))
         return 0
 
     #
     #   Contentish interface methods
     #
     @security.protected(View)
     def SearchableText(self):
         """ Returns a concatination of all searchable text.
 
         Should be overriden by portal objects.
         """
-        return '%s %s' % (self.Title(), self.Description())
+        return f'{self.Title()} {self.Description()}'
 
     def __call__(self):
         """ Invokes the default view.
         """
         ti = self.getTypeInfo()
         method_id = ti and ti.queryMethodID('(Default)', context=self)
         if method_id and method_id != '(Default)':
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/PortalFolder.py` & `Products.CMFCore-3.0/src/Products/CMFCore/PortalFolder.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,14 @@
 ##############################################################################
 """ PortalFolder: CMF-enabled Folder objects.
 """
 
 import marshal
 import re
 
-import six
-from six import get_unbound_function
-
 from AccessControl.class_init import InitializeClass
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from AccessControl.SecurityManagement import getSecurityManager
 from Acquisition import aq_base
 from Acquisition import aq_inner
 from Acquisition import aq_parent
 from OFS.Folder import Folder
@@ -148,15 +145,15 @@
         # Restrict allowed content types
         if filt is None:
             filt = {}
         else:
             # We'll modify it, work on a copy.
             filt = filt.copy()
         pt = filt.get('portal_type', [])
-        if isinstance(pt, six.string_types):
+        if isinstance(pt, str):
             pt = [pt]
         ttool = getUtility(ITypesTool)
         allowed_types = ttool.listContentTypes()
         if not pt:
             pt = allowed_types
         else:
             pt = [t for t in pt if t in allowed_types]
@@ -479,16 +476,15 @@
                 self, REQUEST, portal_status_message='Folder added')
 
 
 InitializeClass(PortalFolder)
 
 PortalFolderFactory = Factory(PortalFolder)
 
-manage_addPortalFolder = get_unbound_function(
-                            PortalFolder.manage_addPortalFolder)
+manage_addPortalFolder = PortalFolder.manage_addPortalFolder
 
 
 class ContentFilter:
 
     """Represent a predicate against a content object's metadata.
     """
 
@@ -540,21 +536,21 @@
                 self.description.append('Modified since: %s' % modified)
             if modified_usage == 'range:max':
                 self.predicates.append(lambda x, md=modified:
                                        md >= x.modified())
                 self.description.append('Modified before: %s' % modified)
 
         if Type:
-            if isinstance(Type, six.string_types):
+            if isinstance(Type, str):
                 Type = [Type]
             self.predicates.append(lambda x, Type=Type: x.Type() in Type)
             self.description.append('Type: %s' % ', '.join(Type))
 
         if portal_type and portal_type is not self.MARKER:
-            if isinstance(portal_type, six.string_types):
+            if isinstance(portal_type, str):
                 portal_type = [portal_type]
             self.predicates.append(lambda x, pt=portal_type:
                                    hasattr(aq_base(x), 'getPortalTypeName')
                                    and x.getPortalTypeName() in pt)
             self.description.append('Portal Type: %s' % ', '.join(portal_type))
 
     def hasSubject(self, obj):
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/PortalObject.py` & `Products.CMFCore-3.0/src/Products/CMFCore/PortalObject.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         (SetOwnProperties, ()),
         (MailForgottenPassword, ()),
         (RequestReview, ()),
         (ReviewPortalContent, ()),
         )
 
     def __init__(self, id, title='', description=''):
-        super(PortalObjectBase, self).__init__(id, title, description)
+        super().__init__(id, title, description)
         components = PersistentComponents('++etc++site')
         components.__parent__ = self
         self.setSiteManager(components)
 
     def __before_publishing_traverse__(self, arg1, arg2=None):
         """ Pre-traversal hook.
         """
@@ -66,12 +66,11 @@
         try:
             notify(BeforeTraverseEvent(self, REQUEST))
         except ComponentLookupError:
             # allow ZMI access, even if the portal's site manager is missing
             pass
         self.setupCurrentSkin(REQUEST)
 
-        super(PortalObjectBase,
-              self).__before_publishing_traverse__(arg1, arg2)
+        super().__before_publishing_traverse__(arg1, arg2)
 
 
 InitializeClass(PortalObjectBase)
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/RegistrationTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/RegistrationTool.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,16 +137,16 @@
         # exception if the given id already exists, the password does not
         # comply with the policy in effect, or the authenticated user is not
         # allowed to grant one of the roles listed (where Member is a special
         # role that can always be granted); these conditions should be
         # detected before the fact so that a cleaner message can be printed.
 
         if not self.isMemberIdAllowed(id):
-            raise ValueError(_(u'The login name you selected is already in '
-                               u'use or is not valid. Please choose another.'))
+            raise ValueError(_('The login name you selected is already in '
+                               'use or is not valid. Please choose another.'))
 
         failMessage = self.testPasswordValidity(password)
         if failMessage is not None:
             raise ValueError(failMessage)
 
         if properties is not None:
             failMessage = self.testPropertiesValidity(properties)
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/Skinnable.py` & `Products.CMFCore-3.0/src/Products/CMFCore/Skinnable.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 """ Base class for object managers which can be "skinned".
 
 Skinnable object managers inherit attributes from a skin specified in
 the browser request.  Skins are stored in a fixed-name subobject.
 """
 
 import logging
-
-from six.moves._thread import get_ident
+from _thread import get_ident
 
 from AccessControl.class_init import InitializeClass
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from Acquisition import aq_base
 from OFS.ObjectManager import ObjectManager
 from ZODB.POSException import ConflictError
 from zope.component import queryUtility
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/SkinsContainer.py` & `Products.CMFCore-3.0/src/Products/CMFCore/SkinsContainer.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/SkinsTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/SkinsTool.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,22 +96,17 @@
                               'manage_overview')
     manage_overview = DTMLFile('explainSkinsTool', _dtmldir)
 
     security.declareProtected(ManagePortal,  # NOQA: flake8: D001
                               'manage_propertiesForm')
     manage_propertiesForm = DTMLFile('dtml/skinProps', globals())
 
-    # the following two methods override those in FindSupport, to
+    # the following method override the one in FindSupport, to
     # support marking of objects used in specific skins
     security.declareProtected(ManagePortal,  # NOQA: flake8: D001
-                              'manage_findResult')
-    manage_findResult = DTMLFile('findResult', _dtmldir,
-                                 management_view='Find')
-
-    security.declareProtected(ManagePortal,  # NOQA: flake8: D001
                               'manage_findForm')
     manage_findForm = DTMLFile('findForm', _dtmldir,
                                management_view='Find')
 
     security.declareProtected(ManagePortal,  # NOQA: flake8: D001
                               'manage_compareResults')
     manage_compareResults = DTMLFile('compareResults', _dtmldir,
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/TypesTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/TypesTool.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 ##############################################################################
 """ Type registration tool.
 """
 
 import logging
 from warnings import warn
 
-import six
-
 from AccessControl.class_init import InitializeClass
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from AccessControl.SecurityManagement import getSecurityManager
 from Acquisition import aq_base
 from Acquisition import aq_get
 from App.special_dtml import DTMLFile
 from OFS.ObjectManager import IFAwareObjectManager
@@ -564,15 +562,15 @@
             # newstyle factory
             factory = getUtility(IFactory, self.factory)
             obj = factory(id, *args, **kw)
             if hasattr(obj, '_setPortalTypeName'):
                 obj._setPortalTypeName(self.getId())
             notify(ObjectCreatedEvent(obj))
             rval = container._setObject(id, obj)
-            newid = isinstance(rval, six.string_types) and rval or id
+            newid = isinstance(rval, str) and rval or id
             obj = container._getOb(newid)
 
         return obj
 
 
 InitializeClass(FactoryTypeInformation)
 
@@ -733,15 +731,15 @@
         """
             Return an instance which implements the
             TypeInformation interface, corresponding to
             the specified 'contentType'.  If contentType is actually
             an object, rather than a string, attempt to look up
             the appropriate type info using its portal_type.
         """
-        if not isinstance(contentType, six.string_types):
+        if not isinstance(contentType, str):
             if hasattr(aq_base(contentType), 'getPortalTypeName'):
                 contentType = contentType.getPortalTypeName()
                 if contentType is None:
                     return None
             else:
                 return None
         ob = getattr(self, contentType, None)
@@ -805,17 +803,15 @@
         info = self.getTypeInfo(type_name)
         if info is None:
             raise ValueError('No such content type: %s' % type_name)
 
         ob = info.constructInstance(container, id, *args, **kw)
 
         if RESPONSE is not None:
-            immediate_url = '%s/%s' % (ob.absolute_url(),
-                                       info.immediate_view)
-            RESPONSE.redirect(immediate_url)
+            RESPONSE.redirect(f'{ob.absolute_url()}/{info.immediate_view}')
 
         return ob.getId()
 
     @security.private
     def listActions(self, info=None, object=None):
         """ List all the actions defined by a provider.
         """
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/URLTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/URLTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/UndoTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/UndoTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/WorkflowCore.py` & `Products.CMFCore-3.0/src/Products/CMFCore/WorkflowCore.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/WorkflowTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/WorkflowTool.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 #
 ##############################################################################
 """ Basic workflow tool.
 """
 
 import sys
 
-import six
-
 from AccessControl.class_init import InitializeClass
 from AccessControl.requestmethod import postonly
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from Acquisition import aq_base
 from Acquisition import aq_inner
 from Acquisition import aq_parent
 from App.special_dtml import DTMLFile
@@ -229,66 +227,66 @@
         """ Perform the given workflow action on 'ob'.
         """
         wfs = self.getWorkflowsFor(ob)
         if wfs is None:
             wfs = ()
         if wf_id is None:
             if not wfs:
-                raise WorkflowException(_(u'No workflows found.'))
+                raise WorkflowException(_('No workflows found.'))
             found = 0
             for wf in wfs:
                 if wf.isActionSupported(ob, action, **kw):
                     found = 1
                     break
             if not found:
-                msg = _(u"No workflow provides the '${action_id}' action.",
+                msg = _("No workflow provides the '${action_id}' action.",
                         mapping={'action_id': action})
                 raise WorkflowException(msg)
         else:
             wf = self.getWorkflowById(wf_id)
             if wf is None:
                 raise WorkflowException(
-                    _(u'Requested workflow definition not found.'))
+                    _('Requested workflow definition not found.'))
         return self._invokeWithNotification(
             wfs, ob, action, wf.doActionFor, (ob, action) + args, kw)
 
     @security.public
     def getInfoFor(self, ob, name, default=_marker, wf_id=None, *args, **kw):
         """ Get the given bit of workflow information for the object.
         """
         if wf_id is None:
             wfs = self.getWorkflowsFor(ob)
             if wfs is None:
                 if default is _marker:
-                    raise WorkflowException(_(u'No workflows found.'))
+                    raise WorkflowException(_('No workflows found.'))
                 else:
                     return default
             found = 0
             for wf in wfs:
                 if wf.isInfoSupported(ob, name):
                     found = 1
                     break
             if not found:
                 if default is _marker:
-                    msg = _(u"No workflow provides '${name}' information.",
+                    msg = _("No workflow provides '${name}' information.",
                             mapping={'name': name})
                     raise WorkflowException(msg)
                 else:
                     return default
         else:
             wf = self.getWorkflowById(wf_id)
             if wf is None:
                 if default is _marker:
                     raise WorkflowException(
-                        _(u'Requested workflow definition not found.'))
+                        _('Requested workflow definition not found.'))
                 else:
                     return default
         res = wf.getInfoFor(ob, name, default, *args, **kw)
         if res is _marker:
-            msg = _(u'Could not get info: ${name}', mapping={'name': name})
+            msg = _('Could not get info: ${name}', mapping={'name': name})
             raise WorkflowException(msg)
         return res
 
     @security.private
     def notifyCreated(self, ob):
         """ Notify all applicable workflows that an object has been created.
         """
@@ -375,15 +373,15 @@
                                REQUEST=None):
         """ Set a chain for specific portal types.
         """
         cbt = self._chains_by_type
         if cbt is None:
             self._chains_by_type = cbt = PersistentMapping()
 
-        if isinstance(chain, six.string_types):
+        if isinstance(chain, str):
             if chain == '(Default)':
                 chain = None
             else:
                 chain = [wf.strip() for wf in chain.split(',') if wf.strip()]
 
         if chain is None:
             for type_id in pt_names:
@@ -412,15 +410,15 @@
         return cbt and sorted(cbt.items()) or ()
 
     @security.private
     def getChainFor(self, ob):
         """ Get the chain that applies to the given object.
         """
         cbt = self._chains_by_type
-        if isinstance(ob, six.string_types):
+        if isinstance(ob, str):
             pt = ob
         elif hasattr(aq_base(ob), 'getPortalTypeName'):
             pt = ob.getPortalTypeName()
         else:
             pt = None
 
         if pt is None:
@@ -611,15 +609,15 @@
 
 
 InitializeClass(WorkflowTool)
 registerToolInterface('portal_workflow', IWorkflowTool)
 
 
 @implementer(IWorkflowStatus)
-class DefaultWorkflowStatus(object):
+class DefaultWorkflowStatus:
     adapts(IWorkflowAware, IWorkflowDefinition)
 
     def __init__(self, context, workflow):
         self.context = aq_base(context)
         self.wf_id = workflow.getId()
 
     def get(self):
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/__init__.py` & `Products.CMFCore-3.0/src/Products/CMFCore/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/browser/actions.py` & `Products.CMFCore-3.0/src/Products/CMFCore/browser/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class ActionAddView(AddWithPresettingsViewBase):
 
     """Add view for Action.
     """
 
     klass = Action
 
-    description = u'An Action object represents a reference to an action.'
+    description = 'An Action object represents a reference to an action.'
 
     def getProfileInfos(self):
         profiles = []
         stool = queryUtility(ISetupTool)
         if stool:
             for info in stool.listContextInfos():
                 obj_ids = []
@@ -62,15 +62,15 @@
             if child.nodeName != 'object':
                 continue
             if child.getAttribute('meta_type') == self.klass.meta_type:
                 action_id = child.getAttribute('name')
                 action_paths.append(action_id)
             else:
                 action_paths += self._extractChildren(child)
-        return [('%s/%s' % (category_id, path)) for path in action_paths]
+        return [f'{category_id}/{path}' for path in action_paths]
 
     def _initSettings(self, obj, profile_id, obj_path):
         stool = queryUtility(ISetupTool)
         if stool is None:
             return
 
         context = stool._getImportContext(profile_id)
@@ -107,14 +107,14 @@
 
     """Add view for ActionCategory.
     """
 
     klass = ActionCategory
 
     description = \
-        u'An Action Category object represents a group of Action objects.'
+        'An Action Category object represents a group of Action objects.'
 
     def getProfileInfos(self):
         return []
 
     def _initSettings(self, obj, profile_id, obj_path):
         pass
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/browser/configure.zcml` & `Products.CMFCore-3.0/src/Products/CMFCore/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/browser/typeinfo.py` & `Products.CMFCore-3.0/src/Products/CMFCore/browser/typeinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class FactoryTypeInformationAddView(AddWithPresettingsViewBase):
 
     """Add view for FactoryTypeInformation.
     """
 
     klass = FactoryTypeInformation
 
-    description = u'A type information object defines a portal type.'
+    description = 'A type information object defines a portal type.'
 
     def getProfileInfos(self):
         profiles = []
         stool = queryUtility(ISetupTool)
         if stool:
             for info in stool.listContextInfos():
                 obj_ids = []
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/content.zcml` & `Products.CMFCore-3.0/src/Products/CMFCore/content.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/addCC.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/addCC.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/addFSDirView.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/addFSDirView.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/addInstance.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/addInstance.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/cachingPolicies.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/cachingPolicies.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/catalogFind.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/catalogFind.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/compareResults.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/compareResults.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/configureRegistrationTool.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/configureRegistrationTool.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/custdtml.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/custdtml.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/custfile.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/custfile.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/custimage.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/custimage.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/custprops.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/custprops.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/custpt.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/custpt.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/custpy.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/custpy.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/custstx.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/custstx.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/custzsql.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/custzsql.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/dirview_properties.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/dirview_properties.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/editToolsActions.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/editToolsActions.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/explainActionsTool.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/explainActionsTool.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/explainTypesTool.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/explainTypesTool.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/majorMinorWidget.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/majorMinorWidget.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/manageActionProviders.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/manageActionProviders.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/memberdataContents.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/memberdataContents.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/membershipRolemapping.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/membershipRolemapping.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/registryPredList.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/registryPredList.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/registryTest.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/registryTest.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/selectWorkflows.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/selectWorkflows.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/skinProps.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/skinProps.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/dtml/zmi_workflows.dtml` & `Products.CMFCore-3.0/src/Products/CMFCore/dtml/zmi_workflows.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/event.zcml` & `Products.CMFCore-3.0/src/Products/CMFCore/event.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exceptions.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,23 +15,18 @@
 """
 
 from AccessControl import ModuleSecurityInfo
 from AccessControl import Unauthorized as AccessControl_Unauthorized
 from OFS.CopySupport import CopyError
 from zExceptions import BadRequest
 from zExceptions import NotFound
+from zExceptions import ResourceLockedError
 from zExceptions import Unauthorized as zExceptions_Unauthorized
 
 
-try:
-    from zExceptions import ResourceLockedError
-except ImportError:
-    from webdav.Lockable import ResourceLockedError
-
-
 security = ModuleSecurityInfo('Products.CMFCore.exceptions')
 
 # Use AccessControl_Unauthorized to raise Unauthorized errors and
 # zExceptions_Unauthorized to catch them all.
 
 security.declarePublic('AccessControl_Unauthorized')
 security.declarePublic('BadRequest')
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/__init__.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/actions.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/actions.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/cachingpolicymgr.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/cachingpolicymgr.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/catalog.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/catalog.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/configure.zcml` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/content.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 #
 ##############################################################################
 """Filesystem exporter / importer adapters.
 """
 
 import itertools
 import operator
+from configparser import ConfigParser
 from csv import reader
 from csv import writer
-
-import six
-from six import StringIO
-from six.moves.configparser import ConfigParser
+from io import StringIO
 
 from DateTime import DateTime
 from zope.component import getUtility
 from zope.interface import implementer
 from zope.publisher.interfaces.http import MethodNotAllowed
 
 from Products.GenericSetup.content import DAVAwareFileAdapter
@@ -43,22 +41,18 @@
 
 
 def importSiteStructure(context):
     IFilesystemImporter(context.getSite()).import_(context, 'structure', True)
 
 
 def encode_if_needed(text, encoding):
-    if six.PY2:
-        if isinstance(text, six.text_type):
-            text = text.encode(encoding)
-    else:
-        if not isinstance(text, six.text_type):
-            text = text.decode(encoding)
-        # no need to encode;
-        # let's avoid double encoding in case of encoded string
+    if not isinstance(text, str):
+        text = text.decode(encoding)
+    # no need to encode;
+    # let's avoid double encoding in case of encoded string
     return text
 
 
 class FolderishDAVAwareFileAdapter(DAVAwareFileAdapter):
     """ A version of the DAVAwareFileAdapter that uses .properties to store
     the DAV result, rather than its own id. For use in serialising folderish
     objects. """
@@ -69,15 +63,15 @@
         return '.properties'
 
 
 #
 #   Filesystem export/import adapters
 #
 @implementer(IFilesystemExporter, IFilesystemImporter)
-class StructureFolderWalkingAdapter(object):
+class StructureFolderWalkingAdapter:
     """ Tree-walking exporter for "folderish" types.
 
     Folderish instances are mapped to directories within the 'structure'
     portion of the profile, where the folder's relative path within the site
     corresponds to the path of its directory under 'structure'.
 
     The subobjects of a folderish instance are enumerated in the '.objects'
@@ -123,15 +117,15 @@
 
         objects_stream = StringIO()
         objects_csv_writer = writer(objects_stream)
         wf_stream = StringIO()
         wf_csv_writer = writer(wf_stream)
 
         if not root:
-            subdir = '%s/%s' % (subdir, self.context.getId())
+            subdir = f'{subdir}/{self.context.getId()}'
 
         try:
             wft = self.context.portal_workflow
         except AttributeError:
             # No workflow tool to export definitions from
             for object_id, object, ignored in exportable:
                 objects_csv_writer.writerow((object_id,
@@ -191,29 +185,29 @@
                 adapter.export(export_context, subdir)
 
     def import_(self, import_context, subdir, root=False):
         """ See IFilesystemImporter.
         """
         context = self.context
         if not root:
-            subdir = '%s/%s' % (subdir, context.getId())
+            subdir = f'{subdir}/{context.getId()}'
 
         objects = self.read_data_file(import_context, '.objects', subdir)
         workflow_states = self.read_data_file(import_context,
                                               '.workflow_states', subdir)
         if objects is None:
             return
 
         dialect = 'excel'
         object_stream = StringIO(objects)
         wf_stream = StringIO(workflow_states)
 
         object_rowiter = reader(object_stream, dialect)
         ours = [_f for _f in tuple(object_rowiter) if _f]
-        our_ids = set([item[0] for item in ours])
+        our_ids = {item[0] for item in ours}
 
         prior = set(context.contentIds())
 
         preserve = self.read_data_file(import_context, '.preserve', subdir)
         if not preserve:
             preserve = set()
         else:
@@ -279,15 +273,15 @@
                     workflow.updateRoleMappingsFor(object)
 
                 object.reindexObject()
 
     def _makeInstance(self, id, portal_type, subdir, import_context):
 
         context = self.context
-        subdir = '%s/%s' % (subdir, id)
+        subdir = f'{subdir}/{id}'
         properties = self.read_data_file(import_context, '.properties',
                                          subdir)
         tool = getUtility(ITypesTool)
 
         try:
             tool.constructContent(portal_type, context, id)
         except ValueError:  # invalid type
@@ -306,18 +300,15 @@
                     pass
 
             lines = properties.splitlines()
 
             stream = StringIO('\n'.join(lines))
             parser = ConfigParser(defaults={'title': '',
                                             'description': 'NONE'})
-            try:
-                parser.read_file(stream)
-            except AttributeError:  # Python 2
-                parser.readfp(stream)
+            parser.read_file(stream)
 
             title = parser.get('DEFAULT', 'title')
             description = parser.get('DEFAULT', 'description')
 
             content.setTitle(title)
             content.setDescription(description)
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/contenttyperegistry.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/contenttyperegistry.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/cookieauth.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/cookieauth.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/mailhost.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/mailhost.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/memberdata.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/memberdata.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/properties.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/properties.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/skins.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/skins.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/__init__.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/conformance.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/conformance.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_actions.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -591,14 +591,15 @@
         context._files['actions.xml'] = _REMOVE_IMPORT
         importActionProviders(context)
 
         self.assertEqual(atool.listActionProviders(), ['portal_foo'])
 
 
 def test_suite():
+    loadTestsFromTestCase = unittest.defaultTestLoader.loadTestsFromTestCase
     return unittest.TestSuite((
-        unittest.makeSuite(ActionNodeAdapterTests),
-        unittest.makeSuite(ActionCategoryNodeAdapterTests),
-        unittest.makeSuite(ActionsToolXMLAdapterTests),
-        unittest.makeSuite(exportActionProvidersTests),
-        unittest.makeSuite(importActionProvidersTests),
-        ))
+        loadTestsFromTestCase(ActionNodeAdapterTests),
+        loadTestsFromTestCase(ActionCategoryNodeAdapterTests),
+        loadTestsFromTestCase(ActionsToolXMLAdapterTests),
+        loadTestsFromTestCase(exportActionProvidersTests),
+        loadTestsFromTestCase(importActionProvidersTests),
+    ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_cachingpolicymgr.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_cachingpolicymgr.py`

 * *Files 4% similar despite different names*

```diff
@@ -208,13 +208,14 @@
         self.assertEqual(policy.getNoTransform(), True)
         self.assertEqual(policy.getPublic(), True)
         self.assertEqual(policy.getPrivate(), True)
         self.assertEqual(policy.getEnable304s(), True)
 
 
 def test_suite():
+    loadTestsFromTestCase = unittest.defaultTestLoader.loadTestsFromTestCase
     return unittest.TestSuite((
-        unittest.makeSuite(CachingPolicyNodeAdapterTests),
-        unittest.makeSuite(CachingPolicyManagerXMLAdapterTests),
-        unittest.makeSuite(exportCachingPolicyManagerTests),
-        unittest.makeSuite(importCachingPolicyManagerTests),
-        ))
+        loadTestsFromTestCase(CachingPolicyNodeAdapterTests),
+        loadTestsFromTestCase(CachingPolicyManagerXMLAdapterTests),
+        loadTestsFromTestCase(exportCachingPolicyManagerTests),
+        loadTestsFromTestCase(importCachingPolicyManagerTests),
+    ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_catalog.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,10 +217,12 @@
         self.assertEqual(len(ctool.objectIds()), 1)
         self.assertEqual(len(ctool.indexes()), 2)
         self.assertEqual(len(ctool.schema()), 2)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(exportCatalogToolTests),
-        unittest.makeSuite(importCatalogToolTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            exportCatalogToolTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            importCatalogToolTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_content.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_content.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,33 +10,31 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Filesystem exporter / importer adapter unit tests.
 """
 
 import unittest
+from configparser import ConfigParser
 from csv import reader
-
-from six import StringIO
-from six import binary_type
-from six.moves.configparser import ConfigParser
+from io import StringIO
 
 from zope.component import getSiteManager
 from zope.testing.cleanup import cleanUp
 
 from Products.GenericSetup.tests.common import DummyExportContext
 from Products.GenericSetup.tests.common import DummyImportContext
 
 from ...interfaces import ITypesTool
 from ...testing import DummyWorkflow
 from .test_workflow import DummyWorkflowTool
 
 
 def safe_bytes(value, encoding='utf8'):
-    if isinstance(value, binary_type):
+    if isinstance(value, bytes):
         return value
     return value.encode(encoding)
 
 
 class SiteStructureExporterTests(unittest.TestCase):
 
     def _getExporter(self):
@@ -90,18 +88,15 @@
 
         provideAdapter(INIAwareFileAdapter,
                        (IINIAware,),
                        IFilesystemImporter)
 
     def _get_config_parser(self, text):
         parser = ConfigParser()
-        try:
-            parser.read_file(StringIO(text))
-        except AttributeError:  # Python 2
-            parser.readfp(StringIO(text))
+        parser.read_file(StringIO(text))
         return parser
 
     def tearDown(self):
         cleanUp()
 
     def test_export_empty_site(self):
         self._setUpAdapters()
@@ -196,16 +191,16 @@
     def test_export_site_with_exportable_simple_items_encoded_string(self):
         self._setUpAdapters()
         ITEM_IDS = ('foo', 'bar', 'baz')
 
         site = _makeFolder('site', site_folder=True)
         site.title = 'AAA'
         site.description = 'DESCRIPTION'
-        ITEMS_TITLE = u'Actualit\xe9'
-        ITEMS_DESCRIPTION = u'Actualit\xe9 r\xe9centes'
+        ITEMS_TITLE = 'Actualit\xe9'
+        ITEMS_DESCRIPTION = 'Actualit\xe9 r\xe9centes'
         for id in ITEM_IDS:
             site._setObject(id, _makeINIAware(id))
             item = getattr(site, id)
             item.setTitle(ITEMS_TITLE.encode('utf8'))
             item.setDescription(ITEMS_DESCRIPTION.encode('utf8'))
 
         context = DummyExportContext(site)
@@ -320,16 +315,16 @@
     def test_export_site_exportable_simple_items_unicode_default_charset(self):
         self._setUpAdapters()
         ITEM_IDS = ('foo', 'bar', 'baz')
 
         site = _makeFolder('site', site_folder=True)
         site.title = 'AAA'
         site.description = 'DESCRIPTION'
-        ITEMS_TITLE = u'Actualit\xe9'
-        ITEMS_DESCRIPTION = u'Actualit\xe9 r\xe9centes'
+        ITEMS_TITLE = 'Actualit\xe9'
+        ITEMS_DESCRIPTION = 'Actualit\xe9 r\xe9centes'
         for id in ITEM_IDS:
             site._setObject(id, _makeINIAware(id))
             item = getattr(site, id)
             item.setTitle(ITEMS_TITLE)
             item.setDescription(ITEMS_DESCRIPTION)
 
         context = DummyExportContext(site)
@@ -368,16 +363,16 @@
         self._setUpAdapters()
         ITEM_IDS = ('foo', 'bar', 'baz')
 
         site = _makeFolder('site', site_folder=True)
         site._setProperty('default_charset', 'iso-8859-1', 'string')
         site.title = 'AAA'
         site.description = 'DESCRIPTION'
-        ITEMS_TITLE = u'Actualit\xe9'
-        ITEMS_DESCRIPTION = u'Actualit\xe9 r\xe9centes'
+        ITEMS_TITLE = 'Actualit\xe9'
+        ITEMS_DESCRIPTION = 'Actualit\xe9 r\xe9centes'
         for id in ITEM_IDS:
             site._setObject(id, _makeINIAware(id))
             item = getattr(site, id)
             item.setTitle(ITEMS_TITLE)
             item.setDescription(ITEMS_DESCRIPTION)
 
         context = DummyExportContext(site)
@@ -569,16 +564,15 @@
         context = DummyImportContext(site)
 
         for id in FOLDER_IDS:
             context._files['structure/%s/.objects' % id] = ''
             context._files['structure/%s/.properties' % id] = (
                 _PROPERTIES_TEMPLATE % id)
 
-        _ROOT_OBJECTS = '\n'.join(['%s,%s' % (id, TEST_FOLDER)
-                                   for id in FOLDER_IDS])
+        _ROOT_OBJECTS = '\n'.join([f'{id},{TEST_FOLDER}' for id in FOLDER_IDS])
 
         context._files['structure/.objects'] = _ROOT_OBJECTS
         context._files['structure/.properties'] = (
                 _PROPERTIES_TEMPLATE % 'Test Site')
 
         importer = self._getImporter()
         importer(context)
@@ -597,15 +591,15 @@
         context = DummyImportContext(site)
 
         for id in FOLDER_IDS:
             context._files['structure/%s/.objects' % id] = ''
             context._files['structure/%s/.properties' % id] = (
                 KNOWN_DAV % ('Title', 'Description', 'Body'))
 
-        _ROOT_OBJECTS = '\n'.join(['%s,%s' % (id, TEST_DAV_FOLDER)
+        _ROOT_OBJECTS = '\n'.join([f'{id},{TEST_DAV_FOLDER}'
                                   for id in FOLDER_IDS])
 
         context._files['structure/.objects'] = _ROOT_OBJECTS
         context._files['structure/.properties'] = (
                 _PROPERTIES_TEMPLATE % 'Test Site')
 
         importer = self._getImporter()
@@ -627,15 +621,15 @@
         context = DummyImportContext(site)
 
         for id in FOLDER_IDS:
             context._files['structure/%s/.objects' % id] = ''
             context._files['structure/%s/.properties' % id] = (
                 _PROPERTIES_TEMPLATE % ('Sub Folder Title',))
 
-        _ROOT_OBJECTS = '\n'.join(['%s,%s' % (id, TEST_DAV_FOLDER)
+        _ROOT_OBJECTS = '\n'.join([f'{id},{TEST_DAV_FOLDER}'
                                    for id in FOLDER_IDS])
 
         context._files['structure/.objects'] = _ROOT_OBJECTS
         context._files['structure/.properties'] = (
                 _PROPERTIES_TEMPLATE % 'Test Site')
 
         importer = self._getImporter()
@@ -649,15 +643,15 @@
         ITEM_IDS = ('foo', 'bar', 'baz')
 
         site = _makeFolder('site', site_folder=True)
 
         context = DummyImportContext(site)
         # We want to add 'baz' to 'foo', without losing 'bar'
         context._files['structure/.objects'] = '\n'.join(
-                            ['%s,%s' % (x, TEST_INI_AWARE) for x in ITEM_IDS])
+            [f'{x},{TEST_INI_AWARE}' for x in ITEM_IDS])
         for index in range(len(ITEM_IDS)):
             id = ITEM_IDS[index]
             context._files[
                     'structure/%s.ini' % id] = KNOWN_INI % ('Title: %s' % id,
                                                             'xyzzy')
         importer = self._getImporter()
         importer(context)
@@ -679,17 +673,17 @@
         wftool.foo_workflow.state_var = 'state'
         wftool.setDefaultChain('foo_workflow')
         wftool.setChainForPortalTypes((TEST_INI_AWARE,),
                                       'foo_workflow', verify=False)
 
         context = DummyImportContext(site)
         context._files['structure/.objects'] = '\n'.join(
-                            ['%s,%s' % (x, TEST_INI_AWARE) for x in ITEM_IDS])
+            [f'{x},{TEST_INI_AWARE}' for x in ITEM_IDS])
         context._files['structure/.workflow_states'] = '\n'.join(
-                            ['%s,foo_workflow,draft' % (x) for x in ITEM_IDS])
+            ['%s,foo_workflow,draft' % (x) for x in ITEM_IDS])
         for index in range(len(ITEM_IDS)):
             id = ITEM_IDS[index]
             context._files[
                     'structure/%s.ini' % id] = KNOWN_INI % ('Title: %s' % id,
                                                             'xyzzy')
         importer = self._getImporter()
         importer(context)
@@ -702,15 +696,15 @@
         self._setUpAdapters()
         ITEM_IDS = ('foo', 'bar', 'baz')
 
         site = _makeFolder('site', site_folder=True)
 
         context = DummyImportContext(site)
         # We want to add 'baz' to 'foo', without losing 'bar'
-        correct = '\n'.join(['%s,%s' % (x, TEST_INI_AWARE) for x in ITEM_IDS])
+        correct = '\n'.join([f'{x},{TEST_INI_AWARE}' for x in ITEM_IDS])
         broken = correct + '\n\n'
         context._files['structure/.objects'] = broken
         for index in range(len(ITEM_IDS)):
             id = ITEM_IDS[index]
             context._files[
                     'structure/%s.ini' % id] = KNOWN_INI % ('Title: %s' % id,
                                                             'xyzzy')
@@ -773,15 +767,15 @@
         for id in ITEM_IDS:
             site._setObject(id, _makeItem(id))
             site._getOb(id).before = True
 
         context = DummyImportContext(site)
         # defined structure => object deleted and recreated
         context._files['structure/.objects'] = '\n'.join(
-            ['%s,%s' % (x, TEST_INI_AWARE) for x in ITEM_IDS])
+            [f'{x},{TEST_INI_AWARE}' for x in ITEM_IDS])
         for index in range(len(ITEM_IDS)):
             id = ITEM_IDS[index]
             context._files[
                     'structure/%s.ini' % id] = KNOWN_INI % ('Title: %s' % id,
                                                             'xyzzy')
 
         importer = self._getImporter()
@@ -798,15 +792,15 @@
         site = _makeFolder('site', site_folder=True)
         for id in ITEM_IDS:
             site._setObject(id, _makeINIAware(id))
             site._getOb(id).before = True
 
         context = DummyImportContext(site)
         context._files['structure/.objects'] = '\n'.join(
-            ['%s,%s' % (x, TEST_INI_AWARE) for x in ITEM_IDS])
+            [f'{x},{TEST_INI_AWARE}' for x in ITEM_IDS])
         for index in range(len(ITEM_IDS)):
             id = ITEM_IDS[index]
             context._files[
                     'structure/%s.ini' % id] = KNOWN_INI % ('Title: %s' % id,
                                                             'xyzzy')
         context._files['structure/.preserve'] = '*'
 
@@ -827,15 +821,15 @@
         site = _makeFolder('site', site_folder=True)
         for id in ITEM_IDS:
             site._setObject(id, _makeINIAware(id))
             site._getOb(id).before = True
 
         context = DummyImportContext(site)
         context._files['structure/.objects'] = '\n'.join(
-            ['%s,%s' % (x, TEST_INI_AWARE) for x in ITEM_IDS])
+            [f'{x},{TEST_INI_AWARE}' for x in ITEM_IDS])
         for index in range(len(ITEM_IDS)):
             id = ITEM_IDS[index]
             context._files[
                     'structure/%s.ini' % id] = KNOWN_INI % ('Title: %s' % id,
                                                             'xyzzy')
         context._files['structure/.preserve'] = 'b*'
 
@@ -857,15 +851,15 @@
         site = _makeFolder('site', site_folder=True)
         for id in ITEM_IDS:
             site._setObject(id, _makeINIAware(id))
             site._getOb(id).before = True
 
         context = DummyImportContext(site)
         context._files['structure/.objects'] = '\n'.join(
-            ['%s,%s' % (x, TEST_INI_AWARE) for x in ITEM_IDS[:-1]])
+            [f'{x},{TEST_INI_AWARE}' for x in ITEM_IDS[:-1]])
         for index in range(len(ITEM_IDS)):
             id = ITEM_IDS[index]
             context._files[
                     'structure/%s.ini' % id] = KNOWN_INI % ('Title: %s' % id,
                                                             'xyzzy')
         context._files['structure/.preserve'] = 'foo'
         context._files['structure/.delete'] = 'baz'
@@ -1117,13 +1111,7 @@
         ttool._setObject(TEST_INI_AWARE, _TypeInfo(TEST_INI_AWARE))
         ttool._setObject(TEST_CONTENT, _TypeInfo(TEST_CONTENT))
         ttool._setObject(TEST_FOLDER, _TypeInfo(TEST_FOLDER))
         ttool._setObject(TEST_DAV_FOLDER, _TypeInfo(TEST_DAV_FOLDER))
         getSiteManager().registerUtility(ttool, ITypesTool)
 
     return folder
-
-
-def test_suite():
-    suite = unittest.TestSuite()
-    suite.addTest(unittest.makeSuite(SiteStructureExporterTests))
-    return suite
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_contenttyperegistry.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_contenttyperegistry.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,48 +122,36 @@
     NAME_REGEX_TYPENAME = _TEST_PREDICATES[3][3]
 
     _EMPTY_EXPORT = """\
 <?xml version="1.0" encoding="utf-8"?>
 <object name="content_type_registry" meta_type="Content Type Registry"/>
 """
 
-    _WITH_POLICY_EXPORT = """\
+    _WITH_POLICY_EXPORT = f"""\
 <?xml version="1.0"  encoding="utf-8"?>
 <object name="content_type_registry" meta_type="Content Type Registry">
- <predicate name="%s" content_type_name="%s"
+ <predicate name="{MAJOR_MINOR_ID}" content_type_name="{MAJOR_MINOR_TYPENAME}"
     predicate_type="major_minor">
-  <argument value="%s"/>
-  <argument value="%s"/>
+  <argument value="{MAJOR}"/>
+  <argument value="{MINOR}"/>
  </predicate>
- <predicate name="%s" content_type_name="%s"
+ <predicate name="{EXTENSION_ID}" content_type_name="{EXTENSION_TYPENAME}"
     predicate_type="extension">
-  <argument value="%s"/>
+  <argument value="{EXTENSIONS}"/>
  </predicate>
- <predicate name="%s" content_type_name="%s"
+ <predicate name="{MIMETYPE_REGEX_ID}" content_type_name="{MIMETYPE_REGEX_TYPENAME}"
     predicate_type="mimetype_regex">
-  <argument value="%s"/>
+  <argument value="{MIMETYPE_REGEX}"/>
  </predicate>
- <predicate name="%s" content_type_name="%s"
+ <predicate name="{NAME_REGEX_ID}" content_type_name="{NAME_REGEX_TYPENAME}"
     predicate_type="name_regex">
-  <argument value="%s"/>
+  <argument value="{NAME_REGEX}"/>
  </predicate>
 </object>
-""" % (MAJOR_MINOR_ID,
-       MAJOR_MINOR_TYPENAME,
-       MAJOR,
-       MINOR,
-       EXTENSION_ID,
-       EXTENSION_TYPENAME,
-       EXTENSIONS,
-       MIMETYPE_REGEX_ID,
-       MIMETYPE_REGEX_TYPENAME,
-       MIMETYPE_REGEX,
-       NAME_REGEX_ID,
-       NAME_REGEX_TYPENAME,
-       NAME_REGEX)
+"""  # NOQA: E501 line too long
 
     def _initSite(self, mit_predikat=False):
         from ...ContentTypeRegistry import ContentTypeRegistry
 
         site = Folder(id='site').__of__(self.app)
         ctr = ContentTypeRegistry()
         getSiteManager().registerUtility(ctr, IContentTypeRegistry)
@@ -280,12 +268,13 @@
 
         self.assertEqual(len(ctr.listPredicates()), len(_TEST_PREDICATES))
         self.assertEqual(ctr.predicate_ids, ('stylesheets', 'plain_text',
                                              'logfiles', 'images'))
 
 
 def test_suite():
+    loadTestsFromTestCase = unittest.defaultTestLoader.loadTestsFromTestCase
     return unittest.TestSuite((
-        unittest.makeSuite(ContentTypeRegistryXMLAdapterTests),
-        unittest.makeSuite(exportContentTypeRegistryTests),
-        unittest.makeSuite(importContentTypeRegistryTests),
-        ))
+        loadTestsFromTestCase(ContentTypeRegistryXMLAdapterTests),
+        loadTestsFromTestCase(exportContentTypeRegistryTests),
+        loadTestsFromTestCase(importContentTypeRegistryTests),
+    ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_cookieauth.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_cookieauth.py`

 * *Files 5% similar despite different names*

```diff
@@ -190,12 +190,13 @@
         self.assertEqual(cc.log_username, 0)
         self.assertEqual(cc.persist_cookie, 'value4')
         self.assertEqual(cc.pw_cookie, 'value5')
         self.assertEqual(cc.local_cookie_path, 1)
 
 
 def test_suite():
+    loadTestsFromTestCase = unittest.defaultTestLoader.loadTestsFromTestCase
     return unittest.TestSuite((
-        unittest.makeSuite(CookieCrumblerXMLAdapterTests),
-        unittest.makeSuite(exportCookieCrumblerTests),
-        unittest.makeSuite(importCookieCrumblerTests),
-        ))
+        loadTestsFromTestCase(CookieCrumblerXMLAdapterTests),
+        loadTestsFromTestCase(exportCookieCrumblerTests),
+        loadTestsFromTestCase(importCookieCrumblerTests),
+    ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_mailhost.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_mailhost.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,10 +133,10 @@
         self.assertEqual(mh.smtp_port, 1)
         self.assertEqual(mh.smtp_queue, False)
         self.assertEqual(mh.smtp_queue_directory, '/tmp')
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(exportMailHostTests),
-        unittest.makeSuite(importMailHostTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(exportMailHostTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(importMailHostTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_memberdata.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_memberdata.py`

 * *Files 13% similar despite different names*

```diff
@@ -148,12 +148,13 @@
         self.assertEqual(mdtool.portal_skin, 'value2')
         self.assertEqual(mdtool.listed, True)
         self.assertEqual(mdtool.login_time, DateTime('2010/01/01'))
         self.assertEqual(mdtool.last_login_time, DateTime('2010/01/01'))
 
 
 def test_suite():
+    loadTestsFromTestCase = unittest.defaultTestLoader.loadTestsFromTestCase
     return unittest.TestSuite((
-        unittest.makeSuite(MemberDataToolXMLAdapterTests),
-        unittest.makeSuite(exportMemberDataToolTests),
-        unittest.makeSuite(importMemberDataToolTests),
-        ))
+        loadTestsFromTestCase(MemberDataToolXMLAdapterTests),
+        loadTestsFromTestCase(exportMemberDataToolTests),
+        loadTestsFromTestCase(importMemberDataToolTests),
+    ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_properties.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_properties.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 #
 ##############################################################################
 """Site properties xml adapter and setup handler unit tests.
 """
 
 import unittest
 
-import six
-
 from Products.GenericSetup.testing import BodyAdapterTestCase
 from Products.GenericSetup.tests.common import BaseRegistryTests
 from Products.GenericSetup.tests.common import DummyExportContext
 from Products.GenericSetup.tests.common import DummyImportContext
 
 from ...testing import ExportImportZCMLLayer
 
@@ -67,15 +65,15 @@
 
         return PropertiesXMLAdapter
 
     def _populate(self, obj):
         obj._setPropValue('title', 'Foo')
         obj._setProperty('default_charset', 'iso-8859-1', 'string')
         obj._setProperty('foo_string', 'foo', 'string')
-        obj._setProperty('bar_string', u'B\xe4r'.encode('iso-8859-1'),
+        obj._setProperty('bar_string', b'B\xe4r',
                          'string')
         obj._setProperty('foo_boolean', False, 'boolean')
 
     def _verifyImport(self, obj):
         self.assertIsInstance(obj.default_charset, str)
         self.assertEqual(obj.default_charset, 'iso-8859-1')
         self.assertIsInstance(obj.title, str)
@@ -229,23 +227,20 @@
 
     layer = ExportImportZCMLLayer
 
     def test_nonascii_no_default_charset(self):
         from ..properties import exportSiteProperties
         from ..properties import importSiteProperties
 
-        NONASCII = u'B\xe4r'
+        NONASCII = 'B\xe4r'
         site = self._initSite(foo=0, bar=0)
         site._updateProperty('title', NONASCII)
 
         self.assertIsInstance(site.title, str)
-        self.assertEqual(
-            site.title,
-            b'B\xc3\xa4r' if six.PY2 else u'B\xe4r',
-        )
+        self.assertEqual(site.title, 'B\xe4r')
 
         # export the site properties
         context = DummyExportContext(site)
         exportSiteProperties(context)
         _filename, text, _content_type = context._wrote[0]
 
         # Clear the title property
@@ -253,20 +248,18 @@
         self.assertEqual(site.title, '')
 
         # Import from the previous export
         context = DummyImportContext(site)
         context._files['properties.xml'] = text
         importSiteProperties(context)
 
-        self.assertEqual(
-            site.title,
-            b'B\xc3\xa4r' if six.PY2 else u'B\xe4r',
-        )
+        self.assertEqual(site.title, 'B\xe4r')
 
 
 def test_suite():
+    loadTestsFromTestCase = unittest.defaultTestLoader.loadTestsFromTestCase
     return unittest.TestSuite((
-        unittest.makeSuite(PropertiesXMLAdapterTests),
-        unittest.makeSuite(exportSitePropertiesTests),
-        unittest.makeSuite(importSitePropertiesTests),
-        unittest.makeSuite(roundtripSitePropertiesTests),
-        ))
+        loadTestsFromTestCase(PropertiesXMLAdapterTests),
+        loadTestsFromTestCase(exportSitePropertiesTests),
+        loadTestsFromTestCase(importSitePropertiesTests),
+        loadTestsFromTestCase(roundtripSitePropertiesTests),
+    ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_skins.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_skins.py`

 * *Files 1% similar despite different names*

```diff
@@ -643,13 +643,14 @@
         skin_paths = skins_tool.getSkinPaths()
         self.assertEqual(len(skin_paths), 1)
         self.assertEqual(skin_paths[0], ('existing', 'one,two,three,four'))
         self.assertEqual(len(skins_tool.objectItems()), 4)
 
 
 def test_suite():
+    loadTestsFromTestCase = unittest.defaultTestLoader.loadTestsFromTestCase
     return unittest.TestSuite((
-        unittest.makeSuite(DirectoryViewAdapterTests),
-        unittest.makeSuite(SkinsToolXMLAdapterTests),
-        unittest.makeSuite(exportSkinsToolTests),
-        unittest.makeSuite(importSkinsToolTests),
-        ))
+        loadTestsFromTestCase(DirectoryViewAdapterTests),
+        loadTestsFromTestCase(SkinsToolXMLAdapterTests),
+        loadTestsFromTestCase(exportSkinsToolTests),
+        loadTestsFromTestCase(importSkinsToolTests),
+    ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_typeinfo.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_typeinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -697,13 +697,14 @@
         self.assertTrue('baz' in tool.objectIds())
         baz = tool['baz']
         actions = baz.listActions()
         self.assertEqual(len(actions), 0)
 
 
 def test_suite():
+    loadTestsFromTestCase = unittest.defaultTestLoader.loadTestsFromTestCase
     return unittest.TestSuite((
-        unittest.makeSuite(TypeInformationXMLAdapterTests),
-        unittest.makeSuite(TypesToolXMLAdapterTests),
-        unittest.makeSuite(exportTypesToolTests),
-        unittest.makeSuite(importTypesToolTests),
-        ))
+        loadTestsFromTestCase(TypeInformationXMLAdapterTests),
+        loadTestsFromTestCase(TypesToolXMLAdapterTests),
+        loadTestsFromTestCase(exportTypesToolTests),
+        loadTestsFromTestCase(importTypesToolTests),
+    ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/tests/test_workflow.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/tests/test_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,12 +368,13 @@
         self.assertEqual(len(wf_tool.objectIds()), 4)
         self.assertEqual(len(wf_tool._default_chain), 1)
         self.assertEqual(wf_tool._default_chain[0], WF_ID_NON % 1)
         self.assertEqual(len(wf_tool._chains_by_type), 0)
 
 
 def test_suite():
+    loadTestsFromTestCase = unittest.defaultTestLoader.loadTestsFromTestCase
     return unittest.TestSuite((
-        unittest.makeSuite(WorkflowToolXMLAdapterTests),
-        unittest.makeSuite(exportWorkflowToolTests),
-        unittest.makeSuite(importWorkflowToolTests),
-        ))
+        loadTestsFromTestCase(WorkflowToolXMLAdapterTests),
+        loadTestsFromTestCase(exportWorkflowToolTests),
+        loadTestsFromTestCase(importWorkflowToolTests),
+    ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/typeinfo.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/typeinfo.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/exportimport/workflow.py` & `Products.CMFCore-3.0/src/Products/CMFCore/exportimport/workflow.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/help/Actions.stx` & `Products.CMFCore-3.0/src/Products/CMFCore/help/Actions.stx`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/help/CPMPolicies.stx` & `Products.CMFCore-3.0/src/Products/CMFCore/help/CPMPolicies.stx`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/indexing.py` & `Products.CMFCore-3.0/src/Products/CMFCore/indexing.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 debug = logger.debug
 
 localQueue = None
 processing = set()
 
 
 @implementer(IPortalCatalogQueueProcessor)
-class PortalCatalogProcessor(object):
+class PortalCatalogProcessor:
     """An index queue processor for the standard portal catalog via
        the `CatalogMultiplex` and `CMFCatalogAware` mixin classes """
 
     def index(self, obj, attributes=None):
         catalog = getToolByName(obj, 'portal_catalog', None)
         if catalog is not None:
             catalog._indexObject(obj)
@@ -68,15 +68,15 @@
     @staticmethod
     def get_dispatcher(obj, name):
         """ return named indexing method according on the used mixin class """
         warn('get_dispatcher is deprecated and will be removed in version 2.5')
         catalog = getToolByName(obj, 'portal_catalog', None)
         if catalog is None:
             return
-        attr = getattr(catalog, '_{0}'.format(name), None)
+        attr = getattr(catalog, f'_{name}', None)
         if attr is None:
             return
         return attr.__func__
 
 
 def getQueue():
     """ return a (thread-local) queue object, create one if necessary """
@@ -99,15 +99,15 @@
             processing.remove(queue)
     return processed
 
 
 class PathProxy(ProxyBase):
 
     def __init__(self, obj):
-        super(PathProxy, self).__init__(obj)
+        super().__init__(obj)
         self._old_path = obj.getPhysicalPath()
 
     @non_overridable
     def getPhysicalPath(self):
         return self._old_path
 
 
@@ -272,15 +272,15 @@
             if obj.isTemporary():
                 return None
         except TypeError:
             return None  # `isTemporary` on the `FactoryTool` expects 2 args
     return obj
 
 
-class QueueSavepoint(object):
+class QueueSavepoint:
     """ transaction savepoints using the IIndexQueue interface """
 
     def __init__(self, queue):
         self.queue = queue
         self.state = queue.getState()
 
     def rollback(self):
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/interfaces/__init__.py` & `Products.CMFCore-3.0/src/Products/CMFCore/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/interfaces/_content.py` & `Products.CMFCore-3.0/src/Products/CMFCore/interfaces/_content.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/interfaces/_cookieCrumbler.py` & `Products.CMFCore-3.0/src/Products/CMFCore/interfaces/_cookieCrumbler.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/interfaces/_events.py` & `Products.CMFCore-3.0/src/Products/CMFCore/interfaces/_events.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/interfaces/_tools.py` & `Products.CMFCore-3.0/src/Products/CMFCore/interfaces/_tools.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/namespace.py` & `Products.CMFCore-3.0/src/Products/CMFCore/namespace.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from zope.traversing.interfaces import ITraversable
 
 from .interfaces import IFolderish
 from .interfaces import ITypesTool
 
 
 @implementer(ITraversable)
-class AddViewTraverser(object):
+class AddViewTraverser:
 
     """Add view traverser.
     """
 
     adapts(IFolderish, Interface)
 
     def __init__(self, context, request):
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/permissions.py` & `Products.CMFCore-3.0/src/Products/CMFCore/permissions.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/permissions.zcml` & `Products.CMFCore-3.0/src/Products/CMFCore/permissions.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/subscribers.py` & `Products.CMFCore-3.0/src/Products/CMFCore/subscribers.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/subscribers.zcml` & `Products.CMFCore-3.0/src/Products/CMFCore/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/testing.py` & `Products.CMFCore-3.0/src/Products/CMFCore/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,18 +29,15 @@
 from .interfaces import IWorkflowDefinition
 from .utils import HAS_ZSERVER
 
 
 class ConformsToFolder:
 
     def test_conforms_to_IWritelock(self):
-        try:
-            from OFS.interfaces import IWriteLock
-        except ImportError:
-            from webdav.interfaces import IWriteLock
+        from OFS.interfaces import IWriteLock
         verifyClass(IWriteLock, self._getTargetClass())
 
     def test_conforms_to_IDynamicType(self):
         from .interfaces import IDynamicType
         verifyClass(IDynamicType, self._getTargetClass())
 
     def test_conforms_to_IFolderish(self):
@@ -85,15 +82,15 @@
 
         verifyClass(ICatalogAware, self._getTargetClass())
         verifyClass(IOpaqueItemManager, self._getTargetClass())
         verifyClass(IWorkflowAware, self._getTargetClass())
 
 
 @implementer(IUserPreferredLanguages)
-class BrowserLanguages(object):
+class BrowserLanguages:
 
     adapts(IHTTPRequest)
 
     def __init__(self, context):
         self.context = context
 
     def getPreferredLanguages(self):
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/testing.zcml` & `Products.CMFCore-3.0/src/Products/CMFCore/testing.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/base/content.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/base/content.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/base/dummy.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/base/dummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,18 +64,18 @@
         while path_elements:
             path_element = path_elements.pop()
             parent = getattr(parent, path_element)
 
         return parent
 
     def icon(self):
-        return '%s ICON' % self._id
+        return f'{self._id} ICON'
 
     def getIconURL(self):
-        return '%s ICON' % self._id
+        return f'{self._id} ICON'
 
     def getId(self):
         return self._id
 
 
 @implementer(ITypeInformation)
 class DummyType(DummyObject):
@@ -203,15 +203,15 @@
         self._folder = folder
 
     def getId(self):
         return 'DummyFactoryDispatcher'
 
     def addFoo(self, id, *args, **kw):
         if getattr(self._folder, '_prefix', None):
-            id = '%s_%s' % (self._folder._prefix, id)
+            id = f'{self._folder._prefix}_{id}'
         foo = DummyContent(id, *args, **kw)
         self._folder._setObject(id, foo, suppress_events=True)
         if getattr(self._folder, '_prefix', None):
             return id
 
     __roles__ = ('FooAdder',)
     __allow_access_to_unprotected_subobjects__ = {'addFoo': 1}
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/base/security.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/base/security.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """ Unit test security.
 """
 
-import six
-
 from AccessControl.interfaces import IUser
 from AccessControl.PermissionRole import rolesForPermissionOn
 from Acquisition import Implicit
 from zope.interface import implementer
 
 
 class PermissiveSecurityPolicy:
@@ -34,15 +32,15 @@
         if name and name.startswith('hidden'):
             return False
         else:
             return True
 
     def checkPermission(self, permission, object, context):
         roles = rolesForPermissionOn(permission, object)
-        if isinstance(roles, six.string_types):
+        if isinstance(roles, str):
             roles = [roles]
         return context.user.allowed(object, roles)
 
 
 @implementer(IUser)
 class _BaseUser(Implicit):
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/base/testcase.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/base/testcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         if ignore is None:
             from ...DirectoryView import ignore
         filepath = join(self.tempname, self._skinname)
         subpath = basename(self.tempname)
         if subpath != 'tests':
             # we have a temp dir in tests
             subpath = 'tests/%s' % subpath
-        reg_key = 'Products.CMFCore:%s/%s' % (subpath, self._skinname)
+        reg_key = f'Products.CMFCore:{subpath}/{self._skinname}'
         _dirreg.registerDirectoryByKey(filepath, reg_key, ignore=ignore)
         if obj is not None:
             ob = obj.ob = DummyFolder()
             info = _dirreg.getDirectoryInfo(reg_key)
             for entry in info.getSubdirs():
                 entry_reg_key = '/'.join((reg_key, entry))
                 createDirectoryView(ob, entry_reg_key, entry)
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/base/tidata.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/base/tidata.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file.swf` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file.swf`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file_two.swf` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file_two.swf`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_ActionInformation.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_ActionInformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,18 +154,28 @@
         a.manage_changeProperties(
             icon_expr='', url_expr='', available_expr='')
         self.assertFalse(hasattr(a, 'icon_expr_object'))
         self.assertFalse(hasattr(a, 'url_expr_object'))
         self.assertFalse(hasattr(a, 'available_expr_object'))
 
 
+class DummyResponse:
+
+    def getHeader(self, key):
+        return ''
+
+    def setHeader(self, key, value):
+        pass
+
+
 class DummyRequest:
 
     charset = 'UTF-8'
     URL = ''
+    RESPONSE = DummyResponse()
 
     def __init__(self):
         self._data = {}
 
     def set(self, k, v):
         self._data[k] = v
 
@@ -504,17 +514,7 @@
                    'description': 'Foo description.', 'id': 'foo',
                    'permissions': ('View',), 'title': 'Foo Title',
                    'url': a._getActionObject(), 'visible': False,
                    'icon': a._getIconExpressionObject(),
                    'link_target': a.link_target},
                   ['url', 'icon'])
         self.assertEqual(a.getInfoData(), WANTED)
-
-
-def test_suite():
-    return unittest.TestSuite((
-        unittest.makeSuite(ActionCategoryTests),
-        unittest.makeSuite(ActionTests),
-        unittest.makeSuite(ActionInfoTests),
-        unittest.makeSuite(ActionInfoSecurityTests),
-        unittest.makeSuite(ActionInformationTests),
-        ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_ActionProviderBase.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_ActionProviderBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """ Unit tests for ActionProviderBase module.
 """
-
-import unittest
 import warnings
 
 from zope.component import getSiteManager
 from zope.interface.verify import verifyClass
 from zope.testing.cleanup import cleanUp
 
 #   We have to import these here to make the "ugly sharing" test case go.
@@ -274,16 +272,9 @@
             # The following is nasty, but I want to make sure the ValueError
             # carries some useful information
             INVALID_ID = 'invalid_id'
             try:
                 rval = apb.getActionInfo('object/%s' % INVALID_ID)
             except ValueError as e:
                 message = e.args[0]
-                detail = '"%s" does not offer action "%s"' % (message,
-                                                              INVALID_ID)
+                detail = f'"{message}" does not offer action "{INVALID_ID}"'
                 self.assertTrue(message.find(INVALID_ID) != -1, detail)
-
-
-def test_suite():
-    return unittest.TestSuite((
-        unittest.makeSuite(ActionProviderBaseTests),
-        ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_ActionsTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_ActionsTool.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,10 +181,11 @@
             warnings.simplefilter('ignore')
             self.assertEqual(tool.listFilteredActionsFor(self.app.foo),
                              expected)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(ActionsToolTests),
-        unittest.makeSuite(ActionsToolSecurityTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(ActionsToolTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            ActionsToolSecurityTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_CMFBTreeFolder.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_CMFBTreeFolder.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,9 +31,9 @@
     def test_empty(self):
         empty = self._makeOne('test')
         self.assertEqual(len(empty.objectIds()), 0)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(CMFBTreeFolderTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(CMFBTreeFolderTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_CMFCatalogAware.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_CMFCatalogAware.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,10 +355,11 @@
 
         site.manage_renameObject(id='bar', new_id='baz')
         self.assertEqual(cat.log, ['unindex /site/bar', 'index /site/baz'])
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(CMFCatalogAwareTests),
-        unittest.makeSuite(CMFCatalogAware_CopySupport_Tests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(CMFCatalogAwareTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            CMFCatalogAware_CopySupport_Tests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_CachingPolicyManager.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_CachingPolicyManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1297,13 +1297,15 @@
         self.assertTrue(headers.get('x-cache-headers-set-by'))
         self.assertEqual(headers.get('vary'), 'doc1')
         self.assertEqual(headers.get('cache-control'), 'max-age=100')
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(CachingPolicyTests),
-        unittest.makeSuite(CachingPolicyManagerTests),
-        unittest.makeSuite(CachingPolicyManager304Tests),
-        unittest.makeSuite(NestedTemplateTests),
-        unittest.makeSuite(OFSCacheTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(CachingPolicyTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            CachingPolicyManagerTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            CachingPolicyManager304Tests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(NestedTemplateTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(OFSCacheTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_CatalogIndexing.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_CatalogIndexing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from threading import Thread
-from threading import currentThread
+from threading import current_thread
 from time import sleep
 from unittest import TestCase
 
 from Acquisition import Implicit
 from transaction import abort
 from transaction import commit
 from transaction import savepoint
@@ -21,15 +21,15 @@
 from ..interfaces import IIndexQueue
 from ..interfaces import IIndexQueueProcessor
 from .base.dummy import DummyContent
 from .base.dummy import DummyFolder
 
 
 @implementer(IIndexing)
-class MockIndexer(object):
+class MockIndexer:
 
     def __init__(self):
         self.queue = []
 
     def index(self, obj, attributes=None):
         self.queue.append((INDEX, obj, attributes))
 
@@ -45,23 +45,23 @@
 
     processed = None
 
     def hook(self):
         pass
 
     def index(self, obj, attributes=None):
-        super(MockQueue, self).index(obj, attributes)
+        super().index(obj, attributes)
         self.hook()
 
     def reindex(self, obj, attributes=None, update_metadata=1):
-        super(MockQueue, self).reindex(obj, attributes)
+        super().reindex(obj, attributes)
         self.hook()
 
     def unindex(self, obj):
-        super(MockQueue, self).unindex(obj)
+        super().unindex(obj)
         self.hook()
 
     def getState(self):
         return list(self.queue)     # better return a copy... :)
 
     def setState(self, state):
         self.queue = state
@@ -102,15 +102,15 @@
     def tearDown(self):
         self.queue.clear()
 
     def testInterface(self):
         self.assertTrue(IIndexQueue.providedBy(self.queue))
 
     def testQueueHook(self):
-        class CaptainHook(object):
+        class CaptainHook:
             def __init__(self):
                 self.hooked = 0
 
             def __call__(self):
                 self.hooked += 1
 
         hook = CaptainHook()
@@ -396,15 +396,15 @@
         me = self.me                    # get the queued indexer...
         queues = {}                     # container for local queues
 
         def makeRunner(name, idx):
             def runner():
                 for n in range(idx):    # index idx times
                     me.index(name)
-                queues[currentThread()] = me.queue
+                queues[current_thread()] = me.queue
             return runner
 
         threads = []
         for idx in range(99):
             threads.append(Thread(target=makeRunner('t%d' % idx, idx)))
         for thread in threads:
             thread.start()
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_CatalogTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_CatalogTool.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,10 +586,11 @@
         ctool.catalog_object(dummy, '/dummy')
         query = {'meta_type': 'Dummy'}
         self.assertEqual(1, len(ctool._catalog.searchResults(query)))
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(IndexableObjectWrapperTests),
-        unittest.makeSuite(CatalogToolTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            IndexableObjectWrapperTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(CatalogToolTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_ContentTypeRegistry.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_ContentTypeRegistry.py`

 * *Files 3% similar despite different names*

```diff
@@ -224,14 +224,15 @@
                                           'asdfljksadf'))
         self.assertFalse(reg.findTypeName('bar', 'text/plain', 'asdfljksadf'))
         self.assertEqual(reg.findTypeName('foo', '', ''), 'Foo')
         self.assertEqual(reg.findTypeName('foo', None, None), 'Foo')
 
 
 def test_suite():
+    loadTestsFromTestCase = unittest.defaultTestLoader.loadTestsFromTestCase
     return unittest.TestSuite((
-        unittest.makeSuite(MajorMinorPredicateTests),
-        unittest.makeSuite(ExtensionPredicateTests),
-        unittest.makeSuite(MimeTypeRegexPredicateTests),
-        unittest.makeSuite(NameRegexPredicateTests),
-        unittest.makeSuite(ContentTypeRegistryTests),
-        ))
+        loadTestsFromTestCase(MajorMinorPredicateTests),
+        loadTestsFromTestCase(ExtensionPredicateTests),
+        loadTestsFromTestCase(MimeTypeRegexPredicateTests),
+        loadTestsFromTestCase(NameRegexPredicateTests),
+        loadTestsFromTestCase(ContentTypeRegistryTests),
+    ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_CookieCrumbler.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_CookieCrumbler.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """CookieCrumbler tests.
 """
 
 import unittest
-
-from six import StringIO
-from six.moves.urllib.parse import quote
+from io import StringIO
+from urllib.parse import quote
 
 from zope.component import eventtesting
 from zope.interface.verify import verifyClass
 from zope.testing.cleanup import cleanUp
 
 from ..utils import base64_encode
 
@@ -253,18 +252,12 @@
 
         bt_removed = getattr(container, '__before_traverse__')
         self.assertEqual(len(bt_removed.items()), 0)
 
 
 # compatibility
 try:
-    # Zope 4.8+/5.5+
+    # Zope 5.5+
     from ZPublisher.cookie import normalizeCookieParameterName
 except ImportError:
     def normalizeCookieParameterName(name):
         return name
-
-
-def test_suite():
-    return unittest.TestSuite((
-        unittest.makeSuite(CookieCrumblerTests),
-        ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_DirectoryView.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_DirectoryView.py`

 * *Files 4% similar despite different names*

```diff
@@ -302,13 +302,14 @@
                          self.use_dir_mtime)
         self._deleteDirectory('test_directory', self.use_dir_mtime)
         self.assertFalse(hasattr(self.ob.fake_skin, 'test_directory'))
 
 
 def test_suite():
     suite = unittest.TestSuite()
-    suite.addTest(unittest.makeSuite(DirectoryViewPathTests))
-    suite.addTest(unittest.makeSuite(DirectoryViewTests))
-    suite.addTest(unittest.makeSuite(DirectoryViewIgnoreTests))
-    suite.addTest(unittest.makeSuite(DirectoryViewFolderTests))
-    suite.addTest(unittest.makeSuite(DebugModeTests))
+    loadTestsFromTestCase = unittest.defaultTestLoader.loadTestsFromTestCase
+    suite.addTest(loadTestsFromTestCase(DirectoryViewPathTests))
+    suite.addTest(loadTestsFromTestCase(DirectoryViewTests))
+    suite.addTest(loadTestsFromTestCase(DirectoryViewIgnoreTests))
+    suite.addTest(loadTestsFromTestCase(DirectoryViewFolderTests))
+    suite.addTest(loadTestsFromTestCase(DebugModeTests))
     return suite
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_DiscussionTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_DiscussionTool.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,10 +36,10 @@
         from ..interfaces import IOldstyleDiscussable
 
         verifyClass(IOldstyleDiscussable, OldDiscussable)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(DiscussionToolTests),
-        unittest.makeSuite(OldDiscussableTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(DiscussionToolTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(OldDiscussableTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_DynamicType.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_DynamicType.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """ Unit tests for DynamicType module.
 """
 
 import unittest
-
-from six import StringIO
+from io import StringIO
 
 from Acquisition import Implicit
 from zope.component import getSiteManager
 from zope.component import provideAdapter
 from zope.interface import alsoProvides
 from zope.interface.verify import verifyClass
 from zope.publisher.browser import BrowserView
+from zope.publisher.interfaces import IDefaultViewName
 from zope.publisher.interfaces.browser import IBrowserRequest
 from zope.publisher.interfaces.browser import IBrowserView
 from zope.testing.cleanup import cleanUp
 from ZPublisher.HTTPRequest import HTTPRequest
 from ZPublisher.HTTPResponse import HTTPResponse
 
 from ..DynamicType import DynamicType
@@ -38,20 +38,14 @@
 from .base.dummy import DummyObject
 from .base.dummy import DummySite
 from .base.dummy import DummyTool
 from .base.testcase import SecurityTest
 from .base.tidata import FTIDATA_CMF
 
 
-try:
-    from zope.publisher.interfaces import IDefaultViewName
-except ImportError:  # BBB: zope.component had this before the ZTK
-    from zope.component.interfaces import IDefaultViewName
-
-
 def defineDefaultViewName(name, for_=None):
     provideAdapter(name, (for_, IBrowserRequest), IDefaultViewName, '')
 
 
 class DummyUninitializedContent(DynamicType, Implicit):
     """ Basic dynamic content class.
     """
@@ -192,17 +186,19 @@
         # The following is nasty, but I want to make sure the ValueError
         # carries some useful information
         INVALID_ID = 'invalid_id'
         try:
             foo.getActionInfo('object/%s' % INVALID_ID)
         except ValueError as e:
             message = e.args[0]
-            detail = '"%s" does not offer action "%s"' % (message, INVALID_ID)
+            detail = f'"{message}" does not offer action "{INVALID_ID}"'
             self.assertTrue(message.find(INVALID_ID) != -1, detail)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(DynamicTypeTests),
-        unittest.makeSuite(DynamicTypeDefaultTraversalTests),
-        unittest.makeSuite(DynamicTypeSecurityTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(DynamicTypeTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            DynamicTypeDefaultTraversalTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            DynamicTypeSecurityTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_Expression.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_Expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,9 +77,9 @@
         self.assertTrue(folder)
         self.assertEqual(folder.id, 'foo')
         self.assertEqual(folder.absolute_url(), 'url_foo')
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(ExpressionTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(ExpressionTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSDTMLMethod.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSDTMLMethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,10 +173,11 @@
         custom_pt = self.custom.testDTML
 
         self.assertEqual(custom_pt.ZCacheable_getManagerId(), cache_id)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(FSDTMLMethodTests),
-        unittest.makeSuite(FSDTMLMethodCustomizationTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(FSDTMLMethodTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            FSDTMLMethodCustomizationTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSFile.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 """ Unit tests for FSFile module.
 """
 
 import os
 import unittest
 import warnings
 
-import six
-
 from zope.component import getSiteManager
 from zope.datetime import rfc1123_date
 from zope.testing.cleanup import cleanUp
 
 from ..interfaces import ICachingPolicyManager
 from .base.dummy import FAKE_ETAG
 from .base.dummy import DummyCachingManager
@@ -75,61 +73,41 @@
         file = self._makeOne('test_file', 'test_file.swf')
         file = file.__of__(self.app)
         self.assertEqual(len(bytes(file)), len(bytes(ref)))
 
     def test_str(self):
         from ZPublisher.HTTPRequest import default_encoding
 
-        if six.PY2:
-            # This test only makes sense under Python 2. The file
-            # being loaded is a binary string, which is what ``str``
-            # under Python 2 returns. Under Python 3 this will lead
-            # to a decoding attempt, which will fail or destroy the data.
-            _path, ref = self._extractFile('test_file.swf')
-            file = self._makeOne('test_file', 'test_file.swf')
-            file = file.__of__(self.app)
-            self.assertEqual(len(str(file)), len(str(ref)))
-
         encoded = b'Th\xc3\xaes \xc3\xaes s\xc3\xb6me t\xc3\xa9xt.'
 
         # This file contains UTF-8 text data
         file = self._makeOne('test_text', 'test_text.txt')
         data = str(file).strip()
 
         self.assertIsInstance(data, str)
-        if six.PY2:
-            self.assertEqual(data, encoded)
-        else:
-            self.assertEqual(data, encoded.decode(default_encoding))
+        self.assertEqual(data, encoded.decode(default_encoding))
 
         # This file contains latin-1 test data
         file = self._makeOne('test_text', 'test_text_latin1.txt')
         data = str(file).strip()
 
         self.assertIsInstance(data, str)
-        if six.PY2:
-            l1_data = encoded.decode(default_encoding).encode('latin-1')
-            self.assertEqual(data, l1_data)
-        else:
-            self.assertEqual(data, encoded.decode(default_encoding))
+        self.assertEqual(data, encoded.decode(default_encoding))
 
         # This file contains non-text binary data
         file = self._makeOne('test_binary', 'test_image.gif')
         _path, real_data = self._extractFile('test_image.gif')
 
         self.assertIsInstance(data, str)
-        if six.PY2:
-            self.assertEqual(str(file), real_data)
-        else:
-            # Calling ``__str__`` on non-text binary data in Python 3
-            # will raise a DeprecationWarning because it makes no sense.
-            # Ignore it here, the warning is irrelevant for the test.
-            with warnings.catch_warnings():
-                warnings.simplefilter('ignore')
-                self.assertRaises(UnicodeDecodeError, file.__str__)
+        # Calling ``__str__`` on non-text binary data
+        # will raise a DeprecationWarning because it makes no sense.
+        # Ignore it here, the warning is irrelevant for the test.
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore')
+            self.assertRaises(UnicodeDecodeError, file.__str__)
 
     def test_index_html(self):
         path, ref = self._extractFile('test_file.swf')
         mod_time = os.stat(path)[8]
 
         file = self._makeOne('test_file', 'test_file.swf')
         file = file.__of__(self.app)
@@ -297,9 +275,9 @@
         file._parsed = False
         file._updateFromFS()
         self.assertTrue(invalidated)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(FSFileTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(FSFileTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSImage.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSImage.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,9 +244,9 @@
         image._parsed = False
         image._updateFromFS()
         self.assertTrue(invalidated)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(FSImageTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(FSImageTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSMetadata.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSMetadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,9 +68,9 @@
         # Test roles
         ob = self.ob.fake_skin.test_dtml
         self._checkProxyRoles(ob, ['Manager', 'Anonymous'])
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(FSMetadata),
+        unittest.defaultTestLoader.loadTestsFromTestCase(FSMetadata),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSPageTemplate.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSPageTemplate.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,34 +105,34 @@
         script()
         self.assertEqual(self.RESPONSE.getHeader('content-type'),
                          'text/xml; charset=utf-8')
 
     def test_CharsetFromFSMetadata(self):
         # testPT3 is an UTF-16 encoded file (see its .metadatafile)
         # is respected
-        unencoded = u'123\xfc\xf6\xe4\xdf'
+        unencoded = '123\xfc\xf6\xe4\xdf'
         script = self._makeOne('testPT3', 'testPT3.pt')
         script = script.__of__(self.app)
         script.charset = 'utf-16'
         data = script.read()
         self.assertTrue(unencoded in data)
         self.assertEqual(script.content_type, 'text/html')
 
     def test_CharsetFrom2FSMetadata(self):
         # testPT4 is an UTF-8 encoded file (see its .metadatafile)
         # is respected
-        unencoded = u'123\xfc\xf6\xe4\xdf'
+        unencoded = '123\xfc\xf6\xe4\xdf'
         script = self._makeOne('testPT4', 'testPT4.pt')
         script = script.__of__(self.app)
         data = script.read()
         self.assertTrue(unencoded in data)
         self.assertEqual(script.content_type, 'text/html')
 
     def test_CharsetFromContentTypeMetadata(self):
-        unencoded = u'123\xfc\xf6\xe4\xdf'
+        unencoded = '123\xfc\xf6\xe4\xdf'
         script = self._makeOne('testPT5', 'testPT5.pt')
         script = script.__of__(self.app)
         data = script.read()
         self.assertTrue(unencoded in data)
         self.assertEqual(script.content_type, 'text/html; charset=utf-16')
 
     def test_BadCall(self):
@@ -233,10 +233,11 @@
 
         customized = self.custom.testPT
         self.assertFalse(customized.expand)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(FSPageTemplateTests),
-        unittest.makeSuite(FSPageTemplateCustomizationTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(FSPageTemplateTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            FSPageTemplateCustomizationTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSPropertiesObject.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSPropertiesObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,9 +111,9 @@
 
         self.assertTrue('test_props' in custom.objectIds())
         self.assertTrue(aq_base(custom._getOb('test_props')) is clone)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(FSPOTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(FSPOTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSPythonScript.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSPythonScript.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,20 +12,19 @@
 ##############################################################################
 """ Unit tests for FSPythonScript module.
 """
 
 import os
 import unittest
 import warnings
+from _thread import start_new_thread
 from os.path import join
 from sys import exc_info
 from time import sleep
 
-from six.moves._thread import start_new_thread
-
 from Acquisition import aq_base
 from DateTime.DateTime import DateTime
 from OFS.Folder import Folder
 from OFS.SimpleItem import SimpleItem
 from Testing import ZopeTestCase
 from zope.testing.cleanup import cleanUp
 
@@ -302,13 +301,14 @@
         with warnings.catch_warnings():
             warnings.simplefilter('ignore')
             self.app.warn_me()
             self.app.warn1()
 
 
 def test_suite():
+    loadTestsFromTestCase = unittest.defaultTestLoader.loadTestsFromTestCase
     return unittest.TestSuite((
-        unittest.makeSuite(FSPythonScriptTests),
-        unittest.makeSuite(FSPythonScriptCustomizationTests),
-        unittest.makeSuite(CustomizedPythonScriptTests),
-        unittest.makeSuite(FSPythonScriptWarningsTests),
-        ))
+        loadTestsFromTestCase(FSPythonScriptTests),
+        loadTestsFromTestCase(FSPythonScriptCustomizationTests),
+        loadTestsFromTestCase(CustomizedPythonScriptTests),
+        loadTestsFromTestCase(FSPythonScriptWarningsTests),
+    ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSReSTMethod.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSReSTMethod.py`

 * *Files 5% similar despite different names*

```diff
@@ -227,10 +227,11 @@
         custom_pt = self.custom.testReST
 
         self.assertEqual(custom_pt.ZCacheable_getManagerId(), cache_id)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(FSReSTMethodTests),
-        unittest.makeSuite(FSReSTMethodCustomizationTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(FSReSTMethodTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            FSReSTMethodCustomizationTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSSTXMethod.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSSTXMethod.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,10 +286,11 @@
         custom_pt = self.custom.testSTX
 
         self.assertEqual(custom_pt.ZCacheable_getManagerId(), cache_id)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(FSSTXMethodTests),
-        unittest.makeSuite(FSSTXMethodCustomizationTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(FSSTXMethodTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            FSSTXMethodCustomizationTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSSecurity.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSSecurity.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from AccessControl.Permission import Permission
 from App.config import getConfiguration
 
 from .base.testcase import LogInterceptor
 from .base.testcase import WritableFSDVTest
 
 
-class MetadataChecker(object):
+class MetadataChecker:
 
     def _checkSettings(self, object, permissionname, acquire=0, roles=[]):
         # check the roles and acquire settings for a permission on an
         # object are as expected
         happy = 0
         for pstuff in object.ac_inherited_permissions(1):
             name, value = pstuff[:2]
@@ -184,10 +184,12 @@
                         self.use_dir_mtime)
         # test
         self._checkSettings(self.ob.fake_skin.test4, 'View', 1, ['Manager'])
 
 
 def test_suite():
     suite = unittest.TestSuite()
-    suite.addTest(unittest.makeSuite(FSSecurityTests))
-    suite.addTest(unittest.makeSuite(DebugModeTests))
+    suite.addTest(
+        unittest.defaultTestLoader.loadTestsFromTestCase(FSSecurityTests))
+    suite.addTest(
+        unittest.defaultTestLoader.loadTestsFromTestCase(DebugModeTests))
     return suite
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_FSZSQLMethod.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_FSZSQLMethod.py`

 * *Files 5% similar despite different names*

```diff
@@ -125,10 +125,11 @@
         self.assertEqual(zsql.class_file_, 'CMFCore.TestRecord')
         self.assertEqual(zsql.connection_hook, 'MyHook')
         self.assertFalse(zsql.allow_simple_one_argument_traversal is None)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(FSZSQLMethodTests),
-        unittest.makeSuite(FSZSQLMethodCustomizationTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(FSZSQLMethodTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            FSZSQLMethodCustomizationTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_MemberDataTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_MemberDataTool.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,10 +208,10 @@
         self.assertEqual(user.__, 'newpw')
         self.assertEqual(list(user.getRoles()), ['NewRole'])
         self.assertEqual(list(user.getDomains()), ['newdomain'])
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(MemberDataToolTests),
-        unittest.makeSuite(MemberAdapterTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(MemberDataToolTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(MemberAdapterTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_MembershipTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_MembershipTool.py`

 * *Files 3% similar despite different names*

```diff
@@ -329,11 +329,13 @@
 
         # Cleanup
         DummyUserFolder.userFolderDelUsers = deletion_method
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(MembershipToolTests),
-        unittest.makeSuite(MembershipToolSecurityTests),
-        unittest.makeSuite(MembershipToolMemberAreaTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(MembershipToolTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            MembershipToolSecurityTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            MembershipToolMemberAreaTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_OpaqueItems.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_OpaqueItems.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 #
 ##############################################################################
 """ Unit tests for IOpaqueItems implementations.
 """
 
 import unittest
 
-import six
-
 from zope.component import getSiteManager
 from zope.interface import implementer
 
 from ..interfaces import ICallableOpaqueItem
 from ..interfaces import ICallableOpaqueItemEvents
 from ..interfaces import IContentish
 from ..interfaces import ITypesTool
@@ -53,15 +51,15 @@
     """
 
     def __init__(self, id='dummy', opaqueItem=None, *args, **kw):
         OriginalDummyContent.__init__(self, id, *args, **kw)
         if opaqueItem is None:
             self.opaqueItem = 'noncallable'
             self.opaqueItemsId = 'opaqueItem'
-        elif isinstance(opaqueItem, six.string_types):
+        elif isinstance(opaqueItem, str):
             Hooks(self, opaqueItem)
             self.opaqueItemsId = opaqueItem
         else:
             opaqueItem(self, 'opaqueItem')
             self.opaqueItemsId = 'opaqueItem'
 
     # Ensure additional attributes get copied
@@ -267,9 +265,10 @@
         self.assertEqual(dummy.isNotifiedByAfterAdd(), 2)
         self.assertEqual(dummy.isNotifiedByAfterClone(), 1)
         self.assertFalse(dummy.isNotifiedByBeforeDelete())
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(ManageBeforeAfterTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            ManageBeforeAfterTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_PortalContent.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_PortalContent.py`

 * *Files 7% similar despite different names*

```diff
@@ -129,9 +129,10 @@
         self.assertEqual(userid, acl_users.all_powerful_Oz.getId())
         self.assertEqual(len(roles), 1)
         self.assertEqual(roles[0], 'Owner')
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(PortalContentTests),
-        unittest.makeSuite(TestContentCopyPaste)))
+        unittest.defaultTestLoader.loadTestsFromTestCase(PortalContentTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(TestContentCopyPaste),
+    ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_PortalFolder.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_PortalFolder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1097,24 +1097,14 @@
         self._initPolicyAndUser()
 
         cookie = folder1.manage_cutObjects(ids=('file',))
         self._assertCopyErrorUnauth(folder2.manage_pasteObjects, cookie,
                                     ce_regex='Not Supported')
 
     def test_move_cant_create_target_metatype_not_allowed(self):
-
-        #
-        #   This test can't succeed on Zope's earlier than 2.7.3 because
-        #   of the DWIM'y behavior of 'guarded_getattr', which tries to
-        #   filter acquired-but-inaccessible objects, rather than raising
-        #   Unauthorized.
-        #
-        #   If you are running with such a Zope, this test will error out
-        #   with an AttributeError (instead of the expected Unauthorized).
-        #
         folder1, folder2 = self._initFolders()
         folder2.all_meta_types = FILE_META_TYPES
 
         def _no_manage_addFile(a, c, n, v, *args, **kw):
             return n != 'manage_addFile'
 
         def _no_add_images_and_files(permission, object, context):
@@ -1260,14 +1250,15 @@
         # copy and pasting the object into the folder should raise
         # an exception
         copy_cookie = self.app.manage_copyObjects(ids=['folder2'])
         self.assertRaises(ValueError, folder1.manage_pasteObjects, copy_cookie)
 
 
 def test_suite():
+    loadTestsFromTestCase = unittest.defaultTestLoader.loadTestsFromTestCase
     return unittest.TestSuite((
-        unittest.makeSuite(PortalFolderFactoryTests),
-        unittest.makeSuite(PortalFolderTests),
-        unittest.makeSuite(PortalFolderSecurityTests),
-        unittest.makeSuite(PortalFolderMoveTests),
-        unittest.makeSuite(ContentFilterTests),
-        unittest.makeSuite(PortalFolderCopySupportTests)))
+        loadTestsFromTestCase(PortalFolderFactoryTests),
+        loadTestsFromTestCase(PortalFolderTests),
+        loadTestsFromTestCase(PortalFolderSecurityTests),
+        loadTestsFromTestCase(PortalFolderMoveTests),
+        loadTestsFromTestCase(ContentFilterTests),
+        loadTestsFromTestCase(PortalFolderCopySupportTests)))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_RegistrationTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_RegistrationTool.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,13 +30,7 @@
         from ..RegistrationTool import RegistrationTool
 
         verifyClass(IRegistrationTool, RegistrationTool)
 
     def test_generatePassword(self):
         rtool = self._makeOne()
         self.assertTrue(len(rtool.generatePassword()) >= 5)
-
-
-def test_suite():
-    return unittest.TestSuite((
-        unittest.makeSuite(RegistrationToolTests),
-        ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_SkinsTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_SkinsTool.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,10 +136,10 @@
         self.REQUEST['HTTP_SKIN_NAME'] = 'skinB'
         stool.addSkinSelection('skinB', ('bar, foo'))
         self.assertEqual(som.getSkinNameFromRequest(self.REQUEST), 'skinB')
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(SkinsContainerTests),
-        unittest.makeSuite(SkinsToolTests),
-        unittest.makeSuite(SkinnableTests)))
+        unittest.defaultTestLoader.loadTestsFromTestCase(SkinsContainerTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(SkinsToolTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(SkinnableTests)))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_TypesTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_TypesTool.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,15 @@
         except Unauthorized:
             self.fail('CMF Collector issue #165 (Ownership bug): '
                       'Unauthorized raised')
 
         self.assertEqual(folder.page2.portal_type, 'Baz')
 
 
-class TypeInfoTests(object):
+class TypeInfoTests:
     # Subclass must define _getTargetClass
 
     def _makeOne(self, id='test', **kw):
         return self._getTargetClass()(id, **kw)
 
     def _makeTypesTool(self):
         from ..TypesTool import TypesTool
@@ -425,15 +425,15 @@
                          'string:${portal_url}/foo_icon_expr.gif')
         self.assertEqual(info_data[0]['visible'], True)
         self.assertEqual(info_data[0]['available'], ti._checkAvailable)
         self.assertEqual(info_data[0]['allowed'], ti._checkAllowed)
         self.assertEqual(info_data[0]['link_target'], ti.link_target)
 
         self.assertEqual(set(info_data[1]),
-                         set(['url', 'icon', 'available', 'allowed']))
+                         {'url', 'icon', 'available', 'allowed'})
 
     def test_getInfoData_without_urls(self):
         ti_data = {'id': 'foo',
                    'title': 'Foo',
                    'description': 'Foo objects are just used for testing.',
                    'content_meta_type': 'Foo Content',
                    'factory': 'cmf.foo'}
@@ -449,15 +449,15 @@
         self.assertEqual(info_data[0]['url'], '')
         self.assertEqual(info_data[0]['icon'], '')
         self.assertEqual(info_data[0]['visible'], True)
         self.assertEqual(info_data[0]['available'], ti._checkAvailable)
         self.assertEqual(info_data[0]['allowed'], ti._checkAllowed)
         self.assertEqual(info_data[0]['link_target'], None)
 
-        self.assertEqual(set(info_data[1]), set(['available', 'allowed']))
+        self.assertEqual(set(info_data[1]), {'available', 'allowed'})
 
     def _checkContentTI(self, ti):
         from ..ActionInformation import ActionInformation
         wanted_aliases = {'view': 'dummy_view', '(Default)': 'dummy_view'}
         wanted_actions_text0 = 'string:${object_url}/dummy_view'
         wanted_actions_text1 = 'string:${object_url}/dummy_edit_form'
         wanted_actions_text2 = 'string:${object_url}/metadata_edit_form'
@@ -665,15 +665,15 @@
         self.assertEqual(majyk_dust.id, 'majyk_dust')
 
     def test_events(self):
         from OFS.interfaces import IObjectWillBeAddedEvent
         from zope.component import adapter
         from zope.component import provideHandler
         from zope.container.interfaces import IContainerModifiedEvent
-        from zope.container.interfaces import IObjectAddedEvent
+        from zope.lifecycleevent.interfaces import IObjectAddedEvent
         from zope.lifecycleevent.interfaces import IObjectCreatedEvent
         events = []
 
         @adapter(IObjectCreatedEvent)
         def _handleObjectCreated(event):
             events.append(event)
         provideHandler(_handleObjectCreated)
@@ -740,15 +740,15 @@
         SecurityTest.tearDown(self)
 
     def test_events(self):
         from OFS.interfaces import IObjectWillBeAddedEvent
         from zope.component import adapter
         from zope.component import provideHandler
         from zope.container.interfaces import IContainerModifiedEvent
-        from zope.container.interfaces import IObjectAddedEvent
+        from zope.lifecycleevent.interfaces import IObjectAddedEvent
         from zope.lifecycleevent.interfaces import IObjectCreatedEvent
         events = []
 
         @adapter(IObjectCreatedEvent)
         def _handleObjectCreated(event):
             events.append(event)
         provideHandler(_handleObjectCreated)
@@ -811,15 +811,16 @@
         self._allow = allow
 
     def allowCreate(self, container, type_id):
         return self._allow
 
 
 def test_suite():
+    loadTestsFromTestCase = unittest.defaultTestLoader.loadTestsFromTestCase
     return unittest.TestSuite((
-        unittest.makeSuite(TypesToolTests),
-        unittest.makeSuite(TypesToolFunctionalTests),
-        unittest.makeSuite(FTIDataTests),
-        unittest.makeSuite(STIDataTests),
-        unittest.makeSuite(FTIOldstyleConstructionTests),
-        unittest.makeSuite(FTINewstyleConstructionTests),
-        ))
+        loadTestsFromTestCase(TypesToolTests),
+        loadTestsFromTestCase(TypesToolFunctionalTests),
+        loadTestsFromTestCase(FTIDataTests),
+        loadTestsFromTestCase(STIDataTests),
+        loadTestsFromTestCase(FTIOldstyleConstructionTests),
+        loadTestsFromTestCase(FTINewstyleConstructionTests),
+    ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_URLTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_URLTool.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,11 +60,7 @@
         self.site._setObject('folder', DummyFolder(id='buz'))
         self.site.folder._setObject('item', DummyContent(id='qux.html'))
         obj = self.site.folder.item
         self.assertEqual(url_tool.getRelativeContentPath(obj),
                          ('buz', 'qux.html'))
         self.assertEqual(url_tool.getRelativeContentURL(obj), 'buz/qux.html')
         self.assertEqual(url_tool.getRelativeUrl(obj), 'buz/qux.html')
-
-
-def test_suite():
-    return unittest.TestSuite((unittest.makeSuite(URLToolTests)))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_UndoTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_UndoTool.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """
 
 import unittest
 
 from zope.interface.verify import verifyClass
 
 
-class DummyFolder(object):
+class DummyFolder:
 
     def undoable_transactions(self, first_transaction=None,
                               last_transaction=None,
                               PrincipiaUndoBatchSize=None):
         return ()
 
 
@@ -46,9 +46,9 @@
         obj = DummyFolder()
         transactions = udtool.listUndoableTransactionsFor(obj)
         self.assertEqual(transactions, ())
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(UndoToolTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(UndoToolTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_WorkflowTool.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_WorkflowTool.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     def notified(self, name):
         return self._notified.setdefault(name, [])
 
     #
     #   WorkflowDefinition interface
     #
     def getCatalogVariablesFor(self, ob):
-        return {'dummy': '%s: %s' % (self.getId(), ob.getId())}
+        return {'dummy': f'{self.getId()}: {ob.getId()}'}
 
     def updateRoleMappingsFor(self, ob):
         pass
 
     def listObjectActions(self, info):
         return ()  # XXX
 
@@ -444,8 +444,8 @@
             and then check to see that the workflows each got called;
             check the resulting count, as well.
         """
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(WorkflowToolTests),))
+        unittest.defaultTestLoader.loadTestsFromTestCase(WorkflowToolTests),))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_utils.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,15 @@
 
         # The values on the object itself should still the the same
         self.assertEqual(len(obj.get_local_roles_for_userid('dummyuser1')), 2)
 
     def test_mergedLocalRolesOnFunctions(self):
         from ..utils import _mergedLocalRoles
 
-        class Dummy(object):
+        class Dummy:
             __ac_local_roles__ = {'a': 'b'}
 
             def render(self):
                 pass
 
         obj = Dummy()
         self.assertDictEqual(
@@ -267,10 +267,11 @@
             sm.removeContext(eo)
 
         self.assertFalse(sm.checkPermission('FOO', obj))
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(CoreUtilsTests),
-        unittest.makeSuite(CoreUtilsSecurityTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(CoreUtilsTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            CoreUtilsSecurityTests),
         ))
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tests/test_zcml.py` & `Products.CMFCore-3.0/src/Products/CMFCore/tests/test_zcml.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/tool.zcml` & `Products.CMFCore-3.0/src/Products/CMFCore/tool.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/utils.py` & `Products.CMFCore-3.0/src/Products/CMFCore/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,21 @@
 ##############################################################################
 """ Utility functions.
 """
 
 import base64
 import re
 import sys
+from _thread import allocate_lock
 from copy import deepcopy
 from os import path as os_path
 from os.path import abspath
 from warnings import warn
 
 import pkg_resources
-import six
-from six.moves._thread import allocate_lock
 
 from AccessControl.class_init import InitializeClass
 from AccessControl.Permission import Permission
 from AccessControl.PermissionRole import rolesForPermissionOn
 from AccessControl.rolemanager import gather_permissions
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from AccessControl.SecurityInfo import ModuleSecurityInfo
@@ -183,15 +182,15 @@
 
     o Use 'valueName' to generate appropriate error messages.
     """
     if isinstance(value, tuple):
         return value
     if isinstance(value, list):
         return tuple(value)
-    if isinstance(value, six.string_types):
+    if isinstance(value, str):
         return tuple(value.split())
     raise ValueError('%s of unsupported type' % valueName)
 
 
 #
 #   Security utilities, callable only from unrestricted code.
 #
@@ -199,15 +198,15 @@
 @security.private
 def _getAuthenticatedUser(self):
     return getSecurityManager().getUser()
 
 
 @security.private
 def _checkPermission(permission, obj):
-    if not isinstance(permission, six.string_types):
+    if not isinstance(permission, str):
         permission = permission.decode()
     return getSecurityManager().checkPermission(permission, obj)
 
 
 # If Zope ever provides a call to getRolesInContext() through
 # the SecurityManager API, the method below needs to be updated.
 @security.private
@@ -285,15 +284,15 @@
     """
     # This mimics what AccessControl/Role.py does.
     # Needless to say, it's crude. :-(
     something_changed = 0
     perm_info = _ac_inherited_permissions(ob, 1)
     for name, settings in map.items():
         cur_roles = rolesForPermissionOn(name, ob)
-        if isinstance(cur_roles, six.string_types):
+        if isinstance(cur_roles, str):
             cur_roles = [cur_roles]
         else:
             cur_roles = list(cur_roles)
         changed = 0
         for (role, allow) in settings.items():
             if not allow:
                 if role in cur_roles:
@@ -610,15 +609,15 @@
 
         if self.icon:
             icon = os_path.split(self.icon)[1]
         else:
             icon = None
         for tool in self.tools:
             tool.__factory_meta_type__ = self.meta_type
-            tool.icon = 'misc_/%s/%s' % (self.product_name, icon)
+            tool.icon = f'misc_/{self.product_name}/{icon}'
 
 
 InitializeClass(ToolInit)
 
 addInstanceForm = HTMLFile('dtml/addInstance', globals())
 
 
@@ -738,15 +737,15 @@
     o 'klass' is the class being decorated.
 
     o 'iconspec' is the path within the product where the icon lives.
     """
     modname = klass.__module__
     pid = modname.split('.')[1]
     name = os_path.split(iconspec)[1]
-    klass.icon = 'misc_/%s/%s' % (pid, name)
+    klass.icon = f'misc_/{pid}/{name}'
     icon = ImageFile(iconspec, _prefix)
     icon.__roles__ = None
     if not hasattr(misc_images, pid):
         setattr(misc_images, pid, MiscImage(pid, {}))
     getattr(misc_images, pid)[name] = icon
 
 
@@ -899,22 +898,16 @@
     """ record-like class """
 
     def __init__(self, **kw):
         self.__dict__.update(kw)
 
 
 def base64_encode(text):
-    # Helper method to avoid deprecation warning under Python 3
-    if six.PY2:
-        return base64.encodestring(text).rstrip()
     return base64.encodebytes(text).rstrip()
 
 
 def base64_decode(text):
-    # Helper method to avoid deprecation warning under Python 3
-    if six.PY2:
-        return base64.decodestring(text)
     return base64.decodebytes(text)
 
 
 security.declarePublic('Message')  # NOQA: flake8: D001
 Message = MessageFactory('cmf_default')
```

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/www/cpsDiff.pt` & `Products.CMFCore-3.0/src/Products/CMFCore/www/cpsDiff.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/www/typeinfoAliases.zpt` & `Products.CMFCore-3.0/src/Products/CMFCore/www/typeinfoAliases.zpt`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/www/typesAliases.zpt` & `Products.CMFCore-3.0/src/Products/CMFCore/www/typesAliases.zpt`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-2.7.0/src/Products/CMFCore/zcml.py` & `Products.CMFCore-3.0/src/Products/CMFCore/zcml.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,34 +30,34 @@
 
 class IRegisterDirectoryDirective(Interface):
 
     """Register directories with the global registry.
     """
 
     name = PythonIdentifier(
-        title=u'Name',
-        description=u'Name of the directory.',
+        title='Name',
+        description='Name of the directory.',
         required=True)
 
     directory = Path(
-        title=u'Path',
-        description=u'Path relative to the package. If not specified, '
-                    u"'skins/<name>' is used.",
+        title='Path',
+        description='Path relative to the package. If not specified, '
+                    "'skins/<name>' is used.",
         required=False)
 
     recursive = Bool(
-        title=u'Recursive?',
-        description=u'False by default. If true, register all subdirectories '
-                    u'as well.',
+        title='Recursive?',
+        description='False by default. If true, register all subdirectories '
+                    'as well.',
         required=False)
 
     ignore = Tokens(
-        title=u'Ignore',
-        description=u'Files and subdirectories that should be ignored. If '
-                    u"not specified, 'CVS' and '.svn' are ignored.",
+        title='Ignore',
+        description='Files and subdirectories that should be ignored. If '
+                    "not specified, 'CVS' and '.svn' are ignored.",
         value_type=ASCIILine(),
         required=False)
 
 
 _directory_regs = []
```

### Comparing `Products.CMFCore-2.7.0/src/Products.CMFCore.egg-info/PKG-INFO` & `Products.CMFCore-3.0/src/Products.CMFCore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 Metadata-Version: 2.1
 Name: Products.CMFCore
-Version: 2.7.0
+Version: 3.0
 Summary: Zope Content Management Framework core components
 Home-page: https://github.com/zopefoundation/Products.CMFCore
 Author: Zope Foundation and Contributors
 Author-email: zope-cmf@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://zope.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/zopefoundation/Products.CMFCore/issues
 Project-URL: Sources, https://github.com/zopefoundation/Products.CMFCore
 Keywords: web application server zope cmf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
-Classifier: Framework :: Zope :: 4
 Classifier: Framework :: Zope :: 5
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: zsql
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 .. image:: https://github.com/zopefoundation/Products.CMFCore/actions/workflows/tests.yml/badge.svg
         :target: https://github.com/zopefoundation/Products.CMFCore/actions/workflows/tests.yml
@@ -62,14 +57,27 @@
 
 
 ------------------------------------------------------------
 
 Products.CMFCore Changelog
 ==========================
 
+3.0 (2023-04-25)
+----------------
+
+- SkinsTool: fix Find form with Zope ZMI
+  (`#127 <https://github.com/zopefoundation/Products.CMFCore/pull/127>`_).
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop support for ``Zope 4.x``.
+
+- Make tests compatible with ``Zope >= 5.7.1``.
+
+
 2.7.0 (2022-12-16)
 ------------------
 
 - Fix insidious buildout configuration bug for tests against Zope 4.
 
 - Add support for Python 3.11.
```

### Comparing `Products.CMFCore-2.7.0/src/Products.CMFCore.egg-info/SOURCES.txt` & `Products.CMFCore-3.0/src/Products.CMFCore.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 CHANGES.rst
 CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
 buildout.cfg
-buildout4.cfg
 rtd.txt
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/changes.rst
 docs/conf.py
 docs/index.rst
-docs/_build/html/_sources/changes.rst.txt
-docs/_build/html/_sources/index.rst.txt
-docs/_build/html/_sources/api/content.rst.txt
-docs/_build/html/_sources/api/tools.rst.txt
 docs/api/content.rst
 docs/api/tools.rst
 src/Products/__init__.py
 src/Products.CMFCore.egg-info/PKG-INFO
 src/Products.CMFCore.egg-info/SOURCES.txt
 src/Products.CMFCore.egg-info/dependency_links.txt
 src/Products.CMFCore.egg-info/entry_points.txt
@@ -117,15 +112,14 @@
 src/Products/CMFCore/dtml/explainSkinsTool.dtml
 src/Products/CMFCore/dtml/explainTypesTool.dtml
 src/Products/CMFCore/dtml/explainURLTool.dtml
 src/Products/CMFCore/dtml/explainUndoTool.dtml
 src/Products/CMFCore/dtml/explainWorkflowTool.dtml
 src/Products/CMFCore/dtml/extensionWidget.dtml
 src/Products/CMFCore/dtml/findForm.dtml
-src/Products/CMFCore/dtml/findResult.dtml
 src/Products/CMFCore/dtml/majorMinorWidget.dtml
 src/Products/CMFCore/dtml/manageActionProviders.dtml
 src/Products/CMFCore/dtml/memberdataContents.dtml
 src/Products/CMFCore/dtml/membershipRolemapping.dtml
 src/Products/CMFCore/dtml/mimetypePredEdit.dtml
 src/Products/CMFCore/dtml/patternWidget.dtml
 src/Products/CMFCore/dtml/registryPredList.dtml
```

### Comparing `Products.CMFCore-2.7.0/tox.ini` & `Products.CMFCore-3.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,39 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/zope-product
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
     py311
     docs
     coverage
 
 [testenv]
 skip_install = true
 deps =
     zc.buildout >= 3.0.1
     wheel > 0.37
 commands_pre =
-    py27,py35: {envbindir}/buildout -nc {toxinidir}/buildout4.cfg buildout:directory={envdir} buildout:develop={toxinidir} install test
-    !py27-!py35: {envbindir}/buildout -nc {toxinidir}/buildout.cfg buildout:directory={envdir} buildout:develop={toxinidir} install test
+    {envbindir}/buildout -nc {toxinidir}/buildout.cfg buildout:directory={envdir} buildout:develop={toxinidir} install test
 commands =
     {envdir}/bin/test {posargs:-cv}
 
 [testenv:lint]
 basepython = python3
 commands_pre =
     mkdir -p {toxinidir}/parts/flake8
 allowlist_externals =
     mkdir
 commands =
     isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
-    - flake8 {toxinidir}/src {toxinidir}/setup.py
     flake8 {toxinidir}/src {toxinidir}/setup.py
     check-manifest
     check-python-versions
 deps =
     check-manifest
     check-python-versions
     flake8
@@ -69,24 +64,22 @@
 basepython = python3
 skip_install = true
 allowlist_externals =
     mkdir
 deps =
     {[testenv]deps}
     coverage
-    coverage-python-version
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run {envdir}/bin/test {posargs:-cv}
     coverage html
     coverage report -m --fail-under=85
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = Products.CMFCore
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

