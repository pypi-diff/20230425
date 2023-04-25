# Comparing `tmp/feffery_antd_components-0.2.2.tar.gz` & `tmp/feffery_antd_components-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feffery_antd_components-0.2.2.tar", last modified: Fri Apr 21 05:58:43 2023, max compression
+gzip compressed data, was "feffery_antd_components-0.2.3.tar", last modified: Tue Apr 25 07:16:07 2023, max compression
```

## Comparing `feffery_antd_components-0.2.2.tar` & `feffery_antd_components-0.2.3.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 05:58:43.791794 feffery_antd_components-0.2.2/
--rw-rw-rw-   0        0        0     1087 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      288 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      346 2023-04-21 05:58:43.791794 feffery_antd_components-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2301 2023-04-18 12:57:49.000000 feffery_antd_components-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 05:58:43.784062 feffery_antd_components-0.2.2/feffery_antd_components/
--rw-rw-rw-   0        0        0     3312 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdAccordion.py
--rw-rw-rw-   0        0        0     2539 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdAccordionItem.py
--rw-rw-rw-   0        0        0     2006 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdAffix.py
--rw-rw-rw-   0        0        0     2627 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdAlert.py
--rw-rw-rw-   0        0        0     2314 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdAnchor.py
--rw-rw-rw-   0        0        0     2586 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdAvatar.py
--rw-rw-rw-   0        0        0     2611 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdAvatarGroup.py
--rw-rw-rw-   0        0        0     1892 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdBackTop.py
--rw-rw-rw-   0        0        0     2730 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdBadge.py
--rw-rw-rw-   0        0        0     2313 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdBreadcrumb.py
--rw-rw-rw-   0        0        0     3218 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdButton.py
--rw-rw-rw-   0        0        0     3356 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdCalendar.py
--rw-rw-rw-   0        0        0     2991 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdCard.py
--rw-rw-rw-   0        0        0     1924 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdCardGrid.py
--rw-rw-rw-   0        0        0     2490 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdCarousel.py
--rw-rw-rw-   0        0        0     5312 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdCascader.py
--rw-rw-rw-   0        0        0     3615 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdCheckCard.py
--rw-rw-rw-   0        0        0     3694 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdCheckCardGroup.py
--rw-rw-rw-   0        0        0     3303 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdCheckbox.py
--rw-rw-rw-   0        0        0     3388 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdCheckboxGroup.py
--rw-rw-rw-   0        0        0     3890 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdCol.py
--rw-rw-rw-   0        0        0     3755 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdCollapse.py
--rw-rw-rw-   0        0        0     3987 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdComment.py
--rw-rw-rw-   0        0        0     2076 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdConfigProvider.py
--rw-rw-rw-   0        0        0     1824 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdContent.py
--rw-rw-rw-   0        0        0     2109 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdCopyText.py
--rw-rw-rw-   0        0        0     2497 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdCountdown.py
--rw-rw-rw-   0        0        0     2530 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdCustomSkeleton.py
--rw-rw-rw-   0        0        0     5353 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdDatePicker.py
--rw-rw-rw-   0        0        0     5418 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdDateRangePicker.py
--rw-rw-rw-   0        0        0     2263 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdDescriptionItem.py
--rw-rw-rw-   0        0        0     2745 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdDescriptions.py
--rw-rw-rw-   0        0        0     2676 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdDivider.py
--rw-rw-rw-   0        0        0     6239 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdDraggerUpload.py
--rw-rw-rw-   0        0        0     3109 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdDrawer.py
--rw-rw-rw-   0        0        0     3612 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdDropdown.py
--rw-rw-rw-   0        0        0     2250 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdEmpty.py
--rw-rw-rw-   0        0        0     1820 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdFooter.py
--rw-rw-rw-   0        0        0     2552 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdForm.py
--rw-rw-rw-   0        0        0     3351 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdFormItem.py
--rw-rw-rw-   0        0        0     1820 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdHeader.py
--rw-rw-rw-   0        0        0     1829 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdIcon.py
--rw-rw-rw-   0        0        0     5562 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdImage.py
--rw-rw-rw-   0        0        0     5674 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdInput.py
--rw-rw-rw-   0        0        0     5082 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdInputNumber.py
--rw-rw-rw-   0        0        0     1820 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdLayout.py
--rw-rw-rw-   0        0        0     3094 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdMentions.py
--rw-rw-rw-   0        0        0     4059 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdMenu.py
--rw-rw-rw-   0        0        0     2110 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdMessage.py
--rw-rw-rw-   0        0        0     5365 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdModal.py
--rw-rw-rw-   0        0        0     2417 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdNotification.py
--rw-rw-rw-   0        0        0     2555 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdPageHeader.py
--rw-rw-rw-   0        0        0     4592 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdPagination.py
--rw-rw-rw-   0        0        0     2752 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdParagraph.py
--rw-rw-rw-   0        0        0     2002 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdPasteImage.py
--rw-rw-rw-   0        0        0     6346 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdPictureUpload.py
--rw-rw-rw-   0        0        0     4807 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdPopconfirm.py
--rw-rw-rw-   0        0        0     3562 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdPopover.py
--rw-rw-rw-   0        0        0     2869 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdPopupCard.py
--rw-rw-rw-   0        0        0     3352 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdProgress.py
--rw-rw-rw-   0        0        0     4008 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdRadioGroup.py
--rw-rw-rw-   0        0        0     3488 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdRate.py
--rw-rw-rw-   0        0        0     2181 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdResult.py
--rw-rw-rw-   0        0        0     2068 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdRibbon.py
--rw-rw-rw-   0        0        0     2489 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdRow.py
--rw-rw-rw-   0        0        0     3715 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdSegmented.py
--rw-rw-rw-   0        0        0     3598 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdSegmentedColoring.py
--rw-rw-rw-   0        0        0     7197 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdSelect.py
--rw-rw-rw-   0        0        0     2846 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdSider.py
--rw-rw-rw-   0        0        0     3193 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdSkeleton.py
--rw-rw-rw-   0        0        0     1934 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdSkeletonAvatar.py
--rw-rw-rw-   0        0        0     2017 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdSkeletonButton.py
--rw-rw-rw-   0        0        0     1604 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdSkeletonImage.py
--rw-rw-rw-   0        0        0     1808 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdSkeletonInput.py
--rw-rw-rw-   0        0        0     4230 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdSlider.py
--rw-rw-rw-   0        0        0     2389 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdSpace.py
--rw-rw-rw-   0        0        0     2931 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdSpin.py
--rw-rw-rw-   0        0        0     2853 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdSpoiler.py
--rw-rw-rw-   0        0        0     2607 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdStatistic.py
--rw-rw-rw-   0        0        0     3223 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdSteps.py
--rw-rw-rw-   0        0        0     3651 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdSwitch.py
--rw-rw-rw-   0        0        0     2314 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdTabPane.py
--rw-rw-rw-   0        0        0    18807 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdTable.py
--rw-rw-rw-   0        0        0     5266 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdTabs.py
--rw-rw-rw-   0        0        0     1950 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdTag.py
--rw-rw-rw-   0        0        0     2820 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdText.py
--rw-rw-rw-   0        0        0     4722 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdTimePicker.py
--rw-rw-rw-   0        0        0     4787 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdTimeRangePicker.py
--rw-rw-rw-   0        0        0     2750 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdTimeline.py
--rw-rw-rw-   0        0        0     2900 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdTitle.py
--rw-rw-rw-   0        0        0     3445 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdTooltip.py
--rw-rw-rw-   0        0        0     4586 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdTransfer.py
--rw-rw-rw-   0        0        0     5301 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdTree.py
--rw-rw-rw-   0        0        0     6685 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdTreeSelect.py
--rw-rw-rw-   0        0        0     5634 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdUpload.py
--rw-rw-rw-   0        0        0     2397 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/AntdWatermark.py
--rw-rw-rw-   0        0        0     1571 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.2/feffery_antd_components/__init__.py
--rw-rw-rw-   0        0        0     5752 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/_imports_.py
--rw-rw-rw-   0        0        0  3770463 2023-04-21 05:58:36.000000 feffery_antd_components-0.2.2/feffery_antd_components/feffery_antd_components.min.js
--rw-rw-rw-   0        0        0   623059 2023-04-21 05:58:42.000000 feffery_antd_components-0.2.2/feffery_antd_components/metadata.json
--rw-rw-rw-   0        0        0     3031 2023-04-21 05:58:38.000000 feffery_antd_components-0.2.2/feffery_antd_components/package-info.json
-drwxrwxrwx   0        0        0        0 2023-04-21 05:58:43.790524 feffery_antd_components-0.2.2/feffery_antd_components.egg-info/
--rw-rw-rw-   0        0        0      346 2023-04-21 05:58:43.000000 feffery_antd_components-0.2.2/feffery_antd_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4341 2023-04-21 05:58:43.000000 feffery_antd_components-0.2.2/feffery_antd_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 05:58:43.000000 feffery_antd_components-0.2.2/feffery_antd_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 05:58:43.000000 feffery_antd_components-0.2.2/feffery_antd_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-21 05:58:43.000000 feffery_antd_components-0.2.2/feffery_antd_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3031 2023-04-21 01:35:02.000000 feffery_antd_components-0.2.2/package.json
--rw-rw-rw-   0        0        0       42 2023-04-21 05:58:43.792808 feffery_antd_components-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      715 2023-04-21 01:19:57.000000 feffery_antd_components-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:16:07.108703 feffery_antd_components-0.2.3/
+-rw-rw-rw-   0        0        0     1087 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      288 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      346 2023-04-25 07:16:07.107653 feffery_antd_components-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2301 2023-04-25 07:15:50.000000 feffery_antd_components-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 07:16:07.101633 feffery_antd_components-0.2.3/feffery_antd_components/
+-rw-rw-rw-   0        0        0     3328 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdAccordion.py
+-rw-rw-rw-   0        0        0     2539 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdAccordionItem.py
+-rw-rw-rw-   0        0        0     2006 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdAffix.py
+-rw-rw-rw-   0        0        0     2627 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdAlert.py
+-rw-rw-rw-   0        0        0     2314 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdAnchor.py
+-rw-rw-rw-   0        0        0     2586 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdAvatar.py
+-rw-rw-rw-   0        0        0     2611 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdAvatarGroup.py
+-rw-rw-rw-   0        0        0     1892 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdBackTop.py
+-rw-rw-rw-   0        0        0     2730 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdBadge.py
+-rw-rw-rw-   0        0        0     2313 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdBreadcrumb.py
+-rw-rw-rw-   0        0        0     3218 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdButton.py
+-rw-rw-rw-   0        0        0     3356 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCalendar.py
+-rw-rw-rw-   0        0        0     2991 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCard.py
+-rw-rw-rw-   0        0        0     1924 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCardGrid.py
+-rw-rw-rw-   0        0        0     2490 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCarousel.py
+-rw-rw-rw-   0        0        0     5312 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCascader.py
+-rw-rw-rw-   0        0        0     3615 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCheckCard.py
+-rw-rw-rw-   0        0        0     3694 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCheckCardGroup.py
+-rw-rw-rw-   0        0        0     3303 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCheckbox.py
+-rw-rw-rw-   0        0        0     3388 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCheckboxGroup.py
+-rw-rw-rw-   0        0        0     3890 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCol.py
+-rw-rw-rw-   0        0        0     3763 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCollapse.py
+-rw-rw-rw-   0        0        0     3987 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdComment.py
+-rw-rw-rw-   0        0        0     2076 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdConfigProvider.py
+-rw-rw-rw-   0        0        0     1824 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdContent.py
+-rw-rw-rw-   0        0        0     2109 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCopyText.py
+-rw-rw-rw-   0        0        0     2497 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCountdown.py
+-rw-rw-rw-   0        0        0     2530 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCustomSkeleton.py
+-rw-rw-rw-   0        0        0     5353 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdDatePicker.py
+-rw-rw-rw-   0        0        0     5418 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdDateRangePicker.py
+-rw-rw-rw-   0        0        0     2263 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdDescriptionItem.py
+-rw-rw-rw-   0        0        0     2745 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdDescriptions.py
+-rw-rw-rw-   0        0        0     2676 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdDivider.py
+-rw-rw-rw-   0        0        0     6274 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdDraggerUpload.py
+-rw-rw-rw-   0        0        0     3109 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdDrawer.py
+-rw-rw-rw-   0        0        0     3744 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdDropdown.py
+-rw-rw-rw-   0        0        0     2250 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdEmpty.py
+-rw-rw-rw-   0        0        0     1820 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdFooter.py
+-rw-rw-rw-   0        0        0     2552 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdForm.py
+-rw-rw-rw-   0        0        0     3351 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdFormItem.py
+-rw-rw-rw-   0        0        0     1820 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdHeader.py
+-rw-rw-rw-   0        0        0     1829 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdIcon.py
+-rw-rw-rw-   0        0        0     5562 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdImage.py
+-rw-rw-rw-   0        0        0     5674 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdInput.py
+-rw-rw-rw-   0        0        0     5082 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdInputNumber.py
+-rw-rw-rw-   0        0        0     1820 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdLayout.py
+-rw-rw-rw-   0        0        0     3094 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdMentions.py
+-rw-rw-rw-   0        0        0     4059 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdMenu.py
+-rw-rw-rw-   0        0        0     2110 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdMessage.py
+-rw-rw-rw-   0        0        0     5365 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdModal.py
+-rw-rw-rw-   0        0        0     2417 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdNotification.py
+-rw-rw-rw-   0        0        0     2555 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdPageHeader.py
+-rw-rw-rw-   0        0        0     4592 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdPagination.py
+-rw-rw-rw-   0        0        0     2752 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdParagraph.py
+-rw-rw-rw-   0        0        0     2002 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdPasteImage.py
+-rw-rw-rw-   0        0        0     6381 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdPictureUpload.py
+-rw-rw-rw-   0        0        0     4807 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdPopconfirm.py
+-rw-rw-rw-   0        0        0     3562 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdPopover.py
+-rw-rw-rw-   0        0        0     2869 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdPopupCard.py
+-rw-rw-rw-   0        0        0     3352 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdProgress.py
+-rw-rw-rw-   0        0        0     4008 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdRadioGroup.py
+-rw-rw-rw-   0        0        0     3488 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdRate.py
+-rw-rw-rw-   0        0        0     2181 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdResult.py
+-rw-rw-rw-   0        0        0     2068 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdRibbon.py
+-rw-rw-rw-   0        0        0     2489 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdRow.py
+-rw-rw-rw-   0        0        0     3715 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSegmented.py
+-rw-rw-rw-   0        0        0     3598 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSegmentedColoring.py
+-rw-rw-rw-   0        0        0     7197 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSelect.py
+-rw-rw-rw-   0        0        0     2846 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSider.py
+-rw-rw-rw-   0        0        0     3193 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeleton.py
+-rw-rw-rw-   0        0        0     1934 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeletonAvatar.py
+-rw-rw-rw-   0        0        0     2017 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeletonButton.py
+-rw-rw-rw-   0        0        0     1604 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeletonImage.py
+-rw-rw-rw-   0        0        0     1808 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeletonInput.py
+-rw-rw-rw-   0        0        0     4230 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSlider.py
+-rw-rw-rw-   0        0        0     2389 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSpace.py
+-rw-rw-rw-   0        0        0     2931 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSpin.py
+-rw-rw-rw-   0        0        0     2853 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSpoiler.py
+-rw-rw-rw-   0        0        0     2607 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdStatistic.py
+-rw-rw-rw-   0        0        0     3223 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSteps.py
+-rw-rw-rw-   0        0        0     3651 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSwitch.py
+-rw-rw-rw-   0        0        0     2314 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTabPane.py
+-rw-rw-rw-   0        0        0    19271 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTable.py
+-rw-rw-rw-   0        0        0     5266 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTabs.py
+-rw-rw-rw-   0        0        0     1950 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTag.py
+-rw-rw-rw-   0        0        0     2820 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdText.py
+-rw-rw-rw-   0        0        0     4722 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTimePicker.py
+-rw-rw-rw-   0        0        0     4787 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTimeRangePicker.py
+-rw-rw-rw-   0        0        0     2750 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTimeline.py
+-rw-rw-rw-   0        0        0     2900 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTitle.py
+-rw-rw-rw-   0        0        0     3445 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTooltip.py
+-rw-rw-rw-   0        0        0     4586 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTransfer.py
+-rw-rw-rw-   0        0        0     5301 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTree.py
+-rw-rw-rw-   0        0        0     6685 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTreeSelect.py
+-rw-rw-rw-   0        0        0     5669 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdUpload.py
+-rw-rw-rw-   0        0        0     2397 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdWatermark.py
+-rw-rw-rw-   0        0        0     1571 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.3/feffery_antd_components/__init__.py
+-rw-rw-rw-   0        0        0     5752 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/_imports_.py
+-rw-rw-rw-   0        0        0  3771264 2023-04-25 07:16:00.000000 feffery_antd_components-0.2.3/feffery_antd_components/feffery_antd_components.min.js
+-rw-rw-rw-   0        0        0   624550 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/metadata.json
+-rw-rw-rw-   0        0        0     3031 2023-04-25 07:16:01.000000 feffery_antd_components-0.2.3/feffery_antd_components/package-info.json
+drwxrwxrwx   0        0        0        0 2023-04-25 07:16:07.106392 feffery_antd_components-0.2.3/feffery_antd_components.egg-info/
+-rw-rw-rw-   0        0        0      346 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4341 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3031 2023-04-24 06:18:25.000000 feffery_antd_components-0.2.3/package.json
+-rw-rw-rw-   0        0        0       42 2023-04-25 07:16:07.108703 feffery_antd_components-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      715 2023-04-25 07:15:34.000000 feffery_antd_components-0.2.3/setup.py
```

### Comparing `feffery_antd_components-0.2.2/LICENSE` & `feffery_antd_components-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/README.md` & `feffery_antd_components-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/CNFeffery/feffery-antd-components.svg)](http://isitmaintained.com/project/CNFeffery/feffery-antd-components "Average time to resolve an issue")
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/CNFeffery/feffery-antd-components.svg)](http://isitmaintained.com/project/CNFeffery/feffery-antd-components "Percentage of issues still open")
 
 </div>
 
 简体中文 | [English](./README-en_US.md)
 
-`feffery-components`计划子项目，`Plotly Dash`第三方组件库，基于`Antd`，将超多具有丰富功能的通用网页常用交互组件引入`Dash`的生态中 🥳，最新稳定版本：`0.2.1`
+`feffery-components`计划子项目，`Plotly Dash`第三方组件库，基于`Antd`，将超多具有丰富功能的通用网页常用交互组件引入`Dash`的生态中 🥳，最新稳定版本：`0.2.3`
 
 ## 1 最新版本安装方式
 
 ```bash
 pip install feffery-antd-components -U
 ```
```

#### html2text {}

```diff
@@ -12,15 +12,15 @@
  components "Average time to resolve an issue") [![Percentage of issues still
       open](http://isitmaintained.com/badge/open/CNFeffery/feffery-antd-
   components.svg)](http://isitmaintained.com/project/CNFeffery/feffery-antd-
                  components "Percentage of issues still open")
 ç®ä½ä¸­æ | [English](./README-en_US.md) `feffery-
 components`è®¡åå­é¡¹ç®ï¼`Plotly
 Dash`ç¬¬ä¸æ¹ç»ä»¶åºï¼åºäº`Antd`ï¼å°è¶å¤å·æä¸°å¯åè½çéç¨ç½é¡µå¸¸ç¨äº¤äºç»ä»¶å¼å¥`Dash`ççæä¸­
-ð¥³ï¼ææ°ç¨³å®çæ¬ï¼`0.2.1` ## 1 ææ°çæ¬å®è£æ¹å¼ ```bash pip
+ð¥³ï¼ææ°ç¨³å®çæ¬ï¼`0.2.3` ## 1 ææ°çæ¬å®è£æ¹å¼ ```bash pip
 install feffery-antd-components -U ``` ## 2 ææ°é¢åå¸çæ¬å®è£æ¹å¼
 ```bash pip install feffery-antd-components --pre -U ``` ## 3 éæèµæº CDN
 å éæ¹æ³ ```Python # édebugæ¨¡å¼ä¸å¯¹Dash
 ()ä¼ å¥åæ°serve_locally=Falseä¼å¼ºå¶æµè§å¨ç«¯ä»unpkg
 cdnå è½½åä¸ªä¾èµç #
 xxx.min.jsç­éæèµæºï¼ä»èé¿åå ç¨æå¡å¨å¸¦å®½ï¼éåä¸­å°åç«ç¹å éè®¿é®
 app = dash.Dash(serve_locally=False) ``` ## 4 å¨çº¿ææ¡£ ææ¡£å°å ## 5
```

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdAccordion.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdAccordion.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 - activeKey (string | list of strings | number | list of numbers; optional)
 
 - bordered (boolean; default True)
 
 - className (string | dict; optional)
 
-- collapsible (a value equal to: 'header', 'disabled'; optional)
+- collapsible (a value equal to: 'header', 'disabled', 'icon'; optional)
 
 - defaultActiveKey (string | list of strings | number | list of numbers; optional)
 
 - expandIconPosition (a value equal to: 'left', 'right'; default 'left')
 
 - ghost (boolean; default False)
 
@@ -33,15 +33,15 @@
 
     `items` is a list of dicts with keys:
 
     - children (a list of or a singular dash component, string or number; optional)
 
     - className (string | dict; optional)
 
-    - collapsible (a value equal to: 'header', 'disabled'; optional)
+    - collapsible (a value equal to: 'header', 'disabled', 'icon'; optional)
 
     - extra (a list of or a singular dash component, string or number; optional)
 
     - forceRender (boolean; optional)
 
     - key (string | number; required)
```

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdAccordionItem.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdAccordionItem.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdAffix.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdAffix.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdAlert.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdAlert.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdAnchor.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdAnchor.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdAvatar.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdAvatar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdAvatarGroup.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdAvatarGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdBackTop.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdBackTop.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdBadge.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdBadge.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdBreadcrumb.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdBreadcrumb.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdButton.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdButton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdCalendar.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdCalendar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdCard.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdCard.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdCardGrid.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdCardGrid.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdCarousel.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdCarousel.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdCascader.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdCascader.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdCheckCard.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdCheckCard.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdCheckCardGroup.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdCheckCardGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdCheckbox.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdCheckbox.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdCheckboxGroup.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdCheckboxGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdCol.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdCol.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdCollapse.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdCollapse.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 - id (string; optional)
 
 - bordered (boolean; default True)
 
 - className (string | dict; optional)
 
-- collapsible (a value equal to: 'header', 'disabled'; optional)
+- collapsible (a value equal to: 'header', 'disabled', 'icon'; optional)
 
 - forceRender (boolean; default False)
 
 - ghost (boolean; default False)
 
 - isOpen (boolean; default True)
```

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdComment.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdComment.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdConfigProvider.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdConfigProvider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdContent.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdContent.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdCopyText.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdCopyText.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdCountdown.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdCountdown.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdCustomSkeleton.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdCustomSkeleton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdDatePicker.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdDatePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdDateRangePicker.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdDateRangePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdDescriptionItem.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdDescriptionItem.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdDescriptions.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdDescriptions.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdDivider.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdDivider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdDraggerUpload.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdDraggerUpload.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
     `defaultFileList` is a list of dicts with keys:
 
     - name (string; optional)
 
     - status (a value equal to: 'done', 'error', 'removed'; optional)
 
+    - taskId (string; optional)
+
     - uid (boolean | number | string | dict | list; optional)
 
     - url (string; optional)
 
 - directory (boolean; default False)
 
 - disabled (boolean; default False)
```

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdDrawer.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdDrawer.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdDropdown.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdDropdown.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 Keyword arguments:
 
 - id (string; optional)
 
 - arrow (boolean; default False)
 
+- autoAdjustOverflow (boolean; default True)
+
 - buttonMode (boolean; default False)
 
 - buttonProps (dict; optional)
 
     `buttonProps` is a dict with keys:
 
     - danger (boolean; optional)
@@ -82,18 +84,18 @@
 
 - visible (boolean; default False)"""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_antd_components'
     _type = 'AntdDropdown'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, key=Component.UNDEFINED, title=Component.UNDEFINED, buttonMode=Component.UNDEFINED, buttonProps=Component.UNDEFINED, clickedKey=Component.UNDEFINED, nClicks=Component.UNDEFINED, menuItems=Component.UNDEFINED, arrow=Component.UNDEFINED, disabled=Component.UNDEFINED, overlayClassName=Component.UNDEFINED, overlayStyle=Component.UNDEFINED, placement=Component.UNDEFINED, trigger=Component.UNDEFINED, visible=Component.UNDEFINED, popupContainer=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'arrow', 'buttonMode', 'buttonProps', 'className', 'clickedKey', 'disabled', 'key', 'loading_state', 'menuItems', 'nClicks', 'overlayClassName', 'overlayStyle', 'placement', 'popupContainer', 'style', 'title', 'trigger', 'visible']
+    def __init__(self, id=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, key=Component.UNDEFINED, title=Component.UNDEFINED, buttonMode=Component.UNDEFINED, buttonProps=Component.UNDEFINED, clickedKey=Component.UNDEFINED, nClicks=Component.UNDEFINED, menuItems=Component.UNDEFINED, arrow=Component.UNDEFINED, disabled=Component.UNDEFINED, overlayClassName=Component.UNDEFINED, overlayStyle=Component.UNDEFINED, placement=Component.UNDEFINED, trigger=Component.UNDEFINED, autoAdjustOverflow=Component.UNDEFINED, visible=Component.UNDEFINED, popupContainer=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'arrow', 'autoAdjustOverflow', 'buttonMode', 'buttonProps', 'className', 'clickedKey', 'disabled', 'key', 'loading_state', 'menuItems', 'nClicks', 'overlayClassName', 'overlayStyle', 'placement', 'popupContainer', 'style', 'title', 'trigger', 'visible']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'arrow', 'buttonMode', 'buttonProps', 'className', 'clickedKey', 'disabled', 'key', 'loading_state', 'menuItems', 'nClicks', 'overlayClassName', 'overlayStyle', 'placement', 'popupContainer', 'style', 'title', 'trigger', 'visible']
+        self.available_properties = ['id', 'arrow', 'autoAdjustOverflow', 'buttonMode', 'buttonProps', 'className', 'clickedKey', 'disabled', 'key', 'loading_state', 'menuItems', 'nClicks', 'overlayClassName', 'overlayStyle', 'placement', 'popupContainer', 'style', 'title', 'trigger', 'visible']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         super(AntdDropdown, self).__init__(**args)
```

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdEmpty.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdEmpty.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdFooter.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdFooter.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdForm.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdForm.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdFormItem.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdFormItem.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdHeader.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdHeader.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdIcon.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdIcon.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdImage.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdImage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdInput.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdInput.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdInputNumber.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdInputNumber.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdLayout.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdLayout.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdMentions.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdMentions.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdMenu.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdMenu.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdMessage.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdMessage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdModal.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdModal.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdNotification.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdNotification.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdPageHeader.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdPageHeader.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdPagination.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdPagination.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdParagraph.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdParagraph.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdPasteImage.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdPasteImage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdPictureUpload.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdPictureUpload.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
     `defaultFileList` is a list of dicts with keys:
 
     - name (string; optional)
 
     - status (a value equal to: 'done', 'error', 'removed'; optional)
 
+    - taskId (string; optional)
+
     - uid (boolean | number | string | dict | list; optional)
 
     - url (string; optional)
 
 - disabled (boolean; default False)
 
 - downloadUrl (string; optional)
```

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdPopconfirm.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdPopconfirm.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdPopover.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdPopover.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdPopupCard.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdPopupCard.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdProgress.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdProgress.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdRadioGroup.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdRadioGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdRate.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdRate.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdResult.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdResult.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdRibbon.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdRibbon.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdRow.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdRow.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdSegmented.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdSegmented.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdSegmentedColoring.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdSegmentedColoring.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdSelect.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdSelect.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdSider.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdSider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdSkeleton.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeleton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdSkeletonAvatar.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeletonAvatar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdSkeletonButton.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeletonButton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdSkeletonImage.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeletonImage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdSkeletonInput.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeletonInput.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdSlider.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdSlider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdSpace.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdSpace.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdSpin.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdSpin.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdSpoiler.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdSpoiler.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdStatistic.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdStatistic.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdSteps.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdSteps.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdSwitch.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdSwitch.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdTabPane.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdTabPane.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdTable.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdTable.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,14 +350,16 @@
 
 - nClicksButton (number; default 0)
 
 - nClicksCell (number; default 0)
 
 - nClicksDropdownItem (number; default 0)
 
+- nDoubleClicksCell (number; default 0)
+
 - pagination (dict; optional)
 
     `pagination` is a dict with keys:
 
     - current (number; optional)
 
     - disabled (boolean; optional)
@@ -390,14 +392,18 @@
 
 - recentlyButtonClickedRow (dict; optional)
 
 - recentlyCellClickColumn (string; optional)
 
 - recentlyCellClickRecord (dict; optional)
 
+- recentlyCellDoubleClickColumn (string; optional)
+
+- recentlyCellDoubleClickRecord (dict; optional)
+
 - recentlyChangedRow (dict; optional)
 
 - recentlyCheckedDataIndex (string; optional)
 
 - recentlyCheckedLabel (string; optional)
 
 - recentlyCheckedRow (dict; optional)
@@ -487,18 +493,18 @@
 
     - title (a list of or a singular dash component, string or number; optional)"""
     _children_props = ['columns[].title', 'summaryRowContents[].content', 'expandedRowKeyToContent[].content', 'emptyContent']
     _base_nodes = ['emptyContent', 'children']
     _namespace = 'feffery_antd_components'
     _type = 'AntdTable'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, key=Component.UNDEFINED, locale=Component.UNDEFINED, containerId=Component.UNDEFINED, columns=Component.UNDEFINED, data=Component.UNDEFINED, bordered=Component.UNDEFINED, maxHeight=Component.UNDEFINED, maxWidth=Component.UNDEFINED, size=Component.UNDEFINED, rowSelectionType=Component.UNDEFINED, selectedRowKeys=Component.UNDEFINED, rowSelectionWidth=Component.UNDEFINED, selectedRows=Component.UNDEFINED, sticky=Component.UNDEFINED, enableHoverListen=Component.UNDEFINED, recentlyMouseEnterColumnDataIndex=Component.UNDEFINED, recentlyMouseEnterRowKey=Component.UNDEFINED, recentlyMouseEnterRow=Component.UNDEFINED, titlePopoverInfo=Component.UNDEFINED, columnsFormatConstraint=Component.UNDEFINED, sortOptions=Component.UNDEFINED, filterOptions=Component.UNDEFINED, pagination=Component.UNDEFINED, currentData=Component.UNDEFINED, recentlyChangedRow=Component.UNDEFINED, sorter=Component.UNDEFINED, filter=Component.UNDEFINED, mode=Component.UNDEFINED, summaryRowContents=Component.UNDEFINED, summaryRowFixed=Component.UNDEFINED, conditionalStyleFuncs=Component.UNDEFINED, expandedRowKeyToContent=Component.UNDEFINED, expandedRowWidth=Component.UNDEFINED, expandRowByClick=Component.UNDEFINED, defaultExpandedRowKeys=Component.UNDEFINED, enableCellClickListenColumns=Component.UNDEFINED, recentlyCellClickColumn=Component.UNDEFINED, recentlyCellClickRecord=Component.UNDEFINED, nClicksCell=Component.UNDEFINED, emptyContent=Component.UNDEFINED, cellUpdateOptimize=Component.UNDEFINED, miniChartHeight=Component.UNDEFINED, miniChartAnimation=Component.UNDEFINED, recentlyButtonClickedRow=Component.UNDEFINED, nClicksButton=Component.UNDEFINED, clickedContent=Component.UNDEFINED, recentlyButtonClickedDataIndex=Component.UNDEFINED, customFormatFuncs=Component.UNDEFINED, recentlyCheckedRow=Component.UNDEFINED, recentlyCheckedLabel=Component.UNDEFINED, recentlyCheckedDataIndex=Component.UNDEFINED, recentlyCheckedStatus=Component.UNDEFINED, recentlySwitchRow=Component.UNDEFINED, recentlySwitchDataIndex=Component.UNDEFINED, recentlySwitchStatus=Component.UNDEFINED, nClicksDropdownItem=Component.UNDEFINED, recentlyClickedDropdownItemTitle=Component.UNDEFINED, recentlyDropdownItemClickedDataIndex=Component.UNDEFINED, recentlyDropdownItemClickedRow=Component.UNDEFINED, recentlySelectRow=Component.UNDEFINED, recentlySelectDataIndex=Component.UNDEFINED, recentlySelectValue=Component.UNDEFINED, hiddenRowKeys=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'bordered', 'cellUpdateOptimize', 'className', 'clickedContent', 'columns', 'columnsFormatConstraint', 'conditionalStyleFuncs', 'containerId', 'currentData', 'customFormatFuncs', 'data', 'defaultExpandedRowKeys', 'emptyContent', 'enableCellClickListenColumns', 'enableHoverListen', 'expandRowByClick', 'expandedRowKeyToContent', 'expandedRowWidth', 'filter', 'filterOptions', 'hiddenRowKeys', 'key', 'loading_state', 'locale', 'maxHeight', 'maxWidth', 'miniChartAnimation', 'miniChartHeight', 'mode', 'nClicksButton', 'nClicksCell', 'nClicksDropdownItem', 'pagination', 'recentlyButtonClickedDataIndex', 'recentlyButtonClickedRow', 'recentlyCellClickColumn', 'recentlyCellClickRecord', 'recentlyChangedRow', 'recentlyCheckedDataIndex', 'recentlyCheckedLabel', 'recentlyCheckedRow', 'recentlyCheckedStatus', 'recentlyClickedDropdownItemTitle', 'recentlyDropdownItemClickedDataIndex', 'recentlyDropdownItemClickedRow', 'recentlyMouseEnterColumnDataIndex', 'recentlyMouseEnterRow', 'recentlyMouseEnterRowKey', 'recentlySelectDataIndex', 'recentlySelectRow', 'recentlySelectValue', 'recentlySwitchDataIndex', 'recentlySwitchRow', 'recentlySwitchStatus', 'rowSelectionType', 'rowSelectionWidth', 'selectedRowKeys', 'selectedRows', 'size', 'sortOptions', 'sorter', 'sticky', 'style', 'summaryRowContents', 'summaryRowFixed', 'titlePopoverInfo']
+    def __init__(self, id=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, key=Component.UNDEFINED, locale=Component.UNDEFINED, containerId=Component.UNDEFINED, columns=Component.UNDEFINED, data=Component.UNDEFINED, bordered=Component.UNDEFINED, maxHeight=Component.UNDEFINED, maxWidth=Component.UNDEFINED, size=Component.UNDEFINED, rowSelectionType=Component.UNDEFINED, selectedRowKeys=Component.UNDEFINED, rowSelectionWidth=Component.UNDEFINED, selectedRows=Component.UNDEFINED, sticky=Component.UNDEFINED, enableHoverListen=Component.UNDEFINED, recentlyMouseEnterColumnDataIndex=Component.UNDEFINED, recentlyMouseEnterRowKey=Component.UNDEFINED, recentlyMouseEnterRow=Component.UNDEFINED, titlePopoverInfo=Component.UNDEFINED, columnsFormatConstraint=Component.UNDEFINED, sortOptions=Component.UNDEFINED, filterOptions=Component.UNDEFINED, pagination=Component.UNDEFINED, currentData=Component.UNDEFINED, recentlyChangedRow=Component.UNDEFINED, sorter=Component.UNDEFINED, filter=Component.UNDEFINED, mode=Component.UNDEFINED, summaryRowContents=Component.UNDEFINED, summaryRowFixed=Component.UNDEFINED, conditionalStyleFuncs=Component.UNDEFINED, expandedRowKeyToContent=Component.UNDEFINED, expandedRowWidth=Component.UNDEFINED, expandRowByClick=Component.UNDEFINED, defaultExpandedRowKeys=Component.UNDEFINED, enableCellClickListenColumns=Component.UNDEFINED, recentlyCellClickColumn=Component.UNDEFINED, recentlyCellClickRecord=Component.UNDEFINED, nClicksCell=Component.UNDEFINED, recentlyCellDoubleClickColumn=Component.UNDEFINED, recentlyCellDoubleClickRecord=Component.UNDEFINED, nDoubleClicksCell=Component.UNDEFINED, emptyContent=Component.UNDEFINED, cellUpdateOptimize=Component.UNDEFINED, miniChartHeight=Component.UNDEFINED, miniChartAnimation=Component.UNDEFINED, recentlyButtonClickedRow=Component.UNDEFINED, nClicksButton=Component.UNDEFINED, clickedContent=Component.UNDEFINED, recentlyButtonClickedDataIndex=Component.UNDEFINED, customFormatFuncs=Component.UNDEFINED, recentlyCheckedRow=Component.UNDEFINED, recentlyCheckedLabel=Component.UNDEFINED, recentlyCheckedDataIndex=Component.UNDEFINED, recentlyCheckedStatus=Component.UNDEFINED, recentlySwitchRow=Component.UNDEFINED, recentlySwitchDataIndex=Component.UNDEFINED, recentlySwitchStatus=Component.UNDEFINED, nClicksDropdownItem=Component.UNDEFINED, recentlyClickedDropdownItemTitle=Component.UNDEFINED, recentlyDropdownItemClickedDataIndex=Component.UNDEFINED, recentlyDropdownItemClickedRow=Component.UNDEFINED, recentlySelectRow=Component.UNDEFINED, recentlySelectDataIndex=Component.UNDEFINED, recentlySelectValue=Component.UNDEFINED, hiddenRowKeys=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'bordered', 'cellUpdateOptimize', 'className', 'clickedContent', 'columns', 'columnsFormatConstraint', 'conditionalStyleFuncs', 'containerId', 'currentData', 'customFormatFuncs', 'data', 'defaultExpandedRowKeys', 'emptyContent', 'enableCellClickListenColumns', 'enableHoverListen', 'expandRowByClick', 'expandedRowKeyToContent', 'expandedRowWidth', 'filter', 'filterOptions', 'hiddenRowKeys', 'key', 'loading_state', 'locale', 'maxHeight', 'maxWidth', 'miniChartAnimation', 'miniChartHeight', 'mode', 'nClicksButton', 'nClicksCell', 'nClicksDropdownItem', 'nDoubleClicksCell', 'pagination', 'recentlyButtonClickedDataIndex', 'recentlyButtonClickedRow', 'recentlyCellClickColumn', 'recentlyCellClickRecord', 'recentlyCellDoubleClickColumn', 'recentlyCellDoubleClickRecord', 'recentlyChangedRow', 'recentlyCheckedDataIndex', 'recentlyCheckedLabel', 'recentlyCheckedRow', 'recentlyCheckedStatus', 'recentlyClickedDropdownItemTitle', 'recentlyDropdownItemClickedDataIndex', 'recentlyDropdownItemClickedRow', 'recentlyMouseEnterColumnDataIndex', 'recentlyMouseEnterRow', 'recentlyMouseEnterRowKey', 'recentlySelectDataIndex', 'recentlySelectRow', 'recentlySelectValue', 'recentlySwitchDataIndex', 'recentlySwitchRow', 'recentlySwitchStatus', 'rowSelectionType', 'rowSelectionWidth', 'selectedRowKeys', 'selectedRows', 'size', 'sortOptions', 'sorter', 'sticky', 'style', 'summaryRowContents', 'summaryRowFixed', 'titlePopoverInfo']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'bordered', 'cellUpdateOptimize', 'className', 'clickedContent', 'columns', 'columnsFormatConstraint', 'conditionalStyleFuncs', 'containerId', 'currentData', 'customFormatFuncs', 'data', 'defaultExpandedRowKeys', 'emptyContent', 'enableCellClickListenColumns', 'enableHoverListen', 'expandRowByClick', 'expandedRowKeyToContent', 'expandedRowWidth', 'filter', 'filterOptions', 'hiddenRowKeys', 'key', 'loading_state', 'locale', 'maxHeight', 'maxWidth', 'miniChartAnimation', 'miniChartHeight', 'mode', 'nClicksButton', 'nClicksCell', 'nClicksDropdownItem', 'pagination', 'recentlyButtonClickedDataIndex', 'recentlyButtonClickedRow', 'recentlyCellClickColumn', 'recentlyCellClickRecord', 'recentlyChangedRow', 'recentlyCheckedDataIndex', 'recentlyCheckedLabel', 'recentlyCheckedRow', 'recentlyCheckedStatus', 'recentlyClickedDropdownItemTitle', 'recentlyDropdownItemClickedDataIndex', 'recentlyDropdownItemClickedRow', 'recentlyMouseEnterColumnDataIndex', 'recentlyMouseEnterRow', 'recentlyMouseEnterRowKey', 'recentlySelectDataIndex', 'recentlySelectRow', 'recentlySelectValue', 'recentlySwitchDataIndex', 'recentlySwitchRow', 'recentlySwitchStatus', 'rowSelectionType', 'rowSelectionWidth', 'selectedRowKeys', 'selectedRows', 'size', 'sortOptions', 'sorter', 'sticky', 'style', 'summaryRowContents', 'summaryRowFixed', 'titlePopoverInfo']
+        self.available_properties = ['id', 'bordered', 'cellUpdateOptimize', 'className', 'clickedContent', 'columns', 'columnsFormatConstraint', 'conditionalStyleFuncs', 'containerId', 'currentData', 'customFormatFuncs', 'data', 'defaultExpandedRowKeys', 'emptyContent', 'enableCellClickListenColumns', 'enableHoverListen', 'expandRowByClick', 'expandedRowKeyToContent', 'expandedRowWidth', 'filter', 'filterOptions', 'hiddenRowKeys', 'key', 'loading_state', 'locale', 'maxHeight', 'maxWidth', 'miniChartAnimation', 'miniChartHeight', 'mode', 'nClicksButton', 'nClicksCell', 'nClicksDropdownItem', 'nDoubleClicksCell', 'pagination', 'recentlyButtonClickedDataIndex', 'recentlyButtonClickedRow', 'recentlyCellClickColumn', 'recentlyCellClickRecord', 'recentlyCellDoubleClickColumn', 'recentlyCellDoubleClickRecord', 'recentlyChangedRow', 'recentlyCheckedDataIndex', 'recentlyCheckedLabel', 'recentlyCheckedRow', 'recentlyCheckedStatus', 'recentlyClickedDropdownItemTitle', 'recentlyDropdownItemClickedDataIndex', 'recentlyDropdownItemClickedRow', 'recentlyMouseEnterColumnDataIndex', 'recentlyMouseEnterRow', 'recentlyMouseEnterRowKey', 'recentlySelectDataIndex', 'recentlySelectRow', 'recentlySelectValue', 'recentlySwitchDataIndex', 'recentlySwitchRow', 'recentlySwitchStatus', 'rowSelectionType', 'rowSelectionWidth', 'selectedRowKeys', 'selectedRows', 'size', 'sortOptions', 'sorter', 'sticky', 'style', 'summaryRowContents', 'summaryRowFixed', 'titlePopoverInfo']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         super(AntdTable, self).__init__(**args)
```

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdTabs.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdTabs.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdTag.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdTag.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdText.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdText.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdTimePicker.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdTimePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdTimeRangePicker.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdTimeRangePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdTimeline.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdTimeline.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdTitle.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdTitle.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdTooltip.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdTooltip.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdTransfer.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdTransfer.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdTree.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdTree.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdTreeSelect.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdTreeSelect.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdUpload.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdUpload.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
     `defaultFileList` is a list of dicts with keys:
 
     - name (string; optional)
 
     - status (a value equal to: 'done', 'error', 'removed'; optional)
 
+    - taskId (string; optional)
+
     - uid (boolean | number | string | dict | list; optional)
 
     - url (string; optional)
 
 - directory (boolean; default False)
 
 - disabled (boolean; default False)
```

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/AntdWatermark.py` & `feffery_antd_components-0.2.3/feffery_antd_components/AntdWatermark.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/__init__.py` & `feffery_antd_components-0.2.3/feffery_antd_components/__init__.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/_imports_.py` & `feffery_antd_components-0.2.3/feffery_antd_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/feffery_antd_components.min.js` & `feffery_antd_components-0.2.3/feffery_antd_components/feffery_antd_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -57,15 +57,15 @@
     return Object.defineProperty(r, "p", {
         get: (t = o().src.split("/").slice(0, -1).join("/") + "/", function() {
             return t
         })
     }), "undefined" != typeof jsonpScriptSrc && (i = jsonpScriptSrc, jsonpScriptSrc = function(t) {
         var e, n = /\/_dash-component-suites\//.test(o().src),
             t = i(t);
-        return n ? ((e = (n = t.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_2m1682056676"), n.splice(-1, 1, e.join(".")), n.join("/")) : t
+        return n ? ((e = (n = t.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_3m1682406921"), n.splice(-1, 1, e.join(".")), n.join("/")) : t
     }), r(r.s = 688)
 }([function(t, e) {
     t.exports = window.React
 }, function(t, e) {
     t.exports = window.PropTypes
 }, function(R, t, e) {
     "use strict";
@@ -89473,14 +89473,15 @@
                         pagination = _this$props.pagination,
                         bordered = _this$props.bordered,
                         maxHeight = _this$props.maxHeight,
                         maxWidth = _this$props.maxWidth,
                         size = _this$props.size,
                         mode = _this$props.mode,
                         nClicksButton = _this$props.nClicksButton,
+                        nDoubleClicksCell = _this$props.nDoubleClicksCell,
                         summaryRowContents = _this$props.summaryRowContents,
                         summaryRowFixed = _this$props.summaryRowFixed,
                         customFormatFuncs = _this$props.customFormatFuncs,
                         conditionalStyleFuncs = _this$props.conditionalStyleFuncs,
                         expandedRowKeyToContent = _this$props.expandedRowKeyToContent,
                         expandedRowWidth = _this$props.expandedRowWidth,
                         expandRowByClick = _this$props.expandRowByClick,
@@ -90084,14 +90085,21 @@
                                 return {
                                     onClick: function(t) {
                                         setProps({
                                             recentlyCellClickColumn: n,
                                             recentlyCellClickRecord: e,
                                             nClicksCell: nClicksCell + 1
                                         })
+                                    },
+                                    onDoubleClick: function(t) {
+                                        setProps({
+                                            recentlyCellDoubleClickColumn: n,
+                                            recentlyCellDoubleClickRecord: e,
+                                            nDoubleClicksCell: nDoubleClicksCell + 1
+                                        })
                                     }
                                 }
                             }
                         })) : t
                     })), rowSelectionType && (rowSelection = {
                         columnWidth: rowSelectionWidth,
                         fixed: !0,
@@ -90429,14 +90437,17 @@
         expandedRowWidth: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.oneOfType([prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string, prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number]),
         expandRowByClick: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool,
         defaultExpandedRowKeys: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.arrayOf(prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string),
         enableCellClickListenColumns: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.arrayOf(prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string),
         recentlyCellClickColumn: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string,
         recentlyCellClickRecord: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.object,
         nClicksCell: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number,
+        recentlyCellDoubleClickColumn: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string,
+        recentlyCellDoubleClickRecord: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.object,
+        nDoubleClicksCell: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number,
         emptyContent: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.node,
         cellUpdateOptimize: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool,
         miniChartHeight: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number,
         miniChartAnimation: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool,
         recentlyButtonClickedRow: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.object,
         nClicksButton: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number,
         clickedContent: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string,
@@ -90475,14 +90486,15 @@
         filterOptions: {},
         mode: "client-side",
         sticky: !1,
         enableHoverListen: !1,
         expandRowByClick: !1,
         enableCellClickListenColumns: [],
         nClicksCell: 0,
+        nDoubleClicksCell: 0,
         cellUpdateOptimize: !1,
         summaryRowFixed: !1,
         conditionalStyleFuncs: {},
         rowSelectionWidth: 32,
         hiddenRowKeys: [],
         nClicksButton: 0,
         miniChartHeight: 30,
@@ -103327,51 +103339,51 @@
             _ = t.popupContainer,
             O = t.readOnly,
             w = t.placement,
             k = t.persistence,
             j = t.persisted_props,
             M = t.persistence_type,
             t = t.loading_state,
-            E = Object(Wt.useContext)(U.a),
+            E = Object(Wt.useContext)(G.a),
             o = E && E.locale || o;
         return Object(Wt.useEffect)(function() {
             b && !g && i({
                 value: b
             }), d && !c ? i({
                 format: "YYYY-MM-DD HH:mm:ss"
             }) : d || c || i({
                 format: "YYYY-MM-DD"
             }), m || i({
                 defaultPickerValue: C()(new Date).format(c || "YYYY-MM-DD")
             })
         }, []), Object(Wt.useEffect)(function() {
-            Object(W.isUndefined)(s) || C.a.locale("en-us" === o ? "en" : o, {
+            Object(V.isUndefined)(s) || C.a.locale("en-us" === o ? "en" : o, {
                 week: {
                     dow: s
                 }
             })
-        }, [s]), F.a.createElement("div", null, F.a.createElement(H.a, {
-            locale: V.b.get(o)
-        }, F.a.createElement(S.a, {
+        }, [s]), H.a.createElement("div", null, H.a.createElement(W.a, {
+            locale: K.b.get(o)
+        }, H.a.createElement(S.a, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             format: c,
             onChange: function(t, e) {
-                Object(W.isString)(e) && i({
+                Object(V.isString)(e) && i({
                     value: e
                 })
             },
             picker: l,
             calendarStartDay: s,
-            disabled: E && !Object(W.isUndefined)(E.componentDisabled) ? E.componentDisabled : u,
+            disabled: E && !Object(V.isUndefined)(E.componentDisabled) ? E.componentDisabled : u,
             placeholder: f,
             bordered: v,
-            size: E && !Object(W.isUndefined)(E.componentSize) ? E.componentSize : y,
+            size: E && !Object(V.isUndefined)(E.componentSize) ? E.componentSize : y,
             disabledDate: h ? function(t) {
                 for (var e = 0; e < h.length; e++) {
                     var n = h[e];
                     if ("eq" === n.mode) {
                         if ("day" === n.target) {
                             if (t.date() === n.value) return !0
                         } else if ("month" === n.target) {
@@ -103484,18 +103496,18 @@
                     } else if ("not-in-enumerate-dates" === n.mode && !n.value.includes(t.format(c))) return !0
                 }
             } : void 0,
             defaultPickerValue: C()(m, c),
             value: g ? C()(g, c) : void 0,
             defaultValue: b ? C()(b, c) : void 0,
             showTime: d,
-            allowClear: Object(W.isUndefined)(O) ? p : !O,
+            allowClear: Object(V.isUndefined)(O) ? p : !O,
             status: x,
             placement: w,
-            open: !(!Object(W.isUndefined)(O) && O) && void 0,
+            open: !(!Object(V.isUndefined)(O) && O) && void 0,
             inputReadOnly: O,
             persistence: k,
             persisted_props: j,
             persistence_type: M,
             "data-dash-is-loading": t && t.is_loading || void 0,
             getPopupContainer: "parent" === _ ? function(t) {
                 return t.parentNode
@@ -103527,45 +103539,45 @@
             _ = t.popupContainer,
             O = t.readOnly,
             w = t.placement,
             k = t.persistence,
             j = t.persisted_props,
             M = t.persistence_type,
             t = t.loading_state,
-            E = Object(Wt.useContext)(U.a),
+            E = Object(Wt.useContext)(G.a),
             o = E && E.locale || o;
         return Object(Wt.useEffect)(function() {
             h && !p && i({
                 value: h
             }), u && !s ? i({
                 format: "YYYY-MM-DD HH:mm:ss"
             }) : u || s || i({
                 format: "YYYY-MM-DD"
             }), y || i({
                 defaultPickerValue: C()(new Date).format(s || "YYYY-MM-DD")
             })
         }, []), Object(Wt.useEffect)(function() {
-            Object(W.isUndefined)(c) || C.a.locale("en-us" === o ? "en" : o, {
+            Object(V.isUndefined)(c) || C.a.locale("en-us" === o ? "en" : o, {
                 week: {
                     dow: c
                 }
             })
-        }, [c]), F.a.createElement("div", null, F.a.createElement(H.a, {
-            locale: V.b.get(o)
-        }, F.a.createElement(L, {
+        }, [c]), H.a.createElement("div", null, H.a.createElement(W.a, {
+            locale: K.b.get(o)
+        }, H.a.createElement(L, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             format: s,
-            size: E && !Object(W.isUndefined)(E.componentSize) ? E.componentSize : v,
+            size: E && !Object(V.isUndefined)(E.componentSize) ? E.componentSize : v,
             picker: l,
             showTime: u,
-            allowClear: Object(W.isUndefined)(O) ? d : !O,
-            disabled: E && !Object(W.isUndefined)(E.componentDisabled) ? [E.componentDisabled, E.componentDisabled] : g && 2 === g.length ? g : void 0,
+            allowClear: Object(V.isUndefined)(O) ? d : !O,
+            disabled: E && !Object(V.isUndefined)(E.componentDisabled) ? [E.componentDisabled, E.componentDisabled] : g && 2 === g.length ? g : void 0,
             allowEmpty: g && 2 === g.length ? g : void 0,
             placeholder: m && 2 === m.length ? m : void 0,
             onChange: function(t, e) {
                 Array.isArray(e) && ("" !== e[0] && "" !== e[1] ? i({
                     value: [e[0], e[1]]
                 }) : i({
                     value: null
@@ -103689,28 +103701,28 @@
                 }
             } : void 0,
             defaultPickerValue: y ? [C()(y, s), C()(y, s)] : void 0,
             value: p && 2 === p.length ? [p[0] ? C()(p[0], s) : void 0, p[1] ? C()(p[1], s) : void 0] : void 0,
             defaultValue: h && 2 === h.length ? [h[0] ? C()(h[0], s) : void 0, h[1] ? C()(h[1], s) : void 0] : void 0,
             status: x,
             placement: w,
-            open: !(!Object(W.isUndefined)(O) && O) && void 0,
+            open: !(!Object(V.isUndefined)(O) && O) && void 0,
             inputReadOnly: O,
             persistence: k,
             persisted_props: j,
             persistence_type: M,
             "data-dash-is-loading": t && t.is_loading || void 0,
             getPopupContainer: "parent" === _ ? function(t) {
                 return t.parentNode
             } : void 0
         })))
     }
 
     function b(t) {
-        var e, n = (a = Wt.useContext(G.b)).getPrefixCls,
+        var e, n = (a = Wt.useContext(q.b)).getPrefixCls,
             a = a.direction,
             r = t.prefixCls,
             o = void 0 === (o = t.type) ? "horizontal" : o,
             i = void 0 === (i = t.orientation) ? "center" : i,
             l = t.orientationMargin,
             c = t.className,
             s = t.children,
@@ -103749,42 +103761,42 @@
             c = t.lineColor,
             s = t.fontSize,
             u = t.fontStyle,
             d = t.fontWeight,
             p = t.fontFamily,
             f = t.fontColor,
             t = t.loading_state;
-        return "horizontal" == o ? F.a.createElement(b, {
+        return "horizontal" == o ? H.a.createElement(b, {
             id: e,
             style: {
                 borderTopColor: c,
                 fontStyle: u,
                 fontWeight: d,
                 fontFamily: p,
                 fontSize: s,
                 color: f
             },
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             key: r,
             dashed: l,
             orientation: i,
             type: "horizontal",
             plain: !0,
             "data-dash-is-loading": t && t.is_loading || void 0
-        }, n) : "vertical" == o ? F.a.createElement(b, {
+        }, n) : "vertical" == o ? H.a.createElement(b, {
             id: e,
             style: {
                 borderLeftColor: c,
                 fontStyle: u,
                 fontWeight: d,
                 fontFamily: p,
                 fontSize: s,
                 color: f
             },
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             key: r,
             dashed: l,
             orientation: i,
             type: "vertical",
             plain: !0,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n) : void 0
@@ -103808,40 +103820,40 @@
             m = t.size,
             g = t.nClicks,
             b = t.debounceWait,
             v = t.icon,
             y = t.loading,
             x = t.autoSpin,
             t = t.loading_state,
-            _ = Object(Wt.useContext)(U.a),
+            _ = Object(Wt.useContext)(G.a),
             b = Object(Z.a)(function() {
                 g++, l(x ? {
                     nClicks: g,
                     loading: !0
                 } : {
                     nClicks: g
                 })
             }, {
                 debounceWait: Math.max(b, 200),
                 debounceLeading: !0,
                 manual: !0
             }).run;
-        return React.createElement(T.a, {
+        return React.createElement(z.a, {
             id: e,
-            className: Object(W.isString)(r) ? r : r ? Object(K.a)(r) : void 0,
+            className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
             style: o,
             key: i,
             type: c,
             href: s,
             target: u,
             block: d,
             danger: p,
-            disabled: _ && !Object(W.isUndefined)(_.componentDisabled) ? _.componentDisabled : f,
+            disabled: _ && !Object(V.isUndefined)(_.componentDisabled) ? _.componentDisabled : f,
             shape: h,
-            size: _ && !Object(W.isUndefined)(_.componentSize) ? _.componentSize : m,
+            size: _ && !Object(V.isUndefined)(_.componentSize) ? _.componentSize : m,
             icon: v,
             onClick: b,
             loading: y,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, y && a || n)
     }
 
@@ -103877,15 +103889,15 @@
             C = t.dropdownAfter,
             I = t.popupContainer,
             S = t.readOnly,
             L = t.loading_state,
             N = t.persistence,
             Y = t.persisted_props,
             t = t.persistence_type,
-            P = Object(Wt.useContext)(U.a),
+            P = Object(Wt.useContext)(G.a),
             o = P && P.locale || o;
         Object(Wt.useEffect)(function() {
             g && !h && i({
                 value: g
             })
         }, []);
         for (var B = Object(Z.a)(function(t) {
@@ -103968,36 +103980,36 @@
                 return React.createElement("div", {
                     style: {
                         flex: "auto",
                         background: t
                     }
                 })
             }))) : u[T].label));
-        return "label" === O && (O = "children"), React.createElement(H.a, {
-            locale: V.b.get(o)
+        return "label" === O && (O = "children"), React.createElement(W.a, {
+            locale: K.b.get(o)
         }, React.createElement(J.a, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: n,
             key: r,
             mode: m,
-            allowClear: Object(W.isUndefined)(S) ? p : !S,
+            allowClear: Object(V.isUndefined)(S) ? p : !S,
             placeholder: l,
-            size: P && !Object(W.isUndefined)(P.componentSize) ? P.componentSize : c,
+            size: P && !Object(V.isUndefined)(P.componentSize) ? P.componentSize : c,
             bordered: s,
             value: h,
             defaultValue: g,
             onChange: function(t) {
                 i({
                     value: t
                 })
             },
             maxTagCount: b,
             listHeight: v,
-            disabled: P && !Object(W.isUndefined)(P.componentDisabled) ? P.componentDisabled : f,
+            disabled: P && !Object(V.isUndefined)(P.componentDisabled) ? P.componentDisabled : f,
             showSearch: !0,
             placement: x,
             status: _,
             optionFilterProp: O,
             autoClearSearchValue: j,
             onSearch: function(t) {
                 i({
@@ -104012,29 +104024,29 @@
             persistence: N,
             persisted_props: Y,
             persistence_type: t,
             "data-dash-is-loading": L && L.is_loading || void 0,
             getPopupContainer: "parent" === I ? function(t) {
                 return t.parentNode
             } : void 0,
-            open: !(!Object(W.isUndefined)(S) && S) && void 0
+            open: !(!Object(V.isUndefined)(S) && S) && void 0
         }, D))
     }
     var Wt = e(0),
-        F = e.n(Wt),
+        H = e.n(Wt),
         n = e(1),
         n = e.n(n),
-        H = e(17),
+        W = e(17),
         S = e(307),
         a = e(14),
         C = e.n(a),
-        W = e(10),
-        V = (e(224), e(25)),
-        K = e(12),
-        U = e(28),
+        V = e(10),
+        K = (e(224), e(25)),
+        U = e(12),
+        G = e(28),
         _ = (m.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             format: n.a.string,
@@ -104130,15 +104142,15 @@
             placement: "bottomLeft",
             popupContainer: "body"
         }, g),
         Et = e(6),
         Vt = e(5),
         a = e(7),
         Kt = e.n(a),
-        G = e(69),
+        q = e(69),
         w = function(t, e) {
             var n = {};
             for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
             if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                 for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
             return n
         },
@@ -104168,15 +104180,15 @@
             direction: "horizontal",
             lineColor: "lightgrey",
             fontStyle: "initial",
             fontWeight: "initial",
             fontFamily: "initial",
             fontColor: "#000000"
         }, v),
-        T = e(62),
+        z = e(62),
         Z = e(707),
         M = (y.propTypes = {
             id: n.a.string,
             children: n.a.node,
             loadingChildren: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
@@ -104292,31 +104304,31 @@
                 style: {
                     display: "flex",
                     justifyContent: "center"
                 }
             }, React.createElement(E.a, null))
         }, x),
         D = e(78),
-        z = e(523),
-        R = e(58);
+        T = e(523),
+        I = e(58);
 
-    function I(t) {
+    function R(t) {
         return null != t && "object" == typeof t && !0 === t["@@functional/placeholder"]
     }
 
     function N(n) {
         return function t(e) {
-            return 0 === arguments.length || I(e) ? t : n.apply(this, arguments)
+            return 0 === arguments.length || R(e) ? t : n.apply(this, arguments)
         }
     }
 
     function B(t) {
         var n;
-        return t && (t = (n = Object(W.cloneDeep)(t)).filter(function(t) {
-            return Object(W.isUndefined)(t.parent)
+        return t && (t = (n = Object(V.cloneDeep)(t)).filter(function(t) {
+            return Object(V.isUndefined)(t.parent)
         }), n.filter(function(t) {
             return t.parent
         }).forEach(function(e) {
             var t = n.find(function(t) {
                 return t.key === e.parent
             });
             t && (t.children ? t.children.push(e) : t.children = [e])
@@ -104383,34 +104395,34 @@
                 })
             }, []), Object(Wt.useMemo)(function() {
                 return B(u)
             }, [u])),
             E = ("flat" === o && (u = E), {
                 expandedKeys: d
             }),
-            E = Object(W.omitBy)(E, W.isUndefined);
-        return React.createElement(z.a, nt({
+            E = Object(V.omitBy)(E, V.isUndefined);
+        return React.createElement(T.a, nt({
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             treeData: function t(e) {
-                if (Object(W.isObject)(e))
+                if (Object(V.isObject)(e))
                     if (e.tooltipProps && (e.title = React.createElement(D.a, e.tooltipProps, e.title)), e.children) {
-                        Object(W.isString)(e.icon) && (e.icon = React.createElement(R.a, {
+                        Object(V.isString)(e.icon) && (e.icon = React.createElement(I.a, {
                             icon: e.icon
                         }));
                         for (var n = 0; n < e.children.length; n++) e.children[n] = t(e.children[n])
-                    } else Object(W.isString)(e.icon) && (e.icon = React.createElement(R.a, {
+                    } else Object(V.isString)(e.icon) && (e.icon = React.createElement(I.a, {
                         icon: e.icon
                     }));
-                if (Object(W.isArray)(e))
+                if (Object(V.isArray)(e))
                     for (var a = 0; a < e.length; a++) e[a] = t(e[a]);
                 return e
-            }(Object(W.cloneDeep)(u)),
+            }(Object(V.cloneDeep)(u)),
             selectedKeys: c,
             checkedKeys: p,
             selectable: l,
             checkable: i,
             defaultExpandAll: f,
             defaultExpandedKeys: h,
             defaultExpandParent: m,
@@ -104461,15 +104473,15 @@
                         t[a].children && r(t[a].children, e, n)
                     }
                 }
                 var a, o, i, e = t.node.key,
                     n = t.dragNode.key,
                     l = t.node.pos.split("-"),
                     l = t.dropPosition - Number(l[l.length - 1]),
-                    c = Object(W.cloneDeep)(u);
+                    c = Object(V.cloneDeep)(u);
                 r(c, n, function(t, e, n) {
                     n.splice(e, 1), a = t
                 }), t.dropToGap ? 0 < (t.node.props.children || []).length && t.node.props.expanded && 1 == l ? r(c, e, function(t) {
                     t.children = t.children || [], t.children.unshift(a)
                 }) : (i = [], r(c, e, function(t, e, n) {
                     i = n, o = e
                 }), -1 == l ? i.splice(o, 0, a) : i.splice(o + 1, 0, a)) : r(c, e, function(t) {
@@ -104816,18 +104828,18 @@
             l.setState({
                 status: xt.Prepare,
                 affixStyle: void 0,
                 placeholderStyle: void 0
             })
         }, l
     }
-    wt.contextType = G.b, yt([dt()], wt.prototype, "updatePosition", null), yt([dt()], wt.prototype, "lazyUpdatePosition", null);
+    wt.contextType = q.b, yt([dt()], wt.prototype, "updatePosition", null), yt([dt()], wt.prototype, "lazyUpdatePosition", null);
     var jt = Wt.forwardRef(function(t, e) {
             var n = t.prefixCls,
-                n = (0, Wt.useContext(G.b).getPrefixCls)("affix", n),
+                n = (0, Wt.useContext(q.b).getPrefixCls)("affix", n),
                 t = Object(Et.a)(Object(Et.a)({}, t), {
                     affixPrefixCls: n
                 });
             return Wt.createElement(wt, Object(Et.a)({}, t, {
                 ref: e
             }))
         }),
@@ -104868,15 +104880,15 @@
             t = Wt.useState(null),
             b = (t = Object(Gt.a)(t, 2))[0],
             v = t[1],
             y = Wt.useRef(b),
             x = Wt.useRef(null),
             _ = Wt.useRef(null),
             O = Wt.useRef(!1),
-            w = (t = Wt.useContext(G.b)).direction,
+            w = (t = Wt.useContext(q.b)).direction,
             t = t.getTargetContainer,
             k = null != (f = null != f ? f : t) ? f : Pt,
             t = JSON.stringify(m),
             j = Wt.useCallback(function(e) {
                 m.includes(e) || g(function(t) {
                     return [].concat(Object(Ut.a)(t), [e])
                 })
@@ -104963,15 +104975,15 @@
             offsetTop: o,
             target: k
         }, r) : r)
     }
 
     function zt(t) {
         var e = t.prefixCls,
-            e = (0, Wt.useContext(G.b).getPrefixCls)("anchor", e);
+            e = (0, Wt.useContext(q.b).getPrefixCls)("anchor", e);
         return Wt.createElement(Tt, Object(Et.a)({}, t, {
             anchorPrefixCls: e
         }))
     }
 
     function At(t) {
         var e = t.id,
@@ -104983,22 +104995,22 @@
             l = t.containerId,
             c = t.targetOffset,
             s = t.affix,
             u = t.bounds,
             d = t.offsetTop,
             p = t.loading_state,
             f = t.setProps;
-        return F.a.createElement("div", {
+        return H.a.createElement("div", {
             style: {
                 float: i
             },
             "data-dash-is-loading": p && p.is_loading || void 0
-        }, F.a.createElement(It, {
+        }, H.a.createElement(It, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             onClick: function(t, e) {
                 f({
                     clickedLink: e
                 })
             },
@@ -105006,19 +105018,19 @@
                 return document.getElementById(l)
             } : void 0,
             targetOffset: c,
             affix: s,
             bounds: u,
             offsetTop: d
         }, function t(e) {
-            if (e.hasOwnProperty("href")) e = e.hasOwnProperty("children") ? F.a.createElement(Nt, {
+            if (e.hasOwnProperty("href")) e = e.hasOwnProperty("children") ? H.a.createElement(Nt, {
                 href: e.href,
                 title: e.title,
                 target: e.target
-            }, t(e.children)) : F.a.createElement(Nt, {
+            }, t(e.children)) : H.a.createElement(Nt, {
                 href: e.href,
                 title: e.title,
                 target: e.target
             });
             else
                 for (var n = 0; n < e.length; n++) e[n] = t(e[n]);
             return e
@@ -105047,15 +105059,15 @@
                 f = e.activeLink;
             Wt.useEffect(function() {
                 return null != n && n(r),
                     function() {
                         null != u && u(r)
                     }
             }, [r, n, u]);
-            return Wt.createElement(G.a, null, function(t) {
+            return Wt.createElement(q.a, null, function(t) {
                 var t = (0, t.getPrefixCls)("anchor", i),
                     e = f === r,
                     n = Kt()("".concat(t, "-link"), c, Object(Vt.a)({}, "".concat(t, "-link-active"), e)),
                     t = Kt()("".concat(t, "-link-title"), Object(Vt.a)({}, "".concat(t, "-link-title-active"), e));
                 return Wt.createElement("div", {
                     className: n
                 }, Wt.createElement("a", {
@@ -105100,15 +105112,15 @@
             bounds: 5
         }, At),
         c = e(91),
         Xt = e.n(c),
         $t = e(30),
         Bt = e(16),
         Ct = e(4),
-        q = e(15),
+        X = e(15),
         Zt = Wt.createContext({
             min: 0,
             max: 0,
             direction: "ltr",
             step: 1,
             includedStart: 0,
             includedEnd: 0,
@@ -105173,36 +105185,36 @@
                     style: Object(Ct.a)(Object(Ct.a)({}, _), l),
                     onMouseDown: n,
                     onTouchStart: n,
                     onKeyDown: function(t) {
                         if (!m) {
                             var e = null;
                             switch (t.which || t.keyCode) {
-                                case q.a.LEFT:
+                                case X.a.LEFT:
                                     e = "ltr" === h || "btt" === h ? -1 : 1;
                                     break;
-                                case q.a.RIGHT:
+                                case X.a.RIGHT:
                                     e = "ltr" === h || "btt" === h ? 1 : -1;
                                     break;
-                                case q.a.UP:
+                                case X.a.UP:
                                     e = "ttb" !== h ? 1 : -1;
                                     break;
-                                case q.a.DOWN:
+                                case X.a.DOWN:
                                     e = "ttb" !== h ? -1 : 1;
                                     break;
-                                case q.a.HOME:
+                                case X.a.HOME:
                                     e = "min";
                                     break;
-                                case q.a.END:
+                                case X.a.END:
                                     e = "max";
                                     break;
-                                case q.a.PAGE_UP:
+                                case X.a.PAGE_UP:
                                     e = 2;
                                     break;
-                                case q.a.PAGE_DOWN:
+                                case X.a.PAGE_DOWN:
                                     e = -2
                             }
                             null !== e && (t.preventDefault(), u(e, o))
                         }
                     },
                     tabIndex: m ? null : Jt(b, o),
                     role: "slider",
@@ -105462,32 +105474,32 @@
             b = t.tooltipSuffix,
             v = t.popupContainer,
             y = t.loading_state,
             x = t.setProps,
             _ = t.persistence,
             O = t.persisted_props,
             t = t.persistence_type,
-            w = Object(Wt.useContext)(U.a);
+            w = Object(Wt.useContext)(G.a);
         return Object(Wt.useEffect)(function() {
             u ? i || x({
                 value: l || [d, p],
                 defaultValue: l || [d, p]
             }) : i || 0 === i || x({
                 value: l || 0 === l ? l : p,
                 defaultValue: l || 0 === l ? l : p
             })
-        }, []), F.a.createElement(me, {
+        }, []), H.a.createElement(me, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             railStyle: r,
             key: o,
             value: i,
             defaultValue: l,
-            disabled: w && !Object(W.isUndefined)(w.componentDisabled) ? w.componentDisabled : c,
+            disabled: w && !Object(V.isUndefined)(w.componentDisabled) ? w.componentDisabled : c,
             vertical: s,
             range: u,
             min: d,
             max: p,
             step: f,
             marks: h,
             tooltip: {
@@ -105932,15 +105944,15 @@
         }),
         me = Wt.forwardRef(function(d, t) {
             function p(e, n) {
                 a(function(t) {
                     return Object(Et.a)(Object(Et.a)({}, t), Object(Vt.a)({}, e, n))
                 })
             }
-            var e = Wt.useContext(G.b),
+            var e = Wt.useContext(q.b),
                 f = e.getPrefixCls,
                 h = e.direction,
                 m = e.getPopupContainer,
                 e = Wt.useState({}),
                 e = Object(Gt.a)(e, 2),
                 g = e[0],
                 a = e[1],
@@ -106252,21 +106264,21 @@
             c = t.className,
             s = t.style,
             u = t.direction,
             t = t.oneWay;
         return Wt.createElement("div", {
             className: c,
             style: s
-        }, Wt.createElement(T.a, {
+        }, Wt.createElement(z.a, {
             type: "primary",
             size: "small",
             disabled: e || !l,
             onClick: a,
             icon: "rtl" !== u ? Wt.createElement(Ve.a, null) : Wt.createElement(We.a, null)
-        }, o), !t && Wt.createElement(T.a, {
+        }, o), !t && Wt.createElement(z.a, {
             type: "primary",
             size: "small",
             disabled: e || !i,
             onClick: n,
             icon: "rtl" !== u ? Wt.createElement(We.a, null) : Wt.createElement(Ve.a, null)
         }, r))
     }
@@ -106506,15 +106518,15 @@
             key: "render",
             value: function() {
                 var S = this;
                 return Wt.createElement(ye.a, {
                     componentName: "Transfer",
                     defaultLocale: xe.a.Transfer
                 }, function(C) {
-                    return Wt.createElement(G.a, null, function(t) {
+                    return Wt.createElement(q.a, null, function(t) {
                         var j = t.getPrefixCls,
                             M = t.renderEmpty,
                             E = t.direction;
                         return Wt.createElement(ve.b.Consumer, null, function(t) {
                             var e = t.hasFeedback,
                                 t = t.status,
                                 n = S.props,
@@ -106814,23 +106826,23 @@
             h = t.disabled,
             m = t.targetKeys,
             g = t.status,
             b = t.persistence,
             v = t.persisted_props,
             y = t.persistence_type,
             t = t.loading_state,
-            x = Object(Wt.useContext)(U.a),
+            x = Object(Wt.useContext)(G.a),
             o = x && x.locale || o,
-            f = f || V.a.AntdTransfer[o].titles;
-        return F.a.createElement(H.a, {
-            locale: V.b.get(o)
-        }, F.a.createElement(qe, {
+            f = f || K.a.AntdTransfer[o].titles;
+        return H.a.createElement(W.a, {
+            locale: K.b.get(o)
+        }, H.a.createElement(qe, {
             id: e,
             style: a,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             key: r,
             dataSource: l,
             targetKeys: m,
             onChange: function(t, e, n) {
                 i({
                     targetKeys: t,
                     moveDirection: e,
@@ -106841,15 +106853,15 @@
                 return t.title
             },
             pagination: s,
             operations: u,
             showSearch: d,
             showSelectAll: p,
             titles: f,
-            disabled: x && !Object(W.isUndefined)(x.componentDisabled) ? x.componentDisabled : h,
+            disabled: x && !Object(V.isUndefined)(x.componentDisabled) ? x.componentDisabled : h,
             status: g,
             persistence: b,
             persisted_props: v,
             persistence_type: y,
             listStyle: {
                 overflowX: "auto",
                 height: c,
@@ -106999,15 +107011,15 @@
             }, u)), c && Wt.createElement("div", {
                 className: "".concat(n, "-item-description")
             }, c))))
         }
     }]);
     var tn, en, nn = on,
         an = ["prefixCls", "style", "className", "children", "direction", "type", "labelPlacement", "iconPrefix", "status", "size", "current", "progressDot", "stepIcon", "initial", "icons", "onChange", "items"],
-        c = (c = F.a.Component, Object(r.a)(rn, c), tn = Object(o.a)(rn), Object(a.a)(rn, [{
+        c = (c = H.a.Component, Object(r.a)(rn, c), tn = Object(o.a)(rn), Object(a.a)(rn, [{
             key: "render",
             value: function() {
                 var a = this,
                     t = this.props,
                     r = t.prefixCls,
                     e = t.style,
                     o = void 0 === e ? {} : e,
@@ -107026,23 +107038,23 @@
                     g = t.onChange,
                     b = t.items,
                     b = void 0 === b ? [] : b,
                     t = Object(Bt.a)(t, an),
                     i = "navigation" === i,
                     l = p ? "vertical" : l,
                     u = Kt()(r, "".concat(r, "-").concat(n), e, (e = {}, Object(Vt.a)(e, "".concat(r, "-").concat(u), u), Object(Vt.a)(e, "".concat(r, "-label-").concat(l), "horizontal" === n), Object(Vt.a)(e, "".concat(r, "-dot"), !!p), Object(Vt.a)(e, "".concat(r, "-navigation"), i), e));
-                return F.a.createElement("div", Object(Et.a)({
+                return H.a.createElement("div", Object(Et.a)({
                     className: u,
                     style: o
                 }, t), b.filter(function(t) {
                     return t
                 }).map(function(t, e) {
                     var t = Object(Ct.a)({}, t),
                         n = h + e;
-                    return "error" === s && e === d - 1 && (t.className = "".concat(r, "-next-error")), t.status || (t.status = n === d ? s : n < d ? "finish" : "wait"), F.a.createElement(nn, Object(Et.a)({}, t, {
+                    return "error" === s && e === d - 1 && (t.className = "".concat(r, "-next-error")), t.status || (t.status = n === d ? s : n < d ? "finish" : "wait"), H.a.createElement(nn, Object(Et.a)({}, t, {
                         active: n === d,
                         stepNumber: n + 1,
                         stepIndex: n,
                         key: n,
                         prefixCls: r,
                         iconPrefix: c,
                         wrapperStyle: o,
@@ -107309,15 +107321,15 @@
             i = t.steps,
             l = t.strokeColor,
             c = void 0 === (c = t.percent) ? 0 : c,
             s = void 0 === (s = t.size) ? "default" : s,
             u = void 0 === (u = t.showInfo) || u,
             d = void 0 === (d = t.type) ? "line" : d,
             p = Ln(t, ["prefixCls", "className", "steps", "strokeColor", "percent", "size", "showInfo", "type"]),
-            f = (h = Wt.useContext(G.b)).getPrefixCls,
+            f = (h = Wt.useContext(q.b)).getPrefixCls,
             h = h.direction,
             f = f("progress", r),
             m = (r = t.status, !Pn.includes(r) && (m = On(t), 100 <= parseInt((void 0 !== m ? m : c).toString(), 10)) ? "success" : r || "normal"),
             g = (r = f, n = m, g = t.format, b = On(t), u ? (v = "line" === d, g || "exception" !== n && "success" !== n ? a = (g || function(t) {
                 return "".concat(t, "%")
             })(_n(c), _n(b)) : "exception" === n ? a = v ? Wt.createElement(dn.a, null) : Wt.createElement(Ze.a, null) : "success" === n && (a = v ? Wt.createElement(un.a, null) : Wt.createElement($e.a, null)), Wt.createElement("span", {
                 className: "".concat(r, "-text"),
@@ -107357,15 +107369,15 @@
                 var n = {};
                 for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                 if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                     for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                 return n
             }(t, ["percent", "size", "className", "direction", "items", "responsive", "current", "children"]),
             u = Object(sn.a)(i).xs,
-            d = (p = Wt.useContext(G.b)).getPrefixCls,
+            d = (p = Wt.useContext(q.b)).getPrefixCls,
             p = p.direction,
             f = Wt.useCallback(function() {
                 return i && u ? "vertical" : r
             }, [u, r]),
             h = d("steps", t.prefixCls),
             d = d("", t.iconPrefix),
             c = (t = c, o || Object(Dn.a)(t).map(function(t) {
@@ -107430,17 +107442,17 @@
             h = t.responsive,
             m = t.setProps,
             t = t.loading_state;
         return m({
             current: o < p.length ? o : p.length
         }), m({
             current: 0 <= o ? o : 0
-        }), F.a.createElement(Tn, {
+        }), H.a.createElement(Tn, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             "data-dash-is-loading": t && t.is_loading || void 0,
             current: o,
             direction: i,
             labelPlacement: l,
             progressDot: c,
@@ -107450,15 +107462,15 @@
             responsive: h,
             onChange: f ? function(t) {
                 return m({
                     current: t
                 })
             } : void 0
         }, p.map(function(t) {
-            return F.a.createElement(zn, {
+            return H.a.createElement(zn, {
                 title: t.title,
                 subTitle: t.subTitle,
                 description: t.description
             })
         }))
     }
     var En = function(t) {
@@ -107703,15 +107715,15 @@
             detail: void 0
         };
         var n = document.createEvent("CustomEvent");
         return n.initCustomEvent(t, e.bubbles, e.cancelable, e.detail), n
     }
 
     function ta(t, e) {
-        if (Object(W.isUndefined)(t) || Object(W.isNull)(t)) {
+        if (Object(V.isUndefined)(t) || Object(V.isNull)(t)) {
             if ("string" != typeof e) throw new TypeError(`Expected a \`string\`, got \`${typeof e}\``);
             return !In.test(e) && Rn.test(e)
         }
         return t
     }
     Qn.prototype = window.Event.prototype;
 
@@ -107749,67 +107761,67 @@
             }, []), function e(t, n) {
                 return Array.isArray(t) ? t = t.map(function(t) {
                     return e(t, n)
                 }) : t.hasOwnProperty("component") && (t = t.hasOwnProperty("children") ? (Object.assign(t, {
                     children: t.children.map(function(t) {
                         return e(t, n)
                     })
-                }), "SubMenu" === t.component ? F.a.createElement(Xn, {
+                }), "SubMenu" === t.component ? H.a.createElement(Xn, {
                     key: t.props.key,
                     title: t.props.title,
                     disabled: t.props.disabled,
-                    icon: F.a.createElement(R.a, {
+                    icon: H.a.createElement(I.a, {
                         icon: t.props.icon
                     })
-                }, t.children) : F.a.createElement(Zn, {
+                }, t.children) : H.a.createElement(Zn, {
                     key: t.props.key,
                     title: t.props.title,
                     disabled: t.props.disabled,
-                    icon: F.a.createElement(R.a, {
+                    icon: H.a.createElement(I.a, {
                         icon: t.props.icon
                     })
-                }, t.children)) : "Divider" === t.component ? F.a.createElement(Jn, {
+                }, t.children)) : "Divider" === t.component ? H.a.createElement(Jn, {
                     dashed: t.props && t.props.dashed
-                }) : t.props.href ? F.a.createElement($n, {
+                }) : t.props.href ? H.a.createElement($n, {
                     key: t.props.key,
                     title: t.props.title,
                     disabled: t.props.disabled,
                     danger: t.props.danger,
-                    icon: F.a.createElement(R.a, {
+                    icon: H.a.createElement(I.a, {
                         icon: t.props.icon
                     }),
                     name: t.props && t.props.name
-                }, F.a.createElement(ra, {
+                }, H.a.createElement(ra, {
                     href: t.props.href,
                     target: t.props.target
-                }, t.props.title)) : F.a.createElement($n, {
+                }, t.props.title)) : H.a.createElement($n, {
                     key: t.props.key,
                     title: t.props.title,
                     disabled: t.props.disabled,
                     danger: t.props.danger,
-                    icon: F.a.createElement(R.a, {
+                    icon: H.a.createElement(I.a, {
                         icon: t.props.icon
                     }),
                     name: t.props && t.props.name
                 }, t.props.title)), t
             }(i, oa));
-        return f ? F.a.createElement("div", {
+        return f ? H.a.createElement("div", {
             style: {
                 width: "100%"
             }
-        }, F.a.createElement(T.a, {
+        }, H.a.createElement(z.a, {
             type: "primary",
             onClick: function() {
                 return g({
                     inlineCollapsed: !m
                 })
             }
-        }, F.a.createElement((m ? Yn : Bn).a)), F.a.createElement(Nn.a, {
+        }, H.a.createElement((m ? Yn : Bn).a)), H.a.createElement(Nn.a, {
             id: n,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             mode: l,
             theme: c,
             selectedKeys: [u],
             openKeys: d,
             defaultOpenKeys: s,
@@ -107824,17 +107836,17 @@
                 return t.parentNode
             } : void 0,
             inlineCollapsed: m,
             persistence: b,
             persisted_props: v,
             persistence_type: y,
             "data-dash-is-loading": t && t.is_loading || void 0
-        }, i)) : F.a.createElement(Nn.a, {
+        }, i)) : H.a.createElement(Nn.a, {
             id: n,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             mode: l,
             theme: c,
             selectedKeys: [u],
             openKeys: d,
             defaultOpenKeys: s,
@@ -107870,17 +107882,17 @@
             p = t.forceRender,
             f = t.setProps,
             h = t.persistence,
             m = t.persisted_props,
             g = t.persistence_type,
             t = t.loading_state,
             n = j(n);
-        return F.a.createElement(la.a, {
+        return H.a.createElement(la.a, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             activeKey: l ? ["1"] : [],
             style: r,
             key: o,
             bordered: c,
             ghost: d,
             collapsible: u,
             onChange: function(t) {
@@ -107890,15 +107902,15 @@
                     isOpen: !1
                 })
             },
             persistence: h,
             persisted_props: m,
             persistence_type: g,
             "data-dash-is-loading": t && t.is_loading || void 0
-        }, F.a.createElement(ca, {
+        }, H.a.createElement(ca, {
             key: "1",
             header: i,
             showArrow: s,
             forceRender: p
         }, n))
     }
 
@@ -107910,17 +107922,17 @@
             o = t.key,
             i = t.align,
             l = t.gutter,
             c = t.justify,
             s = t.wrap,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return F.a.createElement(ua, {
+        return H.a.createElement(ua, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             align: i,
             gutter: l,
             justify: c,
             wrap: s,
             "data-dash-is-loading": t && t.is_loading || void 0
@@ -107968,15 +107980,15 @@
                                 return a
                             }(t, e);
                             if (Object.getOwnPropertySymbols)
                                 for (var r = Object.getOwnPropertySymbols(t), o = 0; o < r.length; o++) n = r[o], 0 <= e.indexOf(n) || Object.prototype.propertyIsEnumerable.call(t, n) && (a[n] = t[n]);
                             return a
                         }(t, Hn),
                         a = o && ta(a, o);
-                    return F.a.createElement("a", Wn({
+                    return H.a.createElement("a", Wn({
                         href: o,
                         target: a ? r : null,
                         download: i && a ? i : null
                     }, t, {
                         onClick: function(t) {
                             return e.updateLocation(t)
                         }
@@ -108034,15 +108046,15 @@
             style: n.a.object,
             key: n.a.string,
             title: n.a.node,
             isOpen: n.a.bool,
             bordered: n.a.bool,
             showArrow: n.a.bool,
             ghost: n.a.bool,
-            collapsible: n.a.oneOf(["header", "disabled"]),
+            collapsible: n.a.oneOf(["header", "disabled", "icon"]),
             forceRender: n.a.bool,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
@@ -108139,17 +108151,17 @@
             f = t.sm,
             h = t.md,
             m = t.lg,
             g = t.xl,
             b = t.xxl,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return F.a.createElement(pa, {
+        return H.a.createElement(pa, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: function(e) {
                 for (var t = 1; t < arguments.length; t++) {
                     var n = null != arguments[t] ? arguments[t] : {};
                     t % 2 ? ha(Object(n), !0).forEach(function(t) {
                         ma(e, t, n[t])
                     }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ha(Object(n)).forEach(function(t) {
                         Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
@@ -108180,68 +108192,68 @@
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return F.a.createElement(ka, {
+        return H.a.createElement(ka, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
     function va(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return F.a.createElement(Ma, {
+        return H.a.createElement(Ma, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
     function ya(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return F.a.createElement(Ca, {
+        return H.a.createElement(Ca, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
     function xa(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return F.a.createElement(La, {
+        return H.a.createElement(La, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
     function _a(t) {
@@ -108258,17 +108270,17 @@
             d = t.reverseArrow,
             p = t.theme,
             f = t.width,
             h = t.trigger,
             m = t.setProps,
             t = t.loading_state,
             n = j(n);
-        return F.a.createElement(Da, {
+        return H.a.createElement(Da, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             collapsed: l,
             collapsedWidth: c,
             collapsible: s,
             defaultCollapsed: u,
             reverseArrow: d,
@@ -108295,41 +108307,41 @@
             l = t.direction,
             c = t.size,
             s = t.split,
             u = t.wrap,
             d = t.addSplitLine,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return d ? "horizontal" === l ? F.a.createElement(za.b, {
+        return d ? "horizontal" === l ? H.a.createElement(za.b, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             align: i,
             direction: l,
             size: c,
-            split: F.a.createElement(b, {
+            split: H.a.createElement(b, {
                 type: "vertical"
             }),
             wrap: u,
             "data-dash-is-loading": t && t.is_loading || void 0
-        }, n) : F.a.createElement(za.b, {
+        }, n) : H.a.createElement(za.b, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             align: i,
             direction: l,
             size: c,
-            split: F.a.createElement(b, null),
+            split: H.a.createElement(b, null),
             wrap: u,
             "data-dash-is-loading": t && t.is_loading || void 0
-        }, n) : F.a.createElement(za.b, {
+        }, n) : H.a.createElement(za.b, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             align: i,
             direction: l,
             size: c,
             split: s,
             wrap: u,
@@ -108554,15 +108566,15 @@
             S = S && Wt.createElement(Wa.a, {
                 actionFn: n,
                 close: r,
                 autoFocus: "cancel" === z,
                 buttonProps: g,
                 prefixCls: "".concat(x, "-btn")
             }, m);
-        return Wt.createElement(H.a, {
+        return Wt.createElement(W.a, {
             prefixCls: x,
             iconPrefixCls: _,
             direction: b
         }, Wt.createElement(Xa, {
             prefixCls: v,
             className: A,
             wrapClassName: Kt()(Object(Vt.a)({}, "".concat(C, "-centered"), !!t.centered), y),
@@ -108636,15 +108648,15 @@
                 null != e && e(t)
             }
 
             function l(t) {
                 var e = o.onOk;
                 null != e && e(t)
             }
-            var t = Wt.useContext(G.b),
+            var t = Wt.useContext(q.b),
                 e = t.getPopupContainer,
                 n = t.getPrefixCls,
                 t = t.direction,
                 a = o.prefixCls,
                 r = o.footer,
                 c = o.visible,
                 s = o.open,
@@ -108672,17 +108684,17 @@
                 }, function(t) {
                     var e = o.okText,
                         n = o.okType,
                         n = void 0 === n ? "primary" : n,
                         a = o.cancelText,
                         r = o.confirmLoading,
                         r = void 0 !== r && r;
-                    return Wt.createElement(Wt.Fragment, null, Wt.createElement(T.a, Object(Et.a)({
+                    return Wt.createElement(Wt.Fragment, null, Wt.createElement(z.a, Object(Et.a)({
                         onClick: i
-                    }, o.cancelButtonProps), a || t.cancelText), Wt.createElement(T.a, Object(Et.a)({}, Object(Ua.a)(n), {
+                    }, o.cancelButtonProps), a || t.cancelText), Wt.createElement(z.a, Object(Et.a)({}, Object(Ua.a)(n), {
                         loading: r,
                         onClick: l
                     }, o.okButtonProps), null != e ? e : t.okText))
                 }),
                 f = Wt.createElement("span", {
                     className: "".concat(a, "-close-x")
                 }, f || Wt.createElement(Ze.a, {
@@ -108727,15 +108739,15 @@
                     for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                     if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                         for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                     return n
                 }(t, ["okText", "cancelText", "prefixCls"]);
             clearTimeout(e), e = setTimeout(function() {
                 var t = Object(qa.b)(),
-                    e = Object(H.b)(),
+                    e = Object(W.b)(),
                     n = e.getPrefixCls,
                     e = e.getIconPrefixCls,
                     n = n(void 0, Za),
                     a = i || "".concat(n, "-modal"),
                     e = e();
                 Object(Ha.a)(Wt.createElement(Aa, Object(Et.a)({}, l, {
                     prefixCls: a,
@@ -108835,15 +108847,15 @@
                 r = Object(Gt.a)(r, 2),
                 o = r[0],
                 i = r[1],
                 r = Wt.useState(t),
                 t = Object(Gt.a)(r, 2),
                 l = t[0],
                 c = t[1],
-                r = Wt.useContext(G.b),
+                r = Wt.useContext(q.b),
                 s = r.direction,
                 t = r.getPrefixCls,
                 u = t("modal"),
                 d = t();
             return Wt.useImperativeHandle(e, function() {
                 return {
                     destroy: n,
@@ -108928,21 +108940,21 @@
             M = t.okCounts,
             E = t.cancelCounts,
             C = t.closeCounts,
             S = t.confirmLoading,
             L = t.confirmAutoSpin,
             P = t.transitionType,
             t = t.loading_state,
-            D = Object(Wt.useContext)(U.a),
+            D = Object(Wt.useContext)(G.a),
             i = D && D.locale || i;
-        return F.a.createElement(H.a, {
-            locale: V.b.get(i)
-        }, F.a.createElement(dr, {
+        return H.a.createElement(W.a, {
+            locale: K.b.get(i)
+        }, H.a.createElement(dr, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: o,
             key: r,
             title: c,
             open: s,
             okText: S && h || f,
             cancelText: m,
             okButtonProps: d,
@@ -109169,15 +109181,15 @@
         e in t ? Object.defineProperty(t, e, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : t[e] = n
     }
-    xr = F.a.PureComponent, u = xr, (d = _r).prototype = Object.create(u.prototype), (d.prototype.constructor = d).__proto__ = u, (d = _r.prototype).componentDidMount = function() {
+    xr = H.a.PureComponent, u = xr, (d = _r).prototype = Object.create(u.prototype), (d.prototype.constructor = d).__proto__ = u, (d = _r.prototype).componentDidMount = function() {
         var t = this,
             e = this.props.delay,
             n = this.state,
             a = n.currentInterval,
             n = n.elements;
         0 < a && 1 < n.length && (this.tickDelay = sr(function() {
             t.tickLoop = sr(t.tick, a)
@@ -109186,23 +109198,23 @@
         var n = this,
             a = this.props,
             r = a.interval,
             o = a.children,
             a = a.delay,
             i = this.state.currentWordIndex,
             l = Array.isArray(r) ? r[i % r.length] : r;
-        e.currentInterval !== l && (this.clearTimeouts(), 0 < l && 1 < F.a.Children.count(o) ? this.tickDelay = sr(function() {
+        e.currentInterval !== l && (this.clearTimeouts(), 0 < l && 1 < H.a.Children.count(o) ? this.tickDelay = sr(function() {
             n.tickLoop = sr(n.tick, l)
         }, a) : this.setState(function(t, e) {
             t = t.currentWordIndex;
             return {
                 currentInterval: Array.isArray(e.interval) ? e.interval[t % e.interval.length] : e.interval
             }
         })), mr()(t.children, o) || this.setState({
-            elements: F.a.Children.toArray(o)
+            elements: H.a.Children.toArray(o)
         })
     }, d.componentWillUnmount = function() {
         this.isUnMounting = !0, this.clearTimeouts()
     }, d.clearTimeouts = function() {
         null != this.tickLoop && ur(this.tickLoop), null != this.tickDelay && ur(this.tickDelay)
     }, d.getOpacity = function() {
         return this.props.fade ? 0 : 1
@@ -109261,15 +109273,15 @@
             verticalAlign: "top"
         }))), yr(vr(e), "elementStyles", hr()({
             display: "inline-block",
             left: 0,
             top: 0,
             whiteSpace: e.props.noWrap ? "nowrap" : "normal"
         }));
-        var e, n = F.a.Children.toArray(t.children);
+        var e, n = H.a.Children.toArray(t.children);
         return e.state = {
             elements: n,
             currentEl: n[0],
             currentWordIndex: 0,
             wordCount: 0,
             currentInterval: Array.isArray(t.interval) ? t.interval[0] : t.interval
         }, e
@@ -109282,34 +109294,34 @@
             stiffness: 340,
             damping: 30
         },
         fade: !0,
         mask: !(d.render = function() {
             var a = this,
                 t = this.props.className;
-            return F.a.createElement("div", {
+            return H.a.createElement("div", {
                 className: this.wrapperStyles + " " + (void 0 === t ? "" : t)
-            }, F.a.createElement(fr.TransitionMotion, {
+            }, H.a.createElement(fr.TransitionMotion, {
                 willLeave: this.willLeave,
                 willEnter: this.willEnter,
                 styles: this.getTransitionMotionStyles()
             }, function(t) {
                 var e = a.getDimensions(),
                     n = e.height,
                     e = e.width,
                     e = null == a.wordBox ? "auto" : e,
                     n = null == a.wordBox ? "auto" : n;
-                return F.a.createElement("div", {
+                return H.a.createElement("div", {
                     style: {
                         transition: "width " + a.props.adjustingSpeed + "ms linear",
                         height: n,
                         width: e
                     }
                 }, t.map(function(t) {
-                    return F.a.createElement("div", {
+                    return H.a.createElement("div", {
                         className: a.elementStyles,
                         ref: function(t) {
                             a.wordBox = t
                         },
                         key: t.key,
                         style: {
                             opacity: t.style.opacity,
@@ -109383,15 +109395,15 @@
                     for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                 return n
             }(t, ["description", "prefixCls", "message", "banner", "className", "style", "onMouseEnter", "onMouseLeave", "onClick", "afterClose", "showIcon", "closable", "closeText", "closeIcon", "action"]),
             v = Wt.useState(!1),
             y = (t = Object(Gt.a)(v, 2))[0],
             x = t[1],
             _ = Wt.useRef(),
-            t = (v = Wt.useContext(G.b)).getPrefixCls,
+            t = (v = Wt.useContext(q.b)).getPrefixCls,
             v = v.direction,
             O = t("alert", e),
             w = !!h || f,
             k = void 0 !== (t = b.type) ? t : o ? "warning" : "info",
             j = !(!o || void 0 !== p) || p,
             M = Kt()(O, "".concat(O, "-").concat(k), (e = {}, Object(Vt.a)(e, "".concat(O, "-with-description"), !!a), Object(Vt.a)(e, "".concat(O, "-no-icon"), !j), Object(Vt.a)(e, "".concat(O, "-banner"), !!o), Object(Vt.a)(e, "".concat(O, "-rtl"), "rtl" === v), e), i),
             E = Object(Cr.a)(b);
@@ -109506,37 +109518,37 @@
             l = t.closable,
             c = t.message,
             s = t.messageRenderMode,
             u = t.description,
             d = t.action,
             p = t.banner,
             t = (t.setProps, t.loading_state);
-        return "loop-text" === s && Array.isArray(c) ? F.a.createElement(Kr, {
+        return "loop-text" === s && Array.isArray(c) ? H.a.createElement(Kr, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
-            message: F.a.createElement(Mr, {
+            message: H.a.createElement(Mr, {
                 mask: !0
             }, c.map(function(t) {
-                return F.a.createElement("div", null, t)
+                return H.a.createElement("div", null, t)
             })),
             type: o,
             description: u,
             showIcon: i,
             closable: l,
             action: d,
             banner: p,
             "data-dash-is-loading": t && t.is_loading || void 0
-        }) : F.a.createElement(Kr, {
+        }) : H.a.createElement(Kr, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
-            message: "marquee" === s ? F.a.createElement(Ur.a, {
+            message: "marquee" === s ? H.a.createElement(Ur.a, {
                 pauseOnHover: !0,
                 gradient: !1
             }, c) : c,
             type: o,
             description: u,
             showIcon: i,
             closable: l,
@@ -109556,31 +109568,31 @@
             c = t.placement,
             s = t.top,
             u = t.bottom,
             d = t.duration,
             p = t.closable,
             f = t.loading_state,
             h = (t.setProps, {
-                className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+                className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
                 style: a,
                 message: o,
                 description: i,
                 placement: c,
                 top: s,
                 bottom: u,
                 duration: d,
-                closeIcon: p ? void 0 : F.a.createElement("span", {
+                closeIcon: p ? void 0 : H.a.createElement("span", {
                     style: {
                         visibility: "hidden"
                     }
                 })
             });
         return Object(Wt.useEffect)(function() {
             "default" === l ? qr.a.open(h) : "success" === l ? qr.a.success(h) : "error" === l ? qr.a.error(h) : "info" === l ? qr.a.info(h) : "warning" === l && qr.a.warning(h)
-        }), F.a.createElement("div", {
+        }), H.a.createElement("div", {
             id: e,
             key: r,
             "data-dash-is-loading": f && f.is_loading || void 0
         })
     }
 
     function zr(t) {
@@ -109592,32 +109604,32 @@
             i = t.type,
             l = t.duration,
             c = t.icon,
             s = t.top,
             u = t.maxCount,
             d = t.loading_state,
             p = (t.setProps, Object(Wt.useEffect)(function() {
-                X.b.config({
+                $.b.config({
                     top: s,
                     maxCount: u
                 })
             }, []), {
-                className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+                className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
                 style: a,
                 content: o,
                 duration: l
             });
-        return c && (p.icon = F.a.createElement(R.a, {
+        return c && (p.icon = H.a.createElement(I.a, {
             icon: c,
             style: {
                 marginRight: 3
             }
         })), Object(Wt.useEffect)(function() {
-            "default" === i ? X.b.open(p) : "success" === i ? X.b.success(p) : "error" === i ? X.b.error(p) : "info" === i ? X.b.info(p) : "warning" === i && X.b.warning(p)
-        }), F.a.createElement("div", {
+            "default" === i ? $.b.open(p) : "success" === i ? $.b.success(p) : "error" === i ? $.b.error(p) : "info" === i ? $.b.info(p) : "warning" === i && $.b.warning(p)
+        }), H.a.createElement("div", {
             id: e,
             key: r,
             "data-dash-is-loading": d && d.is_loading || void 0
         })
     }
 
     function Ar(t) {
@@ -109626,22 +109638,22 @@
             a = t.style,
             r = t.key,
             o = t.content,
             i = t.color,
             l = t.href,
             c = t.target,
             t = (t.setProps, t.loading_state);
-        return F.a.createElement(Zr.a, {
+        return H.a.createElement(Zr.a, {
             id: e,
             key: r,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             color: i,
             "data-dash-is-loading": t && t.is_loading || void 0
-        }, l ? F.a.createElement("a", {
+        }, l ? H.a.createElement("a", {
             href: l,
             target: c
         }, o) : o)
     }
 
     function Rr(t, e) {
         return Wt.createElement(to.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
@@ -109675,15 +109687,15 @@
             a = t.subTitle,
             r = t.title,
             o = t.style,
             i = t.children,
             l = void 0 === (l = t.status) ? "info" : l,
             c = t.icon,
             t = t.extra,
-            s = (u = Wt.useContext(G.b)).getPrefixCls,
+            s = (u = Wt.useContext(q.b)).getPrefixCls,
             u = u.direction,
             s = s("result", e),
             e = Kt()(s, "".concat(s, "-").concat(l), n, Object(Vt.a)({}, "".concat(s, "-rtl"), "rtl" === u));
         return Wt.createElement("div", {
             className: e,
             style: o
         }, Wt.createElement(Ir, {
@@ -109708,20 +109720,20 @@
             a = t.style,
             r = t.key,
             o = t.status,
             i = t.title,
             l = t.subTitle,
             c = t.icon,
             s = t.loading_state;
-        return t.setProps, F.a.createElement(ro, {
+        return t.setProps, H.a.createElement(ro, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
-            icon: c || ("loading" === o ? F.a.createElement(oo.a, {
+            icon: c || ("loading" === o ? H.a.createElement(oo.a, {
                 style: {
                     color: "#1890ff"
                 }
             }) : void 0),
             status: o,
             title: i,
             subTitle: l,
@@ -109771,15 +109783,15 @@
             E = t.debounceWait,
             C = t.readOnly,
             S = t.setProps,
             L = t.loading_state,
             P = t.persistence,
             D = t.persisted_props,
             t = t.persistence_type,
-            T = Object(Wt.useContext)(U.a),
+            T = Object(Wt.useContext)(G.a),
             z = (Object(Wt.useEffect)(function() {
                 y && !d && S({
                     value: y,
                     md5Value: lo()(y)
                 }), d && S({
                     md5Value: lo()(d)
                 })
@@ -109789,53 +109801,53 @@
                 })
             }, {
                 debounceWait: Math.max(E, 200),
                 manual: !0
             }).run);
         return "default" === l ? React.createElement(Ae.a, {
             id: a,
-            className: Object(W.isString)(r) ? r : r ? Object(K.a)(r) : void 0,
+            className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
             style: o,
             key: i,
             placeholder: u,
             autoComplete: s,
             value: d,
-            size: T && !Object(W.isUndefined)(T.componentSize) ? T.componentSize : p,
+            size: T && !Object(V.isUndefined)(T.componentSize) ? T.componentSize : p,
             addonBefore: f,
             addonAfter: h,
             prefix: m,
             suffix: g,
             allowClear: b,
             bordered: v,
             defaultValue: y,
-            disabled: T && !Object(W.isUndefined)(T.componentDisabled) ? T.componentDisabled : x,
+            disabled: T && !Object(V.isUndefined)(T.componentDisabled) ? T.componentDisabled : x,
             maxLength: _,
             status: j,
             readOnly: C,
             onChange: function(t) {
                 e(t), z(t.target.value)
             },
             onPressEnter: n,
             persistence: P,
             persisted_props: D,
             persistence_type: t,
             "data-dash-is-loading": L && L.is_loading || void 0
         }) : "search" === l ? React.createElement(co, {
             id: a,
-            className: Object(W.isString)(r) ? r : r ? Object(K.a)(r) : void 0,
+            className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
             style: o,
             key: i,
             placeholder: u,
             autoComplete: s,
-            size: T && !Object(W.isUndefined)(T.componentSize) ? T.componentSize : p,
+            size: T && !Object(V.isUndefined)(T.componentSize) ? T.componentSize : p,
             allowClear: b,
             bordered: v,
             value: d,
             defaultValue: y,
-            disabled: T && !Object(W.isUndefined)(T.componentDisabled) ? T.componentDisabled : x,
+            disabled: T && !Object(V.isUndefined)(T.componentDisabled) ? T.componentDisabled : x,
             maxLength: _,
             status: j,
             readOnly: C,
             onSearch: function(t) {
                 S({
                     nClicksSearch: w + 1
                 })
@@ -109846,25 +109858,25 @@
             onPressEnter: n,
             persistence: P,
             persisted_props: D,
             persistence_type: t,
             "data-dash-is-loading": L && L.is_loading || void 0
         }) : "text-area" === l ? React.createElement(so, {
             id: a,
-            className: Object(W.isString)(r) ? r : r ? Object(K.a)(r) : void 0,
+            className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
             style: o,
             key: i,
             placeholder: u,
             autoComplete: s,
-            size: T && !Object(W.isUndefined)(T.componentSize) ? T.componentSize : p,
+            size: T && !Object(V.isUndefined)(T.componentSize) ? T.componentSize : p,
             allowClear: b,
             bordered: v,
             value: d,
             defaultValue: y,
-            disabled: T && !Object(W.isUndefined)(T.componentDisabled) ? T.componentDisabled : x,
+            disabled: T && !Object(V.isUndefined)(T.componentDisabled) ? T.componentDisabled : x,
             maxLength: _,
             showCount: O,
             status: j,
             autoSize: M,
             readOnly: C,
             onChange: function(t) {
                 e(t), z(t.target.value)
@@ -109872,22 +109884,22 @@
             onPressEnter: n,
             persistence: P,
             persisted_props: D,
             persistence_type: t,
             "data-dash-is-loading": L && L.is_loading || void 0
         }) : "password" === l ? React.createElement(Ae.a.Password, {
             id: a,
-            className: Object(W.isString)(r) ? r : r ? Object(K.a)(r) : void 0,
+            className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
             style: o,
             key: i,
             placeholder: u,
             autoComplete: s,
-            size: T && !Object(W.isUndefined)(T.componentSize) ? T.componentSize : p,
+            size: T && !Object(V.isUndefined)(T.componentSize) ? T.componentSize : p,
             bordered: v,
-            disabled: T && !Object(W.isUndefined)(T.componentDisabled) ? T.componentDisabled : x,
+            disabled: T && !Object(V.isUndefined)(T.componentDisabled) ? T.componentDisabled : x,
             value: d,
             defaultValue: y,
             maxLength: _,
             status: j,
             prefix: m,
             suffix: g,
             readOnly: C,
@@ -109921,25 +109933,25 @@
             g = t.arrowPointAtCenter,
             b = t.open,
             v = t.permanent,
             y = t.popupContainer,
             x = t.setProps,
             t = t.loading_state,
             n = j(n);
-        return F.a.createElement(D.a, {
+        return H.a.createElement(D.a, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             title: i,
             placement: l,
             color: c,
             mouseEnterDelay: s,
             mouseLeaveDelay: u,
-            overlayClassName: Object(W.isString)(d) ? d : d ? Object(K.a)(d) : void 0,
+            overlayClassName: Object(V.isString)(d) ? d : d ? Object(U.a)(d) : void 0,
             overlayStyle: p,
             overlayInnerStyle: f,
             trigger: h,
             zIndex: m,
             arrowPointAtCenter: g,
             open: b,
             onOpenChange: v ? void 0 : function(t) {
@@ -109964,26 +109976,26 @@
             l = t.checked,
             c = t.indeterminate,
             s = t.setProps,
             u = t.persistence,
             d = t.persisted_props,
             p = t.persistence_type,
             t = t.loading_state,
-            f = Object(Wt.useContext)(U.a);
-        return F.a.createElement(we.a, {
+            f = Object(Wt.useContext)(G.a);
+        return H.a.createElement(we.a, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: n,
             key: r,
             onChange: function(t) {
                 s({
                     checked: t.target.checked
                 })
             },
-            disabled: f && !Object(W.isUndefined)(f.componentDisabled) ? f.componentDisabled : i,
+            disabled: f && !Object(V.isUndefined)(f.componentDisabled) ? f.componentDisabled : i,
             checked: l,
             indeterminate: c,
             persistence: u,
             persisted_props: d,
             persistence_type: p,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, o)
@@ -109998,23 +110010,23 @@
             i = t.value,
             l = t.disabled,
             c = t.setProps,
             s = t.persistence,
             u = t.persisted_props,
             d = t.persistence_type,
             t = t.loading_state,
-            p = Object(Wt.useContext)(U.a);
-        return F.a.createElement(we.a.Group, {
+            p = Object(Wt.useContext)(G.a);
+        return H.a.createElement(we.a.Group, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: n,
             key: r,
             options: o,
             value: i,
-            disabled: p && !Object(W.isUndefined)(p.componentDisabled) ? p.componentDisabled : l,
+            disabled: p && !Object(V.isUndefined)(p.componentDisabled) ? p.componentDisabled : l,
             onChange: function(t) {
                 c({
                     value: t
                 })
             },
             persistence: s,
             persisted_props: u,
@@ -110075,15 +110087,15 @@
             type: "default",
             placement: "topRight",
             top: 24,
             bottom: 24,
             duration: 4.5,
             closable: !0
         }, Tr),
-        X = e(308),
+        $ = e(308),
         $r = (zr.propTypes = {
             id: n.a.string,
             className: n.a.string,
             style: n.a.object,
             key: n.a.string,
             content: n.a.string,
             type: n.a.oneOf(["default", "success", "error", "info", "warning"]),
@@ -111110,19 +111122,19 @@
             }())[0],
             v = t[1],
             y = Object(Wt.useRef)();
         return Object(Wt.useEffect)(function() {
             u && (y.current && clearTimeout(y.current), u.is_loading && !b ? "default" === p ? (m && console.log(u.component_name + "." + u.prop_name), v(!0)) : "exclude" === p ? -1 === f.indexOf(u.component_name + "." + u.prop_name) && (m && console.log(u.component_name + "." + u.prop_name), v(!0)) : "include" === p && -1 !== h.indexOf(u.component_name + "." + u.prop_name) && (m && console.log(u.component_name + "." + u.prop_name), v(!0)) : !u.is_loading && b && (y.current = setTimeout(function() {
                 return v(!1)
             })))
-        }, [u]), F.a.createElement(E.a, {
+        }, [u]), H.a.createElement(E.a, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             key: o,
-            wrapperClassName: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            wrapperClassName: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             spinning: b,
             size: c,
             delay: s,
             tip: d,
             indicator: g,
             "data-dash-is-loading": u && u.is_loading || void 0
@@ -111141,25 +111153,25 @@
             s = t.size,
             u = t.loading,
             d = t.setProps,
             p = t.persistence,
             f = t.persisted_props,
             h = t.persistence_type,
             t = t.loading_state,
-            m = Object(Wt.useContext)(U.a);
+            m = Object(Wt.useContext)(G.a);
         return Object(Wt.useEffect)(function() {
-            Object(W.isUndefined)(i) && d({
+            Object(V.isUndefined)(i) && d({
                 checked: !1
             })
-        }, []), F.a.createElement(wo.a, {
+        }, []), H.a.createElement(wo.a, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: n,
             key: r,
-            disabled: m && !Object(W.isUndefined)(m.componentDisabled) ? m.componentDisabled : o,
+            disabled: m && !Object(V.isUndefined)(m.componentDisabled) ? m.componentDisabled : o,
             defaultChecked: i,
             checkedChildren: l,
             checked: i,
             unCheckedChildren: c,
             size: s,
             loading: u,
             onChange: function(t) {
@@ -111187,22 +111199,22 @@
             u = t.disabled,
             d = t.mark,
             p = t.strong,
             f = t.italic,
             h = t.underline,
             m = t.type,
             t = (t.setProps, t.loading_state),
-            g = Object(Wt.useContext)(U.a),
+            g = Object(Wt.useContext)(G.a),
             i = g && g.locale || i,
             n = j(n);
-        return F.a.createElement(H.a, {
-            locale: V.b.get(i)
-        }, F.a.createElement(jo, {
+        return H.a.createElement(W.a, {
+            locale: K.b.get(i)
+        }, H.a.createElement(jo, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             code: l,
             copyable: c,
             delete: s,
             disabled: u,
             mark: d,
@@ -111228,22 +111240,22 @@
             d = t.mark,
             p = t.strong,
             f = t.italic,
             h = t.underline,
             m = t.type,
             g = t.keyboard,
             t = (t.setProps, t.loading_state),
-            b = Object(Wt.useContext)(U.a),
+            b = Object(Wt.useContext)(G.a),
             i = b && b.locale || i,
             n = j(n);
-        return F.a.createElement(H.a, {
-            locale: V.b.get(i)
-        }, F.a.createElement(Eo, {
+        return H.a.createElement(W.a, {
+            locale: K.b.get(i)
+        }, H.a.createElement(Eo, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             code: l,
             copyable: c,
             delete: s,
             disabled: u,
             mark: d,
@@ -111271,22 +111283,22 @@
             p = t.mark,
             f = t.strong,
             h = t.italic,
             m = t.underline,
             g = t.type,
             b = t.keyboard,
             t = (t.setProps, t.loading_state),
-            v = Object(Wt.useContext)(U.a),
+            v = Object(Wt.useContext)(G.a),
             i = v && v.locale || i,
             n = j(n);
-        return F.a.createElement(H.a, {
-            locale: V.b.get(i)
-        }, F.a.createElement(So, {
+        return H.a.createElement(W.a, {
+            locale: K.b.get(i)
+        }, H.a.createElement(So, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             level: l,
             code: c,
             copyable: s,
             delete: u,
             disabled: d,
@@ -111308,15 +111320,15 @@
             o = t.tab,
             i = t.key,
             l = t.disabled,
             c = t.closable,
             s = t.titleSideInfoPopover,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return F.a.createElement("div", {
+        return H.a.createElement("div", {
             id: e,
             className: a,
             style: r,
             tab: o,
             key: i,
             titleSideInfoPopover: s,
             disabled: l,
@@ -111495,21 +111507,21 @@
         return a
     };
     var zo, Ao = function t(e, n) {
             switch (arguments.length) {
                 case 0:
                     return t;
                 case 1:
-                    return I(e) ? t : N(function(t) {
+                    return R(e) ? t : N(function(t) {
                         return zo(e, t)
                     });
                 default:
-                    return I(e) && I(n) ? t : I(e) ? N(function(t) {
+                    return R(e) && R(n) ? t : R(e) ? N(function(t) {
                         return zo(t, n)
-                    }) : I(n) ? N(function(t) {
+                    }) : R(n) ? N(function(t) {
                         return zo(e, t)
                     }) : zo(e, n)
             }
         },
         Ro = ["id", "className", "style", "tab", "key", "disabled", "closable", "titleSideInfoPopover", "loading_state"];
 
     function Io(t) {
@@ -111604,17 +111616,17 @@
             p && !f && _({
                 activeKey: p
             })
         }, []), c ? (s && (c = c.map(function(t) {
             return s.includes(t.key) ? Bo(Bo({}, t), {}, {
                 disabled: !0
             }) : t
-        })), F.a.createElement(Do.a, {
+        })), H.a.createElement(Do.a, {
             id: a,
-            className: Object(W.isString)(o) ? o : o ? Object(K.a)(o) : void 0,
+            className: Object(V.isString)(o) ? o : o ? Object(U.a)(o) : void 0,
             style: i,
             key: l,
             items: c,
             defaultActiveKey: p,
             activeKey: f,
             size: h,
             tabPosition: m,
@@ -111654,50 +111666,50 @@
                         for (var n, a = {}, r = Object.keys(t), o = 0; o < r.length; o++) n = r[o], 0 <= e.indexOf(n) || (a[n] = t[n]);
                         return a
                     }(t, e);
                     if (Object.getOwnPropertySymbols)
                         for (var r = Object.getOwnPropertySymbols(t), o = 0; o < r.length; o++) n = r[o], 0 <= e.indexOf(n) || Object.prototype.propertyIsEnumerable.call(t, n) && (a[n] = t[n]);
                     return a
                 }(e, Ro);
-            return F.a.createElement(Wo, No({
+            return H.a.createElement(Wo, No({
                 id: n,
                 className: a,
                 style: r,
-                tab: s && s.content ? F.a.createElement(F.a.Fragment, null, F.a.createElement("span", null, o), F.a.createElement(To.a, {
+                tab: s && s.content ? H.a.createElement(H.a.Fragment, null, H.a.createElement("span", null, o), H.a.createElement(To.a, {
                     title: s.title,
-                    content: F.a.createElement("div", {
+                    content: H.a.createElement("div", {
                         style: {
                             maxWidth: "250px",
                             wordWrap: "break-word",
                             whiteSpace: "normal",
                             wordBreak: "break-all"
                         }
                     }, s.content),
                     overlayStyle: {
                         maxWidth: "250px"
                     },
                     placement: "right",
                     getPopupContainer: function(t) {
                         return t.parentNode.parentNode.parentNode.parentNode.parentNode.parentNode
                     }
-                }, F.a.createElement(Fa.a, {
+                }, H.a.createElement(Fa.a, {
                     style: {
                         color: "#8c8c8c",
                         paddingLeft: "4px",
                         cursor: "pointer"
                     }
                 }))) : o,
                 key: i,
                 disabled: l,
                 closable: c,
                 loading_state: u
             }, Ao(["setProps", "persistence", "persistence_type", "persisted_props"], e)), t)
-        }), F.a.createElement(Do.a, {
+        }), H.a.createElement(Do.a, {
             id: a,
-            className: Object(W.isString)(o) ? o : o ? Object(K.a)(o) : void 0,
+            className: Object(V.isString)(o) ? o : o ? Object(U.a)(o) : void 0,
             style: i,
             key: l,
             defaultActiveKey: p,
             activeKey: f,
             size: h,
             tabPosition: m,
             type: g,
@@ -111743,40 +111755,40 @@
             y = t.total,
             x = t.showTotal,
             _ = t.setProps,
             O = t.loading_state,
             w = t.persistence,
             k = t.persisted_props,
             t = t.persistence_type,
-            j = Object(Wt.useContext)(U.a),
+            j = Object(Wt.useContext)(G.a),
             o = j && j.locale || o;
         return Object(Wt.useEffect)(function() {
             i && !c && _({
                 current: i
             }), l && !s && _({
                 pageSize: l
             })
-        }, []), F.a.createElement(H.a, {
-            locale: V.b.get(o)
-        }, F.a.createElement(Me.a, {
+        }, []), H.a.createElement(W.a, {
+            locale: K.b.get(o)
+        }, H.a.createElement(Me.a, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: n,
             key: r,
             pageSize: s || l,
             defaultCurrent: i,
             defaultPageSize: l,
             current: c,
-            disabled: j && !Object(W.isUndefined)(j.componentDisabled) ? j.componentDisabled : u,
+            disabled: j && !Object(V.isUndefined)(j.componentDisabled) ? j.componentDisabled : u,
             hideOnSinglePage: d,
             pageSizeOptions: p,
             showQuickJumper: f,
             showSizeChanger: h,
             showTotal: x ? function(t) {
-                return "".concat(m || V.a.AntdPagination[o].showTotalPrefix, " ").concat(t.toString(), " ").concat(g || V.a.AntdPagination[o].showTotalSuffix)
+                return "".concat(m || K.a.AntdPagination[o].showTotalPrefix, " ").concat(t.toString(), " ").concat(g || K.a.AntdPagination[o].showTotalSuffix)
             } : void 0,
             simple: b,
             size: v,
             total: y,
             onChange: function(t, e) {
                 _({
                     current: t,
@@ -111999,29 +112011,29 @@
             return Wt.useImperativeHandle(t, function() {
                 var t;
                 return {
                     scrollTo: null == (t = E.current) ? void 0 : t.scrollTo,
                     onKeyDown: function(t) {
                         var e, n;
                         switch (t.which) {
-                            case q.a.UP:
-                            case q.a.DOWN:
-                            case q.a.LEFT:
-                            case q.a.RIGHT:
+                            case X.a.UP:
+                            case X.a.DOWN:
+                            case X.a.LEFT:
+                            case X.a.RIGHT:
                                 null != (n = E.current) && n.onKeyDown(t);
                                 break;
-                            case q.a.ENTER:
+                            case X.a.ENTER:
                                 A && (e = (n = (null == A ? void 0 : A.node) || {}).selectable, n = n.value, !1 !== e) && a(0, {
                                     node: {
                                         key: z
                                     },
                                     selected: !y.includes(n)
                                 });
                                 break;
-                            case q.a.ESC:
+                            case X.a.ESC:
                                 l(!1)
                         }
                     },
                     onKeyUp: function() {}
                 }
             }), 0 === C.length ? Wt.createElement("div", {
                 role: "listbox",
@@ -112553,15 +112565,15 @@
                 t = function(t, e) {
                     var n = {};
                     for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                     if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                         for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                     return n
                 }(t, ["prefixCls", "size", "disabled", "bordered", "className", "treeCheckable", "multiple", "listHeight", "listItemHeight", "placement", "notFoundContent", "switcherIcon", "treeLine", "getPopupContainer", "dropdownClassName", "popupClassName", "treeIcon", "transitionName", "choiceTransitionName", "status", "showArrow", "treeExpandAction"]),
-                w = Wt.useContext(G.b),
+                w = Wt.useContext(q.b),
                 I = w.getPopupContainer,
                 k = w.getPrefixCls,
                 j = w.renderEmpty,
                 M = w.direction,
                 N = w.virtual,
                 w = w.dropdownMatchSelectWidth,
                 E = Wt.useContext(fi.b),
@@ -112710,45 +112722,45 @@
             D = t.showCheckedStrategy,
             T = t.dropdownBefore,
             z = t.dropdownAfter,
             R = t.persistence,
             I = t.persisted_props,
             N = t.persistence_type,
             t = t.loading_state,
-            A = Object(Wt.useContext)(U.a),
+            A = Object(Wt.useContext)(G.a),
             o = A && A.locale || o,
             Y = (Object(Wt.useEffect)(function() {
                 !f && h && L({
                     value: h
                 }), !O && _ && L({
                     treeExpandedKeys: _
                 })
             }, []), Object(Wt.useMemo)(function() {
                 return B(i)
             }, [i]));
-        return React.createElement(H.a, {
-            locale: V.b.get(o)
+        return React.createElement(W.a, {
+            locale: K.b.get(o)
         }, React.createElement(gi, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: yi({
                 width: "100%"
             }, n),
             key: r,
             treeData: "flat" === l ? Y : i,
-            allowClear: Object(W.isUndefined)(P) ? c : !P,
+            allowClear: Object(V.isUndefined)(P) ? c : !P,
             bordered: s,
             treeLine: u,
             listHeight: d,
             placeholder: p,
             value: f,
             defaultValue: h,
             maxTagCount: m,
             multiple: g,
-            size: A && !Object(W.isUndefined)(A.componentSize) ? A.componentSize : b,
+            size: A && !Object(V.isUndefined)(A.componentSize) ? A.componentSize : b,
             treeCheckable: v,
             showCheckedStrategy: Oi.get(D),
             treeCheckStrictly: y,
             treeDefaultExpandAll: x,
             treeDefaultExpandedKeys: _,
             treeExpandedKeys: O,
             onChange: function(t) {
@@ -112758,15 +112770,15 @@
                     })
                 } : {
                     value: t
                 })
             },
             showSearch: !0,
             virtual: w,
-            disabled: A && !Object(W.isUndefined)(A.componentDisabled) ? A.componentDisabled : k,
+            disabled: A && !Object(V.isUndefined)(A.componentDisabled) ? A.componentDisabled : k,
             placement: j,
             status: M,
             treeNodeFilterProp: E,
             autoClearSearchValue: C,
             dropdownRender: T || z ? function(t) {
                 return React.createElement(React.Fragment, null, T, t, z)
             } : void 0,
@@ -112778,15 +112790,15 @@
             persistence: R,
             persisted_props: I,
             persistence_type: N,
             "data-dash-is-loading": t && t.is_loading || void 0,
             getPopupContainer: "parent" === S ? function(t) {
                 return t.parentNode
             } : void 0,
-            open: !(!Object(W.isUndefined)(P) && P) && void 0
+            open: !(!Object(V.isUndefined)(P) && P) && void 0
         }))
     }
 
     function _i(t) {
         var e = t.prefixCls,
             n = t.className,
             a = t.style,
@@ -112933,15 +112945,15 @@
             y = t.footerStyle,
             x = t.prefixCls,
             _ = t.getContainer,
             O = t.extra,
             w = t.afterVisibleChange,
             k = t.afterOpenChange,
             t = Di(t, ["width", "height", "size", "closable", "mask", "push", "closeIcon", "bodyStyle", "drawerStyle", "className", "visible", "open", "children", "style", "title", "headerStyle", "onClose", "footer", "footerStyle", "prefixCls", "getContainer", "extra", "afterVisibleChange", "afterOpenChange"]),
-            j = (E = Wt.useContext(G.b)).getPopupContainer,
+            j = (E = Wt.useContext(q.b)).getPopupContainer,
             M = E.getPrefixCls,
             E = E.direction,
             C = M("drawer", x),
             M = void 0 === _ && j ? function() {
                 return j(document.body)
             } : _,
             x = r && Wt.createElement("button", {
@@ -113140,22 +113152,22 @@
                 style: m,
                 tabIndex: -1,
                 ref: E,
                 onKeyDown: function(t) {
                     var e, n = t.keyCode,
                         a = t.shiftKey;
                     switch (n) {
-                        case q.a.TAB:
-                            n === q.a.TAB && (a || document.activeElement !== S.current ? a && document.activeElement === C.current && null != (e = S.current) && e.focus({
+                        case X.a.TAB:
+                            n === X.a.TAB && (a || document.activeElement !== S.current ? a && document.activeElement === C.current && null != (e = S.current) && e.focus({
                                 preventScroll: !0
                             }) : null != (e = C.current) && e.focus({
                                 preventScroll: !0
                             }));
                             break;
-                        case q.a.ESC:
+                        case X.a.ESC:
                             M && s && (t.stopPropagation(), M(t))
                     }
                 }
             }, e, Wt.createElement("div", {
                 tabIndex: 0,
                 ref: C,
                 style: Ci,
@@ -113297,17 +113309,17 @@
             h = t.mask,
             m = t.maskClosable,
             g = t.width,
             b = t.zIndex,
             v = t.extra,
             y = t.setProps,
             t = t.loading_state;
-        return F.a.createElement(Si, {
+        return H.a.createElement(Si, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: p ? Ri(Ri({}, r), {
                 position: "absolute"
             }) : r,
             key: o,
             open: i,
             title: l,
             placement: c,
@@ -113348,32 +113360,32 @@
             f = t.overlayStyle,
             h = t.overlayInnerStyle,
             m = t.trigger,
             g = t.zIndex,
             b = t.popupContainer,
             t = t.loading_state,
             n = j(n);
-        return F.a.createElement(To.a, {
+        return H.a.createElement(To.a, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
-            title: i && i.content ? F.a.createElement("div", null, F.a.createElement(R.a, {
+            title: i && i.content ? H.a.createElement("div", null, H.a.createElement(I.a, {
                 icon: i.prefixIcon
-            }), F.a.createElement("span", {
+            }), H.a.createElement("span", {
                 style: {
                     marginLeft: "5px"
                 }
             }, i.content)) : i,
             content: l,
             placement: c,
             color: s,
             mouseEnterDelay: u,
             mouseLeaveDelay: d,
-            overlayClassName: Object(W.isString)(p) ? p : p ? Object(K.a)(p) : void 0,
+            overlayClassName: Object(V.isString)(p) ? p : p ? Object(U.a)(p) : void 0,
             overlayStyle: f,
             overlayInnerStyle: h,
             trigger: m,
             zIndex: g,
             getPopupContainer: "parent" === b ? function(t) {
                 return t.parentNode
             } : void 0,
@@ -113388,21 +113400,21 @@
             r = t.style,
             o = t.key,
             i = t.locale,
             l = t.description,
             c = t.image,
             s = t.imageStyle,
             t = (t.setProps, t.loading_state),
-            u = Object(Wt.useContext)(U.a),
+            u = Object(Wt.useContext)(G.a),
             i = u && u.locale || i;
-        return F.a.createElement(H.a, {
-            locale: V.b.get(i)
-        }, F.a.createElement(Hi.a, {
+        return H.a.createElement(W.a, {
+            locale: K.b.get(i)
+        }, H.a.createElement(Hi.a, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             description: l,
             image: Wi.get(c) || c,
             imageStyle: s,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n))
@@ -113727,41 +113739,41 @@
             g = n[1],
             b = n[2];
         Wt.useImperativeHandle(t, function() {
             return {
                 onKeyDown: function(t) {
                     var e = t.which;
                     switch (e) {
-                        case q.a.UP:
-                        case q.a.DOWN:
+                        case X.a.UP:
+                        case X.a.DOWN:
                             var n = 0;
-                            e === q.a.UP ? n = -1 : e === q.a.DOWN && (n = 1), 0 !== n && function(t) {
+                            e === X.a.UP ? n = -1 : e === X.a.DOWN && (n = 1), 0 !== n && function(t) {
                                 var e = b.length,
                                     n = g; - 1 === n && t < 0 && (n = e);
                                 for (var a = 0; a < e; a += 1) {
                                     var r = b[n = (n + t + e) % e];
                                     if (r && !r.disabled) return r = r[s.value], r = m.slice(0, -1).concat(r), o(r)
                                 }
                             }(n);
                             break;
-                        case q.a.LEFT:
+                        case X.a.LEFT:
                             (f ? i : r)();
                             break;
-                        case q.a.RIGHT:
+                        case X.a.RIGHT:
                             (f ? r : i)();
                             break;
-                        case q.a.BACKSPACE:
+                        case X.a.BACKSPACE:
                             l || r();
                             break;
-                        case q.a.ENTER:
+                        case X.a.ENTER:
                             m.length && ((n = (null == (n = b[g]) ? void 0 : n[tl]) || []).length ? a(n.map(function(t) {
                                 return t[s.value]
                             }), n[n.length - 1]) : a(m, b[g]));
                             break;
-                        case q.a.ESC:
+                        case X.a.ESC:
                             d(!1), p && t.stopPropagation()
                     }
                 },
                 onKeyUp: function() {}
             }
         })
     }
@@ -113951,47 +113963,47 @@
             O = t.popupContainer,
             w = t.readOnly,
             k = t.setProps,
             j = t.persistence,
             M = t.persisted_props,
             E = t.persistence_type,
             t = t.loading_state,
-            C = Object(Wt.useContext)(U.a),
+            C = Object(Wt.useContext)(G.a),
             o = C && C.locale || o,
             S = (Object(Wt.useEffect)(function() {
                 f && !h && k({
                     value: f
                 })
             }, []), Object(Wt.useMemo)(function() {
                 return B(i)
             }, [i]));
-        return "flat" === l && (i = S), React.createElement(H.a, {
-            locale: V.b.get(o)
+        return "flat" === l && (i = S), React.createElement(W.a, {
+            locale: K.b.get(o)
         }, React.createElement(vl, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: n,
             key: r,
             options: i,
             changeOnSelect: c,
-            size: C && !Object(W.isUndefined)(C.componentSize) ? C.componentSize : s,
+            size: C && !Object(V.isUndefined)(C.componentSize) ? C.componentSize : s,
             bordered: u,
-            disabled: C && !Object(W.isUndefined)(C.componentDisabled) ? C.componentDisabled : d,
+            disabled: C && !Object(V.isUndefined)(C.componentDisabled) ? C.componentDisabled : d,
             placeholder: p,
             defaultValue: f,
             value: h,
             placement: m,
             maxTagCount: g,
             multiple: b,
             persistence: j,
             persisted_props: M,
             persistence_type: E,
             expandTrigger: v,
             status: y,
-            allowClear: Object(W.isUndefined)(w) ? x : !w,
+            allowClear: Object(V.isUndefined)(w) ? x : !w,
             showCheckedStrategy: yl.get(_),
             showSearch: function(e, t) {
                 return t.some(function(t) {
                     return -1 < t.label.toLowerCase().indexOf(e.toLowerCase())
                 })
             },
             onChange: function(t) {
@@ -113999,15 +114011,15 @@
                     value: t
                 })
             },
             "data-dash-is-loading": t && t.is_loading || void 0,
             getPopupContainer: "parent" === O ? function(t) {
                 return t.parentNode
             } : void 0,
-            open: !(!Object(W.isUndefined)(w) && w) && void 0
+            open: !(!Object(V.isUndefined)(w) && w) && void 0
         }))
     }
 
     function sl(t) {
         function e(t) {
             h({
                 value: t.target.value
@@ -114026,56 +114038,56 @@
             p = t.disabled,
             f = t.size,
             h = t.setProps,
             m = t.persistence,
             g = t.persisted_props,
             b = t.persistence_type,
             t = t.loading_state,
-            v = Object(Wt.useContext)(U.a);
+            v = Object(Wt.useContext)(G.a);
         return Object(Wt.useEffect)(function() {
             l && !c && h({
                 value: l
             })
-        }, []), "vertical" === s ? F.a.createElement(_l.a.Group, {
+        }, []), "vertical" === s ? H.a.createElement(_l.a.Group, {
             id: n,
-            className: Object(W.isString)(r) ? r : r ? Object(K.a)(r) : void 0,
+            className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
             style: a,
             key: o,
             defaultValue: l,
             value: c,
             buttonStyle: d,
-            disabled: v && !Object(W.isUndefined)(v.componentDisabled) ? v.componentDisabled : p,
-            size: v && !Object(W.isUndefined)(v.componentSize) ? v.componentSize : f,
+            disabled: v && !Object(V.isUndefined)(v.componentDisabled) ? v.componentDisabled : p,
+            size: v && !Object(V.isUndefined)(v.componentSize) ? v.componentSize : f,
             persistence: m,
             persisted_props: g,
             persistence_type: b,
             onChange: e,
             "data-dash-is-loading": t && t.is_loading || void 0
-        }, F.a.createElement(za.b, {
+        }, H.a.createElement(za.b, {
             direction: "vertical"
         }, i.map(function(t) {
-            return "button" !== u ? F.a.createElement(_l.a, {
+            return "button" !== u ? H.a.createElement(_l.a, {
                 value: t.value,
                 disabled: t.disabled
-            }, t.label) : F.a.createElement(_l.a.Button, {
+            }, t.label) : H.a.createElement(_l.a.Button, {
                 value: t.value,
                 disabled: t.disabled
             }, t.label)
-        }))) : F.a.createElement(_l.a.Group, {
+        }))) : H.a.createElement(_l.a.Group, {
             id: n,
-            className: Object(W.isString)(r) ? r : r ? Object(K.a)(r) : void 0,
+            className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
             style: a,
             key: o,
             options: i,
             defaultValue: l,
             value: c,
             optionType: u,
             buttonStyle: d,
-            disabled: v && !Object(W.isUndefined)(v.componentDisabled) ? v.componentDisabled : p,
-            size: v && !Object(W.isUndefined)(v.componentSize) ? v.componentSize : f,
+            disabled: v && !Object(V.isUndefined)(v.componentDisabled) ? v.componentDisabled : p,
+            size: v && !Object(V.isUndefined)(v.componentSize) ? v.componentSize : f,
             persistence: m,
             persisted_props: g,
             persistence_type: b,
             onChange: e,
             "data-dash-is-loading": t && t.is_loading || void 0
         })
     }
@@ -114101,30 +114113,30 @@
             v = t.cancelButtonProps,
             y = t.confirmCounts,
             x = t.cancelCounts,
             _ = t.trigger,
             O = t.popupContainer,
             w = t.setProps,
             t = t.loading_state,
-            k = Object(Wt.useContext)(U.a),
+            k = Object(Wt.useContext)(G.a),
             i = k && k.locale || i,
             n = j(n);
-        return F.a.createElement(H.a, {
-            locale: V.b.get(i)
-        }, F.a.createElement(wl.a, {
+        return H.a.createElement(W.a, {
+            locale: K.b.get(i)
+        }, H.a.createElement(wl.a, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             title: l,
-            disabled: k && !Object(W.isUndefined)(k.componentDisabled) ? k.componentDisabled : c,
+            disabled: k && !Object(V.isUndefined)(k.componentDisabled) ? k.componentDisabled : c,
             placement: s,
             mouseEnterDelay: u,
             mouseLeaveDelay: d,
-            overlayClassName: Object(W.isString)(p) ? p : p ? Object(K.a)(p) : void 0,
+            overlayClassName: Object(V.isString)(p) ? p : p ? Object(U.a)(p) : void 0,
             overlayStyle: f,
             overlayInnerStyle: h,
             trigger: _,
             okText: m,
             okButtonProps: g,
             cancelText: b,
             cancelButtonProps: v,
@@ -114181,17 +114193,17 @@
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.duration,
             i = t.visibilityHeight,
             l = t.containerId,
             t = (t.setProps, t.loading_state);
-        return F.a.createElement(El, {
+        return H.a.createElement(El, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             target: l ? function() {
                 return document.getElementById(l)
             } : function() {
                 return window
             },
@@ -114531,15 +114543,15 @@
                     var n = {};
                     for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                     if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                         for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                     return n
                 }(t, ["prefixCls", "size", "disabled", "className", "multiple", "bordered", "transitionName", "choiceTransitionName", "popupClassName", "dropdownClassName", "expandIcon", "placement", "showSearch", "allowClear", "notFoundContent", "direction", "getPopupContainer", "status", "showArrow"]),
                 O = Object(ct.a)(O, ["suffixIcon"]),
-                w = Object(Wt.useContext)(G.b),
+                w = Object(Wt.useContext)(q.b),
                 k = w.getPopupContainer,
                 j = w.getPrefixCls,
                 M = w.renderEmpty,
                 w = w.direction,
                 w = v || w,
                 E = "rtl" === w,
                 C = Object(Wt.useContext)(ve.b),
@@ -114813,15 +114825,15 @@
                             l(t)
                         }), l({
                             target: t
                         }),
                         function() {
                             o.current && o.current.remove(), l.cancel()
                         }
-                }, [r.target]), Wt.useContext(G.b)),
+                }, [r.target]), Wt.useContext(q.b)),
                 c = t.getPrefixCls,
                 t = t.direction,
                 s = r.prefixCls,
                 u = r.className,
                 u = void 0 === u ? "" : u,
                 s = c("back-top", s),
                 c = c(),
@@ -114877,15 +114889,15 @@
             l = t.style,
             c = t.children,
             s = void 0 !== (s = t.avatar) && s,
             u = void 0 === (u = t.title) || u,
             d = void 0 === (d = t.paragraph) || d,
             p = t.active,
             f = t.round,
-            h = (m = Wt.useContext(G.b)).getPrefixCls,
+            h = (m = Wt.useContext(q.b)).getPrefixCls,
             m = m.direction,
             h = h("skeleton", r);
         return !o && "loading" in t ? void 0 !== c ? c : null : (r = !!u, o = !!d, (t = !!s) && (c = Object(Et.a)(Object(Et.a)({
             prefixCls: "".concat(h, "-avatar")
         }, r && !o ? {
             size: "large",
             shape: "square"
@@ -114913,15 +114925,15 @@
         var e, n = t.prefixCls,
             a = t.className,
             r = t.active,
             o = t.block,
             o = void 0 !== o && o,
             i = t.size,
             i = void 0 === i ? "default" : i,
-            n = (0, Wt.useContext(G.b).getPrefixCls)("skeleton", n),
+            n = (0, Wt.useContext(q.b).getPrefixCls)("skeleton", n),
             t = Object(ct.a)(t, ["prefixCls"]),
             r = Kt()(n, "".concat(n, "-element"), (e = {}, Object(Vt.a)(e, "".concat(n, "-active"), r), Object(Vt.a)(e, "".concat(n, "-block"), o), e), a);
         return Wt.createElement("div", {
             className: r
         }, Wt.createElement(hl, Object(Et.a)({
             prefixCls: "".concat(n, "-button"),
             size: i
@@ -114930,15 +114942,15 @@
         var e = t.prefixCls,
             n = t.className,
             a = t.active,
             r = t.shape,
             r = void 0 === r ? "circle" : r,
             o = t.size,
             o = void 0 === o ? "default" : o,
-            e = (0, Wt.useContext(G.b).getPrefixCls)("skeleton", e),
+            e = (0, Wt.useContext(q.b).getPrefixCls)("skeleton", e),
             t = Object(ct.a)(t, ["prefixCls", "className"]),
             a = Kt()(e, "".concat(e, "-element"), Object(Vt.a)({}, "".concat(e, "-active"), a), n);
         return Wt.createElement("div", {
             className: a
         }, Wt.createElement(hl, Object(Et.a)({
             prefixCls: "".concat(e, "-avatar"),
             shape: r,
@@ -114947,29 +114959,29 @@
     }, Pl.Input = function(t) {
         var e, n = t.prefixCls,
             a = t.className,
             r = t.active,
             o = t.block,
             i = t.size,
             i = void 0 === i ? "default" : i,
-            n = (0, Wt.useContext(G.b).getPrefixCls)("skeleton", n),
+            n = (0, Wt.useContext(q.b).getPrefixCls)("skeleton", n),
             t = Object(ct.a)(t, ["prefixCls"]),
             r = Kt()(n, "".concat(n, "-element"), (e = {}, Object(Vt.a)(e, "".concat(n, "-active"), r), Object(Vt.a)(e, "".concat(n, "-block"), o), e), a);
         return Wt.createElement("div", {
             className: r
         }, Wt.createElement(hl, Object(Et.a)({
             prefixCls: "".concat(n, "-input"),
             size: i
         }, t)))
     }, Pl.Image = function(t) {
         var e = t.prefixCls,
             n = t.className,
             a = t.style,
             t = t.active,
-            e = (0, Wt.useContext(G.b).getPrefixCls)("skeleton", e),
+            e = (0, Wt.useContext(q.b).getPrefixCls)("skeleton", e),
             t = Kt()(e, "".concat(e, "-element"), Object(Vt.a)({}, "".concat(e, "-active"), t), n);
         return Wt.createElement("div", {
             className: t
         }, Wt.createElement("div", {
             className: Kt()("".concat(e, "-image"), n),
             style: a
         }, Wt.createElement("svg", {
@@ -114982,15 +114994,15 @@
         }))))
     }, Pl.Node = function(t) {
         var e = t.prefixCls,
             n = t.className,
             a = t.style,
             r = t.active,
             t = t.children,
-            e = (0, Wt.useContext(G.b).getPrefixCls)("skeleton", e),
+            e = (0, Wt.useContext(q.b).getPrefixCls)("skeleton", e),
             r = Kt()(e, "".concat(e, "-element"), Object(Vt.a)({}, "".concat(e, "-active"), r), n),
             t = null != t ? t : Wt.createElement(Sl.a, null);
         return Wt.createElement("div", {
             className: r
         }, Wt.createElement("div", {
             className: Kt()("".concat(e, "-image"), n),
             style: a
@@ -115055,17 +115067,17 @@
             }())[0],
             v = t[1],
             y = Object(Wt.useRef)();
         return Object(Wt.useEffect)(function() {
             g && (y.current && clearTimeout(y.current), g.is_loading && !b ? "default" === p ? (m && console.log(g.component_name + "." + g.prop_name), v(!0)) : "exclude" === p ? -1 === f.indexOf(g.component_name + "." + g.prop_name) && (m && console.log(g.component_name + "." + g.prop_name), v(!0)) : "include" === p && -1 !== h.indexOf(g.component_name + "." + g.prop_name) && (m && console.log(g.component_name + "." + g.prop_name), v(!0)) : !g.is_loading && b && (y.current = setTimeout(function() {
                 return v(!1)
             })))
-        }, [g]), F.a.createElement(Dl, {
+        }, [g]), H.a.createElement(Dl, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             loading: b,
             active: l,
             avatar: c,
             paragraph: s,
             round: u,
@@ -115081,17 +115093,17 @@
             r = t.key,
             o = t.children,
             i = t.offsetBottom,
             l = t.offsetTop,
             c = t.target,
             t = (t.setProps, t.loading_state),
             o = j(o);
-        return F.a.createElement(jt, {
+        return H.a.createElement(jt, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             offsetBottom: i,
             offsetTop: l,
             target: function() {
                 return c ? document.getElementById(c) : window
             },
@@ -115109,15 +115121,15 @@
             t = function(t, e) {
                 var n = {};
                 for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                 if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                     for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                 return n
             }(t, ["prefixCls", "separator", "children", "menu", "overlay", "dropdownProps"]),
-            e = (0, Wt.useContext(G.b).getPrefixCls)("breadcrumb", e),
+            e = (0, Wt.useContext(q.b).getPrefixCls)("breadcrumb", e),
             l = t = "href" in t ? Wt.createElement("a", Object(Et.a)({
                 className: "".concat(e, "-link")
             }, t), a) : Wt.createElement("span", Object(Et.a)({
                 className: "".concat(e, "-link")
             }, t), a);
         return t = r || o ? Wt.createElement(Bl.a, Object(Et.a)({
             menu: r,
@@ -115128,15 +115140,15 @@
         }, l, Wt.createElement(Oe.a, null))) : l, null != a ? Wt.createElement("li", null, t, n && Wt.createElement("span", {
             className: "".concat(e, "-separator")
         }, n)) : null
     }
 
     function Il(t) {
         var t = t.children,
-            e = (0, Wt.useContext(G.b).getPrefixCls)("breadcrumb");
+            e = (0, Wt.useContext(q.b).getPrefixCls)("breadcrumb");
         return Wt.createElement("span", {
             className: "".concat(e, "-separator")
         }, t || "/")
     }
     zl._dashprivate_isLoadingComponent = !0, zl.propTypes = {
         id: n.a.string,
         children: n.a.node,
@@ -115225,15 +115237,15 @@
             d = function(t, e) {
                 var n = {};
                 for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                 if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                     for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                 return n
             }(t, ["prefixCls", "separator", "style", "className", "routes", "children", "itemRender", "params"]),
-            p = (t = Wt.useContext(G.b)).getPrefixCls,
+            p = (t = Wt.useContext(q.b)).getPrefixCls,
             t = t.direction,
             p = p("breadcrumb", n),
             n = (l && 0 < l.length ? (r = [], e = l.map(function(t) {
                 var e, n = Xl(t.path, u),
                     a = (n && r.push(n), t.children && t.children.length && (e = Wt.createElement(Nn.a, {
                         items: t.children.map(function(t) {
                             return {
@@ -115266,43 +115278,43 @@
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.separator,
             i = t.items,
             t = (t.setProps, t.loading_state);
-        return F.a.createElement($l, {
+        return H.a.createElement($l, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             separator: o,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, i.map(function(t) {
-            return F.a.createElement($l.Item, {
-                overlay: t.menuItems ? F.a.createElement(Nn.a, null, t.menuItems.map(function(t) {
-                    return F.a.createElement(Nn.a.Item, {
-                        icon: F.a.createElement(R.a, {
+            return H.a.createElement($l.Item, {
+                overlay: t.menuItems ? H.a.createElement(Nn.a, null, t.menuItems.map(function(t) {
+                    return H.a.createElement(Nn.a.Item, {
+                        icon: H.a.createElement(I.a, {
                             icon: t.icon,
                             style: {
                                 marginRight: 3
                             }
                         }),
                         disabled: t.disabled
-                    }, F.a.createElement("a", {
+                    }, H.a.createElement("a", {
                         href: t.href,
                         target: t.target
                     }, t.title))
                 })) : null
-            }, F.a.createElement(R.a, {
+            }, H.a.createElement(I.a, {
                 icon: t.icon,
                 style: {
                     marginRight: 3
                 }
-            }), F.a.createElement("a", {
+            }), H.a.createElement("a", {
                 href: t.href,
                 target: t.target
             }, t.title))
         }))
     }
 
     function Kl(t) {
@@ -115314,68 +115326,70 @@
             i = t.buttonMode,
             l = t.arrow,
             c = t.disabled,
             s = t.overlayClassName,
             u = t.overlayStyle,
             d = t.placement,
             p = t.trigger,
-            f = t.visible,
-            h = t.menuItems,
-            m = t.nClicks,
-            g = t.popupContainer,
-            b = t.buttonProps,
-            v = t.setProps,
+            f = t.autoAdjustOverflow,
+            h = t.visible,
+            m = t.menuItems,
+            g = t.nClicks,
+            b = t.popupContainer,
+            v = t.buttonProps,
+            y = t.setProps,
             t = t.loading_state,
-            y = Object(Wt.useContext)(U.a);
-        return F.a.createElement(ke.a, {
+            x = Object(Wt.useContext)(G.a);
+        return H.a.createElement(ke.a, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
-            overlay: F.a.createElement(Nn.a, {
+            overlay: H.a.createElement(Nn.a, {
                 onClick: function(t, e, n, a) {
-                    return v({
+                    return y({
                         clickedKey: t.key,
-                        nClicks: m + 1
+                        nClicks: g + 1
                     })
                 }
-            }, h.map(function(t) {
-                return t.isDivider ? F.a.createElement(Nn.a.Divider, null) : F.a.createElement(Nn.a.Item, {
-                    icon: F.a.createElement(R.a, {
+            }, m.map(function(t) {
+                return t.isDivider ? H.a.createElement(Nn.a.Divider, null) : H.a.createElement(Nn.a.Item, {
+                    icon: H.a.createElement(I.a, {
                         icon: t.icon
                     }),
                     disabled: t.disabled,
                     key: t.key || t.title
-                }, F.a.createElement("a", {
+                }, H.a.createElement("a", {
                     href: t.href,
                     target: t.target
                 }, t.title))
             })),
             arrow: l,
-            disabled: y && !Object(W.isUndefined)(y.componentDisabled) ? y.componentDisabled : c,
-            overlayClassName: Object(W.isString)(s) ? s : s ? Object(K.a)(s) : void 0,
+            disabled: x && !Object(V.isUndefined)(x.componentDisabled) ? x.componentDisabled : c,
+            overlayClassName: Object(V.isString)(s) ? s : s ? Object(U.a)(s) : void 0,
             overlayStyle: u,
             placement: d,
             trigger: [p],
-            visible: f,
+            autoAdjustOverflow: f,
+            visible: h,
             onVisibleChange: function(t) {
-                return v({
+                return y({
                     visible: t
                 })
             },
-            getPopupContainer: "parent" === g ? function(t) {
+            getPopupContainer: "parent" === b ? function(t) {
                 return t.parentNode
             } : void 0,
             "data-dash-is-loading": t && t.is_loading || void 0
-        }, i ? F.a.createElement(T.a, b, o, " ", F.a.createElement(Oe.a, null)) : F.a.createElement("a", {
+        }, i ? H.a.createElement(z.a, v, o, " ", H.a.createElement(Oe.a, null)) : H.a.createElement("a", {
             className: "ant-dropdown-link",
             onClick: function(t) {
                 return t.preventDefault()
             }
-        }, o, " ", F.a.createElement(Oe.a, null)))
+        }, o, " ", H.a.createElement(Oe.a, null)))
     }
 
     function Ul(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
@@ -115400,43 +115414,43 @@
             w = t.status,
             k = t.debounceWait,
             j = t.setProps,
             M = t.persistence,
             E = t.persisted_props,
             C = t.persistence_type,
             t = t.loading_state,
-            S = Object(Wt.useContext)(U.a),
+            S = Object(Wt.useContext)(G.a),
             L = (Object(Wt.useEffect)(function() {
                 p && !d && j({
                     value: p,
                     debounceValue: p
                 })
             }, []), Object(Z.a)(function(t) {
                 j({
                     debounceValue: t
                 })
             }, {
                 debounceWait: Math.max(k, 200),
                 manual: !0
             }).run);
-        return F.a.createElement(Ql.a, {
+        return H.a.createElement(Ql.a, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
-            size: S && !Object(W.isUndefined)(S.componentSize) ? S.componentSize : o,
+            size: S && !Object(V.isUndefined)(S.componentSize) ? S.componentSize : o,
             addonBefore: i,
             addonAfter: l,
             prefix: c,
             placeholder: h,
             bordered: s,
             controls: u,
             value: d,
             defaultValue: p,
-            disabled: S && !Object(W.isUndefined)(S.componentDisabled) ? S.componentDisabled : f,
+            disabled: S && !Object(V.isUndefined)(S.componentDisabled) ? S.componentDisabled : f,
             keyboard: m,
             min: g,
             max: b,
             step: v,
             precision: y,
             readOnly: x,
             stringMode: _,
@@ -115523,14 +115537,15 @@
             })),
             arrow: n.a.bool,
             disabled: n.a.bool,
             overlayClassName: n.a.oneOfType([n.a.string, n.a.object]),
             overlayStyle: n.a.object,
             placement: n.a.oneOf(["bottomLeft", "bottomCenter", "bottomRight", "topLeft", "topCenter", "topRight"]),
             trigger: n.a.oneOf(["click", "hover"]),
+            autoAdjustOverflow: n.a.bool,
             visible: n.a.bool,
             popupContainer: n.a.oneOf(["parent", "body"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
@@ -115538,15 +115553,16 @@
         }, Kl.defaultProps = {
             arrow: !1,
             disabled: !1,
             visible: !1,
             buttonMode: !1,
             trigger: "hover",
             nClicks: 0,
-            popupContainer: "body"
+            popupContainer: "body",
+            autoAdjustOverflow: !0
         }, Kl),
         Ql = e(708),
         tc = (Ul.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
@@ -115607,15 +115623,15 @@
                 }]
             },
             name: "star",
             theme: "filled"
         },
         nc = (Gl.displayName = "StarFilled", Wt.forwardRef(Gl)),
         ac = e(107),
-        rc = (l = F.a.Component, Object(r.a)(oc, l), ql = Object(o.a)(oc), Object(a.a)(oc, [{
+        rc = (l = H.a.Component, Object(r.a)(oc, l), ql = Object(o.a)(oc), Object(a.a)(oc, [{
             key: "getClassName",
             value: function() {
                 var t = this.props,
                     e = t.prefixCls,
                     n = t.index,
                     a = t.value,
                     r = t.allowHalf,
@@ -115635,28 +115651,28 @@
                     o = a.prefixCls,
                     i = a.character,
                     l = a.characterRender,
                     c = a.index,
                     s = a.count,
                     a = a.value,
                     i = "function" == typeof i ? i(this.props) : i,
-                    e = F.a.createElement("li", {
+                    e = H.a.createElement("li", {
                         className: this.getClassName()
-                    }, F.a.createElement("div", {
+                    }, H.a.createElement("div", {
                         onClick: r ? null : e,
                         onKeyDown: r ? null : n,
                         onMouseMove: r ? null : t,
                         role: "radio",
                         "aria-checked": c < a ? "true" : "false",
                         "aria-posinset": c + 1,
                         "aria-setsize": s,
                         tabIndex: r ? -1 : 0
-                    }, F.a.createElement("div", {
+                    }, H.a.createElement("div", {
                         className: "".concat(o, "-first")
-                    }, i), F.a.createElement("div", {
+                    }, i), H.a.createElement("div", {
                         className: "".concat(o, "-second")
                     }, i)));
                 return e = l ? l(e, this.props) : e
             }
         }]), oc);
 
     function oc() {
@@ -115674,15 +115690,15 @@
                 n = e.onClick,
                 e = e.index;
             13 === t.keyCode && n(t, e)
         }, a
     }
 
     function ic() {}
-    c = F.a.Component, Object(r.a)(cc, c), lc = Object(o.a)(cc), Object(a.a)(cc, [{
+    c = H.a.Component, Object(r.a)(cc, c), lc = Object(o.a)(cc), Object(a.a)(cc, [{
         key: "componentDidMount",
         value: function() {
             var t = this.props,
                 e = t.autoFocus,
                 t = t.disabled;
             e && !t && this.focus()
         }
@@ -115720,15 +115736,15 @@
             "value" in this.props || this.setState({
                 value: t
             }), e(t)
         }
     }, {
         key: "render",
         value: function() {
-            for (var t = this.props, e = t.count, n = t.allowHalf, a = t.style, r = t.prefixCls, o = t.disabled, i = t.className, l = t.character, c = t.characterRender, s = t.tabIndex, t = t.direction, u = this.state, d = u.value, p = u.hoverValue, f = u.focused, h = [], u = o ? "".concat(r, "-disabled") : "", m = 0; m < e; m += 1) h.push(F.a.createElement(rc, {
+            for (var t = this.props, e = t.count, n = t.allowHalf, a = t.style, r = t.prefixCls, o = t.disabled, i = t.className, l = t.character, c = t.characterRender, s = t.tabIndex, t = t.direction, u = this.state, d = u.value, p = u.hoverValue, f = u.focused, h = [], u = o ? "".concat(r, "-disabled") : "", m = 0; m < e; m += 1) h.push(H.a.createElement(rc, {
                 ref: this.saveRef(m),
                 index: m,
                 count: e,
                 disabled: o,
                 prefixCls: "".concat(r, "-star"),
                 allowHalf: n,
                 value: void 0 === p ? d : p,
@@ -115736,15 +115752,15 @@
                 onHover: this.onHover,
                 key: m,
                 character: l,
                 characterRender: c,
                 focused: f
             }));
             u = Kt()(r, u, i, Object(Vt.a)({}, "".concat(r, "-rtl"), "rtl" === t));
-            return F.a.createElement("ul", {
+            return H.a.createElement("ul", {
                 className: u,
                 style: a,
                 onMouseLeave: o ? null : this.onMouseLeave,
                 tabIndex: o ? -1 : s,
                 onFocus: o ? null : this.onFocus,
                 onBlur: o ? null : this.onBlur,
                 onKeyDown: o ? null : this.onKeyDown,
@@ -115798,15 +115814,15 @@
             var e = t.keyCode,
                 n = l.props,
                 a = n.count,
                 r = n.allowHalf,
                 o = n.onKeyDown,
                 n = "rtl" === n.direction,
                 i = l.state.value;
-            e === q.a.RIGHT && i < a && !n ? (l.changeValue(i += r ? .5 : 1), t.preventDefault()) : e === q.a.LEFT && 0 < i && !n || e === q.a.RIGHT && 0 < i && n ? (l.changeValue(i -= r ? .5 : 1), t.preventDefault()) : e === q.a.LEFT && i < a && n && (l.changeValue(i += r ? .5 : 1), t.preventDefault()), o && o(t)
+            e === X.a.RIGHT && i < a && !n ? (l.changeValue(i += r ? .5 : 1), t.preventDefault()) : e === X.a.LEFT && 0 < i && !n || e === X.a.RIGHT && 0 < i && n ? (l.changeValue(i -= r ? .5 : 1), t.preventDefault()) : e === X.a.LEFT && i < a && n && (l.changeValue(i += r ? .5 : 1), t.preventDefault()), o && o(t)
         }, l.saveRef = function(e) {
             return function(t) {
                 l.stars[e] = t
             }
         }, l.saveRate = function(t) {
             l.rate = t
         };
@@ -115844,28 +115860,28 @@
             u = t.defaultValue,
             d = t.value,
             p = t.setProps,
             f = t.loading_state,
             h = t.persistence,
             m = t.persisted_props,
             t = t.persistence_type,
-            g = Object(Wt.useContext)(U.a);
+            g = Object(Wt.useContext)(G.a);
         return Object(Wt.useEffect)(function() {
             u && !d && p({
                 value: u
             })
-        }, []), F.a.createElement(pc, {
+        }, []), H.a.createElement(pc, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             allowClear: o,
             allowHalf: i,
             count: l,
-            disabled: g && !Object(W.isUndefined)(g.componentDisabled) ? g.componentDisabled : c,
+            disabled: g && !Object(V.isUndefined)(g.componentDisabled) ? g.componentDisabled : c,
             tooltips: s,
             value: d,
             onChange: function(t) {
                 return p({
                     value: t
                 })
             },
@@ -115902,15 +115918,15 @@
                 t = function(t, e) {
                     var n = {};
                     for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                     if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                         for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                     return n
                 }(t, ["prefixCls", "tooltips", "character"]),
-                o = Wt.useContext(G.b),
+                o = Wt.useContext(q.b),
                 i = o.getPrefixCls,
                 o = o.direction,
                 i = i("rate", n);
             return Wt.createElement(dc, Object(Et.a)({
                 ref: e,
                 character: r,
                 characterRender: function(t, e) {
@@ -115953,15 +115969,15 @@
             disabled: !1,
             persisted_props: ["value"],
             persistence_type: "local"
         }, sc),
         hc = e(143),
         p = e(519),
         mc = e.n(p),
-        gc = Object(G.c)({
+        gc = Object(q.c)({
             prefixCls: "statistic"
         })(function(t) {
             var e = t.prefixCls,
                 n = t.className,
                 a = t.style,
                 r = t.valueStyle,
                 o = t.value,
@@ -116028,32 +116044,32 @@
             l = t.precision,
             c = t.prefix,
             s = t.suffix,
             u = t.title,
             d = t.titleTooltip,
             p = t.valueStyle,
             t = (t.setProps, t.loading_state);
-        return F.a.createElement(Pc, {
+        return H.a.createElement(Pc, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
-            value: Object(W.isString)(o) || Object(W.isNumber)(o) ? o : void 0,
-            formatter: Object(W.isString)(o) || Object(W.isNumber)(o) ? void 0 : function() {
+            value: Object(V.isString)(o) || Object(V.isNumber)(o) ? o : void 0,
+            formatter: Object(V.isString)(o) || Object(V.isNumber)(o) ? void 0 : function() {
                 return o
             },
             groupSeparator: i ? "," : "",
             precision: l,
             prefix: c,
             suffix: s,
-            title: d ? F.a.createElement(za.b, {
+            title: d ? H.a.createElement(za.b, {
                 size: 5
-            }, u, F.a.createElement(po, {
+            }, u, H.a.createElement(po, {
                 title: d
-            }, F.a.createElement(Dc.a, null))) : u,
+            }, H.a.createElement(Dc.a, null))) : u,
             valueStyle: p,
             "data-dash-is-loading": t && t.is_loading || void 0
         })
     }
 
     function xc(t) {
         var e = t.id,
@@ -116065,43 +116081,43 @@
             l = t.format,
             c = t.prefix,
             s = t.suffix,
             u = t.title,
             d = t.titleTooltip,
             p = t.valueStyle,
             t = (t.setProps, t.loading_state);
-        return F.a.createElement(zc, {
+        return H.a.createElement(zc, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             value: C()(o, i),
             format: l,
             prefix: c,
             suffix: s,
-            title: d ? F.a.createElement(Space, {
+            title: d ? H.a.createElement(Space, {
                 size: 5
-            }, u, F.a.createElement(AntdTooltip, {
+            }, u, H.a.createElement(AntdTooltip, {
                 title: d
-            }, F.a.createElement(QuestionCircleOutlined, null))) : u,
+            }, H.a.createElement(QuestionCircleOutlined, null))) : u,
             valueStyle: p,
             "data-dash-is-loading": t && t.is_loading || void 0
         })
     }
 
     function _c(t) {
         var e = t.prefixCls,
             n = t.className,
             a = void 0 === (a = t.color) ? "blue" : a,
             r = t.dot,
             o = void 0 !== (o = t.pending) && o,
             i = (t.position, t.label),
             l = t.children,
             t = Rc(t, ["prefixCls", "className", "color", "dot", "pending", "position", "label", "children"]),
-            e = (0, Wt.useContext(G.b).getPrefixCls)("timeline", e),
+            e = (0, Wt.useContext(q.b).getPrefixCls)("timeline", e),
             o = Kt()((c = {}, Object(Vt.a)(c, "".concat(e, "-item"), !0), Object(Vt.a)(c, "".concat(e, "-item-pending"), o), c), n),
             n = Kt()((c = {}, Object(Vt.a)(c, "".concat(e, "-item-head"), !0), Object(Vt.a)(c, "".concat(e, "-item-head-custom"), !!r), Object(Vt.a)(c, "".concat(e, "-item-head-").concat(a), !0), c)),
             c = /blue|red|green|gray/.test(a || "") ? void 0 : a;
         return Wt.createElement("li", Object(Et.a)({}, t, {
             className: o
         }), i && Wt.createElement("div", {
             className: "".concat(e, "-item-label")
@@ -116115,15 +116131,15 @@
             }
         }, r), Wt.createElement("div", {
             className: "".concat(e, "-item-content")
         }, l))
     }
 
     function Oc(t) {
-        var e = (n = Wt.useContext(G.b)).getPrefixCls,
+        var e = (n = Wt.useContext(q.b)).getPrefixCls,
             n = n.direction,
             a = t.prefixCls,
             r = void 0 === (o = t.pending) ? null : o,
             o = t.pendingDot,
             i = t.children,
             l = t.className,
             c = void 0 !== (u = t.reverse) && u,
@@ -116169,26 +116185,26 @@
             r = t.key,
             o = t.items,
             i = t.mode,
             l = t.pending,
             c = t.pendingDot,
             s = t.reverse,
             t = (t.setProps, t.loading_state);
-        return F.a.createElement(Ic, {
+        return H.a.createElement(Ic, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             mode: i,
             pending: l,
             pendingDot: c,
             reverse: s,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, o.map(function(t) {
-            return F.a.createElement(Ic.Item, {
+            return H.a.createElement(Ic.Item, {
                 color: t.color,
                 dot: t.icon,
                 label: t.label
             }, t.content)
         }))
     }
 
@@ -116208,17 +116224,17 @@
             f = t.strokeWidth,
             h = t.trailColor,
             m = t.width,
             g = t.gapDegree,
             b = t.gapPosition,
             v = t.steps,
             y = t.loading_state;
-        return t.setProps, F.a.createElement(kn, {
+        return t.setProps, H.a.createElement(kn, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             type: o,
             size: i,
             percent: l,
             format: c ? function(t) {
                 return c && c.content ? c.content : (c && c.prefix ? c.prefix : "") + "".concat(t) + (c && c.suffix ? c.suffix : "%")
@@ -116251,42 +116267,42 @@
             c = t.srcSet,
             s = t.icon,
             u = t.alt,
             d = t.gap,
             p = t.size,
             f = t.shape,
             h = t.loading_state;
-        return t.setProps, "image" === o ? F.a.createElement(Bc.a, {
+        return t.setProps, "image" === o ? H.a.createElement(Bc.a, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             src: l,
             srcSet: c,
             alt: u,
             size: p,
             shape: f,
             "data-dash-is-loading": h && h.is_loading || void 0
-        }) : "text" === o ? F.a.createElement(Bc.a, {
+        }) : "text" === o ? H.a.createElement(Bc.a, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             gap: d,
             size: p,
             shape: f,
             "data-dash-is-loading": h && h.is_loading || void 0
-        }, i) : F.a.createElement(Bc.a, {
+        }, i) : H.a.createElement(Bc.a, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
-            icon: s ? F.a.createElement(R.a, {
+            icon: s ? H.a.createElement(I.a, {
                 icon: s
-            }) : F.a.createElement(R.a, {
+            }) : H.a.createElement(I.a, {
                 icon: "antd-user"
             }),
             size: p,
             shape: f,
             "data-dash-is-loading": h && h.is_loading || void 0
         })
     }
@@ -116299,17 +116315,17 @@
             o = t.key,
             i = t.maxCount,
             l = t.maxPopoverPlacement,
             c = t.maxPopoverTrigger,
             s = t.maxStyle,
             u = t.size,
             d = t.loading_state;
-        return t.setProps, F.a.createElement(Bc.a.Group, {
+        return t.setProps, H.a.createElement(Bc.a.Group, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             maxCount: i,
             maxPopoverPlacement: l,
             maxPopoverTrigger: c,
             maxStyle: s,
             size: u,
@@ -116332,17 +116348,17 @@
             p = t.status,
             f = t.text,
             h = t.title,
             m = t.size,
             g = t.nClicks,
             b = t.loading_state,
             v = t.setProps;
-        return F.a.createElement(Wc.a, {
+        return H.a.createElement(Wc.a, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             color: i,
             count: l,
             dot: c,
             offset: s && 2 === s.length ? s : void 0,
             overflowCount: u,
@@ -116366,17 +116382,17 @@
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.color,
             l = t.placement,
             c = t.text,
             s = t.loading_state;
-        return t.setProps, F.a.createElement(Wc.a.Ribbon, {
+        return t.setProps, H.a.createElement(Wc.a.Ribbon, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             color: i,
             placement: l,
             text: c,
             "data-dash-is-loading": s && s.is_loading || void 0
         }, n)
@@ -116405,54 +116421,54 @@
             x = t.status,
             _ = t.popupContainer,
             O = t.readOnly,
             w = t.persistence,
             k = t.persisted_props,
             j = t.persistence_type,
             t = t.loading_state,
-            M = Object(Wt.useContext)(U.a),
+            M = Object(Wt.useContext)(G.a),
             o = M && M.locale || o;
         return Object(Wt.useEffect)(function() {
             f && !p && i({
                 value: f
             })
-        }, []), F.a.createElement("div", null, F.a.createElement(H.a, {
-            locale: V.b.get(o)
-        }, F.a.createElement(qc, {
+        }, []), H.a.createElement("div", null, H.a.createElement(W.a, {
+            locale: K.b.get(o)
+        }, H.a.createElement(qc, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             onChange: function(t, e) {
-                Object(W.isString)(e) && i({
+                Object(V.isString)(e) && i({
                     value: e
                 })
             },
             placeholder: g,
             placement: b,
             bordered: v,
-            size: M && !Object(W.isUndefined)(M.componentSize) ? M.componentSize : y,
-            disabled: M && !Object(W.isUndefined)(M.componentDisabled) ? M.componentDisabled : l,
+            size: M && !Object(V.isUndefined)(M.componentSize) ? M.componentSize : y,
+            disabled: M && !Object(V.isUndefined)(M.componentDisabled) ? M.componentDisabled : l,
             hourStep: c,
             minuteStep: s,
             secondStep: u,
             format: d,
             value: p ? C()(p, d) : void 0,
             defaultValue: f ? C()(f, d) : void 0,
             use12Hours: h,
-            allowClear: Object(W.isUndefined)(O) ? m : !O,
+            allowClear: Object(V.isUndefined)(O) ? m : !O,
             status: x,
             persistence: w,
             persisted_props: k,
             persistence_type: j,
             "data-dash-is-loading": t && t.is_loading || void 0,
             getPopupContainer: "parent" === _ ? function(t) {
                 return t.parentNode
             } : void 0,
-            open: !(!Object(W.isUndefined)(O) && O) && void 0,
+            open: !(!Object(V.isUndefined)(O) && O) && void 0,
             inputReadOnly: O
         })))
     }
 
     function Lc(t) {
         var e = t.id,
             n = t.className,
@@ -116476,57 +116492,57 @@
             x = t.status,
             _ = t.popupContainer,
             O = t.readOnly,
             w = t.persistence,
             k = t.persisted_props,
             j = t.persistence_type,
             t = t.loading_state,
-            M = Object(Wt.useContext)(U.a),
+            M = Object(Wt.useContext)(G.a),
             o = M && M.locale || o;
         return Object(Wt.useEffect)(function() {
             c && !l && i({
                 value: c
             })
-        }, []), F.a.createElement("div", null, F.a.createElement(H.a, {
-            locale: V.b.get(o)
-        }, F.a.createElement($c, {
+        }, []), H.a.createElement("div", null, H.a.createElement(W.a, {
+            locale: K.b.get(o)
+        }, H.a.createElement($c, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             onChange: function(t, e) {
                 Array.isArray(e) ? i({
                     value: [e[0], e[1]]
                 }) : i({
                     value: null
                 })
             },
-            disabled: M && !Object(W.isUndefined)(M.componentDisabled) ? [M.componentDisabled, M.componentDisabled] : d && 2 === d.length ? d : void 0,
+            disabled: M && !Object(V.isUndefined)(M.componentDisabled) ? [M.componentDisabled, M.componentDisabled] : d && 2 === d.length ? d : void 0,
             allowEmpty: d && 2 === d.length ? d : void 0,
             placeholder: s && 2 === s.length ? s : void 0,
             placement: u,
             bordered: v,
-            size: M && !Object(W.isUndefined)(M.componentSize) ? M.componentSize : y,
+            size: M && !Object(V.isUndefined)(M.componentSize) ? M.componentSize : y,
             hourStep: p,
             minuteStep: f,
             secondStep: h,
             format: m,
             use12Hours: g,
-            allowClear: Object(W.isUndefined)(O) ? b : !O,
+            allowClear: Object(V.isUndefined)(O) ? b : !O,
             defaultValue: c && 2 === c.length ? ["" !== c[0] ? C()(c[0], m) : void 0, "" !== c[1] ? C()(c[1], m) : void 0] : void 0,
             value: l && 2 === l.length ? ["" !== l[0] ? C()(l[0], m) : void 0, "" !== l[1] ? C()(l[1], m) : void 0] : void 0,
             status: x,
             persistence: w,
             persisted_props: k,
             persistence_type: j,
             "data-dash-is-loading": t && t.is_loading || void 0,
             getPopupContainer: "parent" === _ ? function(t) {
                 return t.parentNode
             } : void 0,
-            open: !(!Object(W.isUndefined)(O) && O) && void 0,
+            open: !(!Object(V.isUndefined)(O) && O) && void 0,
             inputReadOnly: O
         })))
     }
     var c = Wt.memo(function(t) {
             var e = t.value,
                 n = t.format,
                 i = void 0 === n ? "HH:mm:ss" : n,
@@ -117041,59 +117057,59 @@
         return t.key + "-" + e
     }
 
     function us(c) {
         var s, u = [],
             d = [],
             p = [],
-            f = F.a.Children.count(c.children),
+            f = H.a.Children.count(c.children),
             h = ys(c),
             m = xs(c);
-        return F.a.Children.forEach(c.children, function(t, e) {
+        return H.a.Children.forEach(c.children, function(t, e) {
             var n, a = {
                     message: "children",
                     index: e,
                     slidesToScroll: c.slidesToScroll,
                     currentSlide: c.currentSlide
                 },
-                r = !c.lazyLoad || c.lazyLoad && 0 <= c.lazyLoadedList.indexOf(e) ? t : F.a.createElement("div", null),
+                r = !c.lazyLoad || c.lazyLoad && 0 <= c.lazyLoadedList.indexOf(e) ? t : H.a.createElement("div", null),
                 o = (o = Object(Ct.a)(Object(Ct.a)({}, c), {}, {
                     index: e
                 }), i = {}, void 0 !== o.variableWidth && !1 !== o.variableWidth || (i.width = o.slideWidth), o.fade && (i.position = "relative", o.vertical ? i.top = -o.index * parseInt(o.slideHeight) : i.left = -o.index * parseInt(o.slideWidth), i.opacity = o.currentSlide === o.index ? 1 : 0, o.useCSS) && (i.transition = "opacity " + o.speed + "ms " + o.cssEase + ", visibility " + o.speed + "ms " + o.cssEase), i),
                 i = r.props.className || "",
                 l = cs(Object(Ct.a)(Object(Ct.a)({}, c), {}, {
                     index: e
                 }));
-            u.push(F.a.cloneElement(r, {
+            u.push(H.a.cloneElement(r, {
                 key: "original" + ss(r, e),
                 "data-index": e,
                 className: Kt()(l, i),
                 tabIndex: "-1",
                 "aria-hidden": !l["slick-active"],
                 style: Object(Ct.a)(Object(Ct.a)({
                     outline: "none"
                 }, r.props.style || {}), o),
                 onClick: function(t) {
                     r.props && r.props.onClick && r.props.onClick(t), c.focusOnSelect && c.focusOnSelect(a)
                 }
             })), c.infinite && !1 === c.fade && ((n = f - e) <= Ls(c) && f !== c.slidesToShow && ((s = -n) >= h && (r = t), l = cs(Object(Ct.a)(Object(Ct.a)({}, c), {}, {
                 index: s
-            })), d.push(F.a.cloneElement(r, {
+            })), d.push(H.a.cloneElement(r, {
                 key: "precloned" + ss(r, s),
                 "data-index": s,
                 tabIndex: "-1",
                 className: Kt()(l, i),
                 "aria-hidden": !l["slick-active"],
                 style: Object(Ct.a)(Object(Ct.a)({}, r.props.style || {}), o),
                 onClick: function(t) {
                     r.props && r.props.onClick && r.props.onClick(t), c.focusOnSelect && c.focusOnSelect(a)
                 }
             }))), f !== c.slidesToShow) && ((s = f + e) < m && (r = t), l = cs(Object(Ct.a)(Object(Ct.a)({}, c), {}, {
                 index: s
-            })), p.push(F.a.cloneElement(r, {
+            })), p.push(H.a.cloneElement(r, {
                 key: "postcloned" + ss(r, s),
                 "data-index": s,
                 tabIndex: "-1",
                 className: Kt()(l, i),
                 "aria-hidden": !l["slick-active"],
                 style: Object(Ct.a)(Object(Ct.a)({}, r.props.style || {}), o),
                 onClick: function(t) {
@@ -117113,17 +117129,17 @@
             l = t.dotPosition,
             c = t.easing,
             s = t.effect,
             u = t.autoplaySpeed,
             d = t.speed,
             p = t.pauseOnHover,
             f = t.loading_state;
-        return t.setProps, F.a.createElement(Ws, {
+        return t.setProps, H.a.createElement(Ws, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             autoplay: i,
             dotPosition: l,
             easing: c,
             effect: s,
             autoplaySpeed: u,
@@ -117236,32 +117252,32 @@
                 if (n) {
                     var o = (e - 1) / 2 + 1;
                     return parseInt(r) > 0 && (o += 1), a || e % 2 != 0 || (o += 1), o
                 }
                 return a ? e - 1 : 0
             }(t) ? "right" : "left"
         },
-        Ts = (c = F.a.PureComponent, Object(r.a)(Xs, c), bs = Object(o.a)(Xs), Object(a.a)(Xs, [{
+        Ts = (c = H.a.PureComponent, Object(r.a)(Xs, c), bs = Object(o.a)(Xs), Object(a.a)(Xs, [{
             key: "render",
             value: function() {
                 var t = us(this.props),
                     e = this.props,
                     e = {
                         onMouseEnter: e.onMouseEnter,
                         onMouseOver: e.onMouseOver,
                         onMouseLeave: e.onMouseLeave
                     };
-                return F.a.createElement("div", Object(Et.a)({
+                return H.a.createElement("div", Object(Et.a)({
                     ref: this.handleRef,
                     className: "slick-track",
                     style: this.props.trackStyle
                 }, e), t)
             }
         }]), Xs),
-        zs = (d = F.a.PureComponent, Object(r.a)(qs, d), gs = Object(o.a)(qs), Object(a.a)(qs, [{
+        zs = (d = H.a.PureComponent, Object(r.a)(qs, d), gs = Object(o.a)(qs), Object(a.a)(qs, [{
             key: "clickHandler",
             value: function(t, e) {
                 e.preventDefault(), this.props.clickHandler(t)
             }
         }, {
             key: "render",
             value: function() {
@@ -117283,26 +117299,26 @@
                     }),
                     f = this.clickHandler.bind(this, {
                         message: "dots",
                         index: d,
                         slidesToScroll: o,
                         currentSlide: c
                     }),
-                    u = u.concat(F.a.createElement("li", {
+                    u = u.concat(H.a.createElement("li", {
                         key: d,
                         className: p
-                    }, F.a.cloneElement(this.props.customPaging(d), {
+                    }, H.a.cloneElement(this.props.customPaging(d), {
                         onClick: f
                     })));
-                return F.a.cloneElement(this.props.appendDots(u), Object(Ct.a)({
+                return H.a.cloneElement(this.props.appendDots(u), Object(Ct.a)({
                     className: this.props.dotsClass
                 }, i))
             }
         }]), qs),
-        As = (p = F.a.PureComponent, Object(r.a)(Gs, p), ms = Object(o.a)(Gs), Object(a.a)(Gs, [{
+        As = (p = H.a.PureComponent, Object(r.a)(Gs, p), ms = Object(o.a)(Gs), Object(a.a)(Gs, [{
             key: "clickHandler",
             value: function(t, e) {
                 e && e.preventDefault(), this.props.clickHandler(t, e)
             }
         }, {
             key: "render",
             value: function() {
@@ -117322,21 +117338,21 @@
                         },
                         onClick: e
                     }),
                     e = {
                         currentSlide: this.props.currentSlide,
                         slideCount: this.props.slideCount
                     };
-                return this.props.prevArrow ? F.a.cloneElement(this.props.prevArrow, Object(Ct.a)(Object(Ct.a)({}, t), e)) : F.a.createElement("button", Object(Et.a)({
+                return this.props.prevArrow ? H.a.cloneElement(this.props.prevArrow, Object(Ct.a)(Object(Ct.a)({}, t), e)) : H.a.createElement("button", Object(Et.a)({
                     key: "0",
                     type: "button"
                 }, t), " ", "Previous")
             }
         }]), Gs),
-        Rs = (l = F.a.PureComponent, Object(r.a)(Us, l), hs = Object(o.a)(Us), Object(a.a)(Us, [{
+        Rs = (l = H.a.PureComponent, Object(r.a)(Us, l), hs = Object(o.a)(Us), Object(a.a)(Us, [{
             key: "clickHandler",
             value: function(t, e) {
                 e && e.preventDefault(), this.props.clickHandler(t, e)
             }
         }, {
             key: "render",
             value: function() {
@@ -117356,62 +117372,62 @@
                         },
                         onClick: e
                     }),
                     e = {
                         currentSlide: this.props.currentSlide,
                         slideCount: this.props.slideCount
                     };
-                return this.props.nextArrow ? F.a.cloneElement(this.props.nextArrow, Object(Ct.a)(Object(Ct.a)({}, t), e)) : F.a.createElement("button", Object(Et.a)({
+                return this.props.nextArrow ? H.a.cloneElement(this.props.nextArrow, Object(Ct.a)(Object(Ct.a)({}, t), e)) : H.a.createElement("button", Object(Et.a)({
                     key: "1",
                     type: "button"
                 }, t), " ", "Next")
             }
         }]), Us),
         Is = e(140),
         Ns = ["animating"],
-        Ys = (c = F.a.Component, Object(r.a)(Ks, c), fs = Object(o.a)(Ks), Object(a.a)(Ks, [{
+        Ys = (c = H.a.Component, Object(r.a)(Ks, c), fs = Object(o.a)(Ks), Object(a.a)(Ks, [{
             key: "didPropsChange",
             value: function(t) {
                 for (var e = !1, n = 0, a = Object.keys(this.props); n < a.length; n++) {
                     var r = a[n];
                     if (!t.hasOwnProperty(r)) {
                         e = !0;
                         break
                     }
                     if ("object" !== Object(qt.a)(t[r]) && "function" != typeof t[r] && t[r] !== this.props[r]) {
                         e = !0;
                         break
                     }
                 }
-                return e || F.a.Children.count(this.props.children) !== F.a.Children.count(t.children)
+                return e || H.a.Children.count(this.props.children) !== H.a.Children.count(t.children)
             }
         }]), Ks),
         d = e(288),
         Bs = e.n(d),
         Fs = {
             accessibility: !0,
             adaptiveHeight: !1,
             afterChange: null,
             appendDots: function(t) {
-                return F.a.createElement("ul", {
+                return H.a.createElement("ul", {
                     style: {
                         display: "block"
                     }
                 }, t)
             },
             arrows: !0,
             autoplay: !1,
             autoplaySpeed: 3e3,
             beforeChange: null,
             centerMode: !1,
             centerPadding: "50px",
             className: "",
             cssEase: "ease",
             customPaging: function(t) {
-                return F.a.createElement("button", null, t + 1)
+                return H.a.createElement("button", null, t + 1)
             },
             dots: !1,
             dotsClass: "slick-dots",
             draggable: !0,
             easing: "linear",
             edgeFriction: .35,
             fade: !1,
@@ -117443,15 +117459,15 @@
             touchThreshold: 5,
             useCSS: !0,
             useTransform: !0,
             variableWidth: !1,
             vertical: !1,
             waitForAnimate: !0
         },
-        Hs = (p = F.a.Component, Object(r.a)(Vs, p), ps = Object(o.a)(Vs), Object(a.a)(Vs, [{
+        Hs = (p = H.a.Component, Object(r.a)(Vs, p), ps = Object(o.a)(Vs), Object(a.a)(Vs, [{
             key: "media",
             value: function(t, e) {
                 function n(t) {
                     t.matches && e()
                 }
                 var a = window.matchMedia(t);
                 a.addListener(n), n(a), this._responsiveMediaHandlers.push({
@@ -117499,44 +117515,44 @@
         }, {
             key: "render",
             value: function() {
                 var t, e = this;
                 (t = this.state.breakpoint ? "unslick" === (a = this.props.responsive.filter(function(t) {
                     return t.breakpoint === e.state.breakpoint
                 }))[0].settings ? "unslick" : Object(Ct.a)(Object(Ct.a)(Object(Ct.a)({}, Fs), this.props), a[0].settings) : Object(Ct.a)(Object(Ct.a)({}, Fs), this.props)).centerMode && (t.slidesToScroll, t.slidesToScroll = 1), t.fade && (t.slidesToShow, t.slidesToScroll, t.slidesToShow = 1, t.slidesToScroll = 1);
-                var n = (n = F.a.Children.toArray(this.props.children)).filter(function(t) {
+                var n = (n = H.a.Children.toArray(this.props.children)).filter(function(t) {
                     return "string" == typeof t ? !!t.trim() : !!t
                 });
                 t.variableWidth && (1 < t.rows || 1 < t.slidesPerRow) && (console.warn("variableWidth is not supported in case of rows > 1 or slidesPerRow > 1"), t.variableWidth = !1);
                 for (var a, r = [], o = null, i = 0; i < n.length; i += t.rows * t.slidesPerRow) {
                     for (var l = [], c = i; c < i + t.rows * t.slidesPerRow; c += t.slidesPerRow) {
-                        for (var s = [], u = c; u < c + t.slidesPerRow && (t.variableWidth && n[u].props.style && (o = n[u].props.style.width), !(u >= n.length)); u += 1) s.push(F.a.cloneElement(n[u], {
+                        for (var s = [], u = c; u < c + t.slidesPerRow && (t.variableWidth && n[u].props.style && (o = n[u].props.style.width), !(u >= n.length)); u += 1) s.push(H.a.cloneElement(n[u], {
                             key: 100 * i + 10 * c + u,
                             tabIndex: -1,
                             style: {
                                 width: "".concat(100 / t.slidesPerRow, "%"),
                                 display: "inline-block"
                             }
                         }));
-                        l.push(F.a.createElement("div", {
+                        l.push(H.a.createElement("div", {
                             key: 10 * i + c
                         }, s))
                     }
-                    t.variableWidth ? r.push(F.a.createElement("div", {
+                    t.variableWidth ? r.push(H.a.createElement("div", {
                         key: i,
                         style: {
                             width: o
                         }
-                    }, l)) : r.push(F.a.createElement("div", {
+                    }, l)) : r.push(H.a.createElement("div", {
                         key: i
                     }, l))
                 }
-                return "unslick" === t ? (a = "regular slider " + (this.props.className || ""), F.a.createElement("div", {
+                return "unslick" === t ? (a = "regular slider " + (this.props.className || ""), H.a.createElement("div", {
                     className: a
-                }, n)) : (r.length <= t.slidesToShow && (t.unslick = !0), F.a.createElement(Ys, Object(Et.a)({
+                }, n)) : (r.length <= t.slidesToShow && (t.unslick = !0), H.a.createElement(Ys, Object(Et.a)({
                     style: this.props.style,
                     ref: this.innerSliderRefHandler
                 }, t), r))
             }
         }]), Vs),
         Ws = Wt.forwardRef(function(t, e) {
             function n(t) {
@@ -117555,15 +117571,15 @@
                 s = function(t, e) {
                     var n = {};
                     for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                     if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                         for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                     return n
                 }(t, ["dots", "arrows", "draggable", "dotPosition", "vertical"]),
-                t = Wt.useContext(G.b),
+                t = Wt.useContext(q.b),
                 u = t.getPrefixCls,
                 t = t.direction,
                 d = Wt.useRef(),
                 p = (Wt.useImperativeHandle(e, function() {
                     return {
                         goTo: n,
                         autoPlay: d.current.innerSlider.autoPlay,
@@ -117651,17 +117667,17 @@
             }), f.props.onLazyLoad) && f.props.onLazyLoad(e), f.adaptHeight();
             var e, n = Object(Ct.a)(Object(Ct.a)({
                     listRef: f.list,
                     trackRef: f.track
                 }, f.props), f.state),
                 a = f.didPropsChange(t);
             a && f.updateState(n, a, function() {
-                f.state.currentSlide >= F.a.Children.count(f.props.children) && f.changeSlide({
+                f.state.currentSlide >= H.a.Children.count(f.props.children) && f.changeSlide({
                     message: "index",
-                    index: F.a.Children.count(f.props.children) - f.props.slidesToShow,
+                    index: H.a.Children.count(f.props.children) - f.props.slidesToShow,
                     currentSlide: f.state.currentSlide
                 }), t.autoplay === f.props.autoplay && t.autoplaySpeed === f.props.autoplaySpeed || (!t.autoplay && f.props.autoplay ? f.autoPlay("playing") : f.props.autoplay ? f.autoPlay("update") : f.pause("paused"))
             })
         }), Object(Vt.a)(Object(s.a)(f), "onWindowResized", function(t) {
             f.debouncedResize && f.debouncedResize.cancel(), f.debouncedResize = Qc()(function() {
                 return f.resizeWindow(t)
             }, 50), f.debouncedResize()
@@ -117672,15 +117688,15 @@
                 trackRef: f.track
             }, f.props), f.state), f.updateState(t, e, function() {
                 f.props.autoplay ? f.autoPlay("update") : f.pause("paused")
             }), f.setState({
                 animating: !1
             }), clearTimeout(f.animationEndCallback), delete f.animationEndCallback)
         }), Object(Vt.a)(Object(s.a)(f), "updateState", function(t, e, n) {
-            a = t, r = F.a.Children.count(a.children), o = a.listRef, d = Math.ceil(ws(o)), p = a.trackRef && a.trackRef.node, p = Math.ceil(ws(p)), u = a.vertical ? d : (u = a.centerMode && 2 * parseInt(a.centerPadding), "string" == typeof a.centerPadding && "%" === a.centerPadding.slice(-1) && (u *= d / 100), Math.ceil((d - u) / a.slidesToShow)), o = o && ks(o.querySelector('[data-index="0"]')), i = o * a.slidesToShow, l = void 0 === a.currentSlide ? a.initialSlide : a.currentSlide, a.rtl && void 0 === a.currentSlide && (l = r - 1 - a.initialSlide), c = a.lazyLoadedList || [], s = vs(Object(Ct.a)(Object(Ct.a)({}, a), {}, {
+            a = t, r = H.a.Children.count(a.children), o = a.listRef, d = Math.ceil(ws(o)), p = a.trackRef && a.trackRef.node, p = Math.ceil(ws(p)), u = a.vertical ? d : (u = a.centerMode && 2 * parseInt(a.centerPadding), "string" == typeof a.centerPadding && "%" === a.centerPadding.slice(-1) && (u *= d / 100), Math.ceil((d - u) / a.slidesToShow)), o = o && ks(o.querySelector('[data-index="0"]')), i = o * a.slidesToShow, l = void 0 === a.currentSlide ? a.initialSlide : a.currentSlide, a.rtl && void 0 === a.currentSlide && (l = r - 1 - a.initialSlide), c = a.lazyLoadedList || [], s = vs(Object(Ct.a)(Object(Ct.a)({}, a), {}, {
                 currentSlide: l,
                 lazyLoadedList: c
             })), r = {
                 slideCount: r,
                 slideWidth: u,
                 listWidth: d,
                 trackWidth: p,
@@ -117692,15 +117708,15 @@
             var a, r, o, i, l, c, s, u = r,
                 d = (t = Object(Ct.a)(Object(Ct.a)(Object(Ct.a)({}, t), u), {}, {
                     slideIndex: u.currentSlide
                 }), Ss(t)),
                 p = (t = Object(Ct.a)(Object(Ct.a)({}, t), {}, {
                     left: d
                 }), Es(t));
-            !e && F.a.Children.count(f.props.children) === F.a.Children.count(t.children) || (u.trackStyle = p), f.setState(u, n)
+            !e && H.a.Children.count(f.props.children) === H.a.Children.count(t.children) || (u.trackStyle = p), f.setState(u, n)
         }), Object(Vt.a)(Object(s.a)(f), "ssrInit", function() {
             if (f.props.variableWidth) {
                 var e = 0,
                     t = 0,
                     n = [],
                     a = Ls(Object(Ct.a)(Object(Ct.a)(Object(Ct.a)({}, f.props), f.state), {}, {
                         slideCount: f.props.children.length
@@ -117718,15 +117734,15 @@
                     width: e + "px",
                     left: -t + "px"
                 };
                 return f.props.centerMode && (s = "".concat(n[f.state.currentSlide], "px"), c.left = "calc(".concat(c.left, " + (100% - ").concat(s, ") / 2 ) ")), {
                     trackStyle: c
                 }
             }
-            var s = F.a.Children.count(f.props.children),
+            var s = H.a.Children.count(f.props.children),
                 c = Object(Ct.a)(Object(Ct.a)(Object(Ct.a)({}, f.props), f.state), {}, {
                     slideCount: s
                 }),
                 s = Ls(c) + is(c) + s,
                 u = 100 / f.props.slidesToShow * s,
                 s = 100 / s,
                 c = -s * (Ls(c) + f.state.currentSlide) * u / 100;
@@ -118082,16 +118098,16 @@
                     focusOnSelect: f.props.focusOnSelect && f.clickable ? f.selectHandler : null
                 }),
                 i = (!0 === f.props.dots && f.state.slideCount >= f.props.slidesToShow && (i = as(r, ["dotsClass", "slideCount", "slidesToShow", "currentSlide", "slidesToScroll", "clickHandler", "children", "customPaging", "infinite", "appendDots"]), n = f.props.pauseOnDotsHover, i = Object(Ct.a)(Object(Ct.a)({}, i), {}, {
                     clickHandler: f.changeSlide,
                     onMouseEnter: n ? f.onDotsLeave : null,
                     onMouseOver: n ? f.onDotsOver : null,
                     onMouseLeave: n ? f.onDotsLeave : null
-                }), n = F.a.createElement(zs, i)), as(r, ["infinite", "centerMode", "currentSlide", "slideCount", "slidesToShow", "prevArrow", "nextArrow"])),
-                r = (i.clickHandler = f.changeSlide, f.props.arrows && (t = F.a.createElement(As, i), e = F.a.createElement(Rs, i)), null),
+                }), n = H.a.createElement(zs, i)), as(r, ["infinite", "centerMode", "currentSlide", "slideCount", "slidesToShow", "prevArrow", "nextArrow"])),
+                r = (i.clickHandler = f.changeSlide, f.props.arrows && (t = H.a.createElement(As, i), e = H.a.createElement(Rs, i)), null),
                 i = (f.props.vertical && (r = {
                     height: f.state.listHeight
                 }), null),
                 r = (!1 === f.props.vertical ? !0 === f.props.centerMode && (i = {
                     padding: "0px " + f.props.centerPadding
                 }) : !0 === f.props.centerMode && (i = {
                     padding: f.props.centerPadding + " 0px"
@@ -118116,22 +118132,22 @@
                     dir: "ltr",
                     style: f.props.style
                 };
             return f.props.unslick && (r = {
                 className: "slick-list"
             }, i = {
                 className: a
-            }), F.a.createElement("div", i, f.props.unslick ? "" : t, F.a.createElement("div", Object(Et.a)({
+            }), H.a.createElement("div", i, f.props.unslick ? "" : t, H.a.createElement("div", Object(Et.a)({
                 ref: f.listRefHandler
-            }, r), F.a.createElement(Ts, Object(Et.a)({
+            }, r), H.a.createElement(Ts, Object(Et.a)({
                 ref: f.trackRefHandler
             }, o), f.props.children)), f.props.unslick ? "" : e, f.props.unslick ? "" : n)
         }), f.list = null, f.track = null, f.state = Object(Ct.a)(Object(Ct.a)({}, Jc), {}, {
             currentSlide: f.props.initialSlide,
-            slideCount: F.a.Children.count(f.props.children)
+            slideCount: H.a.Children.count(f.props.children)
         }), f.callbackTimers = [], f.clickable = !0, f.debouncedResize = null;
         var f, t = f.ssrInit();
         return f.state = Object(Ct.a)(Object(Ct.a)({}, f.state), t), f
     }
 
     function Us() {
         return Object(i.a)(this, Us), hs.apply(this, arguments)
@@ -118196,17 +118212,17 @@
             d = t.tooltip,
             p = t.extra,
             f = t.help,
             h = t.hidden,
             m = t.required,
             g = t.validateStatus,
             t = (t.setProps, t.loading_state);
-        return F.a.createElement(eu.a.Item, {
+        return H.a.createElement(eu.a.Item, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             labelCol: i,
             colon: l,
             wrapperCol: c,
             label: s,
             labelAlign: u,
@@ -118229,17 +118245,17 @@
             o = t.key,
             i = t.labelCol,
             l = t.wrapperCol,
             c = t.colon,
             s = t.labelAlign,
             u = t.layout,
             t = (t.setProps, t.loading_state);
-        return F.a.createElement(eu.a, {
+        return H.a.createElement(eu.a, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             labelCol: i,
             wrapperCol: l,
             colon: c,
             labelAlign: s,
             layout: u,
@@ -118255,15 +118271,15 @@
             o = function(t, e) {
                 var n = {};
                 for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                 if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                     for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                 return n
             }(t, ["prefixCls", "className", "hoverable"]);
-        return Wt.createElement(G.a, null, function(t) {
+        return Wt.createElement(q.a, null, function(t) {
             t = (0, t.getPrefixCls)("card", e), t = Kt()("".concat(t, "-grid"), n, Object(Vt.a)({}, "".concat(t, "-grid-hoverable"), r));
             return Wt.createElement("div", Object(Et.a)({}, o, {
                 className: t
             }))
         })
     }
 
@@ -118272,17 +118288,17 @@
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.hoverable,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return F.a.createElement(ru.Grid, {
+        return H.a.createElement(ru.Grid, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             hoverable: i,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
     var tu = ds,
@@ -118347,15 +118363,15 @@
             setProps: n.a.func
         }, Zs.defaultProps = {
             layout: "horizontal",
             colon: !0,
             labelAlign: "right"
         }, Zs),
         l = Wt.forwardRef(function(n, t) {
-            var e, a = Wt.useContext(G.b),
+            var e, a = Wt.useContext(q.b),
                 r = a.getPrefixCls,
                 a = a.direction,
                 o = Wt.useContext(fi.b),
                 i = n.prefixCls,
                 l = n.className,
                 c = n.extra,
                 s = n.headStyle,
@@ -118447,15 +118463,15 @@
             return Wt.createElement("div", Object(Et.a)({
                 ref: t
             }, M, {
                 className: c
             }), e, _, O, k)
         }),
         ru = (l.Grid = Js, l.Meta = function(l) {
-            return Wt.createElement(G.a, null, function(t) {
+            return Wt.createElement(q.a, null, function(t) {
                 var t = t.getPrefixCls,
                     e = l.prefixCls,
                     n = l.className,
                     a = l.avatar,
                     r = l.title,
                     o = l.description,
                     i = function(t, e) {
@@ -118556,31 +118572,31 @@
             s = t.headStyle,
             u = t.bordered,
             d = t.hoverable,
             p = t.size,
             f = t.title,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return F.a.createElement(ru, {
+        return H.a.createElement(ru, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             bodyStyle: cu({
                 display: "flex",
                 flexWrap: "wrap"
             }, c),
             headStyle: s,
-            extra: F.a.createElement("a", {
+            extra: H.a.createElement("a", {
                 className: i && i.className,
                 style: i && i.style,
                 href: i && i.href,
                 target: i && i.target || "_blank"
             }, i && i.content),
-            cover: F.a.createElement("img", {
+            cover: H.a.createElement("img", {
                 alt: l && l.alt,
                 src: l && l.src,
                 style: l && l.style,
                 className: l && l.className
             }),
             bordered: u,
             hoverable: d,
@@ -118644,15 +118660,15 @@
             i = t.width,
             l = t.height,
             c = t.src,
             s = t.fallback,
             u = t.multiImageMode,
             d = t.preview;
         t.setProps, t.loading_state;
-        o = (t = Object(Wt.useContext)(U.a)) && t.locale || o;
+        o = (t = Object(Wt.useContext)(G.a)) && t.locale || o;
         t = Object(Wt.useState)(!1), p = 2;
         var p = (t = function(t) {
                 if (Array.isArray(t)) return t
             }(t) || function(t, e) {
                 var n = null == t ? null : "undefined" != typeof Symbol && t[Symbol.iterator] || t["@@iterator"];
                 if (null != n) {
                     var a, r, o, i, l = [],
@@ -118678,67 +118694,67 @@
             }(t, p) || function(t, e) {
                 var n;
                 if (t) return "string" == typeof t ? fu(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? fu(t, e) : void 0
             }(t, p) || function() {
                 throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
             }())[0],
             f = t[1];
-        return Array.isArray(c) ? "fold" === u ? F.a.createElement(H.a, {
-            locale: V.b.get(o)
-        }, F.a.createElement(pu.a, {
+        return Array.isArray(c) ? "fold" === u ? H.a.createElement(W.a, {
+            locale: K.b.get(o)
+        }, H.a.createElement(pu.a, {
             id: e,
             style: a,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             key: r,
             preview: {
                 visible: !1
             },
             width: i,
             height: l,
             src: c[0],
             fallback: s,
             onClick: function() {
                 return f(!0)
             }
-        }), F.a.createElement("div", {
+        }), H.a.createElement("div", {
             style: {
                 display: "none"
             }
-        }, F.a.createElement(pu.a.PreviewGroup, {
+        }, H.a.createElement(pu.a.PreviewGroup, {
             preview: {
                 visible: p,
                 onVisibleChange: function(t) {
                     return f(t)
                 }
             }
         }, c.map(function(t) {
-            return F.a.createElement(pu.a, {
+            return H.a.createElement(pu.a, {
                 src: t,
                 fallback: s
             })
-        })))) : F.a.createElement(H.a, {
-            locale: V.b.get(o)
-        }, F.a.createElement(pu.a.PreviewGroup, {
+        })))) : H.a.createElement(W.a, {
+            locale: K.b.get(o)
+        }, H.a.createElement(pu.a.PreviewGroup, {
             id: e,
             style: a,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             key: r
         }, c.map(function(t) {
-            return F.a.createElement(pu.a, {
+            return H.a.createElement(pu.a, {
                 src: t,
                 fallback: s,
                 width: i,
                 height: l
             })
-        }))) : F.a.createElement(H.a, {
-            locale: V.b.get(o)
-        }, F.a.createElement(pu.a, {
+        }))) : H.a.createElement(W.a, {
+            locale: K.b.get(o)
+        }, H.a.createElement(pu.a, {
             id: e,
             style: a,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             key: r,
             width: i,
             height: l,
             src: c,
             fallback: s,
             preview: d
         }))
@@ -118747,15 +118763,15 @@
     function mu(d) {
         function p(t) {
             t = t.width, e(t < 768, !0)
         }
         var t = Object(xu.a)(!1),
             f = (t = Object(Gt.a)(t, 2))[0],
             e = t[1];
-        return Wt.createElement(G.a, null, function(t) {
+        return Wt.createElement(q.a, null, function(t) {
             var e = t.getPrefixCls,
                 n = t.pageHeader,
                 t = t.direction,
                 a = d.prefixCls,
                 r = d.style,
                 o = d.footer,
                 i = d.children,
@@ -118821,17 +118837,17 @@
             c = t.showBackIcon,
             s = t.historyBackDisabled,
             u = t.backClicks,
             d = t.ghost,
             p = t.setProps,
             t = t.loading_state,
             n = j(n);
-        return F.a.createElement(mu, {
+        return H.a.createElement(mu, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             title: i,
             subTitle: l,
             backIcon: !!c && void 0,
             ghost: d,
             onBack: s ? function() {
@@ -119057,15 +119073,15 @@
             h = n.disabledDate,
             m = n.mode,
             g = n.validRange,
             b = void 0 === (M = n.fullscreen) || M,
             v = n.onChange,
             y = n.onPanelChange,
             x = n.onSelect,
-            _ = (M = Wt.useContext(G.b)).getPrefixCls,
+            _ = (M = Wt.useContext(q.b)).getPrefixCls,
             O = M.direction,
             w = _("picker", t),
             k = "".concat(w, "-calendar"),
             j = A.getNow(),
             M = Object($t.a)(function() {
                 return p || A.getNow()
             }, {
@@ -119159,25 +119175,25 @@
             c = t.format,
             s = t.size,
             u = t.setProps,
             d = t.loading_state,
             p = t.persistence,
             f = t.persisted_props,
             t = t.persistence_type,
-            h = Object(Wt.useContext)(U.a),
+            h = Object(Wt.useContext)(G.a),
             o = h && h.locale || o;
         return Object(Wt.useEffect)(function() {
             i && !l && u({
                 value: i
             })
-        }, []), F.a.createElement(H.a, {
-            locale: V.b.get(o)
-        }, F.a.createElement(Pu, {
+        }, []), H.a.createElement(W.a, {
+            locale: K.b.get(o)
+        }, H.a.createElement(Pu, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             defaultValue: i && C()(i, c),
             value: l && C()(l, c),
             onSelect: function(t) {
                 u({
                     value: t.format(c)
@@ -119237,15 +119253,15 @@
             a = t.avatar,
             r = t.children,
             o = t.className,
             i = t.content,
             l = t.prefixCls,
             c = t.datetime,
             t = Hu(t, ["actions", "author", "avatar", "children", "className", "content", "prefixCls", "datetime"]),
-            s = (u = Wt.useContext(G.b)).getPrefixCls,
+            s = (u = Wt.useContext(q.b)).getPrefixCls,
             u = u.direction,
             s = s("comment", l),
             l = a ? Wt.createElement("div", {
                 className: "".concat(s, "-avatar")
             }, "string" == typeof a ? Wt.createElement("img", {
                 src: a,
                 alt: "comment-avatar"
@@ -119314,89 +119330,89 @@
             v = t.dislikesCount,
             y = t.action,
             x = t.defaultAction,
             _ = t.avatarProps,
             O = t.popupContainer,
             w = t.setProps,
             t = t.loading_state,
-            k = Object(Wt.useContext)(U.a),
+            k = Object(Wt.useContext)(G.a),
             k = ("zh-cn" === (o = k && k.locale || o) ? C.a.locale("zh-cn") : "en-us" === o && C.a.locale("en"), n = j(n), Object(Wt.useEffect)(function() {
                 !y && x && w({
                     action: x
                 })
-            }, []), [l ? F.a.createElement(D.a, {
+            }, []), [l ? H.a.createElement(D.a, {
                 key: "comment-basic-like",
                 title: "zh-cn" === o ? "支持" : "like"
-            }, F.a.createElement("span", {
+            }, H.a.createElement("span", {
                 onClick: function() {
                     w({
                         likesCount: "liked" === y ? b - 1 : b + 1,
                         action: "liked" === y ? "default" : "liked",
                         dislikesCount: "disliked" === y ? v - 1 : v
                     })
                 }
-            }, "liked" === y ? F.a.createElement(Vu, {
+            }, "liked" === y ? H.a.createElement(Vu, {
                 style: {
                     color: "rgb(236, 65, 65)"
                 }
-            }) : F.a.createElement(Ku.a, null), F.a.createElement("span", {
+            }) : H.a.createElement(Ku.a, null), H.a.createElement("span", {
                 className: "comment-action"
-            }, b))) : void 0, l ? F.a.createElement(D.a, {
+            }, b))) : void 0, l ? H.a.createElement(D.a, {
                 key: "comment-basic-dislike",
                 title: "zh-cn" === o ? "反对" : "dislike"
-            }, F.a.createElement("span", {
+            }, H.a.createElement("span", {
                 onClick: function() {
                     w({
                         dislikesCount: "disliked" === y ? v - 1 : v + 1,
                         action: "disliked" === y ? "default" : "disliked",
                         likesCount: "liked" === y ? b - 1 : b
                     })
                 }
-            }, F.a.createElement("disliked" === y ? Gu : qu.a), F.a.createElement("span", {
+            }, H.a.createElement("disliked" === y ? Gu : qu.a), H.a.createElement("span", {
                 className: "comment-action"
-            }, v))) : void 0, c ? F.a.createElement("span", {
+            }, v))) : void 0, c ? H.a.createElement("span", {
                 key: "comment-basic-reply-to",
                 onClick: function() {
                     w({
                         replyClicks: u + 1
                     })
                 }
-            }, "zh-cn" === o ? "添加回复" : "Add a reply") : void 0, s ? F.a.createElement(wl.a, {
+            }, "zh-cn" === o ? "添加回复" : "Add a reply") : void 0, s ? H.a.createElement(wl.a, {
                 title: "zh-cn" === o ? "确认删除" : "Confirm deletion",
                 onConfirm: function() {
                     return w({
                         deleteClicks: d + 1
                     })
                 },
                 okText: "zh-cn" === o ? "确认" : "Yes",
                 cancelText: "zh-cn" === o ? "取消" : "No",
                 getPopupContainer: "parent" === O ? function(t) {
                     return t.parentNode
                 } : void 0
-            }, F.a.createElement("span", {
+            }, H.a.createElement("span", {
                 key: "comment-basic-delete"
             }, "zh-cn" === o ? "删除" : "Delete")) : void 0]);
-        return F.a.createElement(H.a, {
-            locale: V.b.get(o)
-        }, F.a.createElement(Iu, {
+        return H.a.createElement(W.a, {
+            locale: K.b.get(o)
+        }, H.a.createElement(Iu, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: i,
             actions: k,
-            author: F.a.createElement("a", {
+            author: H.a.createElement("a", {
                 href: f,
                 target: "_blank"
             }, p),
-            avatar: F.a.createElement(Fc, _),
-            content: F.a.createElement("p", null, g),
-            datetime: F.a.createElement(D.a, {
+            avatar: H.a.createElement(Fc, _),
+            content: H.a.createElement("p", null, g),
+            datetime: H.a.createElement(D.a, {
                 title: C()().format(h.value),
                 placement: "right"
-            }, F.a.createElement("span", null, m ? C()(h.value, h.format || "YYYY-MM-DD HH:mm:ss").fromNow() : h.value)),
+            }, H.a.createElement("span", null, m ? C()(h.value, h.format || "YYYY-MM-DD HH:mm:ss").fromNow() : h.value)),
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n))
     }
     var Fu = Du,
         Hu = function(t, e) {
             var n = {};
             for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
@@ -119646,15 +119662,15 @@
             f = t.layout,
             s = t.children,
             h = t.className,
             m = t.style,
             g = t.size,
             b = t.labelStyle,
             v = t.contentStyle,
-            t = Wt.useContext(G.b),
+            t = Wt.useContext(q.b),
             y = t.getPrefixCls,
             t = t.direction,
             x = y("descriptions", e),
             y = Wt.useState({}),
             e = Object(Gt.a)(y, 2),
             y = e[0],
             _ = e[1],
@@ -119765,28 +119781,28 @@
                             for (var n, a = {}, r = Object.keys(t), o = 0; o < r.length; o++) n = r[o], 0 <= e.indexOf(n) || (a[n] = t[n]);
                             return a
                         }(t, e);
                         if (Object.getOwnPropertySymbols)
                             for (var r = Object.getOwnPropertySymbols(t), o = 0; o < r.length; o++) n = r[o], 0 <= e.indexOf(n) || Object.prototype.propertyIsEnumerable.call(t, n) && (a[n] = t[n]);
                         return a
                     }(e, id);
-                return F.a.createElement(od.Item, ld({
+                return H.a.createElement(od.Item, ld({
                     id: n,
                     className: a,
                     style: r,
                     label: o,
                     span: i,
                     labelStyle: l,
                     contentStyle: c,
                     loading_state: s
                 }, Ao(["setProps", "persistence", "persistence_type", "persisted_props"], e)), t)
             });
-        return F.a.createElement(od, {
+        return H.a.createElement(od, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             title: i,
             column: l,
             bordered: c,
             size: f.get(s),
             layout: u,
@@ -119804,17 +119820,17 @@
             o = t.key,
             i = t.label,
             l = t.span,
             c = t.labelStyle,
             s = t.contentStyle,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return F.a.createElement("div", {
+        return H.a.createElement("div", {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             label: i,
             span: l,
             labelStyle: c,
             contentStyle: s,
             "data-dash-is-loading": t && t.is_loading || void 0
@@ -119839,15 +119855,15 @@
             v = t.offsetTop,
             y = void 0 === (l = t.fontStyle) ? "normal" : l,
             x = void 0 === (l = t.fontWeight) ? "normal" : l,
             _ = void 0 === (l = t.fontColor) ? "rgba(0,0,0,.15)" : l,
             O = void 0 === (l = t.fontSize) ? 16 : l,
             w = void 0 === (l = t.fontFamily) ? "sans-serif" : l,
             l = t.prefixCls,
-            t = (0, Object(Wt.useContext)(H.a.ConfigContext).getPrefixCls)("pro-layout-watermark", l),
+            t = (0, Object(Wt.useContext)(W.a.ConfigContext).getPrefixCls)("pro-layout-watermark", l),
             l = Kt()("".concat(t, "-wrapper"), a),
             a = Kt()(t, o),
             t = Object(Wt.useState)(""),
             t = (o = Object(Gt.a)(t, 2))[0],
             k = o[1];
         return Object(Wt.useEffect)(function() {
             var t, e, n, a = document.createElement("canvas"),
@@ -119858,20 +119874,20 @@
                 c = b || u / 2,
                 s = v || d / 2;
             a.setAttribute("width", i), a.setAttribute("height", l), r ? (r.translate(c * o, s * o), r.rotate(Math.PI / 180 * Number(h)), t = p * o, e = f * o, m ? ((n = new Image).crossOrigin = "anonymous", n.referrerPolicy = "no-referrer", n.src = m, n.onload = function() {
                 r.drawImage(n, 0, 0, t, e), k(a.toDataURL())
             }) : g && (i = Number(O) * o, r.font = "".concat(y, " normal ").concat(x, " ").concat(i, "px/").concat(e, "px ").concat(w), r.fillStyle = _, Array.isArray(g) ? null != g && g.forEach(function(t, e) {
                 return r.fillText(t, 0, 50 * e)
             }) : r.fillText(g, 0, 0), k(a.toDataURL()))) : console.error("当前环境不支持Canvas")
-        }, [u, d, b, v, h, y, x, p, f, w, _, m, g, O]), Object($.jsxs)("div", {
+        }, [u, d, b, v, h, y, x, p, f, w, _, m, g, O]), Object(F.jsxs)("div", {
             style: Object(Ct.a)({
                 position: "relative"
             }, n),
             className: l,
-            children: [e, Object($.jsx)("div", {
+            children: [e, Object(F.jsx)("div", {
                 className: a,
                 style: Object(Ct.a)(Object(Ct.a)({
                     zIndex: i,
                     position: "absolute",
                     left: 0,
                     top: 0,
                     width: "100%",
@@ -119897,15 +119913,15 @@
             c = t.zIndex,
             s = t.fontColor,
             u = t.fontSize,
             d = t.gapX,
             p = t.gapY,
             t = t.loading_state,
             n = j(n);
-        return F.a.createElement(ud, {
+        return H.a.createElement(ud, {
             id: e,
             className: a,
             style: r,
             key: o,
             content: i,
             rotate: l,
             zIndex: c,
@@ -119976,15 +119992,15 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
         }, sd.defaultProps = {
             span: 1
         }, sd),
-        $ = (e(298), e(31)),
+        F = (e(298), e(31)),
         gd = (dd.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.string,
             style: n.a.object,
             key: n.a.string,
             content: n.a.string,
@@ -120204,15 +120220,15 @@
                 a = t.className,
                 r = t.block,
                 o = t.options,
                 i = void 0 === o ? [] : o,
                 o = t.size,
                 o = void 0 === o ? "middle" : o,
                 t = _d(t, ["prefixCls", "className", "block", "options", "size"]),
-                l = Wt.useContext(G.b),
+                l = Wt.useContext(q.b),
                 c = l.getPrefixCls,
                 l = l.direction,
                 s = c("segmented", n),
                 c = Wt.useContext(fi.b),
                 n = o || c,
                 o = Wt.useMemo(function() {
                     return i.map(function(t) {
@@ -120288,37 +120304,37 @@
             s = t.disabled,
             u = t.size,
             d = t.setProps,
             p = t.persistence,
             f = t.persisted_props,
             h = t.persistence_type,
             t = t.loading_state,
-            m = Object(Wt.useContext)(U.a),
+            m = Object(Wt.useContext)(G.a),
             o = o || [];
         return Object(Wt.useEffect)(function() {
             i && !l && d({
                 value: i
             })
-        }, []), F.a.createElement(wd, {
+        }, []), H.a.createElement(wd, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: n,
             key: r,
             options: o.map(function(t) {
                 return Md(Md({}, t), {}, {
-                    icon: t.icon && F.a.createElement(R.a, {
+                    icon: t.icon && H.a.createElement(I.a, {
                         icon: t.icon
                     })
                 })
             }),
             defaultValue: i,
             value: l,
             block: c,
-            disabled: m && !Object(W.isUndefined)(m.componentDisabled) ? m.componentDisabled : s,
-            size: m && !Object(W.isUndefined)(m.componentSize) ? m.componentSize : u,
+            disabled: m && !Object(V.isUndefined)(m.componentDisabled) ? m.componentDisabled : s,
+            size: m && !Object(V.isUndefined)(m.componentSize) ? m.componentSize : u,
             persistence: p,
             persisted_props: f,
             persistence_type: h,
             onChange: function(t) {
                 d({
                     value: t
                 })
@@ -120330,78 +120346,78 @@
     function Cd(t, e) {
         return t = Object($t.a)(t, e), [(e = Object(Gt.a)(t, 2))[0], e[1]]
     }
 
     function Sd(t) {
         var t = t.prefixCls,
             e = "".concat(t, "-loading-block");
-        return Object($.jsxs)("div", {
+        return Object(F.jsxs)("div", {
             className: "".concat(t, "-loading-content"),
-            children: [Object($.jsx)(ua, {
+            children: [Object(F.jsx)(ua, {
                 gutter: 8,
-                children: Object($.jsx)(pa, {
+                children: Object(F.jsx)(pa, {
                     span: 22,
-                    children: Object($.jsx)("div", {
+                    children: Object(F.jsx)("div", {
                         className: e
                     })
                 })
-            }), Object($.jsxs)(ua, {
+            }), Object(F.jsxs)(ua, {
                 gutter: 8,
-                children: [Object($.jsx)(pa, {
+                children: [Object(F.jsx)(pa, {
                     span: 8,
-                    children: Object($.jsx)("div", {
+                    children: Object(F.jsx)("div", {
                         className: e
                     })
-                }), Object($.jsx)(pa, {
+                }), Object(F.jsx)(pa, {
                     span: 15,
-                    children: Object($.jsx)("div", {
+                    children: Object(F.jsx)("div", {
                         className: e
                     })
                 })]
-            }), Object($.jsxs)(ua, {
+            }), Object(F.jsxs)(ua, {
                 gutter: 8,
-                children: [Object($.jsx)(pa, {
+                children: [Object(F.jsx)(pa, {
                     span: 6,
-                    children: Object($.jsx)("div", {
+                    children: Object(F.jsx)("div", {
                         className: e
                     })
-                }), Object($.jsx)(pa, {
+                }), Object(F.jsx)(pa, {
                     span: 18,
-                    children: Object($.jsx)("div", {
+                    children: Object(F.jsx)("div", {
                         className: e
                     })
                 })]
-            }), Object($.jsxs)(ua, {
+            }), Object(F.jsxs)(ua, {
                 gutter: 8,
-                children: [Object($.jsx)(pa, {
+                children: [Object(F.jsx)(pa, {
                     span: 13,
-                    children: Object($.jsx)("div", {
+                    children: Object(F.jsx)("div", {
                         className: e
                     })
-                }), Object($.jsx)(pa, {
+                }), Object(F.jsx)(pa, {
                     span: 9,
-                    children: Object($.jsx)("div", {
+                    children: Object(F.jsx)("div", {
                         className: e
                     })
                 })]
-            }), Object($.jsxs)(ua, {
+            }), Object(F.jsxs)(ua, {
                 gutter: 8,
-                children: [Object($.jsx)(pa, {
+                children: [Object(F.jsx)(pa, {
                     span: 4,
-                    children: Object($.jsx)("div", {
+                    children: Object(F.jsx)("div", {
                         className: e
                     })
-                }), Object($.jsx)(pa, {
+                }), Object(F.jsx)(pa, {
                     span: 3,
-                    children: Object($.jsx)("div", {
+                    children: Object(F.jsx)("div", {
                         className: e
                     })
-                }), Object($.jsx)(pa, {
+                }), Object(F.jsx)(pa, {
                     span: 16,
-                    children: Object($.jsx)("div", {
+                    children: Object(F.jsx)("div", {
                         className: e
                     })
                 })]
             })]
         })
     }
 
@@ -120409,15 +120425,15 @@
         var t = Cd(n.defaultChecked || !1, {
                 value: n.checked,
                 onChange: n.onChange
             }),
             a = (t = Object(Gt.a)(t, 2))[0],
             r = t[1],
             o = Object(Wt.useContext)(Rd),
-            t = Object(Wt.useContext)(H.a.ConfigContext).getPrefixCls,
+            t = Object(Wt.useContext)(W.a.ConfigContext).getPrefixCls,
             e = (Object(Wt.useEffect)(function() {
                 var t;
                 return null != o && null != (t = o.registerValue) && t.call(o, n.value),
                     function() {
                         var t;
                         return null == o || null == (t = o.cancelValue) ? void 0 : t.call(o, n.value)
                     }
@@ -120439,50 +120455,50 @@
             g = f.loading,
             b = void 0 === (b = f.bordered) || b,
             f = f.checked,
             e = "large" === e ? "lg" : "small" === e ? "sm" : "",
             e = Kt()(h, i, (i = {}, Object(Vt.a)(i, "".concat(h, "-loading"), g), Object(Vt.a)(i, "".concat(h, "-").concat(e), e), Object(Vt.a)(i, "".concat(h, "-checked"), f), Object(Vt.a)(i, "".concat(h, "-multiple"), t), Object(Vt.a)(i, "".concat(h, "-disabled"), m), Object(Vt.a)(i, "".concat(h, "-bordered"), b), i)),
             f = Object(Wt.useMemo)(function() {
                 var t, e, n, a;
-                return g ? Object($.jsx)(Sd, {
+                return g ? Object(F.jsx)(Sd, {
                     prefixCls: h || ""
-                }) : u ? (t = h || "", e = u, Object($.jsx)("div", {
+                }) : u ? (t = h || "", e = u, Object(F.jsx)("div", {
                     className: "".concat(t, "-cover"),
-                    children: "string" == typeof e ? Object($.jsx)("img", {
+                    children: "string" == typeof e ? Object(F.jsx)("img", {
                         src: e,
                         alt: "checkcard"
                     }) : e
-                })) : (t = l ? Object($.jsx)("div", {
+                })) : (t = l ? Object(F.jsx)("div", {
                     className: "".concat(h, "-avatar"),
-                    children: "string" == typeof l ? Object($.jsx)(Bc.a, {
+                    children: "string" == typeof l ? Object(F.jsx)(Bc.a, {
                         size: 48,
                         shape: "square",
                         src: l
                     }) : l
-                }) : null, e = (c || d) && Object($.jsxs)("div", {
+                }) : null, e = (c || d) && Object(F.jsxs)("div", {
                     className: "".concat(h, "-header"),
-                    children: [Object($.jsx)("div", {
+                    children: [Object(F.jsx)("div", {
                         className: "".concat(h, "-title"),
                         children: c
-                    }), d && Object($.jsx)("div", {
+                    }), d && Object(F.jsx)("div", {
                         className: "".concat(h, "-extra"),
                         children: d
                     })]
-                }), n = s ? Object($.jsx)("div", {
+                }), n = s ? Object(F.jsx)("div", {
                     className: "".concat(h, "-description"),
                     children: s
-                }) : null, a = Kt()("".concat(h, "-content"), Object(Vt.a)({}, "".concat(h, "-avatar-header"), t && e && !n)), Object($.jsxs)("div", {
+                }) : null, a = Kt()("".concat(h, "-content"), Object(Vt.a)({}, "".concat(h, "-avatar-header"), t && e && !n)), Object(F.jsxs)("div", {
                     className: a,
-                    children: [t, e || n ? Object($.jsxs)("div", {
+                    children: [t, e || n ? Object(F.jsxs)("div", {
                         className: "".concat(h, "-detail"),
                         children: [e, n]
                     }) : null]
                 }))
             }, [l, g, u, s, d, h, c]);
-        return Object($.jsx)("div", {
+        return Object(F.jsx)("div", {
             className: e,
             style: p,
             onClick: function(t) {
                 var e;
                 g || m || (null != n && null != (e = n.onClick) && e.call(n, t), e = !a, null != o && null != (t = o.toggleOption) && t.call(o, {
                     value: n.value
                 }), null != r && r(e))
@@ -120504,30 +120520,30 @@
             u = t.disabled,
             d = t.size,
             p = t.setProps,
             f = t.loading_state,
             h = t.persistence,
             m = t.persisted_props,
             t = t.persistence_type,
-            g = Object(Wt.useContext)(U.a);
+            g = Object(Wt.useContext)(G.a);
         return Object(Wt.useEffect)(function() {
-            !Object(W.isUndefined)(s) && Object(W.isUndefined)(i) && p({
+            !Object(V.isUndefined)(s) && Object(V.isUndefined)(i) && p({
                 checked: s
             })
-        }, []), F.a.createElement(Nd, {
+        }, []), H.a.createElement(Nd, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             description: n,
             checked: i,
             bordered: l,
             value: c,
             defaultChecked: s,
-            disabled: g && !Object(W.isUndefined)(g.componentDisabled) ? g.componentDisabled : u,
+            disabled: g && !Object(V.isUndefined)(g.componentDisabled) ? g.componentDisabled : u,
             size: d,
             onChange: function(t) {
                 return p({
                     checked: t
                 })
             },
             persistence: h,
@@ -120550,29 +120566,29 @@
             u = t.disabled,
             d = t.size,
             p = t.setProps,
             f = t.loading_state,
             h = t.persistence,
             m = t.persisted_props,
             t = t.persistence_type,
-            g = Object(Wt.useContext)(U.a);
+            g = Object(Wt.useContext)(G.a);
         return Object(Wt.useEffect)(function() {
             s && !c && p({
                 value: s
             })
-        }, []), n = j(n), F.a.createElement(Nd.Group, {
+        }, []), n = j(n), H.a.createElement(Nd.Group, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             multiple: i,
             bordered: l,
             value: c,
             defaultValue: s,
-            disabled: g && !Object(W.isUndefined)(g.componentDisabled) ? g.componentDisabled : u,
+            disabled: g && !Object(V.isUndefined)(g.componentDisabled) ? g.componentDisabled : u,
             size: d,
             onChange: function(t) {
                 return p({
                     value: t
                 })
             },
             persistence: h,
@@ -120597,17 +120613,17 @@
             p = t.ghost,
             f = t.loading_state,
             h = t.setProps;
         return Object(Wt.useEffect)(function() {
             c && !l && h({
                 activeKey: c
             })
-        }, []), F.a.createElement(la.a, {
+        }, []), H.a.createElement(la.a, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             accordion: i,
             activeKey: l,
             defaultActiveKey: c,
             bordered: s,
             collapsible: u,
@@ -120616,16 +120632,16 @@
             onChange: function(t) {
                 return h({
                     activeKey: t
                 })
             },
             "data-dash-is-loading": f && f.is_loading || void 0
         }, o ? o.map(function(t) {
-            return F.a.createElement(Fd, {
-                className: Object(W.isString)(t.className) ? t.className : t.className ? Object(K.a)(t.className) : void 0,
+            return H.a.createElement(Fd, {
+                className: Object(V.isString)(t.className) ? t.className : t.className ? Object(U.a)(t.className) : void 0,
                 style: t.style,
                 key: t.key,
                 collapsible: t.collapsible,
                 header: t.title,
                 extra: t.extra,
                 showArrow: t.showArrow,
                 forceRender: t.forceRender
@@ -120677,15 +120693,15 @@
                 r = a.loading,
                 i = void 0 !== r && r,
                 r = a.multiple,
                 l = void 0 !== r && r,
                 r = a.bordered,
                 r = void 0 === r || r,
                 c = (a.onChange, Object(Bt.a)(a, Ad)),
-                s = Object(Wt.useContext)(H.a.ConfigContext),
+                s = Object(Wt.useContext)(W.a.ConfigContext),
                 u = Object(Wt.useCallback)(function() {
                     return null == o ? void 0 : o.map(function(t) {
                         return "string" == typeof t ? {
                             title: t,
                             value: t
                         } : t
                     })
@@ -120702,35 +120718,35 @@
                 }),
                 c = Object(Gt.a)(c, 2),
                 d = c[0],
                 p = c[1],
                 f = Object(Wt.useRef)(new Map),
                 c = Object(Wt.useMemo)(function() {
                     var n;
-                    return i ? new Array(o.length || F.a.Children.toArray(a.children).length || 1).fill(0).map(function(t, e) {
-                        return Object($.jsx)(Nd, {
+                    return i ? new Array(o.length || H.a.Children.toArray(a.children).length || 1).fill(0).map(function(t, e) {
+                        return Object(F.jsx)(Nd, {
                             loading: !0
                         }, e)
                     }) : o && 0 < o.length ? (n = d, u().map(function(t) {
                         var e;
-                        return Object($.jsx)(Nd, {
+                        return Object(F.jsx)(Nd, {
                             disabled: t.disabled,
                             size: null != (e = t.size) ? e : a.size,
                             value: t.value,
                             checked: l ? null == n ? void 0 : n.includes(t.value) : n === t.value,
                             onChange: t.onChange,
                             title: t.title,
                             avatar: t.avatar,
                             description: t.description,
                             cover: t.cover
                         }, t.value.toString())
                     })) : a.children
                 }, [u, i, l, o, a.children, a.size, d]),
                 t = Kt()(t, e);
-            return Object($.jsx)(Rd.Provider, {
+            return Object(F.jsx)(Rd.Provider, {
                 value: {
                     toggleOption: function(e) {
                         var t, n, a, r;
                         l || (r = d === e.value ? void 0 : e.value, null == p) || p(r), l && (r = [], n = null == (t = d) ? void 0 : t.includes(e.value), r = Object(Ut.a)(t || []), n || r.push(e.value), n && (r = r.filter(function(t) {
                             return t !== e.value
                         })), a = u(), r = null == (t = r) || null == (n = t.filter(function(t) {
                             return f.current.has(t)
@@ -120753,15 +120769,15 @@
                         null != (e = f.current) && e.set(t, !0)
                     },
                     cancelValue: function(t) {
                         var e;
                         null != (e = f.current) && e.delete(t)
                     }
                 },
-                children: Object($.jsx)("div", Object(Ct.a)(Object(Ct.a)({
+                children: Object(F.jsx)("div", Object(Ct.a)(Object(Ct.a)({
                     className: t,
                     style: n
                 }, s), {}, {
                     children: c
                 }))
             })
         }, Ld),
@@ -120830,25 +120846,25 @@
             style: n.a.object,
             key: n.a.string,
             items: n.a.arrayOf(n.a.exact({
                 children: n.a.node,
                 className: n.a.oneOfType([n.a.string, n.a.object]),
                 style: n.a.object,
                 key: n.a.oneOfType([n.a.string, n.a.number]).isRequired,
-                collapsible: n.a.oneOf(["header", "disabled"]),
+                collapsible: n.a.oneOf(["header", "disabled", "icon"]),
                 title: n.a.node,
                 extra: n.a.node,
                 showArrow: n.a.bool,
                 forceRender: n.a.bool
             })),
             accordion: n.a.bool,
             activeKey: n.a.oneOfType([n.a.string, n.a.arrayOf(n.a.string), n.a.number, n.a.arrayOf(n.a.number)]),
             defaultActiveKey: n.a.oneOfType([n.a.string, n.a.arrayOf(n.a.string), n.a.number, n.a.arrayOf(n.a.number)]),
             bordered: n.a.bool,
-            collapsible: n.a.oneOf(["header", "disabled"]),
+            collapsible: n.a.oneOf(["header", "disabled", "icon"]),
             expandIconPosition: n.a.oneOf(["left", "right"]),
             ghost: n.a.bool,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
@@ -121026,19 +121042,19 @@
                         onKeyDown: p ? this.onKeyDown : function() {},
                         onMouseEnter: f,
                         onMouseLeave: h,
                         onDrop: this.onFileDrop,
                         onDragOver: this.onFileDrop,
                         tabIndex: "0"
                     };
-                return F.a.createElement(e, Object(Et.a)({}, m, {
+                return H.a.createElement(e, Object(Et.a)({}, m, {
                     className: n,
                     role: "button",
                     style: i
-                }), F.a.createElement("input", Object(Et.a)({}, Object(Ud.a)(t, {
+                }), H.a.createElement("input", Object(Et.a)({}, Object(Ud.a)(t, {
                     aria: !0,
                     data: !0
                 }), {
                     id: o,
                     type: "file",
                     ref: this.saveFileInput,
                     onClick: function(t) {
@@ -121171,15 +121187,15 @@
         key: "abort",
         value: function(t) {
             this.uploader.abort(t)
         }
     }, {
         key: "render",
         value: function() {
-            return F.a.createElement(np, Object(Et.a)({}, this.props, {
+            return H.a.createElement(np, Object(Et.a)({}, this.props, {
                 ref: this.saveUploader
             }))
         }
     }]);
     var op, c = ip;
 
     function ip() {
@@ -121490,15 +121506,15 @@
                 L = "picture-card" === i && "uploading" !== k && Wt.createElement("span", {
                     className: "".concat(n, "-list-item-actions")
                 }, y, "done" === k && m, u),
                 h = l.response && "string" == typeof l.response ? l.response : (null == (g = l.error) ? void 0 : g.statusText) || (null == (v = l.error) ? void 0 : v.message) || o.uploadError,
                 b = Wt.createElement("span", {
                     className: t
                 }, S, d),
-                y = (0, Wt.useContext(G.b).getPrefixCls)(),
+                y = (0, Wt.useContext(q.b).getPrefixCls)(),
                 m = Wt.createElement("div", {
                     className: f
                 }, Wt.createElement("div", {
                     className: "".concat(n, "-list-item-info")
                 }, b), L, M && Wt.createElement(Er.b, {
                     motionName: "".concat(y, "-fade"),
                     visible: "uploading" === k,
@@ -121556,17 +121572,17 @@
                     title: a,
                     onClick: function(t) {
                         n(), Object(je.c)(e) && e.props.onClick && e.props.onClick(t)
                     },
                     className: "".concat(t, "-list-item-card-actions-btn")
                 }, Object(je.c)(e) ? (t = Object(je.a)(e, Object(Et.a)(Object(Et.a)({}, e.props), {
                     onClick: function() {}
-                })), Wt.createElement(T.a, Object(Et.a)({}, a, {
+                })), Wt.createElement(z.a, Object(Et.a)({}, a, {
                     icon: t
-                }))) : Wt.createElement(T.a, Object(Et.a)({}, a), Wt.createElement("span", null, e))
+                }))) : Wt.createElement(z.a, Object(Et.a)({}, a), Wt.createElement("span", null, e))
             }
             var n = t.listType,
                 s = void 0 === n ? "text" : n,
                 n = t.previewFile,
                 a = void 0 === n ? wp : n,
                 u = t.onPreview,
                 d = t.onDownload,
@@ -121610,15 +121626,15 @@
                 }, [s, b, a]), Wt.useEffect(function() {
                     S(!0)
                 }, []), Wt.useImperativeHandle(e, function() {
                     return {
                         handlePreview: r,
                         handleDownload: o
                     }
-                }), Wt.useContext(G.b)),
+                }), Wt.useContext(q.b)),
                 e = t.getPrefixCls,
                 t = t.direction,
                 L = e("upload", n),
                 n = Kt()((e = {}, Object(Vt.a)(e, "".concat(L, "-list"), !0), Object(Vt.a)(e, "".concat(L, "-list-").concat(s), !0), Object(Vt.a)(e, "".concat(L, "-list-rtl"), "rtl" === t), e)),
                 t = Object(Ut.a)(b.map(function(t) {
                     return {
                         key: t.uid,
@@ -121853,15 +121869,15 @@
                         onBatchStart: e,
                         onSuccess: n,
                         onProgress: a,
                         onError: r,
                         fileList: D,
                         upload: T.current
                     }
-                }), Wt.useContext(G.b)),
+                }), Wt.useContext(q.b)),
                 p = c.getPrefixCls,
                 t = c.direction,
                 A = p("upload", x),
                 c = Object(Et.a)(Object(Et.a)({
                     onBatchStart: e,
                     onError: r,
                     onProgress: a,
@@ -122087,15 +122103,15 @@
 
     function Jp() {
         for (var t = [], e = 0; e < arguments.length; e++) t[e] = arguments[e];
         return t.filter(function(t) {
             return "string" == typeof t && 0 < t.length
         }).join(" ").trim()
     }
-    Qp = F.a.Component, Bp(tf = f, l = Qp), tf.prototype = null === l ? Object.create(l) : (nf.prototype = l.prototype, new nf), f.prototype.componentDidMount = function() {
+    Qp = H.a.Component, Bp(tf = f, l = Qp), tf.prototype = null === l ? Object.create(l) : (nf.prototype = l.prototype, new nf), f.prototype.componentDidMount = function() {
         this.currentDoc && this.currentWindow && (this.containerRef && (this.containerRef.ownerDocument && (this.currentDoc = this.containerRef.ownerDocument), this.currentDoc.defaultView && (this.currentWindow = this.currentDoc.defaultView), this.initResizeObserver(), void 0 === window.ResizeObserver && this.currentWindow.addEventListener("resize", this.computeSizes), this.props.zoomWithScroll && this.containerRef.addEventListener("wheel", this.onWheel, {
             passive: !1
         }), this.containerRef.addEventListener("gesturestart", this.onGestureStart)), this.props.disableAutomaticStylesInjection || (this.styleRef = this.currentDoc.createElement("style"), this.styleRef.setAttribute("type", "text/css"), this.props.nonce && this.styleRef.setAttribute("nonce", this.props.nonce), this.styleRef.innerHTML = ".reactEasyCrop_Container {\n  position: absolute;\n  top: 0;\n  left: 0;\n  right: 0;\n  bottom: 0;\n  overflow: hidden;\n  user-select: none;\n  touch-action: none;\n  cursor: move;\n  display: flex;\n  justify-content: center;\n  align-items: center;\n}\n\n.reactEasyCrop_Image,\n.reactEasyCrop_Video {\n  will-change: transform; /* this improves performances and prevent painting issues on iOS Chrome */\n}\n\n.reactEasyCrop_Contain {\n  max-width: 100%;\n  max-height: 100%;\n  margin: auto;\n  position: absolute;\n  top: 0;\n  bottom: 0;\n  left: 0;\n  right: 0;\n}\n.reactEasyCrop_Cover_Horizontal {\n  width: 100%;\n  height: auto;\n}\n.reactEasyCrop_Cover_Vertical {\n  width: auto;\n  height: 100%;\n}\n\n.reactEasyCrop_CropArea {\n  position: absolute;\n  left: 50%;\n  top: 50%;\n  transform: translate(-50%, -50%);\n  border: 1px solid rgba(255, 255, 255, 0.5);\n  box-sizing: border-box;\n  box-shadow: 0 0 0 9999em;\n  color: rgba(0, 0, 0, 0.5);\n  overflow: hidden;\n}\n\n.reactEasyCrop_CropAreaRound {\n  border-radius: 50%;\n}\n\n.reactEasyCrop_CropAreaGrid::before {\n  content: ' ';\n  box-sizing: border-box;\n  position: absolute;\n  border: 1px solid rgba(255, 255, 255, 0.5);\n  top: 0;\n  bottom: 0;\n  left: 33.33%;\n  right: 33.33%;\n  border-top: 0;\n  border-bottom: 0;\n}\n\n.reactEasyCrop_CropAreaGrid::after {\n  content: ' ';\n  box-sizing: border-box;\n  position: absolute;\n  border: 1px solid rgba(255, 255, 255, 0.5);\n  top: 33.33%;\n  bottom: 33.33%;\n  left: 0;\n  right: 0;\n  border-left: 0;\n  border-right: 0;\n}\n", this.currentDoc.head.appendChild(this.styleRef)), this.imageRef.current && this.imageRef.current.complete && this.onMediaLoad(), this.props.setImageRef && this.props.setImageRef(this.imageRef), this.props.setVideoRef) && this.props.setVideoRef(this.videoRef)
     }, f.prototype.componentWillUnmount = function() {
         var t;
         this.currentDoc && this.currentWindow && (void 0 === window.ResizeObserver && this.currentWindow.removeEventListener("resize", this.computeSizes), null != (t = this.resizeObserver) && t.disconnect(), this.containerRef && this.containerRef.removeEventListener("gesturestart", this.preventZoomSafari), this.styleRef && null != (t = this.styleRef.parentNode) && t.removeChild(this.styleRef), this.cleanEvents(), this.props.zoomWithScroll) && this.clearScrollEvent()
     }, f.prototype.componentDidUpdate = function(t) {
@@ -122142,52 +122158,52 @@
             h = p.cropAreaStyle,
             p = p.mediaStyle,
             m = t.classes,
             g = m.containerClassName,
             b = m.cropAreaClassName,
             m = m.mediaClassName,
             t = t.objectFit;
-        return F.a.createElement("div", {
+        return H.a.createElement("div", {
             onMouseDown: this.onMouseDown,
             onTouchStart: this.onTouchStart,
             ref: function(t) {
                 return e.containerRef = t
             },
             "data-testid": "container",
             style: f,
             className: Jp("reactEasyCrop_Container", g)
-        }, n ? F.a.createElement("img", Fp({
+        }, n ? H.a.createElement("img", Fp({
             alt: "",
             className: Jp("reactEasyCrop_Image", "contain" === t && "reactEasyCrop_Contain", "horizontal-cover" === t && "reactEasyCrop_Cover_Horizontal", "vertical-cover" === t && "reactEasyCrop_Cover_Vertical", "auto-cover" === t && (this.mediaSize.naturalWidth > this.mediaSize.naturalHeight ? "reactEasyCrop_Cover_Horizontal" : "reactEasyCrop_Cover_Vertical"), m)
         }, r, {
             src: n,
             ref: this.imageRef,
             style: Fp(Fp({}, p), {
                 transform: o || "translate(".concat(l, "px, ").concat(i, "px) rotate(").concat(c, "deg) scale(").concat(s, ")")
             }),
             onLoad: this.onMediaLoad
-        })) : a && F.a.createElement("video", Fp({
+        })) : a && H.a.createElement("video", Fp({
             autoPlay: !0,
             loop: !0,
             muted: !0,
             className: Jp("reactEasyCrop_Video", "contain" === t && "reactEasyCrop_Contain", "horizontal-cover" === t && "reactEasyCrop_Cover_Horizontal", "vertical-cover" === t && "reactEasyCrop_Cover_Vertical", "auto-cover" === t && (this.mediaSize.naturalWidth > this.mediaSize.naturalHeight ? "reactEasyCrop_Cover_Horizontal" : "reactEasyCrop_Cover_Vertical"), m)
         }, r, {
             ref: this.videoRef,
             onLoadedMetadata: this.onMediaLoad,
             style: Fp(Fp({}, p), {
                 transform: o || "translate(".concat(l, "px, ").concat(i, "px) rotate(").concat(c, "deg) scale(").concat(s, ")")
             }),
             controls: !1
         }), (Array.isArray(a) ? a : [{
             src: a
         }]).map(function(t) {
-            return F.a.createElement("source", Fp({
+            return H.a.createElement("source", Fp({
                 key: t.src
             }, t))
-        })), this.state.cropSize && F.a.createElement("div", {
+        })), this.state.cropSize && H.a.createElement("div", {
             style: Fp(Fp({}, h), {
                 width: this.state.cropSize.width,
                 height: this.state.cropSize.height
             }),
             "data-testid": "cropper",
             className: Jp("reactEasyCrop_CropArea", "round" === u && "reactEasyCrop_CropAreaRound", d && "reactEasyCrop_CropAreaGrid", b)
         }))
@@ -122217,15 +122233,15 @@
             y: Number(t.clientY)
         }
     };
     var Qp, tf, ef = f;
 
     function f() {
         var d = null !== Qp && Qp.apply(this, arguments) || this;
-        return d.imageRef = F.a.createRef(), d.videoRef = F.a.createRef(), d.containerRef = null, d.styleRef = null, d.containerRect = null, d.mediaSize = {
+        return d.imageRef = H.a.createRef(), d.videoRef = H.a.createRef(), d.containerRef = null, d.styleRef = null, d.containerRect = null, d.mediaSize = {
             width: 0,
             height: 0,
             naturalWidth: 0,
             naturalHeight: 0
         }, d.dragStartPosition = {
             x: 0,
             y: 0
@@ -122472,16 +122488,16 @@
             Object(Wt.useImperativeHandle)(e, () => ({
                 setZoom: g,
                 rotation: b,
                 setRotation: v,
                 cropPixelsRef: k
             }));
             t = "flex items-center w-3/5 mx-auto", e = "flex items-center justify-center w-8 h-8 bg-transparent border-0 font-[inherit] text-[18px] cursor-pointer disabled:opacity-20 disabled:cursor-default";
-            return Object($.jsxs)($.Fragment, {
-                children: [Object($.jsx)(ef, Object.assign({}, f, {
+            return Object(F.jsxs)(F.Fragment, {
+                children: [Object(F.jsx)(ef, Object.assign({}, f, {
                     ref: n,
                     image: l,
                     crop: O,
                     zoom: m,
                     rotation: b,
                     aspect: y,
                     minZoom: s,
@@ -122493,84 +122509,84 @@
                     onZoomChange: g,
                     onRotationChange: v,
                     onCropComplete: j,
                     classes: {
                         containerClassName: af + "-container !relative w-full h-[40vh] [&~section:first-of-type]:mt-4 [&~section:last-of-type]:mb-4",
                         mediaClassName: af + "-media"
                     }
-                })), a && Object($.jsxs)("section", Object.assign({
+                })), a && Object(F.jsxs)("section", Object.assign({
                     className: af + `-control ${af}-control-zoom ` + t
                 }, {
-                    children: [Object($.jsx)("button", Object.assign({
+                    children: [Object(F.jsx)("button", Object.assign({
                         className: e,
                         onClick: () => g(m - .1),
                         disabled: !0
                     }, {
                         children: "－"
-                    })), Object($.jsx)(me, {
+                    })), Object(F.jsx)(me, {
                         className: "flex-1 mx-2",
                         min: s,
                         max: u,
                         step: .1,
                         value: m,
                         onChange: g
-                    }), Object($.jsx)("button", Object.assign({
+                    }), Object(F.jsx)("button", Object.assign({
                         className: e,
                         onClick: () => g(m + .1),
                         disabled: m + .1 > u
                     }, {
                         children: "＋"
                     }))]
-                })), r && Object($.jsxs)("section", Object.assign({
+                })), r && Object(F.jsxs)("section", Object.assign({
                     className: af + `-control ${af}-control-rotation ` + t
                 }, {
-                    children: [Object($.jsx)("button", Object.assign({
+                    children: [Object(F.jsx)("button", Object.assign({
                         className: e + " !text-[16px]",
                         onClick: () => v(b - 1),
                         disabled: -180 === b
                     }, {
                         children: "↺"
-                    })), Object($.jsx)(me, {
+                    })), Object(F.jsx)(me, {
                         className: "flex-1 mx-2",
                         min: -180,
                         max: 180,
                         step: 1,
                         value: b,
                         onChange: v
-                    }), Object($.jsx)("button", Object.assign({
+                    }), Object(F.jsx)("button", Object.assign({
                         className: e + " !text-[16px]",
                         onClick: () => v(b + 1),
                         disabled: 180 === b
                     }, {
                         children: "↻"
                     }))]
-                })), o && Object($.jsxs)("section", Object.assign({
+                })), o && Object(F.jsxs)("section", Object.assign({
                     className: af + `-control ${af}-control-aspect ` + t
                 }, {
-                    children: [Object($.jsx)("button", Object.assign({
+                    children: [Object(F.jsx)("button", Object.assign({
                         className: e,
                         onClick: () => x(y - .01),
                         disabled: y - .01 < .5
                     }, {
                         children: "↕️"
-                    })), Object($.jsx)(me, {
+                    })), Object(F.jsx)(me, {
                         className: "flex-1 mx-2",
                         min: .5,
                         max: 2,
                         step: .01,
                         value: y,
                         onChange: x
-                    }), Object($.jsx)("button", Object.assign({
+                    }), Object(F.jsx)("button", Object.assign({
                         className: e,
                         onClick: () => x(y + .01),
                         disabled: 2 < y + .01
                     }, {
                         children: "↔️"
                     }))]
-                })), i && (a || r || o) && Object($.jsx)(T.a, Object.assign({
+                })), i && (a || r || o) && Object(F.jsx)(z.a, Object.assign({
                     className: "absolute bottom-[20px]",
                     style: _ ? {} : {
                         opacity: .3,
                         pointerEvents: "none"
                     },
                     onClick: () => {
                         g(1), v(0), x(c)
@@ -122682,26 +122698,26 @@
                             e = yield S.current(n, [n]);
                         !0 === e ? L.current(t) : !1 === e ? P.current(new Error("beforeUpload → false")) : L.current(e)
                     } catch (t) {
                         P.current(new Error("beforeUpload → reject"))
                     } else L.current(t)
                 }), d, m)
             }), [g, m, O]), Y = af + "-modal" + (l ? " " + l : ""), A = "zh-CN" === ("undefined" == typeof window ? "" : window.navigator.language), B = c || (A ? "编辑图片" : "Edit image");
-            return Object($.jsxs)($.Fragment, {
-                children: [D, M && Object($.jsx)(dr, Object.assign({}, b, R, {
+            return Object(F.jsxs)(F.Fragment, {
+                children: [D, M && Object(F.jsx)(dr, Object.assign({}, b, R, {
                     [lf]: !0
                 }, {
                     title: B,
                     onOk: N,
                     onCancel: I,
                     wrapClassName: Y,
                     maskClosable: !1,
                     destroyOnClose: !0
                 }, {
-                    children: Object($.jsx)(of, {
+                    children: Object(F.jsx)(of, {
                         ref: T,
                         cropperRef: e,
                         zoomSlider: _,
                         rotationSlider: O,
                         aspectSlider: n,
                         showReset: p,
                         image: M,
@@ -123132,52 +123148,54 @@
             d = t.editable,
             p = t.editConfig,
             f = t.uploadId,
             h = t.fileListMaxLength,
             m = t.buttonContent,
             g = t.fileTypes,
             b = t.fileMaxSize,
-            v = t.failedTooltipInfo,
-            y = t.showRemoveIcon,
-            x = t.showPreviewIcon,
-            _ = t.confirmBeforeDelete,
-            O = t.showPercent,
-            w = t.progressProps,
-            R = t.showSuccessMessage,
-            I = t.showErrorMessage,
-            k = t.listUploadTaskRecord,
-            j = t.defaultFileList,
-            M = t.disabled,
-            E = t.status,
-            C = t.loading_state,
-            S = t.setProps,
-            l = (t = Object(Wt.useContext)(U.a)) && t.locale || l,
-            L = (A = k = k || [], n = new Map, A.forEach(function(t) {
+            R = t.failedTooltipInfo,
+            v = t.showRemoveIcon,
+            y = t.showPreviewIcon,
+            x = t.confirmBeforeDelete,
+            _ = t.showPercent,
+            O = t.progressProps,
+            I = t.showSuccessMessage,
+            N = t.showErrorMessage,
+            w = t.listUploadTaskRecord,
+            k = t.defaultFileList,
+            j = t.disabled,
+            M = t.status,
+            E = t.loading_state,
+            C = t.setProps,
+            l = (t = Object(Wt.useContext)(G.a)) && t.locale || l,
+            S = (A = w = w || [], n = new Map, A.forEach(function(t) {
                 n.set(t.uid, t.completeTimestamp)
             }), n);
         Object(Wt.useEffect)(function() {
-            f || S({
+            f || (k && 0 < k.length ? C({
+                uploadId: k[0].taskId || Object(Wd.a)()
+            }) : C({
                 uploadId: Object(Wd.a)()
-            })
+            }))
         }, []);
-        var j = (A = gf(Object(Wt.useState)(j || k.map(function(t) {
+        var L = (A = gf(Object(Wt.useState)(k || w.map(function(t) {
                 return {
                     name: t.fileName,
                     status: t.taskStatus,
                     uid: t.uid,
                     url: t.url
                 }
             })), 2))[0],
-            N = A[1],
+            Y = A[1],
             P = (A = gf(Object(Wt.useState)(!1), 2))[0],
             D = A[1],
             T = (A = gf(Object(Wt.useState)(""), 2))[0],
-            Y = A[1],
-            z = (A = gf(Object(Wt.useState)(""), 2))[0],
             B = A[1],
+            z = (A = gf(Object(Wt.useState)(""), 2))[0],
+            F = A[1],
             A = function() {
                 var l;
                 l = hf().mark(function t(e) {
                     return hf().wrap(function(t) {
                         for (;;) switch (t.prev = t.next) {
                             case 0:
                                 if (e.url || e.preview) {
@@ -123193,15 +123211,15 @@
                                     }, n.onerror = function(t) {
                                         return e(t)
                                     }
                                 });
                             case 3:
                                 e.preview = t.sent;
                             case 4:
-                                Y(e.url || e.preview), D(!0), B(e.name || e.url.substring(e.url.lastIndexOf("/") + 1));
+                                B(e.url || e.preview), D(!0), F(e.name || e.url.substring(e.url.lastIndexOf("/") + 1));
                             case 7:
                             case "end":
                                 return t.stop()
                         }
                     }, t)
                 });
                 return function(t) {
@@ -123219,183 +123237,183 @@
                                 mf(a, e, n, r, o, "throw", t)
                             }
                             r(void 0)
                         })
                     }.apply(this, arguments)
                 }
             }(),
-            m = F.a.createElement("div", null, F.a.createElement(Dp.a, null), F.a.createElement("div", {
+            m = H.a.createElement("div", null, H.a.createElement(Dp.a, null), H.a.createElement("div", {
                 style: {
                     marginTop: 8
                 }
             }, m)),
             c = {
                 name: "file",
                 action: c + "?uploadId=".concat(f),
                 headers: s,
                 data: {
                     uploadId: f
                 },
                 beforeUpload: function(t) {
                     var e = t.size / 1024 / 1024 < b;
-                    return e || X.b.error("".concat(t.name).concat(V.a.Upload[l].sizeError[0]).concat(b).concat(V.a.Upload[l].sizeError[1])), g ? (-1 === g.indexOf(t.name.split(".")[t.name.split(".").length - 1]) && X.b.error("".concat(V.a.Upload[l].typeError[0]).concat(t.name).concat(V.a.Upload[l].typeError[1])), e && -1 !== g.indexOf(t.name.split(".")[t.name.split(".").length - 1])) : e
+                    return e || $.b.error("".concat(t.name).concat(K.a.Upload[l].sizeError[0]).concat(b).concat(K.a.Upload[l].sizeError[1])), g ? (-1 === g.indexOf(t.name.split(".")[t.name.split(".").length - 1]) && $.b.error("".concat(K.a.Upload[l].typeError[0]).concat(t.name).concat(K.a.Upload[l].typeError[1])), e && -1 !== g.indexOf(t.name.split(".")[t.name.split(".").length - 1])) : e
                 },
                 onChange: function(t) {
-                    var e, n = "removed" === t.file.status ? 0 : t.fileList.length - k.length,
-                        t = ("removed" === t.file.status ? S({
+                    var e, n = "removed" === t.file.status ? 0 : t.fileList.length - w.length,
+                        t = ("removed" === t.file.status ? C({
                             listUploadTaskRecord: t.fileList.map(function(t) {
                                 var e = u && "done" === t.status ? {
                                     url: u + "?taskId=".concat(f, "&filename=").concat(t.name)
                                 } : {};
                                 return ff({
                                     fileName: t.name,
                                     fileSize: t.size,
-                                    completeTimestamp: L.get(t.uid) || (new Date).getTime(),
+                                    completeTimestamp: S.get(t.uid) || (new Date).getTime(),
                                     taskStatus: "done" === t.status ? "success" : "failed",
                                     taskId: f,
                                     uid: t.uid
                                 }, e)
                             })
-                        }) : "done" !== t.file.status && "error" !== t.file.status && t.file.status || S({
+                        }) : "done" !== t.file.status && "error" !== t.file.status && t.file.status || C({
                             lastUploadTaskRecord: {
                                 fileName: t.file.name,
                                 fileSize: t.file.size,
                                 completeTimestamp: (new Date).getTime(),
                                 taskStatus: "done" === t.file.status ? "success" : "failed",
                                 taskId: f
                             },
                             listUploadTaskRecord: t.fileList.map(function(t) {
                                 var e = u && "done" === t.status ? {
                                     url: u + "?taskId=".concat(f, "&filename=").concat(t.name)
                                 } : {};
                                 return ff({
                                     fileName: t.name,
                                     fileSize: t.size,
-                                    completeTimestamp: L.get(t.uid) || (new Date).getTime(),
+                                    completeTimestamp: S.get(t.uid) || (new Date).getTime(),
                                     taskStatus: "done" === t.status ? "success" : "failed",
                                     taskId: f,
                                     uid: t.uid
                                 }, e)
                             })
-                        }), "done" === t.file.status && R ? X.b.success("".concat(t.file.name, " 上传成功！")) : "error" === t.file.status && I && X.b.error("".concat(t.file.name, " 上传失败！")), function(t) {
+                        }), "done" === t.file.status && I ? $.b.success("".concat(t.file.name, " 上传成功！")) : "error" === t.file.status && N && $.b.error("".concat(t.file.name, " 上传失败！")), function(t) {
                             if (Array.isArray(t)) return vf(t)
                         }(e = t.fileList) || function() {
                             if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
                         }() || bf(e) || function() {
                             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                         }());
                     h && (t = t.slice(-h)), 0 != n && (t = t.slice(0, t.length - n).concat(t.slice(-n).map(function(t) {
-                        return "error" !== t.status && t.status || (t.status = "error", t.response = v || "上传失败"), t
-                    }))), N(u ? t.map(function(t) {
+                        return "error" !== t.status && t.status || (t.status = "error", t.response = R || "上传失败"), t
+                    }))), Y(u ? t.map(function(t) {
                         return ff(ff({}, t), {}, {
                             url: u + "?taskId=".concat(f, "&filename=").concat(t.name)
                         })
                     }) : t)
                 }
             };
         return g && 0 != g.length && Object.assign(c, {
             accept: "." + g.join(",.")
-        }), d ? F.a.createElement(H.a, {
-            locale: V.b.get(l)
-        }, F.a.createElement("div", {
+        }), d ? H.a.createElement(W.a, {
+            locale: K.b.get(l)
+        }, H.a.createElement("div", {
             id: a,
-            className: Object(W.isString)(r) ? r : r ? Object(K.a)(r) : void 0,
+            className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
             style: ff(ff({
                 border: "1px solid transparent",
                 transition: "border 0.3s"
-            }, xf.get(E)), o),
+            }, xf.get(M)), o),
             key: i
-        }, F.a.createElement(sf, df({
+        }, H.a.createElement(sf, df({
             modalOk: "zh-cn" === l ? "确定" : "OK",
             modalCancel: "zh-cn" === l ? "取消" : "Cancel"
-        }, p), F.a.createElement(Pp, df({}, c, {
-            fileList: j,
+        }, p), H.a.createElement(Pp, df({}, c, {
+            fileList: L,
             listType: "picture-card",
-            disabled: t && !Object(W.isUndefined)(t.componentDisabled) ? t.componentDisabled : M,
-            progress: w || O ? {
-                strokeColor: w && w.strokeColor,
-                strokeWidth: w && w.strokeWidth || 2,
-                format: O ? function(t) {
-                    return t && "".concat(w && w.prefix || "").concat(parseFloat(t.toFixed(1))).concat(w && w.suffix || "%")
+            disabled: t && !Object(V.isUndefined)(t.componentDisabled) ? t.componentDisabled : j,
+            progress: O || _ ? {
+                strokeColor: O && O.strokeColor,
+                strokeWidth: O && O.strokeWidth || 2,
+                format: _ ? function(t) {
+                    return t && "".concat(O && O.prefix || "").concat(parseFloat(t.toFixed(1))).concat(O && O.suffix || "%")
                 } : void 0
             } : void 0,
             showUploadList: {
-                showRemoveIcon: y,
-                showPreviewIcon: x
+                showRemoveIcon: v,
+                showPreviewIcon: y
             },
             onPreview: A,
-            onRemove: _ ? function() {
+            onRemove: x ? function() {
                 return new Promise(function(t, e) {
                     dr.confirm({
-                        title: V.a.AntdPictureUpload[l].confirmBeforeDeleteTitle,
-                        okText: V.a.AntdPictureUpload[l].confirmBeforeDeleteOkText,
-                        cancelText: V.a.AntdPictureUpload[l].confirmBeforeDeleteCancelText,
+                        title: K.a.AntdPictureUpload[l].confirmBeforeDeleteTitle,
+                        okText: K.a.AntdPictureUpload[l].confirmBeforeDeleteOkText,
+                        cancelText: K.a.AntdPictureUpload[l].confirmBeforeDeleteCancelText,
                         onOk: function() {
                             t(!0)
                         }
                     })
                 })
             } : void 0,
-            "data-dash-is-loading": C && C.is_loading || void 0
-        }), m)), F.a.createElement(dr, {
+            "data-dash-is-loading": E && E.is_loading || void 0
+        }), m)), H.a.createElement(dr, {
             visible: P,
             title: z,
             footer: null,
             onCancel: e
-        }, F.a.createElement("img", {
+        }, H.a.createElement("img", {
             alt: "",
             style: {
                 width: "100%"
             },
             src: T
-        })))) : F.a.createElement(H.a, {
-            locale: V.b.get(l)
-        }, F.a.createElement("div", {
+        })))) : H.a.createElement(W.a, {
+            locale: K.b.get(l)
+        }, H.a.createElement("div", {
             id: a,
-            className: Object(W.isString)(r) ? r : r ? Object(K.a)(r) : void 0,
+            className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
             style: ff(ff({
                 border: "1px solid transparent",
                 transition: "border 0.3s"
-            }, xf.get(E)), o),
+            }, xf.get(M)), o),
             key: i
-        }, F.a.createElement(Pp, df({}, c, {
-            fileList: j,
+        }, H.a.createElement(Pp, df({}, c, {
+            fileList: L,
             listType: "picture-card",
-            disabled: t && !Object(W.isUndefined)(t.componentDisabled) ? t.componentDisabled : M,
-            progress: w || O ? {
-                strokeColor: w && w.strokeColor,
-                strokeWidth: w && w.strokeWidth || 2,
-                format: O ? function(t) {
-                    return t && "".concat(w && w.prefix || "").concat(parseFloat(t.toFixed(1))).concat(w && w.suffix || "%")
+            disabled: t && !Object(V.isUndefined)(t.componentDisabled) ? t.componentDisabled : j,
+            progress: O || _ ? {
+                strokeColor: O && O.strokeColor,
+                strokeWidth: O && O.strokeWidth || 2,
+                format: _ ? function(t) {
+                    return t && "".concat(O && O.prefix || "").concat(parseFloat(t.toFixed(1))).concat(O && O.suffix || "%")
                 } : void 0
             } : void 0,
             showUploadList: {
-                showRemoveIcon: y,
-                showPreviewIcon: x
+                showRemoveIcon: v,
+                showPreviewIcon: y
             },
             onPreview: A,
-            onRemove: _ ? function() {
+            onRemove: x ? function() {
                 return new Promise(function(t, e) {
                     dr.confirm({
-                        title: V.a.AntdPictureUpload[l].confirmBeforeDeleteTitle,
-                        okText: V.a.AntdPictureUpload[l].confirmBeforeDeleteOkText,
-                        cancelText: V.a.AntdPictureUpload[l].confirmBeforeDeleteCancelText,
+                        title: K.a.AntdPictureUpload[l].confirmBeforeDeleteTitle,
+                        okText: K.a.AntdPictureUpload[l].confirmBeforeDeleteOkText,
+                        cancelText: K.a.AntdPictureUpload[l].confirmBeforeDeleteCancelText,
                         onOk: function() {
                             t(!0)
                         }
                     })
                 })
             } : void 0,
-            "data-dash-is-loading": C && C.is_loading || void 0
-        }), m), F.a.createElement(dr, {
+            "data-dash-is-loading": E && E.is_loading || void 0
+        }), m), H.a.createElement(dr, {
             visible: P,
             title: z,
             footer: null,
             onCancel: e
-        }, F.a.createElement("img", {
+        }, H.a.createElement("img", {
             alt: "",
             style: {
                 width: "100%"
             },
             src: T
         }))))
     }
@@ -123482,15 +123500,16 @@
                 uid: n.a.string,
                 url: n.a.string
             })),
             defaultFileList: n.a.arrayOf(n.a.exact({
                 name: n.a.string,
                 status: n.a.oneOf(["done", "error", "removed"]),
                 uid: n.a.any,
-                url: n.a.string
+                url: n.a.string,
+                taskId: n.a.string
             })),
             disabled: n.a.bool,
             status: n.a.oneOf(["error", "warning"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
@@ -123605,31 +123624,33 @@
             M = t.showErrorMessage,
             E = t.listUploadTaskRecord,
             C = t.defaultFileList,
             S = t.disabled,
             L = t.status,
             P = t.loading_state,
             D = t.setProps,
-            c = (t = Object(Wt.useContext)(U.a)) && t.locale || c,
+            c = (t = Object(Wt.useContext)(G.a)) && t.locale || c,
             T = (A = E = E || [], e = new Map, A.forEach(function(t) {
                 e.set(t.uid, t.completeTimestamp)
             }), e);
         Object(Wt.useEffect)(function() {
-            h || D({
+            h || (C && 0 < C.length ? D({
+                uploadId: C[0].taskId || Object(Wd.a)()
+            }) : D({
                 uploadId: Object(Wd.a)()
-            })
+            }))
         }, []), A = Object(Wt.useState)(C || E.map(function(t) {
             return {
                 name: t.fileName,
                 status: t.taskStatus,
                 uid: t.uid,
                 url: t.url
             }
-        })), C = 2;
-        var C = (A = function(t) {
+        })), z = 2;
+        var z = (A = function(t) {
                 if (Array.isArray(t)) return t
             }(A) || function(t, e) {
                 var n = null == t ? null : "undefined" != typeof Symbol && t[Symbol.iterator] || t["@@iterator"];
                 if (null != n) {
                     var a, r, o, i, l = [],
                         c = !0,
                         s = !1;
@@ -123646,28 +123667,28 @@
                             if (!c && null != n.return && (i = n.return(), Object(i) !== i)) return
                         } finally {
                             if (s) throw r
                         }
                     }
                     return l
                 }
-            }(A, C) || Mf(A, C) || function() {
+            }(A, z) || Mf(A, z) || function() {
                 throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
             }())[0],
-            z = A[1],
+            R = A[1],
             A = {
                 name: "file",
                 action: s + "?uploadId=".concat(h),
                 headers: u,
                 data: {
                     uploadId: h
                 },
                 beforeUpload: function(t) {
                     var e = t.size / 1024 / 1024 < b;
-                    return e || X.b.error("".concat(t.name).concat(V.a.Upload[c].sizeError[0]).concat(b).concat(V.a.Upload[c].sizeError[1])), g ? (-1 === g.indexOf(t.name.split(".")[t.name.split(".").length - 1]) && X.b.error("".concat(V.a.Upload[c].typeError[0]).concat(t.name).concat(V.a.Upload[c].typeError[1])), e && -1 !== g.indexOf(t.name.split(".")[t.name.split(".").length - 1])) : e
+                    return e || $.b.error("".concat(t.name).concat(K.a.Upload[c].sizeError[0]).concat(b).concat(K.a.Upload[c].sizeError[1])), g ? (-1 === g.indexOf(t.name.split(".")[t.name.split(".").length - 1]) && $.b.error("".concat(K.a.Upload[c].typeError[0]).concat(t.name).concat(K.a.Upload[c].typeError[1])), e && -1 !== g.indexOf(t.name.split(".")[t.name.split(".").length - 1])) : e
                 },
                 onChange: function(t) {
                     var e, n = "removed" === t.file.status ? 0 : t.fileList.length - E.length,
                         t = (y || x ? "removed" === t.file.status ? D({
                             listUploadTaskRecord: t.fileList.map(function(t) {
                                 var e = d && "done" === t.status ? {
                                     url: d + "?taskId=".concat(h, "&filename=").concat(t.name)
@@ -123739,77 +123760,77 @@
                                     fileSize: t.size,
                                     completeTimestamp: T.get(t.uid) || (new Date).getTime(),
                                     taskStatus: "done" === t.status ? "success" : "failed",
                                     taskId: h,
                                     uid: t.uid
                                 }, e)
                             })
-                        }), "done" === t.file.status && j ? X.b.success("".concat(t.file.name, " 上传成功！")) : "error" === t.file.status && M && X.b.error("".concat(t.file.name, " 上传失败！")), function(t) {
+                        }), "done" === t.file.status && j ? $.b.success("".concat(t.file.name, " 上传成功！")) : "error" === t.file.status && M && $.b.error("".concat(t.file.name, " 上传失败！")), function(t) {
                             if (Array.isArray(t)) return Ef(t)
                         }(e = t.fileList) || function() {
                             if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
                         }() || Mf(e) || function() {
                             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                         }());
                     m && (t = t.slice(-m)), 0 != n && (t = t.slice(0, t.length - n).concat(t.slice(-n).map(function(t) {
                         return "error" !== t.status && t.status || (t.status = "error", t.response = _ || "上传失败"), t
-                    }))), z(d ? t.map(function(t) {
+                    }))), R(d ? t.map(function(t) {
                         return jf(jf({}, t), {}, {
                             url: d + "?taskId=".concat(h, "&filename=").concat(t.name)
                         })
                     }) : t)
                 }
             };
         return g && 0 != g.length && Object.assign(A, {
             accept: "." + g.join(",.")
-        }), F.a.createElement(H.a, {
-            locale: V.b.get(c)
-        }, F.a.createElement("div", {
+        }), H.a.createElement(W.a, {
+            locale: K.b.get(c)
+        }, H.a.createElement("div", {
             id: n,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: jf(jf({
                 border: "1px solid transparent",
                 transition: "border 0.3s"
             }, Pf.get(L)), r),
             key: l,
             "data-dash-is-loading": P && P.is_loading || void 0
-        }, F.a.createElement(Lf, wf({
+        }, H.a.createElement(Lf, wf({
             draggerStyle: i,
-            draggerClassName: Object(W.isString)(o) ? o : o ? Object(K.a)(o) : void 0,
-            fileList: C,
+            draggerClassName: Object(V.isString)(o) ? o : o ? Object(U.a)(o) : void 0,
+            fileList: z,
             showUploadList: v,
             multiple: y,
             directory: x,
-            disabled: t && !Object(W.isUndefined)(t.componentDisabled) ? t.componentDisabled : S,
+            disabled: t && !Object(V.isUndefined)(t.componentDisabled) ? t.componentDisabled : S,
             progress: k || w ? {
                 strokeColor: k && k.strokeColor,
                 strokeWidth: k && k.strokeWidth || 2,
                 format: w ? function(t) {
                     return t && "".concat(k && k.prefix || "").concat(parseFloat(t.toFixed(1))).concat(k && k.suffix || "%")
                 } : void 0
             } : void 0,
             onRemove: O ? function() {
                 return new Promise(function(t, e) {
                     dr.confirm({
-                        title: V.a.AntdPictureUpload[c].confirmBeforeDeleteTitle,
-                        okText: V.a.AntdPictureUpload[c].confirmBeforeDeleteOkText,
-                        cancelText: V.a.AntdPictureUpload[c].confirmBeforeDeleteCancelText,
+                        title: K.a.AntdPictureUpload[c].confirmBeforeDeleteTitle,
+                        okText: K.a.AntdPictureUpload[c].confirmBeforeDeleteOkText,
+                        cancelText: K.a.AntdPictureUpload[c].confirmBeforeDeleteCancelText,
                         onOk: function() {
                             t(!0)
                         }
                     })
                 })
             } : void 0
-        }, A), F.a.createElement("p", {
+        }, A), H.a.createElement("p", {
             className: "ant-upload-drag-icon"
-        }, F.a.createElement(R.a, {
+        }, H.a.createElement(I.a, {
             icon: "antd-cloud-upload"
-        })), F.a.createElement("p", {
+        })), H.a.createElement("p", {
             className: "ant-upload-text"
-        }, p), F.a.createElement("p", {
+        }, p), H.a.createElement("p", {
             className: "ant-upload-hint"
         }, f))))
     }
 
     function Sf(t, e) {
         return Wt.createElement(to.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
             ref: e,
@@ -123897,15 +123918,16 @@
                 uid: n.a.string,
                 url: n.a.string
             }))]),
             defaultFileList: n.a.arrayOf(n.a.exact({
                 name: n.a.string,
                 status: n.a.oneOf(["done", "error", "removed"]),
                 uid: n.a.any,
-                url: n.a.string
+                url: n.a.string,
+                taskId: n.a.string
             })),
             disabled: n.a.bool,
             status: n.a.oneOf(["error", "warning"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
@@ -124034,33 +124056,35 @@
             w = t.showErrorMessage,
             k = t.listUploadTaskRecord,
             j = t.defaultFileList,
             M = t.disabled,
             E = t.status,
             C = t.loading_state,
             S = t.setProps,
-            i = (t = Object(Wt.useContext)(U.a)) && t.locale || i,
-            L = (D = k = k || [], e = new Map, D.forEach(function(t) {
+            i = (t = Object(Wt.useContext)(G.a)) && t.locale || i,
+            L = (T = k = k || [], e = new Map, T.forEach(function(t) {
                 e.set(t.uid, t.completeTimestamp)
             }), e);
         Object(Wt.useEffect)(function() {
-            u || S({
+            u || (j && 0 < j.length ? S({
+                uploadId: j[0].taskId || Object(Wd.a)()
+            }) : S({
                 uploadId: Object(Wd.a)()
-            })
-        }, []), D = Object(Wt.useState)(j || k.map(function(t) {
+            }))
+        }, []), T = Object(Wt.useState)(j || k.map(function(t) {
             return {
                 name: t.fileName,
                 status: t.taskStatus,
                 uid: t.uid,
                 url: t.url
             }
-        })), j = 2;
-        var j = (D = function(t) {
+        })), P = 2;
+        var P = (T = function(t) {
                 if (Array.isArray(t)) return t
-            }(D) || function(t, e) {
+            }(T) || function(t, e) {
                 var n = null == t ? null : "undefined" != typeof Symbol && t[Symbol.iterator] || t["@@iterator"];
                 if (null != n) {
                     var a, r, o, i, l = [],
                         c = !0,
                         s = !1;
                     try {
                         if (o = (n = n.call(t)).next, 0 === e) {
@@ -124075,28 +124099,28 @@
                             if (!c && null != n.return && (i = n.return(), Object(i) !== i)) return
                         } finally {
                             if (s) throw r
                         }
                     }
                     return l
                 }
-            }(D, j) || Yf(D, j) || function() {
+            }(T, P) || Yf(T, P) || function() {
                 throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
             }())[0],
-            P = D[1],
-            D = {
+            D = T[1],
+            T = {
                 name: "file",
                 action: l + "?uploadId=".concat(u),
                 headers: c,
                 data: {
                     uploadId: u
                 },
                 beforeUpload: function(t) {
                     var e = t.size / 1024 / 1024 < h;
-                    return e || X.b.error("".concat(t.name).concat(V.a.Upload[i].sizeError[0]).concat(h).concat(V.a.Upload[i].sizeError[1])), f ? (-1 === f.indexOf(t.name.split(".")[t.name.split(".").length - 1]) && X.b.error("".concat(V.a.Upload[i].typeError[0]).concat(t.name).concat(V.a.Upload[i].typeError[1])), e && -1 !== f.indexOf(t.name.split(".")[t.name.split(".").length - 1])) : e
+                    return e || $.b.error("".concat(t.name).concat(K.a.Upload[i].sizeError[0]).concat(h).concat(K.a.Upload[i].sizeError[1])), f ? (-1 === f.indexOf(t.name.split(".")[t.name.split(".").length - 1]) && $.b.error("".concat(K.a.Upload[i].typeError[0]).concat(t.name).concat(K.a.Upload[i].typeError[1])), e && -1 !== f.indexOf(t.name.split(".")[t.name.split(".").length - 1])) : e
                 },
                 onChange: function(t) {
                     var e, n = "removed" === t.file.status ? 0 : t.fileList.length - k.length,
                         t = (g || b ? "removed" === t.file.status ? S({
                             listUploadTaskRecord: t.fileList.map(function(t) {
                                 var e = s && "done" === t.status ? {
                                     url: s + "?taskId=".concat(u, "&filename=").concat(t.name)
@@ -124168,71 +124192,71 @@
                                     fileSize: t.size,
                                     completeTimestamp: L.get(t.uid) || (new Date).getTime(),
                                     taskStatus: "done" === t.status ? "success" : "failed",
                                     taskId: u,
                                     uid: t.uid
                                 }, e)
                             })
-                        }), "done" === t.file.status && O ? X.b.success("".concat(t.file.name, " 上传成功！")) : "error" === t.file.status && w && X.b.error("".concat(t.file.name, " 上传失败！")), function(t) {
+                        }), "done" === t.file.status && O ? $.b.success("".concat(t.file.name, " 上传成功！")) : "error" === t.file.status && w && $.b.error("".concat(t.file.name, " 上传失败！")), function(t) {
                             if (Array.isArray(t)) return Bf(t)
                         }(e = t.fileList) || function() {
                             if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
                         }() || Yf(e) || function() {
                             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                         }());
                     d && (t = t.slice(-d)), 0 != n && (t = t.slice(0, t.length - n).concat(t.slice(-n).map(function(t) {
                         return "error" !== t.status && t.status || (t.status = "error", t.response = v || "上传失败"), t
-                    }))), P(s ? t.map(function(t) {
+                    }))), D(s ? t.map(function(t) {
                         return Nf(Nf({}, t), {}, {
                             url: s + "?taskId=".concat(u, "&filename=").concat(t.name)
                         })
                     }) : t)
                 }
             };
-        return f && 0 != f.length && Object.assign(D, {
+        return f && 0 != f.length && Object.assign(T, {
             accept: "." + f.join(",.")
-        }), F.a.createElement(H.a, {
-            locale: V.b.get(i)
-        }, F.a.createElement("div", {
+        }), H.a.createElement(W.a, {
+            locale: K.b.get(i)
+        }, H.a.createElement("div", {
             id: n,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: Nf(Nf({
                 border: "1px solid transparent",
                 transition: "border 0.3s"
             }, Hf.get(E)), r),
             key: o
-        }, F.a.createElement(Pp, Rf({}, D, {
-            fileList: j,
+        }, H.a.createElement(Pp, Rf({}, T, {
+            fileList: P,
             multiple: g,
             showUploadList: m,
             directory: b,
-            disabled: t && !Object(W.isUndefined)(t.componentDisabled) ? t.componentDisabled : M,
+            disabled: t && !Object(V.isUndefined)(t.componentDisabled) ? t.componentDisabled : M,
             progress: _ || x ? {
                 strokeColor: _ && _.strokeColor,
                 strokeWidth: _ && _.strokeWidth || 2,
                 format: x ? function(t) {
                     return t && "".concat(_ && _.prefix || "").concat(parseFloat(t.toFixed(1))).concat(_ && _.suffix || "%")
                 } : void 0
             } : void 0,
             onRemove: y ? function() {
                 return new Promise(function(t, e) {
                     dr.confirm({
-                        title: V.a.AntdPictureUpload[i].confirmBeforeDeleteTitle,
-                        okText: V.a.AntdPictureUpload[i].confirmBeforeDeleteOkText,
-                        cancelText: V.a.AntdPictureUpload[i].confirmBeforeDeleteCancelText,
+                        title: K.a.AntdPictureUpload[i].confirmBeforeDeleteTitle,
+                        okText: K.a.AntdPictureUpload[i].confirmBeforeDeleteOkText,
+                        cancelText: K.a.AntdPictureUpload[i].confirmBeforeDeleteCancelText,
                         onOk: function() {
                             t(!0)
                         }
                     })
                 })
             } : void 0,
             "data-dash-is-loading": C && C.is_loading || void 0
-        }), F.a.createElement(T.a, {
-            icon: F.a.createElement(zf, null),
-            disabled: t && !Object(W.isUndefined)(t.componentDisabled) ? t.componentDisabled : M
+        }), H.a.createElement(z.a, {
+            icon: H.a.createElement(zf, null),
+            disabled: t && !Object(V.isUndefined)(t.componentDisabled) ? t.componentDisabled : M
         }, p || "点击上传文件"))))
     }
     var Hf = new Map([
             ["warning", {
                 border: "1px solid #faad14",
                 borderRadius: "2px",
                 padding: "6px 10px",
@@ -124300,15 +124324,16 @@
                 uid: n.a.string,
                 url: n.a.string
             })),
             defaultFileList: n.a.arrayOf(n.a.exact({
                 name: n.a.string,
                 status: n.a.oneOf(["done", "error", "removed"]),
                 uid: n.a.any,
-                url: n.a.string
+                url: n.a.string,
+                taskId: n.a.string
             })),
             disabled: n.a.bool,
             status: n.a.oneOf(["error", "warning"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
@@ -124383,17 +124408,17 @@
             }())[0],
             h = t[1],
             m = Object(Wt.useRef)();
         return Object(Wt.useEffect)(function() {
             p && (m.current && clearTimeout(m.current), p.is_loading && !f ? "default" === c ? (d && console.log(p.component_name + "." + p.prop_name), h(!0)) : "exclude" === c ? -1 === s.indexOf(p.component_name + "." + p.prop_name) && (d && console.log(p.component_name + "." + p.prop_name), h(!0)) : "include" === c && -1 !== u.indexOf(p.component_name + "." + p.prop_name) && (d && console.log(p.component_name + "." + p.prop_name), h(!0)) : !p.is_loading && f && (m.current = setTimeout(function() {
                 return h(!1)
             })))
-        }, [p]), F.a.createElement("div", {
+        }, [p]), H.a.createElement("div", {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             "data-dash-is-loading": p && p.is_loading || void 0
         }, f ? i : o)
     }
 
     function Uf(t) {
@@ -124401,18 +124426,18 @@
             n = t.style,
             a = t.className,
             r = t.key,
             o = t.active,
             i = t.shape,
             l = t.size,
             c = t.loading_state;
-        return t.setProps, F.a.createElement(Dl.Avatar, {
+        return t.setProps, H.a.createElement(Dl.Avatar, {
             id: e,
             style: n,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             key: r,
             active: o,
             shape: i,
             size: l,
             "data-dash-is-loading": c && c.is_loading || void 0
         })
     }
@@ -124423,18 +124448,18 @@
             a = t.className,
             r = t.key,
             o = t.active,
             i = t.block,
             l = t.shape,
             c = t.size,
             s = t.loading_state;
-        return t.setProps, F.a.createElement(Dl.Button, {
+        return t.setProps, H.a.createElement(Dl.Button, {
             id: e,
             style: n,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             key: r,
             active: o,
             block: i,
             shape: l,
             size: c,
             "data-dash-is-loading": s && s.is_loading || void 0
         })
@@ -124444,35 +124469,35 @@
         var e = t.id,
             n = t.style,
             a = t.className,
             r = t.key,
             o = t.active,
             i = t.size,
             l = t.loading_state;
-        return t.setProps, F.a.createElement(Dl.Input, {
+        return t.setProps, H.a.createElement(Dl.Input, {
             id: e,
             style: n,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             key: r,
             active: o,
             size: i,
             "data-dash-is-loading": l && l.is_loading || void 0
         })
     }
 
     function Xf(t) {
         var e = t.id,
             n = t.style,
             a = t.className,
             r = t.key,
             o = t.loading_state;
-        return t.setProps, F.a.createElement(Dl.Image, {
+        return t.setProps, H.a.createElement(Dl.Image, {
             id: e,
             style: n,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             key: r,
             "data-dash-is-loading": o && o.is_loading || void 0
         })
     }
     Kf._dashprivate_isLoadingComponent = !0, Kf.propTypes = {
         id: n.a.string,
         children: n.a.node,
@@ -124652,45 +124677,45 @@
             v = t.colors,
             y = t.inputNumberStyle,
             x = t.colorBlockPosition,
             _ = t.colorBlockStyle,
             O = t.pureLegendLabelStyle,
             w = t.loading_state,
             k = t.setProps,
-            c = (t = Object(Wt.useContext)(U.a)) && !Object(W.isUndefined)(t.componentDisabled) ? t.componentDisabled : c,
-            o = t && !Object(W.isUndefined)(t.componentSize) ? t.componentSize : o;
-        return F.a.createElement(za.b, {
+            c = (t = Object(Wt.useContext)(G.a)) && !Object(V.isUndefined)(t.componentDisabled) ? t.componentDisabled : c,
+            o = t && !Object(V.isUndefined)(t.componentSize) ? t.componentSize : o;
+        return H.a.createElement(za.b, {
             id: e,
             key: n,
             style: oh({
                 borderRadius: "2px",
                 padding: "12px 20px"
             }, r),
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             direction: "vertical",
             "data-dash-is-loading": w && w.is_loading || void 0
         }, b.slice(0, b.length - 1).map(function(t, n) {
-            return F.a.createElement(za.b, {
+            return H.a.createElement(za.b, {
                 style: {
                     display: "flex"
                 },
                 size: "small"
-            }, "left" === x ? F.a.createElement("div", {
+            }, "left" === x ? H.a.createElement("div", {
                 style: oh({
                     height: sh.get(o),
                     backgroundColor: v[n],
                     width: sh.get(o)
                 }, _)
-            }) : null, g ? F.a.createElement(F.a.Fragment, null, F.a.createElement(ch, {
+            }) : null, g ? H.a.createElement(H.a.Fragment, null, H.a.createElement(ch, {
                 style: O
-            }, b[n].toFixed(h)), F.a.createElement(ch, {
+            }, b[n].toFixed(h)), H.a.createElement(ch, {
                 style: O
-            }, "~"), F.a.createElement(ch, {
+            }, "~"), H.a.createElement(ch, {
                 style: O
-            }, b[n + 1].toFixed(h))) : F.a.createElement(F.a.Fragment, null, F.a.createElement(Ql.a, {
+            }, b[n + 1].toFixed(h))) : H.a.createElement(H.a.Fragment, null, H.a.createElement(Ql.a, {
                 style: y,
                 size: o,
                 bordered: i,
                 controls: l,
                 disabled: c,
                 keyboard: s,
                 placeholder: u,
@@ -124702,20 +124727,20 @@
                 value: b[n],
                 onChange: function(t) {
                     var e;
                     null !== t && 0 === n && t < b[n + 1] ? ((e = nh(b))[n] = t, k({
                         breakpoints: e
                     })) : null !== t && 0 < n && t > b[n - 1] && t < b[n + 1] ? ((e = nh(b))[n] = t, k({
                         breakpoints: e
-                    })) : null !== t && X.b.warning({
+                    })) : null !== t && $.b.warning({
                         content: "数值超出相邻断点，请调整后再输入！",
                         duration: 1.5
                     })
                 }
-            }), F.a.createElement("span", null, "~"), F.a.createElement(Ql.a, {
+            }), H.a.createElement("span", null, "~"), H.a.createElement(Ql.a, {
                 style: y,
                 size: o,
                 bordered: i,
                 controls: l,
                 disabled: c,
                 keyboard: s,
                 placeholder: u,
@@ -124727,20 +124752,20 @@
                 value: b[n + 1],
                 onChange: function(t) {
                     var e;
                     null !== t && n === b.length - 2 && t > b[n] ? ((e = nh(b))[n + 1] = t, k({
                         breakpoints: e
                     })) : null !== t && t > b[n] && t < b[n + 2] ? ((e = nh(b))[n + 1] = t, k({
                         breakpoints: e
-                    })) : null !== t && X.b.warning({
+                    })) : null !== t && $.b.warning({
                         content: "数值超出相邻断点，请调整后再输入！",
                         duration: 1.5
                     })
                 }
-            })), "right" === x ? F.a.createElement("div", {
+            })), "right" === x ? H.a.createElement("div", {
                 style: oh({
                     height: sh.get(o),
                     backgroundColor: v[n],
                     width: sh.get(o)
                 }, _)
             }) : null)
         }))
@@ -124752,21 +124777,21 @@
             a = t.style,
             r = t.key,
             o = t.locale,
             i = t.text,
             l = t.beforeIcon,
             c = t.afterIcon,
             t = (t.setProps, t.loading_state),
-            s = Object(Wt.useContext)(U.a),
+            s = Object(Wt.useContext)(G.a),
             o = s && s.locale || o;
-        return F.a.createElement(H.a, {
-            locale: V.b.get(o)
-        }, F.a.createElement(dh, {
+        return H.a.createElement(W.a, {
+            locale: K.b.get(o)
+        }, H.a.createElement(dh, {
             id: e,
-            className: Object(W.isString)(n) ? n : n ? Object(K.a)(n) : void 0,
+            className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             copyable: {
                 text: i,
                 icon: [l, c]
             },
             "data-dash-is-loading": t && t.is_loading || void 0
@@ -124906,57 +124931,57 @@
                 left: 0,
                 top: 0,
                 bottom: 0,
                 right: 0
             }), 2))[0],
             x = g[1],
             _ = Object(Wt.useRef)(null);
-        return F.a.createElement(dr, {
+        return H.a.createElement(dr, {
             id: e,
-            className: Object(W.isString)(a) ? a : a ? Object(K.a)(a) : void 0,
+            className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: o,
             key: r,
-            title: F.a.createElement("div", {
+            title: H.a.createElement("div", {
                 style: {
                     width: "100%",
                     cursor: p ? "move" : "inherit"
                 },
                 onMouseOver: function() {
                     b && v(!1)
                 },
                 onMouseOut: function() {
                     v(!0)
                 }
-            }, l, u ? "outlined" === d ? F.a.createElement(Ya.a, {
+            }, l, u ? "outlined" === d ? H.a.createElement(Ya.a, {
                 style: {
                     position: "absolute",
                     top: -12,
                     right: -12,
                     fontSize: 24,
                     cursor: "pointer"
                 },
                 onClick: function() {
                     return m({
                         visible: !1
                     })
                 }
-            }) : "two-tone" == d ? F.a.createElement(fh.a, {
+            }) : "two-tone" == d ? H.a.createElement(fh.a, {
                 style: {
                     position: "absolute",
                     top: -12,
                     right: -12,
                     fontSize: 24,
                     cursor: "pointer"
                 },
                 onClick: function() {
                     return m({
                         visible: !1
                     })
                 }
-            }) : F.a.createElement(dn.a, {
+            }) : H.a.createElement(dn.a, {
                 style: {
                     position: "absolute",
                     top: -12,
                     right: -12,
                     fontSize: 24,
                     cursor: "pointer"
                 },
@@ -124973,27 +124998,27 @@
             bodyStyle: h,
             mask: !1,
             maskClosable: !1,
             closable: !1,
             footer: !1,
             wrapClassName: "ant-modal-wrap-overwrite",
             modalRender: p ? function(t) {
-                return F.a.createElement(mh.a, {
+                return H.a.createElement(mh.a, {
                     disabled: b,
                     bounds: y,
                     onStart: function(t, e) {
                         var n, a, r;
                         e = e, n = window.document.documentElement, a = n.clientWidth, n = n.clientHeight, (r = _.current.getBoundingClientRect()) && x({
                             left: -r.left + e.x,
                             right: a - (r.right - e.x),
                             top: -r.top + e.y,
                             bottom: n - (r.bottom - e.y)
                         })
                     }
-                }, F.a.createElement("div", {
+                }, H.a.createElement("div", {
                     ref: _
                 }, t))
             } : void 0,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
@@ -125003,26 +125028,26 @@
             a = t.key,
             r = t.primaryColor,
             o = t.componentDisabled,
             i = t.componentSize,
             l = t.locale,
             t = (t.setProps, t.loading_state);
         return Object(Wt.useEffect)(function() {
-            H.a.config({
+            W.a.config({
                 theme: {
                     primaryColor: r
                 }
             })
-        }, [r]), F.a.createElement(U.a.Provider, {
+        }, [r]), H.a.createElement(G.a.Provider, {
             value: {
                 locale: l,
                 componentDisabled: o,
                 componentSize: i
             }
-        }, F.a.createElement(H.a, {
+        }, H.a.createElement(W.a, {
             id: e,
             key: a,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n))
     }
     vh.propTypes = {
         id: n.a.string,
@@ -125193,43 +125218,43 @@
                             })
                         })
                     })).observe(e),
                     function() {
                         t.disconnect()
                     }
             }, [], n), e);
-        return F.a.createElement("div", {
+        return H.a.createElement("div", {
             id: r,
             key: c,
-            className: Object(W.isString)(i) ? i : i ? Object(K.a)(i) : void 0,
+            className: Object(V.isString)(i) ? i : i ? Object(U.a)(i) : void 0,
             style: l,
             "data-dash-is-loading": v && v.is_loading || void 0
-        }, F.a.createElement("div", {
-            className: Object(W.isString)(u) ? u : u ? Object(K.a)(u) : void 0,
+        }, H.a.createElement("div", {
+            className: Object(V.isString)(u) ? u : u ? Object(U.a)(u) : void 0,
             style: Dh(Dh({
                 transitionTimingFunction: "ease"
             }, d), {}, {
                 maxHeight: m ? x && x.height : g,
                 transitionDuration: "".concat(b, "s"),
                 transitionProperty: "max-height",
                 overflow: "hidden"
             })
-        }, F.a.createElement("div", {
+        }, H.a.createElement("div", {
             ref: t
-        }, o)), F.a.createElement("div", {
+        }, o)), H.a.createElement("div", {
             style: {
                 textAlign: h
             }
-        }, F.a.createElement(zh, {
+        }, H.a.createElement(zh, {
             onClick: function() {
                 y({
                     open: !m
                 })
             }
-        }, m ? p || V.a.AntdSpoiler[s].hideLabel : f || V.a.AntdSpoiler[s].showLabel)))
+        }, m ? p || K.a.AntdSpoiler[s].hideLabel : f || K.a.AntdSpoiler[s].showLabel)))
     }
     var zh = u.a.Link,
         Ah = (Th.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
@@ -125345,15 +125370,15 @@
     }), e.d(t, "AntdCascader", function() {
         return xl
     }), e.d(t, "AntdRadioGroup", function() {
         return Ol
     }), e.d(t, "AntdUpload", function() {
         return Wf
     }), e.d(t, "AntdIcon", function() {
-        return R.a
+        return I.a
     }), e.d(t, "AntdPopconfirm", function() {
         return kl
     }), e.d(t, "AntdBackTop", function() {
         return Cl
     }), e.d(t, "AntdSkeleton", function() {
         return Nl
     }), e.d(t, "AntdAffix", function() {
```

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/metadata.json` & `feffery_antd_components-0.2.3/feffery_antd_components/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999395955492285%*

 * *Differences: {"'src/lib/components/AntdAccordion.react.js'": "{'props': {'items': {'type': {'value': {'value': "*

 * *                                                "{'collapsible': {'value': {insert: [(2, "*

 * *                                                'OrderedDict([(\'value\', "\'icon\'"), '*

 * *                                                "('computed', False)]))]}}}}}}, 'collapsible': "*

 * *                                                "{'type': {'value': {insert: [(2, "*

 * *                                                'Or […]*

```diff
@@ -84,14 +84,18 @@
                         {
                             "computed": false,
                             "value": "'header'"
                         },
                         {
                             "computed": false,
                             "value": "'disabled'"
+                        },
+                        {
+                            "computed": false,
+                            "value": "'icon'"
                         }
                     ]
                 }
             },
             "defaultActiveKey": {
                 "description": "",
                 "required": false,
@@ -189,14 +193,18 @@
                                     {
                                         "computed": false,
                                         "value": "'header'"
                                     },
                                     {
                                         "computed": false,
                                         "value": "'disabled'"
+                                    },
+                                    {
+                                        "computed": false,
+                                        "value": "'icon'"
                                     }
                                 ]
                             },
                             "extra": {
                                 "name": "node",
                                 "required": false
                             },
@@ -3177,14 +3185,18 @@
                         {
                             "computed": false,
                             "value": "'header'"
                         },
                         {
                             "computed": false,
                             "value": "'disabled'"
+                        },
+                        {
+                            "computed": false,
+                            "value": "'icon'"
                         }
                     ]
                 }
             },
             "forceRender": {
                 "defaultValue": {
                     "computed": false,
@@ -5463,14 +5475,25 @@
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
+            "autoAdjustOverflow": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "true"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            },
             "buttonMode": {
                 "defaultValue": {
                     "computed": false,
                     "value": "false"
                 },
                 "description": "",
                 "required": false,
@@ -15104,14 +15127,25 @@
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "number"
                 }
             },
+            "nDoubleClicksCell": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "0"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
             "pagination": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "union",
                     "value": [
                         {
@@ -15244,14 +15278,28 @@
             "recentlyCellClickRecord": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "object"
                 }
             },
+            "recentlyCellDoubleClickColumn": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "recentlyCellDoubleClickRecord": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            },
             "recentlyChangedRow": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "object"
                 }
             },
@@ -23140,14 +23188,18 @@
                                     },
                                     {
                                         "computed": false,
                                         "value": "'removed'"
                                     }
                                 ]
                             },
+                            "taskId": {
+                                "name": "string",
+                                "required": false
+                            },
                             "uid": {
                                 "name": "any",
                                 "required": false
                             },
                             "url": {
                                 "name": "string",
                                 "required": false
@@ -23689,14 +23741,18 @@
                                     },
                                     {
                                         "computed": false,
                                         "value": "'removed'"
                                     }
                                 ]
                             },
+                            "taskId": {
+                                "name": "string",
+                                "required": false
+                            },
                             "uid": {
                                 "name": "any",
                                 "required": false
                             },
                             "url": {
                                 "name": "string",
                                 "required": false
@@ -24235,14 +24291,18 @@
                                     },
                                     {
                                         "computed": false,
                                         "value": "'removed'"
                                     }
                                 ]
                             },
+                            "taskId": {
+                                "name": "string",
+                                "required": false
+                            },
                             "uid": {
                                 "name": "any",
                                 "required": false
                             },
                             "url": {
                                 "name": "string",
                                 "required": false
```

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components/package-info.json` & `feffery_antd_components-0.2.3/feffery_antd_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.2.3'"}*

```diff
@@ -84,9 +84,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_antd_components -p package-info.json --r-prefix 'feffery' --jl-prefix 'feffery'",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.2"
+    "version": "0.2.3"
 }
```

### Comparing `feffery_antd_components-0.2.2/feffery_antd_components.egg-info/SOURCES.txt` & `feffery_antd_components-0.2.3/feffery_antd_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.2/package.json` & `feffery_antd_components-0.2.3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.2.3'"}*

```diff
@@ -84,9 +84,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_antd_components -p package-info.json --r-prefix 'feffery' --jl-prefix 'feffery'",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.2"
+    "version": "0.2.3"
 }
```

### Comparing `feffery_antd_components-0.2.2/setup.py` & `feffery_antd_components-0.2.3/setup.py`

 * *Files identical despite different names*

