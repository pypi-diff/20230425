# Comparing `tmp/dhi-platform-1.0.6.tar.gz` & `tmp/dhi-platform-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhi-platform-1.0.6.tar", last modified: Fri Feb  3 12:56:31 2023, max compression
+gzip compressed data, was "dhi-platform-1.0.7.tar", last modified: Tue Apr 25 12:34:07 2023, max compression
```

## Comparing `dhi-platform-1.0.6.tar` & `dhi-platform-1.0.7.tar`

### file list

```diff
@@ -1,174 +1,181 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.358211 dhi-platform-1.0.6/
--rw-r--r--   0 vsts      (1001) docker     (123)     1005 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)     7342 2023-02-03 12:56:31.358211 dhi-platform-1.0.6/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     6570 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.326210 dhi-platform-1.0.6/bin/
--rw-r--r--   0 vsts      (1001) docker     (123)      905 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/bin/plt
--rw-r--r--   0 vsts      (1001) docker     (123)     1245 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/bin/plt.bat
--rw-r--r--   0 vsts      (1001) docker     (123)      103 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-02-03 12:56:31.358211 dhi-platform-1.0.6/setup.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.326210 dhi-platform-1.0.6/src/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.318210 dhi-platform-1.0.6/src/dhi/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.338210 dhi-platform-1.0.6/src/dhi/platform/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)       18 2023-02-03 12:56:21.000000 dhi-platform-1.0.6/src/dhi/platform/_version.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11926 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/args.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12925 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/authentication.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.338210 dhi-platform-1.0.6/src/dhi/platform/base/
--rw-r--r--   0 vsts      (1001) docker     (123)    18010 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/base/client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1394 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/base/constants.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2144 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/base/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      667 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/base/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.338210 dhi-platform-1.0.6/src/dhi/platform/cli/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.338210 dhi-platform-1.0.6/src/dhi/platform/cli/cfg/
--rw-r--r--   0 vsts      (1001) docker     (123)     4615 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/cfg/login.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.342210 dhi-platform-1.0.6/src/dhi/platform/cli/ds/
--rw-r--r--   0 vsts      (1001) docker     (123)     1746 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ds/append.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2550 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ds/convert.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1227 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ds/download.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1569 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ds/downloadc.py
--rw-r--r--   0 vsts      (1001) docker     (123)      831 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ds/info.py
--rw-r--r--   0 vsts      (1001) docker     (123)      855 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ds/infor.py
--rw-r--r--   0 vsts      (1001) docker     (123)      818 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ds/ls.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1138 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ds/lsh.py
--rw-r--r--   0 vsts      (1001) docker     (123)      728 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ds/lsra.py
--rw-r--r--   0 vsts      (1001) docker     (123)      560 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ds/restore.py
--rw-r--r--   0 vsts      (1001) docker     (123)      551 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ds/rm.py
--rw-r--r--   0 vsts      (1001) docker     (123)      557 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ds/rmhard.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1742 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ds/update.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ds/upload.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1883 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ds/uploadstaged.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.342210 dhi-platform-1.0.6/src/dhi/platform/cli/eng/
--rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/eng/cancel.py
--rw-r--r--   0 vsts      (1001) docker     (123)      689 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/eng/configurations.py
--rw-r--r--   0 vsts      (1001) docker     (123)      755 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/eng/diag.py
--rw-r--r--   0 vsts      (1001) docker     (123)      787 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/eng/engine.py
--rw-r--r--   0 vsts      (1001) docker     (123)      645 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/eng/engines.py
--rw-r--r--   0 vsts      (1001) docker     (123)      830 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/eng/info.py
--rw-r--r--   0 vsts      (1001) docker     (123)      635 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/eng/input.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1936 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/eng/list.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2783 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/eng/listmy.py
--rw-r--r--   0 vsts      (1001) docker     (123)      571 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/eng/rm.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2379 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/eng/run.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2395 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/eng/runp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2552 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/eng/sbmessages.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.342210 dhi-platform-1.0.6/src/dhi/platform/cli/gw/
--rw-r--r--   0 vsts      (1001) docker     (123)      740 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/gw/service.py
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/gw/services.py
--rw-r--r--   0 vsts      (1001) docker     (123)      366 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/help.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.346210 dhi-platform-1.0.6/src/dhi/platform/cli/prj/
--rw-r--r--   0 vsts      (1001) docker     (123)      822 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prj/capabilities.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1659 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prj/create.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1656 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prj/createsub.py
--rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prj/info.py
--rw-r--r--   0 vsts      (1001) docker     (123)      806 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prj/infor.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1496 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prj/ls.py
--rw-r--r--   0 vsts      (1001) docker     (123)      978 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prj/lsh.py
--rw-r--r--   0 vsts      (1001) docker     (123)      708 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prj/lsr.py
--rw-r--r--   0 vsts      (1001) docker     (123)      740 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prj/path.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1732 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prj/prepare.py
--rw-r--r--   0 vsts      (1001) docker     (123)      561 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prj/restore.py
--rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prj/rm.py
--rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prj/rmhard.py
--rw-r--r--   0 vsts      (1001) docker     (123)      567 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prj/sas.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1519 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prj/sub.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1637 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prj/update.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.346210 dhi-platform-1.0.6/src/dhi/platform/cli/prjm/
--rw-r--r--   0 vsts      (1001) docker     (123)     1054 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prjm/add.py
--rw-r--r--   0 vsts      (1001) docker     (123)      871 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prjm/all.py
--rw-r--r--   0 vsts      (1001) docker     (123)      667 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prjm/ls.py
--rw-r--r--   0 vsts      (1001) docker     (123)      741 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/prjm/rm.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.346210 dhi-platform-1.0.6/src/dhi/platform/cli/raw/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/raw/blocks.py
--rw-r--r--   0 vsts      (1001) docker     (123)      729 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/raw/checksums.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1110 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/raw/copystatus.py
--rw-r--r--   0 vsts      (1001) docker     (123)      684 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/raw/download.py
--rw-r--r--   0 vsts      (1001) docker     (123)      779 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/raw/stagingurls.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1596 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/raw/upload.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.346210 dhi-platform-1.0.6/src/dhi/platform/cli/rb/
--rw-r--r--   0 vsts      (1001) docker     (123)      937 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/rb/ls.py
--rw-r--r--   0 vsts      (1001) docker     (123)      934 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/rb/lsmy.py
--rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/rb/restore.py
--rw-r--r--   0 vsts      (1001) docker     (123)      559 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/rb/rmds.py
--rw-r--r--   0 vsts      (1001) docker     (123)      559 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/rb/rmprj.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.346210 dhi-platform-1.0.6/src/dhi/platform/cli/reader/
--rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/reader/info.py
--rw-r--r--   0 vsts      (1001) docker     (123)      817 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/reader/ls.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.346210 dhi-platform-1.0.6/src/dhi/platform/cli/tool/
--rw-r--r--   0 vsts      (1001) docker     (123)    25298 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/tool/openapi2py.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.346210 dhi-platform-1.0.6/src/dhi/platform/cli/tr/
--rw-r--r--   0 vsts      (1001) docker     (123)      997 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/tr/download.py
--rw-r--r--   0 vsts      (1001) docker     (123)      921 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/tr/info.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1153 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/tr/ls.py
--rw-r--r--   0 vsts      (1001) docker     (123)      959 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/tr/lss.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.346210 dhi-platform-1.0.6/src/dhi/platform/cli/ts/
--rw-r--r--   0 vsts      (1001) docker     (123)     1794 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ts/add.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1572 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ts/dscreate.py
--rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ts/dsinfo.py
--rw-r--r--   0 vsts      (1001) docker     (123)      723 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ts/info.py
--rw-r--r--   0 vsts      (1001) docker     (123)      686 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/ts/list.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.350211 dhi-platform-1.0.6/src/dhi/platform/cli/writer/
--rw-r--r--   0 vsts      (1001) docker     (123)      827 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/writer/info.py
--rw-r--r--   0 vsts      (1001) docker     (123)      817 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/cli/writer/ls.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14844 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/commonmodels.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10904 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/config.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11456 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/engine.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3191 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/enginehelper.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10421 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/eventing.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9459 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/eventinghelper.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7510 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/fmt.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.350211 dhi-platform-1.0.6/src/dhi/platform/generated/
--rw-r--r--   0 vsts      (1001) docker     (123)    29816 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/generated/enginegen.py
--rw-r--r--   0 vsts      (1001) docker     (123)    27842 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/generated/gisgen.py
--rw-r--r--   0 vsts      (1001) docker     (123)   450750 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/generated/metadatagen.py
--rw-r--r--   0 vsts      (1001) docker     (123)   154021 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/generated/multidimensionalgen.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3921 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/generated/pubsubgen.py
--rw-r--r--   0 vsts      (1001) docker     (123)    27583 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/generated/rawgen.py
--rw-r--r--   0 vsts      (1001) docker     (123)    31866 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/generated/sharinggen.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9353 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/generated/tilesgen.py
--rw-r--r--   0 vsts      (1001) docker     (123)    83996 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/generated/timeseriesgen.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1468 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/gis.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35585 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/metadata.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10389 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/metadatahelper.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18101 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/multidimensional.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.354210 dhi-platform-1.0.6/src/dhi/platform/protobufparser/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/protobufparser/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1722 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/protobufparser/api_implementation.py
--rw-r--r--   0 vsts      (1001) docker     (123)    21559 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/protobufparser/containers.py
--rw-r--r--   0 vsts      (1001) docker     (123)    40365 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/protobufparser/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2006 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/protobufparser/decoderdatetime.py
--rw-r--r--   0 vsts      (1001) docker     (123)    45172 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/protobufparser/descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (123)    28682 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/protobufparser/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1941 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/protobufparser/enums.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14452 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/protobufparser/message.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8492 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/protobufparser/wire_format.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1483 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/pubsub.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1469 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/raw.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2973 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/rawhelper.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1488 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/sharing.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.358211 dhi-platform-1.0.6/src/dhi/platform/tests/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.358211 dhi-platform-1.0.6/src/dhi/platform/tests/data/
--rw-r--r--   0 vsts      (1001) docker     (123)     2815 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/tests/data/EqD2.dfs2
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/tests/data/esbjergSmall.txt
--rw-r--r--   0 vsts      (1001) docker     (123)     5360 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/tests/engine_tests.py
--rw-r--r--   0 vsts      (1001) docker     (123)      687 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/tests/exceptions_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4103 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/tests/metadata_dataset_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8704 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/tests/metadata_project_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3724 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/tests/multidimensional_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)      510 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/tests/testcredentials.py
--rw-r--r--   0 vsts      (1001) docker     (123)    20051 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/tests/timeseries_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6803 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/tests/transfer_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6016 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/tests/transfer_tests_integration.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1691 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/tests/upload_download_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1478 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/tiles.py
--rw-r--r--   0 vsts      (1001) docker     (123)    21279 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/timeseries.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2676 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/timeserieshelper.py
--rw-r--r--   0 vsts      (1001) docker     (123)    82728 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/transfer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1851 2023-02-03 12:56:01.000000 dhi-platform-1.0.6/src/dhi/platform/transferuploadhelper.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-03 12:56:31.358211 dhi-platform-1.0.6/src/dhi_platform.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     7342 2023-02-03 12:56:31.000000 dhi-platform-1.0.6/src/dhi_platform.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     5143 2023-02-03 12:56:31.000000 dhi-platform-1.0.6/src/dhi_platform.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-02-03 12:56:31.000000 dhi-platform-1.0.6/src/dhi_platform.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      116 2023-02-03 12:56:31.000000 dhi-platform-1.0.6/src/dhi_platform.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        4 2023-02-03 12:56:31.000000 dhi-platform-1.0.6/src/dhi_platform.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.032268 dhi-platform-1.0.7/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1005 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)     7342 2023-04-25 12:34:07.032268 dhi-platform-1.0.7/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     6570 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.008268 dhi-platform-1.0.7/bin/
+-rw-r--r--   0 vsts      (1001) docker     (123)      905 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/bin/plt
+-rw-r--r--   0 vsts      (1001) docker     (123)     1245 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/bin/plt.bat
+-rw-r--r--   0 vsts      (1001) docker     (123)      103 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-04-25 12:34:07.032268 dhi-platform-1.0.7/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.008268 dhi-platform-1.0.7/src/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.008268 dhi-platform-1.0.7/src/dhi/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.016268 dhi-platform-1.0.7/src/dhi/platform/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       18 2023-04-25 12:33:59.000000 dhi-platform-1.0.7/src/dhi/platform/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11926 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/args.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12925 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/authentication.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.016268 dhi-platform-1.0.7/src/dhi/platform/base/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18071 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/base/client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1394 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/base/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2144 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/base/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      667 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/base/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.016268 dhi-platform-1.0.7/src/dhi/platform/cli/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.016268 dhi-platform-1.0.7/src/dhi/platform/cli/cfg/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4615 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/cfg/login.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.016268 dhi-platform-1.0.7/src/dhi/platform/cli/ds/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1746 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/append.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2550 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/convert.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2196 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/cp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2609 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/cpbh.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2914 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/cph.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1227 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/download.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1569 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/downloadc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      831 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/info.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      855 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/infor.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      818 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/ls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1138 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/lsh.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      728 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/lsra.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      560 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/restore.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      551 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/rm.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      557 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/rmhard.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1742 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/update.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/upload.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1883 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/uploadstaged.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.020268 dhi-platform-1.0.7/src/dhi/platform/cli/eng/
+-rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/cancel.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      689 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/configurations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      755 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/diag.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      787 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/engine.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      645 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/engines.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      830 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/info.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      635 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/input.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1936 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/list.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2751 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/listmy.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      571 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/rm.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3076 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/run.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3092 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/runp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2552 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/sbmessages.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.020268 dhi-platform-1.0.7/src/dhi/platform/cli/gw/
+-rw-r--r--   0 vsts      (1001) docker     (123)      740 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/gw/service.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/gw/services.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      366 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/help.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.020268 dhi-platform-1.0.7/src/dhi/platform/cli/prj/
+-rw-r--r--   0 vsts      (1001) docker     (123)      822 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/capabilities.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1659 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/create.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1656 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/createsub.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/info.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      806 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/infor.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1496 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/ls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      978 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/lsh.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      708 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/lsr.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      740 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/path.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1732 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/prepare.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      561 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/restore.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/rm.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/rmhard.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      567 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/sas.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1519 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/sub.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1637 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/update.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.020268 dhi-platform-1.0.7/src/dhi/platform/cli/prjm/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1054 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prjm/add.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      871 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prjm/all.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      667 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prjm/ls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      741 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prjm/rm.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.024268 dhi-platform-1.0.7/src/dhi/platform/cli/raw/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/raw/blocks.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      729 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/raw/checksums.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1110 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/raw/copystatus.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      684 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/raw/download.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      779 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/raw/stagingurls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1596 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/raw/upload.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.024268 dhi-platform-1.0.7/src/dhi/platform/cli/rb/
+-rw-r--r--   0 vsts      (1001) docker     (123)      937 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/rb/ls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      934 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/rb/lsmy.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/rb/restore.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      559 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/rb/rmds.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      559 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/rb/rmprj.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.024268 dhi-platform-1.0.7/src/dhi/platform/cli/reader/
+-rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/reader/info.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      817 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/reader/ls.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.024268 dhi-platform-1.0.7/src/dhi/platform/cli/tool/
+-rw-r--r--   0 vsts      (1001) docker     (123)    26826 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/tool/openapi2py.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.024268 dhi-platform-1.0.7/src/dhi/platform/cli/tr/
+-rw-r--r--   0 vsts      (1001) docker     (123)      997 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/tr/download.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      921 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/tr/info.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1153 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/tr/ls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      959 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/tr/lss.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.024268 dhi-platform-1.0.7/src/dhi/platform/cli/ts/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1794 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ts/add.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1572 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ts/dscreate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ts/dsinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      723 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ts/info.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      686 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ts/list.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.024268 dhi-platform-1.0.7/src/dhi/platform/cli/writer/
+-rw-r--r--   0 vsts      (1001) docker     (123)      827 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/writer/info.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      817 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/writer/ls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14844 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/commonmodels.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10904 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11456 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/engine.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3191 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/enginehelper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10421 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/eventing.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9459 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/eventinghelper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7510 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/fmt.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.028268 dhi-platform-1.0.7/src/dhi/platform/generated/
+-rw-r--r--   0 vsts      (1001) docker     (123)    30129 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/enginegen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    27842 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/gisgen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    33115 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/jobgen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   450751 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/metadatagen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   154021 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/multidimensionalgen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3921 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/pubsubgen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    27555 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/rawgen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    31866 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/sharinggen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9353 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/tilesgen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    83996 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/timeseriesgen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1468 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/gis.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8171 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/job.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    35673 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11244 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/metadatahelper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18101 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/multidimensional.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.028268 dhi-platform-1.0.7/src/dhi/platform/protobufparser/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1722 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/api_implementation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    21559 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/containers.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    40365 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2006 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/decoderdatetime.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    45172 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    28682 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1941 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14452 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/message.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8492 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/wire_format.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1483 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/pubsub.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1469 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/raw.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2973 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/rawhelper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18696 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/sharing.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.028268 dhi-platform-1.0.7/src/dhi/platform/tests/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.032268 dhi-platform-1.0.7/src/dhi/platform/tests/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2815 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/data/EqD2.dfs2
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/data/esbjergSmall.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     5360 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/engine_tests.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      687 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/exceptions_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3778 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/job_tests.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4103 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/metadata_dataset_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8704 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/metadata_project_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3724 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/multidimensional_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3095 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/sharing_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      510 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/testcredentials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    20051 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/timeseries_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6803 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/transfer_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7669 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/transfer_tests_integration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1691 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/upload_download_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1478 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tiles.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    21279 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/timeseries.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2676 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/timeserieshelper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    89248 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/transfer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2397 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/transferhelper.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.032268 dhi-platform-1.0.7/src/dhi_platform.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7342 2023-04-25 12:34:06.000000 dhi-platform-1.0.7/src/dhi_platform.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     5366 2023-04-25 12:34:07.000000 dhi-platform-1.0.7/src/dhi_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-25 12:34:06.000000 dhi-platform-1.0.7/src/dhi_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      116 2023-04-25 12:34:06.000000 dhi-platform-1.0.7/src/dhi_platform.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        4 2023-04-25 12:34:06.000000 dhi-platform-1.0.7/src/dhi_platform.egg-info/top_level.txt
```

### Comparing `dhi-platform-1.0.6/LICENSE` & `dhi-platform-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/PKG-INFO` & `dhi-platform-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhi-platform
-Version: 1.0.6
+Version: 1.0.7
 Summary: MIKE Cloud Platform SDK for Python
 Home-page: https://develop.mike-cloud.com/
 Author: DHI
 Author-email: wdpservice@dhigroup.com
 License: MIT License
 Project-URL: Open API, https://develop.mike-cloud.com/swagger/index.html
 Project-URL: Documentation, https://develop.mike-cloud.com/docs/
```

### Comparing `dhi-platform-1.0.6/README.md` & `dhi-platform-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/bin/plt` & `dhi-platform-1.0.7/bin/plt`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/bin/plt.bat` & `dhi-platform-1.0.7/bin/plt.bat`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/setup.cfg` & `dhi-platform-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/args.py` & `dhi-platform-1.0.7/src/dhi/platform/args.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/authentication.py` & `dhi-platform-1.0.7/src/dhi/platform/authentication.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/base/client.py` & `dhi-platform-1.0.7/src/dhi/platform/base/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,18 +248,19 @@
     @staticmethod
     def GetVersionHeaders(version, headers=None):
         result = headers if headers else {}
         if version:
             result["api-version"] = version
         return result
 
-    def GetBasicHeaders(self, includeheaders=None, api_version=None, content_type=None, **kwargs):
+    def GetBasicHeaders(self, includeheaders=None, api_version=None, content_type=None, noauthentication=False, **kwargs):
         #headers = {"dhi-open-api-key": apikey, "dhi-project-id": projectid, "dhi-service-id": "engine"}
         headers = self.__basicHeaders.copy()
-        self.__authenticator.UpdateHeaders(headers)
+        if not noauthentication:
+            self.__authenticator.UpdateHeaders(headers)
         if api_version:
             headers["api-version"] = api_version
         if projectid := kwargs.get("projectid"):
             headers["dhi-project-id"] = projectid
         if datasetid := kwargs.get("datasetid"):
             headers["dhi-dataset-id"] = datasetid
         if recursivetoken := kwargs.get("recursivetoken"):
```

### Comparing `dhi-platform-1.0.6/src/dhi/platform/base/constants.py` & `dhi-platform-1.0.7/src/dhi/platform/base/constants.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/base/exceptions.py` & `dhi-platform-1.0.7/src/dhi/platform/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/base/utils.py` & `dhi-platform-1.0.7/src/dhi/platform/base/utils.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/cfg/login.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/cfg/login.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ds/append.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ds/append.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ds/convert.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ds/convert.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ds/download.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ds/download.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ds/downloadc.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ds/downloadc.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ds/info.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ds/info.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ds/infor.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ds/infor.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ds/ls.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ds/ls.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ds/lsh.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ds/lsh.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ds/lsra.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ds/lsra.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ds/restore.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ds/restore.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ds/rm.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ds/rm.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ds/rmhard.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ds/rmhard.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ds/update.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ds/update.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ds/upload.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ds/upload.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ds/uploadstaged.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ds/uploadstaged.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/eng/cancel.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/eng/cancel.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/eng/configurations.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/eng/configurations.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/eng/diag.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/eng/diag.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/eng/engine.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/eng/engine.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/eng/engines.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/eng/engines.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/eng/info.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/eng/info.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/eng/input.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/eng/input.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/eng/list.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/eng/list.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/eng/listmy.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/eng/listmy.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     clientv2 = EngineGenClientV2(**vars(args))
 
     def getResponses():
         cursor = None
         nextlink = None
         while True:
             if cursor:
-                response = clientv2.GetMyExecutions(args.projectid, cursor=cursor)
+                response = clientv2.GetMyExecutions(cursor=cursor)
             else:
-                response = clientv2.GetMyExecutions(args.projectid, args.sortby, args.sortorder, args.starttime, args.endtime, args.scenarioname, args.status, args.project, args.limit, cursor=cursor)
+                response = clientv2.GetMyExecutions(args.sortby, args.sortorder, args.starttime, args.endtime, args.scenarioname, args.status, args.project, args.limit, cursor=cursor)
             yield response
             cursor = response.Body.get("cursor")
             nextlink = response.Body.get("@nextLink")
             listobjdata = response.Body.get("data")
             if (not cursor and not nextlink) or not listobjdata:
                 break
     responses = getResponses()
```

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/eng/rm.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/eng/rm.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/eng/run.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/eng/runp.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from dhi.platform.eventinghelper import ExecutionSession
 from dhi.platform.generated.enginegen import EngineGenClientV2
 from dhi.platform.generated.metadatagen import MetadataGenClientV2, MetadataGenClientV3
 from dhi.platform.fmt import Format
 
 def __initParser(parser):
     parser.add_argument("-f", "--inputfile", default=ClientArgs.GetDefault("DHIINPUT"), help="Input file path")
+    parser.add_argument("--pooltype", help="Pool type", choices=["VM-S-5", "VM-S-40", "VM-S-100", "VM-H-60", "VM-G-5", "VM-G-40"])
+    parser.add_argument("--nodecount", type=int, help="Node count")
+    parser.add_argument("--maxtime", type=float, help="Max execution time [hours]")
     parser.add_argument("-w", "--wait", default=False, help="Wait to finish", action="store_true")
     parser.add_argument("-l", "--showlog", default=False, help="Show log", action="store_true")
 
 async def main():
     args = ClientArgs.ParseForProject(description="Run engine", init=__initParser, defaultformat="yaml")
     ClientConfig.UpdateProjectFromConfiguration(args)
     clientv2 = EngineGenClientV2(**vars(args))
@@ -21,23 +24,33 @@
     metadataclientv3 = MetadataGenClientV3(**vars(args))
     executionsession = ExecutionSession(args.showlog, metadataclientv2, metadataclientv3, args.verbose)
     async with executionsession.subscribe(args.projectid, ["/dhi/platform/engineexecution"], 200, None):
         try:
             await executionsession.wait_pubsubconnected()
 
             input = ClientArgs.LoadJson(args.inputfile)
+            options = input.get("options")
+            if not options:
+                options = dict()
+                input["options"] = options
+            if args.pooltype:
+                options["poolType"] = args.pooltype
+            if args.nodecount:
+                options["nodeCount"] = args.nodecount
+            if args.maxtime:
+                options["maxExecutionElapsedTimeHours"] = args.maxtime
             if args.showlog:
-                inputitems = input.get("inputs")
-                if inputitems:
-                    for i in inputitems:
+                modelitems = input.get("models")
+                if modelitems:
+                    for i in modelitems:
                         if i.get("engine"):
                             tmp = i.get("reportLogUpdatesLines")
                             if not tmp or tmp == 0:
                                 i["reportLogUpdatesLines"] = 300
-            response = clientv2.RunExecution(args.projectid, input)
+            response = clientv2.RunExecutionWithPlatformData(args.projectid, input)
 
             executionsession.set_resourceid(response.Body.get("executionId"))
 
             tablefields = ["executionId", "outputLocation"]
             Format.FormatResponse(response, lambda r: r.Body, args.format, None, tablefields)
 
             if args.wait:
```

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/eng/runp.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ds/cp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 #!/usr/bin/env python
-import asyncio, platform
+from time import sleep
 from dhi.platform.args import ClientArgs
 from dhi.platform.config import ClientConfig
-from dhi.platform.eventinghelper import ExecutionSession
-from dhi.platform.generated.enginegen import EngineGenClientV2
-from dhi.platform.generated.metadatagen import MetadataGenClientV2, MetadataGenClientV3
+from dhi.platform.metadatahelper import MetadataClientV2Helper
+from dhi.platform.generated.metadatagen import MetadataGenClientV2, StagedFilesUploadInputV1, StagedFileUploadInputV1
+from dhi.platform.generated.rawgen import RawGenClientV2
 from dhi.platform.fmt import Format
 
 def __initParser(parser):
-    parser.add_argument("-f", "--inputfile", default=ClientArgs.GetDefault("DHIINPUT"), help="Input file path")
-    parser.add_argument("-w", "--wait", default=False, help="Wait to finish", action="store_true")
-    parser.add_argument("-l", "--showlog", default=False, help="Show log", action="store_true")
+    parser.add_argument("-s", "--sourceprojectid", default=None, help="Source projectid")
 
-async def main():
-    args = ClientArgs.ParseForProject(description="Run engine", init=__initParser, defaultformat="yaml")
-    ClientConfig.UpdateProjectFromConfiguration(args)
-    clientv2 = EngineGenClientV2(**vars(args))
+def __getSelectedDatasets(rawclientv2: RawGenClientV2, sourceprojectid: str, datasetids: list):
+    response = rawclientv2.GetDownloadDatasets(sourceprojectid, datasetids)
+    return (x for x in response.Body.get("data"))
 
-    metadataclientv2 = MetadataGenClientV2(**vars(args))
-    metadataclientv3 = MetadataGenClientV3(**vars(args))
-    executionsession = ExecutionSession(args.showlog, metadataclientv2, metadataclientv3, args.verbose)
-    async with executionsession.subscribe(args.projectid, ["/dhi/platform/engineexecution"], 200, None):
-        try:
-            await executionsession.wait_pubsubconnected()
-
-            input = ClientArgs.LoadJson(args.inputfile)
-            if args.showlog:
-                modelitems = input.get("models")
-                if modelitems:
-                    for i in modelitems:
-                        if i.get("engine"):
-                            tmp = i.get("reportLogUpdatesLines")
-                            if not tmp or tmp == 0:
-                                i["reportLogUpdatesLines"] = 300
-            response = clientv2.RunExecutionWithPlatformData(args.projectid, input)
-
-            executionsession.set_resourceid(response.Body.get("executionId"))
-
-            tablefields = ["executionId", "outputLocation"]
-            Format.FormatResponse(response, lambda r: r.Body, args.format, None, tablefields)
-
-            if args.wait:
-                await executionsession.wait_finished()
-        finally:
-            await executionsession.wait(0)
+def main():
+    args = ClientArgs.ParseForDatasetListOpt(description="Copy selected datasets", init=__initParser)
+    ClientConfig.UpdateProjectFromConfiguration(args)
+    rawclientv2 = RawGenClientV2(**vars(args))
+    clientv2 = MetadataGenClientV2(**vars(args))
+    stageblobs = None
+    input = StagedFilesUploadInputV1()
+    input.files = list()
+
+    if args.datasetids:
+        for dataset in __getSelectedDatasets(rawclientv2, args.sourceprojectid, args.datasetids):
+            print(f"dataset: {dataset}")
+
+            name = dataset.get("name")
+            dataseturl = dataset.get("url")
+
+            if not stageblobs:
+                response = rawclientv2.GetStagingUrls(args.projectid, 10)
+                stageblobs = [x.get("url") for x in response.Body.get("data")]
+            tmpurl = stageblobs.pop()
+
+            print(f"Copy {name} -> {tmpurl}")
+            uploadresult = MetadataClientV2Helper.UploadBlobFromUrl(tmpurl, dataseturl)
+            print(f"  -> uploadresult: {uploadresult}")
+            print(f"  -> copy {name} done")
+
+            file = StagedFileUploadInputV1()
+            file.fileName = name
+            file.url = tmpurl
+            input.files.append(file)
+
+        # wait for copy operations to finish
+        sleep(1.0)
+
+        print(f"Upload staged files")
+        clientv2.UploadStagedFilesV2(input.to_dict(), args.projectid)
+        print(f"  -> upload done")
 
 if __name__ == '__main__':
-    if platform.system() == 'Windows':
-        asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-    asyncio.run(main())
+    main()
```

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/eng/sbmessages.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/eng/sbmessages.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/gw/service.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/gw/service.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/gw/services.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/gw/services.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prj/capabilities.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prj/capabilities.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prj/create.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prj/create.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prj/createsub.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prj/createsub.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prj/info.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prj/info.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prj/infor.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prj/infor.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prj/ls.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prj/ls.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prj/lsh.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prj/lsh.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prj/lsr.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prj/lsr.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prj/path.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prj/path.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prj/prepare.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prj/prepare.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prj/restore.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prj/restore.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prj/rm.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prj/rm.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prj/rmhard.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prj/rmhard.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prj/sas.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prj/sas.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prj/sub.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prj/sub.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prj/update.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prj/update.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prjm/add.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prjm/add.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prjm/all.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prjm/all.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prjm/ls.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prjm/ls.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/prjm/rm.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/prjm/rm.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/raw/blocks.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/raw/blocks.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/raw/checksums.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/raw/checksums.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/raw/copystatus.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/raw/copystatus.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/raw/download.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/raw/download.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/raw/stagingurls.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/raw/stagingurls.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/raw/upload.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/raw/upload.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/rb/ls.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/rb/ls.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/rb/lsmy.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/rb/lsmy.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/rb/restore.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/rb/restore.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/rb/rmds.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/rb/rmds.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/rb/rmprj.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/rb/rmprj.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/reader/info.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/reader/info.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/reader/ls.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/reader/ls.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/tool/openapi2py.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/tool/openapi2py.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     parser.add_argument("-c", "--classname", help="Class name", default="OpenapiClient")
     parser.add_argument("-n", "--classnum", help="First class number", type=int, default=1)
     parser.add_argument("-s", "--dhiservice", help="Platform service id")
     parser.add_argument("-r", "--headerparams", help="Header parameters", metavar="PARAMETERS")
     parser.add_argument("-i", "--inputtoheader", help="Input to header parameters", metavar="INPUTPARAMETERS")
     parser.add_argument("-k", "--kwargsfor", help="Operation to use **kwargs", metavar="OPERATIONS")
     parser.add_argument("-f", "--headersfor", help="Additional headers for endpoints", metavar="HEADERDEF")
+    parser.add_argument("-p", "--skipheadersfor", help="Skip headers for endpoints", metavar="SKIPHEADERDEF")
+    parser.add_argument("-a", "--skipauthfor", help="Skip authentication for endpoints", metavar="SKIPAUTHDEF")
     parser.add_argument("-t", "--datafields", help="Additional data fields for data contracts", metavar="FIELDDEF")
     parser.add_argument("-d", "--includedeprecated", help="Include deprecated methods", metavar="OPERATIONS")
     parser.add_argument("-o", "--output", default="-", help="Write output to a file")
     #parser.add_argument("--relative", help="show relative paths", action="store_false")
     #parser.add_argument("--transitivedeps", help="show transitive dependencies", action="store_false")
     #parser.add_argument("--shownotfound", help="show not found projects", action="store_true")
     #parser.add_argument("--shownotfounddeps", help="show not found dependencies", action="store_true")
@@ -63,14 +65,18 @@
 
 def writeFiles(args, outfile):
     n = 0
     kwargsoperations = set()
     if args.kwargsfor:
         kwargsoperations.update(args.kwargsfor.split(","))
     headersfor = Helper.initheadersfor(args.headersfor)
+    skipheadersfor = Helper.initskipheadersfor(args.skipheadersfor)
+    skipauthfor = set()
+    if args.skipauthfor:
+        skipauthfor.update(args.skipauthfor.split(","))
     datafields = Helper.initdatafields(args.datafields)
     includedeprecated = set()
     if args.includedeprecated:
         includedeprecated.update(args.includedeprecated.split(","))
     headerparams = []
     if args.headerparams:
         headerparams.extend(args.headerparams.split(","))
@@ -78,15 +84,15 @@
     if args.inputtoheader:
         inputtoheader.update(dict([reversed(x.split('=')) for x in args.inputtoheader.split(",")]))
     Helper.writeFileHeader(outfile)
     for inputfile in args.files:
         openapiObj = Helper.getOpenApiObj(inputfile)
         classname = f"{args.classname}{n+args.classnum}"
         suffix = f"V{n+args.classnum}"
-        Helper.generateApiClasses(openapiObj, suffix, inputfile, classname, kwargsoperations, headersfor, datafields, headerparams, inputtoheader, includedeprecated, args.dhiservice, outfile)
+        Helper.generateApiClasses(openapiObj, suffix, inputfile, classname, kwargsoperations, headersfor, skipheadersfor, skipauthfor, datafields, headerparams, inputtoheader, includedeprecated, args.dhiservice, outfile)
         n += 1
         #with urllib.urlopen(f) as response:
         #    obj = json.load(f)
         #    print(obj)
         #    #html = response.read()
 
 def __parseBasic(prog=None, description=None, init=None):
@@ -150,14 +156,30 @@
                     if headers := result.get(op):
                         headers.update(content)
                     else:
                         result[op] = content
         return result
 
     @classmethod
+    def initskipheadersfor(cls, skipheadersfor):
+        result = dict()
+        if skipheadersfor:
+            for h in skipheadersfor.split(","):
+                parts = h.split(":")
+                if len(parts) != 2:
+                    sys.exit(f"wrong format in skip header info (endpoint:header): {h}")
+                if op := parts[0]:
+                    content = set([parts[1]])
+                    if headers := result.get(op):
+                        headers.update(content)
+                    else:
+                        result[op] = content
+        return result
+
+    @classmethod
     def initdatafields(cls, datafields):
         result = dict()
         if datafields:
             for d in datafields.split(","):
                 parts = d.split(":")
                 if len(parts) != 4:
                     sys.exit(f"wrong format in data field info (datacontract:field:type:value): {d}")
@@ -166,28 +188,29 @@
                     if fields := result.get(dc):
                         fields.update(content)
                     else:
                         result[dc] = content
         return result
 
     @classmethod
-    def generateApiClasses(cls, openapiObj, suffix, inputfile, className, kwargsoperations, headersfor, datafields, headerparams, inputtoheader, includedeprecated, service=None, out=sys.stdout):
+    def generateApiClasses(cls, openapiObj, suffix, inputfile, className, kwargsoperations, headersfor, skipheadersfor, skipauthfor, datafields, headerparams, inputtoheader, includedeprecated, service=None, out=sys.stdout):
         info = openapiObj["info"]
         print(file=out)
         print(file=out)
         cls.__writeApiInfo(info, inputfile, out)
         cls.__generateContracts(openapiObj, info, suffix, inputfile, className, kwargsoperations, datafields, headerparams, inputtoheader, includedeprecated, service, out)
-        cls.__generateEndpointsClass(openapiObj, info, suffix, inputfile, className, kwargsoperations, headersfor, headerparams, inputtoheader, includedeprecated, service, out)
+        cls.__generateEndpointsClass(openapiObj, info, suffix, inputfile, className, kwargsoperations, headersfor, skipheadersfor, skipauthfor, headerparams, inputtoheader, includedeprecated, service, out)
 
     @classmethod
     def __writeApiInfo(cls, info, inputfile, out):
         print(f"# {inputfile}", file=out)
         print(f"# {info[cls.TITLE]}", file=out)
         print(f"# {info[cls.DESCRIPTION]}", file=out)
         print(f"# {info[cls.VERSION]}", file=out)
+
     @classmethod
     def __generateContracts(cls, openapiObj, info, suffix, inputfile, className, kwargsoperations, datafields, headerparams, inputtoheader, includedeprecated, service, out):
         if components := openapiObj["components"]:
             if schemas := components["schemas"]:
                 allcontracts = dict()
                 for name, content in schemas.items():
                     allcontracts[name] = ContractInfo(name, content, cls.__getContractDependson(name, content))
@@ -203,14 +226,15 @@
                     top = heapq.heappop(contractslist)
                     name = top.name
                     content = top.content
                     for dep in top.dependsonme:
                         if deponmeitem := allcontracts.get(dep):
                             deponmeitem.refcount -= 1
                     cls.__generateContract(name, datafields.get(name), content, openapiObj, info, suffix, inputfile, className, kwargsoperations, headerparams, inputtoheader, includedeprecated, service, out)
+
     @classmethod
     def __getContractDependson(cls, name, schema):
         result = set()
         if schema.get("type") == "object":
             if parentclassname := cls.__getParentClassType(schema, ""):
                 result.add(parentclassname)
             properties = schema.get("properties")
@@ -220,14 +244,15 @@
                         result.add(propertytype)
                     else:
                         if tmp := propertyinfo.get("type"):
                             if tmp == "array":
                                 #TODO: if it is multidimensional array, it should get nested item type
                                 result.add(cls.__getArrayItemType(propertyinfo, ""))
         return result
+
     @classmethod
     def __generateContract(cls, name, customfields, schema, openapiObj, info, suffix, inputfile, className, kwargsoperations, headerparams, inputtoheader, includedeprecated, service, out):
         classname = f"{name}{suffix}"
         print(file=out)
         if enuminfo := schema.get("enum"):
             print(f"class {classname}(str, Enum):", file=out)
             description = schema.get(cls.DESCRIPTION)
@@ -277,14 +302,15 @@
             print(f"        result.update(cls.__renamed)", file=out)
             print(f"        return result", file=out)
             print("    @classmethod", file=out)
             print(f"    def from_dict(cls: {classname}Type, src_dict: Dict[str, Any]) -> {classname}Type:", file=out)
             print(f"        obj = {classname}()", file=out)
             print(f"        obj.load_dict(src_dict)", file=out)
             print(f"        return obj", file=out)
+
     @classmethod
     def __getPropertyType(cls, propertyinfo, suffix):
         if propertyinfo:
             propertytype = cls.__getParentClassType(propertyinfo, suffix)
             if propertytype:
                 return propertytype
             if type := propertyinfo.get("type"):
@@ -295,52 +321,52 @@
                 elif type == "number":
                     return "float"
                 elif type == "array":
                     return f"List[{cls.__getArrayItemType(propertyinfo, suffix)}]"
                 return "str"
             return cls.__getReftype(propertyinfo.get("$ref"), suffix)
         return None
+
     @classmethod
     def __getArrayItemType(cls, propertyinfo, suffix):
         if itemsinfo := propertyinfo.get("items"):
             if itemtype := cls.__getReftype(itemsinfo.get("$ref"), suffix):
                 return itemtype
             return cls.__getPropertyType(itemsinfo, suffix)
         return None
+
     @classmethod
     def __getParentClassType(cls, schema, suffix):
         if schema:
             if allOf := schema.get("allOf"):
                 for _, reftype in allOf[0].items():
                     return cls.__getReftype(reftype, suffix)
         return None
+
     @classmethod
     def __getReftype(cls, reftype, suffix):
         if reftype:
             if reftype == "string":
                 return "str"
             elif reftype == "integer":
                 return "int"
             elif reftype == "number":
                 return "float"
             elif (reftype.startswith("#/components/schemas/")):
                 tmp = reftype.replace("#/components/schemas/", "")
                 return f"{tmp}{suffix}"
         return reftype
+
     @classmethod
-    def __generateEndpointsClass(cls, openapiObj, info, suffix, inputfile, className, kwargsoperations, headersfor, headerparams, inputtoheader, includedeprecated, service, out):
+    def __generateEndpointsClass(cls, openapiObj, info, suffix, inputfile, className, kwargsoperations, headersfor, skipheadersfor, skipauthfor, addheaderparams, inputtoheader, includedeprecated, service, out):
         print(file=out)
         print(f"class {className}(PlatformClient):", file=out)
         print(f"    def __init__(self, inspectFnc=PlatformClient.DefaultInspectFnc, **kwargs):", file=out)
         includeheaders = f", includeheaders=PlatformClient.GetServiceHeaders({cls.__getInitParam(service)})" if service else ""
         print(f"        super().__init__(inspectFnc{includeheaders}, **kwargs)", file=out)
-        headerparamsstr1 = ", ".join(headerparams)
-        headerparamsstr1 = f", {headerparamsstr1}" if headerparamsstr1 else headerparamsstr1
-        headerparamsstr2 = ", ".join([f"{x}={x}" for x in headerparams]) if headerparams else ""
-        headerparamsstr2 = f", {headerparamsstr2}" if headerparamsstr2 else headerparamsstr2
         for url, ops in openapiObj["paths"].items():
             for method, opObj in ops.items():
                 operation = cls.__getOperationId(opObj, method)
                 if operation and (operation in includedeprecated or not opObj.get("deprecated")):
                     renamedparams = {}
                     queryparams = []
                     queryoptparams = []
@@ -367,14 +393,26 @@
                                 pathparams.append(paramname)
                             elif tmpIn == "header":
                                 headers[paramname] = p[cls.SCHEMA].get(cls.DEFAULT)
                     print(file=out)
                     hfparams = []
                     if hf := headersfor.get(operation):
                         hfparams = [f"{h}={v}" for h, v in hf.items()]
+
+                    opheaderparams = addheaderparams
+                    skiphf = skipheadersfor.get(operation)
+                    if skiphf:
+                        opheaderparams = [x for x in addheaderparams if x not in skiphf]
+                    headerparamsstr1 = ", ".join(opheaderparams)
+                    headerparamsstr1 = f", {headerparamsstr1}" if headerparamsstr1 else headerparamsstr1
+                    headerparamsstr2 = ", ".join([f"{x}={x}" for x in opheaderparams]) if opheaderparams else ""
+                    headerparamsstr2 = f", {headerparamsstr2}" if headerparamsstr2 else headerparamsstr2
+
+                    skipauth = ", noauthentication=True" if operation in skipauthfor else ""
+
                     hfparamsstr = ", ".join(hfparams)
                     hfparamsstr = f", {hfparamsstr}" if hfparamsstr else ""
                     kwargsparam = ", **kwargs" if operation in kwargsoperations or "*" in kwargsoperations else ""
                     print(f"    def {operation}(self{headerparamsstr1}{bodyparam}{cls.__convertParams(pathparams, renamedparams)}{cls.__convertParams(queryparams, renamedparams)}{cls.__convertOptParams(queryoptparams, renamedparams)}{kwargsparam}) -> Response:", file=out)
                     doclines = []
                     if tmp := opObj.get(cls.SUMMARY):
                         doclines.append(tmp)
@@ -393,20 +431,22 @@
                             kwparam = ""
                         print(f"        queryparams = self.GetQueryParams({cls.__convertQueryParams(otherparams, renamedparams)}{kwparam})", file=out)
                         qp = "queryparams"
                     else:
                         qp = "None"
                     ppf = "f" if pathparams else ""
                     requestUrl = cls.__convertUrl(url, renamedparams) if ppf else url
-                    print(f"        return self.{method.capitalize()}Request({ppf}\"{requestUrl}\"{callbodyparam}, {qp}{cls.__convertHeaders(headers)}{headerparamsstr2}{cls.__convertHeaders(headerparams, params=True)}{hfparamsstr}{kwargsparam})", file=out)
+                    print(f"        return self.{method.capitalize()}Request({ppf}\"{requestUrl}\"{callbodyparam}, {qp}{cls.__convertHeaders(headers)}{headerparamsstr2}{cls.__convertHeaders(headerparams, params=True)}{hfparamsstr}{skipauth}{kwargsparam})", file=out)
+
     @staticmethod
     def __printLines(lines, prefix, suffix="", out=sys.stdout):
         if lines:
             for l in lines.splitlines():
                 print(f"{prefix}{l}{suffix}", file=out)
+
     @staticmethod
     def __printLines2(lines, prefix1, prefix2, suffix="", out=sys.stdout):
         if lines:
             firstline = True
             for line in lines:
                 if line:
                     isfirst = firstline
@@ -416,71 +456,83 @@
                             firstline = False
                         else:
                             print(f"{prefix2}{l}", file=out)
                     if isfirst and not firstline:
                         print("", file=out)
             if not firstline:
                 print(suffix, file=out)
+
     @classmethod
     def __getOperationId(cls, op, method):
         #result = op.get(cls.OPERATIONID)
         #tmp = "operation"
         #return result if result else f"{method.capitalize()}Operation{cls.__nextNum(tmp)}"
         result = op.get(cls.OPERATIONID)
         return result.replace(" ", "_") if result else None
+
     @classmethod
     def __nextNum(cls, method):
         num = cls.MethodNumbers.get(method)
         num = num+1 if num else 1
         cls.MethodNumbers[method] = num
         return num
+
     @staticmethod
     def __isReserved(param):
         return param.find("@") >= 0 or param in ["from", "def", "import", "class", "return", "if", "else", "in", "body", "array"]
+
     @staticmethod
     def __mangleReserved(param, renamedparams):
         attempt = 0
         p = param
         while True:
             attempt += 1
             if attempt == 1 and p.find("@") >= 0:
                 p = p.replace("@", "_")
             else:
                 #p = f"{param}param{random.randint(0, 1000)}"
                 p = f"{p}_"
             if p not in renamedparams:
                 return p 
+
     @classmethod
     def __safeParam(cls, param, renamedparams):
         return cls.__mangleReserved(param, renamedparams) if cls.__isReserved(param) else param
+
     @classmethod
     def __convertReservedParams(cls, params, renamedparams):
         return ", ".join([f"\"{x}\": {renamedparams.get(x)}" for x in params])
+
     @classmethod
     def __convertParams(cls, params, renamedparams, sep=", ", withprefix=True):
         result = sep.join([renamedparams.get(x) for x in params])
         return f"{sep}{result}" if result and withprefix else result
+
     @classmethod
     def __convertOptParams(cls, params, renamedparams, sep=", ", withprefix=True):
         result = sep.join([f"{renamedparams.get(x)}=None" for x in params])
         return f"{sep}{result}" if result and withprefix else result
+
     @staticmethod
     def __convertQueryParams(params, renamedparams, sep=", ", withprefix=False):
         result = sep.join([f"{x}={renamedparams.get(x)}" for x in params])
         return f"{sep}{result}" if result and withprefix else result
+
     @staticmethod
     def __convertHeaders(headers, sep=", ", withprefix=True, params=False):
         fixvarname = lambda x: x.replace("-", "_")
         rightside = (lambda x: x) if params else (lambda x: f"\"{x}\"")
         tmp = [f"{fixvarname(n)}={rightside(v)}" for n, v in headers.items()]
         result = sep.join(tmp)
         return f"{sep}{result}" if result and withprefix else result
+
     @staticmethod
     def __convertUrl(url, renamedparams):
         pattern = re.compile(r'{([^}]*)}')
         return pattern.sub(lambda m: f"{{{renamedparams.get(m.group(1))}}}", url)
+
     @staticmethod
     def __getInitParam(value):
         return f"\"{value}\"" if value else "None"
 
 if __name__ == '__main__':
     main()
```

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/tr/download.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/tr/download.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/tr/info.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/tr/info.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/tr/ls.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/tr/ls.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/tr/lss.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/tr/lss.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ts/add.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ts/add.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ts/dscreate.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ts/dscreate.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ts/dsinfo.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ts/dsinfo.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ts/info.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ts/info.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/ts/list.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/ts/list.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/writer/info.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/writer/info.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/cli/writer/ls.py` & `dhi-platform-1.0.7/src/dhi/platform/cli/writer/ls.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/commonmodels.py` & `dhi-platform-1.0.7/src/dhi/platform/commonmodels.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/config.py` & `dhi-platform-1.0.7/src/dhi/platform/config.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/engine.py` & `dhi-platform-1.0.7/src/dhi/platform/engine.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/enginehelper.py` & `dhi-platform-1.0.7/src/dhi/platform/enginehelper.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/eventing.py` & `dhi-platform-1.0.7/src/dhi/platform/eventing.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/eventinghelper.py` & `dhi-platform-1.0.7/src/dhi/platform/eventinghelper.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/fmt.py` & `dhi-platform-1.0.7/src/dhi/platform/fmt.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/generated/enginegen.py` & `dhi-platform-1.0.7/src/dhi/platform/generated/enginegen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated using openapi2py.py
-# openapi2py.py "--dhiservice" "engine" "--classname" "EngineGenClientV" "-n" "2" "-r" "projectid" "-f" "RunExecutionWithPlatformData:recursivetoken:true" "--out" "C:\work\devops\mike-platform-sdk-py\src\dhi\platform\generated\enginegen.py" "https://apispec-mike-platform-dev0.eu.mike-cloud-dev0.com/engine/v2"
-# 2022-04-28 08:13:38.410516Z
+# openapi2py.py "--dhiservice" "engine" "--classname" "EngineGenClientV" "-n" "2" "-r" "projectid" "-p" "GetAllConfigurations:projectid,GetAllEngines:projectid,GetEngine:projectid,GetMyExecutions:projectid" "-f" "RunExecutionWithPlatformData:recursivetoken:true" "-a" "GetAllConfigurations,GetAllEngines,GetEngine" "--out" "C:\work\devops\mike-platform-sdk-py\src\dhi\platform\generated\enginegen.py" "https://apispec-mike-platform-dev0.eu.mike-cloud-dev0.com/engine/v2"
+# 2023-02-21 10:07:18.820338Z
 from typing import Any, Dict, List, NewType, Type, TypeVar, Union
 from enum import Enum
 import attr
 from ..base.client import DataContract, PlatformClient, Response
 
 
 # https://apispec-mike-platform-dev0.eu.mike-cloud-dev0.com/engine/v2
@@ -172,14 +172,15 @@
     engine: str = None
     version: str = None
     resultsRelativePath: str = None
     overwriteResultsIfExists: str = None
     runParameters: List[EngineRunParameterV2] = None
     reportLogUpdatesLines: int = None
     logFiles: List[str] = None
+    terminateOnNoProgressForSec: int = None
     __renamed = {  }
     def to_dict(self) -> Dict[str, Any]:
         return self.get_dictionary(self.get_renamed())
     def load_dict(self, src_dict: Dict[str, Any]) -> None:
         DataContract.load_from_directory(self, src_dict, self.get_renamed())
     @classmethod
     def get_renamed(cls) -> Dict[str, str]:
@@ -219,32 +220,32 @@
         return result
     @classmethod
     def from_dict(cls: ProblemDetailsV2Type, src_dict: Dict[str, Any]) -> ProblemDetailsV2Type:
         obj = ProblemDetailsV2()
         obj.load_dict(src_dict)
         return obj
 
-ValidationProblemDetailsV2Type = TypeVar("ValidationProblemDetailsV2Type", bound="ValidationProblemDetailsV2")
+HttpValidationProblemDetailsV2Type = TypeVar("HttpValidationProblemDetailsV2Type", bound="HttpValidationProblemDetailsV2")
 
 @attr.s(auto_attribs=True)
-class ValidationProblemDetailsV2(ProblemDetailsV2):
+class HttpValidationProblemDetailsV2(ProblemDetailsV2):
     errors: str = None
     __renamed = {  }
     def to_dict(self) -> Dict[str, Any]:
         return self.get_dictionary(self.get_renamed())
     def load_dict(self, src_dict: Dict[str, Any]) -> None:
         DataContract.load_from_directory(self, src_dict, self.get_renamed())
     @classmethod
     def get_renamed(cls) -> Dict[str, str]:
         result = ProblemDetailsV2.get_renamed().copy()
         result.update(cls.__renamed)
         return result
     @classmethod
-    def from_dict(cls: ValidationProblemDetailsV2Type, src_dict: Dict[str, Any]) -> ValidationProblemDetailsV2Type:
-        obj = ValidationProblemDetailsV2()
+    def from_dict(cls: HttpValidationProblemDetailsV2Type, src_dict: Dict[str, Any]) -> HttpValidationProblemDetailsV2Type:
+        obj = HttpValidationProblemDetailsV2()
         obj.load_dict(src_dict)
         return obj
 
 EngineGetOutputV2Type = TypeVar("EngineGetOutputV2Type", bound="EngineGetOutputV2")
 
 @attr.s(auto_attribs=True)
 class EngineGetOutputV2(DataContract):
@@ -487,14 +488,15 @@
     uri: str = None
     localPath: str = None
     engine: str = None
     version: str = None
     runParameters: List[EngineRunParameterV2] = None
     reportLogUpdatesLines: int = None
     logFiles: List[str] = None
+    terminateOnNoProgressForSec: int = None
     __renamed = {  }
     def to_dict(self) -> Dict[str, Any]:
         return self.get_dictionary(self.get_renamed())
     def load_dict(self, src_dict: Dict[str, Any]) -> None:
         DataContract.load_from_directory(self, src_dict, self.get_renamed())
     @classmethod
     def get_renamed(cls) -> Dict[str, str]:
@@ -644,31 +646,31 @@
 
     def GetAllConfigurations(self) -> Response:
         """Get the list of hardware configurations.
 
         Configuration
         GET /api/compute/configuration/list
         """
-        return self.GetRequest("/api/compute/configuration/list", None, api_version="2")
+        return self.GetRequest("/api/compute/configuration/list", None, api_version="2", noauthentication=True)
 
     def GetAllEngines(self) -> Response:
         """Get the list of registered engines/tools.
 
         Engine
         GET /api/compute/engine/list
         """
-        return self.GetRequest("/api/compute/engine/list", None, api_version="2")
+        return self.GetRequest("/api/compute/engine/list", None, api_version="2", noauthentication=True)
 
     def GetEngine(self, name) -> Response:
         """Get the engine/tool information.
 
         Engine
         GET /api/compute/engine/{name}
         """
-        return self.GetRequest(f"/api/compute/engine/{name}", None, api_version="2")
+        return self.GetRequest(f"/api/compute/engine/{name}", None, api_version="2", noauthentication=True)
 
     def RunExecution(self, projectid, body) -> Response:
         """Run the engine/tool with input data from any blob storage. Create permission on the project is required.
 
         Execution
         POST /api/compute/execution
         """
@@ -679,22 +681,22 @@
 
         Execution
         GET /api/compute/execution/list
         """
         queryparams = self.GetQueryParams(startTime=starttime, endTime=endtime, cursor=cursor)
         return self.GetRequest("/api/compute/execution/list", queryparams, api_version="2", projectid=projectid)
 
-    def GetMyExecutions(self, projectid, sortby=None, sortorder=None, starttime=None, endtime=None, scenarioname=None, status=None, project=None, limit=None, cursor=None) -> Response:
+    def GetMyExecutions(self, sortby=None, sortorder=None, starttime=None, endtime=None, scenarioname=None, status=None, project=None, limit=None, cursor=None) -> Response:
         """Get information about executions run by the user.
 
         Execution
         GET /api/compute/execution/my-list
         """
         queryparams = self.GetQueryParams(sortBy=sortby, sortOrder=sortorder, startTime=starttime, endTime=endtime, scenarioName=scenarioname, status=status, project=project, limit=limit, cursor=cursor)
-        return self.GetRequest("/api/compute/execution/my-list", queryparams, api_version="2", projectid=projectid)
+        return self.GetRequest("/api/compute/execution/my-list", queryparams, api_version="2")
 
     def RunExecutionWithPlatformData(self, projectid, body) -> Response:
         """Run the engine/tool with input data from MIKE Cloud Platform. Create permission on the project is required.
 
         Execution
         POST /api/compute/execution/platform
         """
```

### Comparing `dhi-platform-1.0.6/src/dhi/platform/generated/gisgen.py` & `dhi-platform-1.0.7/src/dhi/platform/generated/gisgen.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/generated/metadatagen.py` & `dhi-platform-1.0.7/src/dhi/platform/generated/metadatagen.py`

 * *Files 0% similar despite different names*

```diff
@@ -3144,15 +3144,15 @@
 
 StagedFilesUploadInputV1Type = TypeVar("StagedFilesUploadInputV1Type", bound="StagedFilesUploadInputV1")
 
 @attr.s(auto_attribs=True)
 class StagedFilesUploadInputV1(DataContract):
     files: List[StagedFileUploadInputV1] = None
     destinationPath: str = None
-    createDestinationPathIfNotExists: str = None
+    createDestinationPathIfNotExists: bool = None
     __renamed = {  }
     def to_dict(self) -> Dict[str, Any]:
         return self.get_dictionary(self.get_renamed())
     def load_dict(self, src_dict: Dict[str, Any]) -> None:
         DataContract.load_from_directory(self, src_dict, self.get_renamed())
     @classmethod
     def get_renamed(cls) -> Dict[str, str]:
```

### Comparing `dhi-platform-1.0.6/src/dhi/platform/generated/multidimensionalgen.py` & `dhi-platform-1.0.7/src/dhi/platform/generated/multidimensionalgen.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/generated/pubsubgen.py` & `dhi-platform-1.0.7/src/dhi/platform/generated/pubsubgen.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/generated/rawgen.py` & `dhi-platform-1.0.7/src/dhi/platform/generated/rawgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -574,24 +574,24 @@
     def GetFilesChecksums(self, projectid, id=None) -> Response:
         """Get checksums for selected or all files in a folder.
 
         FileSync
         GET /api/filesync/checksums
         """
         queryparams = self.GetQueryParams(id=id)
-        return self.GetRequest("/api/filesync/checksums", queryparams, api_version="2", projectid=projectid, datasetid=id)
+        return self.GetRequest("/api/filesync/checksums", queryparams, api_version="2", projectid=projectid)
 
     def GetDownloadDatasets(self, projectid, id=None) -> Response:
         """Get download info for selected or all files in a folder.
 
         FileSync
         GET /api/filesync/prepare-download
         """
         queryparams = self.GetQueryParams(id=id)
-        return self.GetRequest("/api/filesync/prepare-download", queryparams, api_version="2", projectid=projectid, datasetid=id)
+        return self.GetRequest("/api/filesync/prepare-download", queryparams, api_version="2", projectid=projectid)
 
     def UploadBulkFiles(self, projectid, body) -> Response:
         """Upload file datasets from the staging area or another storage.
         Files in the staging area moved, all other files are copied.
         Check the copy operations with "POST /api/filesync/upload/status".
 
         FileSync
```

### Comparing `dhi-platform-1.0.6/src/dhi/platform/generated/sharinggen.py` & `dhi-platform-1.0.7/src/dhi/platform/generated/sharinggen.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/generated/tilesgen.py` & `dhi-platform-1.0.7/src/dhi/platform/generated/tilesgen.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/generated/timeseriesgen.py` & `dhi-platform-1.0.7/src/dhi/platform/generated/timeseriesgen.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/gis.py` & `dhi-platform-1.0.7/src/dhi/platform/gis.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/metadata.py` & `dhi-platform-1.0.7/src/dhi/platform/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -899,31 +899,32 @@
         :param includesastokens: if True, the response will include sas tokens where possible, default is False
         :return: Generator of DatasetOutput instances
         """
         response = self._client3.GetDatasetListV3(project_id, includesastokens=includesastokens)
         data = response.Body["data"]
         return (DatasetOutput.from_dict(d) for d in data)
 
-    def list_datasets_recursive(self, project_id, includesastokens:bool=False, dataset_type:DatasetType=None) -> Generator[DatasetOutput, None, None]:
+    def list_datasets_recursive(self, project_id, includesastokens:bool=False, dataset_type:DatasetType=None) -> Generator[DatasetRecursiveListOutput, None, None]:
         """
         List datasets in a project recursively
         
         :param project_id: ID of the project where the datasets reside
         :param includesastokens: if True, the response will include sas tokens where possible, default is False
         :param dataset_type: Return only datasets of selected dataset type, default is None for all dataset types
         :return: Generator of DatasetRecursiveListOutput instances
         """
         limit = 1000
         offset = 0
         first_query = True
+        request_dataset_type = getattr(dataset_type, 'name', None)
         while True:
             if not first_query:
                 if not response.Body["data"]:
                     break
-            response = self._client3.GetRecursiveDatasetListV3(project_id, offset=offset, limit=limit, includesastokens=includesastokens, datasettype=dataset_type)
+            response = self._client3.GetRecursiveDatasetListV3(project_id, offset=offset, limit=limit, includesastokens=includesastokens, datasettype=request_dataset_type)
             for i in response.Body["data"]:
                 yield DatasetRecursiveListOutput.from_dict(i)
             offset = offset + limit + 1
             first_query = False
 
     def get_dataset(self, dataset_id):
         """
```

### Comparing `dhi-platform-1.0.6/src/dhi/platform/metadatahelper.py` & `dhi-platform-1.0.7/src/dhi/platform/metadatahelper.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 import itertools
 import os
+from types import SimpleNamespace
 from .base.client import Contracts
 from .generated.metadatagen import MetadataGenClientV2
 
 
 class MetadataClientV2Helper:
     @classmethod
     def UploadFromFile(cls, filepath, clientv2: MetadataGenClientV2):
@@ -38,14 +39,27 @@
     @staticmethod
     def UploadBlobFromFile(url, filepath):
         from azure.storage.blob import BlobClient
         blob = BlobClient.from_blob_url(url)
         with open(filepath, "rb") as f:
             blob.upload_blob(f)
 
+    @classmethod
+    def UploadFromUrl(cls, url, clientv2: MetadataGenClientV2):
+        uploadurlresponse = clientv2.GetUploadUrlV2()
+        uploadurl = uploadurlresponse.Body.get("data")
+        cls.UploadBlobFromUrl(uploadurl, url)
+        return uploadurl
+
+    @staticmethod
+    def UploadBlobFromUrl(url, sourceurl):
+        from azure.storage.blob import BlobClient
+        blob = BlobClient.from_blob_url(url)
+        return blob.start_copy_from_url(sourceurl)
+
     @staticmethod
     def DownloadBlobToFile(url, filepath):
         from azure.storage.blob import BlobClient
         blob = BlobClient.from_blob_url(url)
         download = blob.download_blob()
         if not filepath:
             filepath = os.path.basename(download.name)
@@ -58,14 +72,21 @@
     @staticmethod
     def DeleteBlob(url):
         from azure.storage.blob import BlobClient
         blob = BlobClient.from_blob_url(url)
         if blob.exists():
             blob.delete_blob()
 
+    @staticmethod
+    def ListBlobs(url, prefix):
+        from azure.storage.blob import ContainerClient
+        container = ContainerClient.from_container_url(url)
+        for blob in container.list_blobs(prefix):
+            blobclient = container.get_blob_client(blob.name)
+            yield SimpleNamespace(url = blobclient.url, name = blob.name)
 
 class MetadataClientV2Contracts(Contracts):
     @classmethod
     def PrepareUploadStagedFilesInput(cls, input=None, uploadurl=None, filename=None, destinationpath=None, createdestinationpathifnotexists=None):
         body = input.copy() if input else {}
         files = body.get("files")
         if not files:
```

### Comparing `dhi-platform-1.0.6/src/dhi/platform/multidimensional.py` & `dhi-platform-1.0.7/src/dhi/platform/multidimensional.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/protobufparser/api_implementation.py` & `dhi-platform-1.0.7/src/dhi/platform/protobufparser/api_implementation.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/protobufparser/containers.py` & `dhi-platform-1.0.7/src/dhi/platform/protobufparser/containers.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/protobufparser/decoder.py` & `dhi-platform-1.0.7/src/dhi/platform/protobufparser/decoder.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/protobufparser/decoderdatetime.py` & `dhi-platform-1.0.7/src/dhi/platform/protobufparser/decoderdatetime.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/protobufparser/descriptor.py` & `dhi-platform-1.0.7/src/dhi/platform/protobufparser/descriptor.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/protobufparser/encoder.py` & `dhi-platform-1.0.7/src/dhi/platform/protobufparser/encoder.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/protobufparser/enums.py` & `dhi-platform-1.0.7/src/dhi/platform/protobufparser/enums.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/protobufparser/message.py` & `dhi-platform-1.0.7/src/dhi/platform/protobufparser/message.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/protobufparser/wire_format.py` & `dhi-platform-1.0.7/src/dhi/platform/protobufparser/wire_format.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/pubsub.py` & `dhi-platform-1.0.7/src/dhi/platform/pubsub.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/raw.py` & `dhi-platform-1.0.7/src/dhi/platform/raw.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/rawhelper.py` & `dhi-platform-1.0.7/src/dhi/platform/rawhelper.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/sharing.py` & `dhi-platform-1.0.7/src/dhi/platform/tiles.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-from .generated.sharinggen import SharingGenClientV1
+from .generated.tilesgen import TilesGenClientV1
 
-class SharingClientV1(SharingGenClientV1):
-    def __init__(self, inspectFnc=SharingGenClientV1.DefaultInspectFnc, **kwargs):
+class TilesClientV1(TilesGenClientV1):
+    def __init__(self, inspectFnc=TilesGenClientV1.DefaultInspectFnc, **kwargs):
         super().__init__(inspectFnc, **kwargs)
 
 
 if __name__ == '__main__':
     print(__file__)
     print(dir())
```

### Comparing `dhi-platform-1.0.6/src/dhi/platform/tests/data/EqD2.dfs2` & `dhi-platform-1.0.7/src/dhi/platform/tests/data/EqD2.dfs2`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/tests/engine_tests.py` & `dhi-platform-1.0.7/src/dhi/platform/tests/engine_tests.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/tests/exceptions_test.py` & `dhi-platform-1.0.7/src/dhi/platform/tests/exceptions_test.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/tests/metadata_dataset_test.py` & `dhi-platform-1.0.7/src/dhi/platform/tests/metadata_dataset_test.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/tests/metadata_project_test.py` & `dhi-platform-1.0.7/src/dhi/platform/tests/metadata_project_test.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/tests/multidimensional_test.py` & `dhi-platform-1.0.7/src/dhi/platform/tests/multidimensional_test.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/tests/timeseries_test.py` & `dhi-platform-1.0.7/src/dhi/platform/tests/timeseries_test.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/tests/transfer_test.py` & `dhi-platform-1.0.7/src/dhi/platform/tests/transfer_test.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/tests/transfer_tests_integration.py` & `dhi-platform-1.0.7/src/dhi/platform/tests/transfer_tests_integration.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,45 @@
+from pathlib import Path
 import unittest
 import datetime
 from unittest.case import _AssertRaisesContext
-import uuid
+import tempfile
 
 from dhi.platform import metadata, transfer
 from .testcredentials import TEST_IDENTITY
 import os
 import hashlib
 import requests
 
 class TestTransferTestIntegration(unittest.TestCase):
 
     _verbosity = 0
     _project_id = None
+    _projects_to_remove = []
     
     def setUp(self) -> None:
         self._metadataclient = metadata.MetadataClient(verbose=self._verbosity, identity=TEST_IDENTITY)
         self._transferclient = transfer.TransferClient(verbose=self._verbosity, identity=TEST_IDENTITY)
         self._test_data_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
         
         if not self._project_id:
             stamp = datetime.datetime.now().strftime('%Y%m%d%H%M%S')
             name = 'Python test ' + stamp
             projectInput = metadata.CreateProjectInput(name, 'Project created by Python SDK test')
             project = self._metadataclient.create_project(projectInput)
             self._project_id = project.id
+            self._projects_to_remove.append(self._project_id)
 
             self._temp_dir = os.path.join(self._test_data_dir, 'temp' + stamp)
             os.mkdir(self._temp_dir)
 
     def tearDown(self) -> None:
         super().tearDown()
-        if self._project_id:
-            self._metadataclient.delete_project(self._project_id, permanently=True)
+        for pid in self._projects_to_remove:
+            self._metadataclient.delete_project(pid, permanently=True)
         
         if os.path.exists(self._temp_dir):
             import shutil
             shutil.rmtree(self._temp_dir)
 
     def test_get_readers_is_ok(self):
         readers = self._transferclient.get_readers()
@@ -146,11 +149,53 @@
             local_md5 = hashlib.md5(stream.read()).digest()
         
         processed_md5 = ''
         with open(processed_file, 'rb') as stream:
             processed_md5 = hashlib.md5(stream.read()).digest()
         
         self.assertEqual(local_md5, processed_md5)
+
+    def test_folder_project_upload_download(self):
+
+        stamp = datetime.datetime.now().strftime('%Y%m%d%H%M%S')
+        name = 'Python test ' + stamp
+        projectInput = metadata.CreateProjectInput(name, 'Project created by Python SDK test')
+        project = self._metadataclient.create_project(projectInput)
+        self._projects_to_remove.append(project.id)
+
+        temp_dir = tempfile.gettempdir()
+        root_dir = os.path.join(temp_dir, f'foo{stamp}')
+        Path(root_dir).mkdir(parents=True, exist_ok=True)
+        
+        files = [
+            'aaa/one.csv',
+            'aaa/two.csv',
+            'bbb/alfa.dat',
+            'bbb/beta.dat',
+            'bbb/gamma.dat',
+            'bbb/bbb1/ein.nc',
+            'bbb/bbb2/uno.txt',
+            'bbb/bbb2/due.txt',
+            'bbb/bbb2/tres.txt',
+            'ccc/dva.shp',
+            'ccc/jeden.shp'
+        ]
+
+        # create tree structure of files
+        for f in files:
+            file_path = os.path.join(root_dir, f)
+            Path(os.path.dirname(file_path)).mkdir(parents=True, exist_ok=True)
+            with open(file_path, 'w') as o:
+                o.write("hello\n")
+        
+        # create empty folder
+        Path(os.path.join(root_dir, 'ccc', 'ccc1')).mkdir(parents=True, exist_ok=True)
+        
+        uploaded = self._transferclient.upload_folder_to_project(root_dir, project.id)
+        downloaded = self._transferclient.download_project_to_folder(project.id, root_dir)
+
+        for d in downloaded:
+            os.remove(d)
         
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `dhi-platform-1.0.6/src/dhi/platform/tests/upload_download_test.py` & `dhi-platform-1.0.7/src/dhi/platform/tests/upload_download_test.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/timeseries.py` & `dhi-platform-1.0.7/src/dhi/platform/timeseries.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/timeserieshelper.py` & `dhi-platform-1.0.7/src/dhi/platform/timeserieshelper.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.6/src/dhi/platform/transfer.py` & `dhi-platform-1.0.7/src/dhi/platform/transfer.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,28 +18,29 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 import os
+from pathlib import Path
 import time
 import uuid
 import datetime
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Generator, List, Tuple
 from dhi.platform.base.exceptions import MikeCloudException
 from dhi.platform.raw import RawClientV2
-from dhi.platform.transferuploadhelper import TransferUploadHelper
+from dhi.platform.transferhelper import TransferUploadHelper, download_file
 from .generated.metadatagen import MetadataGenClientV1
-from .metadata import MetadataClientV2, MetadataClientV3
+from .metadata import MetadataClient, MetadataClientV2, MetadataClientV3, SubprojectInput
 from .base import constants
 from azure.storage.blob import BlobClient
-from .commonmodels import PropertyDefinition, ItemId, TemporalValueFilter, UnitId, SpatialFilter, TemporalFilter, VerticalFilter
+from .commonmodels import DatasetType, PropertyDefinition, ItemId, TemporalValueFilter, UnitId, SpatialFilter, TemporalFilter, VerticalFilter
 
 
 class ParameterDefinition:
     def __init__(self, name:str, description:str, data_type:str, required:bool, default:object=None, allowed:Tuple[object]=None) -> None:
         self._name = name
         self._description = description
         self._data_type = data_type
@@ -1917,14 +1918,15 @@
 
 
 class TransferClient():
     
     def __init__(self, inspectFnc=MetadataGenClientV1.DefaultInspectFnc, **kwargs):
         self._metadata2 = kwargs.get("MetadataClientV2", MetadataClientV2(inspectFnc, **kwargs))
         self._metadata3 = kwargs.get("MetadataClientV3", MetadataClientV3(inspectFnc, **kwargs))
+        self._metadata_client = kwargs.get("MetadataClient", MetadataClient(inspectFnc, **kwargs))
         self._raw2 = kwargs.get("RawClientV2", RawClientV2(inspectFnc, **kwargs))
         self._transfer_upload_helper = TransferUploadHelper(self._metadata2)
         self._transfer_process_invoker = TransferProcessInvoker(self._metadata2, self._metadata3, self._transfer_upload_helper)
         self._transfer_process_awaiter = TransferProcessAwaiter(self._metadata2)
 
     def upload_file(self, local_file_path:str, project_id:str, name:str=None, description:str=None, metadata:dict=None, verbose:bool=False, timeout=60, reporter=lambda message: print(message)) -> str:
         """
@@ -2346,12 +2348,139 @@
         :param project_id: Project id
         :param input: Info about uploaded files
         :return: Info about succeeded and failed uploads
         :rtype: StagedFilesUploadOutput
         """
         response = self._metadata2.UploadStagedFilesV2(input.body(), project_id)
         return StagedFilesUploadOutput.from_body(response.Body)
+    
+    def _get_or_create_subproject(self, project_id, path, description="", members=None, metadata=None):
+        name = os.path.basename(path)
+        existing_subprojects = self._metadata_client.list_subprojects(project_id)
+        existing_subproject = [p for p in existing_subprojects if p.name == name]
+        if len(existing_subproject) > 0:
+            return existing_subproject[0].id
+        else:
+            subproject = self._metadata_client.create_subproject(project_id, SubprojectInput(name, description, metadata, members))
+            return subproject.id
+
+    def _upload_files_to_project(self, project_id, files:list, progress_reporter = None) -> List[str]:
+        uploaded = []
+        for f in files:
+
+            if progress_reporter is not None:
+                progress_reporter(f)
+
+            dataset_id = self.upload_file(f, project_id)
+            uploaded.append((f, project_id, dataset_id))
+        
+        return uploaded
+
+    def _remove_existing_datasets(self, subproject_id:str, files:List[str], permanently):
+        datasets = self._metadata_client.list_datasets(subproject_id)
+        dataset_lookup = dict([(d.name, d.id) for d in datasets])
+        for f in files:
+            name = os.path.basename(f)
+            if name in dataset_lookup:
+                self._metadata_client.delete_dataset(dataset_lookup[name], permanently=permanently)
+    
+    def upload_folder_to_project(self, directory, project_id, overwrite=True, filter=None, permanently=False, progress_reporter=lambda p: print(p)) -> List[tuple]:
+        """
+        Upload folder recursively to a project. Files are uploaded as 'File' datasets.
+
+        Note that 'overwrite' parameter affects only datasets. If a subproject with the same name exists, it is reused. 
+        This can lead to problems when for example the identity has right to read the project but not upload data there.
+        To avoid any of these problems, upload to an empty project.
+
+        :param directory: Local directory to upload from
+        :param project_id: ID of the project to upload to
+        :param overwrite: Overwrite datasets with the same name if they already exist, default is True.
+        :param filter: Callable that takes local file path and returns True if the dataset should be downloaded. Default is None for all files. Note that this does not affect folders.
+        :param progress_reporter: Callable that takes file path as parameter and prints a message when uploading the file. Set to None for no reporting.
+        :param permanently: If overwrite is True. If True, datasets with conflicting names will be permanently removed, if False, they will only be moved to recycle bin
+        :return: Generator of uploaded (file path, project id, dataset id)
+        :rtype: Generator[str, str, str]
+        """
+        results = []
+
+        projects = {directory: project_id}
+
+        files = [os.path.join(directory, f) for f in os.listdir(directory) if os.path.isfile(os.path.join(directory, f))]
+
+        if filter is not None:
+            files = [f for f in files if filter(f)]
+
+        if overwrite:
+            self._remove_existing_datasets(project_id, files, permanently)
+
+        self._upload_files_to_project(project_id, files, progress_reporter)
+
+        for (dirpath, dirnames, filenames) in os.walk(directory):
+            if dirpath != directory:
+                parent_folder = os.path.dirname(dirpath)
+                parent_project_id = projects.get(parent_folder, None)
+                
+                if parent_project_id is None:
+                    raise Exception(f'Invalid folder, no parent project id found for folder {parent_folder}')
+                
+                subproject_id = projects.get(dirpath, None)
+                if subproject_id is None:
+                    subproject_id = self._get_or_create_subproject(parent_project_id, dirpath)
+                    projects[dirpath] = subproject_id
+
+                files = [os.path.join(dirpath, f) for f in filenames]
+
+                if filter is not None:
+                    files = [f for f in files if filter(f)]
+
+                if overwrite:
+                    self._remove_existing_datasets(subproject_id, files, permanently)
+                    
+                uploaded = self._upload_files_to_project(subproject_id, files, progress_reporter)
+                for u in uploaded:
+                    results.append(u)
+
+        return results
+
+
+    def download_project_to_folder(self, project_id, directory, overwrite = True, filter = None, progress_reporter=lambda d: print(os.path.join(d.relativePath, d.name))) -> List[str]:
+        """
+        Download project content recursively to local folder. Only 'File' datasets are downloaded.
+
+        :param project_id: ID of the project to download from
+        :param directory: Local directory to download to. It will be created if not exists
+        :param overwrite: Overwrite files if they already exists, default is True
+        :param filter: Callable that takes DatasetRecursiveListOutput and returns True if the dataset should be downloaded. Default is None for all files.
+        :param progress_reporter: Callable that takes DatasetRecursiveListOutput and prints a message when downloading the file. Set to None for no reporting.
+        :return: List of downloaded file paths
+        :rtype: List[str]
+        """
+        file_paths = []
+        
+        datasets = self._metadata_client.list_datasets_recursive(project_id, includesastokens = True, dataset_type = DatasetType.FILE)
+        for d in datasets:
+            dirpath = os.path.join(directory, d.relativePath)
+            Path(dirpath).mkdir(parents=True, exist_ok=True)
+            file_path = os.path.join(dirpath, d.name)
+            
+            if filter is not None:
+                if not filter(d):
+                    continue
+            
+            if progress_reporter is not None:
+                progress_reporter(d)
+            
+            if os.path.isfile(file_path):
+                if overwrite:
+                    os.remove(file_path)
+                    download_file(d.datasetUrl, file_path)
+                    file_paths.append(file_path)
+            else:
+                download_file(d.datasetUrl, file_path)
+                file_paths.append(file_path)
+        
+        return file_paths
 
 
 if __name__ == '__main__':
     print(__file__)
     print(dir())
```

### Comparing `dhi-platform-1.0.6/src/dhi_platform.egg-info/PKG-INFO` & `dhi-platform-1.0.7/src/dhi_platform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhi-platform
-Version: 1.0.6
+Version: 1.0.7
 Summary: MIKE Cloud Platform SDK for Python
 Home-page: https://develop.mike-cloud.com/
 Author: DHI
 Author-email: wdpservice@dhigroup.com
 License: MIT License
 Project-URL: Open API, https://develop.mike-cloud.com/swagger/index.html
 Project-URL: Documentation, https://develop.mike-cloud.com/docs/
```

### Comparing `dhi-platform-1.0.6/src/dhi_platform.egg-info/SOURCES.txt` & `dhi-platform-1.0.7/src/dhi_platform.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,34 +12,38 @@
 src/dhi/platform/config.py
 src/dhi/platform/engine.py
 src/dhi/platform/enginehelper.py
 src/dhi/platform/eventing.py
 src/dhi/platform/eventinghelper.py
 src/dhi/platform/fmt.py
 src/dhi/platform/gis.py
+src/dhi/platform/job.py
 src/dhi/platform/metadata.py
 src/dhi/platform/metadatahelper.py
 src/dhi/platform/multidimensional.py
 src/dhi/platform/pubsub.py
 src/dhi/platform/raw.py
 src/dhi/platform/rawhelper.py
 src/dhi/platform/sharing.py
 src/dhi/platform/tiles.py
 src/dhi/platform/timeseries.py
 src/dhi/platform/timeserieshelper.py
 src/dhi/platform/transfer.py
-src/dhi/platform/transferuploadhelper.py
+src/dhi/platform/transferhelper.py
 src/dhi/platform/base/client.py
 src/dhi/platform/base/constants.py
 src/dhi/platform/base/exceptions.py
 src/dhi/platform/base/utils.py
 src/dhi/platform/cli/help.py
 src/dhi/platform/cli/cfg/login.py
 src/dhi/platform/cli/ds/append.py
 src/dhi/platform/cli/ds/convert.py
+src/dhi/platform/cli/ds/cp.py
+src/dhi/platform/cli/ds/cpbh.py
+src/dhi/platform/cli/ds/cph.py
 src/dhi/platform/cli/ds/download.py
 src/dhi/platform/cli/ds/downloadc.py
 src/dhi/platform/cli/ds/info.py
 src/dhi/platform/cli/ds/infor.py
 src/dhi/platform/cli/ds/ls.py
 src/dhi/platform/cli/ds/lsh.py
 src/dhi/platform/cli/ds/lsra.py
@@ -107,14 +111,15 @@
 src/dhi/platform/cli/ts/dsinfo.py
 src/dhi/platform/cli/ts/info.py
 src/dhi/platform/cli/ts/list.py
 src/dhi/platform/cli/writer/info.py
 src/dhi/platform/cli/writer/ls.py
 src/dhi/platform/generated/enginegen.py
 src/dhi/platform/generated/gisgen.py
+src/dhi/platform/generated/jobgen.py
 src/dhi/platform/generated/metadatagen.py
 src/dhi/platform/generated/multidimensionalgen.py
 src/dhi/platform/generated/pubsubgen.py
 src/dhi/platform/generated/rawgen.py
 src/dhi/platform/generated/sharinggen.py
 src/dhi/platform/generated/tilesgen.py
 src/dhi/platform/generated/timeseriesgen.py
@@ -127,17 +132,19 @@
 src/dhi/platform/protobufparser/encoder.py
 src/dhi/platform/protobufparser/enums.py
 src/dhi/platform/protobufparser/message.py
 src/dhi/platform/protobufparser/wire_format.py
 src/dhi/platform/tests/__init__.py
 src/dhi/platform/tests/engine_tests.py
 src/dhi/platform/tests/exceptions_test.py
+src/dhi/platform/tests/job_tests.py
 src/dhi/platform/tests/metadata_dataset_test.py
 src/dhi/platform/tests/metadata_project_test.py
 src/dhi/platform/tests/multidimensional_test.py
+src/dhi/platform/tests/sharing_test.py
 src/dhi/platform/tests/testcredentials.py
 src/dhi/platform/tests/timeseries_test.py
 src/dhi/platform/tests/transfer_test.py
 src/dhi/platform/tests/transfer_tests_integration.py
 src/dhi/platform/tests/upload_download_test.py
 src/dhi/platform/tests/data/EqD2.dfs2
 src/dhi/platform/tests/data/esbjergSmall.txt
```

