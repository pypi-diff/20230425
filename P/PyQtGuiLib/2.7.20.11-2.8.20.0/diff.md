# Comparing `tmp/PyQtGuiLib-2.7.20.11.tar.gz` & `tmp/PyQtGuiLib-2.8.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtGuiLib-2.7.20.11.tar", last modified: Fri Apr 21 06:54:09 2023, max compression
+gzip compressed data, was "PyQtGuiLib-2.8.20.0.tar", last modified: Tue Apr 25 08:32:57 2023, max compression
```

## Comparing `PyQtGuiLib-2.7.20.11.tar` & `PyQtGuiLib-2.8.20.0.tar`

### file list

```diff
@@ -1,260 +1,247 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.915737 PyQtGuiLib-2.7.20.11/
--rw-rw-rw-   0        0        0     1091 2022-12-10 10:29:38.000000 PyQtGuiLib-2.7.20.11/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.636746 PyQtGuiLib-2.7.20.11/Log/
--rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/Log/__init__.py
--rw-rw-rw-   0        0        0     9740 2023-04-21 06:44:31.000000 PyQtGuiLib-2.7.20.11/Log/developmentLog.py
--rw-rw-rw-   0        0        0    17825 2023-04-21 06:54:09.915737 PyQtGuiLib-2.7.20.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.639739 PyQtGuiLib-2.7.20.11/PyQtGuiLib/
--rw-rw-rw-   0        0        0      108 2023-04-15 02:34:22.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.651710 PyQtGuiLib-2.7.20.11/PyQtGuiLib/animation/
--rw-rw-rw-   0        0        0     6805 2023-04-20 03:22:30.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/animation/PropertyAnimation.py
--rw-rw-rw-   0        0        0      208 2023-04-20 09:47:43.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/animation/__init__.py
--rw-rw-rw-   0        0        0     6552 2023-04-20 09:28:51.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/animation/animation.py
--rw-rw-rw-   0        0        0     2465 2023-04-20 09:28:51.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/animation/test_animation.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.665668 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/
--rw-rw-rw-   0        0        0      602 2023-04-21 06:44:31.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/__init__.py
--rw-rw-rw-   0        0        0     5953 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/bubbleWidget.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.671681 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/comboBox/
--rw-rw-rw-   0        0        0      218 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/comboBox/__init__.py
--rw-rw-rw-   0        0        0     4854 2023-02-13 10:30:41.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/comboBox/combBox.py
--rw-rw-rw-   0        0        0     8171 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/comboBox/comboBox.py
--rw-rw-rw-   0        0        0     4107 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/comboBox/comboBox2.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.673651 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/drawers/
--rw-rw-rw-   0        0        0      107 2023-04-20 09:35:26.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/drawers/__init__.py
--rw-rw-rw-   0        0        0     3192 2023-04-21 06:46:15.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/drawers/drawer.py
--rw-rw-rw-   0        0        0     4203 2023-04-17 07:41:59.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/expansionBar.py
--rw-rw-rw-   0        0        0     3886 2023-02-08 01:08:13.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/flowLayout.py
--rw-rw-rw-   0        0        0     2583 2023-04-17 06:05:25.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/imageButton.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.675642 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/lineedit/
--rw-rw-rw-   0        0        0      170 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/lineedit/__init__.py
--rw-rw-rw-   0        0        0     3967 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/lineedit/dynamicTLine.py
--rw-rw-rw-   0        0        0     5090 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/listWidget.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.682647 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/logBrowser/
--rw-rw-rw-   0        0        0      107 2023-03-27 09:33:07.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/logBrowser/__init__.py
--rw-rw-rw-   0        0        0     1823 2023-03-31 09:04:34.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/logBrowser/loadLogTh.py
--rw-rw-rw-   0        0        0     5112 2023-04-03 02:45:06.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/logBrowser/logBrowser.py
--rw-rw-rw-   0        0        0      554 2023-03-31 09:29:33.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/logBrowser/logSizeTh.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.684618 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/notice/
--rw-rw-rw-   0        0        0        0 2023-02-08 01:08:13.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/notice/__init__.py
--rw-rw-rw-   0        0        0     4822 2023-02-10 11:02:17.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/notice/notice.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.688632 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/palettes/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/palettes/__init__.py
--rw-rw-rw-   0        0        0     9818 2023-02-18 01:06:47.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/palettes/colorHsv.py
--rw-rw-rw-   0        0        0     6728 2023-02-18 01:06:47.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/palettes/paletteFrame.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.696596 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/
--rw-rw-rw-   0        0        0      325 2023-04-13 08:34:31.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/__init__.py
--rw-rw-rw-   0        0        0     5602 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/circularBar.py
--rw-rw-rw-   0        0        0     6401 2023-04-13 08:34:31.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/circularProgressBar.py
--rw-rw-rw-   0        0        0     3943 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/gradientBar.py
--rw-rw-rw-   0        0        0     4365 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/loadBar.py
--rw-rw-rw-   0        0        0     6734 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/waterBar.py
--rw-rw-rw-   0        0        0     5092 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/pullOver.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.698611 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/resolver/
--rw-rw-rw-   0        0        0       59 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/resolver/__init__.py
--rw-rw-rw-   0        0        0      674 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/resolver/controls.py
--rw-rw-rw-   0        0        0     7628 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/rollWidget.py
--rw-rw-rw-   0        0        0    10547 2023-04-15 10:18:10.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/slideShow.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.700599 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/slider/
--rw-rw-rw-   0        0        0        0 2023-02-14 00:37:29.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/slider/__init__.py
--rw-rw-rw-   0        0        0     8596 2023-04-13 07:56:58.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/slider/slider.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.702580 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/switchButtons/
--rw-rw-rw-   0        0        0       63 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/switchButtons/__init__.py
--rw-rw-rw-   0        0        0     4993 2023-02-23 01:29:46.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/switchButtons/swButton.py
--rw-rw-rw-   0        0        0     2743 2023-03-06 05:54:08.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/toolBox.py
--rw-rw-rw-   0        0        0     5588 2023-03-14 01:24:55.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/toolList.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.710572 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/
--rw-rw-rw-   0        0        0    11338 2023-04-13 05:09:14.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/WidgetABC.py
--rw-rw-rw-   0        0        0      260 2023-02-09 10:20:35.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/__init__.py
--rw-rw-rw-   0        0        0     3995 2023-02-10 07:29:38.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/borderlessMainWindow.py
--rw-rw-rw-   0        0        0      303 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/borderlessWidget.py
--rw-rw-rw-   0        0        0     4935 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/statusBar.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.714575 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/tets/
--rw-rw-rw-   0        0        0      375 2023-02-27 10:18:30.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/tets/1.py
--rw-rw-rw-   0        0        0     3504 2023-02-27 00:36:50.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/tets/2.py
--rw-rw-rw-   0        0        0        0 2023-02-24 00:57:42.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/tets/__init__.py
--rw-rw-rw-   0        0        0    17840 2023-02-10 03:56:26.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/titleBar.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.720546 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.731493 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/__init__.py
--rw-rw-rw-   0        0        0     5130 2023-04-13 07:48:56.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qt.py
--rw-rw-rw-   0        0        0     2729 2023-04-13 07:53:03.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qtCore.py
--rw-rw-rw-   0        0        0     3019 2023-04-13 07:51:53.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qtGui.py
--rw-rw-rw-   0        0        0      509 2023-02-09 08:33:46.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qtSip.py
--rw-rw-rw-   0        0        0      505 2023-02-13 08:07:57.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qtUic.py
--rw-rw-rw-   0        0        0     6996 2023-02-18 02:58:53.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qtWidgets.py
--rw-rw-rw-   0        0        0      632 2023-02-13 08:14:52.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/__init__.py
--rw-rw-rw-   0        0        0     6404 2023-04-13 07:50:28.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/customStyle.py
--rw-rw-rw-   0        0        0      262 2023-02-10 01:34:45.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/error.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.733512 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/py/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/py/__init__.py
--rw-rw-rw-   0        0        0      103 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/py/common.py
--rw-rw-rw-   0        0        0     3684 2023-04-13 08:06:22.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/utility.py
--rw-rw-rw-   0        0        0      396 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/versions.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.735510 PyQtGuiLib-2.7.20.11/PyQtGuiLib/layoutDeformation/
--rw-rw-rw-   0        0        0      106 2023-03-04 03:38:59.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/layoutDeformation/__init__.py
--rw-rw-rw-   0        0        0     4425 2023-03-07 08:03:39.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/layoutDeformation/test.py
--rw-rw-rw-   0        0        0     2452 2023-04-17 03:52:57.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/listTree.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.738475 PyQtGuiLib-2.7.20.11/PyQtGuiLib/particle/
--rw-rw-rw-   0        0        0      107 2023-04-20 06:55:28.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/particle/__init__.py
--rw-rw-rw-   0        0        0     2729 2023-04-20 09:11:21.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/particle/particle.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.743485 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/
--rw-rw-rw-   0        0        0      362 2023-04-21 06:50:57.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.749445 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/builtStyleDesigner/
--rw-rw-rw-   0        0        0      105 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/builtStyleDesigner/__init__.py
--rw-rw-rw-   0        0        0     7168 2023-02-24 00:57:42.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py
--rw-rw-rw-   0        0        0     5062 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py
--rw-rw-rw-   0        0        0     1237 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.752460 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/buttons/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/buttons/__init__.py
--rw-rw-rw-   0        0        0      620 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/buttons/buttonStyle.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.758441 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/
--rw-rw-rw-   0        0        0      106 2023-02-20 02:36:19.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/__init__.py
--rw-rw-rw-   0        0        0    26952 2023-02-23 01:15:37.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/component.py
--rw-rw-rw-   0        0        0     8822 2023-03-13 01:50:58.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/controlType.py
--rw-rw-rw-   0        0        0    11557 2023-02-23 09:01:24.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/styleLinker.py
--rw-rw-rw-   0        0        0     1444 2023-02-22 03:17:40.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/styleLinkerUi.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.762424 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/
--rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.766423 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/drak/
--rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/drak/__init__.py
--rw-rw-rw-   0        0        0      187 2023-03-29 08:26:42.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/drak/config.py
--rw-rw-rw-   0        0        0    11537 2023-03-30 09:13:08.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/drak/qssDrak.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.771398 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/image/
--rw-rw-rw-   0        0        0      107 2023-03-29 03:26:49.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/image/__init__.py
--rw-rw-rw-   0        0        0    29060 2023-03-30 10:20:11.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/image/image_rc.py
--rw-rw-rw-   0        0        0      300 2023-03-30 10:19:06.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/image/qssFile.py
--rw-rw-rw-   0        0        0    20518 2023-03-30 10:20:35.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/qssFile.py
--rw-rw-rw-   0        0        0     6221 2023-04-20 09:24:50.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/test.py
--rw-rw-rw-   0        0        0    10615 2023-02-09 08:32:36.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/skinABC.py
--rw-rw-rw-   0        0        0     8581 2023-04-13 08:00:22.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/styleAnalysis.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.773381 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/superPainter/
--rw-rw-rw-   0        0        0      107 2023-03-18 07:49:47.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/superPainter/__init__.py
--rw-rw-rw-   0        0        0    13068 2023-04-21 01:53:12.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/superPainter/superPainter.py
--rw-rw-rw-   0        0        0    17854 2023-03-10 06:22:00.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/superPainter.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.775392 PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.777387 PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/UI/
--rw-rw-rw-   0        0        0      193 2023-04-11 03:59:36.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/UI/__init__.py
--rw-rw-rw-   0        0        0     5539 2023-04-13 05:40:13.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.784375 PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/Window/
--rw-rw-rw-   0        0        0      107 2023-04-10 09:41:12.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/Window/__init__.py
--rw-rw-rw-   0        0        0     9497 2023-04-15 10:09:10.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py
--rw-rw-rw-   0        0        0      189 2023-04-11 04:44:35.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.646721 PyQtGuiLib-2.7.20.11/PyQtGuiLib.egg-info/
--rw-rw-rw-   0        0        0    17825 2023-04-21 06:54:09.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7127 2023-04-21 06:54:09.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 06:54:09.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-21 06:54:09.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    17395 2023-03-27 01:38:52.000000 PyQtGuiLib-2.7.20.11/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.794348 PyQtGuiLib-2.7.20.11/abandonCase/
--rw-rw-rw-   0        0        0      108 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.800333 PyQtGuiLib-2.7.20.11/abandonCase/acrylic/
--rw-rw-rw-   0        0        0       37 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/acrylic/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/acrylic/acrylicWidget.py
--rw-rw-rw-   0        0        0     1550 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/acrylic/cstruct.py
--rw-rw-rw-   0        0        0     2183 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/acrylic/windowEffect.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.807314 PyQtGuiLib-2.7.20.11/abandonCase/animation/
--rw-rw-rw-   0        0        0      107 2023-04-20 09:24:50.000000 PyQtGuiLib-2.7.20.11/abandonCase/animation/__init__.py
--rw-rw-rw-   0        0        0    21249 2023-04-20 09:24:50.000000 PyQtGuiLib-2.7.20.11/abandonCase/animation/animation.py
--rw-rw-rw-   0        0        0     2792 2023-03-28 09:06:54.000000 PyQtGuiLib-2.7.20.11/abandonCase/animation/animationDrawType.py
--rw-rw-rw-   0        0        0    11526 2023-04-20 09:24:50.000000 PyQtGuiLib-2.7.20.11/abandonCase/animation/animationFactory.py
--rw-rw-rw-   0        0        0     1636 2023-03-20 04:02:29.000000 PyQtGuiLib-2.7.20.11/abandonCase/animation/animationLayout.py
--rw-rw-rw-   0        0        0     2292 2023-03-15 01:17:54.000000 PyQtGuiLib-2.7.20.11/abandonCase/animation/customAniTest.py
--rw-rw-rw-   0        0        0     9981 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/bubbleWidget.py
--rw-rw-rw-   0        0        0     3620 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/bubbleWidget_case.py
--rw-rw-rw-   0        0        0     1411 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/nodeBar.py
--rw-rw-rw-   0        0        0     9873 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/slideShow.py
--rw-rw-rw-   0        0        0     7801 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/slideShow2.py
--rw-rw-rw-   0        0        0        0 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/spaceWidget.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.818264 PyQtGuiLib-2.7.20.11/abandonCase/widgets/
--rw-rw-rw-   0        0        0      110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/widgets/__init__.py
--rw-rw-rw-   0        0        0     1389 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessFrame.py
--rw-rw-rw-   0        0        0     1962 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessMainWindow.py
--rw-rw-rw-   0        0        0     1441 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessStackedWidget.py
--rw-rw-rw-   0        0        0     1402 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessWidget.py
--rw-rw-rw-   0        0        0    10095 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessWidgetABC.py
--rw-rw-rw-   0        0        0     5034 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/widgets/statusBar.py
--rw-rw-rw-   0        0        0    17577 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/widgets/titleBar.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.821252 PyQtGuiLib-2.7.20.11/auxiliaryMeans/
--rw-rw-rw-   0        0        0        0 2023-04-17 01:54:33.000000 PyQtGuiLib-2.7.20.11/auxiliaryMeans/__init__.py
--rw-rw-rw-   0        0        0     5067 2023-04-17 02:06:33.000000 PyQtGuiLib-2.7.20.11/auxiliaryMeans/toolNewProject.py
--rw-rw-rw-   0        0        0       42 2023-04-21 06:54:09.915737 PyQtGuiLib-2.7.20.11/setup.cfg
--rw-rw-rw-   0        0        0      744 2023-04-21 06:52:57.000000 PyQtGuiLib-2.7.20.11/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.859177 PyQtGuiLib-2.7.20.11/tests/
--rw-rw-rw-   0        0        0      107 2023-03-06 03:09:41.000000 PyQtGuiLib-2.7.20.11/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.877131 PyQtGuiLib-2.7.20.11/tests/test_Animation/
--rw-rw-rw-   0        0        0     1994 2023-04-05 10:25:59.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/1.py
--rw-rw-rw-   0        0        0      606 2023-03-15 09:52:36.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/__init__.py
--rw-rw-rw-   0        0        0     3180 2023-04-20 09:24:50.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/eg1.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.881121 PyQtGuiLib-2.7.20.11/tests/test_Animation/test_ani/
--rw-rw-rw-   0        0        0     1589 2023-04-20 01:28:51.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/test_ani/1.py
--rw-rw-rw-   0        0        0      107 2023-03-27 05:53:58.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/test_ani/__init__.py
--rw-rw-rw-   0        0        0     1654 2023-03-28 08:45:42.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_1.py
--rw-rw-rw-   0        0        0     1824 2023-03-28 08:48:45.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_10.py
--rw-rw-rw-   0        0        0     1305 2023-03-28 08:45:46.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_2.py
--rw-rw-rw-   0        0        0     2011 2023-03-28 08:45:51.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_3.py
--rw-rw-rw-   0        0        0     1276 2023-03-28 08:45:56.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_4.py
--rw-rw-rw-   0        0        0     1851 2023-03-28 08:46:24.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_5.py
--rw-rw-rw-   0        0        0     1759 2023-03-28 08:46:54.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_6.py
--rw-rw-rw-   0        0        0     2206 2023-03-28 08:47:16.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_7.py
--rw-rw-rw-   0        0        0     2000 2023-03-28 08:47:46.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_8.py
--rw-rw-rw-   0        0        0     1712 2023-03-28 08:48:15.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_9.py
--rw-rw-rw-   0        0        0     1541 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_BubbleWidget.py
--rw-rw-rw-   0        0        0     2738 2023-04-13 08:35:22.000000 PyQtGuiLib-2.7.20.11/tests/test_CircularProgressBar.py
--rw-rw-rw-   0        0        0     1596 2023-04-19 07:50:47.000000 PyQtGuiLib-2.7.20.11/tests/test_Notice.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.891065 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/
--rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-04-06 02:24:28.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg1.py
--rw-rw-rw-   0        0        0     2306 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg2.py
--rw-rw-rw-   0        0        0     1891 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg3.py
--rw-rw-rw-   0        0        0     2110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg4.py
--rw-rw-rw-   0        0        0     2519 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg5.py
--rw-rw-rw-   0        0        0     1881 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg6.py
--rw-rw-rw-   0        0        0     2617 2023-03-22 05:45:33.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg7.py
--rw-rw-rw-   0        0        0     2042 2023-04-06 03:41:23.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/test.py
--rw-rw-rw-   0        0        0     2275 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis.py
--rw-rw-rw-   0        0        0     2605 2023-04-13 09:27:46.000000 PyQtGuiLib-2.7.20.11/tests/test_SlideShow.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.896791 PyQtGuiLib-2.7.20.11/tests/test_StyleLinker/
--rw-rw-rw-   0        0        0        0 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_StyleLinker/__init__.py
--rw-rw-rw-   0        0        0      949 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_StyleLinker/eg1_QPushButton.py
--rw-rw-rw-   0        0        0      807 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_StyleLinker/eg2_QLabel.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.906780 PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/
--rw-rw-rw-   0        0        0      871 2023-04-20 09:50:12.000000 PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/1.py
--rw-rw-rw-   0        0        0      106 2023-04-07 09:06:55.000000 PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/__init__.py
--rw-rw-rw-   0        0        0     1568 2023-04-07 09:19:44.000000 PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/eg1.py
--rw-rw-rw-   0        0        0     2143 2023-04-10 00:27:52.000000 PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/eg2.py
--rw-rw-rw-   0        0        0     1648 2023-04-07 09:39:03.000000 PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/eg3.py
--rw-rw-rw-   0        0        0     3527 2023-04-19 03:20:23.000000 PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/eg4.py
--rw-rw-rw-   0        0        0     2538 2023-04-21 02:10:44.000000 PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/test.py
--rw-rw-rw-   0        0        0     2465 2023-04-13 01:50:22.000000 PyQtGuiLib-2.7.20.11/tests/test_barset.py
--rw-rw-rw-   0        0        0     1648 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_circularBar.py
--rw-rw-rw-   0        0        0     1723 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_colorPalette.py
--rw-rw-rw-   0        0        0     1042 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_comboBox.py
--rw-rw-rw-   0        0        0     1161 2023-04-21 06:51:11.000000 PyQtGuiLib-2.7.20.11/tests/test_drawer.py
--rw-rw-rw-   0        0        0      289 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_dumpStructure.py
--rw-rw-rw-   0        0        0      830 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_dynamicTLine.py
--rw-rw-rw-   0        0        0      613 2023-04-17 06:35:12.000000 PyQtGuiLib-2.7.20.11/tests/test_expansionBar.py
--rw-rw-rw-   0        0        0     1315 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_flowLayot.py
--rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_gradientBar.py
--rw-rw-rw-   0        0        0      903 2023-04-17 05:57:17.000000 PyQtGuiLib-2.7.20.11/tests/test_imageButton.py
--rw-rw-rw-   0        0        0     1865 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_listWidget.py
--rw-rw-rw-   0        0        0     1398 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_loadbar.py
--rw-rw-rw-   0        0        0     2498 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_no_border.py
--rw-rw-rw-   0        0        0     1365 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_no_border_pullOver.py
--rw-rw-rw-   0        0        0     1022 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_pullOverWidget.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.908780 PyQtGuiLib-2.7.20.11/tests/test_qssFile/
--rw-rw-rw-   0        0        0      107 2023-03-29 06:12:59.000000 PyQtGuiLib-2.7.20.11/tests/test_qssFile/__init__.py
--rw-rw-rw-   0        0        0      584 2023-04-04 06:18:57.000000 PyQtGuiLib-2.7.20.11/tests/test_qssFile/test.py
--rw-rw-rw-   0        0        0     1444 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_rollWidget.py
--rw-rw-rw-   0        0        0     1666 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_slider.py
--rw-rw-rw-   0        0        0     1778 2023-04-13 01:45:35.000000 PyQtGuiLib-2.7.20.11/tests/test_statusBar.py
--rw-rw-rw-   0        0        0     1014 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_styles.py
--rw-rw-rw-   0        0        0     1122 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_switchButton.py
--rw-rw-rw-   0        0        0      543 2023-04-17 01:43:36.000000 PyQtGuiLib-2.7.20.11/tests/test_template.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.911750 PyQtGuiLib-2.7.20.11/tests/test_templateWindow/
--rw-rw-rw-   0        0        0      107 2023-04-11 04:44:35.000000 PyQtGuiLib-2.7.20.11/tests/test_templateWindow/__init__.py
--rw-rw-rw-   0        0        0     2718 2023-04-13 10:00:15.000000 PyQtGuiLib-2.7.20.11/tests/test_templateWindow/test_listTemplateWindow.py
--rw-rw-rw-   0        0        0     1356 2023-03-13 08:03:45.000000 PyQtGuiLib-2.7.20.11/tests/test_toolList.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.913743 PyQtGuiLib-2.7.20.11/tests/test_uic/
--rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_uic/__init__.py
--rw-rw-rw-   0        0        0      377 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_uic/test_uic.py
--rw-rw-rw-   0        0        0     1547 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_waterBar.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.248136 PyQtGuiLib-2.8.20.0/
+-rw-rw-rw-   0        0        0     1091 2022-12-10 10:29:38.000000 PyQtGuiLib-2.8.20.0/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.005160 PyQtGuiLib-2.8.20.0/Log/
+-rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/Log/__init__.py
+-rw-rw-rw-   0        0        0    10517 2023-04-25 08:27:49.000000 PyQtGuiLib-2.8.20.0/Log/developmentLog.py
+-rw-rw-rw-   0        0        0    17824 2023-04-25 08:32:57.247138 PyQtGuiLib-2.8.20.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.006157 PyQtGuiLib-2.8.20.0/PyQtGuiLib/
+-rw-rw-rw-   0        0        0      108 2023-04-15 02:34:22.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.016132 PyQtGuiLib-2.8.20.0/PyQtGuiLib/animation/
+-rw-rw-rw-   0        0        0     6805 2023-04-20 03:22:30.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/animation/PropertyAnimation.py
+-rw-rw-rw-   0        0        0      232 2023-04-25 06:49:49.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/animation/__init__.py
+-rw-rw-rw-   0        0        0     6552 2023-04-20 09:28:51.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/animation/animation.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.029096 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/
+-rw-rw-rw-   0        0        0      682 2023-04-25 08:12:03.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/__init__.py
+-rw-rw-rw-   0        0        0     5953 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/bubbleWidget.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.031090 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/
+-rw-rw-rw-   0        0        0      218 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/__init__.py
+-rw-rw-rw-   0        0        0     8171 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboBox.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.036077 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboCheckBox/
+-rw-rw-rw-   0        0        0      107 2023-04-25 08:09:32.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboCheckBox/__init__.py
+-rw-rw-rw-   0        0        0    21095 2023-04-25 08:15:03.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboCheckBox/comboCheckBox.py
+-rw-rw-rw-   0        0        0     2327 2023-04-25 08:09:33.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboCheckBox/py_message_box.py
+-rw-rw-rw-   0        0        0    28106 2023-04-25 03:37:41.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboCheckBox/py_style.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.038072 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/drawers/
+-rw-rw-rw-   0        0        0      107 2023-04-20 09:35:26.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/drawers/__init__.py
+-rw-rw-rw-   0        0        0     3190 2023-04-25 06:51:00.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/drawers/drawer.py
+-rw-rw-rw-   0        0        0     4203 2023-04-17 07:41:59.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/expansionBar.py
+-rw-rw-rw-   0        0        0     3886 2023-02-08 01:08:13.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/flowLayout.py
+-rw-rw-rw-   0        0        0     2583 2023-04-17 06:05:25.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/imageButton.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.040067 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/lineedit/
+-rw-rw-rw-   0        0        0      170 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/lineedit/__init__.py
+-rw-rw-rw-   0        0        0     3967 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/lineedit/dynamicTLine.py
+-rw-rw-rw-   0        0        0     5090 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/listWidget.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.046079 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/logBrowser/
+-rw-rw-rw-   0        0        0      107 2023-03-27 09:33:07.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/logBrowser/__init__.py
+-rw-rw-rw-   0        0        0     1823 2023-03-31 09:04:34.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/logBrowser/loadLogTh.py
+-rw-rw-rw-   0        0        0     5112 2023-04-03 02:45:06.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/logBrowser/logBrowser.py
+-rw-rw-rw-   0        0        0      554 2023-03-31 09:29:33.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/logBrowser/logSizeTh.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.048045 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/notice/
+-rw-rw-rw-   0        0        0        0 2023-02-08 01:08:13.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/notice/__init__.py
+-rw-rw-rw-   0        0        0     4822 2023-02-10 11:02:17.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/notice/notice.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.051037 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/palettes/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/palettes/__init__.py
+-rw-rw-rw-   0        0        0     9818 2023-02-18 01:06:47.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/palettes/colorHsv.py
+-rw-rw-rw-   0        0        0     6728 2023-02-18 01:06:47.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/palettes/paletteFrame.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.058035 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/
+-rw-rw-rw-   0        0        0      325 2023-04-13 08:34:31.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/__init__.py
+-rw-rw-rw-   0        0        0     5602 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/circularBar.py
+-rw-rw-rw-   0        0        0     6372 2023-04-25 07:41:31.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/circularProgressBar.py
+-rw-rw-rw-   0        0        0     3943 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/gradientBar.py
+-rw-rw-rw-   0        0        0     4365 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/loadBar.py
+-rw-rw-rw-   0        0        0     6734 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/waterBar.py
+-rw-rw-rw-   0        0        0     5092 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/pullOver.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.061027 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/resolver/
+-rw-rw-rw-   0        0        0       59 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/resolver/__init__.py
+-rw-rw-rw-   0        0        0      674 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/resolver/controls.py
+-rw-rw-rw-   0        0        0     7628 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/rollWidget.py
+-rw-rw-rw-   0        0        0    10547 2023-04-15 10:18:10.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/slideShow.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.063022 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/slider/
+-rw-rw-rw-   0        0        0        0 2023-02-14 00:37:29.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/slider/__init__.py
+-rw-rw-rw-   0        0        0     8596 2023-04-13 07:56:58.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/slider/slider.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.065024 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/switchButtons/
+-rw-rw-rw-   0        0        0       63 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/switchButtons/__init__.py
+-rw-rw-rw-   0        0        0     4993 2023-02-23 01:29:46.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/switchButtons/swButton.py
+-rw-rw-rw-   0        0        0     2743 2023-03-06 05:54:08.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/toolBox.py
+-rw-rw-rw-   0        0        0     5588 2023-03-14 01:24:55.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/toolList.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.071998 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/
+-rw-rw-rw-   0        0        0    11338 2023-04-13 05:09:14.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/WidgetABC.py
+-rw-rw-rw-   0        0        0      260 2023-02-09 10:20:35.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3995 2023-02-10 07:29:38.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/borderlessMainWindow.py
+-rw-rw-rw-   0        0        0      303 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/borderlessWidget.py
+-rw-rw-rw-   0        0        0     4935 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/statusBar.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.075987 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/tets/
+-rw-rw-rw-   0        0        0      375 2023-02-27 10:18:30.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/tets/1.py
+-rw-rw-rw-   0        0        0     3504 2023-02-27 00:36:50.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/tets/2.py
+-rw-rw-rw-   0        0        0        0 2023-02-24 00:57:42.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/tets/__init__.py
+-rw-rw-rw-   0        0        0    17840 2023-02-10 03:56:26.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/titleBar.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.082968 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.089949 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/__init__.py
+-rw-rw-rw-   0        0        0     5834 2023-04-25 06:29:09.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/qt.py
+-rw-rw-rw-   0        0        0      534 2023-04-25 05:53:49.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/qtCore.py
+-rw-rw-rw-   0        0        0      502 2023-04-25 05:53:10.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/qtGui.py
+-rw-rw-rw-   0        0        0      509 2023-02-09 08:33:46.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/qtSip.py
+-rw-rw-rw-   0        0        0      505 2023-02-13 08:07:57.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/qtUic.py
+-rw-rw-rw-   0        0        0      460 2023-04-25 04:13:46.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/qtWidgets.py
+-rw-rw-rw-   0        0        0      763 2023-04-25 05:46:15.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/__init__.py
+-rw-rw-rw-   0        0        0     6406 2023-04-25 05:54:19.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/customStyle.py
+-rw-rw-rw-   0        0        0      262 2023-02-10 01:34:45.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/error.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.091944 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/py/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/py/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/py/common.py
+-rw-rw-rw-   0        0        0     3658 2023-04-25 05:55:44.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/utility.py
+-rw-rw-rw-   0        0        0      396 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/versions.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.094936 PyQtGuiLib-2.8.20.0/PyQtGuiLib/layoutDeformation/
+-rw-rw-rw-   0        0        0      106 2023-03-04 03:38:59.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/layoutDeformation/__init__.py
+-rw-rw-rw-   0        0        0     4425 2023-03-07 08:03:39.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/layoutDeformation/test.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.096931 PyQtGuiLib-2.8.20.0/PyQtGuiLib/particle/
+-rw-rw-rw-   0        0        0      107 2023-04-20 06:55:28.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/particle/__init__.py
+-rw-rw-rw-   0        0        0     2729 2023-04-20 09:11:21.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/particle/particle.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.100921 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/
+-rw-rw-rw-   0        0        0      364 2023-04-25 07:58:50.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.105907 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/builtStyleDesigner/
+-rw-rw-rw-   0        0        0      105 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/builtStyleDesigner/__init__.py
+-rw-rw-rw-   0        0        0     7168 2023-02-24 00:57:42.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py
+-rw-rw-rw-   0        0        0     5062 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py
+-rw-rw-rw-   0        0        0     1237 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.107901 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/buttons/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/buttons/__init__.py
+-rw-rw-rw-   0        0        0      620 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/buttons/buttonStyle.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.111891 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/
+-rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.114883 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/drak/
+-rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/drak/__init__.py
+-rw-rw-rw-   0        0        0      187 2023-03-29 08:26:42.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/drak/config.py
+-rw-rw-rw-   0        0        0    11537 2023-03-30 09:13:08.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/drak/qssDrak.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.118872 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/image/
+-rw-rw-rw-   0        0        0      107 2023-03-29 03:26:49.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/image/__init__.py
+-rw-rw-rw-   0        0        0    29060 2023-03-30 10:20:11.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/image/image_rc.py
+-rw-rw-rw-   0        0        0      300 2023-03-30 10:19:06.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/image/qssFile.py
+-rw-rw-rw-   0        0        0    20518 2023-03-30 10:20:35.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/qssFile.py
+-rw-rw-rw-   0        0        0     6221 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/test.py
+-rw-rw-rw-   0        0        0    10615 2023-02-09 08:32:36.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/skinABC.py
+-rw-rw-rw-   0        0        0     8591 2023-04-24 09:43:40.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/styleAnalysis.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.121864 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/superPainter/
+-rw-rw-rw-   0        0        0      107 2023-03-18 07:49:47.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/superPainter/__init__.py
+-rw-rw-rw-   0        0        0    13068 2023-04-21 01:53:12.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/superPainter/superPainter.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.122862 PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.125854 PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/UI/
+-rw-rw-rw-   0        0        0      193 2023-04-11 03:59:36.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/UI/__init__.py
+-rw-rw-rw-   0        0        0     5539 2023-04-13 05:40:13.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.127848 PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/Window/
+-rw-rw-rw-   0        0        0      107 2023-04-10 09:41:12.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/Window/__init__.py
+-rw-rw-rw-   0        0        0     9497 2023-04-15 10:09:10.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py
+-rw-rw-rw-   0        0        0      189 2023-04-11 04:44:35.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.012170 PyQtGuiLib-2.8.20.0/PyQtGuiLib.egg-info/
+-rw-rw-rw-   0        0        0    17824 2023-04-25 08:32:56.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6721 2023-04-25 08:32:56.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 08:32:56.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-25 08:32:56.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17395 2023-03-27 01:38:52.000000 PyQtGuiLib-2.8.20.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.137833 PyQtGuiLib-2.8.20.0/abandonCase/
+-rw-rw-rw-   0        0        0      108 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.143416 PyQtGuiLib-2.8.20.0/abandonCase/acrylic/
+-rw-rw-rw-   0        0        0       37 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/acrylic/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/acrylic/acrylicWidget.py
+-rw-rw-rw-   0        0        0     1550 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/acrylic/cstruct.py
+-rw-rw-rw-   0        0        0     2183 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/acrylic/windowEffect.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.150397 PyQtGuiLib-2.8.20.0/abandonCase/animation/
+-rw-rw-rw-   0        0        0      107 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.20.0/abandonCase/animation/__init__.py
+-rw-rw-rw-   0        0        0    21249 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.20.0/abandonCase/animation/animation.py
+-rw-rw-rw-   0        0        0     2792 2023-03-28 09:06:54.000000 PyQtGuiLib-2.8.20.0/abandonCase/animation/animationDrawType.py
+-rw-rw-rw-   0        0        0    11526 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.20.0/abandonCase/animation/animationFactory.py
+-rw-rw-rw-   0        0        0     1636 2023-03-20 04:02:29.000000 PyQtGuiLib-2.8.20.0/abandonCase/animation/animationLayout.py
+-rw-rw-rw-   0        0        0     2292 2023-03-15 01:17:54.000000 PyQtGuiLib-2.8.20.0/abandonCase/animation/customAniTest.py
+-rw-rw-rw-   0        0        0     9981 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/bubbleWidget.py
+-rw-rw-rw-   0        0        0     3620 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/bubbleWidget_case.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.156381 PyQtGuiLib-2.8.20.0/abandonCase/linker/
+-rw-rw-rw-   0        0        0      106 2023-02-20 02:36:19.000000 PyQtGuiLib-2.8.20.0/abandonCase/linker/__init__.py
+-rw-rw-rw-   0        0        0    26952 2023-02-23 01:15:37.000000 PyQtGuiLib-2.8.20.0/abandonCase/linker/component.py
+-rw-rw-rw-   0        0        0     8822 2023-03-13 01:50:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/linker/controlType.py
+-rw-rw-rw-   0        0        0    11488 2023-04-25 08:02:33.000000 PyQtGuiLib-2.8.20.0/abandonCase/linker/styleLinker.py
+-rw-rw-rw-   0        0        0     1444 2023-02-22 03:17:40.000000 PyQtGuiLib-2.8.20.0/abandonCase/linker/styleLinkerUi.py
+-rw-rw-rw-   0        0        0     1411 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/nodeBar.py
+-rw-rw-rw-   0        0        0     9873 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/slideShow.py
+-rw-rw-rw-   0        0        0     7801 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/slideShow2.py
+-rw-rw-rw-   0        0        0        0 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/spaceWidget.py
+-rw-rw-rw-   0        0        0    17813 2023-04-25 08:21:59.000000 PyQtGuiLib-2.8.20.0/abandonCase/superPainter.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.170344 PyQtGuiLib-2.8.20.0/abandonCase/widgets/
+-rw-rw-rw-   0        0        0      110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1389 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessFrame.py
+-rw-rw-rw-   0        0        0     1962 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessMainWindow.py
+-rw-rw-rw-   0        0        0     1441 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessStackedWidget.py
+-rw-rw-rw-   0        0        0     1402 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessWidget.py
+-rw-rw-rw-   0        0        0    10095 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessWidgetABC.py
+-rw-rw-rw-   0        0        0     5034 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/widgets/statusBar.py
+-rw-rw-rw-   0        0        0    17577 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/widgets/titleBar.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.173337 PyQtGuiLib-2.8.20.0/auxiliaryMeans/
+-rw-rw-rw-   0        0        0        0 2023-04-17 01:54:33.000000 PyQtGuiLib-2.8.20.0/auxiliaryMeans/__init__.py
+-rw-rw-rw-   0        0        0     5067 2023-04-17 02:06:33.000000 PyQtGuiLib-2.8.20.0/auxiliaryMeans/toolNewProject.py
+-rw-rw-rw-   0        0        0       42 2023-04-25 08:32:57.248136 PyQtGuiLib-2.8.20.0/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-04-25 08:26:52.000000 PyQtGuiLib-2.8.20.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.214227 PyQtGuiLib-2.8.20.0/tests/
+-rw-rw-rw-   0        0        0      107 2023-03-06 03:09:41.000000 PyQtGuiLib-2.8.20.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.217218 PyQtGuiLib-2.8.20.0/tests/test_Animation/
+-rw-rw-rw-   0        0        0     1994 2023-04-05 10:25:59.000000 PyQtGuiLib-2.8.20.0/tests/test_Animation/1.py
+-rw-rw-rw-   0        0        0      606 2023-03-15 09:52:36.000000 PyQtGuiLib-2.8.20.0/tests/test_Animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.220212 PyQtGuiLib-2.8.20.0/tests/test_Animation/test_ani/
+-rw-rw-rw-   0        0        0     1589 2023-04-20 01:28:51.000000 PyQtGuiLib-2.8.20.0/tests/test_Animation/test_ani/1.py
+-rw-rw-rw-   0        0        0      107 2023-03-27 05:53:58.000000 PyQtGuiLib-2.8.20.0/tests/test_Animation/test_ani/__init__.py
+-rw-rw-rw-   0        0        0     2320 2023-04-25 07:55:39.000000 PyQtGuiLib-2.8.20.0/tests/test_Animation/test_animation.py
+-rw-rw-rw-   0        0        0     1541 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_BubbleWidget.py
+-rw-rw-rw-   0        0        0     2738 2023-04-13 08:35:22.000000 PyQtGuiLib-2.8.20.0/tests/test_CircularProgressBar.py
+-rw-rw-rw-   0        0        0     1288 2023-04-25 08:18:48.000000 PyQtGuiLib-2.8.20.0/tests/test_ComboCheckBox.py
+-rw-rw-rw-   0        0        0     1596 2023-04-19 07:50:47.000000 PyQtGuiLib-2.8.20.0/tests/test_Notice.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.230184 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/
+-rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-04-06 02:24:28.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg1.py
+-rw-rw-rw-   0        0        0     2306 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg2.py
+-rw-rw-rw-   0        0        0     1891 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg3.py
+-rw-rw-rw-   0        0        0     2110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg4.py
+-rw-rw-rw-   0        0        0     2519 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg5.py
+-rw-rw-rw-   0        0        0     1881 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg6.py
+-rw-rw-rw-   0        0        0     2617 2023-03-22 05:45:33.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg7.py
+-rw-rw-rw-   0        0        0     2042 2023-04-06 03:41:23.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/test.py
+-rw-rw-rw-   0        0        0     2275 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis.py
+-rw-rw-rw-   0        0        0     2605 2023-04-13 09:27:46.000000 PyQtGuiLib-2.8.20.0/tests/test_SlideShow.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.239161 PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/
+-rw-rw-rw-   0        0        0      871 2023-04-20 09:50:12.000000 PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/1.py
+-rw-rw-rw-   0        0        0      106 2023-04-07 09:06:55.000000 PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/__init__.py
+-rw-rw-rw-   0        0        0     1568 2023-04-07 09:19:44.000000 PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/eg1.py
+-rw-rw-rw-   0        0        0     2143 2023-04-10 00:27:52.000000 PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/eg2.py
+-rw-rw-rw-   0        0        0     1648 2023-04-07 09:39:03.000000 PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/eg3.py
+-rw-rw-rw-   0        0        0     3527 2023-04-19 03:20:23.000000 PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/eg4.py
+-rw-rw-rw-   0        0        0     2538 2023-04-21 02:10:44.000000 PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/test.py
+-rw-rw-rw-   0        0        0     2465 2023-04-13 01:50:22.000000 PyQtGuiLib-2.8.20.0/tests/test_barset.py
+-rw-rw-rw-   0        0        0     1648 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_circularBar.py
+-rw-rw-rw-   0        0        0     1723 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_colorPalette.py
+-rw-rw-rw-   0        0        0     1161 2023-04-21 06:51:11.000000 PyQtGuiLib-2.8.20.0/tests/test_drawer.py
+-rw-rw-rw-   0        0        0      289 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_dumpStructure.py
+-rw-rw-rw-   0        0        0      830 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_dynamicTLine.py
+-rw-rw-rw-   0        0        0      613 2023-04-17 06:35:12.000000 PyQtGuiLib-2.8.20.0/tests/test_expansionBar.py
+-rw-rw-rw-   0        0        0     1315 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_flowLayot.py
+-rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_gradientBar.py
+-rw-rw-rw-   0        0        0      903 2023-04-17 05:57:17.000000 PyQtGuiLib-2.8.20.0/tests/test_imageButton.py
+-rw-rw-rw-   0        0        0     1865 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_listWidget.py
+-rw-rw-rw-   0        0        0     1398 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_loadbar.py
+-rw-rw-rw-   0        0        0     2498 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_no_border.py
+-rw-rw-rw-   0        0        0     1365 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_no_border_pullOver.py
+-rw-rw-rw-   0        0        0     1022 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_pullOverWidget.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.242152 PyQtGuiLib-2.8.20.0/tests/test_qssFile/
+-rw-rw-rw-   0        0        0      107 2023-03-29 06:12:59.000000 PyQtGuiLib-2.8.20.0/tests/test_qssFile/__init__.py
+-rw-rw-rw-   0        0        0      584 2023-04-04 06:18:57.000000 PyQtGuiLib-2.8.20.0/tests/test_qssFile/test.py
+-rw-rw-rw-   0        0        0     1444 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_rollWidget.py
+-rw-rw-rw-   0        0        0     1666 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_slider.py
+-rw-rw-rw-   0        0        0     1778 2023-04-13 01:45:35.000000 PyQtGuiLib-2.8.20.0/tests/test_statusBar.py
+-rw-rw-rw-   0        0        0     1014 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_styles.py
+-rw-rw-rw-   0        0        0     1122 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_switchButton.py
+-rw-rw-rw-   0        0        0      543 2023-04-17 01:43:36.000000 PyQtGuiLib-2.8.20.0/tests/test_template.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.244146 PyQtGuiLib-2.8.20.0/tests/test_templateWindow/
+-rw-rw-rw-   0        0        0      107 2023-04-11 04:44:35.000000 PyQtGuiLib-2.8.20.0/tests/test_templateWindow/__init__.py
+-rw-rw-rw-   0        0        0     2718 2023-04-13 10:00:15.000000 PyQtGuiLib-2.8.20.0/tests/test_templateWindow/test_listTemplateWindow.py
+-rw-rw-rw-   0        0        0     1356 2023-03-13 08:03:45.000000 PyQtGuiLib-2.8.20.0/tests/test_toolList.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.246141 PyQtGuiLib-2.8.20.0/tests/test_uic/
+-rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_uic/__init__.py
+-rw-rw-rw-   0        0        0      377 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_uic/test_uic.py
+-rw-rw-rw-   0        0        0     1547 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_waterBar.py
```

### Comparing `PyQtGuiLib-2.7.20.11/LICENSE.txt` & `PyQtGuiLib-2.8.20.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/Log/developmentLog.py` & `PyQtGuiLib-2.8.20.0/Log/developmentLog.py`

 * *Files 6% similar despite different names*

```diff
@@ -165,14 +165,25 @@
 2023.4.13 
      感谢! PyQt5学习爱好群-(讨厌自己) 贡献 CircularProgressBar 进度条模块
      导入方式 from PyQtGuiLib.core.progressBar import CircularProgressBar
 2023.4.20
     - 新增 抽屉控件(Drawer) -- 编写中
 2023.4.21 
     -抽屉控件(Drawer)完成
+2023.4.25
+    -修复PySide2导入pyqtProperty的BUG
+    -重构了动画框架,并删除老代码以及老的测试用例,新的动画案例还未编写
+    -删除styles包下整个linker项目,以及测试用例
+    -所有由其他人贡献的功能模块里面都会有一个author()方法来记录作者信息
+    -新增控件ComboCheckBox,该控件是一个具体提示的输入框,同时也是一个多项选择框,
+        控件由 "PyQt5学习爱好群-知行合一" 贡献
+        该控件目前PySide系列支持性比较好,PyQt系列存在提示BUG
+        导入方式 from PyQtGuiLib.core import ComboCheckBox
+    -删除老版本的超级画师代码,重构版本的超级画师目前代码提示还不完善
+    -目前所有文档还未更新,
 '''
 
 
 # -------------------------------
 '''
     暂时搁浅的任务
 1.新无边框窗口主窗口,(还没有设计完成,暂时先放下 2023.1.31)
```

### Comparing `PyQtGuiLib-2.7.20.11/PKG-INFO` & `PyQtGuiLib-2.8.20.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtGuiLib
-Version: 2.7.20.11
+Version: 2.8.20.0
 Summary: Python version of the qt component library.
 Home-page: https://github.com/LX-sys/PyQtGuiLib
 Author: LX
 Author-email: lx984608061@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/animation/PropertyAnimation.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/animation/PropertyAnimation.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/animation/animation.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/animation/animation.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/animation/test_animation.py` & `PyQtGuiLib-2.8.20.0/tests/test_Animation/test_animation.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,15 @@
     sys,
     QWidget,
     QPoint,
     QPushButton,
     QSpinBox
 )
 
-# from PyQtGuiLib.animation.new_animation.PropertyAnimation import PropertyAnimation,SequentialAnimationGroup,ParallelAnimationGroup
-from PyQtGuiLib.animation.animation import Animation, ParallelAnimationGroup
-
+from PyQtGuiLib.animation import Animation,ParallelAnimationGroup
 
 
 class Test(QWidget):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
         self.resize(800,600)
 
@@ -55,14 +53,15 @@
         self.ani2.addSeriesAni(sv="5px", ev=12,evs=[20,3,11], targetObj=self.btn, propertyName="font-size", selector="QPushButton")
 
         # self.ani.start()
         self.g = ParallelAnimationGroup()
         self.g.builds([self.ani,self.ani2])
         self.g.start()
 
+
 if __name__ == '__main__':
     app = QApplication(sys.argv)
 
     win = Test()
     win.show()
 
     if PYQT_VERSIONS in ["PyQt6","PySide6"]:
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/__init__.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,8 +4,9 @@
 from PyQtGuiLib.core.flowLayout import FlowLayout
 from PyQtGuiLib.core.listWidget import ListWidget
 from PyQtGuiLib.core.rollWidget import RollWidget
 from PyQtGuiLib.core.palettes.paletteFrame import PaletteFrame
 from PyQtGuiLib.core.notice.notice import Notice,Notices
 from PyQtGuiLib.core.slider.slider import Slider
 from PyQtGuiLib.core.toolList import ToolListWidget,ToolListItem
-from PyQtGuiLib.core.drawers.drawer import DrawerItem,Drawer
+from PyQtGuiLib.core.drawers.drawer import DrawerItem,Drawer
+from PyQtGuiLib.core.comboBox.comboCheckBox.comboCheckBox import ComboCheckBox
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/bubbleWidget.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/bubbleWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/comboBox/combBox.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/notice/notice.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,170 +1,175 @@
-# -*- coding:utf-8 -*-
-# @time:2023/2/1313:52
-# @author:LX
-# @file:combBox.py
-# @software:PyCharm
 from PyQtGuiLib.header import (
-    PYQT_VERSIONS,
-    QApplication,
-    sys,
-    Qt,
-    QGraphicsDropShadowEffect,
     QWidget,
-    QLineEdit,
-    qt,
-    QListWidget,
     Widget,
+    QPainter,
+    QBrush,
+    QColor,
+    QFont,
+    QPaintEvent,
+    qt,
+    Qt,
+    textSize,
+    QThread,
     Signal,
-    QSize,
-    QResizeEvent,
-    QPropertyAnimation
+    QGraphicsDropShadowEffect,
+    QPropertyAnimation,
+    QPoint,
+    QObject
 )
 
+U_Center = "U_Center"
+Left_Down = "Left_Down"
+Rigth_Down = "Rigth_Down"
 
-from PyQt5.QtWidgets import QMessageBox
-
-class LineEdit(QLineEdit):
-    clicked = Signal(bool)
-
+class Time(QThread):
+    finish = Signal()
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
+        self._time = 2500
 
-        self.press = False
+    def setTime(self,d):
+        self._time = d
 
-    def mousePressEvent(self, e) -> None:
-        self.setEnabled(False)
-        if self.press is False:
-            self.clicked.emit(True)
-            self.press = True
-        else:
-            self.clicked.emit(False)
-            self.press = False
-        self.setEnabled(True)
-        # super().mousePressEvent(e)
+    def run(self) -> None:
+        self.msleep(self._time)
+        self.finish.emit()
 
-    def mouseReleaseEvent(self, e) -> None:
-        super().mouseReleaseEvent(e)
 
+'''
+    通知栏
+'''
+class Notice(Widget):
+    finish = Signal(QObject)
 
-class ComBox(Widget):
-    def __init__(self,*args,**kwargs):
-        super().__init__(*args,**kwargs)
-        self.setWindowFlags(qt.FramelessWindowHint)
-        self.setAttribute(qt.WA_TranslucentBackground,True)
-
-        self.shadowX,self.shadowY = 10,10
-        self.spacing = 0
-
-
-        # 输入框高度
-        self.line_height = 40
-
-        # 展开区域高度
-        self.list_widget_height = 300
+    def __init__(self,parent=None):
+        super().__init__(parent)
+        self.resize(220,40)
+        self.__parent = parent
 
+        self.setWindowFlags(qt.FramelessWindowHint|qt.WindowStaysOnTopHint|qt.WindowTransparentForInput)
+        self.setAttribute(qt.WA_TranslucentBackground,True)
 
-        self.Init()
-        self.myEvent()
+        self.__text = "hello wrold"
+        self.__pos = U_Center
 
-        self.resize(500, 300)
+        self.tth = Time()
+        self.tth.finish.connect(self.finish_event)
 
-    def resize(self, *args) -> None:
-        if len(args) == 1 and isinstance(args[0],QSize):
-            super().resize(QSize(args[0].width(),args[1].height()+10))
-            self.line_height = args[1].height()
+        self.shadow = QGraphicsDropShadowEffect(self)
+        self.shadow.setBlurRadius(2)
+        self.shadow.setOffset(2,2)
+        self.shadow.setColor(qt.gray)
+        self.setGraphicsEffect(self.shadow)
+
+    def finish_event(self):
+        self.finish.emit(self)
+        self.deleteLater()
+        self.__parent.update()
+
+    def setText(self,text,interval=8000):
+        self.__text = text
+        self.updatePos()
+        self.tth.setTime(interval)
+        self.tth.start()
+
+    def text(self)->str:
+        return self.__text
+
+    def updatePos(self):
+        w = self.__parent.width()
+        h = self.__parent.height()
+
+        if self.__pos == Left_Down:
+            self.move(self.get_margin(),h-self.height()-self.get_margin()*2)
+        elif self.__pos == Rigth_Down:
+            self.move(w-self.width()-self.get_margin(),h-self.height()-self.get_margin()*2)
         else:
-            super().resize(args[0],args[1]+10)
-            # self.line_height = args[1]
+            self.move(w//2-self.width()//2,self.get_margin())
 
-        self.line.resize(self.width() - self.shadowX, self.line_height)
-        self.line.move(0, 0)
+    def paintEvent(self, event:QPaintEvent) -> None:
+        painter = QPainter(self)
 
-        self.list_widget.move(0, self.line.height() + self.spacing)
-        self.list_widget.resize(self.width() - self.shadowX,0)
-
-    def Init(self):
-        self.line = LineEdit(self)
-        self.list_widget = QListWidget(self)
-        self.defaultStyle()
-        self.shadow()
-        self.updateGeometry()
-
-        self.list_widget.resize(self.width(),0)
-        print("dsa")
-        self.resize(self.width(), self.line.height())
-
-    def hideListWidget(self):
-        def callback():
-            self.resize(self.width(), self.line.height())
-        self.ani(self.list_widget.size(), QSize(self.width() - self.shadowX, 0),callback)
-
-    def showListWidget(self):
-        self.resize(self.width(),self.line.height()+self.list_widget_height+10)
-        self.ani(QSize(self.width()- self.shadowX,0),
-                 QSize(self.width() - self.shadowX,self.list_widget_height - self.line.height() - self.shadowY))
-
-
-    def shadow(self):
-        self.line_shadow = QGraphicsDropShadowEffect(self)
-        self.line_shadow.setBlurRadius(9)
-        self.line_shadow.setOffset(5,5)
-        self.line_shadow.setColor(qt.gray)
-        self.line.setGraphicsEffect(self.line_shadow)
-
-        self.widget_shadow = QGraphicsDropShadowEffect(self)
-        self.widget_shadow.setBlurRadius(9)
-        self.widget_shadow.setOffset(5, 5)
-        self.widget_shadow.setColor(qt.gray)
-        self.list_widget.setGraphicsEffect(self.widget_shadow)
-
-    def defaultStyle(self):
-        self.setStyleSheet('''
-        QLineEdit,QListWidget{
-        border:none;
-        }
-        QLineEdit{
-        }
-        QListWidget{
-        background-color: rgb(221, 221, 110);
-        }
-        ''')
-
-    def updateGeometry(self):
-        self.line.resize(self.width()- self.shadowX, self.line_height)
-        self.line.move(0, 0)
-
-        self.list_widget.move(0, self.line.height() + self.spacing)
-        self.list_widget.resize(self.width() - self.shadowX, self.list_widget_height - self.line.height() - self.shadowY)
-
-        self.resize(self.width(),
-                    self.line.height()+self.spacing+self.list_widget_height)
-
-    def myEvent(self):
-        self.line.clicked.connect(self.listExpansion_Event)
-
-    def listExpansion_Event(self,b):
-        if b:
-            self.showListWidget()
+        painter.setPen(qt.NoPen)
+        bru = QBrush(self.get_backgroundColor())
+        painter.setBrush(bru)
+
+        painter.drawRoundedRect(self.rect(),self.get_radius(),self.get_radius())
+
+        painter.setPen(self.get_color())
+        font = QFont(self.text())
+        font.setPointSize(self.get_fontSize())
+
+        painter.setFont(font)
+
+        fs = textSize(font,self.text())
+        x = self.width()//2 - fs.width()//2
+        y = self.height()//2 + fs.height()//2
+        painter.drawText(x,y,self.text())
+
+        painter.end()
+
+    def closeEvent(self, event) -> None:
+        super().closeEvent(event)
+
+
+class Notices(QObject):
+    def __init__(self,parent:QWidget):
+        super().__init__(parent)
+        self.winp = parent
+
+        # 通知组
+        self.notices = []
+        # 记录高度
+        self.notice_heights = []
+
+        self.spacing = 9
+
+        self.style = ""
+
+    def setSpacing(self,n):
+        self.spacing = n
+
+    def count(self)->int:
+        return len(self.notices)
+
+    def finish_event(self,obj:QObject):
+        self.notices.remove(obj)
+        # 未写完
+        if self.notices:
+            for tip in self.notices:
+                self.aniPos(tip,
+                            tip.pos(),
+                            QPoint(tip.x(), tip.y()-tip.height()-self.spacing))
+                # tip.move(tip.x(), tip.y()-tip.height()-self.spacing)
+
+    # 动画
+    def aniPos(self,obj,spos:QPoint,epos:QPoint):
+        self.ani = QPropertyAnimation(self)
+        self.ani.setTargetObject(obj)
+        self.ani.setPropertyName(b"pos")
+        self.ani.setStartValue(spos)
+        self.ani.setEndValue(epos)
+        self.ani.setDuration(100)
+        self.ani.start()
+
+    def appendTip(self,text:str,interval=3):
+        tip = Notice(self.winp)
+        tip.finish.connect(self.finish_event)
+        tip.setText(text,interval*1000)
+        if self.style:
+            tip.setStyleSheet(self.style)
+        self.notices.append(tip)
+        self.notice_heights.append(QPoint(tip.x(),self.count()*tip.height()+self.spacing))
+        print(self.notice_heights)
+        if self.count()>1:
+            # t_tip = self.notices[-1]
+            self.aniPos(tip,QPoint(tip.x(),0),
+                        self.notice_heights[self.count()-2])
+            # tip.move(tip.x(), t_tip.y()+t_tip.height()+self.spacing)
         else:
-            self.hideListWidget()
+            tip.move(tip.x(), 0)
+
+        tip.show()
 
-    def ani(self,s:QSize,e:QSize,callback=None):
-        ani = QPropertyAnimation(self.list_widget, b"size", self)
-        ani.setStartValue(s)
-        ani.setEndValue(e)
-        ani.setDuration(200)
-        if callback:
-            ani.finished.connect(callback)
-        ani.start()
-
-
-if __name__ == '__main__':
-    app = QApplication(sys.argv)
-
-    win = ComBox()
-    win.show()
-
-    if PYQT_VERSIONS in ["PyQt6","PySide6"]:
-        sys.exit(app.exec())
-    else:
-        sys.exit(app.exec_())
+    def setStyleSheet(self,style:str):
+        self.style = style
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/comboBox/comboBox.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/comboBox/comboBox2.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/layoutDeformation/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,159 +1,165 @@
 # -*- coding:utf-8 -*-
-# @time:2022/12/2912:42
+# @time:2023/3/411:37
 # @author:LX
-# @file:comboBox2.py
+# @file:eg1.py
 # @software:PyCharm
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
-    sys,
     QApplication,
+    sys,
     QWidget,
-    QThread,
-    Signal,
-    QLineEdit,
-    QInputMethodEvent,
-    QKeyEvent,
+    qt,
+    QPushButton,
+    Qt,
+    QPalette,
+    QColor,
     QPaintEvent,
-    QMouseEvent,
     QPainter,
-    QPen,
-    QFont,
-    QResizeEvent,
-    QRect,
     QBrush,
-    QColor,
-    QScrollArea,
-    QVBoxLayout,
-    QPushButton,
+    QSize,
+    QMainWindow,
+    QLineEdit,
+    desktopCenter,
+    QPixmap,
+    QLinearGradient,
     QLabel,
+    QFont,
+    textSize,
+    QFontMetricsF,
     Qt,
+    QMouseEvent,
     QPropertyAnimation,
-    QPoint,
-    QSize,
-    QMoveEvent,
-    QComboBox,
-    qt
+    QRect,
+    QParallelAnimationGroup,
+    QResizeEvent
 )
+from PyQtGuiLib.core.flowLayout import FlowLayout
+import time
+from PyQt5.QtWidgets import QSplashScreen,QDialog,QProxyStyle,QButtonGroup
+from PyQt5.QtCore import QThread,QRunnable,QThreadPool
+from PyQt5.QtGui import QFontMetrics,QFocusEvent
+
+# QSplashScreen
+'''
+    测试用例的标准模板,该代码用于复制
+'''
+from PyQtGuiLib.core.resolver import dumpStructure
+from PyQtGuiLib.styles import ButtonStyle
 
-class ScrollArea(QScrollArea):
-    # 风格
-    Style_Card = "card"  # 卡片
-
-    def __init__(self,*args,**kwargs):
-        super().__init__(*args,**kwargs)
-
-        self.resize(500,500)
-
-        self.setAttribute(qt.WA_TranslucentBackground, True)
-        self.setWindowFlags(qt.FramelessWindowHint)
-        self.setAttribute(qt.WA_DeleteOnClose)
-
-        # 风格模式
-        self.style_mode = ScrollArea.Style_Card
-
-        self.__vlay = QVBoxLayout(self)
-        self.__vlay.setContentsMargins(0,0,0,0)
-        self.__vlay.setSpacing(3)
-
-        self.item_fixed_size = (self.width(),30)
-
-    # 卡片风格颜色
-    def styleCrad(self)->str:
-        style ='''
-background-color: rgb(176, 255, 225);
-border:1px solid gray;
-border-radius:5px;
-        '''
-        return style
-
-    def addWidget(self,widget:QWidget):
-        if isinstance(widget,str):
-            widget = QLabel(widget)
-            print(widget)
-            widget.setFixedHeight(30)
-            widget.setAlignment(qt.AlignCenter)
-            if self.style_mode == ScrollArea.Style_Card:
-                widget.setStyleSheet(self.styleCrad())
-        self.__vlay.addWidget(widget)
-        self.adjustSize()
-
-
-class LineEdit(QLineEdit):
-    clicked = Signal() # 点击事件
 
+class Test(QWidget):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
+        self.resize(600,600)
 
-        self.resize(300,40)
-        # 图标大小
-        self.icon_w, self.icon_h = 12, 12
-        # 图标位置靠右的位置,距离边的距离
-        self.icon_right_margin = 25
-        # 圆角
-        self.icon_radius = (6,6)
-        self.icon_color = QColor(0, 255, 0)
-
-        # 动画开关
-        self.animation_switch = False
-
-        #
-        self.scroll_area = ScrollArea()
-        # self.startTimer(100)
-
-    def mousePressEvent(self, e:QMouseEvent) -> None:
-        self.clicked.emit()
-        self.animation_switch = True
-        self.scroll_area.show()
-        self.scroll_area.move(self.pos().x(),self.pos().y()+70)
-        self.scroll_area.resize(self.width(),200)
-        super().mousePressEvent(e)
-
-    def mouseReleaseEvent(self, e: QMouseEvent) -> None:
-        super().mouseReleaseEvent(e)
-
-    def moveEvent(self, e: QMoveEvent) -> None:
-        self.scroll_area.move(e.pos().x(),e.pos().y()+self.height())
-        super().moveEvent(e)
-
-    # 绘制图标
-    def drawIcon(self,painter:QPainter):
-        parent = self # 父类对象
-        h = self.height()//2-self.icon_h//2
-        rect = QRect(parent.width() - self.icon_right_margin, h, self.icon_w,self.icon_h)
-
-        op = QPen()
-        op.setColor(self.icon_color)
-        bush = QBrush(self.icon_color)
-
-        painter.setPen(op)
-        painter.setBrush(bush)
-
-        painter.drawRoundedRect(rect,*self.icon_radius)
-
-    # def timerEvent(self, e) -> None:
-    #     self.update()
-
-    def paintEvent(self, e: QPaintEvent) -> None:
-        super().paintEvent(e)
-        painter = QPainter(self)
-        painter.setRenderHints(qt.Antialiasing | qt.SmoothPixmapTransform | qt.TextAntialiasing)
-
-        # 绘制图标
-        self.drawIcon(painter)
-
-        painter.end()
-
-
-    def closeEvent(self, e) -> None:
-        self.scroll_area.close()
-        super().closeEvent(e)
+        self.a = QWidget(self)
+        self.b = QWidget(self)
+        self.a.setObjectName("a")
+        self.b.setObjectName("b")
+
+        self.a.resize(self.width(),150)
+        self.b.resize(self.width(),self.height()-150)
+        self.b.move(0,150)
+
+        self.setStyleSheet('''
+#a{
+border:1px solid red;
+}
+#b{
+border:1px solid blue;
+}
+        ''')
+
+        # ---
+        self.af = FlowLayout(self.a)
+        self.bf = FlowLayout(self.b)
+
+        for ai in range(8):
+            btn = QPushButton("test_{}".format(ai))
+            btn.setFixedSize(100,50)
+            btn.setStyleSheet(ButtonStyle.randomStyle())  # 使用 皮肤包
+            self.af.addWidget(btn)
+
+        for bi in range(10):
+            btn = QPushButton("test_{}".format(bi))
+            btn.setFixedSize(130, 60)
+            btn.setStyleSheet(ButtonStyle.randomStyle())  # 使用 皮肤包
+            self.bf.addWidget(btn)
+
+
+        self.isf = False
+        self.btn = QPushButton("开始 影像形变-布局",self)
+        self.btn.resize(150,60)
+        self.btn.move(300,300)
+        self.btn.clicked.connect(self.test_start)
+        # self.anim()
+
+    def test_start(self):
+        if self.isf is False:
+            self.anim()
+            self.btn.setText("恢复 影像形变-布局")
+            self.isf = True
+        else:
+            self.anim_re()
+            self.btn.setText("开始 影像形变-布局")
+            self.isf = False
+
+
+    def anim(self):
+        pain = QParallelAnimationGroup(self)
+        # pain.setDirection(3000)
+
+        ani = QPropertyAnimation(self.a,b"geometry",self)
+        ani.setDuration(1000)
+        ani.setStartValue(self.a.rect())
+        ani.setEndValue(QRect(self.a.x(),self.a.y(),
+                              self.a.height(),self.a.width()))
+
+
+        anib = QPropertyAnimation(self.b,b"geometry",self)
+        anib.setDuration(1000)
+        anib.setStartValue(self.b.rect())
+        anib.setEndValue(QRect(150,0,
+                              self.b.width()-150,self.height()))
+
+        pain.addAnimation(ani)
+        pain.addAnimation(anib)
+        pain.start()
+
+
+    def anim_re(self):
+        pain = QParallelAnimationGroup(self)
+        # pain.setDirection(3000)
+
+        ani = QPropertyAnimation(self.a, b"geometry", self)
+        ani.setDuration(1000)
+        ani.setStartValue(self.a.rect())
+        ani.setEndValue(QRect(self.a.x(), self.a.y(),
+                              self.a.height(), self.a.width()))
+
+        anib = QPropertyAnimation(self.b, b"geometry", self)
+        anib.setDuration(1000)
+        anib.setStartValue(self.b.rect())
+        anib.setEndValue(QRect(0, 150,
+                               self.width(), self.height()- 150))
+
+        pain.addAnimation(ani)
+        pain.addAnimation(anib)
+        pain.start()
+
+
+    def resizeEvent(self, e: QResizeEvent) -> None:
+        self.a.resize(self.width(), 150)
+        self.b.resize(self.width(), self.height() - 150)
+        super().resizeEvent(e)
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
-    win = LineEdit()
+
+    win = Test()
     win.show()
 
-    if PYQT_VERSIONS == "PyQt6":
+    if PYQT_VERSIONS in ["PyQt6","PySide6"]:
         sys.exit(app.exec())
     else:
         sys.exit(app.exec_())
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/drawers/drawer.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/drawers/drawer.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     QSizePolicy,
     QScrollArea,
     qt
 )
 
 from PyQtGuiLib.animation import Animation
 
-
 class DrawerItem(QWidget):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.resize(300, 300)
 
         self.__vboy = QVBoxLayout(self)
         self.__vboy.setSpacing(0)
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/expansionBar.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/expansionBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/flowLayout.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/flowLayout.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/imageButton.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/imageButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/lineedit/dynamicTLine.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/lineedit/dynamicTLine.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/listWidget.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/listWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/logBrowser/loadLogTh.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/logBrowser/loadLogTh.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/logBrowser/logBrowser.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/logBrowser/logBrowser.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/logBrowser/logSizeTh.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/logBrowser/logSizeTh.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/notice/notice.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/statusBar.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,175 +1,187 @@
 from PyQtGuiLib.header import (
+    is_win_sys,
+    is_mac_sys,
+    time,
+    QThread,
+    Signal,
     QWidget,
-    Widget,
+    QFrame,
+    QHBoxLayout,
+    QLabel,
+    QPushButton,
+    QSpacerItem,
+    QSizePolicy,
     QPainter,
-    QBrush,
-    QColor,
-    QFont,
     QPaintEvent,
-    qt,
-    Qt,
-    textSize,
-    QThread,
-    Signal,
-    QGraphicsDropShadowEffect,
-    QPropertyAnimation,
-    QPoint,
-    QObject
+    QStyleOption,
+    QStyle,
+    qt
 )
+from PyQtGuiLib.core.widgets import WidgetABC
 
-U_Center = "U_Center"
-Left_Down = "Left_Down"
-Rigth_Down = "Rigth_Down"
+# 倒计时类
+class CountDownThread(QThread):
+    # 计时完成信号
+    timeOuted = Signal()
 
-class Time(QThread):
-    finish = Signal()
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
-        self._time = 2500
+        self.time_ = 0
 
-    def setTime(self,d):
-        self._time = d
+    # 设置时间
+    def setTime(self,time:int):
+        self.time_ = time
 
     def run(self) -> None:
-        self.msleep(self._time)
-        self.finish.emit()
+        while self.time_:
+            self.sleep(1)
+            self.time_-=1
+        self.timeOuted.emit()
 
 
-'''
-    通知栏
-'''
-class Notice(Widget):
-    finish = Signal(QObject)
-
-    def __init__(self,parent=None):
-        super().__init__(parent)
-        self.resize(220,40)
-        self.__parent = parent
+class StatusBar(WidgetABC):
+
+    PosBottom = "PosBottom"
+    PosTop = "PosTop"
 
-        self.setWindowFlags(qt.FramelessWindowHint|qt.WindowStaysOnTopHint|qt.WindowTransparentForInput)
-        self.setAttribute(qt.WA_TranslucentBackground,True)
+    def __init__(self,*args,**kwargs):
+        super().__init__(*args,**kwargs)
 
-        self.__text = "hello wrold"
-        self.__pos = U_Center
+        self.setAttribute(qt.WA_StyledBackground,True)
 
-        self.tth = Time()
-        self.tth.finish.connect(self.finish_event)
+        self.h = 30
 
-        self.shadow = QGraphicsDropShadowEffect(self)
-        self.shadow.setBlurRadius(2)
-        self.shadow.setOffset(2,2)
-        self.shadow.setColor(qt.gray)
-        self.setGraphicsEffect(self.shadow)
-
-    def finish_event(self):
-        self.finish.emit(self)
-        self.deleteLater()
-        self.__parent.update()
-
-    def setText(self,text,interval=8000):
-        self.__text = text
-        self.updatePos()
-        self.tth.setTime(interval)
-        self.tth.start()
-
-    def text(self)->str:
-        return self.__text
-
-    def updatePos(self):
-        w = self.__parent.width()
-        h = self.__parent.height()
-
-        if self.__pos == Left_Down:
-            self.move(self.get_margin(),h-self.height()-self.get_margin()*2)
-        elif self.__pos == Rigth_Down:
-            self.move(w-self.width()-self.get_margin(),h-self.height()-self.get_margin()*2)
-        else:
-            self.move(w//2-self.width()//2,self.get_margin())
+        # 默认半径
+        # self.setRadius((0, self.radius()[0]))
+        # print(self.radius())
+        # self.setRadius((3, 5))
+        # self.setBorderWidth(0)
 
-    def paintEvent(self, event:QPaintEvent) -> None:
-        painter = QPainter(self)
+        self.__parent = None #  type:QWidget
 
-        painter.setPen(qt.NoPen)
-        bru = QBrush(self.get_backgroundColor())
-        painter.setBrush(bru)
-
-        painter.drawRoundedRect(self.rect(),self.get_radius(),self.get_radius())
-
-        painter.setPen(self.get_color())
-        font = QFont(self.text())
-        font.setPointSize(self.get_fontSize())
-
-        painter.setFont(font)
-
-        fs = textSize(font,self.text())
-        x = self.width()//2 - fs.width()//2
-        y = self.height()//2 + fs.height()//2
-        painter.drawText(x,y,self.text())
-
-        painter.end()
-
-    def closeEvent(self, event) -> None:
-        super().closeEvent(event)
-
-
-class Notices(QObject):
-    def __init__(self,parent:QWidget):
-        super().__init__(parent)
-        self.winp = parent
-
-        # 通知组
-        self.notices = []
-        # 记录高度
-        self.notice_heights = []
-
-        self.spacing = 9
-
-        self.style = ""
-
-    def setSpacing(self,n):
-        self.spacing = n
-
-    def count(self)->int:
-        return len(self.notices)
-
-    def finish_event(self,obj:QObject):
-        self.notices.remove(obj)
-        # 未写完
-        if self.notices:
-            for tip in self.notices:
-                self.aniPos(tip,
-                            tip.pos(),
-                            QPoint(tip.x(), tip.y()-tip.height()-self.spacing))
-                # tip.move(tip.x(), tip.y()-tip.height()-self.spacing)
-
-    # 动画
-    def aniPos(self,obj,spos:QPoint,epos:QPoint):
-        self.ani = QPropertyAnimation(self)
-        self.ani.setTargetObject(obj)
-        self.ani.setPropertyName(b"pos")
-        self.ani.setStartValue(spos)
-        self.ani.setEndValue(epos)
-        self.ani.setDuration(100)
-        self.ani.start()
-
-    def appendTip(self,text:str,interval=3):
-        tip = Notice(self.winp)
-        tip.finish.connect(self.finish_event)
-        tip.setText(text,interval*1000)
-        if self.style:
-            tip.setStyleSheet(self.style)
-        self.notices.append(tip)
-        self.notice_heights.append(QPoint(tip.x(),self.count()*tip.height()+self.spacing))
-        print(self.notice_heights)
-        if self.count()>1:
-            # t_tip = self.notices[-1]
-            self.aniPos(tip,QPoint(tip.x(),0),
-                        self.notice_heights[self.count()-2])
-            # tip.move(tip.x(), t_tip.y()+t_tip.height()+self.spacing)
-        else:
-            tip.move(tip.x(), 0)
+        # 状态栏位置
+        self.status_pos = StatusBar.PosBottom
+
+        if args:
+            self.setParent(args[0])
+
+        # 本地时间
+        self.format = "%Y-%m-%d %H:%M:%S"
+        self.local_time = time.strftime(self.format, time.localtime())
+        self.l_time = QLabel(self.local_time)
 
-        tip.show()
+        # 创建倒计时类
+        self.cd = CountDownThread()
 
-    def setStyleSheet(self,style:str):
-        self.style = style
+        self.__hlay = QHBoxLayout(self)
+        self.__hlay.setContentsMargins(6,0,6,0)
+        if is_win_sys:
+            self.__hlay.setSpacing(6)
+        if is_mac_sys:
+            self.__hlay.setSpacing(6*3)
+
+        self.hSpacer = QSpacerItem(704, 20, qt.PolicyExpanding, qt.PolicyMinimum)
+
+        self.defaultStyle()
+
+        # self.startTimer(1000)
+
+    def defaultStyle(self):
+        self.setStyleSheet("background-color: rgb(193, 193, 193);")
+
+    # 设置时间格式
+    def setTimeFormat(self,format:str="%Y-%m-%d %H:%M:%S"):
+        self.format = format
+
+    def setParent(self, parent:QWidget) -> None:
+        self.__parent = parent
+        super().setParent(parent)
+
+        if self.__parent is not None:
+            self.updateStatusSize()
+
+    def parent(self):
+        return self.__parent
+
+    # 设置状态栏位置
+    def setStatusPos(self,mode:str):
+        self.status_pos = mode
+
+    def __addSpacer(self):
+        self.__hlay.addItem(self.hSpacer)
+        self.__hlay.removeItem(self.hSpacer)
+        self.__hlay.addItem(self.hSpacer)
+
+    # 添加文本
+    def addText(self,text:str,style:str=None,duration:int=0):
+        '''
+            text:文本
+            style:样式
+            duration:持续时间后消失
+        '''
+        l = QLabel(text)
+        if style:
+            l.setStyleSheet(style)
+
+        self.__hlay.addWidget(l)
+        self.__addSpacer()
+
+        # 移除布局
+        def _del():
+            self.__hlay.removeWidget(l)
+            l.deleteLater()  # 销毁自己
+
+        if duration > 0:
+            self.cd.setTime(duration)
+            self.cd.timeOuted.connect(lambda :_del())
+            self.cd.start()
+
+    # 添加按钮
+    def addButton(self,text:str,style:str=None,callback=None):
+        btn = QPushButton(text)
+        if style:
+            btn.setStyleSheet(style)
+        if callback:
+            btn.clicked.connect(callback)
+        self.__hlay.addWidget(btn)
+        self.__addSpacer()
+
+    # 添加widget
+    def addWidget(self,widget:QWidget,style:str=None):
+        if style:
+            widget.setStyleSheet(style)
+        self.__hlay.addWidget(widget)
+        self.__addSpacer()
+
+    # 添加时间
+    def addTime(self,style:str="background-color:transparent"):
+        if style:
+            self.l_time.setStyleSheet(style)
+        self.__hlay.addWidget(self.l_time)
+        self.__addSpacer()
+
+    def updateStatusSize(self):
+        if self.status_pos == StatusBar.PosTop:
+            self.resize(self.__parent.width(), self.h)
+            self.move(0, 0)
+        else:
+            print(0, self.__parent.height() - self.h)
+            self.resize(self.__parent.width(), self.h)
+            self.move(0, self.__parent.height() - self.h)
+
+    def timerEvent(self,e) -> None:
+        try:
+            self.local_time = time.strftime(self.format, time.localtime())
+            self.l_time.setText(self.local_time)
+        except KeyboardInterrupt:
+            pass
+
+
+    def paintEvent(self, e: QPaintEvent) -> None:
+        super().paintEvent(e)
+        self.updateStatusSize()
+        # painter = QPainter(self)
+        #
+        # self.updateStatusSize()
+        #
+        # painter.end()
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/palettes/colorHsv.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/palettes/colorHsv.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/palettes/paletteFrame.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/palettes/paletteFrame.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/circularBar.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/circularBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/circularProgressBar.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/circularProgressBar.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
         self._step = 0
         self._numSteps = 100
         self._interval = 30
 
         self._timer.timeout.connect(self._animate)
         self._timer.setInterval(self._interval)
 
-    # 关于作者的信息
     def author(self) -> str:
         return self.__personalInformation
 
     def setChunkWidth(self, w: int):
         """设置圆环的宽度"""
         self._penWidth = w
         self.update()
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/gradientBar.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/gradientBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/loadBar.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/loadBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/waterBar.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/waterBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/pullOver.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/pullOver.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/resolver/controls.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/resolver/controls.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/rollWidget.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/rollWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/slideShow.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/slideShow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/slider/slider.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/slider/slider.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/switchButtons/swButton.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/switchButtons/swButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/toolBox.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/toolBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/toolList.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/toolList.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/WidgetABC.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/WidgetABC.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/borderlessMainWindow.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/borderlessMainWindow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/statusBar.py` & `PyQtGuiLib-2.8.20.0/abandonCase/widgets/statusBar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,32 @@
+# -*- coding:utf-8 -*-
+# @time:2023/1/411:16
+# @author:LX
+# @file:statusBar.py
+# @software:PyCharm
+from PyQt5.QtCore import QObject
+
 from PyQtGuiLib.header import (
     is_win_sys,
     is_mac_sys,
     time,
     QThread,
     Signal,
     QWidget,
-    QFrame,
     QHBoxLayout,
     QLabel,
     QPushButton,
     QSpacerItem,
-    QSizePolicy,
-    QPainter,
     QPaintEvent,
-    QStyleOption,
-    QStyle,
     qt
 )
-from PyQtGuiLib.core.widgets import WidgetABC
+'''
+    状态栏
+'''
+
 
 # 倒计时类
 class CountDownThread(QThread):
     # 计时完成信号
     timeOuted = Signal()
 
     def __init__(self,*args,**kwargs):
@@ -34,15 +39,15 @@
 
     def run(self) -> None:
         while self.time_:
             self.sleep(1)
             self.time_-=1
         self.timeOuted.emit()
 
-
+from PyQtGuiLib.core.widgets2 import WidgetABC
 class StatusBar(WidgetABC):
 
     PosBottom = "PosBottom"
     PosTop = "PosTop"
 
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
@@ -96,15 +101,15 @@
     def setParent(self, parent:QWidget) -> None:
         self.__parent = parent
         super().setParent(parent)
 
         if self.__parent is not None:
             self.updateStatusSize()
 
-    def parent(self):
+    def parent(self) -> QObject:
         return self.__parent
 
     # 设置状态栏位置
     def setStatusPos(self,mode:str):
         self.status_pos = mode
 
     def __addSpacer(self):
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/tets/2.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/tets/2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/titleBar.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/titleBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qt.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/qt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 # @time:2023/1/68:49
 # @author:LX
 # @file:qt.py
 # @software:PyCharm
 from PyQtGuiLib.header.versions import PYQT_VERSIONS
-from PyQtGuiLib.header import Qt,QPainter,QStyle,QSizePolicy,QEasingCurve
+from PyQtGuiLib.header import Qt,QPainter,QStyle,QSizePolicy,QEasingCurve,QCompleter
 
 
 if PYQT_VERSIONS == "PyQt5"  :
     FramelessWindowHint = Qt.FramelessWindowHint
     WindowTransparentForInput = Qt.WindowTransparentForInput
     Window = Qt.Window
     WindingFill = Qt.WindingFill
@@ -59,15 +59,24 @@
     TabFocus = Qt.TabFocus
     ClickFocus = Qt.ClickFocus
     StrongFocus = Qt.StrongFocus
     OutBounce = QEasingCurve.OutBounce
     CosineCurve = QEasingCurve.CosineCurve
     SineCurve = QEasingCurve.SineCurve
     InCurve = QEasingCurve.InCurve
-
+    Checked = Qt.Checked
+    Unchecked = Qt.Unchecked
+    PartiallyChecked = Qt.PartiallyChecked
+    AscendingOrder=Qt.AscendingOrder
+    DescendingOrder = Qt.DescendingOrder
+    MatchContains = Qt.MatchContains
+    PopupCompletion = QCompleter.PopupCompletion
+    Key_Enter = Qt.Key_Enter
+    Key_Backspace = Qt.Key_Backspace
+    Key_Return = Qt.Key_Return
 
 
 if PYQT_VERSIONS in ["PyQt6","PySide2","PySide6"]:
     WindowTransparentForInput = Qt.WindowType.WindowTransparentForInput
     FramelessWindowHint = Qt.WindowType.FramelessWindowHint
     Window = Qt.WindowType.Window
     WindingFill = Qt.FillRule.WindingFill
@@ -120,7 +129,14 @@
     OutBounce = QEasingCurve.Type.OutBounce
     CosineCurve = QEasingCurve.Type.CosineCurve
     SineCurve = QEasingCurve.Type.SineCurve
     InCurve = QEasingCurve.Type.InCurve
     Unchecked = Qt.CheckState.Unchecked
     Checked = Qt.CheckState.Checked
     PartiallyChecked = Qt.CheckState.PartiallyChecked
+    AscendingOrder = Qt.SortOrder.AscendingOrder
+    DescendingOrder = Qt.SortOrder.DescendingOrder
+    MatchContains = Qt.MatchFlag.MatchContains
+    PopupCompletion = QCompleter.CompletionMode.PopupCompletion
+    Key_Enter = Qt.Key.Key_Enter
+    Key_Backspace = Qt.Key.Key_Backspace
+    Key_Return = Qt.Key.Key_Return
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/customStyle.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/customStyle.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     QColor,
     qt,
     Qt,
     QPoint,
     QRect,
     pyqtProperty,
 )
+
 import re
 import json
 '''
     公共自定义样式
 '''
 
 def strRGBA_to_RGBA(rgba_str:str)->list:
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/utility.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-import platform,math
+import platform
+import math
+
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
     DesktopWidget,
     QPoint,
     QSize,
     QFontMetricsF,
     QFont,
     QWidget,
+    CustomStyle
 )
-from PyQtGuiLib.header.customStyle import CustomStyle
+
 '''
 QListWidget 在Pyqt5页面刷新的方式 update(),其他版本可以用repaint()来达到一样的效果
 QListWidget 的update(item)需要传递一个参数
 '''
 
 is_win_sys = True if platform.system() == "win32" else False
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/listTree.py` & `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,108 +1,89 @@
 # -*- coding:utf-8 -*-
-# @time:2023/4/158:55
+# @time:2023/2/918:26
 # @author:LX
-# @file:listTree.py
-# @software:PyCharm
+# @file:eg2.py
+
+
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
     QApplication,
     sys,
     QWidget,
-    QPainter,
-    QFont,
-    QColor,
-    QSize,
-    QPaintEvent,
-    QRect,
+    qt,
+    QPushButton,
+    QLabel,
     Qt,
-    textSize,
-    QPoint,
-    QToolButton,
-    QAction,
-    QMenu,
-    Qt
+    QFrame,
+    QStyleOption,
+    QPainter,
+    QStyle
 )
 
+from PyQtGuiLib.styles import QssStyleAnalysis
 
 
-class ListTree(QWidget):
+class Test(QWidget):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
-        self.resize(300,600)
+        self.resize(600,600)
+
 
-        # 默认节点高度
-        self.__item_height = 55
-        self.__margin = 5
-
-        self.__items = [
-            {"bg":{
-            "rect": QRect(5, 5, -1, 50)
-           },
-           "text":{
-                "text":"hello",
-               "pos":QPoint(-1,25)
-        }},
-            {"bg":{
-            "rect": QRect(5,5*2+50,-1,50)
-           },
-           "text":{
-                "text":"hello",
-               "pos":QPoint(-1,75)
-        }}]
-
-    def count(self)->int:
-        return len(self.__items)
-
-    def addItem(self,text:str):
-        if self.count() == 0:
-            self.__items.append({
-
-            })
-        elif self.count() > 0:
-            pass
-
-    def addItems(self,data:list):
-        for info in data:
-            pass
-
-
-
-    def paintEvent(self, e: QPaintEvent) -> None:
-        painter = QPainter(self)
-
-        for item in self.__items:
-            rect = item["bg"]["rect"] # type:QRect
-            text = item["text"]["text"] # type:str
-            t_pos = item["text"]["pos"] # type:QPoint
-
-            # 绘制背景
-            painter.setPen(Qt.NoPen)
-            painter.setBrush(QColor("#55ffff"))
-            x,y = rect.x(),rect.y()
-            if rect.width() == -1:
-                w = self.width()-x*2
-            h = rect.height()
-            painter.drawRoundedRect(x,y,w,h,5,5)
-
-            # 绘制文本
-            painter.setPen(QColor("#000"))
-            f = QFont(text)
-            fsize = textSize(f,text)
-            fw,fh = fsize.width(),fsize.height()
-            x = w//2-fw//2
-            y = t_pos.y()+fh//2+5
-            painter.drawText(x,y,text)
+        self.setAttribute(Qt.WA_StyledBackground,True)
 
-        painter.end()
+        self.l = QLabel("测试标签",self)
+        self.btn = QPushButton("测试按钮",self)
+        self.btn.setObjectName("btn")
+        self.btn2 = QPushButton("测试按钮2号",self)
+        self.l.move(30, 30)
+        self.btn.resize(150, 80)
+        self.btn.move(80, 80)
+        self.btn2.resize(100,60)
+        self.btn2.move(250,80)
+
+        '''
+            解析 测试2
+        '''
+
+        # 创建一个针对整个窗口的 QSS 解析器
+        self.qss = QssStyleAnalysis(self)
+        # 对窗口上所有按钮,标签设置样式
+        self.qss.setQSS('''
+        QPushButton{
+        color: rgb(0, 255, 127);
+        background-color:rgb(0, 170, 0);
+        }
+        QLabel{
+        color: rgb(42, 55, 127);
+        background-color:rgb(255, 170, 0);
+        }
+        ''')
+
+        print("-------------------------------")
+        print(self.qss.selector("QPushButton").attr("color")) # 获取该选择器下面某个属性的值
+        self.qss.selector("QPushButton").updateAttr("background-color","red") # 修改背景样式
+        # self.qss.selector("QLabel").removeAttr("background-color") # 移除该标签的属性
+        self.qss.removeSelector("QPushButton") # 移除该选择器的所有样式
+
+        print("--------")
+        self.qss.appendQSSDict({
+            "QPushButton":{
+                "border":"2px solid red"
+            }
+        })
+        self.qss.appendQSS('''
+        QPushButton:hover{
+        border:2px solid blue;
+        }
+        ''')
 
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
 
-    win = ListTree()
+    win = Test()
     win.show()
 
     if PYQT_VERSIONS in ["PyQt6","PySide6"]:
         sys.exit(app.exec())
     else:
         sys.exit(app.exec_())
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/particle/particle.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/particle/particle.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/buttons/buttonStyle.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/buttons/buttonStyle.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/component.py` & `PyQtGuiLib-2.8.20.0/abandonCase/linker/component.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/controlType.py` & `PyQtGuiLib-2.8.20.0/abandonCase/linker/controlType.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/styleLinker.py` & `PyQtGuiLib-2.8.20.0/abandonCase/linker/styleLinker.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,33 +15,31 @@
     PYQT_VERSIONS,
     QApplication,
     sys,
     QWidget,
     QPushButton,
     QLabel,
     QObject,
-    qt,
     QTreeWidgetItem,
     QLineEdit,
     Qt,
     QMenu,
     QAction,
     QCursor,
     QListWidget,
     QListWidgetItem,
     QMessageBox
 )
 from PyQtGuiLib.styles import QssStyleAnalysis
 from functools import partial
-from PyQtGuiLib.core import PaletteFrame
 from PyQtGuiLib.core.flowLayout import FlowLayout
-from PyQtGuiLib.styles.linker.styleLinkerUi import StyleLinkerUI
+from abandonCase.linker.styleLinkerUi import StyleLinkerUI
 
-from PyQtGuiLib.styles.linker.controlType import getStyleLists,getStyleCommentLists,getMergeStyles
-from PyQtGuiLib.styles.linker.component import (
+from abandonCase.linker.controlType import getStyleLists,getStyleCommentLists,getMergeStyles
+from abandonCase.linker.component import (
     RegisterComponent
 )
 
 
 # 改类是TAB上创建的QWidget
 class TWidget(QWidget):
     def __init__(self,*args,**kwargs):
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/styleLinkerUi.py` & `PyQtGuiLib-2.8.20.0/abandonCase/linker/styleLinkerUi.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/drak/qssDrak.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/drak/qssDrak.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/image/image_rc.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/image/image_rc.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/qssFile.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/qssFile.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/test.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/skinABC.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/skinABC.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/styleAnalysis.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/styleAnalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     QMutex
 )
 import typing
 import re
 
 Ang = typing.TypeVar("Any",str,int)
 
+
 def dictTostr(qss_dict)->str:
     combination = ""
     for selector, attribute in qss_dict.items():
         combination += selector + "{\n"
         for attrk, attrv in attribute.items():
             combination += "%s:%s;\n" % (attrk, attrv)
         combination += "}\n"
@@ -238,28 +239,28 @@
             return self.removeSelectorIndex(ang)
         elif isinstance(ang, str):
             return self.removeSelectorKey(ang)
         else:
             raise TypeError("Parameter error!")
 
     def isSelectKey(self,key:str):
-        if self._map_qss.get(key,-1)>=0:
+        if self._map_qss.get(key,-1) >= 0:
             return True
         return False
 
-    def toDict(self)->dict:
+    def toDict(self) -> dict:
         qss_dict = dict()
         for i in range(self.count()):
             qss_dict.update(self.selectorIndex(i).toDict())
         return qss_dict
 
-    def header(self)->list:
+    def header(self) -> list:
         return list(self.toDict().keys())
 
-    def toStr(self)->str:
+    def toStr(self) -> str:
         return dictTostr(self.toDict())
 
     def __updateStyle(self, parent):
         # Thread safety
         self.__mutex.lock()
         parent.setStyleSheet("")
         parent.setStyleSheet(self.toStr())
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/superPainter/superPainter.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/superPainter/superPainter.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/superPainter.py` & `PyQtGuiLib-2.8.20.0/abandonCase/superPainter.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self.__brush = None
         self.__font = None
 
         self.__parent = parent  # type:QWidget
 
         if parent:
             self.begin()
-            self.painter().setRenderHints(QPainter.Antialiasing | QPainter.HighQualityAntialiasing | QPainter.SmoothPixmapTransform)
+            self.painter().setRenderHints(qt.Antialiasing | qt.SmoothPixmapTransform | qt.TextAntialiasing)
 
         # 默认画笔
         op = QPen()
         op.setColor(qt.black)
         self.setPen(op)
 
     def painter(self) -> QPainter:
@@ -497,26 +497,21 @@
 
 
     def paintEvent(self, event:QPaintEvent) -> None:
         # -------
         painter = SuperPainter(self)
         painter.setRenderHints(qt.Antialiasing | qt.SmoothPixmapTransform | qt.TextAntialiasing)
 
-        # painter.drawRoundedRect(300,300,100,100,openAttr={"c":QColor(0,0,255)},
-        #                  brushAttr={"c":QColor(0,255,0)})
-        # painter.drawLine(100,50,80)
-        # painter.drawText(50,50)
+        painter.drawRoundedRect(300,300,100,100,openAttr={"c":QColor(0,0,255)},
+                         brushAttr={"c":QColor(0,255,0)})
+        painter.drawLine(100,50,80)
+        painter.drawText(50,50)
         # painter.drawArc()
         # painter.drawChord()
-        painter.drawConvexPolygon([QPoint(50,50),QPoint(350,50)],openAttr={"c":QColor(255,60,60)})
-
-
-
-
-
+        # painter.drawConvexPolygon([QPoint(50,50),QPoint(350,50)],openAttr={"c":QColor(255,60,60)})
 '''
 drawRect().hover()
 '''
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
     win = Test()
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib.egg-info/PKG-INFO` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtGuiLib
-Version: 2.7.20.11
+Version: 2.8.20.0
 Summary: Python version of the qt component library.
 Home-page: https://github.com/LX-sys/PyQtGuiLib
 Author: LX
 Author-email: lx984608061@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyQtGuiLib-2.7.20.11/PyQtGuiLib.egg-info/SOURCES.txt` & `PyQtGuiLib-2.8.20.0/PyQtGuiLib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 LICENSE.txt
 README.md
 setup.py
 Log/__init__.py
 Log/developmentLog.py
 PyQtGuiLib/__init__.py
-PyQtGuiLib/listTree.py
 PyQtGuiLib.egg-info/PKG-INFO
 PyQtGuiLib.egg-info/SOURCES.txt
 PyQtGuiLib.egg-info/dependency_links.txt
 PyQtGuiLib.egg-info/top_level.txt
 PyQtGuiLib/animation/PropertyAnimation.py
 PyQtGuiLib/animation/__init__.py
 PyQtGuiLib/animation/animation.py
-PyQtGuiLib/animation/test_animation.py
 PyQtGuiLib/core/__init__.py
 PyQtGuiLib/core/bubbleWidget.py
 PyQtGuiLib/core/expansionBar.py
 PyQtGuiLib/core/flowLayout.py
 PyQtGuiLib/core/imageButton.py
 PyQtGuiLib/core/listWidget.py
 PyQtGuiLib/core/pullOver.py
 PyQtGuiLib/core/rollWidget.py
 PyQtGuiLib/core/slideShow.py
 PyQtGuiLib/core/toolBox.py
 PyQtGuiLib/core/toolList.py
 PyQtGuiLib/core/comboBox/__init__.py
-PyQtGuiLib/core/comboBox/combBox.py
 PyQtGuiLib/core/comboBox/comboBox.py
-PyQtGuiLib/core/comboBox/comboBox2.py
+PyQtGuiLib/core/comboBox/comboCheckBox/__init__.py
+PyQtGuiLib/core/comboBox/comboCheckBox/comboCheckBox.py
+PyQtGuiLib/core/comboBox/comboCheckBox/py_message_box.py
+PyQtGuiLib/core/comboBox/comboCheckBox/py_style.py
 PyQtGuiLib/core/drawers/__init__.py
 PyQtGuiLib/core/drawers/drawer.py
 PyQtGuiLib/core/lineedit/__init__.py
 PyQtGuiLib/core/lineedit/dynamicTLine.py
 PyQtGuiLib/core/logBrowser/__init__.py
 PyQtGuiLib/core/logBrowser/loadLogTh.py
 PyQtGuiLib/core/logBrowser/logBrowser.py
@@ -79,26 +79,20 @@
 PyQtGuiLib/layoutDeformation/__init__.py
 PyQtGuiLib/layoutDeformation/test.py
 PyQtGuiLib/particle/__init__.py
 PyQtGuiLib/particle/particle.py
 PyQtGuiLib/styles/__init__.py
 PyQtGuiLib/styles/skinABC.py
 PyQtGuiLib/styles/styleAnalysis.py
-PyQtGuiLib/styles/superPainter.py
 PyQtGuiLib/styles/builtStyleDesigner/__init__.py
 PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py
 PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py
 PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py
 PyQtGuiLib/styles/buttons/__init__.py
 PyQtGuiLib/styles/buttons/buttonStyle.py
-PyQtGuiLib/styles/linker/__init__.py
-PyQtGuiLib/styles/linker/component.py
-PyQtGuiLib/styles/linker/controlType.py
-PyQtGuiLib/styles/linker/styleLinker.py
-PyQtGuiLib/styles/linker/styleLinkerUi.py
 PyQtGuiLib/styles/qssFile/__init__.py
 PyQtGuiLib/styles/qssFile/qssFile.py
 PyQtGuiLib/styles/qssFile/test.py
 PyQtGuiLib/styles/qssFile/drak/__init__.py
 PyQtGuiLib/styles/qssFile/drak/config.py
 PyQtGuiLib/styles/qssFile/drak/qssDrak.py
 PyQtGuiLib/styles/qssFile/image/__init__.py
@@ -114,44 +108,50 @@
 abandonCase/__init__.py
 abandonCase/bubbleWidget.py
 abandonCase/bubbleWidget_case.py
 abandonCase/nodeBar.py
 abandonCase/slideShow.py
 abandonCase/slideShow2.py
 abandonCase/spaceWidget.py
+abandonCase/superPainter.py
 abandonCase/acrylic/__init__.py
 abandonCase/acrylic/acrylicWidget.py
 abandonCase/acrylic/cstruct.py
 abandonCase/acrylic/windowEffect.py
 abandonCase/animation/__init__.py
 abandonCase/animation/animation.py
 abandonCase/animation/animationDrawType.py
 abandonCase/animation/animationFactory.py
 abandonCase/animation/animationLayout.py
 abandonCase/animation/customAniTest.py
+abandonCase/linker/__init__.py
+abandonCase/linker/component.py
+abandonCase/linker/controlType.py
+abandonCase/linker/styleLinker.py
+abandonCase/linker/styleLinkerUi.py
 abandonCase/widgets/__init__.py
 abandonCase/widgets/borderlessFrame.py
 abandonCase/widgets/borderlessMainWindow.py
 abandonCase/widgets/borderlessStackedWidget.py
 abandonCase/widgets/borderlessWidget.py
 abandonCase/widgets/borderlessWidgetABC.py
 abandonCase/widgets/statusBar.py
 abandonCase/widgets/titleBar.py
 auxiliaryMeans/__init__.py
 auxiliaryMeans/toolNewProject.py
 tests/__init__.py
 tests/test_BubbleWidget.py
 tests/test_CircularProgressBar.py
+tests/test_ComboCheckBox.py
 tests/test_Notice.py
 tests/test_QssStyleAnalysis.py
 tests/test_SlideShow.py
 tests/test_barset.py
 tests/test_circularBar.py
 tests/test_colorPalette.py
-tests/test_comboBox.py
 tests/test_drawer.py
 tests/test_dumpStructure.py
 tests/test_dynamicTLine.py
 tests/test_expansionBar.py
 tests/test_flowLayot.py
 tests/test_gradientBar.py
 tests/test_imageButton.py
@@ -166,39 +166,26 @@
 tests/test_styles.py
 tests/test_switchButton.py
 tests/test_template.py
 tests/test_toolList.py
 tests/test_waterBar.py
 tests/test_Animation/1.py
 tests/test_Animation/__init__.py
-tests/test_Animation/eg1.py
-tests/test_Animation/tutorial_1.py
-tests/test_Animation/tutorial_10.py
-tests/test_Animation/tutorial_2.py
-tests/test_Animation/tutorial_3.py
-tests/test_Animation/tutorial_4.py
-tests/test_Animation/tutorial_5.py
-tests/test_Animation/tutorial_6.py
-tests/test_Animation/tutorial_7.py
-tests/test_Animation/tutorial_8.py
-tests/test_Animation/tutorial_9.py
+tests/test_Animation/test_animation.py
 tests/test_Animation/test_ani/1.py
 tests/test_Animation/test_ani/__init__.py
 tests/test_QssStyleAnalysis/__init__.py
 tests/test_QssStyleAnalysis/eg1.py
 tests/test_QssStyleAnalysis/eg2.py
 tests/test_QssStyleAnalysis/eg3.py
 tests/test_QssStyleAnalysis/eg4.py
 tests/test_QssStyleAnalysis/eg5.py
 tests/test_QssStyleAnalysis/eg6.py
 tests/test_QssStyleAnalysis/eg7.py
 tests/test_QssStyleAnalysis/test.py
-tests/test_StyleLinker/__init__.py
-tests/test_StyleLinker/eg1_QPushButton.py
-tests/test_StyleLinker/eg2_QLabel.py
 tests/test_SuperPainter/1.py
 tests/test_SuperPainter/__init__.py
 tests/test_SuperPainter/eg1.py
 tests/test_SuperPainter/eg2.py
 tests/test_SuperPainter/eg3.py
 tests/test_SuperPainter/eg4.py
 tests/test_SuperPainter/test.py
```

### Comparing `PyQtGuiLib-2.7.20.11/README.md` & `PyQtGuiLib-2.8.20.0/README.md`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/acrylic/acrylicWidget.py` & `PyQtGuiLib-2.8.20.0/abandonCase/acrylic/acrylicWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/acrylic/cstruct.py` & `PyQtGuiLib-2.8.20.0/abandonCase/acrylic/cstruct.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/acrylic/windowEffect.py` & `PyQtGuiLib-2.8.20.0/abandonCase/acrylic/windowEffect.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/animation/animation.py` & `PyQtGuiLib-2.8.20.0/abandonCase/animation/animation.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/animation/animationDrawType.py` & `PyQtGuiLib-2.8.20.0/abandonCase/animation/animationDrawType.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/animation/animationFactory.py` & `PyQtGuiLib-2.8.20.0/abandonCase/animation/animationFactory.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/animation/animationLayout.py` & `PyQtGuiLib-2.8.20.0/abandonCase/animation/animationLayout.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/animation/customAniTest.py` & `PyQtGuiLib-2.8.20.0/abandonCase/animation/customAniTest.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/bubbleWidget.py` & `PyQtGuiLib-2.8.20.0/abandonCase/bubbleWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/bubbleWidget_case.py` & `PyQtGuiLib-2.8.20.0/abandonCase/bubbleWidget_case.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/nodeBar.py` & `PyQtGuiLib-2.8.20.0/abandonCase/nodeBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/slideShow.py` & `PyQtGuiLib-2.8.20.0/abandonCase/slideShow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/slideShow2.py` & `PyQtGuiLib-2.8.20.0/abandonCase/slideShow2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessFrame.py` & `PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessFrame.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessMainWindow.py` & `PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessMainWindow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessStackedWidget.py` & `PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessStackedWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessWidget.py` & `PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessWidgetABC.py` & `PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessWidgetABC.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/abandonCase/widgets/titleBar.py` & `PyQtGuiLib-2.8.20.0/abandonCase/widgets/titleBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/auxiliaryMeans/toolNewProject.py` & `PyQtGuiLib-2.8.20.0/auxiliaryMeans/toolNewProject.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/setup.py` & `PyQtGuiLib-2.8.20.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 
 setup(
     name="PyQtGuiLib",
     packages =find_packages(),
-    version="2.7.20.11",
+    version="2.8.20.0",
     author="LX",
     author_email = "lx984608061@163.com",
     description = "Python version of the qt component library.",
     long_description=open('README.md', 'r',encoding="utf8").read(),
     long_description_content_type="text/markdown",
     url = "https://github.com/LX-sys/PyQtGuiLib",
     classifiers = [
```

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_Animation/1.py` & `PyQtGuiLib-2.8.20.0/tests/test_Animation/1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_Animation/__init__.py` & `PyQtGuiLib-2.8.20.0/tests/test_Animation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_Animation/test_ani/1.py` & `PyQtGuiLib-2.8.20.0/tests/test_Animation/test_ani/1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_1.py` & `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,74 @@
 # -*- coding:utf-8 -*-
-# @time:2023/3/2210:55
+# @time:2023/4/69:35
 # @author:LX
-# @file:tutorial_1.py
+# @file:test.py
 # @software:PyCharm
+
+
 from PyQtGuiLib.header import (
-    QApplication,
     PYQT_VERSIONS,
+    QApplication,
     sys,
     QWidget,
     QPushButton,
-    QRect,
-    QPoint
+    QLabel,
+    Qt,
 )
 
-# 动画框架
-from PyQtGuiLib.animation import Animation
+from PyQtGuiLib.styles import QssStyleAnalysis
+
 
 class Test(QWidget):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
         self.resize(600,600)
-        '''
-             Animation 动画框架 案例一,移动一个按钮
-        '''
 
-        self.btn = QPushButton("按钮",self)
-        self.btn.move(50,50)
-        self.btn.resize(100,60)
-
-        # 实例化动画类
-        self.ani = Animation(self)
-        # 设置动画时长
-        self.ani.setDuration(2000) # 2秒
 
-        # 对按钮添加移动动画
+        self.setAttribute(Qt.WA_StyledBackground,True)
+
+        self.l = QLabel("测试标签",self)
+        self.btn = QPushButton("测试按钮",self)
+        self.btn.setObjectName("btn")
+        self.btn.setObjectName("btn")
+        self.btn2 = QPushButton("测试按钮2号",self)
+        self.l.move(30, 30)
+        self.btn.resize(150, 80)
+        self.btn.move(80, 80)
+        self.btn2.resize(100,60)
+        self.btn2.move(250,80)
+
         '''
-            addAni() 这个方法是一个非常常用的函数,用于添加一个动画
-            参数是一个json格式,
-            这里使用的参数含义
-            targetObj:表示动画的作用对象
-            propertyName: 动画的动作
-            sv:起始值
-            ev:结束值
+            解析 测试1 
         '''
-        self.ani.addAni({
-            "targetObj": self.btn,
-            "propertyName": b"pos", # pos动作 是表示移动
-            "sv": self.btn.pos(),
-            "ev": QPoint(300,100)
-        })
-        # 开始动画
-        self.ani.start()
 
+        # 创建一个针对整个窗口的 QSS 解析器
+        self.qss = QssStyleAnalysis(self)
+        # 对窗口上所有按钮,标签设置样式
+        self.qss.setQSS('''
+        /*===========这是一个按钮的QSS============*/
+        QWidget #btn{
+        color: rgb(0, 255, 127);
+        background-color:rgb(0, 170, 0);
+        }
+        /*
+            这是标签的样式
+        */
+        QLabel{
+        color: rgb(42, 55, 127);
+        background-color:rgb(255, 170, 0);
+        }
+        ''')
+        # print(self.qss.toStr()) # 返回样式的原始的类型
+        # print(self.qss.toDict()) # 返回样式的字典类型
+
+
+        # self.qss.selector("QPushButton").updateAttr("color","yellow")
+        print( self.qss.selector("QWidget #btn").toStr())
+        # print( self.qss.selector("QWidget #btn").headerSubdivision())
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
 
     win = Test()
     win.show()
```

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_2.py` & `PyQtGuiLib-2.8.20.0/tests/test_ComboCheckBox.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,42 @@
 # -*- coding:utf-8 -*-
-# @time:2023/3/2211:07
+# @time:2023/4/2516:11
 # @author:LX
-# @file:tutorial_2.py
+# @file:test_ComboCheckBox.py
 # @software:PyCharm
 from PyQtGuiLib.header import (
-    QApplication,
     PYQT_VERSIONS,
+    QApplication,
     sys,
     QWidget,
-    QPushButton,
-    QRect,
-    QPoint,
-    QSize
 )
 
-# 动画框架
-from PyQtGuiLib.animation import Animation
+from PyQtGuiLib.core import ComboCheckBox
+
 
 class Test(QWidget):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
         self.resize(600,600)
-        '''
-             Animation 动画框架 案例二,改变一个按钮的大小
-        '''
-
-        self.btn = QPushButton("按钮",self)
-        self.btn.move(50,50)
-        self.btn.resize(100,60)
-
-        # 实例化动画类
-        self.ani = Animation(self)
-        # 设置动画时长
-        self.ani.setDuration(2000) # 2秒
-
-        # 对按钮添加缩放动画
-        self.ani.addAni({
-            "targetObj": self.btn,
-            "propertyName": b"size",
-            "sv": self.btn.size(),
-            "ev": QSize(150,100)
-        })
-        # 开始动画
-        self.ani.start()
+
+        self.combox = ComboCheckBox(
+            self,
+            obj_name='extendCCBox',
+            spacing=0,
+            width=500,
+            items=[]
+        )
+        lst = ['齐辉0', '齐辉1', '齐辉2', '齐辉3', '悯农', '骆宾王', '凡士林', '孙悟空', '李逵', '迈阿密', '黑龙江', '石油',
+               '前十', '酱油', '狐狸', '寒冰', '开户行', '天行健君子以自强不息', '业精于勤荒于嬉行成于思毁于随']
+
+        self.combox.add_items(lst)
+        self.combox.only_text('齐辉0')
+
+        self.combox.linSignal[object].connect(lambda x: print(x))
+        print(self.combox.currentText())
 
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
 
     win = Test()
     win.show()
```

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_5.py` & `PyQtGuiLib-2.8.20.0/tests/test_toolList.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,57 @@
 # -*- coding:utf-8 -*-
-# @time:2023/3/2211:19
+# @time:2023/3/1311:27
 # @author:LX
-# @file:tutorial_5.py
+# @file:test_toolList.py
 # @software:PyCharm
 from PyQtGuiLib.header import (
-    QApplication,
     PYQT_VERSIONS,
+    QApplication,
     sys,
     QWidget,
+    qt,
     QPushButton,
-    QRect,
-    QPoint,
-    QSize
+    QHBoxLayout,
+    QListWidget
+
 )
+'''
+    ToolListWidget 测试
+'''
+
+from functools import partial
+
+from PyQtGuiLib.core import ToolListWidget,ToolListItem
 
-# 动画框架
-from PyQtGuiLib.animation import Animation
 
 class Test(QWidget):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
+
         self.resize(600,600)
-        '''
-             Animation 动画框架 案例五,串行动画
-             让一个按钮先移动完成之后,在变大,
-             
-             注意: 动作的执行顺序,与添加动作的顺序有关
-        '''
-
-        self.btn = QPushButton("按钮",self)
-        self.btn.move(50,50)
-        self.btn.resize(100,60)
-
-        # 实例化动画类
-        self.ani = Animation(self)
-        # 关键设置(Animation.Sequential 表示串行动画)
-        self.ani.setAniMode(Animation.Sequential) # Animation.Parallel 这个是默认设置,也就是并行动画
-        # 设置动画时长
-        self.ani.setDuration(2000) # 2秒
-
-        # 再添加一个移动的动画
-        self.ani.addAni({
-            "targetObj": self.btn,
-            "propertyName": b"pos",
-            "sv": self.btn.pos(),
-            "ev": QPoint(300, 100)
-        })
-        # 对按钮添加缩放动画
-        self.ani.addAni({
-            "targetObj": self.btn,
-            "propertyName": b"size",
-            "sv": self.btn.size(),
-            "ev": QSize(150, 100)
-        })
 
-        # 开始动画
-        self.ani.start()
+        self.hboy = QHBoxLayout(self)
+
+        self.left = ToolListWidget()
+        self.left.setFixedWidth(200)
+        self.rigth = QWidget()
+        self.rigth.setStyleSheet('''
+        border:1px solid red;
+        ''')
+
+        self.hboy.addWidget(self.left)
+        self.hboy.addWidget(self.rigth)
+
+        # temp1 = ToolListItem("测试数据一号")
+        # temp2 = ToolListItem("测试数据二号")
+        #
+        # self.left.addItem(temp1)
+        # self.left.addItem(temp2)
+        self.left.addItems(["111","xx"])
+        print(self.left.getUnfoldItems())
 
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
 
     win = Test()
     win.show()
```

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_9.py` & `PyQtGuiLib-2.8.20.0/tests/test_circularBar.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,68 @@
-# -*- coding:utf-8 -*-
-# @time:2023/3/239:14
-# @author:LX
-# @file:tutorial_9.py
-# @software:PyCharm
 from PyQtGuiLib.header import (
-    QApplication,
     PYQT_VERSIONS,
     sys,
-    QWidget,
-    QPushButton,
-    QColor,
-    QLabel
+    QApplication,
+    QMainWindow,
+    QThread,
+    Signal,
+    QColor
 )
 
-# 动画框架
-from PyQtGuiLib.animation import Animation
+from PyQtGuiLib.core.progressBar import CircularBar
 
 
-class Test(QWidget):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.resize(600, 600)
-        '''
-             Animation 动画框架 案例九,利用QSS属性动作,
-             来 制作透明动画
-
-             注意:使用这一类动画时,你的控件必须有qss样式
-        '''
-        self.btn = QPushButton("按钮", self)
-        self.btn.move(50, 50)
-        self.btn.resize(100, 60)
-        # 这里我们写一个带透明度的背景样式
-        self.btn.setStyleSheet('''
-        QPushButton{
-            background-color:rgba(234,234,234,255);
-        }
+class DurationTimeThread(QThread):
+    added = Signal(int)
+    def __init__(self,*args,**kwargs):
+        super().__init__(*args,**kwargs)
+
+
+    def run(self) -> None:
+        n=1
+        while True:
+            self.added.emit(n)
+            n+=1
+            self.msleep(80)
+            if n == 100+1:
+                break
+
+class TestPullOverWidget(QMainWindow):
+    def __init__(self,*args,**kwargs):
+        super().__init__(*args,**kwargs)
+        self.resize(500,500)
+
+        self.setObjectName("test")
+        self.setStyleSheet('''
+#test{
+background-color: rgb(25, 25, 25);
+}
         ''')
 
-        # 实例化动画类
-        self.ani = Animation(self)
-        # 设置动画时长
-        self.ani.setDuration(3000)  # 3秒
-
-        # 添加一个QSS属性动画,通过降低rgba 中的 a属性来达到透明效果
-        self.ani.addAni({
-            "targetObj": self.btn,
-            "propertyName": b"background-color",
-            "sv":"this",
-            "ev": QColor(234,234,234,50),
-            "selector": "QPushButton"
-        })
-        # 开始动画
-        self.ani.start()
+        self.th = DurationTimeThread()
+        self.th.added.connect(self.test)
+
 
+        self.cir = CircularBar(self)
+        self.cir.resize(150,150)
+        self.cir.setVariableLineSegment(CircularBar.Double)
+        self.cir.setOuterStyle(CircularBar.CustomDashLine)
+        self.cir.setOuterDashPattern([2,3,5,6])
+        self.cir.setInnerStyle(CircularBar.DashLine)
+        self.cir.setTextSize(15)
+        self.cir.move(50,50)
+        self.cir.valueChange.connect(lambda v:print("v:",v))
+
+        self.th.start()
+
+    def test(self,n):
+        self.cir.setValue(n)
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
-
-    win = Test()
+    win = TestPullOverWidget()
     win.show()
 
     if PYQT_VERSIONS in ["PyQt6", "PySide6"]:
         sys.exit(app.exec())
     else:
         sys.exit(app.exec_())
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_BubbleWidget.py` & `PyQtGuiLib-2.8.20.0/tests/test_BubbleWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_CircularProgressBar.py` & `PyQtGuiLib-2.8.20.0/tests/test_CircularProgressBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_Notice.py` & `PyQtGuiLib-2.8.20.0/tests/test_Notice.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/__init__.py` & `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg1.py` & `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg2.py` & `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,80 @@
 # -*- coding:utf-8 -*-
-# @time:2023/2/918:26
+# @time:2023/2/818:14
 # @author:LX
-# @file:eg2.py
+# @file:test_QssStyleAnalysis.py
+# @software:PyCharm
 
 
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
     QApplication,
     sys,
     QWidget,
     qt,
     QPushButton,
     QLabel,
     Qt,
-    QFrame,
-    QStyleOption,
-    QPainter,
-    QStyle
+    QMainWindow,
+    QPainterPath
 )
 
 from PyQtGuiLib.styles import QssStyleAnalysis
 
 
-class Test(QWidget):
+class Test(QMainWindow):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
         self.resize(600,600)
 
-
-        self.setAttribute(Qt.WA_StyledBackground,True)
-
         self.l = QLabel("测试标签",self)
         self.btn = QPushButton("测试按钮",self)
-        self.btn.setObjectName("btn")
-        self.btn2 = QPushButton("测试按钮2号",self)
+
+        # QSS 解析器
+        # self.qss = QssStyleAnalysis(self)
+        # self.qss.setQSS('''
+        # QPushButton{
+        # color: rgb(0, 255, 127);
+        # background-color:rgb(0, 170, 0);
+        # }
+        # QPushButton:hover{
+        # }
+        # ''')
+        # self.qss.appendQSSDict({
+        #     "QLabel":{
+        #         "border":"2px solid yellow",
+        #         "background-color":"rgb(150,20,200)",
+        #     },
+        #     "QLabel:hover": {
+        #         "border": "2px solid blue",
+        #         "color": "red",
+        #     }
+        # })
+        # self.qss.selector("QPushButton").updateAttr("background-color", "rgb(255,0,0)")
+        # # self.qss.selectorPoint("QPushButton.color")
+
         self.l.move(30, 30)
-        self.btn.resize(150, 80)
-        self.btn.move(80, 80)
-        self.btn2.resize(100,60)
-        self.btn2.move(250,80)
-
-        '''
-            解析 测试2
-        '''
+        self.btn.resize(150,80)
+        self.btn.move(80,80)
 
         # 创建一个针对整个窗口的 QSS 解析器
         self.qss = QssStyleAnalysis(self)
         # 对窗口上所有按钮,标签设置样式
         self.qss.setQSS('''
-        QPushButton{
-        color: rgb(0, 255, 127);
-        background-color:rgb(0, 170, 0);
-        }
-        QLabel{
-        color: rgb(42, 55, 127);
-        background-color:rgb(255, 170, 0);
-        }
-        ''')
-
-        print("-------------------------------")
-        print(self.qss.selector("QPushButton").attr("color")) # 获取该选择器下面某个属性的值
-        self.qss.selector("QPushButton").updateAttr("background-color","red") # 修改背景样式
-        # self.qss.selector("QLabel").removeAttr("background-color") # 移除该标签的属性
-        self.qss.removeSelector("QPushButton") # 移除该选择器的所有样式
-
-        print("--------")
-        self.qss.appendQSSDict({
-            "QPushButton":{
-                "border":"2px solid red"
-            }
-        })
-        self.qss.appendQSS('''
-        QPushButton:hover{
-        border:2px solid blue;
-        }
-        ''')
+                QPushButton{
+                color: rgb(0, 255, 127);
+                background-color:rgb(0, 170, 0);
+                }
+                QLabel{
+                color: rgb(42, 55, 127);
+                background-color:rgb(255, 170, 0);
+                }
+                ''')
+        self.qss.selector("QPushButton").updateAttr("background-color", "red")  #
+        print(self.styleSheet())
 
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
 
     win = Test()
     win.show()
```

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg3.py` & `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg3.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg4.py` & `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg4.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg5.py` & `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg5.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg6.py` & `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg6.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg7.py` & `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg7.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis.py` & `PyQtGuiLib-2.8.20.0/tests/test_no_border.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,81 @@
 # -*- coding:utf-8 -*-
-# @time:2023/2/818:14
+# @time:2022/12/2710:59
 # @author:LX
-# @file:test_QssStyleAnalysis.py
+# @file:test_gradientBar.py
 # @software:PyCharm
-
-
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
-    QApplication,
     sys,
-    QWidget,
-    qt,
+    QApplication,
     QPushButton,
-    QLabel,
-    Qt,
-    QMainWindow,
-    QPainterPath
+    qt,
+    QPropertyAnimation,
+    QColor,
+    QGraphicsBlurEffect,
+    QLabel
 )
 
-from PyQtGuiLib.styles import QssStyleAnalysis
-
+from PyQtGuiLib.core.widgets import BorderlessWidget
+'''
+    无边框QWidget窗口 测试
+'''
 
-class Test(QMainWindow):
+class TestNoBorder(BorderlessWidget):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
-        self.resize(600,600)
+        self.resize(500,500)
 
-        self.l = QLabel("测试标签",self)
-        self.btn = QPushButton("测试按钮",self)
+        # self.setEnableGColor(True)
+        self.setStyleSheet('''
+        WidgetABC{
+        qproperty-radius:10;
+        qproperty-backgroundColor: rgba(240, 240, 240,255);
+        /*qproperty-linearDirection:"LR";
+        qproperty-linearColor:"rgba(142, 144, 69, 255) rgba(176, 184, 130, 255) rgba(130, 184, 130, 255)";
+        qproperty-linear:"LR rgba(142, 144, 69, 255) rgba(176, 184, 130, 255) rgba(130, 184, 130, 255)";*/
+        qproperty-border:"1 solid rgba(0, 0, 0, 255)";
+        /*qproperty-ani:xx; 窗口动画*/
+        }
+        #     ''')
 
-        # QSS 解析器
-        # self.qss = QssStyleAnalysis(self)
-        # self.qss.setQSS('''
-        # QPushButton{
-        # color: rgb(0, 255, 127);
-        # background-color:rgb(0, 170, 0);
-        # }
-        # QPushButton:hover{
-        # }
-        # ''')
-        # self.qss.appendQSSDict({
-        #     "QLabel":{
-        #         "border":"2px solid yellow",
-        #         "background-color":"rgb(150,20,200)",
-        #     },
-        #     "QLabel:hover": {
-        #         "border": "2px solid blue",
-        #         "color": "red",
-        #     }
-        # })
-        # self.qss.selector("QPushButton").updateAttr("background-color", "rgb(255,0,0)")
-        # # self.qss.selectorPoint("QPushButton.color")
-
-        self.l.move(30, 30)
-        self.btn.resize(150,80)
-        self.btn.move(80,80)
-
-        # 创建一个针对整个窗口的 QSS 解析器
-        self.qss = QssStyleAnalysis(self)
-        # 对窗口上所有按钮,标签设置样式
-        self.qss.setQSS('''
-                QPushButton{
-                color: rgb(0, 255, 127);
-                background-color:rgb(0, 170, 0);
-                }
-                QLabel{
-                color: rgb(42, 55, 127);
-                background-color:rgb(255, 170, 0);
-                }
-                ''')
-        self.qss.selector("QPushButton").updateAttr("background-color", "red")  #
-        print(self.styleSheet())
 
 
+        self.flag = False
+        # self.btn = QPushButton("固定", self)
+        # self.btn.resize(self.size())
+        # self.btn.move(100, 100)
+        # self.btn.clicked.connect(self.test)
+
+
+    def test(self):
+        if self.flag is False:
+            self.btn.setText("解放")
+            self.windowHandle().setFlags(self.windowFlags() | qt.WindowStaysOnTopHint)
+            self.flag= True
+
+            self.ani = QPropertyAnimation(self, b"backgroundColor")
+            self.ani.setDuration(4000)
+            self.ani.setLoopCount(-1)
+            self.ani.setStartValue(self.get_backgroundColor())
+            self.ani.setKeyValueAt(0.4, QColor(200, 100, 45, 230))
+            self.ani.setKeyValueAt(0.6, QColor(200, 50, 45, 200))
+            self.ani.setKeyValueAt(0.8, QColor(200, 0, 45, 150))
+            self.ani.setEndValue(self.get_backgroundColor())
+            #
+            self.ani.start()
+        else:
+            self.btn.setText("固定")
+            self.windowHandle().setFlags(self.windowFlags() | qt.Widget)
+            self.flag = False
+        self.show()
+        self.update()
+
 if __name__ == '__main__':
     app = QApplication(sys.argv)
-
-    win = Test()
+    win = TestNoBorder()
     win.show()
 
-    if PYQT_VERSIONS in ["PyQt6","PySide6"]:
+    if PYQT_VERSIONS in ["PyQt6", "PySide6"]:
         sys.exit(app.exec())
     else:
         sys.exit(app.exec_())
```

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_SlideShow.py` & `PyQtGuiLib-2.8.20.0/tests/test_SlideShow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_StyleLinker/eg1_QPushButton.py` & `PyQtGuiLib-2.8.20.0/tests/test_rollWidget.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,60 @@
+# -*- coding:utf-8 -*-
+# @time:2023/1/1214:50
+# @author:LX
+# @file:test_rollWidget.py
+# @software:PyCharm
+
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
     QApplication,
     sys,
     QWidget,
     QPushButton
 )
 
-from PyQtGuiLib.styles import StyleLinker
+'''
+    滚动栏 测试用例
+'''
+
+from PyQtGuiLib.core import RollWidget
+from PyQtGuiLib.styles import ButtonStyle
+
 
-class Test(QWidget):
+class Test_RollWidget(QWidget):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
         self.resize(800,600)
 
-        self.btn = QPushButton("测试1",self)
-        self.btn.setStyleSheet('''
-        QPushButton{
-        background-color: rgb(255, 85, 127);
-        }
-        QPushButton:hover{
-        background-color: rgb(0, 85, 127);
-        }
-        ''')
-        self.btn.setGeometry(100,100,300,300)
-
-
-        self.styleLinker = StyleLinker()
-        self.styleLinker.addQObject(self.btn)
-        self.styleLinker.show()
+        # 滚动栏
+        self.rlw = RollWidget(self)
+        self.rlw.resize(500,60)
+        self.rlw.move(10,100)
+        self.rlw.changed.connect(self.test)
+
+        self.addbtn = QPushButton("动态添加",self)
+        self.addbtn.move(10,10)
+        self.addbtn.clicked.connect(self.AddBtn)
+
+        # ---
+        for i in range(3):
+            btn = QPushButton("test_{}".format(i))
+            btn.setStyleSheet("background-color:rgb(255, 255, 127);")
+            self.rlw.addWidget(btn)
+
+    def test(self,wid):
+        print(wid.text())
+
+    def AddBtn(self):
+        bt = QPushButton("dsa")
+        bt.setStyleSheet(ButtonStyle.contrastStyle())
+        self.rlw.addWidget(bt)
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
-    win = Test()
+    win = Test_RollWidget()
     win.show()
 
-    if PYQT_VERSIONS in ["PyQt6", "PySide6"]:
+    if PYQT_VERSIONS in ["PyQt6","PySide6"]:
         sys.exit(app.exec())
     else:
         sys.exit(app.exec_())
```

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_StyleLinker/eg2_QLabel.py` & `PyQtGuiLib-2.8.20.0/tests/test_template.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
     QApplication,
     sys,
     QWidget,
-    QLabel
 )
 
-from PyQtGuiLib.styles import StyleLinker
+
+# QSplashScreen
+'''
+    测试用例的标准模板,该代码用于复制
+'''
+
 
 class Test(QWidget):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
-        self.resize(800,600)
-
-        self.setStyleSheet('''
-background-color: rgb(0, 0, 0);
-        ''')
+        self.resize(600,600)
 
-        self.l = QLabel("我是标签",self)
-        self.l.setGeometry(100,100,300,300)
-
-
-        self.styleLinker = StyleLinker()
-        self.styleLinker.addQObject(self.l)
-        self.styleLinker.show()
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
+
     win = Test()
     win.show()
 
-    if PYQT_VERSIONS in ["PyQt6", "PySide6"]:
+    if PYQT_VERSIONS in ["PyQt6","PySide6"]:
         sys.exit(app.exec())
     else:
         sys.exit(app.exec_())
```

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/1.py` & `PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/eg1.py` & `PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/eg1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/eg2.py` & `PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/eg2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/eg3.py` & `PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/eg3.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/eg4.py` & `PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/eg4.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/test.py` & `PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_barset.py` & `PyQtGuiLib-2.8.20.0/tests/test_barset.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_circularBar.py` & `PyQtGuiLib-2.8.20.0/tests/test_gradientBar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+# -*- coding:utf-8 -*-
+# @time:2022/12/2710:59
+# @author:LX
+# @file:test_gradientBar.py
+# @software:PyCharm
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
     sys,
     QApplication,
     QMainWindow,
     QThread,
     Signal,
-    QColor
+    QColor,
+    QThread
 )
 
-from PyQtGuiLib.core.progressBar import CircularBar
+from PyQtGuiLib.core.progressBar import GradientBar
 
 
 class DurationTimeThread(QThread):
     added = Signal(int)
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
 
@@ -22,47 +28,48 @@
         while True:
             self.added.emit(n)
             n+=1
             self.msleep(80)
             if n == 100+1:
                 break
 
-class TestPullOverWidget(QMainWindow):
+'''
+    线性渐变进度条 测试用例
+'''
+
+class TestGradientBar(QMainWindow):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
-        self.resize(500,500)
+        self.resize(800,500)
 
-        self.setObjectName("test")
-        self.setStyleSheet('''
-#test{
-background-color: rgb(25, 25, 25);
-}
-        ''')
+        self.gbar = GradientBar(self)
+        self.gbar.move(50,50)
+        self.gbar.resize(500,10)
+        self.gbar.setValue(0)
+        self.gbar.setColorAts(
+            [(0.2, QColor(170, 170, 255)), (0.4, QColor(170, 255, 127)), (0.6, QColor(85, 170, 127))]
+        )
+        # self.gbar.appendColor((0.5,QColor(85, 85, 127)))
+        self.gbar.setRadius(3)
 
         self.th = DurationTimeThread()
         self.th.added.connect(self.test)
-
-
-        self.cir = CircularBar(self)
-        self.cir.resize(150,150)
-        self.cir.setVariableLineSegment(CircularBar.Double)
-        self.cir.setOuterStyle(CircularBar.CustomDashLine)
-        self.cir.setOuterDashPattern([2,3,5,6])
-        self.cir.setInnerStyle(CircularBar.DashLine)
-        self.cir.setTextSize(15)
-        self.cir.move(50,50)
-        self.cir.valueChange.connect(lambda v:print("v:",v))
-
         self.th.start()
 
     def test(self,n):
-        self.cir.setValue(n)
+        print(n)
+        # if n > 20 and n <50:
+        #     self.gbar.setRadius(2)
+        # elif n>50:
+        #     self.gbar.setRadius(5)
+        self.gbar.setValue(n)
+
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
-    win = TestPullOverWidget()
+    win = TestGradientBar()
     win.show()
 
     if PYQT_VERSIONS in ["PyQt6", "PySide6"]:
         sys.exit(app.exec())
     else:
         sys.exit(app.exec_())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_colorPalette.py` & `PyQtGuiLib-2.8.20.0/tests/test_colorPalette.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_comboBox.py` & `PyQtGuiLib-2.8.20.0/tests/test_loadbar.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,62 @@
 # -*- coding:utf-8 -*-
-# @time:2022/12/296:18
+# @time:2022/12/2215:14
 # @author:LX
-# @file:test_comboBox.py
+# @file:test_loadbar.py
 # @software:PyCharm
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
     sys,
     QApplication,
     QMainWindow,
     QThread,
     Signal,
-    QColor,
-    QThread,
-    Qt,
-    QPushButton
+    QColor
 )
 
-from PyQtGuiLib.core.comboBox.combBox import ComBox
+from PyQtGuiLib.core.progressBar import LoadBar
 
-'''
-    下拉框 测试用例
-'''
 
-class TestComboBox(QMainWindow):
-    sed = Signal()
+class DurationTimeThread(QThread):
+    added = Signal(int)
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
-        self.resize(800,500)
 
-        self.combox = ComBox(self)
-        # self.combox.setFocus()
-        self.combox.resize(300,50)
-        self.combox.move(100,100)
-        print(self.styleSheet())
 
-        # print(self.combox.pos())
+    def run(self) -> None:
+        n=1
+        while True:
+            self.added.emit(n)
+            n+=1
+            self.msleep(100)
+            if n == 100+1:
+                print("完成")
+                break
+
+class TestPullOverWidget(QMainWindow):
+    def __init__(self,*args,**kwargs):
+        super().__init__(*args,**kwargs)
+        self.resize(800,500)
+
+        self.loadbar = LoadBar(self)
+        self.loadbar.move(50,100)
+        self.loadbar.resize(350,45)
+        self.loadbar.setValue(0)
+
+        self.th = DurationTimeThread()
+        self.th.added.connect(self.test)
+        self.th.start()
+
+    def test(self,v):
+        print(v)
+        self.loadbar.setValue(v)
 
-    # def test(self,e):
-    #     print(e)
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
-    win = TestComboBox()
+    win = TestPullOverWidget()
     win.show()
 
     if PYQT_VERSIONS in ["PyQt6", "PySide6"]:
         sys.exit(app.exec())
     else:
         sys.exit(app.exec_())
```

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_drawer.py` & `PyQtGuiLib-2.8.20.0/tests/test_drawer.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_dynamicTLine.py` & `PyQtGuiLib-2.8.20.0/tests/test_dynamicTLine.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_expansionBar.py` & `PyQtGuiLib-2.8.20.0/tests/test_expansionBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_flowLayot.py` & `PyQtGuiLib-2.8.20.0/tests/test_flowLayot.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_imageButton.py` & `PyQtGuiLib-2.8.20.0/tests/test_imageButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_listWidget.py` & `PyQtGuiLib-2.8.20.0/tests/test_listWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_loadbar.py` & `PyQtGuiLib-2.8.20.0/tests/test_waterBar.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,68 @@
 # -*- coding:utf-8 -*-
-# @time:2022/12/2215:14
+# @time:2022/12/2217:18
 # @author:LX
-# @file:test_loadbar.py
+# @file:test_waterBar.py
 # @software:PyCharm
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
     sys,
     QApplication,
     QMainWindow,
     QThread,
     Signal,
-    QColor
+    QColor,
+    QSlider,
 )
 
-from PyQtGuiLib.core.progressBar import LoadBar
-
+from PyQtGuiLib.core.progressBar import WaterBar
 
 class DurationTimeThread(QThread):
     added = Signal(int)
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
 
 
     def run(self) -> None:
         n=1
         while True:
             self.added.emit(n)
-            n+=1
+            n += 1
             self.msleep(100)
             if n == 100+1:
                 print("完成")
                 break
 
 class TestPullOverWidget(QMainWindow):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
         self.resize(800,500)
 
-        self.loadbar = LoadBar(self)
-        self.loadbar.move(50,100)
-        self.loadbar.resize(350,45)
-        self.loadbar.setValue(0)
+        self.setObjectName("test")
+#         self.setStyleSheet('''
+# #test{
+# background-color: rgb(0, 0, 0);
+# }
+#         ''')
+
+        self.waterbar = WaterBar(self)
+        self.waterbar.resize(120,120)
+        self.waterbar.setTextSize(30)
+        self.waterbar.move(50,100)
 
         self.th = DurationTimeThread()
-        self.th.added.connect(self.test)
+        self.th.added.connect(self.test1)
         self.th.start()
 
-    def test(self,v):
-        print(v)
-        self.loadbar.setValue(v)
+    def test1(self,v):
+        self.waterbar.setValue(v)
 
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
     win = TestPullOverWidget()
     win.show()
 
-    if PYQT_VERSIONS in ["PyQt6", "PySide6"]:
+    if PYQT_VERSIONS in ["PyQt6","PySide6"]:
         sys.exit(app.exec())
     else:
         sys.exit(app.exec_())
```

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_no_border_pullOver.py` & `PyQtGuiLib-2.8.20.0/tests/test_no_border_pullOver.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_pullOverWidget.py` & `PyQtGuiLib-2.8.20.0/tests/test_pullOverWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_qssFile/test.py` & `PyQtGuiLib-2.8.20.0/tests/test_qssFile/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_slider.py` & `PyQtGuiLib-2.8.20.0/tests/test_slider.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_statusBar.py` & `PyQtGuiLib-2.8.20.0/tests/test_statusBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_styles.py` & `PyQtGuiLib-2.8.20.0/tests/test_styles.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_switchButton.py` & `PyQtGuiLib-2.8.20.0/tests/test_switchButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.20.11/tests/test_templateWindow/test_listTemplateWindow.py` & `PyQtGuiLib-2.8.20.0/tests/test_templateWindow/test_listTemplateWindow.py`

 * *Files identical despite different names*

