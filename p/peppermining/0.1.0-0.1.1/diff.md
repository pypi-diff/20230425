# Comparing `tmp/peppermining-0.1.0.tar.gz` & `tmp/peppermining-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peppermining-0.1.0.tar", last modified: Tue Apr 18 09:00:40 2023, max compression
+gzip compressed data, was "peppermining-0.1.1.tar", last modified: Tue Apr 25 06:56:17 2023, max compression
```

## Comparing `peppermining-0.1.0.tar` & `peppermining-0.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 09:00:40.132352 peppermining-0.1.0/
--rw-rw-rw-   0        0        0     1079 2023-02-03 08:26:19.000000 peppermining-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      816 2023-04-18 09:00:40.130350 peppermining-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       72 2023-02-03 08:25:19.000000 peppermining-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 09:00:39.887359 peppermining-0.1.0/peppermining/
--rw-rw-rw-   0        0        0      341 2023-04-18 07:21:19.000000 peppermining-0.1.0/peppermining/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:00:39.955400 peppermining-0.1.0/peppermining/conformance/
--rw-rw-rw-   0        0        0      341 2023-04-17 14:28:27.000000 peppermining-0.1.0/peppermining/conformance/__init__.py
--rw-rw-rw-   0        0        0     5714 2023-04-18 07:11:06.000000 peppermining-0.1.0/peppermining/conformance/conformance.py
--rw-rw-rw-   0        0        0     5196 2023-04-18 07:02:57.000000 peppermining-0.1.0/peppermining/conformance/process_model.py
--rw-rw-rw-   0        0        0     1915 2023-04-18 07:02:51.000000 peppermining-0.1.0/peppermining/conformance/root_cause_analysis.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:00:40.006353 peppermining-0.1.0/peppermining/conformance/violation/
--rw-rw-rw-   0        0        0      647 2023-04-17 14:31:09.000000 peppermining-0.1.0/peppermining/conformance/violation/__init__.py
--rw-rw-rw-   0        0        0     5627 2023-04-18 07:06:10.000000 peppermining-0.1.0/peppermining/conformance/violation/pepper_violation.py
--rw-rw-rw-   0        0        0     3430 2023-04-18 07:06:37.000000 peppermining-0.1.0/peppermining/conformance/violation/run_by_same_user.py
--rw-rw-rw-   0        0        0     2218 2023-04-18 07:06:44.000000 peppermining-0.1.0/peppermining/conformance/violation/undesired_activity.py
--rw-rw-rw-   0        0        0     3427 2023-04-18 07:06:51.000000 peppermining-0.1.0/peppermining/conformance/violation/undesired_connection.py
--rw-rw-rw-   0        0        0     2684 2023-04-18 07:06:58.000000 peppermining-0.1.0/peppermining/conformance/violation/undesired_end.py
--rw-rw-rw-   0        0        0     2700 2023-04-18 07:05:05.000000 peppermining-0.1.0/peppermining/conformance/violation/undesired_start.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:00:40.062353 peppermining-0.1.0/peppermining/filters/
--rw-rw-rw-   0        0        0      767 2023-04-18 07:07:46.000000 peppermining-0.1.0/peppermining/filters/__init__.py
--rw-rw-rw-   0        0        0     2162 2023-04-18 07:00:57.000000 peppermining-0.1.0/peppermining/filters/case_activity_filter.py
--rw-rw-rw-   0        0        0     2497 2023-04-18 07:01:11.000000 peppermining-0.1.0/peppermining/filters/case_between_time_filter.py
--rw-rw-rw-   0        0        0     2443 2023-04-18 07:01:23.000000 peppermining-0.1.0/peppermining/filters/case_end_activity_filter.py
--rw-rw-rw-   0        0        0     1914 2023-04-18 07:01:35.000000 peppermining-0.1.0/peppermining/filters/case_filter.py
--rw-rw-rw-   0        0        0     2325 2023-04-18 07:01:44.000000 peppermining-0.1.0/peppermining/filters/case_size_filter.py
--rw-rw-rw-   0        0        0     2446 2023-04-18 07:01:55.000000 peppermining-0.1.0/peppermining/filters/case_start_activity_filter.py
--rw-rw-rw-   0        0        0     4281 2023-04-18 07:00:08.000000 peppermining-0.1.0/peppermining/filters/pepper_filter.py
--rw-rw-rw-   0        0        0     2724 2023-04-18 06:59:27.000000 peppermining-0.1.0/peppermining/filters/variant_filter.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:00:40.113360 peppermining-0.1.0/peppermining/kpi/
--rw-rw-rw-   0        0        0      573 2023-04-18 06:58:51.000000 peppermining-0.1.0/peppermining/kpi/__init__.py
--rw-rw-rw-   0        0        0     1387 2023-04-18 06:56:33.000000 peppermining-0.1.0/peppermining/kpi/average_events_per_case.py
--rw-rw-rw-   0        0        0     2445 2023-04-18 06:57:43.000000 peppermining-0.1.0/peppermining/kpi/number_of_activities.py
--rw-rw-rw-   0        0        0     5790 2023-04-18 06:57:49.000000 peppermining-0.1.0/peppermining/kpi/number_of_cases.py
--rw-rw-rw-   0        0        0     4555 2023-04-18 06:57:55.000000 peppermining-0.1.0/peppermining/kpi/number_of_events.py
--rw-rw-rw-   0        0        0     4761 2023-04-18 06:57:31.000000 peppermining-0.1.0/peppermining/kpi/pepper_kpi.py
--rw-rw-rw-   0        0        0     2944 2023-04-18 06:58:01.000000 peppermining-0.1.0/peppermining/kpi/rework.py
--rw-rw-rw-   0        0        0     6905 2023-04-18 06:58:08.000000 peppermining-0.1.0/peppermining/kpi/throughput_time.py
--rw-rw-rw-   0        0        0      571 2023-04-14 07:56:01.000000 peppermining-0.1.0/peppermining/main.py
--rw-rw-rw-   0        0        0    17091 2023-04-18 07:05:34.000000 peppermining-0.1.0/peppermining/pepper.py
--rw-rw-rw-   0        0        0    11957 2023-04-18 07:19:14.000000 peppermining-0.1.0/peppermining/peppermining.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:00:40.127352 peppermining-0.1.0/peppermining/utils/
--rw-rw-rw-   0        0        0      149 2023-04-18 07:09:13.000000 peppermining-0.1.0/peppermining/utils/__init__.py
--rw-rw-rw-   0        0        0     1221 2023-04-12 06:39:57.000000 peppermining-0.1.0/peppermining/utils/enum.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:00:39.930355 peppermining-0.1.0/peppermining.egg-info/
--rw-rw-rw-   0        0        0      816 2023-04-18 09:00:39.000000 peppermining-0.1.0/peppermining.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1588 2023-04-18 09:00:39.000000 peppermining-0.1.0/peppermining.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 09:00:39.000000 peppermining-0.1.0/peppermining.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-18 09:00:39.000000 peppermining-0.1.0/peppermining.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-18 09:00:39.000000 peppermining-0.1.0/peppermining.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      669 2023-04-18 08:58:59.000000 peppermining-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 09:00:40.133354 peppermining-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1315 2023-04-18 08:21:49.000000 peppermining-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:56:17.091800 peppermining-0.1.1/
+-rw-rw-rw-   0        0        0     1079 2023-02-03 08:26:19.000000 peppermining-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      816 2023-04-25 06:56:17.079803 peppermining-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2023-02-03 08:25:19.000000 peppermining-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 06:56:15.383800 peppermining-0.1.1/peppermining/
+-rw-rw-rw-   0        0        0     1777 2023-04-25 06:46:58.000000 peppermining-0.1.1/peppermining/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:56:16.019824 peppermining-0.1.1/peppermining/conformance/
+-rw-rw-rw-   0        0        0      341 2023-04-17 14:28:27.000000 peppermining-0.1.1/peppermining/conformance/__init__.py
+-rw-rw-rw-   0        0        0     5714 2023-04-18 07:11:06.000000 peppermining-0.1.1/peppermining/conformance/conformance.py
+-rw-rw-rw-   0        0        0     5196 2023-04-18 07:02:57.000000 peppermining-0.1.1/peppermining/conformance/process_model.py
+-rw-rw-rw-   0        0        0     1915 2023-04-18 07:02:51.000000 peppermining-0.1.1/peppermining/conformance/root_cause_analysis.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:56:16.191799 peppermining-0.1.1/peppermining/conformance/violation/
+-rw-rw-rw-   0        0        0      647 2023-04-17 14:31:09.000000 peppermining-0.1.1/peppermining/conformance/violation/__init__.py
+-rw-rw-rw-   0        0        0     5627 2023-04-18 07:06:10.000000 peppermining-0.1.1/peppermining/conformance/violation/pepper_violation.py
+-rw-rw-rw-   0        0        0     3430 2023-04-18 07:06:37.000000 peppermining-0.1.1/peppermining/conformance/violation/run_by_same_user.py
+-rw-rw-rw-   0        0        0     2218 2023-04-18 07:06:44.000000 peppermining-0.1.1/peppermining/conformance/violation/undesired_activity.py
+-rw-rw-rw-   0        0        0     3427 2023-04-18 07:06:51.000000 peppermining-0.1.1/peppermining/conformance/violation/undesired_connection.py
+-rw-rw-rw-   0        0        0     2684 2023-04-18 07:06:58.000000 peppermining-0.1.1/peppermining/conformance/violation/undesired_end.py
+-rw-rw-rw-   0        0        0     2700 2023-04-18 07:05:05.000000 peppermining-0.1.1/peppermining/conformance/violation/undesired_start.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:56:16.714800 peppermining-0.1.1/peppermining/filters/
+-rw-rw-rw-   0        0        0      767 2023-04-18 07:07:46.000000 peppermining-0.1.1/peppermining/filters/__init__.py
+-rw-rw-rw-   0        0        0     2162 2023-04-18 07:00:57.000000 peppermining-0.1.1/peppermining/filters/case_activity_filter.py
+-rw-rw-rw-   0        0        0     2497 2023-04-18 07:01:11.000000 peppermining-0.1.1/peppermining/filters/case_between_time_filter.py
+-rw-rw-rw-   0        0        0     2443 2023-04-18 07:01:23.000000 peppermining-0.1.1/peppermining/filters/case_end_activity_filter.py
+-rw-rw-rw-   0        0        0     1914 2023-04-18 07:01:35.000000 peppermining-0.1.1/peppermining/filters/case_filter.py
+-rw-rw-rw-   0        0        0     2325 2023-04-18 07:01:44.000000 peppermining-0.1.1/peppermining/filters/case_size_filter.py
+-rw-rw-rw-   0        0        0     2446 2023-04-18 07:01:55.000000 peppermining-0.1.1/peppermining/filters/case_start_activity_filter.py
+-rw-rw-rw-   0        0        0     4281 2023-04-18 07:00:08.000000 peppermining-0.1.1/peppermining/filters/pepper_filter.py
+-rw-rw-rw-   0        0        0     2724 2023-04-18 06:59:27.000000 peppermining-0.1.1/peppermining/filters/variant_filter.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:56:16.997801 peppermining-0.1.1/peppermining/kpi/
+-rw-rw-rw-   0        0        0      573 2023-04-18 06:58:51.000000 peppermining-0.1.1/peppermining/kpi/__init__.py
+-rw-rw-rw-   0        0        0     1387 2023-04-18 06:56:33.000000 peppermining-0.1.1/peppermining/kpi/average_events_per_case.py
+-rw-rw-rw-   0        0        0     2445 2023-04-18 06:57:43.000000 peppermining-0.1.1/peppermining/kpi/number_of_activities.py
+-rw-rw-rw-   0        0        0     5790 2023-04-18 06:57:49.000000 peppermining-0.1.1/peppermining/kpi/number_of_cases.py
+-rw-rw-rw-   0        0        0     4555 2023-04-18 06:57:55.000000 peppermining-0.1.1/peppermining/kpi/number_of_events.py
+-rw-rw-rw-   0        0        0     4761 2023-04-18 06:57:31.000000 peppermining-0.1.1/peppermining/kpi/pepper_kpi.py
+-rw-rw-rw-   0        0        0     2944 2023-04-18 06:58:01.000000 peppermining-0.1.1/peppermining/kpi/rework.py
+-rw-rw-rw-   0        0        0     6905 2023-04-18 06:58:08.000000 peppermining-0.1.1/peppermining/kpi/throughput_time.py
+-rw-rw-rw-   0        0        0      571 2023-04-14 07:56:01.000000 peppermining-0.1.1/peppermining/main.py
+-rw-rw-rw-   0        0        0    17091 2023-04-18 07:05:34.000000 peppermining-0.1.1/peppermining/pepper.py
+-rw-rw-rw-   0        0        0    11956 2023-04-19 09:46:35.000000 peppermining-0.1.1/peppermining/peppermining.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:56:17.063807 peppermining-0.1.1/peppermining/utils/
+-rw-rw-rw-   0        0        0      149 2023-04-18 07:09:13.000000 peppermining-0.1.1/peppermining/utils/__init__.py
+-rw-rw-rw-   0        0        0     1221 2023-04-12 06:39:57.000000 peppermining-0.1.1/peppermining/utils/enum.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:56:15.717800 peppermining-0.1.1/peppermining.egg-info/
+-rw-rw-rw-   0        0        0      816 2023-04-25 06:56:13.000000 peppermining-0.1.1/peppermining.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1588 2023-04-25 06:56:13.000000 peppermining-0.1.1/peppermining.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 06:56:13.000000 peppermining-0.1.1/peppermining.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-25 06:56:13.000000 peppermining-0.1.1/peppermining.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-25 06:56:13.000000 peppermining-0.1.1/peppermining.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      669 2023-04-25 06:55:17.000000 peppermining-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 06:56:17.104804 peppermining-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1315 2023-04-25 06:55:25.000000 peppermining-0.1.1/setup.py
```

### Comparing `peppermining-0.1.0/LICENSE.txt` & `peppermining-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/PKG-INFO` & `peppermining-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peppermining
-Version: 0.1.0
+Version: 0.1.1
 Summary: PepperMining is a free Process Mining framework.
 Home-page: https://github.com/ThoberDetofeno/peppermining
 Author: Thober Detofeno
 Author-email: Thober Detofeno <thober@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ThoberDetofeno/peppermining
 Project-URL: Bug Tracker, https://github.com/ThoberDetofeno/peppermining/issues
```

### Comparing `peppermining-0.1.0/peppermining/conformance/conformance.py` & `peppermining-0.1.1/peppermining/conformance/conformance.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/conformance/process_model.py` & `peppermining-0.1.1/peppermining/conformance/process_model.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/conformance/root_cause_analysis.py` & `peppermining-0.1.1/peppermining/conformance/root_cause_analysis.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/conformance/violation/__init__.py` & `peppermining-0.1.1/peppermining/conformance/violation/__init__.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/conformance/violation/pepper_violation.py` & `peppermining-0.1.1/peppermining/conformance/violation/pepper_violation.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/conformance/violation/run_by_same_user.py` & `peppermining-0.1.1/peppermining/conformance/violation/run_by_same_user.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/conformance/violation/undesired_activity.py` & `peppermining-0.1.1/peppermining/conformance/violation/undesired_activity.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/conformance/violation/undesired_connection.py` & `peppermining-0.1.1/peppermining/conformance/violation/undesired_connection.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/conformance/violation/undesired_end.py` & `peppermining-0.1.1/peppermining/conformance/violation/undesired_end.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/conformance/violation/undesired_start.py` & `peppermining-0.1.1/peppermining/conformance/violation/undesired_start.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/filters/__init__.py` & `peppermining-0.1.1/peppermining/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/filters/case_activity_filter.py` & `peppermining-0.1.1/peppermining/filters/case_activity_filter.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/filters/case_between_time_filter.py` & `peppermining-0.1.1/peppermining/filters/case_between_time_filter.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/filters/case_end_activity_filter.py` & `peppermining-0.1.1/peppermining/filters/case_end_activity_filter.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/filters/case_filter.py` & `peppermining-0.1.1/peppermining/filters/case_filter.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/filters/case_size_filter.py` & `peppermining-0.1.1/peppermining/filters/case_size_filter.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/filters/case_start_activity_filter.py` & `peppermining-0.1.1/peppermining/filters/case_start_activity_filter.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/filters/pepper_filter.py` & `peppermining-0.1.1/peppermining/filters/pepper_filter.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/filters/variant_filter.py` & `peppermining-0.1.1/peppermining/filters/variant_filter.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/kpi/__init__.py` & `peppermining-0.1.1/peppermining/kpi/__init__.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/kpi/average_events_per_case.py` & `peppermining-0.1.1/peppermining/kpi/average_events_per_case.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/kpi/number_of_activities.py` & `peppermining-0.1.1/peppermining/kpi/number_of_activities.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/kpi/number_of_cases.py` & `peppermining-0.1.1/peppermining/kpi/number_of_cases.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/kpi/number_of_events.py` & `peppermining-0.1.1/peppermining/kpi/number_of_events.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/kpi/pepper_kpi.py` & `peppermining-0.1.1/peppermining/kpi/pepper_kpi.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/kpi/rework.py` & `peppermining-0.1.1/peppermining/kpi/rework.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/kpi/throughput_time.py` & `peppermining-0.1.1/peppermining/kpi/throughput_time.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/main.py` & `peppermining-0.1.1/peppermining/main.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/pepper.py` & `peppermining-0.1.1/peppermining/pepper.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining/peppermining.py` & `peppermining-0.1.1/peppermining/peppermining.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                              'check ticket', 'examine casually', 'decide'],
                 'event_time': ['2022-02-01 11:02:00', '2022-02-02 10:06:00', '2022-02-02 15:12:00', '2022-02-03 11:18:00', '2022-02-03 14:24:00',
                                '2022-02-01 11:32:00', '2022-02-01 12:12:00', '2022-02-01 14:16:00', '2022-02-03 11:22:00'],
                 'user': ['Pete', 'Sue', 'Mike', 'Sara', 'Pete', 'Mike', 'Mike', 'Sean', 'Sara']}
     >>> df = pd.DataFrame(data, columns=['case_id', 'activity', 'event_time', 'user'])
     >>> pm = PepperMining()
     >>> pm.set_event_log(df)
-    >>> pm.get_event_data()
+    >>> pm.get_event_log()
     """
     # TODO: Read IEEE XES files. http://www.xes-standard.org/
 
     def __init__(self):
         """Created PepperMining object.
         """
         super().__init__()
```

### Comparing `peppermining-0.1.0/peppermining/utils/enum.py` & `peppermining-0.1.1/peppermining/utils/enum.py`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/peppermining.egg-info/PKG-INFO` & `peppermining-0.1.1/peppermining.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peppermining
-Version: 0.1.0
+Version: 0.1.1
 Summary: PepperMining is a free Process Mining framework.
 Home-page: https://github.com/ThoberDetofeno/peppermining
 Author: Thober Detofeno
 Author-email: Thober Detofeno <thober@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ThoberDetofeno/peppermining
 Project-URL: Bug Tracker, https://github.com/ThoberDetofeno/peppermining/issues
```

### Comparing `peppermining-0.1.0/peppermining.egg-info/SOURCES.txt` & `peppermining-0.1.1/peppermining.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peppermining-0.1.0/pyproject.toml` & `peppermining-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "peppermining"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Thober Detofeno", email="thober@gmail.com" },
 ]
 description = "PepperMining is a free Process Mining framework."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `peppermining-0.1.0/setup.py` & `peppermining-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(name='peppermining',
-      version='0.1.0',
+      version='0.1.1',
       author='Thober Detofeno',
       author_email='thober@gmail.com',
       description="PepperMining is a free Process Mining framework.",
       long_description="PepperMining is a open source Process Mining platform written in Python.",
       license='MIT',
       long_description_content_type='text/markdown',
       install_requires=['numpy', 'pandas', 'pydot', 'deepdiff'],
```

