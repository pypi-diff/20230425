# Comparing `tmp/feffery_antd_components-0.2.3.tar.gz` & `tmp/feffery_antd_components-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feffery_antd_components-0.2.3.tar", last modified: Tue Apr 25 07:16:07 2023, max compression
+gzip compressed data, was "feffery_antd_components-0.2.5.tar", last modified: Tue Apr 25 08:45:38 2023, max compression
```

## Comparing `feffery_antd_components-0.2.3.tar` & `feffery_antd_components-0.2.5.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 07:16:07.108703 feffery_antd_components-0.2.3/
--rw-rw-rw-   0        0        0     1087 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      288 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0      346 2023-04-25 07:16:07.107653 feffery_antd_components-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2301 2023-04-25 07:15:50.000000 feffery_antd_components-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 07:16:07.101633 feffery_antd_components-0.2.3/feffery_antd_components/
--rw-rw-rw-   0        0        0     3328 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdAccordion.py
--rw-rw-rw-   0        0        0     2539 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdAccordionItem.py
--rw-rw-rw-   0        0        0     2006 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdAffix.py
--rw-rw-rw-   0        0        0     2627 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdAlert.py
--rw-rw-rw-   0        0        0     2314 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdAnchor.py
--rw-rw-rw-   0        0        0     2586 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdAvatar.py
--rw-rw-rw-   0        0        0     2611 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdAvatarGroup.py
--rw-rw-rw-   0        0        0     1892 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdBackTop.py
--rw-rw-rw-   0        0        0     2730 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdBadge.py
--rw-rw-rw-   0        0        0     2313 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdBreadcrumb.py
--rw-rw-rw-   0        0        0     3218 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdButton.py
--rw-rw-rw-   0        0        0     3356 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCalendar.py
--rw-rw-rw-   0        0        0     2991 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCard.py
--rw-rw-rw-   0        0        0     1924 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCardGrid.py
--rw-rw-rw-   0        0        0     2490 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCarousel.py
--rw-rw-rw-   0        0        0     5312 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCascader.py
--rw-rw-rw-   0        0        0     3615 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCheckCard.py
--rw-rw-rw-   0        0        0     3694 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCheckCardGroup.py
--rw-rw-rw-   0        0        0     3303 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCheckbox.py
--rw-rw-rw-   0        0        0     3388 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCheckboxGroup.py
--rw-rw-rw-   0        0        0     3890 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCol.py
--rw-rw-rw-   0        0        0     3763 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCollapse.py
--rw-rw-rw-   0        0        0     3987 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdComment.py
--rw-rw-rw-   0        0        0     2076 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdConfigProvider.py
--rw-rw-rw-   0        0        0     1824 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdContent.py
--rw-rw-rw-   0        0        0     2109 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCopyText.py
--rw-rw-rw-   0        0        0     2497 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCountdown.py
--rw-rw-rw-   0        0        0     2530 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdCustomSkeleton.py
--rw-rw-rw-   0        0        0     5353 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdDatePicker.py
--rw-rw-rw-   0        0        0     5418 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdDateRangePicker.py
--rw-rw-rw-   0        0        0     2263 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdDescriptionItem.py
--rw-rw-rw-   0        0        0     2745 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdDescriptions.py
--rw-rw-rw-   0        0        0     2676 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdDivider.py
--rw-rw-rw-   0        0        0     6274 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdDraggerUpload.py
--rw-rw-rw-   0        0        0     3109 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdDrawer.py
--rw-rw-rw-   0        0        0     3744 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdDropdown.py
--rw-rw-rw-   0        0        0     2250 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdEmpty.py
--rw-rw-rw-   0        0        0     1820 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdFooter.py
--rw-rw-rw-   0        0        0     2552 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdForm.py
--rw-rw-rw-   0        0        0     3351 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdFormItem.py
--rw-rw-rw-   0        0        0     1820 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdHeader.py
--rw-rw-rw-   0        0        0     1829 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdIcon.py
--rw-rw-rw-   0        0        0     5562 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdImage.py
--rw-rw-rw-   0        0        0     5674 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdInput.py
--rw-rw-rw-   0        0        0     5082 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdInputNumber.py
--rw-rw-rw-   0        0        0     1820 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdLayout.py
--rw-rw-rw-   0        0        0     3094 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdMentions.py
--rw-rw-rw-   0        0        0     4059 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdMenu.py
--rw-rw-rw-   0        0        0     2110 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdMessage.py
--rw-rw-rw-   0        0        0     5365 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdModal.py
--rw-rw-rw-   0        0        0     2417 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdNotification.py
--rw-rw-rw-   0        0        0     2555 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdPageHeader.py
--rw-rw-rw-   0        0        0     4592 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdPagination.py
--rw-rw-rw-   0        0        0     2752 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdParagraph.py
--rw-rw-rw-   0        0        0     2002 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdPasteImage.py
--rw-rw-rw-   0        0        0     6381 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdPictureUpload.py
--rw-rw-rw-   0        0        0     4807 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdPopconfirm.py
--rw-rw-rw-   0        0        0     3562 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdPopover.py
--rw-rw-rw-   0        0        0     2869 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdPopupCard.py
--rw-rw-rw-   0        0        0     3352 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdProgress.py
--rw-rw-rw-   0        0        0     4008 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdRadioGroup.py
--rw-rw-rw-   0        0        0     3488 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdRate.py
--rw-rw-rw-   0        0        0     2181 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdResult.py
--rw-rw-rw-   0        0        0     2068 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdRibbon.py
--rw-rw-rw-   0        0        0     2489 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdRow.py
--rw-rw-rw-   0        0        0     3715 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSegmented.py
--rw-rw-rw-   0        0        0     3598 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSegmentedColoring.py
--rw-rw-rw-   0        0        0     7197 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSelect.py
--rw-rw-rw-   0        0        0     2846 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSider.py
--rw-rw-rw-   0        0        0     3193 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeleton.py
--rw-rw-rw-   0        0        0     1934 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeletonAvatar.py
--rw-rw-rw-   0        0        0     2017 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeletonButton.py
--rw-rw-rw-   0        0        0     1604 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeletonImage.py
--rw-rw-rw-   0        0        0     1808 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeletonInput.py
--rw-rw-rw-   0        0        0     4230 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSlider.py
--rw-rw-rw-   0        0        0     2389 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSpace.py
--rw-rw-rw-   0        0        0     2931 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSpin.py
--rw-rw-rw-   0        0        0     2853 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSpoiler.py
--rw-rw-rw-   0        0        0     2607 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdStatistic.py
--rw-rw-rw-   0        0        0     3223 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSteps.py
--rw-rw-rw-   0        0        0     3651 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdSwitch.py
--rw-rw-rw-   0        0        0     2314 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTabPane.py
--rw-rw-rw-   0        0        0    19271 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTable.py
--rw-rw-rw-   0        0        0     5266 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTabs.py
--rw-rw-rw-   0        0        0     1950 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTag.py
--rw-rw-rw-   0        0        0     2820 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdText.py
--rw-rw-rw-   0        0        0     4722 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTimePicker.py
--rw-rw-rw-   0        0        0     4787 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTimeRangePicker.py
--rw-rw-rw-   0        0        0     2750 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTimeline.py
--rw-rw-rw-   0        0        0     2900 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTitle.py
--rw-rw-rw-   0        0        0     3445 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTooltip.py
--rw-rw-rw-   0        0        0     4586 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTransfer.py
--rw-rw-rw-   0        0        0     5301 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTree.py
--rw-rw-rw-   0        0        0     6685 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdTreeSelect.py
--rw-rw-rw-   0        0        0     5669 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdUpload.py
--rw-rw-rw-   0        0        0     2397 2023-04-25 07:16:05.000000 feffery_antd_components-0.2.3/feffery_antd_components/AntdWatermark.py
--rw-rw-rw-   0        0        0     1571 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.3/feffery_antd_components/__init__.py
--rw-rw-rw-   0        0        0     5752 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/_imports_.py
--rw-rw-rw-   0        0        0  3771264 2023-04-25 07:16:00.000000 feffery_antd_components-0.2.3/feffery_antd_components/feffery_antd_components.min.js
--rw-rw-rw-   0        0        0   624550 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components/metadata.json
--rw-rw-rw-   0        0        0     3031 2023-04-25 07:16:01.000000 feffery_antd_components-0.2.3/feffery_antd_components/package-info.json
-drwxrwxrwx   0        0        0        0 2023-04-25 07:16:07.106392 feffery_antd_components-0.2.3/feffery_antd_components.egg-info/
--rw-rw-rw-   0        0        0      346 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4341 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-25 07:16:06.000000 feffery_antd_components-0.2.3/feffery_antd_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3031 2023-04-24 06:18:25.000000 feffery_antd_components-0.2.3/package.json
--rw-rw-rw-   0        0        0       42 2023-04-25 07:16:07.108703 feffery_antd_components-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      715 2023-04-25 07:15:34.000000 feffery_antd_components-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:45:38.104397 feffery_antd_components-0.2.5/
+-rw-rw-rw-   0        0        0     1087 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      288 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      346 2023-04-25 08:45:38.104397 feffery_antd_components-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2301 2023-04-25 07:15:50.000000 feffery_antd_components-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 08:45:38.097055 feffery_antd_components-0.2.5/feffery_antd_components/
+-rw-rw-rw-   0        0        0     3328 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdAccordion.py
+-rw-rw-rw-   0        0        0     2539 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdAccordionItem.py
+-rw-rw-rw-   0        0        0     2006 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdAffix.py
+-rw-rw-rw-   0        0        0     2627 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdAlert.py
+-rw-rw-rw-   0        0        0     2314 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdAnchor.py
+-rw-rw-rw-   0        0        0     2586 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdAvatar.py
+-rw-rw-rw-   0        0        0     2611 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdAvatarGroup.py
+-rw-rw-rw-   0        0        0     1892 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdBackTop.py
+-rw-rw-rw-   0        0        0     2730 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdBadge.py
+-rw-rw-rw-   0        0        0     2313 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdBreadcrumb.py
+-rw-rw-rw-   0        0        0     3218 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdButton.py
+-rw-rw-rw-   0        0        0     3356 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCalendar.py
+-rw-rw-rw-   0        0        0     2991 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCard.py
+-rw-rw-rw-   0        0        0     1924 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCardGrid.py
+-rw-rw-rw-   0        0        0     2490 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCarousel.py
+-rw-rw-rw-   0        0        0     5312 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCascader.py
+-rw-rw-rw-   0        0        0     3615 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCheckCard.py
+-rw-rw-rw-   0        0        0     3694 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCheckCardGroup.py
+-rw-rw-rw-   0        0        0     3303 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCheckbox.py
+-rw-rw-rw-   0        0        0     3388 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCheckboxGroup.py
+-rw-rw-rw-   0        0        0     3890 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCol.py
+-rw-rw-rw-   0        0        0     3763 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCollapse.py
+-rw-rw-rw-   0        0        0     3987 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdComment.py
+-rw-rw-rw-   0        0        0     2076 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdConfigProvider.py
+-rw-rw-rw-   0        0        0     1824 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdContent.py
+-rw-rw-rw-   0        0        0     2109 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCopyText.py
+-rw-rw-rw-   0        0        0     2497 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCountdown.py
+-rw-rw-rw-   0        0        0     2530 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCustomSkeleton.py
+-rw-rw-rw-   0        0        0     5353 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdDatePicker.py
+-rw-rw-rw-   0        0        0     5418 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdDateRangePicker.py
+-rw-rw-rw-   0        0        0     2263 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdDescriptionItem.py
+-rw-rw-rw-   0        0        0     2745 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdDescriptions.py
+-rw-rw-rw-   0        0        0     2676 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdDivider.py
+-rw-rw-rw-   0        0        0     6274 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdDraggerUpload.py
+-rw-rw-rw-   0        0        0     3109 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdDrawer.py
+-rw-rw-rw-   0        0        0     3744 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdDropdown.py
+-rw-rw-rw-   0        0        0     2250 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdEmpty.py
+-rw-rw-rw-   0        0        0     1820 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdFooter.py
+-rw-rw-rw-   0        0        0     2552 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdForm.py
+-rw-rw-rw-   0        0        0     3351 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdFormItem.py
+-rw-rw-rw-   0        0        0     1820 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdHeader.py
+-rw-rw-rw-   0        0        0     1829 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdIcon.py
+-rw-rw-rw-   0        0        0     5562 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdImage.py
+-rw-rw-rw-   0        0        0     5674 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdInput.py
+-rw-rw-rw-   0        0        0     5082 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdInputNumber.py
+-rw-rw-rw-   0        0        0     1820 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdLayout.py
+-rw-rw-rw-   0        0        0     3094 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdMentions.py
+-rw-rw-rw-   0        0        0     4059 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdMenu.py
+-rw-rw-rw-   0        0        0     2110 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdMessage.py
+-rw-rw-rw-   0        0        0     5365 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdModal.py
+-rw-rw-rw-   0        0        0     2417 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdNotification.py
+-rw-rw-rw-   0        0        0     2555 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdPageHeader.py
+-rw-rw-rw-   0        0        0     4592 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdPagination.py
+-rw-rw-rw-   0        0        0     2752 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdParagraph.py
+-rw-rw-rw-   0        0        0     2002 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdPasteImage.py
+-rw-rw-rw-   0        0        0     6381 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdPictureUpload.py
+-rw-rw-rw-   0        0        0     4807 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdPopconfirm.py
+-rw-rw-rw-   0        0        0     3562 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdPopover.py
+-rw-rw-rw-   0        0        0     2869 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdPopupCard.py
+-rw-rw-rw-   0        0        0     3352 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdProgress.py
+-rw-rw-rw-   0        0        0     4008 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdRadioGroup.py
+-rw-rw-rw-   0        0        0     3488 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdRate.py
+-rw-rw-rw-   0        0        0     2181 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdResult.py
+-rw-rw-rw-   0        0        0     2068 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdRibbon.py
+-rw-rw-rw-   0        0        0     2489 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdRow.py
+-rw-rw-rw-   0        0        0     3715 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSegmented.py
+-rw-rw-rw-   0        0        0     3598 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSegmentedColoring.py
+-rw-rw-rw-   0        0        0     7197 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSelect.py
+-rw-rw-rw-   0        0        0     2846 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSider.py
+-rw-rw-rw-   0        0        0     3193 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeleton.py
+-rw-rw-rw-   0        0        0     1934 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeletonAvatar.py
+-rw-rw-rw-   0        0        0     2017 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeletonButton.py
+-rw-rw-rw-   0        0        0     1604 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeletonImage.py
+-rw-rw-rw-   0        0        0     1808 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeletonInput.py
+-rw-rw-rw-   0        0        0     4230 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSlider.py
+-rw-rw-rw-   0        0        0     2389 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSpace.py
+-rw-rw-rw-   0        0        0     2931 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSpin.py
+-rw-rw-rw-   0        0        0     2853 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSpoiler.py
+-rw-rw-rw-   0        0        0     2607 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdStatistic.py
+-rw-rw-rw-   0        0        0     3223 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSteps.py
+-rw-rw-rw-   0        0        0     3651 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSwitch.py
+-rw-rw-rw-   0        0        0     2314 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTabPane.py
+-rw-rw-rw-   0        0        0    19271 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTable.py
+-rw-rw-rw-   0        0        0     5266 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTabs.py
+-rw-rw-rw-   0        0        0     1950 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTag.py
+-rw-rw-rw-   0        0        0     2820 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdText.py
+-rw-rw-rw-   0        0        0     4722 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTimePicker.py
+-rw-rw-rw-   0        0        0     4787 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTimeRangePicker.py
+-rw-rw-rw-   0        0        0     2750 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTimeline.py
+-rw-rw-rw-   0        0        0     2900 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTitle.py
+-rw-rw-rw-   0        0        0     3445 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTooltip.py
+-rw-rw-rw-   0        0        0     4586 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTransfer.py
+-rw-rw-rw-   0        0        0     5301 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTree.py
+-rw-rw-rw-   0        0        0     6685 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTreeSelect.py
+-rw-rw-rw-   0        0        0     5669 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdUpload.py
+-rw-rw-rw-   0        0        0     2397 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdWatermark.py
+-rw-rw-rw-   0        0        0     1571 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.5/feffery_antd_components/__init__.py
+-rw-rw-rw-   0        0        0     5752 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components/_imports_.py
+-rw-rw-rw-   0        0        0  3771264 2023-04-25 08:45:31.000000 feffery_antd_components-0.2.5/feffery_antd_components/feffery_antd_components.min.js
+-rw-rw-rw-   0        0        0   624550 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components/metadata.json
+-rw-rw-rw-   0        0        0     3031 2023-04-25 08:45:32.000000 feffery_antd_components-0.2.5/feffery_antd_components/package-info.json
+drwxrwxrwx   0        0        0        0 2023-04-25 08:45:38.102376 feffery_antd_components-0.2.5/feffery_antd_components.egg-info/
+-rw-rw-rw-   0        0        0      346 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4341 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3031 2023-04-25 08:45:01.000000 feffery_antd_components-0.2.5/package.json
+-rw-rw-rw-   0        0        0       42 2023-04-25 08:45:38.105395 feffery_antd_components-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      715 2023-04-25 07:15:34.000000 feffery_antd_components-0.2.5/setup.py
```

### Comparing `feffery_antd_components-0.2.3/LICENSE` & `feffery_antd_components-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/README.md` & `feffery_antd_components-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdAccordion.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdAccordion.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdAccordionItem.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdAccordionItem.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdAffix.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdAffix.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdAlert.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdAlert.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdAnchor.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdAnchor.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdAvatar.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdAvatar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdAvatarGroup.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdAvatarGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdBackTop.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdBackTop.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdBadge.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdBadge.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdBreadcrumb.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdBreadcrumb.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdButton.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdButton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdCalendar.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdCalendar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdCard.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdCard.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdCardGrid.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdCardGrid.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdCarousel.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdCarousel.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdCascader.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdCascader.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdCheckCard.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdCheckCard.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdCheckCardGroup.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdCheckCardGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdCheckbox.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdCheckbox.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdCheckboxGroup.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdCheckboxGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdCol.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdCol.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdCollapse.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdCollapse.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdComment.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdComment.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdConfigProvider.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdConfigProvider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdContent.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdContent.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdCopyText.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdCopyText.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdCountdown.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdCountdown.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdCustomSkeleton.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdCustomSkeleton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdDatePicker.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdDatePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdDateRangePicker.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdDateRangePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdDescriptionItem.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdDescriptionItem.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdDescriptions.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdDescriptions.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdDivider.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdDivider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdDraggerUpload.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdDraggerUpload.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdDrawer.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdDrawer.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdDropdown.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdDropdown.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdEmpty.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdEmpty.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdFooter.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdFooter.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdForm.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdForm.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdFormItem.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdFormItem.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdHeader.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdHeader.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdIcon.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdIcon.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdImage.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdImage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdInput.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdInput.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdInputNumber.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdInputNumber.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdLayout.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdLayout.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdMentions.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdMentions.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdMenu.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdMenu.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdMessage.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdMessage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdModal.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdModal.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdNotification.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdNotification.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdPageHeader.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdPageHeader.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdPagination.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdPagination.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdParagraph.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdParagraph.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdPasteImage.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdPasteImage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdPictureUpload.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdPictureUpload.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdPopconfirm.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdPopconfirm.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdPopover.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdPopover.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdPopupCard.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdPopupCard.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdProgress.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdProgress.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdRadioGroup.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdRadioGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdRate.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdRate.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdResult.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdResult.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdRibbon.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdRibbon.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdRow.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdRow.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdSegmented.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdSegmented.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdSegmentedColoring.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdSegmentedColoring.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdSelect.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdSelect.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdSider.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdSider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeleton.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeleton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeletonAvatar.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeletonAvatar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeletonButton.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeletonButton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeletonImage.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeletonImage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdSkeletonInput.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeletonInput.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdSlider.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdSlider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdSpace.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdSpace.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdSpin.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdSpin.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdSpoiler.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdSpoiler.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdStatistic.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdStatistic.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdSteps.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdSteps.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdSwitch.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdSwitch.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdTabPane.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdTabPane.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdTable.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdTable.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdTabs.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdTabs.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdTag.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdTag.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdText.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdText.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdTimePicker.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdTimePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdTimeRangePicker.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdTimeRangePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdTimeline.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdTimeline.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdTitle.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdTitle.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdTooltip.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdTooltip.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdTransfer.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdTransfer.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdTree.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdTree.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdTreeSelect.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdTreeSelect.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdUpload.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdUpload.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/AntdWatermark.py` & `feffery_antd_components-0.2.5/feffery_antd_components/AntdWatermark.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/__init__.py` & `feffery_antd_components-0.2.5/feffery_antd_components/__init__.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/_imports_.py` & `feffery_antd_components-0.2.5/feffery_antd_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/feffery_antd_components.min.js` & `feffery_antd_components-0.2.5/feffery_antd_components/feffery_antd_components.min.js`

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
-        return n ? ((e = (n = t.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_3m1682406921"), n.splice(-1, 1, e.join(".")), n.join("/")) : t
+        return n ? ((e = (n = t.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_5m1682412291"), n.splice(-1, 1, e.join(".")), n.join("/")) : t
     }), r(r.s = 688)
 }([function(t, e) {
     t.exports = window.React
 }, function(t, e) {
     t.exports = window.PropTypes
 }, function(R, t, e) {
     "use strict";
```

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/metadata.json` & `feffery_antd_components-0.2.5/feffery_antd_components/metadata.json`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components/package-info.json` & `feffery_antd_components-0.2.5/feffery_antd_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.2.5'"}*

```diff
@@ -84,9 +84,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_antd_components -p package-info.json --r-prefix 'feffery' --jl-prefix 'feffery'",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.3"
+    "version": "0.2.5"
 }
```

### Comparing `feffery_antd_components-0.2.3/feffery_antd_components.egg-info/SOURCES.txt` & `feffery_antd_components-0.2.5/feffery_antd_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.3/package.json` & `feffery_antd_components-0.2.5/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.2.5'"}*

```diff
@@ -84,9 +84,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_antd_components -p package-info.json --r-prefix 'feffery' --jl-prefix 'feffery'",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.3"
+    "version": "0.2.5"
 }
```

### Comparing `feffery_antd_components-0.2.3/setup.py` & `feffery_antd_components-0.2.5/setup.py`

 * *Files identical despite different names*

