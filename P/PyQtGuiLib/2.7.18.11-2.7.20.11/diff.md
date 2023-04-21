# Comparing `tmp/PyQtGuiLib-2.7.18.11.tar.gz` & `tmp/PyQtGuiLib-2.7.20.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtGuiLib-2.7.18.11.tar", last modified: Tue Apr 11 06:07:32 2023, max compression
+gzip compressed data, was "PyQtGuiLib-2.7.20.11.tar", last modified: Fri Apr 21 06:54:09 2023, max compression
```

## Comparing `PyQtGuiLib-2.7.18.11.tar` & `PyQtGuiLib-2.7.20.11.tar`

### file list

```diff
@@ -1,239 +1,260 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.381422 PyQtGuiLib-2.7.18.11/
--rw-rw-rw-   0        0        0     1091 2022-12-10 10:29:38.000000 PyQtGuiLib-2.7.18.11/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.134484 PyQtGuiLib-2.7.18.11/Log/
--rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/Log/__init__.py
--rw-rw-rw-   0        0        0     9452 2023-04-11 05:53:43.000000 PyQtGuiLib-2.7.18.11/Log/developmentLog.py
--rw-rw-rw-   0        0        0    17825 2023-04-11 06:07:32.380418 PyQtGuiLib-2.7.18.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.135482 PyQtGuiLib-2.7.18.11/PyQtGuiLib/
--rw-rw-rw-   0        0        0      106 2023-04-03 06:49:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.149443 PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/
--rw-rw-rw-   0        0        0      216 2023-03-17 10:17:57.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/__init__.py
--rw-rw-rw-   0        0        0    21262 2023-03-28 10:15:34.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/animation.py
--rw-rw-rw-   0        0        0     2792 2023-03-28 09:06:54.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/animationDrawType.py
--rw-rw-rw-   0        0        0    11607 2023-03-27 02:05:15.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/animationFactory.py
--rw-rw-rw-   0        0        0     1636 2023-03-20 04:02:29.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/animationLayout.py
--rw-rw-rw-   0        0        0     2292 2023-03-15 01:17:54.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/customAniTest.py
--rw-rw-rw-   0        0        0     3076 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/lmlmAni.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.160414 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/
--rw-rw-rw-   0        0        0      540 2023-03-13 03:28:34.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/__init__.py
--rw-rw-rw-   0        0        0     5953 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/bubbleWidget.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.165401 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/comboBox/
--rw-rw-rw-   0        0        0      218 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/comboBox/__init__.py
--rw-rw-rw-   0        0        0     4854 2023-02-13 10:30:41.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/comboBox/combBox.py
--rw-rw-rw-   0        0        0     8171 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/comboBox/comboBox.py
--rw-rw-rw-   0        0        0     4107 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/comboBox/comboBox2.py
--rw-rw-rw-   0        0        0     3886 2023-02-08 01:08:13.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/flowLayout.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.167396 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/lineedit/
--rw-rw-rw-   0        0        0      170 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/lineedit/__init__.py
--rw-rw-rw-   0        0        0     3967 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/lineedit/dynamicTLine.py
--rw-rw-rw-   0        0        0     5090 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/listWidget.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.173380 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/logBrowser/
--rw-rw-rw-   0        0        0      107 2023-03-27 09:33:07.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/logBrowser/__init__.py
--rw-rw-rw-   0        0        0     1823 2023-03-31 09:04:34.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/logBrowser/loadLogTh.py
--rw-rw-rw-   0        0        0     5112 2023-04-03 02:45:06.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/logBrowser/logBrowser.py
--rw-rw-rw-   0        0        0      554 2023-03-31 09:29:33.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/logBrowser/logSizeTh.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.176372 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/notice/
--rw-rw-rw-   0        0        0        0 2023-02-08 01:08:13.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/notice/__init__.py
--rw-rw-rw-   0        0        0     4822 2023-02-10 11:02:17.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/notice/notice.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.179364 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/palettes/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/palettes/__init__.py
--rw-rw-rw-   0        0        0     9818 2023-02-18 01:06:47.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/palettes/colorHsv.py
--rw-rw-rw-   0        0        0     6728 2023-02-18 01:06:47.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/palettes/paletteFrame.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.185352 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/
--rw-rw-rw-   0        0        0      244 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/__init__.py
--rw-rw-rw-   0        0        0     5602 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/circularBar.py
--rw-rw-rw-   0        0        0     3943 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/gradientBar.py
--rw-rw-rw-   0        0        0     4365 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/loadBar.py
--rw-rw-rw-   0        0        0     6734 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/waterBar.py
--rw-rw-rw-   0        0        0     5092 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/pullOver.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.188340 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/resolver/
--rw-rw-rw-   0        0        0       59 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/resolver/__init__.py
--rw-rw-rw-   0        0        0      674 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/resolver/controls.py
--rw-rw-rw-   0        0        0     7628 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/rollWidget.py
--rw-rw-rw-   0        0        0     8775 2023-04-11 04:20:04.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/slideShow.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.191332 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/slider/
--rw-rw-rw-   0        0        0        0 2023-02-14 00:37:29.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/slider/__init__.py
--rw-rw-rw-   0        0        0     8623 2023-03-06 01:03:54.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/slider/slider.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.193326 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/switchButtons/
--rw-rw-rw-   0        0        0       63 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/switchButtons/__init__.py
--rw-rw-rw-   0        0        0     4993 2023-02-23 01:29:46.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/switchButtons/swButton.py
--rw-rw-rw-   0        0        0     2743 2023-03-06 05:54:08.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/toolBox.py
--rw-rw-rw-   0        0        0     5588 2023-03-14 01:24:55.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/toolList.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.202302 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/
--rw-rw-rw-   0        0        0    11338 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/WidgetABC.py
--rw-rw-rw-   0        0        0      260 2023-02-09 10:20:35.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/__init__.py
--rw-rw-rw-   0        0        0     3995 2023-02-10 07:29:38.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/borderlessMainWindow.py
--rw-rw-rw-   0        0        0      303 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/borderlessWidget.py
--rw-rw-rw-   0        0        0     4935 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/statusBar.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.206292 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/tets/
--rw-rw-rw-   0        0        0      375 2023-02-27 10:18:30.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/tets/1.py
--rw-rw-rw-   0        0        0     3504 2023-02-27 00:36:50.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/tets/2.py
--rw-rw-rw-   0        0        0        0 2023-02-24 00:57:42.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/tets/__init__.py
--rw-rw-rw-   0        0        0    17840 2023-02-10 03:56:26.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/titleBar.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.212276 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.221252 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/__init__.py
--rw-rw-rw-   0        0        0     4997 2023-02-09 08:40:57.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qt.py
--rw-rw-rw-   0        0        0     2672 2023-02-18 03:01:28.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qtCore.py
--rw-rw-rw-   0        0        0     3019 2023-02-18 05:34:36.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qtGui.py
--rw-rw-rw-   0        0        0      509 2023-02-09 08:33:46.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qtSip.py
--rw-rw-rw-   0        0        0      505 2023-02-13 08:07:57.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qtUic.py
--rw-rw-rw-   0        0        0     6996 2023-02-18 02:58:53.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qtWidgets.py
--rw-rw-rw-   0        0        0      632 2023-02-13 08:14:52.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/__init__.py
--rw-rw-rw-   0        0        0     6403 2023-02-14 05:59:02.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/customStyle.py
--rw-rw-rw-   0        0        0      262 2023-02-10 01:34:45.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/error.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.224244 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/py/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/py/__init__.py
--rw-rw-rw-   0        0        0      103 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/py/common.py
--rw-rw-rw-   0        0        0     3516 2023-02-13 08:24:26.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/utility.py
--rw-rw-rw-   0        0        0      396 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/versions.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.226239 PyQtGuiLib-2.7.18.11/PyQtGuiLib/layoutDeformation/
--rw-rw-rw-   0        0        0      106 2023-03-04 03:38:59.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/layoutDeformation/__init__.py
--rw-rw-rw-   0        0        0     4425 2023-03-07 08:03:39.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/layoutDeformation/test.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.231225 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/
--rw-rw-rw-   0        0        0      302 2023-04-07 09:06:55.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.236212 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/builtStyleDesigner/
--rw-rw-rw-   0        0        0      105 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/builtStyleDesigner/__init__.py
--rw-rw-rw-   0        0        0     7168 2023-02-24 00:57:42.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py
--rw-rw-rw-   0        0        0     5062 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py
--rw-rw-rw-   0        0        0     1237 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.239204 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/buttons/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/buttons/__init__.py
--rw-rw-rw-   0        0        0      620 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/buttons/buttonStyle.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.245838 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/
--rw-rw-rw-   0        0        0      106 2023-02-20 02:36:19.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/__init__.py
--rw-rw-rw-   0        0        0    26952 2023-02-23 01:15:37.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/component.py
--rw-rw-rw-   0        0        0     8822 2023-03-13 01:50:58.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/controlType.py
--rw-rw-rw-   0        0        0    11557 2023-02-23 09:01:24.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/styleLinker.py
--rw-rw-rw-   0        0        0     1444 2023-02-22 03:17:40.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/styleLinkerUi.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.248830 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/
--rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.252820 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/drak/
--rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/drak/__init__.py
--rw-rw-rw-   0        0        0      187 2023-03-29 08:26:42.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/drak/config.py
--rw-rw-rw-   0        0        0    11537 2023-03-30 09:13:08.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/drak/qssDrak.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.256808 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/image/
--rw-rw-rw-   0        0        0      107 2023-03-29 03:26:49.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/image/__init__.py
--rw-rw-rw-   0        0        0    29060 2023-03-30 10:20:11.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/image/image_rc.py
--rw-rw-rw-   0        0        0      300 2023-03-30 10:19:06.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/image/qssFile.py
--rw-rw-rw-   0        0        0    20518 2023-03-30 10:20:35.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/qssFile.py
--rw-rw-rw-   0        0        0     6314 2023-03-30 09:24:42.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/test.py
--rw-rw-rw-   0        0        0    10615 2023-02-09 08:32:36.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/skinABC.py
--rw-rw-rw-   0        0        0     8474 2023-04-11 01:23:59.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/styleAnalysis.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.258803 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/superPainter/
--rw-rw-rw-   0        0        0      107 2023-03-18 07:49:47.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/superPainter/__init__.py
--rw-rw-rw-   0        0        0    11549 2023-04-10 04:38:34.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/superPainter/superPainter.py
--rw-rw-rw-   0        0        0    17854 2023-03-10 06:22:00.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/superPainter.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.259810 PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.262792 PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/UI/
--rw-rw-rw-   0        0        0      193 2023-04-11 03:59:36.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/UI/__init__.py
--rw-rw-rw-   0        0        0     4564 2023-04-11 05:44:28.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.264787 PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/Window/
--rw-rw-rw-   0        0        0      107 2023-04-10 09:41:12.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/Window/__init__.py
--rw-rw-rw-   0        0        0     4891 2023-04-11 05:44:46.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py
--rw-rw-rw-   0        0        0      189 2023-04-11 04:44:35.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.140468 PyQtGuiLib-2.7.18.11/PyQtGuiLib.egg-info/
--rw-rw-rw-   0        0        0    17825 2023-04-11 06:07:32.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6566 2023-04-11 06:07:32.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 06:07:32.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-11 06:07:32.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    17395 2023-03-27 01:38:52.000000 PyQtGuiLib-2.7.18.11/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.275758 PyQtGuiLib-2.7.18.11/abandonCase/
--rw-rw-rw-   0        0        0      108 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.280744 PyQtGuiLib-2.7.18.11/abandonCase/acrylic/
--rw-rw-rw-   0        0        0       37 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/acrylic/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/acrylic/acrylicWidget.py
--rw-rw-rw-   0        0        0     1550 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/acrylic/cstruct.py
--rw-rw-rw-   0        0        0     2183 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/acrylic/windowEffect.py
--rw-rw-rw-   0        0        0     9981 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/bubbleWidget.py
--rw-rw-rw-   0        0        0     3620 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/bubbleWidget_case.py
--rw-rw-rw-   0        0        0     1411 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/nodeBar.py
--rw-rw-rw-   0        0        0     9873 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/slideShow.py
--rw-rw-rw-   0        0        0     7801 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/slideShow2.py
--rw-rw-rw-   0        0        0        0 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/spaceWidget.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.292712 PyQtGuiLib-2.7.18.11/abandonCase/widgets/
--rw-rw-rw-   0        0        0      110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/widgets/__init__.py
--rw-rw-rw-   0        0        0     1389 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessFrame.py
--rw-rw-rw-   0        0        0     1962 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessMainWindow.py
--rw-rw-rw-   0        0        0     1441 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessStackedWidget.py
--rw-rw-rw-   0        0        0     1402 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessWidget.py
--rw-rw-rw-   0        0        0    10095 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessWidgetABC.py
--rw-rw-rw-   0        0        0     5034 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/widgets/statusBar.py
--rw-rw-rw-   0        0        0    17577 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/widgets/titleBar.py
--rw-rw-rw-   0        0        0       42 2023-04-11 06:07:32.381422 PyQtGuiLib-2.7.18.11/setup.cfg
--rw-rw-rw-   0        0        0      744 2023-04-11 05:55:32.000000 PyQtGuiLib-2.7.18.11/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.326562 PyQtGuiLib-2.7.18.11/tests/
--rw-rw-rw-   0        0        0      107 2023-03-06 03:09:41.000000 PyQtGuiLib-2.7.18.11/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.342519 PyQtGuiLib-2.7.18.11/tests/test_Animation/
--rw-rw-rw-   0        0        0     1994 2023-04-05 10:25:59.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/1.py
--rw-rw-rw-   0        0        0      606 2023-03-15 09:52:36.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/__init__.py
--rw-rw-rw-   0        0        0     3285 2023-03-24 08:50:00.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/eg1.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.345511 PyQtGuiLib-2.7.18.11/tests/test_Animation/test_ani/
--rw-rw-rw-   0        0        0     6145 2023-04-05 10:32:05.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/test_ani/1.py
--rw-rw-rw-   0        0        0      107 2023-03-27 05:53:58.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/test_ani/__init__.py
--rw-rw-rw-   0        0        0     1654 2023-03-28 08:45:42.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_1.py
--rw-rw-rw-   0        0        0     1824 2023-03-28 08:48:45.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_10.py
--rw-rw-rw-   0        0        0     1305 2023-03-28 08:45:46.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_2.py
--rw-rw-rw-   0        0        0     2011 2023-03-28 08:45:51.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_3.py
--rw-rw-rw-   0        0        0     1276 2023-03-28 08:45:56.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_4.py
--rw-rw-rw-   0        0        0     1851 2023-03-28 08:46:24.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_5.py
--rw-rw-rw-   0        0        0     1759 2023-03-28 08:46:54.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_6.py
--rw-rw-rw-   0        0        0     2206 2023-03-28 08:47:16.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_7.py
--rw-rw-rw-   0        0        0     2000 2023-03-28 08:47:46.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_8.py
--rw-rw-rw-   0        0        0     1712 2023-03-28 08:48:15.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_9.py
--rw-rw-rw-   0        0        0     1541 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_BubbleWidget.py
--rw-rw-rw-   0        0        0     1592 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_Notice.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.357510 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/
--rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-04-06 02:24:28.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg1.py
--rw-rw-rw-   0        0        0     2306 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg2.py
--rw-rw-rw-   0        0        0     1891 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg3.py
--rw-rw-rw-   0        0        0     2110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg4.py
--rw-rw-rw-   0        0        0     2519 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg5.py
--rw-rw-rw-   0        0        0     1881 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg6.py
--rw-rw-rw-   0        0        0     2617 2023-03-22 05:45:33.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg7.py
--rw-rw-rw-   0        0        0     2042 2023-04-06 03:41:23.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/test.py
--rw-rw-rw-   0        0        0     2275 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis.py
--rw-rw-rw-   0        0        0     2278 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_SlideShow.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.361493 PyQtGuiLib-2.7.18.11/tests/test_StyleLinker/
--rw-rw-rw-   0        0        0        0 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_StyleLinker/__init__.py
--rw-rw-rw-   0        0        0      949 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_StyleLinker/eg1_QPushButton.py
--rw-rw-rw-   0        0        0      807 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_StyleLinker/eg2_QLabel.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.371457 PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/
--rw-rw-rw-   0        0        0        0 2023-04-10 02:56:18.000000 PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/1.py
--rw-rw-rw-   0        0        0      106 2023-04-07 09:06:55.000000 PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/__init__.py
--rw-rw-rw-   0        0        0     1568 2023-04-07 09:19:44.000000 PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/eg1.py
--rw-rw-rw-   0        0        0     2143 2023-04-10 00:27:52.000000 PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/eg2.py
--rw-rw-rw-   0        0        0     1648 2023-04-07 09:39:03.000000 PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/eg3.py
--rw-rw-rw-   0        0        0     2372 2023-04-07 09:54:15.000000 PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/eg4.py
--rw-rw-rw-   0        0        0     2111 2023-04-10 03:46:57.000000 PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/test.py
--rw-rw-rw-   0        0        0     2457 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_barset.py
--rw-rw-rw-   0        0        0     1648 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_circularBar.py
--rw-rw-rw-   0        0        0     1723 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_colorPalette.py
--rw-rw-rw-   0        0        0     1042 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_comboBox.py
--rw-rw-rw-   0        0        0      289 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_dumpStructure.py
--rw-rw-rw-   0        0        0      830 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_dynamicTLine.py
--rw-rw-rw-   0        0        0     1315 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_flowLayot.py
--rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_gradientBar.py
--rw-rw-rw-   0        0        0     1865 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_listWidget.py
--rw-rw-rw-   0        0        0     1398 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_loadbar.py
--rw-rw-rw-   0        0        0     2498 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_no_border.py
--rw-rw-rw-   0        0        0     1365 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_no_border_pullOver.py
--rw-rw-rw-   0        0        0     1022 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_pullOverWidget.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.374434 PyQtGuiLib-2.7.18.11/tests/test_qssFile/
--rw-rw-rw-   0        0        0      107 2023-03-29 06:12:59.000000 PyQtGuiLib-2.7.18.11/tests/test_qssFile/__init__.py
--rw-rw-rw-   0        0        0      584 2023-04-04 06:18:57.000000 PyQtGuiLib-2.7.18.11/tests/test_qssFile/test.py
--rw-rw-rw-   0        0        0     1444 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_rollWidget.py
--rw-rw-rw-   0        0        0     1666 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_slider.py
--rw-rw-rw-   0        0        0     1721 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_statusBar.py
--rw-rw-rw-   0        0        0     1014 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_styles.py
--rw-rw-rw-   0        0        0     1122 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_switchButton.py
--rw-rw-rw-   0        0        0     1138 2023-03-10 08:33:39.000000 PyQtGuiLib-2.7.18.11/tests/test_template.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.377426 PyQtGuiLib-2.7.18.11/tests/test_templateWindow/
--rw-rw-rw-   0        0        0      107 2023-04-11 04:44:35.000000 PyQtGuiLib-2.7.18.11/tests/test_templateWindow/__init__.py
--rw-rw-rw-   0        0        0     2048 2023-04-11 05:48:48.000000 PyQtGuiLib-2.7.18.11/tests/test_templateWindow/test_listTemplateWindow.py
--rw-rw-rw-   0        0        0     1356 2023-03-13 08:03:45.000000 PyQtGuiLib-2.7.18.11/tests/test_toolList.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.379420 PyQtGuiLib-2.7.18.11/tests/test_uic/
--rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_uic/__init__.py
--rw-rw-rw-   0        0        0      377 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_uic/test_uic.py
--rw-rw-rw-   0        0        0     1547 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_waterBar.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.915737 PyQtGuiLib-2.7.20.11/
+-rw-rw-rw-   0        0        0     1091 2022-12-10 10:29:38.000000 PyQtGuiLib-2.7.20.11/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.636746 PyQtGuiLib-2.7.20.11/Log/
+-rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/Log/__init__.py
+-rw-rw-rw-   0        0        0     9740 2023-04-21 06:44:31.000000 PyQtGuiLib-2.7.20.11/Log/developmentLog.py
+-rw-rw-rw-   0        0        0    17825 2023-04-21 06:54:09.915737 PyQtGuiLib-2.7.20.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.639739 PyQtGuiLib-2.7.20.11/PyQtGuiLib/
+-rw-rw-rw-   0        0        0      108 2023-04-15 02:34:22.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.651710 PyQtGuiLib-2.7.20.11/PyQtGuiLib/animation/
+-rw-rw-rw-   0        0        0     6805 2023-04-20 03:22:30.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/animation/PropertyAnimation.py
+-rw-rw-rw-   0        0        0      208 2023-04-20 09:47:43.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/animation/__init__.py
+-rw-rw-rw-   0        0        0     6552 2023-04-20 09:28:51.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/animation/animation.py
+-rw-rw-rw-   0        0        0     2465 2023-04-20 09:28:51.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/animation/test_animation.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.665668 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/
+-rw-rw-rw-   0        0        0      602 2023-04-21 06:44:31.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/__init__.py
+-rw-rw-rw-   0        0        0     5953 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/bubbleWidget.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.671681 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/comboBox/
+-rw-rw-rw-   0        0        0      218 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/comboBox/__init__.py
+-rw-rw-rw-   0        0        0     4854 2023-02-13 10:30:41.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/comboBox/combBox.py
+-rw-rw-rw-   0        0        0     8171 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/comboBox/comboBox.py
+-rw-rw-rw-   0        0        0     4107 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/comboBox/comboBox2.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.673651 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/drawers/
+-rw-rw-rw-   0        0        0      107 2023-04-20 09:35:26.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/drawers/__init__.py
+-rw-rw-rw-   0        0        0     3192 2023-04-21 06:46:15.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/drawers/drawer.py
+-rw-rw-rw-   0        0        0     4203 2023-04-17 07:41:59.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/expansionBar.py
+-rw-rw-rw-   0        0        0     3886 2023-02-08 01:08:13.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/flowLayout.py
+-rw-rw-rw-   0        0        0     2583 2023-04-17 06:05:25.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/imageButton.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.675642 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/lineedit/
+-rw-rw-rw-   0        0        0      170 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/lineedit/__init__.py
+-rw-rw-rw-   0        0        0     3967 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/lineedit/dynamicTLine.py
+-rw-rw-rw-   0        0        0     5090 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/listWidget.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.682647 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/logBrowser/
+-rw-rw-rw-   0        0        0      107 2023-03-27 09:33:07.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/logBrowser/__init__.py
+-rw-rw-rw-   0        0        0     1823 2023-03-31 09:04:34.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/logBrowser/loadLogTh.py
+-rw-rw-rw-   0        0        0     5112 2023-04-03 02:45:06.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/logBrowser/logBrowser.py
+-rw-rw-rw-   0        0        0      554 2023-03-31 09:29:33.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/logBrowser/logSizeTh.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.684618 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/notice/
+-rw-rw-rw-   0        0        0        0 2023-02-08 01:08:13.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/notice/__init__.py
+-rw-rw-rw-   0        0        0     4822 2023-02-10 11:02:17.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/notice/notice.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.688632 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/palettes/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/palettes/__init__.py
+-rw-rw-rw-   0        0        0     9818 2023-02-18 01:06:47.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/palettes/colorHsv.py
+-rw-rw-rw-   0        0        0     6728 2023-02-18 01:06:47.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/palettes/paletteFrame.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.696596 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/
+-rw-rw-rw-   0        0        0      325 2023-04-13 08:34:31.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/__init__.py
+-rw-rw-rw-   0        0        0     5602 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/circularBar.py
+-rw-rw-rw-   0        0        0     6401 2023-04-13 08:34:31.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/circularProgressBar.py
+-rw-rw-rw-   0        0        0     3943 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/gradientBar.py
+-rw-rw-rw-   0        0        0     4365 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/loadBar.py
+-rw-rw-rw-   0        0        0     6734 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/waterBar.py
+-rw-rw-rw-   0        0        0     5092 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/pullOver.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.698611 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/resolver/
+-rw-rw-rw-   0        0        0       59 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/resolver/__init__.py
+-rw-rw-rw-   0        0        0      674 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/resolver/controls.py
+-rw-rw-rw-   0        0        0     7628 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/rollWidget.py
+-rw-rw-rw-   0        0        0    10547 2023-04-15 10:18:10.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/slideShow.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.700599 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/slider/
+-rw-rw-rw-   0        0        0        0 2023-02-14 00:37:29.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/slider/__init__.py
+-rw-rw-rw-   0        0        0     8596 2023-04-13 07:56:58.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/slider/slider.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.702580 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/switchButtons/
+-rw-rw-rw-   0        0        0       63 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/switchButtons/__init__.py
+-rw-rw-rw-   0        0        0     4993 2023-02-23 01:29:46.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/switchButtons/swButton.py
+-rw-rw-rw-   0        0        0     2743 2023-03-06 05:54:08.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/toolBox.py
+-rw-rw-rw-   0        0        0     5588 2023-03-14 01:24:55.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/toolList.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.710572 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/
+-rw-rw-rw-   0        0        0    11338 2023-04-13 05:09:14.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/WidgetABC.py
+-rw-rw-rw-   0        0        0      260 2023-02-09 10:20:35.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3995 2023-02-10 07:29:38.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/borderlessMainWindow.py
+-rw-rw-rw-   0        0        0      303 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/borderlessWidget.py
+-rw-rw-rw-   0        0        0     4935 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/statusBar.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.714575 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/tets/
+-rw-rw-rw-   0        0        0      375 2023-02-27 10:18:30.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/tets/1.py
+-rw-rw-rw-   0        0        0     3504 2023-02-27 00:36:50.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/tets/2.py
+-rw-rw-rw-   0        0        0        0 2023-02-24 00:57:42.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/tets/__init__.py
+-rw-rw-rw-   0        0        0    17840 2023-02-10 03:56:26.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/titleBar.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.720546 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.731493 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/__init__.py
+-rw-rw-rw-   0        0        0     5130 2023-04-13 07:48:56.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qt.py
+-rw-rw-rw-   0        0        0     2729 2023-04-13 07:53:03.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qtCore.py
+-rw-rw-rw-   0        0        0     3019 2023-04-13 07:51:53.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qtGui.py
+-rw-rw-rw-   0        0        0      509 2023-02-09 08:33:46.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qtSip.py
+-rw-rw-rw-   0        0        0      505 2023-02-13 08:07:57.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qtUic.py
+-rw-rw-rw-   0        0        0     6996 2023-02-18 02:58:53.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qtWidgets.py
+-rw-rw-rw-   0        0        0      632 2023-02-13 08:14:52.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/__init__.py
+-rw-rw-rw-   0        0        0     6404 2023-04-13 07:50:28.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/customStyle.py
+-rw-rw-rw-   0        0        0      262 2023-02-10 01:34:45.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/error.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.733512 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/py/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/py/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/py/common.py
+-rw-rw-rw-   0        0        0     3684 2023-04-13 08:06:22.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/utility.py
+-rw-rw-rw-   0        0        0      396 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/versions.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.735510 PyQtGuiLib-2.7.20.11/PyQtGuiLib/layoutDeformation/
+-rw-rw-rw-   0        0        0      106 2023-03-04 03:38:59.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/layoutDeformation/__init__.py
+-rw-rw-rw-   0        0        0     4425 2023-03-07 08:03:39.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/layoutDeformation/test.py
+-rw-rw-rw-   0        0        0     2452 2023-04-17 03:52:57.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/listTree.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.738475 PyQtGuiLib-2.7.20.11/PyQtGuiLib/particle/
+-rw-rw-rw-   0        0        0      107 2023-04-20 06:55:28.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/particle/__init__.py
+-rw-rw-rw-   0        0        0     2729 2023-04-20 09:11:21.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/particle/particle.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.743485 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/
+-rw-rw-rw-   0        0        0      362 2023-04-21 06:50:57.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.749445 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/builtStyleDesigner/
+-rw-rw-rw-   0        0        0      105 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/builtStyleDesigner/__init__.py
+-rw-rw-rw-   0        0        0     7168 2023-02-24 00:57:42.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py
+-rw-rw-rw-   0        0        0     5062 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py
+-rw-rw-rw-   0        0        0     1237 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.752460 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/buttons/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/buttons/__init__.py
+-rw-rw-rw-   0        0        0      620 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/buttons/buttonStyle.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.758441 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/
+-rw-rw-rw-   0        0        0      106 2023-02-20 02:36:19.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/__init__.py
+-rw-rw-rw-   0        0        0    26952 2023-02-23 01:15:37.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/component.py
+-rw-rw-rw-   0        0        0     8822 2023-03-13 01:50:58.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/controlType.py
+-rw-rw-rw-   0        0        0    11557 2023-02-23 09:01:24.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/styleLinker.py
+-rw-rw-rw-   0        0        0     1444 2023-02-22 03:17:40.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/styleLinkerUi.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.762424 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/
+-rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.766423 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/drak/
+-rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/drak/__init__.py
+-rw-rw-rw-   0        0        0      187 2023-03-29 08:26:42.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/drak/config.py
+-rw-rw-rw-   0        0        0    11537 2023-03-30 09:13:08.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/drak/qssDrak.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.771398 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/image/
+-rw-rw-rw-   0        0        0      107 2023-03-29 03:26:49.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/image/__init__.py
+-rw-rw-rw-   0        0        0    29060 2023-03-30 10:20:11.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/image/image_rc.py
+-rw-rw-rw-   0        0        0      300 2023-03-30 10:19:06.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/image/qssFile.py
+-rw-rw-rw-   0        0        0    20518 2023-03-30 10:20:35.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/qssFile.py
+-rw-rw-rw-   0        0        0     6221 2023-04-20 09:24:50.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/test.py
+-rw-rw-rw-   0        0        0    10615 2023-02-09 08:32:36.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/skinABC.py
+-rw-rw-rw-   0        0        0     8581 2023-04-13 08:00:22.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/styleAnalysis.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.773381 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/superPainter/
+-rw-rw-rw-   0        0        0      107 2023-03-18 07:49:47.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/superPainter/__init__.py
+-rw-rw-rw-   0        0        0    13068 2023-04-21 01:53:12.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/superPainter/superPainter.py
+-rw-rw-rw-   0        0        0    17854 2023-03-10 06:22:00.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/superPainter.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.775392 PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.777387 PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/UI/
+-rw-rw-rw-   0        0        0      193 2023-04-11 03:59:36.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/UI/__init__.py
+-rw-rw-rw-   0        0        0     5539 2023-04-13 05:40:13.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.784375 PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/Window/
+-rw-rw-rw-   0        0        0      107 2023-04-10 09:41:12.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/Window/__init__.py
+-rw-rw-rw-   0        0        0     9497 2023-04-15 10:09:10.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py
+-rw-rw-rw-   0        0        0      189 2023-04-11 04:44:35.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.646721 PyQtGuiLib-2.7.20.11/PyQtGuiLib.egg-info/
+-rw-rw-rw-   0        0        0    17825 2023-04-21 06:54:09.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7127 2023-04-21 06:54:09.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 06:54:09.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-21 06:54:09.000000 PyQtGuiLib-2.7.20.11/PyQtGuiLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17395 2023-03-27 01:38:52.000000 PyQtGuiLib-2.7.20.11/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.794348 PyQtGuiLib-2.7.20.11/abandonCase/
+-rw-rw-rw-   0        0        0      108 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.800333 PyQtGuiLib-2.7.20.11/abandonCase/acrylic/
+-rw-rw-rw-   0        0        0       37 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/acrylic/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/acrylic/acrylicWidget.py
+-rw-rw-rw-   0        0        0     1550 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/acrylic/cstruct.py
+-rw-rw-rw-   0        0        0     2183 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/acrylic/windowEffect.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.807314 PyQtGuiLib-2.7.20.11/abandonCase/animation/
+-rw-rw-rw-   0        0        0      107 2023-04-20 09:24:50.000000 PyQtGuiLib-2.7.20.11/abandonCase/animation/__init__.py
+-rw-rw-rw-   0        0        0    21249 2023-04-20 09:24:50.000000 PyQtGuiLib-2.7.20.11/abandonCase/animation/animation.py
+-rw-rw-rw-   0        0        0     2792 2023-03-28 09:06:54.000000 PyQtGuiLib-2.7.20.11/abandonCase/animation/animationDrawType.py
+-rw-rw-rw-   0        0        0    11526 2023-04-20 09:24:50.000000 PyQtGuiLib-2.7.20.11/abandonCase/animation/animationFactory.py
+-rw-rw-rw-   0        0        0     1636 2023-03-20 04:02:29.000000 PyQtGuiLib-2.7.20.11/abandonCase/animation/animationLayout.py
+-rw-rw-rw-   0        0        0     2292 2023-03-15 01:17:54.000000 PyQtGuiLib-2.7.20.11/abandonCase/animation/customAniTest.py
+-rw-rw-rw-   0        0        0     9981 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/bubbleWidget.py
+-rw-rw-rw-   0        0        0     3620 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/bubbleWidget_case.py
+-rw-rw-rw-   0        0        0     1411 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/nodeBar.py
+-rw-rw-rw-   0        0        0     9873 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/slideShow.py
+-rw-rw-rw-   0        0        0     7801 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/slideShow2.py
+-rw-rw-rw-   0        0        0        0 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/spaceWidget.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.818264 PyQtGuiLib-2.7.20.11/abandonCase/widgets/
+-rw-rw-rw-   0        0        0      110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1389 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessFrame.py
+-rw-rw-rw-   0        0        0     1962 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessMainWindow.py
+-rw-rw-rw-   0        0        0     1441 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessStackedWidget.py
+-rw-rw-rw-   0        0        0     1402 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessWidget.py
+-rw-rw-rw-   0        0        0    10095 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessWidgetABC.py
+-rw-rw-rw-   0        0        0     5034 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/widgets/statusBar.py
+-rw-rw-rw-   0        0        0    17577 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/abandonCase/widgets/titleBar.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.821252 PyQtGuiLib-2.7.20.11/auxiliaryMeans/
+-rw-rw-rw-   0        0        0        0 2023-04-17 01:54:33.000000 PyQtGuiLib-2.7.20.11/auxiliaryMeans/__init__.py
+-rw-rw-rw-   0        0        0     5067 2023-04-17 02:06:33.000000 PyQtGuiLib-2.7.20.11/auxiliaryMeans/toolNewProject.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 06:54:09.915737 PyQtGuiLib-2.7.20.11/setup.cfg
+-rw-rw-rw-   0        0        0      744 2023-04-21 06:52:57.000000 PyQtGuiLib-2.7.20.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.859177 PyQtGuiLib-2.7.20.11/tests/
+-rw-rw-rw-   0        0        0      107 2023-03-06 03:09:41.000000 PyQtGuiLib-2.7.20.11/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.877131 PyQtGuiLib-2.7.20.11/tests/test_Animation/
+-rw-rw-rw-   0        0        0     1994 2023-04-05 10:25:59.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/1.py
+-rw-rw-rw-   0        0        0      606 2023-03-15 09:52:36.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/__init__.py
+-rw-rw-rw-   0        0        0     3180 2023-04-20 09:24:50.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/eg1.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.881121 PyQtGuiLib-2.7.20.11/tests/test_Animation/test_ani/
+-rw-rw-rw-   0        0        0     1589 2023-04-20 01:28:51.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/test_ani/1.py
+-rw-rw-rw-   0        0        0      107 2023-03-27 05:53:58.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/test_ani/__init__.py
+-rw-rw-rw-   0        0        0     1654 2023-03-28 08:45:42.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_1.py
+-rw-rw-rw-   0        0        0     1824 2023-03-28 08:48:45.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_10.py
+-rw-rw-rw-   0        0        0     1305 2023-03-28 08:45:46.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_2.py
+-rw-rw-rw-   0        0        0     2011 2023-03-28 08:45:51.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_3.py
+-rw-rw-rw-   0        0        0     1276 2023-03-28 08:45:56.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_4.py
+-rw-rw-rw-   0        0        0     1851 2023-03-28 08:46:24.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_5.py
+-rw-rw-rw-   0        0        0     1759 2023-03-28 08:46:54.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_6.py
+-rw-rw-rw-   0        0        0     2206 2023-03-28 08:47:16.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_7.py
+-rw-rw-rw-   0        0        0     2000 2023-03-28 08:47:46.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_8.py
+-rw-rw-rw-   0        0        0     1712 2023-03-28 08:48:15.000000 PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_9.py
+-rw-rw-rw-   0        0        0     1541 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_BubbleWidget.py
+-rw-rw-rw-   0        0        0     2738 2023-04-13 08:35:22.000000 PyQtGuiLib-2.7.20.11/tests/test_CircularProgressBar.py
+-rw-rw-rw-   0        0        0     1596 2023-04-19 07:50:47.000000 PyQtGuiLib-2.7.20.11/tests/test_Notice.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.891065 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/
+-rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-04-06 02:24:28.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg1.py
+-rw-rw-rw-   0        0        0     2306 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg2.py
+-rw-rw-rw-   0        0        0     1891 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg3.py
+-rw-rw-rw-   0        0        0     2110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg4.py
+-rw-rw-rw-   0        0        0     2519 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg5.py
+-rw-rw-rw-   0        0        0     1881 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg6.py
+-rw-rw-rw-   0        0        0     2617 2023-03-22 05:45:33.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg7.py
+-rw-rw-rw-   0        0        0     2042 2023-04-06 03:41:23.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/test.py
+-rw-rw-rw-   0        0        0     2275 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis.py
+-rw-rw-rw-   0        0        0     2605 2023-04-13 09:27:46.000000 PyQtGuiLib-2.7.20.11/tests/test_SlideShow.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.896791 PyQtGuiLib-2.7.20.11/tests/test_StyleLinker/
+-rw-rw-rw-   0        0        0        0 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_StyleLinker/__init__.py
+-rw-rw-rw-   0        0        0      949 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_StyleLinker/eg1_QPushButton.py
+-rw-rw-rw-   0        0        0      807 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_StyleLinker/eg2_QLabel.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.906780 PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/
+-rw-rw-rw-   0        0        0      871 2023-04-20 09:50:12.000000 PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/1.py
+-rw-rw-rw-   0        0        0      106 2023-04-07 09:06:55.000000 PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/__init__.py
+-rw-rw-rw-   0        0        0     1568 2023-04-07 09:19:44.000000 PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/eg1.py
+-rw-rw-rw-   0        0        0     2143 2023-04-10 00:27:52.000000 PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/eg2.py
+-rw-rw-rw-   0        0        0     1648 2023-04-07 09:39:03.000000 PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/eg3.py
+-rw-rw-rw-   0        0        0     3527 2023-04-19 03:20:23.000000 PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/eg4.py
+-rw-rw-rw-   0        0        0     2538 2023-04-21 02:10:44.000000 PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/test.py
+-rw-rw-rw-   0        0        0     2465 2023-04-13 01:50:22.000000 PyQtGuiLib-2.7.20.11/tests/test_barset.py
+-rw-rw-rw-   0        0        0     1648 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_circularBar.py
+-rw-rw-rw-   0        0        0     1723 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_colorPalette.py
+-rw-rw-rw-   0        0        0     1042 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_comboBox.py
+-rw-rw-rw-   0        0        0     1161 2023-04-21 06:51:11.000000 PyQtGuiLib-2.7.20.11/tests/test_drawer.py
+-rw-rw-rw-   0        0        0      289 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_dumpStructure.py
+-rw-rw-rw-   0        0        0      830 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_dynamicTLine.py
+-rw-rw-rw-   0        0        0      613 2023-04-17 06:35:12.000000 PyQtGuiLib-2.7.20.11/tests/test_expansionBar.py
+-rw-rw-rw-   0        0        0     1315 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_flowLayot.py
+-rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_gradientBar.py
+-rw-rw-rw-   0        0        0      903 2023-04-17 05:57:17.000000 PyQtGuiLib-2.7.20.11/tests/test_imageButton.py
+-rw-rw-rw-   0        0        0     1865 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_listWidget.py
+-rw-rw-rw-   0        0        0     1398 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_loadbar.py
+-rw-rw-rw-   0        0        0     2498 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_no_border.py
+-rw-rw-rw-   0        0        0     1365 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_no_border_pullOver.py
+-rw-rw-rw-   0        0        0     1022 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_pullOverWidget.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.908780 PyQtGuiLib-2.7.20.11/tests/test_qssFile/
+-rw-rw-rw-   0        0        0      107 2023-03-29 06:12:59.000000 PyQtGuiLib-2.7.20.11/tests/test_qssFile/__init__.py
+-rw-rw-rw-   0        0        0      584 2023-04-04 06:18:57.000000 PyQtGuiLib-2.7.20.11/tests/test_qssFile/test.py
+-rw-rw-rw-   0        0        0     1444 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_rollWidget.py
+-rw-rw-rw-   0        0        0     1666 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_slider.py
+-rw-rw-rw-   0        0        0     1778 2023-04-13 01:45:35.000000 PyQtGuiLib-2.7.20.11/tests/test_statusBar.py
+-rw-rw-rw-   0        0        0     1014 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_styles.py
+-rw-rw-rw-   0        0        0     1122 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_switchButton.py
+-rw-rw-rw-   0        0        0      543 2023-04-17 01:43:36.000000 PyQtGuiLib-2.7.20.11/tests/test_template.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.911750 PyQtGuiLib-2.7.20.11/tests/test_templateWindow/
+-rw-rw-rw-   0        0        0      107 2023-04-11 04:44:35.000000 PyQtGuiLib-2.7.20.11/tests/test_templateWindow/__init__.py
+-rw-rw-rw-   0        0        0     2718 2023-04-13 10:00:15.000000 PyQtGuiLib-2.7.20.11/tests/test_templateWindow/test_listTemplateWindow.py
+-rw-rw-rw-   0        0        0     1356 2023-03-13 08:03:45.000000 PyQtGuiLib-2.7.20.11/tests/test_toolList.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:54:09.913743 PyQtGuiLib-2.7.20.11/tests/test_uic/
+-rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_uic/__init__.py
+-rw-rw-rw-   0        0        0      377 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_uic/test_uic.py
+-rw-rw-rw-   0        0        0     1547 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.20.11/tests/test_waterBar.py
```

### Comparing `PyQtGuiLib-2.7.18.11/LICENSE.txt` & `PyQtGuiLib-2.7.20.11/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/Log/developmentLog.py` & `PyQtGuiLib-2.7.20.11/Log/developmentLog.py`

 * *Files 8% similar despite different names*

```diff
@@ -158,14 +158,21 @@
     - Animation 动画框架 已经快接近完成,目前大部分功能已经可用
     - 修改QSS解析器的已知BUG,并且在多线程时,是安全的
     - 新增 SuperPainter 超级画师类
         - 导入方法 from PyQtGuiLib.styles import SuperPainter
         - 教学案例在test\test_SuperPainter 目录下
 2023.4.7 - 2023.4.11
     - 更新模板窗口 ListTemplateWindow
+2023.4.13 
+     感谢! PyQt5学习爱好群-(讨厌自己) 贡献 CircularProgressBar 进度条模块
+     导入方式 from PyQtGuiLib.core.progressBar import CircularProgressBar
+2023.4.20
+    - 新增 抽屉控件(Drawer) -- 编写中
+2023.4.21 
+    -抽屉控件(Drawer)完成
 '''
 
 
 # -------------------------------
 '''
     暂时搁浅的任务
 1.新无边框窗口主窗口,(还没有设计完成,暂时先放下 2023.1.31)
```

### Comparing `PyQtGuiLib-2.7.18.11/PKG-INFO` & `PyQtGuiLib-2.7.20.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtGuiLib
-Version: 2.7.18.11
+Version: 2.7.20.11
 Summary: Python version of the qt component library.
 Home-page: https://github.com/LX-sys/PyQtGuiLib
 Author: LX
 Author-email: lx984608061@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/animation.py` & `PyQtGuiLib-2.7.20.11/abandonCase/animation/animation.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 from typing import TypeVar,List
 from collections.abc import Callable
 import copy
 '''
     重构动画框架
     Animation 仅创建,管理,播放动画
 '''
-import pprint
-from PyQtGuiLib.animation.animationFactory import AnimationFactory,PropertyAnimation
-from PyQtGuiLib.animation.animationDrawType import AniNumber,AniNumbers,AniColor,AniRect,AniShadow,AniPoint
+from abandonCase.animation.animationFactory import AnimationFactory,PropertyAnimation
+from abandonCase.animation.animationDrawType import AniNumber,AniNumbers,AniColor,AniRect,AniShadow,AniPoint
 
 AniMode = int
 ObjMode = str
 AniStartType = TypeVar("AniStartType",AniNumber,AniNumbers,AniColor,AniRect)
 AniEndType = TypeVar("AniEndType",list,QColor,QRect)
 AnimationModeType = TypeVar("AnimationModeType",QParallelAnimationGroup,QSequentialAnimationGroup)
```

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/animationDrawType.py` & `PyQtGuiLib-2.7.20.11/abandonCase/animation/animationDrawType.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/animationFactory.py` & `PyQtGuiLib-2.7.20.11/abandonCase/animation/animationFactory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import re
 import typing
 from PyQtGuiLib.header import (
     QPropertyAnimation,
     QObject,
     QColor,
-    QRect,
-    QPoint,
-    QSize,
-    pyqtProperty,
     Signal,
-    QGraphicsDropShadowEffect,
-    QGraphicsBlurEffect
+    QGraphicsDropShadowEffect
 )
 from PyQtGuiLib.styles import QssStyleAnalysis
-from PyQtGuiLib.animation.animationDrawType import AniNumber
+from abandonCase.animation.animationDrawType import AniNumber
 '''
     QPropertyAnimation: you're trying to animate a non-existing property value of your QObject
     该警告出现mac下,部分win可能也会出现,可以忽略该警告
 '''
 
 
 # 公用动画基类
```

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/animationLayout.py` & `PyQtGuiLib-2.7.20.11/abandonCase/animation/animationLayout.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/customAniTest.py` & `PyQtGuiLib-2.7.20.11/abandonCase/animation/customAniTest.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/lmlmAni.py` & `PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_8.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,124 +1,71 @@
 # -*- coding:utf-8 -*-
-# @time:2022/12/1211:45
+# @time:2023/3/239:06
 # @author:LX
-# @file:lmlm.py
+# @file:tutorial_8.py
 # @software:PyCharm
-
-'''
-    若隐若现
-'''
 from PyQtGuiLib.header import (
-    sys,
     QApplication,
-    QPropertyAnimation,
+    PYQT_VERSIONS,
+    sys,
     QWidget,
     QPushButton,
-    PYQT_VERSIONS,
-    QGraphicsOpacityEffect,
-    QThread,
-    Signal
+    QColor,
+    QLabel
 )
 
-# 时间
-class DurationTimeThread(QThread):
-    finished = Signal()
-
-    def __init__(self,lmlm:QGraphicsOpacityEffect,*args,**kwargs):
-        super().__init__(*args,**kwargs)
-        self.lmlm = lmlm
-        self.mode = "show"
-        self.dur_time = 3
-
-    def setMode(self,mode:str):
-        self.mode = mode
-
-    def setDurationTime(self, seconds: int):
-        self.dur_time = seconds
-
-    def run(self):
-        n = round((1 / self.dur_time) / 10, 2)
-        opacity_v = 0
-        if self.mode == "hide":
-            opacity_v = 1
-            n = -n
-
-        while self.dur_time:
-            self.lmlm.setOpacity(opacity_v)
-            self.msleep(100)
-            opacity_v += n
-            if opacity_v >= 1 or opacity_v <= 0:
-                break
-        self.finished.emit()
-
-
-# 若隐若现 动画
-class LmLmAnimation(QGraphicsOpacityEffect):
-    finished = Signal()  # 完成信号
-
-    Show = "show"
-    Hide = "hide"
-
-    def __init__(self,*args,**kwargs):
-        super().__init__(*args,**kwargs)
-        self.dtt = DurationTimeThread(self)
-
-    def setMode(self,mode:str="show"):
-        self.dtt.setMode(mode)
-
-    # 这样写是为了,统一api的用法
-    def setTargetObject(self,widget:QWidget):
-        widget.setGraphicsEffect(self)
-
-    def setDuration(self,msecs:int):
-        self.dtt.setDurationTime(msecs//1000)
-
-    def start(self):
-        self.dtt.start()
-        self.dtt.finished.connect(self.finished)
-
+# 动画框架
+from PyQtGuiLib.animation import Animation
 
 
 class Test(QWidget):
-    def __init__(self):
-        super(Test, self).__init__()
-        self.resize(800,600)
-
-        self.btn = QPushButton("测试",self)
-        self.btn.resize(150,70)
-        self.btn.move(100,100)
-
-        self.op =LmLmAnimation()
-        self.op.setMode(LmLmAnimation.Hide)
-        self.op.setTargetObject(self.btn)
-        self.op.setDuration(5000)
-        self.op.start()
-        self.op.finished.connect(lambda :print("Dasdasd"))
-
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.resize(600, 600)
+        '''
+             Animation 动画框架 案例八,QSS属性动画特性二,动态QSS属性动画
+             背景和前景色动画
 
+             注意:使用这一类动画时,你的控件必须有qss样式
         '''
-        geometry 位置和大小
-        pos 位置
-        size 大小
-        windowOpacity 透明度
-        alpha  自定义
+        self.btn = QPushButton("按钮", self)
+        self.btn.move(50, 50)
+        self.btn.resize(100, 60)
+        # 写一个简单,标准的样式,按钮添加一个背景颜色
         '''
-        # self.ani = QPropertyAnimation()
-        # self.ani.setTargetObject(self.btn)
-        # self.ani.setPropertyName(b"windowOpacity")
-        # self.ani.setDuration(10000)
-        # self.ani.setStartValue(1)
-        # self.ani.setEndValue(0.3)
-        # self.ani.setStartValue(QRect(150, 30, 100, 100))
-        # self.ani.setEndValue(QRect(150, 30, 200, 200))
-        # self.ani.start()
+            在上一个案例中,我们知道这个简单标准的QSS动画,
+            那么我们去掉QSS中 background-color 这个属性在运行
+        '''
+        self.btn.setStyleSheet('''
+        QPushButton{
+            color:rgb(255,0,0);
+        }
+        ''')
+
+        # 实例化动画类
+        self.ani = Animation(self)
+        # 设置动画时长
+        self.ani.setDuration(3000)  # 3秒
+
+        # 添加一个QSS属性动画
+        self.ani.addAni({
+            "targetObj": self.btn,
+            "propertyName": b"background-color",
+            # "sv":"this",  # 注意: 在对原本控件中没有样式经行动画时,是不允许使用 "this" 指向自己的
+            "sv": QColor(0,255,0),
+            "ev": QColor(200, 200, 100),
+            "selector": "QPushButton"
+        })
+        # 开始动画
+        self.ani.start()
 
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
+
     win = Test()
     win.show()
 
-    if PYQT_VERSIONS == "PyQt6":
+    if PYQT_VERSIONS in ["PyQt6", "PySide6"]:
         sys.exit(app.exec())
     else:
         sys.exit(app.exec_())
```

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/__init__.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,8 +3,9 @@
 from PyQtGuiLib.core.slideShow import SlideShow
 from PyQtGuiLib.core.flowLayout import FlowLayout
 from PyQtGuiLib.core.listWidget import ListWidget
 from PyQtGuiLib.core.rollWidget import RollWidget
 from PyQtGuiLib.core.palettes.paletteFrame import PaletteFrame
 from PyQtGuiLib.core.notice.notice import Notice,Notices
 from PyQtGuiLib.core.slider.slider import Slider
-from PyQtGuiLib.core.toolList import ToolListWidget,ToolListItem
+from PyQtGuiLib.core.toolList import ToolListWidget,ToolListItem
+from PyQtGuiLib.core.drawers.drawer import DrawerItem,Drawer
```

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/bubbleWidget.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/bubbleWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/comboBox/combBox.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/comboBox/combBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/comboBox/comboBox.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/comboBox/comboBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/comboBox/comboBox2.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/comboBox/comboBox2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/flowLayout.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/flowLayout.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/lineedit/dynamicTLine.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/lineedit/dynamicTLine.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/listWidget.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/listWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/logBrowser/loadLogTh.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/logBrowser/loadLogTh.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/logBrowser/logBrowser.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/logBrowser/logBrowser.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/logBrowser/logSizeTh.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/logBrowser/logSizeTh.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/notice/notice.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/notice/notice.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/palettes/colorHsv.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/palettes/colorHsv.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/palettes/paletteFrame.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/palettes/paletteFrame.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/circularBar.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/circularBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/gradientBar.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/gradientBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/loadBar.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/loadBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/waterBar.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/progressBar/waterBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/pullOver.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/pullOver.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/resolver/controls.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/resolver/controls.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/rollWidget.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/rollWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/slideShow.py` & `PyQtGuiLib-2.7.20.11/abandonCase/slideShow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,219 @@
 # -*- coding:utf-8 -*-
-# @time:2023/1/10 12:41
+# @time:2022/12/2317:54
 # @author:LX
 # @file:SlideShow.py
 # @software:PyCharm
-
 from PyQtGuiLib.header import (
+    PYQT_VERSIONS,
+    QApplication,
+    sys,
     QWidget,
+    QResizeEvent,
     QPushButton,
     QPoint,
+    QSize,
     QPropertyAnimation,
-    Signal,
-    QSize
+    Signal
 )
 
+
+
 '''
-    组件轮播 2023.3.7 当前控件的所有功能均处于稳定状态
-    SlideShow 独立版本 3.0
+
+    轮播图功能
+        风格: 扁平
 '''
 class SlideShow(QWidget):
     # 切换窗口事件
-    changeWidget = Signal(QWidget)
+    switchWidgeted = Signal(int)
+
+    # 扁平 风格
+    FlatMode = "flat"  # 经典
 
     # 动画的方向模式
     Ani_Left = "left"
     Ani_Right = "right"
     Ani_Down = "down"
     Ani_Up = "up"
 
+
+    # 动画
+    Translation = "translation"  # 平移
+
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
         self.resize(700, 300)
-        #
-        self.widgets = []
 
-        self.animation_time = 800 # 毫秒
+        self.show_mode = SlideShow.FlatMode # 展示模式
+        self.animation_mode = SlideShow.Translation  # 动画模式
 
-        # 动画运行方向,当前动作
-        self.ani_direction = (SlideShow.Ani_Left, SlideShow.Ani_Right)
+        self.animation_time = 300 # 毫秒
+
+        self.index = [-1,0]  # 索引
+        self.cu_index = self.index[1]  # 当前索引
 
         # 设置自动轮播,自动轮播的方向
         self.is_auto_slide = False
-        self.auto_ani_direction = "R"
-
-        # 窗口索引
-        self.index = 0
-
-        # 指向两个当前窗口
-        self.cursor_widget_p = None # type:QWidget
-        self.cursor_widget_p2 = None # type:QWidget
-
-        # 创建两侧按钮
-        self.createButtons()
-
-    def setDuration(self,p_int):
-        self.animation_time = p_int
-
-    # 设置自动轮播
-    def setAutoSlideShow(self,b:bool,interval=1500,direction_:str="R"):
-        if direction_ not in ["R","L"]:
-            raise TypeError("Parameter error, Support only 'R' or 'L' !")
+        self.auto_direction = SlideShow.Ani_Right
 
-        if interval <= self.animation_time:
-            raise ValueError("The interval between auto wheel casting must be longer than the animation time!")
-
-        self.is_auto_slide = b
-        self.startTimer(interval)
-        self.auto_ani_direction = direction_
-
-    # 左上方向
-    def lu_direction(self) -> str:
-        return self.ani_direction[0]
-
-    # 右下方向
-    def rd_direction(self) -> str:
-        return self.ani_direction[1]
-
-    # 创建两侧按钮
-    def createButtons(self):
         # 左右按钮
         self.Ani_Left_btn = QPushButton("左",self)
         self.Ani_Right_btn = QPushButton("右",self)
         self.Ani_Left_btn.setObjectName("Ani_Left_btn")
         self.Ani_Right_btn.setObjectName("Ani_Right_btn")
         self.Ani_Left_btn.resize(50,50)
         self.Ani_Right_btn.resize(50,50)
-        self.Ani_Left_btn.clicked.connect(lambda :self.moveWidget("L"))
-        self.Ani_Right_btn.clicked.connect(lambda :self.moveWidget("R"))
+        self.Ani_Left_btn.clicked.connect(lambda :self.roll_event(SlideShow.Ani_Left))
+        self.Ani_Right_btn.clicked.connect(lambda :self.roll_event(SlideShow.Ani_Right))
         self.btnStyle()
-        self.btnPos()
+
+        # 窗口
+        self.widgets = []  # 所有已经添加的窗口
+        self.current_widgets = None # 当前已经展示出来的轮播窗口对象
+
+        self.defaultBackground()
+
+    def defaultBackground(self):
+        '''
+            默认背景,只有当前没有添加任何窗口时显示
+        :return:
+        '''
+        print(self.isEmpty())
+        if self.isEmpty():
+            self.setStyleSheet('''
+background-color:gray;
+border-radius:5px;
+            ''')
+    
+    # 设置动画方向模式
+    def setAinDirectionMode(self,modes:tuple):
+        if isinstance(modes,tuple):
+            self.Ani_Left_btn.disconnect()
+            self.Ani_Right_btn.disconnect()
+            self.Ani_Left_btn.clicked.connect(lambda: self.roll_event(modes[0]))
+            self.Ani_Right_btn.clicked.connect(lambda: self.roll_event(modes[1]))
+
+    # 设置动画间隔时间
+    def setAnimationTime(self,interval:int=300):
+        self.animation_time = interval
+
+    # 自动轮播
+    def setAutoSlideShow(self,b:bool,interval:int=2000,direction: str="Ani_Right",is_not_show_btn:bool=True):
+        '''
+            b: 是否启动自动轮播
+            interval:切换窗口的事件间隔
+            direction:轮播方向
+            is_not_show_btn:是否需要显示左右按钮
+        '''
+        self.is_auto_slide = b
+        if b:
+            self.startTimer(interval)
+
+        self.setHideButtons(is_not_show_btn)
+
+        self.auto_direction = direction
+        self.Ani_Left_btn.setEnabled(not b)
+        self.Ani_Right_btn.setEnabled(not b)
+
+    # 设置隐藏/显示左右按钮
+    def setHideButtons(self,b:bool=False):
+        if b:
+            self.Ani_Left_btn.hide()
+            self.Ani_Right_btn.hide()
+        else:
+            self.Ani_Left_btn.show()
+            self.Ani_Right_btn.show()
+
+    # 获取当前窗口的数量
+    def getWidgetCount(self) -> int:
+        return len(self.widgets)
+
+    # 轮播事件
+    def roll_event(self, direction: str):
+        if self.show_mode == SlideShow.FlatMode:  # 经典模式
+            widgets_count = self.getWidgetCount()
+
+            if self.isEmpty():
+                return
+
+            self.index[0] += 1
+            self.index[1] += 1
+
+            if self.index[0] > widgets_count - 1:
+                self.index[0] = 0
+
+            if self.index[1] > widgets_count - 1:
+                self.index[1] = 0
+
+            self.cu_index = self.index[1] # 设置当前索引
+            self.switchWidgeted.emit(self.index[1]) # 发送事件
+            self.rollShow(direction)
+
+    # 通过索引获取窗口
+    def getWidget(self,index:int) -> QWidget:
+        return self.widgets[index]
+
+    def isEmpty(self) -> bool:
+        return True if not self.widgets else False
+
+    # 滚动显示
+    def rollShow(self,direction: str):
+        widget = self.widgets[self.index[0]] # type:QWidget
+        widget2 = self.widgets[self.index[1]] # type:QWidget
+        self.__createWidget(widget2)
+        self.animation_(direction,widget,widget2)
+
+    # 添加窗口
+    def addWidget(self,widget:QWidget):
+        self.widgets.append(widget)
+        # 展示
+        self.show_()
+
+    # 移除窗口(2022.12.26该方法处于测试中,可能有BUG)
+    def removeWidget(self,obj_or_index):
+        '''
+            obj_or_index: 窗口对象,或者是索引
+        '''
+
+        if isinstance(obj_or_index,int):
+            widget = self.widgets[obj_or_index] # type:QWidget
+            self.widgets.remove(widget)
+            widget.hide()
+        else:
+            obj_or_index.hide()
+            self.widgets.remove(obj_or_index)
+
+    # 切换到指定窗口(暂时放弃改函数)
+    def setCurrentIndex(self,index:int=0,is_animation:bool=False):
+        if not is_animation:
+            widget = self.getWidget(index)
+
+            self.__createWidget(widget)
+
+    # 获取当前索引
+    def getIndex(self)->int:
+        if self.isEmpty():
+           return None
+
+        return self.cu_index
+
+    # 切换到下一个窗口
+    def next(self):
+        self.roll_event(SlideShow.Ani_Right)
+
+    # 切换到上一个窗口
+    def Ani_Up(self):
+        self.roll_event(SlideShow.Ani_Left)
+
+    # 两侧的按钮
+    def btnPos(self):
+        self.Ani_Left_btn.move(5, self.height() // 2 - self.Ani_Left_btn.height() // 2)
+        self.Ani_Right_btn.move(self.width() - self.Ani_Right_btn.width() - 5,
+                            self.height() // 2 - self.Ani_Left_btn.height() // 2)
 
     # 按钮样式
     def btnStyle(self):
         self.Ani_Left_btn.setStyleSheet('''
 #Ani_Left_btn{
 background-color:transparent;
 border:2px solid #73ffcc;
@@ -110,179 +232,86 @@
 border-radius:5px;
 }
 #Ani_Right_btn:hover{
 border:2px solid #00557f;
 }
                 ''')
 
-    def btnPos(self):
-        self.Ani_Left_btn.move(5, self.height() // 2 - self.Ani_Left_btn.height() // 2)
-        self.Ani_Right_btn.move(self.width() - self.Ani_Right_btn.width() - 5,
-                            self.height() // 2 - self.Ani_Left_btn.height() // 2)
-
-    def count(self) -> int:
-        return len(self.widgets)
-
-    # 移动窗口
-    def moveWidget(self,direction_:str):
-        direction = None
-
-        w_1 = self.widgets[self.index]
-        if direction_ == "R": # self.index < self.count() - 1
-            direction = self.rd_direction()
-            self.index += 1
-            if self.index > self.count()-1:
-                self.index = 0
-
-        if direction_ == "L": # and self.index >= 0
-            direction = self.lu_direction()
-            self.index -= 1
-            if self.index < -self.count():
-                self.index = -1
-
-        if not direction:
-            return
-
-
-        w_2 = self.widgets[self.index]
-        self.cursor_widget_p = w_2 # 保存当前窗口
-        self.cursor_widget_p2 = w_1
-        self.changeWidget.emit(w_2)# 切换窗口时发送信号
-        w_1.show()
-        w_2.show()
+    # 返回左右按钮对象
+    def getButtons(self) -> tuple:
+        return self.Ani_Left_btn,self.Ani_Right_btn
 
-        self.ani_(w_1, w_2, direction)
+    # 展示
+    def show_(self):
+        if self.show_mode == SlideShow.FlatMode:  # 经典模式
+
+            if self.isEmpty():
+                return
+
+            # 优先展示第一个窗口
+            widget = self.widgets[self.cu_index]  # type:QWidget
+            self.__createWidget(widget)
+
+            # 隐藏除了显示的以外的所有窗口
+            for i in range(self.getWidgetCount()):
+                if i != self.getIndex():
+                    self.getWidget(i).hide()
 
-    def addWidget(self,widget:QWidget):
+    # 创建窗口
+    def __createWidget(self,widget:QWidget):
         widget.setParent(self)
-
-        widget.resize(self.size())
+        widget.resize(QSize(self.width(),self.height()))
         widget.lower()
-        self.widgets.append(widget)
+        widget.move(QPoint(0,0))
+        widget.show()
 
-        if self.count() > 1:
-            widget.hide()
-        else:
-            self.cursor_widget_p = widget
-
-    # 设置动作模式
-    def setAinDirectionMode(self, mode:tuple):
-        if mode[0] not in [SlideShow.Ani_Up,SlideShow.Ani_Left] and\
-            mode[1] not in [SlideShow.Ani_Right,SlideShow.Ani_Down]:
-            raise TypeError("Parameter error!")
-
-        self.ani_direction = mode
-
-    # 设置按钮的隐藏和显示
-    def setButtonsHide(self,b:bool):
-        self.Ani_Left_btn.setHidden(b)
-        self.Ani_Right_btn.setHidden(b)
-
-    def aniDirection(self) -> tuple:
-        return self.ani_direction
-
-    # 移除窗口
-    def removeWidget(self,widget:QWidget):
-        widget.hide()
-        if widget == self.cursor_widget_p:
-            index = self.widgets.index(widget)
-            if index == 0 and self.count() >=1:
-                wid = self.widgets[index+1]
-                wid.resize(self.size())
-                wid.show()
-                self.cursor_widget_p = wid
-            else:
-                self.cursor_widget_p = None
-        if widget == self.cursor_widget_p2:
-            self.cursor_widget_p2 = None
-        self.widgets.remove(widget)
-        del widget
-
-    # 切换到指定窗口
-    def setCurrentIndex(self,index:int=0):
-        n = 0
-        direction = "R"
-        if index > self.index:
-            n = index - self.index
-
-        if index < self.index:
-            direction = "L"
-            n = self.index - index
-
-        for _ in range(abs(n)):
-            self.moveWidget(direction)
-
-    def ani_(self,widget_out:QWidget,widget_show:QWidget,direction:str):
-        '''
-            widget_out:被移走的窗口
-            widget_show:准备显示的窗口
-        '''
-
-        if not widget_out.parent():
-            widget_out.setParent(self)
-
-        if not widget_show.parent():
-            widget_show.setParent(self)
-
-        wid1,wid2 = widget_out,widget_show
-        wid1.resize(self.size())
-        wid2.resize(self.size())
-
-
-        ani_1 = QPropertyAnimation(wid1,b"pos",self)
-        ani_2 = QPropertyAnimation(wid2,b"pos",self)
-        ani_1.setDuration(self.animation_time)
-        ani_2.setDuration(self.animation_time)
-
-        if direction == SlideShow.Ani_Left:
-            s_ani_1, e_ani_1 = QPoint(0, 0), QPoint(-self.width(), 0)
-            s_ani_2, e_ani_2 = QPoint(self.width(), 0), QPoint(0, 0)
-        elif direction == SlideShow.Ani_Up:
-            s_ani_1, e_ani_1 = QPoint(0, 0), QPoint(0, -self.height())
-            s_ani_2, e_ani_2 = QPoint(0, self.height()), QPoint(0, 0)
-        elif direction == SlideShow.Ani_Down:
-            s_ani_1, e_ani_1 = QPoint(0, 0), QPoint(0, self.height())
-            s_ani_2, e_ani_2 = QPoint(0, -self.height()), QPoint(0, 0)
-        else:
-            s_ani_1,e_ani_1 = QPoint(0,0),QPoint(self.width(),0)
-            s_ani_2,e_ani_2 = QPoint(-self.width(),0),QPoint(0,0)
-
-        # 在移出窗口动画完成时,执行隐藏
-        ani_1.finished.connect(lambda :wid1.hide())
+    # 动画
+    def animation_(self,direction:str,widget:QWidget,widget2:QWidget):
+        if self.animation_mode == SlideShow.Translation:
+            if len(self.widgets) >= 2:
+                move_ani = QPropertyAnimation(self)
+                move_ani2 = QPropertyAnimation(self)
+                move_ani.setPropertyName(b"pos")
+                move_ani2.setPropertyName(b"pos")
+                move_ani.setTargetObject(widget)
+                move_ani2.setTargetObject(widget2)
+
+                move_ani.setStartValue(widget.pos())
+                if direction == SlideShow.Ani_Right:
+                    end_value,start_value = QPoint(widget.width(), 0),QPoint(-widget.width(), 0)
+                elif direction == SlideShow.Ani_Left:
+                    end_value,start_value = QPoint(-widget.width(), 0),QPoint(widget.width(), 0)
+                elif direction == SlideShow.Ani_Down:
+                    end_value,start_value = QPoint(0,widget.height()),QPoint(0,-widget.height())
+                elif direction == SlideShow.Ani_Up:
+                    end_value, start_value = QPoint(0, -widget.height()), QPoint(0, widget.height())
+                else:
+                    end_value, start_value = QPoint(widget.width(), 0), QPoint(-widget.width(), 0)
+                move_ani.setEndValue(end_value)
+                move_ani2.setStartValue(start_value)
+                move_ani2.setEndValue(QPoint(0, 0))
 
-        ani_1.setStartValue(s_ani_1)
-        ani_1.setEndValue(e_ani_1)
 
-        ani_2.setStartValue(s_ani_2)
-        ani_2.setEndValue(e_ani_2)
+                move_ani.setDuration(self.animation_time)
+                move_ani2.setDuration(self.animation_time)
 
-        ani_1.start()
-        ani_2.start()
+                move_ani.start()
+                move_ani2.start()
 
-    # 通过索引获取窗口
-    def getWidget(self,index:int) -> QWidget:
-        return self.widgets[index]
-
-    # 反按钮对象
-    def getButtons(self)->tuple:
-        return self.Ani_Left_btn,self.Ani_Right_btn
-
-    def isEmpty(self) -> bool:
-        return True if not self.widgets else False
+    def resizeEvent(self, e:QResizeEvent) -> None:
+        self.btnPos()
+        self.show_()
+        super().resizeEvent(e)
 
-    def timerEvent(self, event) -> None:
+    def timerEvent(self, e) -> None:
         if self.is_auto_slide:
-            self.moveWidget(self.auto_ani_direction)
-
-    # 返回当前的窗口
-    def getCursorWidget(self)->QWidget:
-        return self.cursor_widget
-
-    def resizeEvent(self, event) -> None:
-        self.btnPos()
-        if self.cursor_widget_p:
-            self.cursor_widget_p.resize(self.size())
-            # 窗口大小改变时只显示当前窗口,隐藏其他窗口
-            if self.cursor_widget_p2 and self.cursor_widget_p2.isHidden() is False:
-                self.cursor_widget_p2.hide()
+            self.roll_event(self.auto_direction)
 
-        super().resizeEvent(event)
+if __name__ == '__main__':
+    app = QApplication(sys.argv)
+    win = SlideShow()
+    win.show()
+
+    if PYQT_VERSIONS in ["PyQt6", "PySide6"]:
+        sys.exit(app.exec())
+    else:
+        sys.exit(app.exec_())
```

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/slider/slider.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/slider/slider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from PyQt5 import QtGui
-
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
     QApplication,sys,
     Signal,
     Widget,
     QPainter,
     QColor,
```

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/switchButtons/swButton.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/switchButtons/swButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/toolBox.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/toolBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/toolList.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/toolList.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/WidgetABC.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/WidgetABC.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/borderlessMainWindow.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/borderlessMainWindow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/statusBar.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/statusBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/tets/2.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/tets/2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/titleBar.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/core/widgets/titleBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qt.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qt.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,7 +117,10 @@
     TabFocus = Qt.FocusPolicy.TabFocus
     ClickFocus = Qt.FocusPolicy.ClickFocus
     StrongFocus = Qt.FocusPolicy.StrongFocus
     OutBounce = QEasingCurve.Type.OutBounce
     CosineCurve = QEasingCurve.Type.CosineCurve
     SineCurve = QEasingCurve.Type.SineCurve
     InCurve = QEasingCurve.Type.InCurve
+    Unchecked = Qt.CheckState.Unchecked
+    Checked = Qt.CheckState.Checked
+    PartiallyChecked = Qt.CheckState.PartiallyChecked
```

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qtCore.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qtCore.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     #     Property as pyqtProperty,
     #     QEvent,
     #     QObject,
     #     QFile
     # )
 if PYQT_VERSIONS == "PySide6":
     from PySide6.QtCore import *
+    from PySide6.QtCore import Property as pyqtProperty
     # from PySide6.QtCore import (
     #     Qt,
     #     QUrl,
     #     Signal,
     #     QSize,
     #     QPoint,
     #     QPointF,
```

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qtGui.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qtGui.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qtWidgets.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/Qt/qtWidgets.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/__init__.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/customStyle.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/customStyle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from PyQtGuiLib.header import (
     QColor,
     qt,
     Qt,
     QPoint,
     QRect,
-    pyqtProperty
+    pyqtProperty,
 )
 import re
 import json
 '''
     公共自定义样式
 '''
```

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/utility.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/header/utility.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,18 @@
     QPoint,
     QSize,
     QFontMetricsF,
     QFont,
     QWidget,
 )
 from PyQtGuiLib.header.customStyle import CustomStyle
-
+'''
+QListWidget 在Pyqt5页面刷新的方式 update(),其他版本可以用repaint()来达到一样的效果
+QListWidget 的update(item)需要传递一个参数
+'''
 
 is_win_sys = True if platform.system() == "win32" else False
 
 is_mac_sys = True if platform.system() == "Darwin" else False
 
 
 '''
```

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/layoutDeformation/test.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/layoutDeformation/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/buttons/buttonStyle.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/buttons/buttonStyle.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/component.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/component.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/controlType.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/controlType.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/styleLinker.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/styleLinker.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/styleLinkerUi.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/linker/styleLinkerUi.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/drak/qssDrak.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/drak/qssDrak.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/image/image_rc.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/image/image_rc.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/qssFile.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/qssFile.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/test.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/qssFile/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,18 @@
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 import sys
 from PyQt5.QtWidgets import QApplication, QWidget
-from PyQt5 import QtCore, QtGui, QtWidgets
-from PyQt5.QtGui import QColor
+from PyQt5 import QtCore, QtWidgets
 
 from PyQtGuiLib.styles.qssFile.drak.qssDrak import QSSDrak
 from PyQtGuiLib.styles import QssStyleAnalysis
-from PyQtGuiLib.animation.animation import Animation
 
 
 class Test(QWidget):
     def __init__(self, *args,**kwargs) -> None:
         super().__init__(*args,**kwargs)
         self.setupUi()
```

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/skinABC.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/skinABC.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/styleAnalysis.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/styleAnalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # @software:PyCharm
 
 '''
 
     QSS 样式解析器
 '''
 from PyQtGuiLib.header import (
+    PYQT_VERSIONS,
     SyntaxError,
     KeyError,
     QMutex
 )
 import typing
 import re
 
@@ -258,15 +259,18 @@
         return dictTostr(self.toDict())
 
     def __updateStyle(self, parent):
         # Thread safety
         self.__mutex.lock()
         parent.setStyleSheet("")
         parent.setStyleSheet(self.toStr())
-        parent.update()
+        if PYQT_VERSIONS == "PyQt5":
+            parent.update()
+        else:
+            parent.repaint()
         self.__mutex.unlock()
 
     # updata QSS
     def updateStyleSheet(self,ang=None,parent=None):
         if ang is None:
             ang = self._qss[0].header()
         if parent is None and self.__parent is None:
```

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/superPainter/superPainter.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/superPainter/superPainter.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,17 @@
     QPen,
     QBrush,
     QFont,
     qt,
     Qt,
     QColor,
     QPaintEvent,
+    QPoint,
+    QRect,
+    QLine
 )
 import typing
 
 '''
         drawRect 有(x,y)
         drawRoundedRect  有(x,y)
         drawLine 有(x,y)
@@ -54,14 +57,22 @@
 
 
 class VirtualObject:
     def __init__(self,vobj_name:str,**kwargs):
         self.__vobj_name = vobj_name
         self.__vir_attr = kwargs # 虚拟属性
 
+        self.__isHide = False
+
+    def setHide(self,b:bool):
+        self.__isHide = b
+
+    def isHide(self)->bool:
+        return self.__isHide
+
     def type(self)->str:
         return self.getVirtualFunc().__name__
 
     def virName(self) -> str:
         return self.__vobj_name
 
     def getVirtualObjectAttr(self) -> dict:
@@ -97,31 +108,46 @@
     def updateDraw(self,*args,**kwargs):
         self.updateArgs(self.virtualObjName(),*args)
         openAttr = kwargs.get("openAttr", None)
         brushAttr = kwargs.get("brushAttr", None)
         self.updateOpenAttr(self.virtualObjName(),openAttr)
         self.updateBrushAttr(self.virtualObjName(),brushAttr)
 
+    def __getRect(self)->QRect:
+        return QRect(*self.getVirtualArgs())
+
+    # 移动
     def move(self,x,y):
         if patternClassification(self.type()) == "Rect":
             args = self.getVirtualArgs()[2:]
             self.updateArgs(x,y,*args)
 
+    # 缩放
     def scale(self,proportion:float):
         if patternClassification(self.type()) == "Rect":
-            xy = self.getVirtualArgs()[:2]
-            wh = self.getVirtualArgs()[2:4]
-            w,h = int(wh[0]*proportion),int(wh[1]*proportion)
-            self.updateArgs(*xy,w,h)
+            x, y, w, h = self.getVirtualArgs()
+            w,h = int(w*proportion),int(h*proportion)
+            self.updateArgs(x,y,w,h)
 
+    # 检测鼠标是否点在图形上
+    def isClick(self,pos:QPoint)->bool:
+        if patternClassification(self.type()) == "Rect":
+            x,y,w,h =self.getVirtualArgs()
+            cx,cy = pos.x(),pos.y()
+
+            if cx >= x and cx <= x+w and cy >= y and cy <= y+h:
+                return True
+            return False
 
 # 虚拟图形对象管理类
 class VirtualObjectManagement:
     def __init__(self):
-        # 虚拟对象字典
+        '''
+            虚拟对象管理
+        '''
         self.__virtualObjects = dict()  # type:typing.Dict[str:typing.List]
 
     def virtualObjName(self,vobj_name:str)->str:
         if self.isVirtualObject(vobj_name):
             return self.__virtualObjects[vobj_name]
         else:
             raise Exception("[{}] The virtual object does not exist!".format(vobj_name))
@@ -130,15 +156,14 @@
         return True if self.__virtualObjects.get(vobj_name,None) else False
 
     def appendVirtualObject(self, vobj_name: str, **kwargs):
         if not self.isVirtualObject(vobj_name):
             self.__virtualObjects[vobj_name] = VirtualObject(vobj_name,**kwargs)
 
 
-
 class SuperPainterAttr(QPainter):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
 
         self.__op = QPen(QColor(0,0,0))  # type:QPen
         self.__brush = QBrush(QColor(0,0,0)) # type: QBrush
         self.__font = None  # type: QFont
@@ -281,20 +306,22 @@
                         kwargs["openAttr"] = openAttr
                     if brushAttr:brushAttr = vir_brushAttr
                     elif vir_brushAttr:
                         brushAttr = vir_brushAttr
                         kwargs["brushAttr"] = brushAttr
 
                 self.__privateAttr(openAttr, brushAttr)
-                if openAttr:del kwargs["openAttr"]
-                if brushAttr:del kwargs["brushAttr"]
+                if openAttr: del kwargs["openAttr"]
+                if brushAttr: del kwargs["brushAttr"]
                 if virtual_object_name: del kwargs["virtualObjectName"]
-                value = func(*args,**kwargs)
-                self.__restorePrivateAttr(op,brush)
-                return value
+                if virtual_object_name and vir_obj.isHide() is False:
+                    func(*args, **kwargs)
+                else:
+                    func(*args, **kwargs)
+                self.__restorePrivateAttr(op, brush)
             return wrapper
 
         self.drawRect = decorator(self.drawRect)
         self.drawRoundedRect = decorator(self.drawRoundedRect)
         self.drawLine = decorator(self.drawLine)
         self.drawLines = decorator(self.drawLines)
         self.drawArc = decorator(self.drawArc)
@@ -313,13 +340,29 @@
         self.drawConvexPolygon = decorator(self.drawConvexPolygon)
         self.drawGlyphRun = decorator(self.drawGlyphRun)
         self.drawPixmap = decorator(self.drawPixmap)
         self.drawImage = decorator(self.drawImage)
         self.drawPixmapFragments = decorator(self.drawPixmapFragments)
         self.drawTiledPixmap = decorator(self.drawTiledPixmap)
 
+    # ------------下面代码是作为工具的提示代码------------
+
+    def drawRect(self, x:int,y:int,w:int,h:int,
+                 openAttr:dict=None,brushAttr:dict=None,virtualObjectName:str="") -> None:
+        super().drawRect(x,y,w,h)
+
+    def drawRoundedRect(self, x:int,y:int,w:int,h:int,r:int=5,r2:int=5,
+                        openAttr:dict=None,brushAttr:dict=None,virtualObjectName:str="") -> None:
+        super().drawRoundedRect(x,y,w,h,r,r2)
+
+    def drawLine(self, x:int,y:int,x1:int,y1:int,
+                 openAttr:dict=None,brushAttr:dict=None,virtualObjectName:str="") -> None:
+        super().drawLine(x,y,x1,y1)
+
+    def drawLines(self,*args,openAttr:dict=None,brushAttr:dict=None,virtualObjectName:str="")->None:
+        super().drawLines(*args)
 
 class SuperPainter(SuperPainterAttr):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
         self.decorator_to_all_draw_methods()
```

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/superPainter.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/styles/superPainter.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,20 +12,55 @@
     QWidget,
     QHBoxLayout,
     QVBoxLayout,
     QListWidget,
     QSize,
     QPushButton,
     qt,
+    Qt,
     QGridLayout,
     QIcon,
+    QSizePolicy,
+    QBitmap,
+    QColor,
+    QPainter,
+    QFrame
 )
 from PyQtGuiLib.core import SlideShow
 from PyQtGuiLib.styles import QssStyleAnalysis
 
+
+class CoreWidget(QFrame):
+    def __init__(self,*args,**kwargs):
+        super().__init__(*args,**kwargs)
+
+        # 悬浮标准
+        self.__suspension = False
+
+    # 设置悬浮
+    def setSuspension(self,b:bool):
+        self.__suspension = b
+
+    def paintEvent(self, e) -> None:
+        if self.__suspension:
+            mask = QBitmap(self.size())
+            mask.fill(Qt.black)
+            painter = QPainter(mask)
+            painter.setRenderHints(qt.Antialiasing | qt.SmoothPixmapTransform | qt.TextAntialiasing)
+            painter.setBrush(QColor(Qt.white))
+            painter.drawEllipse(self.width()-98, -6, 110, 105)
+            self.setMask(mask)
+            painter.end()
+        else:
+            mask = QBitmap(self.size())
+            mask.fill(Qt.black)
+            self.setMask(mask)
+
+
+
 class ListTemplateWindowUI(QWidget):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
 
         self.setWindowTitle("ListTemplateWindow")
         self.setupUi()
         self.defaultStyle()
@@ -36,45 +71,46 @@
         self.gridLayout.setContentsMargins(1, 1, 1, 1)
         self.gridLayout.setSpacing(0)
         self.gridLayout.setObjectName("gridLayout")
         self.listWidget = QListWidget(self)
         self.listWidget.setMaximumSize(QSize(260, 16777215))
         self.listWidget.setObjectName("listWidget")
         self.gridLayout.addWidget(self.listWidget, 0, 0, 2, 1)
-        self.widget_2 = QWidget(self)
-        self.widget_2.setMinimumSize(QSize(0, 130))
-        self.widget_2.setMaximumSize(QSize(16777215, 130))
-        self.widget_2.setObjectName("widget_2")
-        self.horizontalLayout = QHBoxLayout(self.widget_2)
+        self.widget_head = QWidget(self)
+        self.widget_head.setMinimumSize(QSize(0, 130))
+        self.widget_head.setMaximumSize(QSize(16777215, 130))
+        self.widget_head.setObjectName("widget_2")
+        self.horizontalLayout = QHBoxLayout(self.widget_head)
         self.horizontalLayout.setContentsMargins(5, 0, 5, 0)
         self.horizontalLayout.setSpacing(0)
         self.horizontalLayout.setObjectName("horizontalLayout")
-        self.btn_fold = QPushButton(self.widget_2)
+        self.btn_fold = QPushButton(self.widget_head)
         self.btn_fold.setText("三")
         self.btn_fold.setMinimumSize(QSize(50, 50))
         self.btn_fold.setMaximumSize(QSize(50, 50))
         self.btn_fold.setStyleSheet("background-color: rgb(234, 234, 234);\n"
 "border:none;\n"
 "font: 14pt \"黑体\";")
         self.btn_fold.setObjectName("btn_fold")
         self.horizontalLayout.addWidget(self.btn_fold)
-        self.head_middle_widget = QWidget(self.widget_2)
+        self.head_middle_widget = QWidget(self.widget_head)
         self.head_middle_vbody = QVBoxLayout(self.head_middle_widget)
         self.head_middle_vbody.setContentsMargins(0,0,0,0)
         self.head_middle_vbody.setSpacing(0)
         self.head_middle_widget.setObjectName("head_middle_widget")
         self.horizontalLayout.addWidget(self.head_middle_widget)
-        self.btn_head_picture = QPushButton(self.widget_2)
+        self.btn_head_picture = QPushButton()
         self.btn_head_picture.setMinimumSize(QSize(100, 100))
         self.btn_head_picture.setMaximumSize(QSize(100, 100))
         self.btn_head_picture.setObjectName("btn_head_picture")
         self.horizontalLayout.addWidget(self.btn_head_picture)
-        self.gridLayout.addWidget(self.widget_2, 0, 1, 1, 1)
-        self.core_widget = QWidget(self)
+        self.gridLayout.addWidget(self.widget_head, 0, 1, 1, 1)
+        self.core_widget = CoreWidget(self)
         self.core_widget.setObjectName("core_widget")
+        self.core_widget.setSizePolicy(QSizePolicy.Expanding,QSizePolicy.Expanding)
         self.gridLayout.addWidget(self.core_widget, 1, 1, 1, 1)
         self.core_vboy = QVBoxLayout(self.core_widget)
         self.core_vboy.setContentsMargins(6,6,6,6)
         self.stackedWidget = SlideShow()
         self.stackedWidget.setButtonsHide(True)
         self.core_vboy.addWidget(self.stackedWidget)
 
@@ -83,50 +119,41 @@
 
     def defaultStyle(self):
         self.setStyleSheet('''
         background-color: #fff;
         border:none;
         ''')
 
-        self.btn_head_picture.setStyleSheet(r'''
+        self.qss_head_picture = QssStyleAnalysis(self.btn_head_picture)
+        self.qss_head_picture.setQSS(r'''
         QPushButton{
         border:2px solid #789ac9;
         border-radius:50px;
         }
         QPushButton:hover{
         border:2px solid #f7e151;
         }
         ''')
-        self.qss = QssStyleAnalysis(self.listWidget)
-        self.qss.setQSS('''
+        self.qss_head_picture.selector("QPushButton").updateAttr("border-radius","{}px".format(self.btn_head_picture.width()//2))
+
+        self.qss_listwiget = QssStyleAnalysis(self.listWidget)
+        self.qss_listwiget.setQSS('''
 QListView {
 border-right:1px solid rgb(234,234,234);
 outline: 0px;
 background-color: #fff;
 color: #000;
 font: 14pt "黑体";
 }
 QListView::item{
 padding: 5px;
 }
 QListView::item:hover{
-border-right:5px solid #0055ff;
 background-color: rgba(170, 255, 255,100);
 color: #000;
 }
 QListView::item:selected{
 border-right:5px solid #0055ff;
 background-color: rgba(170, 255, 255,200);
 color: #000;
 }
         ''')
-
-if __name__ == '__main__':
-    app = QApplication(sys.argv)
-
-    win = ListTemplateWindowUI()
-    win.show()
-
-    if PYQT_VERSIONS in ["PyQt6","PySide6"]:
-        sys.exit(app.exec())
-    else:
-        sys.exit(app.exec_())
```

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py` & `PyQtGuiLib-2.7.20.11/abandonCase/widgets/statusBar.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,157 +1,192 @@
 # -*- coding:utf-8 -*-
-# @time:2023/4/1110:30
+# @time:2023/1/411:16
 # @author:LX
-# @file:listTemplateWindow.py
+# @file:statusBar.py
 # @software:PyCharm
+from PyQt5.QtCore import QObject
+
 from PyQtGuiLib.header import (
-    PYQT_VERSIONS,
-    QApplication,
-    sys,
+    is_win_sys,
+    is_mac_sys,
+    time,
+    QThread,
+    Signal,
     QWidget,
-    QListWidgetItem,
-    QIcon,
-    QSize,
-    QPropertyAnimation,
-    QGridLayout,
-    qt,
-    Qt,
-    QMenu,
-    QAction,
-    QPoint,
-    QGraphicsDropShadowEffect,
-    QColor
+    QHBoxLayout,
+    QLabel,
+    QPushButton,
+    QSpacerItem,
+    QPaintEvent,
+    qt
 )
-from random import randint
-import typing
+'''
+    状态栏
+'''
 
-from PyQtGuiLib.templateWindow.UI.listTemplateWindowUI import ListTemplateWindowUI
 
+# 倒计时类
+class CountDownThread(QThread):
+    # 计时完成信号
+    timeOuted = Signal()
 
-class ListTemplateWindow(ListTemplateWindowUI):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
+        self.time_ = 0
+
+    # 设置时间
+    def setTime(self,time:int):
+        self.time_ = time
+
+    def run(self) -> None:
+        while self.time_:
+            self.sleep(1)
+            self.time_-=1
+        self.timeOuted.emit()
+
+from PyQtGuiLib.core.widgets2 import WidgetABC
+class StatusBar(WidgetABC):
+
+    PosBottom = "PosBottom"
+    PosTop = "PosTop"
+
+    def __init__(self,*args,**kwargs):
+        super().__init__(*args,**kwargs)
+
+        self.setAttribute(qt.WA_StyledBackground,True)
+
+        self.h = 30
 
-        # 伸缩标记,伸缩值
-        self.__flexible_flag = True
-        self.__flexible_value = (260,60)
-
-        self.listWidget.setIconSize(QSize(50,50))
-
-        self.__ani = QPropertyAnimation(self)
-        self.__ani.setTargetObject(self.listWidget)
-        self.__ani.setPropertyName(b"size")
-        self.__ani.setDuration(600)
-
-        self.setContextMenuPolicy(Qt.CustomContextMenu)
-
-        self.__shadow = QGraphicsDropShadowEffect(self)
-        self.__shadow.setOffset(0,0)
-        self.__shadow.setBlurRadius(30)
-        self.__shadow.setColor(QColor("#8ab2e7"))
-        self.btn_head_picture.setGraphicsEffect(self.__shadow)
-
-        # 菜单列表
-        self.__menus = []
-        self.__meun_list = []
-
-        self.__myEvent()
-
-    def addMenu(self,item:dict):
-        self.__menus.append(item)
-
-    def __menu_event(self):
-        if not self.__menus:
-            return
-
-        self.menu = QMenu(self)
-        self.menu.setStyleSheet('''
-        QMenu {
-        border:none;
-        font: 12pt "黑体";
-        border-radius:5px;
-        padding: 0,0,0,15px;
-        }
-        QMenu::item:selected{
-        background-color:#789ac9;
-        }
-                ''')
-
-        for act in self.__menus:
-            text = act["text"]
-            call = act.get("call",None)
-            obj = act.get("obj",None)
-            if obj is None:
-                act["obj"] = QAction(text)
-                obj = act["obj"]
-                if call:
-                    obj.triggered.connect(call)
-            self.menu.addAction(obj)
-
-        x = self.btn_head_picture.pos().x()+self.x()+self.listWidget.width()
-        y = self.btn_head_picture.pos().y()+self.y()+self.head_middle_widget.height()+10
-
-        pos = QPoint(x,y)
-        self.menu.popup(pos)
-
-    # 设置头像
-    def setHeadPicture(self,path:str,size:tuple=(100,100)):
-        self.btn_head_picture.setIconSize(QSize(*size))
-        self.btn_head_picture.setIcon(QIcon(path))
-
-    def addItem(self,text:typing.Union[str,QListWidgetItem],widget:QWidget,icon:str=None):
-        if isinstance(text,QListWidgetItem):
-            if icon:
-                text.setIcon(QIcon(icon))
-            self.listWidget.addItem(text)
-            return
-
-        item = QListWidgetItem()
-        item.setText(text)
-        if icon:
-            item.setIcon(QIcon(icon))
-        self.listWidget.addItem(item)
-        self.stackedWidget.addWidget(widget)
-
-    # 添加头部窗口
-    def addHeadWidget(self,widget:QWidget):
-        self.head_middle_vbody.addWidget(widget)
-
-    def __ani_event(self):
-        if self.stackedWidget.count() < 1:
-            return
-
-        self.__ani.setStartValue(self.listWidget.size())
-        if self.__flexible_flag:
-            self.qss.selector("QListView::item:hover").removeAttr("border-right")
-            self.qss.selector("QListView::item:selected").removeAttr("border-right")
-            self.__ani.setEndValue(QSize(self.__flexible_value[1],self.listWidget.height()))
-            self.__flexible_flag = False
+        # 默认半径
+        # self.setRadius((0, self.radius()[0]))
+        # print(self.radius())
+        # self.setRadius((3, 5))
+        # self.setBorderWidth(0)
+
+        self.__parent = None #  type:QWidget
+
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
+
+        # 创建倒计时类
+        self.cd = CountDownThread()
+
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
+    def parent(self) -> QObject:
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
         else:
-            self.qss.selector("QListView::item:hover").updateAttr("border-right","5px solid #0055ff;")
-            self.qss.selector("QListView::item:selected").updateAttr("border-right","5px solid #0055ff")
-            self.__ani.setEndValue(QSize(self.__flexible_value[0], self.listWidget.height()))
-            self.__flexible_flag = True
-
-        self.__ani.valueChanged.connect(lambda v:self.listWidget.setMaximumWidth(v.width()))
-        self.__ani.start()
-
-    def __change_st_event(self,item:QListWidgetItem):
-        index = self.listWidget.indexFromItem(item).row()
-        self.stackedWidget.setCurrentIndex(index)
-
-    def __myEvent(self):
-        self.listWidget.itemClicked.connect(self.__change_st_event)
-        self.btn_fold.clicked.connect(self.__ani_event)
-        self.btn_head_picture.clicked.connect(self.__menu_event)
-
-
-if __name__ == '__main__':
-    app = QApplication(sys.argv)
-
-    win = ListTemplateWindow()
-    win.show()
-
-    if PYQT_VERSIONS in ["PyQt6","PySide6"]:
-        sys.exit(app.exec())
-    else:
-        sys.exit(app.exec_())
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

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib.egg-info/PKG-INFO` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtGuiLib
-Version: 2.7.18.11
+Version: 2.7.20.11
 Summary: Python version of the qt component library.
 Home-page: https://github.com/LX-sys/PyQtGuiLib
 Author: LX
 Author-email: lx984608061@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyQtGuiLib-2.7.18.11/PyQtGuiLib.egg-info/SOURCES.txt` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 LICENSE.txt
 README.md
 setup.py
 Log/__init__.py
 Log/developmentLog.py
 PyQtGuiLib/__init__.py
+PyQtGuiLib/listTree.py
 PyQtGuiLib.egg-info/PKG-INFO
 PyQtGuiLib.egg-info/SOURCES.txt
 PyQtGuiLib.egg-info/dependency_links.txt
 PyQtGuiLib.egg-info/top_level.txt
+PyQtGuiLib/animation/PropertyAnimation.py
 PyQtGuiLib/animation/__init__.py
 PyQtGuiLib/animation/animation.py
-PyQtGuiLib/animation/animationDrawType.py
-PyQtGuiLib/animation/animationFactory.py
-PyQtGuiLib/animation/animationLayout.py
-PyQtGuiLib/animation/customAniTest.py
-PyQtGuiLib/animation/lmlmAni.py
+PyQtGuiLib/animation/test_animation.py
 PyQtGuiLib/core/__init__.py
 PyQtGuiLib/core/bubbleWidget.py
+PyQtGuiLib/core/expansionBar.py
 PyQtGuiLib/core/flowLayout.py
+PyQtGuiLib/core/imageButton.py
 PyQtGuiLib/core/listWidget.py
 PyQtGuiLib/core/pullOver.py
 PyQtGuiLib/core/rollWidget.py
 PyQtGuiLib/core/slideShow.py
 PyQtGuiLib/core/toolBox.py
 PyQtGuiLib/core/toolList.py
 PyQtGuiLib/core/comboBox/__init__.py
 PyQtGuiLib/core/comboBox/combBox.py
 PyQtGuiLib/core/comboBox/comboBox.py
 PyQtGuiLib/core/comboBox/comboBox2.py
+PyQtGuiLib/core/drawers/__init__.py
+PyQtGuiLib/core/drawers/drawer.py
 PyQtGuiLib/core/lineedit/__init__.py
 PyQtGuiLib/core/lineedit/dynamicTLine.py
 PyQtGuiLib/core/logBrowser/__init__.py
 PyQtGuiLib/core/logBrowser/loadLogTh.py
 PyQtGuiLib/core/logBrowser/logBrowser.py
 PyQtGuiLib/core/logBrowser/logSizeTh.py
 PyQtGuiLib/core/notice/__init__.py
 PyQtGuiLib/core/notice/notice.py
 PyQtGuiLib/core/palettes/__init__.py
 PyQtGuiLib/core/palettes/colorHsv.py
 PyQtGuiLib/core/palettes/paletteFrame.py
 PyQtGuiLib/core/progressBar/__init__.py
 PyQtGuiLib/core/progressBar/circularBar.py
+PyQtGuiLib/core/progressBar/circularProgressBar.py
 PyQtGuiLib/core/progressBar/gradientBar.py
 PyQtGuiLib/core/progressBar/loadBar.py
 PyQtGuiLib/core/progressBar/waterBar.py
 PyQtGuiLib/core/resolver/__init__.py
 PyQtGuiLib/core/resolver/controls.py
 PyQtGuiLib/core/slider/__init__.py
 PyQtGuiLib/core/slider/slider.py
@@ -71,14 +74,16 @@
 PyQtGuiLib/header/Qt/qtSip.py
 PyQtGuiLib/header/Qt/qtUic.py
 PyQtGuiLib/header/Qt/qtWidgets.py
 PyQtGuiLib/header/py/__init__.py
 PyQtGuiLib/header/py/common.py
 PyQtGuiLib/layoutDeformation/__init__.py
 PyQtGuiLib/layoutDeformation/test.py
+PyQtGuiLib/particle/__init__.py
+PyQtGuiLib/particle/particle.py
 PyQtGuiLib/styles/__init__.py
 PyQtGuiLib/styles/skinABC.py
 PyQtGuiLib/styles/styleAnalysis.py
 PyQtGuiLib/styles/superPainter.py
 PyQtGuiLib/styles/builtStyleDesigner/__init__.py
 PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py
 PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py
@@ -113,35 +118,47 @@
 abandonCase/slideShow.py
 abandonCase/slideShow2.py
 abandonCase/spaceWidget.py
 abandonCase/acrylic/__init__.py
 abandonCase/acrylic/acrylicWidget.py
 abandonCase/acrylic/cstruct.py
 abandonCase/acrylic/windowEffect.py
+abandonCase/animation/__init__.py
+abandonCase/animation/animation.py
+abandonCase/animation/animationDrawType.py
+abandonCase/animation/animationFactory.py
+abandonCase/animation/animationLayout.py
+abandonCase/animation/customAniTest.py
 abandonCase/widgets/__init__.py
 abandonCase/widgets/borderlessFrame.py
 abandonCase/widgets/borderlessMainWindow.py
 abandonCase/widgets/borderlessStackedWidget.py
 abandonCase/widgets/borderlessWidget.py
 abandonCase/widgets/borderlessWidgetABC.py
 abandonCase/widgets/statusBar.py
 abandonCase/widgets/titleBar.py
+auxiliaryMeans/__init__.py
+auxiliaryMeans/toolNewProject.py
 tests/__init__.py
 tests/test_BubbleWidget.py
+tests/test_CircularProgressBar.py
 tests/test_Notice.py
 tests/test_QssStyleAnalysis.py
 tests/test_SlideShow.py
 tests/test_barset.py
 tests/test_circularBar.py
 tests/test_colorPalette.py
 tests/test_comboBox.py
+tests/test_drawer.py
 tests/test_dumpStructure.py
 tests/test_dynamicTLine.py
+tests/test_expansionBar.py
 tests/test_flowLayot.py
 tests/test_gradientBar.py
+tests/test_imageButton.py
 tests/test_listWidget.py
 tests/test_loadbar.py
 tests/test_no_border.py
 tests/test_no_border_pullOver.py
 tests/test_pullOverWidget.py
 tests/test_rollWidget.py
 tests/test_slider.py
```

### Comparing `PyQtGuiLib-2.7.18.11/README.md` & `PyQtGuiLib-2.7.20.11/README.md`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/abandonCase/acrylic/acrylicWidget.py` & `PyQtGuiLib-2.7.20.11/abandonCase/acrylic/acrylicWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/abandonCase/acrylic/cstruct.py` & `PyQtGuiLib-2.7.20.11/abandonCase/acrylic/cstruct.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/abandonCase/acrylic/windowEffect.py` & `PyQtGuiLib-2.7.20.11/abandonCase/acrylic/windowEffect.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/abandonCase/bubbleWidget.py` & `PyQtGuiLib-2.7.20.11/abandonCase/bubbleWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/abandonCase/bubbleWidget_case.py` & `PyQtGuiLib-2.7.20.11/abandonCase/bubbleWidget_case.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/abandonCase/nodeBar.py` & `PyQtGuiLib-2.7.20.11/abandonCase/nodeBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/abandonCase/slideShow.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,317 +1,285 @@
 # -*- coding:utf-8 -*-
-# @time:2022/12/2317:54
+# @time:2023/4/1110:30
 # @author:LX
-# @file:SlideShow.py
+# @file:listTemplateWindow.py
 # @software:PyCharm
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
     QApplication,
     sys,
     QWidget,
-    QResizeEvent,
-    QPushButton,
-    QPoint,
+    QListWidgetItem,
+    QIcon,
     QSize,
     QPropertyAnimation,
-    Signal
+    QGridLayout,
+    qt,
+    Qt,
+    QMenu,
+    QAction,
+    QPoint,
+    QGraphicsDropShadowEffect,
+    QColor,
+    QResizeEvent,
+    QShortcut,
+    QKeySequence,
+    QVBoxLayout
 )
+from random import randint
+import typing
 
+from PyQtGuiLib.templateWindow.UI.listTemplateWindowUI import ListTemplateWindowUI
 
 
-'''
-
-    轮播图功能
-        风格: 扁平
-'''
-class SlideShow(QWidget):
-    # 切换窗口事件
-    switchWidgeted = Signal(int)
-
-    # 扁平 风格
-    FlatMode = "flat"  # 经典
-
-    # 动画的方向模式
-    Ani_Left = "left"
-    Ani_Right = "right"
-    Ani_Down = "down"
-    Ani_Up = "up"
+# 文档外框
+class DocumentFrame(QWidget):
+    def __init__(self, widget:QWidget,st,index,documents:list):
+        super().__init__()
+        self.resize(500,500)
+        self.vboy = QVBoxLayout(self)
 
 
-    # 动画
-    Translation = "translation"  # 平移
+        self.widget = widget
+        self.st = st
+        self.index = index
+        self.documents = documents
+        print(st,index)
 
-    def __init__(self,*args,**kwargs):
-        super().__init__(*args,**kwargs)
-        self.resize(700, 300)
+        self.vboy.addWidget(self.widget)
 
-        self.show_mode = SlideShow.FlatMode # 展示模式
-        self.animation_mode = SlideShow.Translation  # 动画模式
+    def closeEvent(self, e) -> None:
+        self.st.insertWidget(self.index,self.widget)
+        self.documents.remove(self.widget)
+        super().closeEvent(e)
 
-        self.animation_time = 300 # 毫秒
+class ListTemplateWindow(ListTemplateWindowUI):
+    def __init__(self,*args,**kwargs):
+        # 头像状态记录
+        self.head_suspension = {
+            "isSuspension": False
+        }
 
-        self.index = [-1,0]  # 索引
-        self.cu_index = self.index[1]  # 当前索引
-
-        # 设置自动轮播,自动轮播的方向
-        self.is_auto_slide = False
-        self.auto_direction = SlideShow.Ani_Right
-
-        # 左右按钮
-        self.Ani_Left_btn = QPushButton("左",self)
-        self.Ani_Right_btn = QPushButton("右",self)
-        self.Ani_Left_btn.setObjectName("Ani_Left_btn")
-        self.Ani_Right_btn.setObjectName("Ani_Right_btn")
-        self.Ani_Left_btn.resize(50,50)
-        self.Ani_Right_btn.resize(50,50)
-        self.Ani_Left_btn.clicked.connect(lambda :self.roll_event(SlideShow.Ani_Left))
-        self.Ani_Right_btn.clicked.connect(lambda :self.roll_event(SlideShow.Ani_Right))
-        self.btnStyle()
-
-        # 窗口
-        self.widgets = []  # 所有已经添加的窗口
-        self.current_widgets = None # 当前已经展示出来的轮播窗口对象
+        super().__init__(*args,**kwargs)
 
-        self.defaultBackground()
+        # 伸缩标记,伸缩值
+        self.__flexible_flag = True
+        self.__flexible_value = (260,60)
+
+        # 模块图标大小
+        self.listWidget.setIconSize(QSize(50,50))
+
+        # 文档窗口存储
+        self.documents = []
+
+        self.__ani = QPropertyAnimation(self)
+        self.__ani.setTargetObject(self.listWidget)
+        self.__ani.setPropertyName(b"size")
+        self.__ani.setDuration(600)
+
+        self.setContextMenuPolicy(Qt.CustomContextMenu)
+
+        self.__shadow = QGraphicsDropShadowEffect(self)
+        self.__shadow.setOffset(0,0)
+        self.__shadow.setBlurRadius(30)
+        self.__shadow.setColor(QColor("#8ab2e7"))
+        self.btn_head_picture.setGraphicsEffect(self.__shadow)
+
+        # 菜单列表
+        self.__menus = []
+        self.__meun_list = []
+
+        self.__myEvent()
+        self.__builtInMenu()
+        self.__shortcutKey()
+
+    def __builtInMenu(self):
+        self.addMenus([{
+            "text":"隐藏/显示菜单(内置功能)",
+            "call":self.sidebar_event
+            },
+            {
+                "text":"头像悬浮(内置功能)",
+                "call":self.__suspension
+            }
+        ])
+
+    # 移除头部,头像悬浮功能
+    def __suspension(self):
+        scale = 0.8  # 缩放倍率
+
+        if self.head_suspension["isSuspension"]:
+            self.btn_head_picture.setParent(None)
+            w = int(self.btn_head_picture.width() / scale)
+            h = int(self.btn_head_picture.height() / scale)
+            self.btn_head_picture.setFixedSize(w, h)
+            self.qss_head_picture.selector("QPushButton").updateAttr("border-radius",
+                                                                     "{}px".format(self.btn_head_picture.width() // 2))
+            iw = int(self.btn_head_picture.iconSize().width() / scale)
+            ih = int(self.btn_head_picture.iconSize().height() / scale)
+            self.btn_head_picture.setIconSize(QSize(iw, ih))
+            self.horizontalLayout.addWidget(self.btn_head_picture)
+            self.widget_head.show()
+            self.head_suspension["isSuspension"] = False
+            self.core_widget.setSuspension(False)
+            return
 
-    def defaultBackground(self):
         '''
-            默认背景,只有当前没有添加任何窗口时显示
-        :return:
+            将头像按钮从布局中移出,在隐藏会整个头部,
+            在将头像按钮的父级设置为整个窗口
         '''
-        print(self.isEmpty())
-        if self.isEmpty():
-            self.setStyleSheet('''
-background-color:gray;
-border-radius:5px;
-            ''')
-    
-    # 设置动画方向模式
-    def setAinDirectionMode(self,modes:tuple):
-        if isinstance(modes,tuple):
-            self.Ani_Left_btn.disconnect()
-            self.Ani_Right_btn.disconnect()
-            self.Ani_Left_btn.clicked.connect(lambda: self.roll_event(modes[0]))
-            self.Ani_Right_btn.clicked.connect(lambda: self.roll_event(modes[1]))
-
-    # 设置动画间隔时间
-    def setAnimationTime(self,interval:int=300):
-        self.animation_time = interval
+        self.horizontalLayout.removeWidget(self.btn_head_picture)
+        self.widget_head.hide()
+        self.btn_head_picture.setParent(self)
+        self.btn_head_picture.show()
+        self.btn_head_picture.move(self.width()-self.btn_head_picture.width()+10,10)
+        # 样式,图片大小跟随缩小
+        w = int(self.btn_head_picture.width()*scale)
+        h = int(self.btn_head_picture.height()*scale)
+        self.btn_head_picture.setFixedSize(w,h)
+        self.qss_head_picture.selector("QPushButton").updateAttr("border-radius","{}px".format(self.btn_head_picture.width() // 2))
+        iw = int(self.btn_head_picture.iconSize().width()*scale)
+        ih = int(self.btn_head_picture.iconSize().height()*scale)
+        self.btn_head_picture.setIconSize(QSize(iw,ih))
+
+        self.head_suspension["isSuspension"] = True
+        self.core_widget.setSuspension(True)
+
+    def addMenu(self,item:dict):
+        self.__menus.append(item)
+
+    def addMenus(self,items:typing.List[dict]):
+        for item in items:
+            self.addMenu(item)
+
+    def removeMenu(self,text:str):
+        del self.__menus[text]
+
+    def __menu_event(self):
+        if not self.__menus:
+            return
+
+        self.menu = QMenu(self)
+        self.menu.setStyleSheet('''
+        QMenu {
+        border:none;
+        font: 12pt "黑体";
+        border-radius:5px;
+        padding: 0,0,0,15px;
+        }
+        QMenu::item:selected{
+        background-color:#789ac9;
+        }
+                ''')
 
-    # 自动轮播
-    def setAutoSlideShow(self,b:bool,interval:int=2000,direction: str="Ani_Right",is_not_show_btn:bool=True):
-        '''
-            b: 是否启动自动轮播
-            interval:切换窗口的事件间隔
-            direction:轮播方向
-            is_not_show_btn:是否需要显示左右按钮
-        '''
-        self.is_auto_slide = b
-        if b:
-            self.startTimer(interval)
-
-        self.setHideButtons(is_not_show_btn)
-
-        self.auto_direction = direction
-        self.Ani_Left_btn.setEnabled(not b)
-        self.Ani_Right_btn.setEnabled(not b)
-
-    # 设置隐藏/显示左右按钮
-    def setHideButtons(self,b:bool=False):
-        if b:
-            self.Ani_Left_btn.hide()
-            self.Ani_Right_btn.hide()
-        else:
-            self.Ani_Left_btn.show()
-            self.Ani_Right_btn.show()
+        for act in self.__menus:
+            text = act["text"]
+            call = act.get("call",None)
+            obj = act.get("obj",None)
+            if obj is None:
+                act["obj"] = QAction(text)
+                obj = act["obj"]
+                if call:
+                    obj.triggered.connect(call)
+            self.menu.addAction(obj)
 
-    # 获取当前窗口的数量
-    def getWidgetCount(self) -> int:
-        return len(self.widgets)
-
-    # 轮播事件
-    def roll_event(self, direction: str):
-        if self.show_mode == SlideShow.FlatMode:  # 经典模式
-            widgets_count = self.getWidgetCount()
-
-            if self.isEmpty():
-                return
-
-            self.index[0] += 1
-            self.index[1] += 1
-
-            if self.index[0] > widgets_count - 1:
-                self.index[0] = 0
-
-            if self.index[1] > widgets_count - 1:
-                self.index[1] = 0
-
-            self.cu_index = self.index[1] # 设置当前索引
-            self.switchWidgeted.emit(self.index[1]) # 发送事件
-            self.rollShow(direction)
-
-    # 通过索引获取窗口
-    def getWidget(self,index:int) -> QWidget:
-        return self.widgets[index]
-
-    def isEmpty(self) -> bool:
-        return True if not self.widgets else False
-
-    # 滚动显示
-    def rollShow(self,direction: str):
-        widget = self.widgets[self.index[0]] # type:QWidget
-        widget2 = self.widgets[self.index[1]] # type:QWidget
-        self.__createWidget(widget2)
-        self.animation_(direction,widget,widget2)
-
-    # 添加窗口
-    def addWidget(self,widget:QWidget):
-        self.widgets.append(widget)
-        # 展示
-        self.show_()
+        if self.listWidget.isHidden():
+            x = self.btn_head_picture.x() + self.x()
+        else:
+            x = self.btn_head_picture.x() + self.x() + self.listWidget.width()
+        y = self.btn_head_picture.y()+self.y()+self.head_middle_widget.height() + 10
 
-    # 移除窗口(2022.12.26该方法处于测试中,可能有BUG)
-    def removeWidget(self,obj_or_index):
-        '''
-            obj_or_index: 窗口对象,或者是索引
-        '''
+        pos = QPoint(x,y)
+        self.menu.popup(pos)
 
-        if isinstance(obj_or_index,int):
-            widget = self.widgets[obj_or_index] # type:QWidget
-            self.widgets.remove(widget)
-            widget.hide()
+    # 设置头像
+    def setHeadPicture(self,path:str,size:tuple=(100,100)):
+        self.btn_head_picture.setIconSize(QSize(*size))
+        self.btn_head_picture.setIcon(QIcon(path))
+
+    def addItem(self,text:typing.Union[str,QListWidgetItem],widget:QWidget,icon:str=None):
+        if isinstance(text,QListWidgetItem):
+            if icon:
+                text.setIcon(QIcon(icon))
+            self.listWidget.addItem(text)
+            return
+
+        item = QListWidgetItem()
+        item.setText(text)
+        if icon:
+            item.setIcon(QIcon(icon))
+        self.listWidget.addItem(item)
+        self.stackedWidget.addWidget(widget)
+
+    # 添加头部窗口
+    def addHeadWidget(self,widget:QWidget):
+        self.head_middle_vbody.addWidget(widget)
+
+    # 隐藏/显示侧边栏
+    def sidebar_event(self):
+        if self.listWidget.isHidden():
+            self.listWidget.show()
+            self.btn_fold.show()
         else:
-            obj_or_index.hide()
-            self.widgets.remove(obj_or_index)
-
-    # 切换到指定窗口(暂时放弃改函数)
-    def setCurrentIndex(self,index:int=0,is_animation:bool=False):
-        if not is_animation:
-            widget = self.getWidget(index)
-
-            self.__createWidget(widget)
-
-    # 获取当前索引
-    def getIndex(self)->int:
-        if self.isEmpty():
-           return None
-
-        return self.cu_index
-
-    # 切换到下一个窗口
-    def next(self):
-        self.roll_event(SlideShow.Ani_Right)
-
-    # 切换到上一个窗口
-    def Ani_Up(self):
-        self.roll_event(SlideShow.Ani_Left)
-
-    # 两侧的按钮
-    def btnPos(self):
-        self.Ani_Left_btn.move(5, self.height() // 2 - self.Ani_Left_btn.height() // 2)
-        self.Ani_Right_btn.move(self.width() - self.Ani_Right_btn.width() - 5,
-                            self.height() // 2 - self.Ani_Left_btn.height() // 2)
-
-    # 按钮样式
-    def btnStyle(self):
-        self.Ani_Left_btn.setStyleSheet('''
-#Ani_Left_btn{
-background-color:transparent;
-border:2px solid #73ffcc;
-color:#73ffcc;
-border-radius:5px;
-}
-#Ani_Left_btn:hover{
-border:2px solid #00557f;
-}
-        ''')
-        self.Ani_Right_btn.setStyleSheet('''
-#Ani_Right_btn{
-background-color:transparent;
-border:2px solid #73ffcc;
-color:#73ffcc;
-border-radius:5px;
-}
-#Ani_Right_btn:hover{
-border:2px solid #00557f;
-}
-                ''')
+            self.listWidget.hide()
+            self.btn_fold.hide()
 
-    # 返回左右按钮对象
-    def getButtons(self) -> tuple:
-        return self.Ani_Left_btn,self.Ani_Right_btn
-
-    # 展示
-    def show_(self):
-        if self.show_mode == SlideShow.FlatMode:  # 经典模式
-
-            if self.isEmpty():
-                return
-
-            # 优先展示第一个窗口
-            widget = self.widgets[self.cu_index]  # type:QWidget
-            self.__createWidget(widget)
-
-            # 隐藏除了显示的以外的所有窗口
-            for i in range(self.getWidgetCount()):
-                if i != self.getIndex():
-                    self.getWidget(i).hide()
-
-    # 创建窗口
-    def __createWidget(self,widget:QWidget):
-        widget.setParent(self)
-        widget.resize(QSize(self.width(),self.height()))
-        widget.lower()
-        widget.move(QPoint(0,0))
-        widget.show()
-
-    # 动画
-    def animation_(self,direction:str,widget:QWidget,widget2:QWidget):
-        if self.animation_mode == SlideShow.Translation:
-            if len(self.widgets) >= 2:
-                move_ani = QPropertyAnimation(self)
-                move_ani2 = QPropertyAnimation(self)
-                move_ani.setPropertyName(b"pos")
-                move_ani2.setPropertyName(b"pos")
-                move_ani.setTargetObject(widget)
-                move_ani2.setTargetObject(widget2)
-
-                move_ani.setStartValue(widget.pos())
-                if direction == SlideShow.Ani_Right:
-                    end_value,start_value = QPoint(widget.width(), 0),QPoint(-widget.width(), 0)
-                elif direction == SlideShow.Ani_Left:
-                    end_value,start_value = QPoint(-widget.width(), 0),QPoint(widget.width(), 0)
-                elif direction == SlideShow.Ani_Down:
-                    end_value,start_value = QPoint(0,widget.height()),QPoint(0,-widget.height())
-                elif direction == SlideShow.Ani_Up:
-                    end_value, start_value = QPoint(0, -widget.height()), QPoint(0, widget.height())
-                else:
-                    end_value, start_value = QPoint(widget.width(), 0), QPoint(-widget.width(), 0)
-                move_ani.setEndValue(end_value)
-                move_ani2.setStartValue(start_value)
-                move_ani2.setEndValue(QPoint(0, 0))
-
-
-                move_ani.setDuration(self.animation_time)
-                move_ani2.setDuration(self.animation_time)
-
-                move_ani.start()
-                move_ani2.start()
-
-    def resizeEvent(self, e:QResizeEvent) -> None:
-        self.btnPos()
-        self.show_()
+    # 通过索引隐藏/显示,某个item
+    def setHideItem(self,index:int,b:bool=True):
+        item = self.listWidget.item(index) # type:QListWidgetItem
+        item.setHidden(b)
+
+    def __ani_event(self):
+        if self.stackedWidget.count() < 1:
+            return
+
+        self.__ani.setStartValue(self.listWidget.size())
+        if self.__flexible_flag:
+            self.qss_listwiget.selector("QListView::item:selected").removeAttr("border-right")
+            self.__ani.setEndValue(QSize(self.__flexible_value[1],self.listWidget.height()))
+            self.__flexible_flag = False
+        else:
+            self.qss_listwiget.selector("QListView::item:selected").updateAttr("border-right","5px solid #0055ff")
+            self.__ani.setEndValue(QSize(self.__flexible_value[0], self.listWidget.height()))
+            self.__flexible_flag = True
+
+        self.__ani.valueChanged.connect(lambda v:self.listWidget.setMaximumWidth(v.width()))
+        self.__ani.start()
+
+    def __change_st_event(self,item:QListWidgetItem):
+        index = self.listWidget.indexFromItem(item).row()
+        self.stackedWidget.setCurrentIndex(index)
+
+    def __myEvent(self):
+        self.listWidget.itemClicked.connect(self.__change_st_event)
+        self.btn_fold.clicked.connect(self.__ani_event)
+        self.btn_head_picture.clicked.connect(self.__menu_event)
+
+    # 默认快捷键
+    def __shortcutKey(self):
+        QShortcut(QKeySequence(self.tr("Ctrl+Q")),self,self.shortcut_ctrl_q)
+
+    def shortcut_ctrl_q(self):
+        index = self.stackedWidget.getCursorWidgetIndex()
+        widget = self.stackedWidget.popWidget(self.stackedWidget.getCursorWidget())
+        pp = DocumentFrame(widget,self.stackedWidget,index,self.documents)
+        pp.show()
+        self.documents.append(pp)
+
+
+    def resizeEvent(self, e: QResizeEvent) -> None:
+        # 在这里面处理头像悬浮状态下的位置
+        if self.head_suspension["isSuspension"]:
+            self.btn_head_picture.move(self.width() - self.btn_head_picture.width()-10, 10)
         super().resizeEvent(e)
 
-    def timerEvent(self, e) -> None:
-        if self.is_auto_slide:
-            self.roll_event(self.auto_direction)
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
-    win = SlideShow()
+
+    win = ListTemplateWindow()
     win.show()
 
-    if PYQT_VERSIONS in ["PyQt6", "PySide6"]:
+    if PYQT_VERSIONS in ["PyQt6","PySide6"]:
         sys.exit(app.exec())
     else:
-        sys.exit(app.exec_())
+        sys.exit(app.exec_())
```

### Comparing `PyQtGuiLib-2.7.18.11/abandonCase/slideShow2.py` & `PyQtGuiLib-2.7.20.11/abandonCase/slideShow2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessFrame.py` & `PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessFrame.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessMainWindow.py` & `PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessMainWindow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessStackedWidget.py` & `PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessStackedWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessWidget.py` & `PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessWidgetABC.py` & `PyQtGuiLib-2.7.20.11/abandonCase/widgets/borderlessWidgetABC.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/abandonCase/widgets/titleBar.py` & `PyQtGuiLib-2.7.20.11/abandonCase/widgets/titleBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/setup.py` & `PyQtGuiLib-2.7.20.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 
 setup(
     name="PyQtGuiLib",
     packages =find_packages(),
-    version="2.7.18.11",
+    version="2.7.20.11",
     author="LX",
     author_email = "lx984608061@163.com",
     description = "Python version of the qt component library.",
     long_description=open('README.md', 'r',encoding="utf8").read(),
     long_description_content_type="text/markdown",
     url = "https://github.com/LX-sys/PyQtGuiLib",
     classifiers = [
```

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_Animation/1.py` & `PyQtGuiLib-2.7.20.11/tests/test_Animation/1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_Animation/__init__.py` & `PyQtGuiLib-2.7.20.11/tests/test_Animation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_Animation/eg1.py` & `PyQtGuiLib-2.7.20.11/tests/test_Animation/eg1.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,23 +7,19 @@
     PYQT_VERSIONS,
     QApplication,
     sys,
     QWidget,
     QPoint,
     qt,
     QPushButton,
-    QSize,
-    QPainter,
     QColor,
-    QLinearGradient,
-    QRect
+    QLinearGradient
 )
 
 from PyQtGuiLib.animation import Animation
-from PyQtGuiLib.animation.animationLayout import AnimationLayout
 
 
 class Test(QWidget):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
         self.resize(1200,800)
```

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_1.py` & `PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_10.py` & `PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_10.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_2.py` & `PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_3.py` & `PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_3.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_4.py` & `PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_4.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_5.py` & `PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_5.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_6.py` & `PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_6.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_7.py` & `PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_7.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_8.py` & `PyQtGuiLib-2.7.20.11/tests/test_Animation/tutorial_9.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding:utf-8 -*-
-# @time:2023/3/239:06
+# @time:2023/3/239:14
 # @author:LX
-# @file:tutorial_8.py
+# @file:tutorial_9.py
 # @software:PyCharm
 from PyQtGuiLib.header import (
     QApplication,
     PYQT_VERSIONS,
     sys,
     QWidget,
     QPushButton,
@@ -18,45 +18,40 @@
 
 
 class Test(QWidget):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.resize(600, 600)
         '''
-             Animation 动画框架 案例八,QSS属性动画特性二,动态QSS属性动画
-             背景和前景色动画
+             Animation 动画框架 案例九,利用QSS属性动作,
+             来 制作透明动画
 
              注意:使用这一类动画时,你的控件必须有qss样式
         '''
         self.btn = QPushButton("按钮", self)
         self.btn.move(50, 50)
         self.btn.resize(100, 60)
-        # 写一个简单,标准的样式,按钮添加一个背景颜色
-        '''
-            在上一个案例中,我们知道这个简单标准的QSS动画,
-            那么我们去掉QSS中 background-color 这个属性在运行
-        '''
+        # 这里我们写一个带透明度的背景样式
         self.btn.setStyleSheet('''
         QPushButton{
-            color:rgb(255,0,0);
+            background-color:rgba(234,234,234,255);
         }
         ''')
 
         # 实例化动画类
         self.ani = Animation(self)
         # 设置动画时长
         self.ani.setDuration(3000)  # 3秒
 
-        # 添加一个QSS属性动画
+        # 添加一个QSS属性动画,通过降低rgba 中的 a属性来达到透明效果
         self.ani.addAni({
             "targetObj": self.btn,
             "propertyName": b"background-color",
-            # "sv":"this",  # 注意: 在对原本控件中没有样式经行动画时,是不允许使用 "this" 指向自己的
-            "sv": QColor(0,255,0),
-            "ev": QColor(200, 200, 100),
+            "sv":"this",
+            "ev": QColor(234,234,234,50),
             "selector": "QPushButton"
         })
         # 开始动画
         self.ani.start()
 
 
 if __name__ == '__main__':
```

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_9.py` & `PyQtGuiLib-2.7.20.11/tests/test_circularBar.py`

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

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_BubbleWidget.py` & `PyQtGuiLib-2.7.20.11/tests/test_BubbleWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_Notice.py` & `PyQtGuiLib-2.7.20.11/tests/test_Notice.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     QMoveEvent,
     QThread,
     Signal
 )
 from random import randint
 from PyQtGuiLib.core import Notice,Notices
 
+
 class Time(QThread):
     add = Signal()
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
 
 
     def run(self) -> None:
@@ -22,14 +23,15 @@
         while True:
             self.sleep(randint(1,1))
             self.add.emit()
             if n == 5:
                 break
             n+=1
 
+
 class Test(QWidget):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
         self.resize(600,600)
 
         self.th = Time()
         self.th.add.connect(self.test_add)
```

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/__init__.py` & `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg1.py` & `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg2.py` & `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg3.py` & `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg3.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg4.py` & `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg4.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg5.py` & `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg5.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg6.py` & `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg6.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg7.py` & `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/eg7.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/test.py` & `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis.py` & `PyQtGuiLib-2.7.20.11/tests/test_QssStyleAnalysis.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_SlideShow.py` & `PyQtGuiLib-2.7.20.11/tests/test_SlideShow.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,23 +33,34 @@
 
         # self.ss.setAutoSlideShow(True)
         # self.ss.setButtonsHide(True)
         self.ss.move(50,50)
         # self.ss.resize(600,200)
         self.test()  # 添加测试窗口
 
+        self.flag = True
         self.boyy.addWidget(self.ss)
 
         self.ss.changeWidget.connect(self.my_event)
 
     def my_event(self,index:int):
-        print("当前索引:",index)
+        pass
+        # print("当前索引:",index)
 
     def change(self):
-        self.ss.removeWidget(self.ss.getWidget(1))
+        # self.ss.removeWidget(self.ss.getWidget(0))
+        if self.flag:
+            self.pp = self.ss.popWidget(self.ss.getWidget(0))  # type:QWidget
+            self.pp.move(30,30)
+            self.pp.show()
+            self.flag =False
+        else:
+            self.flag=True
+            self.ss.insertWidget(0,self.pp)
+
 
     def test(self):
         t = QWidget()
         tl = QLabel("1")
         tl.setAlignment(qt.AlignCenter)
         lh = QHBoxLayout(t)
         btn1 = QPushButton("删除")
```

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_StyleLinker/eg1_QPushButton.py` & `PyQtGuiLib-2.7.20.11/tests/test_StyleLinker/eg1_QPushButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_StyleLinker/eg2_QLabel.py` & `PyQtGuiLib-2.7.20.11/tests/test_StyleLinker/eg2_QLabel.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/eg1.py` & `PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/eg1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/eg2.py` & `PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/eg2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/eg3.py` & `PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/eg3.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/eg4.py` & `PyQtGuiLib-2.7.20.11/tests/test_SuperPainter/eg4.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 # @software:PyCharm
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
     QApplication,
     sys,
     QWidget,
     QColor,
-    QPushButton
+    QPushButton,
+    QPoint
 )
 from PyQtGuiLib.styles import SuperPainter
 
 
 class Test(QWidget):
     def __init__(self):
         super().__init__()
@@ -27,38 +28,68 @@
         self.painter = SuperPainter()  # 创建一个画师对象,注意这个对象不要创建在paintEvent里面
 
         # 这个创建一个按钮,等下点击这个按钮来修改图形
         self.btn = QPushButton("修改图形",self)
         self.btn.move(200,50)
         self.btn.clicked.connect(self.updateDraw)
 
+        self.setMouseTracking(True)
+        self.cupos = QPoint(-1,-1)
+
+    def mousePressEvent(self, e):
+        myrect = self.painter.virtualObj("myrect")
+        myrect2 = self.painter.virtualObj("myrect2")
+        print("是否点击在myrect图形上",myrect.isClick(self.cupos))
+        print("是否点击在myrect2图形上",myrect2.isClick(self.cupos))
+        super().mousePressEvent(e)
+
+    def mouseMoveEvent(self, e):
+        self.cupos = e.pos()
+        myrect2 = self.painter.virtualObj("myrect2")
+        if myrect2.isClick(self.cupos):
+            myrect2.updateOpenAttr(openAttr={"color": "red", "width": 3})
+        else:
+            myrect2.updateOpenAttr(openAttr={"color": "green", "width": 3})
+        self.update()
+        super().mouseMoveEvent(e)
+
     # 修改图形事件
     def updateDraw(self):
         '''
             所有与虚拟对象有关的方法都在 self.painter.virtualObj() 这个下面
 
             几乎所有的虚拟对象方法的第一个参数都是 "虚拟对象名称",就像self一样
 
             这里用的两个方法:
                 getVirtualArgs() 获取当前图形的位置大小等信息
                 updateArgs() 修改当前图形的位置大小等信息
                 updateOpenAttr() 修改当前图形的属性
         '''
-        print(self.painter.virtualObj().getVirtualArgs("myrect"))
-        self.painter.virtualObj().updateArgs("myrect",20,20,100,100)
-        # 注意一下,目前版本中,这句修改属性的句话,必须在创建图形虚拟对象的有才可以修改,如果没有,这修改无效
-        self.painter.virtualObj().updateOpenAttr("myrect",openAttr={"color":"red"})
+        myrect=self.painter.virtualObj("myrect")
+        myrect.updateArgs(20,20,100,100)
+        myrect.updateOpenAttr(openAttr={"color":"red","width":3})
+        myrect.updateBrushAttr(brushAttr={"color":QColor("green")})
+
+
+        myrect2=self.painter.virtualObj("myrect2")
+        myrect2.scale(1.2)
+        # myrect2.setHide(True) # True隐藏图形
+        # myrect2.move(300,300)
+        # myrect2.updateOpenAttr(openAttr={"color":"red","width":3})
+        # myrect2.updateBrushAttr(brushAttr={"color":QColor("green")})
+
         self.update() # 这里必须调用一下,来刷新图形
 
     def paintEvent(self, QPaintEvent):
         self.painter.begin(self)
 
         # 创建一个 图形虚拟对象
         self.painter.drawRect(20, 20, 50, 50,openAttr={"color":"green"}, virtualObjectName="myrect")
-
+        self.painter.drawRect(200, 200, 50, 50,openAttr={"color":"green"}, virtualObjectName="myrect2")
+        self.painter.drawRoundedRect(10,300,150,80,openAttr={"c":"#00557f"})
         self.painter.end()
 
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
 
     win = Test()
```

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/test.py` & `PyQtGuiLib-2.7.20.11/tests/test_barset.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,103 @@
 # -*- coding:utf-8 -*-
-# @time:2023/4/1010:09
+# @time:2022/12/2316:33
 # @author:LX
-# @file:test.py
+# @file:test_barset.py
 # @software:PyCharm
+
+'''
+
+    进度条集合测试
+'''
+
 from PyQtGuiLib.header import (
-    QApplication,
     PYQT_VERSIONS,
     sys,
+    QApplication,
     QWidget,
-    QPainter,
-    QPen,
-    QBrush,
-    QFont,
-    qt,
-    Qt,
+    QThread,
+    Signal,
+    QHBoxLayout,
     QColor,
-    QPaintEvent,
-    QPushButton,
-    QRect
+    QSlider
 )
 
-from PyQtGuiLib.animation import Animation
-from PyQtGuiLib.styles import SuperPainter
+from PyQtGuiLib.core.progressBar import WaterBar
+from PyQtGuiLib.core.progressBar import CircularBar
+from PyQtGuiLib.core.progressBar import LoadBar
+from PyQtGuiLib.core.progressBar import GradientBar
 
-class Test(QWidget):
+
+class DurationTimeThread(QThread):
+    added = Signal(int)
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
-        self.resize(600,600)
-        self.painter = SuperPainter()
-        self.btn = QPushButton("变大",self)
-        self.btn2 = QPushButton("变小",self)
-        self.btn.move(300,50)
-        self.btn2.move(380,50)
-        self.btn.clicked.connect(lambda :self.test_update(1.3))
-        self.btn2.clicked.connect(lambda :self.test_update(0.8))
-
-        # self.ani = Animation(self)
-
-    def test_update(self,v):
-        rrent = self.painter.virtualObj("rrent")
-        rrent.scale(v)
-
-        # rrent.move(200,200)
-
-        # print(rrent.type())
-        # print(rrent.getVirtualObjectAttr())
-        # # rrent.updateArgs(50,50,100,100,3,3)
-        # # rrent.updateArgs(50,50,100,100)
-        # rrent.updateOpenAttr(openAttr={"color":"red"})
-        # rrent.updateBrushAttr(brushAttr={"color":"blue"})
-        self.update()
-
-    def paintEvent(self, e:QPaintEvent) -> None:
-        self.painter.begin(self)
-        self.painter.setRenderHints(qt.Antialiasing | qt.SmoothPixmapTransform | qt.TextAntialiasing)
-        # self.painter.drawRoundedRect(50,50,50,50,5,5,virtualObjectName="rrent")
-        self.painter.drawRect(50,50,50,50,virtualObjectName="rrent")
 
-        self.painter.end()
 
-'''
-    修复说明
-    重新优化结构,将虚拟对象图形类,拆分为(虚拟对象图形管理类,虚拟对象图形类)
-'''
+    def run(self) -> None:
+        n=1
+        while True:
+            self.added.emit(n)
+            n+=1
+            self.msleep(100)
+            if n == 100+1:
+                print("完成")
+                break
 
-if __name__ == '__main__':
-    app = QApplication(sys.argv)
+class TestPullOverWidget(QWidget):
+    def __init__(self,*args,**kwargs):
+        super().__init__(*args,**kwargs)
+        self.resize(800,500)
 
-    win = Test()
+        self.setObjectName("test")
+#         self.setStyleSheet('''
+# #test{
+# background-color: rgb(0, 0, 0);
+# }
+#         ''')
+
+        # self.vboy = QHBoxLayout(self)
+
+        self.waterbar = WaterBar(self)
+        self.waterbar.move(100,250)
+
+        # 加载进度条
+        self.loadbar = LoadBar(self)
+        self.loadbar.move(250,100)
+        self.loadbar.resize(350,45)
+
+
+        # 圆环进度条
+        self.cir = CircularBar(self)
+        self.cir.resize(120, 120)
+        self.cir.setVariableLineSegment(CircularBar.Double)
+        self.cir.setOuterStyle(CircularBar.CustomDashLine)
+        self.cir.setOuterDashPattern([2, 3, 5, 6])
+        self.cir.setInnerStyle(CircularBar.DashLine)
+        self.cir.setTextSize(15)
+        self.cir.move(50, 50)
+
+        # self.vboy.addWidget(self.waterbar)
+        # self.vboy.addWidget(self.loadbar)
+        # self.vboy.addWidget(self.cir)
+        #
+        self.th = DurationTimeThread()
+        self.th.added.connect(self.test)
+        self.th.start()
+
+
+    def test(self, n):
+        self.cir.setValue(n)
+        self.loadbar.setValue(n)
+        self.waterbar.setValue(n)
 
+
+
+if __name__ == '__main__':
+    app = QApplication(sys.argv)
+    win = TestPullOverWidget()
     win.show()
 
-    if PYQT_VERSIONS in ["PyQt6","PySide6"]:
+    if PYQT_VERSIONS in ["PyQt6", "PySide6"]:
         sys.exit(app.exec())
     else:
-        sys.exit(app.exec_())
+        sys.exit(app.exec_())
```

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_barset.py` & `PyQtGuiLib-2.7.20.11/tests/test_templateWindow/test_listTemplateWindow.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,103 +1,102 @@
 # -*- coding:utf-8 -*-
-# @time:2022/12/2316:33
+# @time:2023/4/1112:42
 # @author:LX
-# @file:test_barset.py
+# @file:test_listTemplateWindow.py
 # @software:PyCharm
-
-'''
-
-    进度条集合测试
-'''
-
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
-    sys,
     QApplication,
+    sys,
     QWidget,
-    QThread,
-    Signal,
-    QHBoxLayout,
-    QColor,
-    QSlider
+    QLabel,
+    Qt
 )
 
-from PyQtGuiLib.core.progressBar import WaterBar
-from PyQtGuiLib.core.progressBar import CircularBar
-from PyQtGuiLib.core.progressBar import LoadBar
-from PyQtGuiLib.core.progressBar import GradientBar
+from random import randint
+from PyQtGuiLib.templateWindow import ListTemplateWindow
 
+'''
+    测试 实际使用 模板窗口
+'''
 
-class DurationTimeThread(QThread):
-    added = Signal(int)
-    def __init__(self,*args,**kwargs):
-        super().__init__(*args,**kwargs)
-
-
-    def run(self) -> None:
-        n=1
-        while True:
-            self.added.emit(n)
-            n+=1
-            self.msleep(100)
-            if n == 100+1:
-                print("完成")
-                break
-
-class TestPullOverWidget(QWidget):
+class myWidget(ListTemplateWindow):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
-        self.resize(800,500)
-
-        self.setObjectName("test")
-#         self.setStyleSheet('''
-# #test{
-# background-color: rgb(0, 0, 0);
-# }
-#         ''')
-
-        self.vboy = QHBoxLayout(self)
-
-        self.waterbar = WaterBar(self)
-        self.waterbar.move(100,250)
-
-        # 加载进度条
-        self.loadbar = LoadBar(self)
-        self.loadbar.move(250,100)
-        self.loadbar.resize(350,45)
-
-
-        # 圆环进度条
-        self.cir = CircularBar(self)
-        self.cir.resize(120, 120)
-        self.cir.setVariableLineSegment(CircularBar.Double)
-        self.cir.setOuterStyle(CircularBar.CustomDashLine)
-        self.cir.setOuterDashPattern([2, 3, 5, 6])
-        self.cir.setInnerStyle(CircularBar.DashLine)
-        self.cir.setTextSize(15)
-        self.cir.move(50, 50)
-
-        self.vboy.addWidget(self.waterbar)
-        self.vboy.addWidget(self.loadbar)
-        self.vboy.addWidget(self.cir)
-        #
-        self.th = DurationTimeThread()
-        self.th.added.connect(self.test)
-        self.th.start()
-
-
-    def test(self, n):
-        self.cir.setValue(n)
-        self.loadbar.setValue(n)
-        self.waterbar.setValue(n)
-
 
+        # 添加菜单
+        self.addMenu({
+            "text": "测试",
+            "call": self.test,
+        })
+        self.addMenu(
+            {
+                "text":"隐藏第二页(测试功能)",
+                "call":self.test_hide
+            }
+        )
+
+        # 添加头像
+        self.setHeadPicture(r"D:\code\PyQtGuiLib\tests\temp_image\python1.png")
+
+        # 添加页面
+        self.addItem("首页",self.frist_page(),r"D:\code\PyQtGuiLib\tests\temp_image\python1.png")
+        self.addItem("第二页",self.two_page(),r"D:\code\PyQtGuiLib\tests\temp_image\python1.png")
+        self.addItem("第三页",self.three_page(),r"D:\code\PyQtGuiLib\tests\temp_image\python1.png")
+
+        # 头部窗口
+        self.addHeadWidget(self.headWidget())
+
+    def test_hide(self):
+        if self.listWidget.item(1).isHidden():
+            self.setHideItem(1,False)
+        else:
+            self.setHideItem(1)
+
+    def test(self):
+        print("测试回调函数")
+
+    def frist_page(self):
+        widget = QLabel("我是首页")
+        widget.setAlignment(Qt.AlignCenter)
+        widget.setStyleSheet('''
+background-color: rgb(229, 229, 229);
+font: 22pt "黑体";
+        ''')
+        return widget
+
+    def three_page(self):
+        widget = QLabel("第三页")
+        widget.setAlignment(Qt.AlignCenter)
+        widget.setStyleSheet('''
+background-color: rgb(100, 100, 45);
+font: 22pt "黑体";
+        ''')
+        return widget
+
+    def two_page(self):
+        widget = QLabel("我是第二页")
+        widget.setAlignment(Qt.AlignCenter)
+        widget.setStyleSheet('''
+        background-color: #ffd997;
+        font: 22pt "黑体";
+                ''')
+        return widget
+
+    def headWidget(self):
+        widget = QLabel("头部窗口")
+        widget.setAlignment(Qt.AlignCenter)
+        widget.setStyleSheet('''
+        font: 22pt "黑体";
+                ''')
+        return widget
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
-    win = TestPullOverWidget()
+
+    win = myWidget()
     win.show()
 
-    if PYQT_VERSIONS in ["PyQt6", "PySide6"]:
+    if PYQT_VERSIONS in ["PyQt6","PySide6"]:
         sys.exit(app.exec())
     else:
-        sys.exit(app.exec_())
+        sys.exit(app.exec_())
```

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_circularBar.py` & `PyQtGuiLib-2.7.20.11/tests/test_gradientBar.py`

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

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_colorPalette.py` & `PyQtGuiLib-2.7.20.11/tests/test_colorPalette.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_comboBox.py` & `PyQtGuiLib-2.7.20.11/tests/test_comboBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_dynamicTLine.py` & `PyQtGuiLib-2.7.20.11/tests/test_dynamicTLine.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_flowLayot.py` & `PyQtGuiLib-2.7.20.11/tests/test_flowLayot.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_listWidget.py` & `PyQtGuiLib-2.7.20.11/tests/test_listWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_loadbar.py` & `PyQtGuiLib-2.7.20.11/tests/test_loadbar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_no_border.py` & `PyQtGuiLib-2.7.20.11/tests/test_no_border.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_no_border_pullOver.py` & `PyQtGuiLib-2.7.20.11/tests/test_no_border_pullOver.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_pullOverWidget.py` & `PyQtGuiLib-2.7.20.11/tests/test_pullOverWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_qssFile/test.py` & `PyQtGuiLib-2.7.20.11/tests/test_qssFile/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_rollWidget.py` & `PyQtGuiLib-2.7.20.11/tests/test_rollWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_slider.py` & `PyQtGuiLib-2.7.20.11/tests/test_slider.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_statusBar.py` & `PyQtGuiLib-2.7.20.11/tests/test_statusBar.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 # @author:LX
 # @file:test_gradientBar.py
 # @software:PyCharm
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
     sys,
     QApplication,
+    QWidget
 )
 
 from abandonCase.widgets import (
     BorderlessWidget,     # 无边框矩形QWidget窗口
     )
 
 from abandonCase.widgets import StatusBar
 from PyQtGuiLib.core.progressBar import GradientBar
 
 '''
+    这个例子无法运行 2023.4.13 号
     测试 状态栏
 '''
 
 class TestStatusBar(BorderlessWidget):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
         self.resize(800,500)
```

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_styles.py` & `PyQtGuiLib-2.7.20.11/tests/test_styles.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_switchButton.py` & `PyQtGuiLib-2.7.20.11/tests/test_switchButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_templateWindow/test_listTemplateWindow.py` & `PyQtGuiLib-2.7.20.11/PyQtGuiLib/listTree.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,108 @@
 # -*- coding:utf-8 -*-
-# @time:2023/4/1112:42
+# @time:2023/4/158:55
 # @author:LX
-# @file:test_listTemplateWindow.py
+# @file:listTree.py
 # @software:PyCharm
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
     QApplication,
     sys,
     QWidget,
-    QLabel,
+    QPainter,
+    QFont,
+    QColor,
+    QSize,
+    QPaintEvent,
+    QRect,
+    Qt,
+    textSize,
+    QPoint,
+    QToolButton,
+    QAction,
+    QMenu,
     Qt
 )
 
-from random import randint
-from PyQtGuiLib.templateWindow import ListTemplateWindow
 
-'''
-    测试 实际使用 模板窗口
-'''
 
-class myWidget(ListTemplateWindow):
+class ListTree(QWidget):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
+        self.resize(300,600)
+
+        # 默认节点高度
+        self.__item_height = 55
+        self.__margin = 5
+
+        self.__items = [
+            {"bg":{
+            "rect": QRect(5, 5, -1, 50)
+           },
+           "text":{
+                "text":"hello",
+               "pos":QPoint(-1,25)
+        }},
+            {"bg":{
+            "rect": QRect(5,5*2+50,-1,50)
+           },
+           "text":{
+                "text":"hello",
+               "pos":QPoint(-1,75)
+        }}]
+
+    def count(self)->int:
+        return len(self.__items)
+
+    def addItem(self,text:str):
+        if self.count() == 0:
+            self.__items.append({
+
+            })
+        elif self.count() > 0:
+            pass
+
+    def addItems(self,data:list):
+        for info in data:
+            pass
+
+
+
+    def paintEvent(self, e: QPaintEvent) -> None:
+        painter = QPainter(self)
+
+        for item in self.__items:
+            rect = item["bg"]["rect"] # type:QRect
+            text = item["text"]["text"] # type:str
+            t_pos = item["text"]["pos"] # type:QPoint
+
+            # 绘制背景
+            painter.setPen(Qt.NoPen)
+            painter.setBrush(QColor("#55ffff"))
+            x,y = rect.x(),rect.y()
+            if rect.width() == -1:
+                w = self.width()-x*2
+            h = rect.height()
+            painter.drawRoundedRect(x,y,w,h,5,5)
+
+            # 绘制文本
+            painter.setPen(QColor("#000"))
+            f = QFont(text)
+            fsize = textSize(f,text)
+            fw,fh = fsize.width(),fsize.height()
+            x = w//2-fw//2
+            y = t_pos.y()+fh//2+5
+            painter.drawText(x,y,text)
+
+        painter.end()
 
-        # 添加菜单
-        self.addMenu({
-            "text": "测试",
-            "call": self.test,
-        })
-
-        # 添加头像
-        self.setHeadPicture(r"D:\code\PyQtGuiLib\tests\temp_image\python1.png")
-
-        # 添加页面
-        self.addItem("首页",self.frist_page(),r"D:\code\PyQtGuiLib\tests\temp_image\python1.png")
-        self.addItem("第二页",self.two_page(),r"D:\code\PyQtGuiLib\tests\temp_image\python1.png")
-
-        # 头部窗口
-        self.addHeadWidget(self.headWidget())
-
-    def test(self):
-        print("测试回调函数")
-
-    def frist_page(self):
-        widget = QLabel("我是首页")
-        widget.setAlignment(Qt.AlignCenter)
-        widget.setStyleSheet('''
-background-color: rgb(229, 229, 229);
-font: 22pt "黑体";
-        ''')
-        return widget
-
-    def two_page(self):
-        widget = QLabel("我是第二页")
-        widget.setAlignment(Qt.AlignCenter)
-        widget.setStyleSheet('''
-        background-color: #ffd997;
-        font: 22pt "黑体";
-                ''')
-        return widget
-
-    def headWidget(self):
-        widget = QLabel("头部窗口")
-        widget.setAlignment(Qt.AlignCenter)
-        widget.setStyleSheet('''
-        font: 22pt "黑体";
-                ''')
-        return widget
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
 
-    win = myWidget()
+    win = ListTree()
     win.show()
 
     if PYQT_VERSIONS in ["PyQt6","PySide6"]:
         sys.exit(app.exec())
     else:
-        sys.exit(app.exec_())
+        sys.exit(app.exec_())
```

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_toolList.py` & `PyQtGuiLib-2.7.20.11/tests/test_toolList.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.7.18.11/tests/test_waterBar.py` & `PyQtGuiLib-2.7.20.11/tests/test_waterBar.py`

 * *Files identical despite different names*

