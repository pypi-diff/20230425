# Comparing `tmp/retentioneering-3.0.0b2.tar.gz` & `tmp/retentioneering-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retentioneering-3.0.0b2.tar", max compression
+gzip compressed data, was "retentioneering-3.0.0rc1.tar", max compression
```

## Comparing `retentioneering-3.0.0b2.tar` & `retentioneering-3.0.0rc1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
--rw-r--r--   0        0        0     7341 2022-09-06 07:58:30.273796 retentioneering-3.0.0b2/LICENSE
--rw-r--r--   0        0        0     1947 2023-04-19 10:57:10.934033 retentioneering-3.0.0b2/pyproject.toml
--rw-r--r--   0        0        0      375 2023-04-19 10:56:29.220603 retentioneering-3.0.0b2/retentioneering/__init__.py
--rw-r--r--   0        0        0       84 2023-01-16 14:26:06.541078 retentioneering-3.0.0b2/retentioneering/backend/__init__.py
--rw-r--r--   0        0        0      113 2023-01-16 14:26:06.541078 retentioneering-3.0.0b2/retentioneering/backend/callback/__init__.py
--rw-r--r--   0        0        0      490 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/backend/callback/list_dataprocessors.py
--rw-r--r--   0        0        0     5220 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/backend/callback/mock_list_dataprocessor.py
--rw-r--r--   0        0        0     1097 2023-01-16 14:26:06.541078 retentioneering-3.0.0b2/retentioneering/backend/jupiter_server.py
--rw-r--r--   0        0        0     5293 2023-04-03 06:56:53.875728 retentioneering-3.0.0b2/retentioneering/backend/server_manager.py
--rw-r--r--   0        0        0      149 2023-04-17 15:56:20.806436 retentioneering-3.0.0b2/retentioneering/backend/tracker/__init__.py
--rw-r--r--   0        0        0     1675 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/backend/tracker/connector.py
--rw-r--r--   0        0        0     2036 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/backend/tracker/hwid.py
--rw-r--r--   0        0        0     2381 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/backend/tracker/tracker.py
--rw-r--r--   0        0        0     1162 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/backend/tracker/tracking_info.py
--rw-r--r--   0        0        0       59 2023-03-07 11:03:25.184838 retentioneering-3.0.0b2/retentioneering/constants/__init__.py
--rw-r--r--   0        0        0      345 2023-03-07 11:03:25.184838 retentioneering-3.0.0b2/retentioneering/constants/constants.py
--rw-r--r--   0        0        0       42 2023-01-16 14:26:06.541078 retentioneering-3.0.0b2/retentioneering/data_processor/__init__.py
--rw-r--r--   0        0        0     2190 2023-03-07 11:03:25.184838 retentioneering-3.0.0b2/retentioneering/data_processor/data_processor.py
--rw-r--r--   0        0        0     1744 2023-03-07 11:03:25.184838 retentioneering-3.0.0b2/retentioneering/data_processor/registry.py
--rw-r--r--   0        0        0      843 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/__init__.py
--rw-r--r--   0        0        0     3887 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/add_negative_events.py
--rw-r--r--   0        0        0     3794 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/add_positive_events.py
--rw-r--r--   0        0        0     2449 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/add_start_end_events.py
--rw-r--r--   0        0        0     4781 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/collapse_loops.py
--rw-r--r--   0        0        0     3517 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/drop_paths.py
--rw-r--r--   0        0        0     2342 2023-04-03 06:56:53.879061 retentioneering-3.0.0b2/retentioneering/data_processors_lib/filter_events.py
--rw-r--r--   0        0        0     3332 2023-04-03 06:56:53.879061 retentioneering-3.0.0b2/retentioneering/data_processors_lib/group_events.py
--rw-r--r--   0        0        0     5454 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/label_cropped_paths.py
--rw-r--r--   0        0        0     4633 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/label_lost_users.py
--rw-r--r--   0        0        0     3186 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/label_new_users.py
--rw-r--r--   0        0        0     1760 2023-03-17 11:02:30.068802 retentioneering-3.0.0b2/retentioneering/data_processors_lib/rename.py
--rw-r--r--   0        0        0     8492 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/split_sessions.py
--rw-r--r--   0        0        0     6575 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/truncate_paths.py
--rw-r--r--   0        0        0       56 2023-01-16 14:26:06.544412 retentioneering-3.0.0b2/retentioneering/datasets/__init__.py
--rw-r--r--   0        0        0        0 2023-01-16 14:26:06.544412 retentioneering-3.0.0b2/retentioneering/datasets/data/__init__.py
--rw-r--r--   0        0        0  1903381 2023-01-16 14:26:06.551078 retentioneering-3.0.0b2/retentioneering/datasets/data/ab_test_demo.csv
--rw-r--r--   0        0        0  1467900 2023-03-07 11:03:25.188171 retentioneering-3.0.0b2/retentioneering/datasets/data/simple-onlineshop.csv
--rw-r--r--   0        0        0     1352 2023-03-07 11:03:25.188171 retentioneering-3.0.0b2/retentioneering/datasets/load.py
--rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/edgelist/__init__.py
--rw-r--r--   0        0        0     4222 2023-04-03 06:56:53.879061 retentioneering-3.0.0b2/retentioneering/edgelist/edgelist.py
--rw-r--r--   0        0        0      486 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/eventstream/__init__.py
--rw-r--r--   0        0        0    42992 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/eventstream.py
--rw-r--r--   0        0        0      792 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/__init__.py
--rw-r--r--   0        0        0     1476 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/add_negative_events_helper.py
--rw-r--r--   0        0        0     1475 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/add_positive_events_helper.py
--rw-r--r--   0        0        0     1129 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/add_start_end_events_helper.py
--rw-r--r--   0        0        0     1539 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/collapse_loops_helper.py
--rw-r--r--   0        0        0     1373 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/drop_paths_helper.py
--rw-r--r--   0        0        0     1239 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/filter_events_helper.py
--rw-r--r--   0        0        0     1556 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/group_events_helper.py
--rw-r--r--   0        0        0     1557 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/label_cropped_paths_helper.py
--rw-r--r--   0        0        0     1513 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/label_lost_users_helper.py
--rw-r--r--   0        0        0     1336 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/label_new_users_helper.py
--rw-r--r--   0        0        0      781 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/rename_helper.py
--rw-r--r--   0        0        0     1946 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/split_sessions_helper.py
--rw-r--r--   0        0        0     1803 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/truncate_paths_helper.py
--rw-r--r--   0        0        0     4157 2023-04-03 06:56:53.879061 retentioneering-3.0.0b2/retentioneering/eventstream/schema.py
--rw-r--r--   0        0        0     2389 2023-04-03 06:56:53.879061 retentioneering-3.0.0b2/retentioneering/eventstream/types.py
--rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/exceptions/__init__.py
--rw-r--r--   0        0        0       45 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/exceptions/base.py
--rw-r--r--   0        0        0     1242 2023-03-22 12:39:29.884664 retentioneering-3.0.0b2/retentioneering/exceptions/server.py
--rw-r--r--   0        0        0      306 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/exceptions/widget.py
--rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/nodelist/__init__.py
--rw-r--r--   0        0        0     1071 2023-04-03 06:56:53.879061 retentioneering-3.0.0b2/retentioneering/nodelist/nodelist.py
--rw-r--r--   0        0        0       38 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/params_model/__init__.py
--rw-r--r--   0        0        0    11842 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/params_model/params_model.py
--rw-r--r--   0        0        0      952 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/params_model/registry.py
--rw-r--r--   0        0        0      105 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/preprocessing_graph/__init__.py
--rw-r--r--   0        0        0     4223 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/preprocessing_graph/nodes.py
--rw-r--r--   0        0        0    14182 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/preprocessing_graph/preprocessing_graph.py
--rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/preprocessor/__init__.py
--rw-r--r--   0        0        0       65 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/templates/__init__.py
--rw-r--r--   0        0        0       45 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/templates/preprocessing_graph/__init__.py
--rw-r--r--   0        0        0     1704 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/templates/preprocessing_graph/preprocessing_graph.html
--rw-r--r--   0        0        0      736 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/templates/preprocessing_graph/show.py
--rw-r--r--   0        0        0       42 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/templates/transition_graph/__init__.py
--rw-r--r--   0        0        0       22 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/templates/transition_graph/body.html
--rw-r--r--   0        0        0      713 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/templates/transition_graph/full.html
--rw-r--r--   0        0        0      894 2023-04-17 15:56:16.596442 retentioneering-3.0.0b2/retentioneering/templates/transition_graph/init_template.py
--rw-r--r--   0        0        0     1507 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/templates/transition_graph/inner_iframe.html
--rw-r--r--   0        0        0     1143 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/templates/transition_graph/show.py
--rw-r--r--   0        0        0      382 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/__init__.py
--rw-r--r--   0        0        0       33 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/_describe/__init__.py
--rw-r--r--   0        0        0     4543 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/_describe/_describe.py
--rw-r--r--   0        0        0       46 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/_describe_events/__init__.py
--rw-r--r--   0        0        0     4750 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/_describe_events/_describe_events.py
--rw-r--r--   0        0        0       50 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/_transition_matrix/__init__.py
--rw-r--r--   0        0        0     1319 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/_transition_matrix/_transition_matrix.py
--rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/tooling/clusters/__init__.py
--rw-r--r--   0        0        0    33471 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/clusters/clusters.py
--rw-r--r--   0        0        0     2039 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/tooling/clusters/segments.py
--rw-r--r--   0        0        0     3166 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/tooling/clusters/userlist.py
--rw-r--r--   0        0        0       29 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/tooling/cohorts/__init__.py
--rw-r--r--   0        0        0    13160 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/cohorts/cohorts.py
--rw-r--r--   0        0        0       39 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/tooling/constants/__init__.py
--rw-r--r--   0        0        0      240 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/tooling/constants/constants.py
--rw-r--r--   0        0        0       53 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/tooling/event_timestamp_hist/__init__.py
--rw-r--r--   0        0        0     5596 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/event_timestamp_hist/event_timestamp_hist.py
--rw-r--r--   0        0        0       27 2023-01-16 14:26:06.561078 retentioneering-3.0.0b2/retentioneering/tooling/funnel/__init__.py
--rw-r--r--   0        0        0    12195 2023-04-03 06:56:53.882394 retentioneering-3.0.0b2/retentioneering/tooling/funnel/funnel.py
--rw-r--r--   0        0        0       43 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/tooling/mixins/__init__.py
--rw-r--r--   0        0        0     1516 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/mixins/ended_events.py
--rw-r--r--   0        0        0       71 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/stattests/__init__.py
--rw-r--r--   0        0        0      171 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/stattests/constants.py
--rw-r--r--   0        0        0    11923 2023-04-17 15:56:20.813103 retentioneering-3.0.0b2/retentioneering/tooling/stattests/stattests.py
--rw-r--r--   0        0        0       36 2023-01-16 14:26:06.561078 retentioneering-3.0.0b2/retentioneering/tooling/step_matrix/__init__.py
--rw-r--r--   0        0        0    21738 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/tooling/step_matrix/step_matrix.py
--rw-r--r--   0        0        0       36 2023-01-16 14:26:06.561078 retentioneering-3.0.0b2/retentioneering/tooling/step_sankey/__init__.py
--rw-r--r--   0        0        0    24641 2023-04-17 15:56:20.813103 retentioneering-3.0.0b2/retentioneering/tooling/step_sankey/step_sankey.py
--rw-r--r--   0        0        0      110 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/tooling/timedelta_hist/__init__.py
--rw-r--r--   0        0        0      186 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/tooling/timedelta_hist/constants.py
--rw-r--r--   0        0        0    13318 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/tooling/timedelta_hist/timedelta_hist.py
--rw-r--r--   0        0        0       46 2023-04-03 06:56:53.882394 retentioneering-3.0.0b2/retentioneering/tooling/transition_graph/__init__.py
--rw-r--r--   0        0        0    35854 2023-04-17 15:56:20.813103 retentioneering-3.0.0b2/retentioneering/tooling/transition_graph/transition_graph.py
--rw-r--r--   0        0        0        0 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/tooling/typing/__init__.py
--rw-r--r--   0        0        0      171 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/tooling/typing/transition_graph/__init__.py
--rw-r--r--   0        0        0     1327 2023-04-03 06:56:53.882394 retentioneering-3.0.0b2/retentioneering/tooling/typing/transition_graph/graph_types.py
--rw-r--r--   0        0        0       49 2023-01-16 14:26:06.561078 retentioneering-3.0.0b2/retentioneering/tooling/user_lifetime_hist/__init__.py
--rw-r--r--   0        0        0     6555 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/tooling/user_lifetime_hist/user_lifetime_hist.py
--rw-r--r--   0        0        0      458 2023-01-16 14:26:06.561078 retentioneering-3.0.0b2/retentioneering/utils/__init__.py
--rw-r--r--   0        0        0      122 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/utils/dict.py
--rw-r--r--   0        0        0      465 2023-01-16 14:26:06.561078 retentioneering-3.0.0b2/retentioneering/utils/list.py
--rw-r--r--   0        0        0      444 2023-01-16 14:26:06.561078 retentioneering-3.0.0b2/retentioneering/utils/pandas.py
--rw-r--r--   0        0        0      986 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/utils/registry.py
--rw-r--r--   0        0        0      269 2023-01-16 14:26:06.561078 retentioneering-3.0.0b2/retentioneering/utils/singleton.py
--rw-r--r--   0        0        0       77 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/widget/__init__.py
--rw-r--r--   0        0        0     7265 2023-03-22 12:39:29.887997 retentioneering-3.0.0b2/retentioneering/widget/widgets.py
--rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 retentioneering-3.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     7341 2022-09-06 07:58:30.273796 retentioneering-3.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     1948 2023-04-25 09:10:37.994103 retentioneering-3.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      375 2023-04-19 10:56:29.220603 retentioneering-3.0.0rc1/retentioneering/__init__.py
+-rw-r--r--   0        0        0       84 2023-01-16 14:26:06.541078 retentioneering-3.0.0rc1/retentioneering/backend/__init__.py
+-rw-r--r--   0        0        0      113 2023-01-16 14:26:06.541078 retentioneering-3.0.0rc1/retentioneering/backend/callback/__init__.py
+-rw-r--r--   0        0        0      490 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/backend/callback/list_dataprocessors.py
+-rw-r--r--   0        0        0     5220 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/backend/callback/mock_list_dataprocessor.py
+-rw-r--r--   0        0        0     1097 2023-01-16 14:26:06.541078 retentioneering-3.0.0rc1/retentioneering/backend/jupiter_server.py
+-rw-r--r--   0        0        0     5293 2023-04-03 06:56:53.875728 retentioneering-3.0.0rc1/retentioneering/backend/server_manager.py
+-rw-r--r--   0        0        0      238 2023-04-25 12:22:39.634379 retentioneering-3.0.0rc1/retentioneering/backend/tracker/__init__.py
+-rw-r--r--   0        0        0     1825 2023-04-25 10:18:51.331519 retentioneering-3.0.0rc1/retentioneering/backend/tracker/connector.py
+-rw-r--r--   0        0        0     2250 2023-04-25 10:01:07.873883 retentioneering-3.0.0rc1/retentioneering/backend/tracker/hwid.py
+-rw-r--r--   0        0        0     2875 2023-04-25 10:03:20.421185 retentioneering-3.0.0rc1/retentioneering/backend/tracker/tracker.py
+-rw-r--r--   0        0        0     1162 2023-04-22 16:00:11.500677 retentioneering-3.0.0rc1/retentioneering/backend/tracker/tracking_info.py
+-rw-r--r--   0        0        0       59 2023-03-07 11:03:25.184838 retentioneering-3.0.0rc1/retentioneering/constants/__init__.py
+-rw-r--r--   0        0        0      345 2023-03-07 11:03:25.184838 retentioneering-3.0.0rc1/retentioneering/constants/constants.py
+-rw-r--r--   0        0        0       42 2023-01-16 14:26:06.541078 retentioneering-3.0.0rc1/retentioneering/data_processor/__init__.py
+-rw-r--r--   0        0        0     2190 2023-03-07 11:03:25.184838 retentioneering-3.0.0rc1/retentioneering/data_processor/data_processor.py
+-rw-r--r--   0        0        0     1744 2023-03-07 11:03:25.184838 retentioneering-3.0.0rc1/retentioneering/data_processor/registry.py
+-rw-r--r--   0        0        0      843 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/__init__.py
+-rw-r--r--   0        0        0     3887 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/add_negative_events.py
+-rw-r--r--   0        0        0     3794 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/add_positive_events.py
+-rw-r--r--   0        0        0     2449 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/add_start_end_events.py
+-rw-r--r--   0        0        0     4781 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/collapse_loops.py
+-rw-r--r--   0        0        0     3517 2023-04-21 10:45:45.328652 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/drop_paths.py
+-rw-r--r--   0        0        0     2342 2023-04-03 06:56:53.879061 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/filter_events.py
+-rw-r--r--   0        0        0     3332 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/group_events.py
+-rw-r--r--   0        0        0     5454 2023-04-21 11:46:01.978908 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/label_cropped_paths.py
+-rw-r--r--   0        0        0     4633 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/label_lost_users.py
+-rw-r--r--   0        0        0     3186 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/label_new_users.py
+-rw-r--r--   0        0        0     1760 2023-03-17 11:02:30.068802 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/rename.py
+-rw-r--r--   0        0        0     8492 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/split_sessions.py
+-rw-r--r--   0        0        0     6575 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/truncate_paths.py
+-rw-r--r--   0        0        0       56 2023-01-16 14:26:06.544412 retentioneering-3.0.0rc1/retentioneering/datasets/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-16 14:26:06.544412 retentioneering-3.0.0rc1/retentioneering/datasets/data/__init__.py
+-rw-r--r--   0        0        0  1903381 2023-01-16 14:26:06.551078 retentioneering-3.0.0rc1/retentioneering/datasets/data/ab_test_demo.csv
+-rw-r--r--   0        0        0  1467900 2023-03-07 11:03:25.188171 retentioneering-3.0.0rc1/retentioneering/datasets/data/simple-onlineshop.csv
+-rw-r--r--   0        0        0     1352 2023-03-07 11:03:25.188171 retentioneering-3.0.0rc1/retentioneering/datasets/load.py
+-rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/edgelist/__init__.py
+-rw-r--r--   0        0        0     4222 2023-04-21 11:46:51.235714 retentioneering-3.0.0rc1/retentioneering/edgelist/edgelist.py
+-rw-r--r--   0        0        0      486 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/eventstream/__init__.py
+-rw-r--r--   0        0        0    42818 2023-04-25 09:09:49.820705 retentioneering-3.0.0rc1/retentioneering/eventstream/eventstream.py
+-rw-r--r--   0        0        0      792 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/__init__.py
+-rw-r--r--   0        0        0     1431 2023-04-25 09:09:49.820705 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/add_negative_events_helper.py
+-rw-r--r--   0        0        0     1430 2023-04-25 09:09:49.820705 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/add_positive_events_helper.py
+-rw-r--r--   0        0        0     1084 2023-04-25 09:09:49.820705 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/add_start_end_events_helper.py
+-rw-r--r--   0        0        0     1494 2023-04-25 09:09:49.820705 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/collapse_loops_helper.py
+-rw-r--r--   0        0        0     1328 2023-04-25 09:09:49.820705 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/drop_paths_helper.py
+-rw-r--r--   0        0        0     1194 2023-04-25 09:09:49.824038 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/filter_events_helper.py
+-rw-r--r--   0        0        0     1511 2023-04-25 09:09:49.824038 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/group_events_helper.py
+-rw-r--r--   0        0        0     1512 2023-04-25 09:09:49.824038 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/label_cropped_paths_helper.py
+-rw-r--r--   0        0        0     1468 2023-04-25 09:09:49.824038 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/label_lost_users_helper.py
+-rw-r--r--   0        0        0     1291 2023-04-25 09:09:49.824038 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/label_new_users_helper.py
+-rw-r--r--   0        0        0      736 2023-04-25 09:09:49.824038 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/rename_helper.py
+-rw-r--r--   0        0        0     1901 2023-04-25 09:09:49.827372 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/split_sessions_helper.py
+-rw-r--r--   0        0        0     1758 2023-04-25 09:09:49.827372 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/truncate_paths_helper.py
+-rw-r--r--   0        0        0     4157 2023-04-03 06:56:53.879061 retentioneering-3.0.0rc1/retentioneering/eventstream/schema.py
+-rw-r--r--   0        0        0     2389 2023-04-03 06:56:53.879061 retentioneering-3.0.0rc1/retentioneering/eventstream/types.py
+-rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/exceptions/__init__.py
+-rw-r--r--   0        0        0       45 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/exceptions/base.py
+-rw-r--r--   0        0        0     1242 2023-03-22 12:39:29.884664 retentioneering-3.0.0rc1/retentioneering/exceptions/server.py
+-rw-r--r--   0        0        0      306 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/exceptions/widget.py
+-rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/nodelist/__init__.py
+-rw-r--r--   0        0        0     1071 2023-04-03 06:56:53.879061 retentioneering-3.0.0rc1/retentioneering/nodelist/nodelist.py
+-rw-r--r--   0        0        0       38 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/params_model/__init__.py
+-rw-r--r--   0        0        0    11910 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/params_model/params_model.py
+-rw-r--r--   0        0        0      952 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/params_model/registry.py
+-rw-r--r--   0        0        0      105 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/preprocessing_graph/__init__.py
+-rw-r--r--   0        0        0     4223 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/preprocessing_graph/nodes.py
+-rw-r--r--   0        0        0    14182 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/preprocessing_graph/preprocessing_graph.py
+-rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/preprocessor/__init__.py
+-rw-r--r--   0        0        0       65 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/templates/__init__.py
+-rw-r--r--   0        0        0       45 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/templates/preprocessing_graph/__init__.py
+-rw-r--r--   0        0        0     1704 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/templates/preprocessing_graph/preprocessing_graph.html
+-rw-r--r--   0        0        0      736 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/templates/preprocessing_graph/show.py
+-rw-r--r--   0        0        0       42 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/__init__.py
+-rw-r--r--   0        0        0       22 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/body.html
+-rw-r--r--   0        0        0      713 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/full.html
+-rw-r--r--   0        0        0      894 2023-04-17 15:56:16.596442 retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/init_template.py
+-rw-r--r--   0        0        0     1507 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/inner_iframe.html
+-rw-r--r--   0        0        0     1143 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/show.py
+-rw-r--r--   0        0        0      382 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/__init__.py
+-rw-r--r--   0        0        0       33 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/_describe/__init__.py
+-rw-r--r--   0        0        0     4543 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/_describe/_describe.py
+-rw-r--r--   0        0        0       46 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/_describe_events/__init__.py
+-rw-r--r--   0        0        0     4750 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/_describe_events/_describe_events.py
+-rw-r--r--   0        0        0       50 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/_transition_matrix/__init__.py
+-rw-r--r--   0        0        0     1319 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/_transition_matrix/_transition_matrix.py
+-rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/tooling/clusters/__init__.py
+-rw-r--r--   0        0        0    30782 2023-04-25 09:09:49.827372 retentioneering-3.0.0rc1/retentioneering/tooling/clusters/clusters.py
+-rw-r--r--   0        0        0     2039 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/tooling/clusters/segments.py
+-rw-r--r--   0        0        0     3166 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/tooling/clusters/userlist.py
+-rw-r--r--   0        0        0       29 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/tooling/cohorts/__init__.py
+-rw-r--r--   0        0        0    13526 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/tooling/cohorts/cohorts.py
+-rw-r--r--   0        0        0       39 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/tooling/constants/__init__.py
+-rw-r--r--   0        0        0      240 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/tooling/constants/constants.py
+-rw-r--r--   0        0        0       53 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/tooling/event_timestamp_hist/__init__.py
+-rw-r--r--   0        0        0     6284 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/tooling/event_timestamp_hist/event_timestamp_hist.py
+-rw-r--r--   0        0        0       27 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc1/retentioneering/tooling/funnel/__init__.py
+-rw-r--r--   0        0        0    12972 2023-04-25 09:09:49.827372 retentioneering-3.0.0rc1/retentioneering/tooling/funnel/funnel.py
+-rw-r--r--   0        0        0       43 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/tooling/mixins/__init__.py
+-rw-r--r--   0        0        0     1516 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/mixins/ended_events.py
+-rw-r--r--   0        0        0       71 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/stattests/__init__.py
+-rw-r--r--   0        0        0      171 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/stattests/constants.py
+-rw-r--r--   0        0        0    13243 2023-04-25 09:09:49.827372 retentioneering-3.0.0rc1/retentioneering/tooling/stattests/stattests.py
+-rw-r--r--   0        0        0       36 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc1/retentioneering/tooling/step_matrix/__init__.py
+-rw-r--r--   0        0        0    22300 2023-04-25 09:09:49.827372 retentioneering-3.0.0rc1/retentioneering/tooling/step_matrix/step_matrix.py
+-rw-r--r--   0        0        0       36 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc1/retentioneering/tooling/step_sankey/__init__.py
+-rw-r--r--   0        0        0    25006 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/tooling/step_sankey/step_sankey.py
+-rw-r--r--   0        0        0      110 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/tooling/timedelta_hist/__init__.py
+-rw-r--r--   0        0        0      186 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/tooling/timedelta_hist/constants.py
+-rw-r--r--   0        0        0    13342 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/tooling/timedelta_hist/timedelta_hist.py
+-rw-r--r--   0        0        0       46 2023-04-03 06:56:53.882394 retentioneering-3.0.0rc1/retentioneering/tooling/transition_graph/__init__.py
+-rw-r--r--   0        0        0    36518 2023-04-24 11:53:04.647152 retentioneering-3.0.0rc1/retentioneering/tooling/transition_graph/transition_graph.py
+-rw-r--r--   0        0        0        0 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/tooling/typing/__init__.py
+-rw-r--r--   0        0        0      171 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/tooling/typing/transition_graph/__init__.py
+-rw-r--r--   0        0        0     1327 2023-04-03 06:56:53.882394 retentioneering-3.0.0rc1/retentioneering/tooling/typing/transition_graph/graph_types.py
+-rw-r--r--   0        0        0       49 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc1/retentioneering/tooling/user_lifetime_hist/__init__.py
+-rw-r--r--   0        0        0     7385 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/tooling/user_lifetime_hist/user_lifetime_hist.py
+-rw-r--r--   0        0        0      458 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc1/retentioneering/utils/__init__.py
+-rw-r--r--   0        0        0      122 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/utils/dict.py
+-rw-r--r--   0        0        0      465 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc1/retentioneering/utils/list.py
+-rw-r--r--   0        0        0      444 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc1/retentioneering/utils/pandas.py
+-rw-r--r--   0        0        0      986 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/utils/registry.py
+-rw-r--r--   0        0        0      269 2023-04-22 16:00:11.500677 retentioneering-3.0.0rc1/retentioneering/utils/singleton.py
+-rw-r--r--   0        0        0       77 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/widget/__init__.py
+-rw-r--r--   0        0        0     7265 2023-03-22 12:39:29.887997 retentioneering-3.0.0rc1/retentioneering/widget/widgets.py
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 retentioneering-3.0.0rc1/PKG-INFO
```

### Comparing `retentioneering-3.0.0b2/LICENSE` & `retentioneering-3.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/pyproject.toml` & `retentioneering-3.0.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "retentioneering"
-version = "3.0.0b2"
+version = "3.0.0rc1"
 description = "universal framework for data processing"
 authors = ["Retentioneering User Trajectory Analysis Lab <you@example.com>"]
 packages = [
     { include = "retentioneering"}
 ]
 
 [[tool.poetry.source]]
```

### Comparing `retentioneering-3.0.0b2/retentioneering/backend/callback/mock_list_dataprocessor.py` & `retentioneering-3.0.0rc1/retentioneering/backend/callback/mock_list_dataprocessor.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/backend/jupiter_server.py` & `retentioneering-3.0.0rc1/retentioneering/backend/jupiter_server.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/backend/server_manager.py` & `retentioneering-3.0.0rc1/retentioneering/backend/server_manager.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/backend/tracker/connector.py` & `retentioneering-3.0.0rc1/retentioneering/backend/tracker/connector.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,18 +36,22 @@
             post_thread = threading.Thread(target=self._post_job, args=(data,))
             post_thread.start()
         except Exception:
             # supress any exceptions in tracking
             # @TODO: store exceptions to tracking base or sentry. Vladimir Makhanov
             pass
 
-    def _post_job(self, data: dict) -> requests.Response:
-        data["source"] = self.source
-        with self.session.post(self.url, data=json.dumps(data)) as response:
-            return response
+    def _post_job(self, data: dict) -> requests.Response | None:
+        try:
+            data["source"] = self.source
+            with self.session.post(self.url, data=json.dumps(data)) as response:
+                return response
+        except Exception:
+            # supress any exceptions in tracking. Vladimir Makhanov
+            return None
 
     def _prepare_data(self, data: TrackingInfo) -> dict:
         prepared_data = asdict(data)
         prepared_data["source"] = self.source
         prepared_data["params"] = str(prepared_data["params"])
         return prepared_data
```

### Comparing `retentioneering-3.0.0b2/retentioneering/backend/tracker/hwid.py` & `retentioneering-3.0.0rc1/retentioneering/backend/tracker/hwid.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,34 +10,38 @@
 UNDEFINED_WINDOWS_PLATFORM_UUID = uuid.UUID("00000000-0000-0000-aaaa-aaaaaaaaaaaa")
 UNDEFINED_LINUX_PLATFORM_UUID = uuid.UUID("00000000-0000-0000-aaaa-bbbbbbbbbbbb")
 UNDEFINED_MAC_PLATFORM_UUID = uuid.UUID("00000000-0000-0000-aaaa-cccccccccccc")
 
 
 def get_windows_hwid() -> str:
     try:
-        current_machine_id = str(subprocess.check_output("wmic csproduct get uuid"), "utf-8").split("\n")[1].strip()
+        current_machine_id = (
+            str(subprocess.check_output("wmic csproduct get uuid", stderr=subprocess.DEVNULL), "utf-8")
+            .split("\n")[1]
+            .strip()
+        )
         hwid = str(uuid.UUID(current_machine_id))
     except Exception:  # not sure if this is the right exception, but I don't know right one. Vladimir Makhanov.
         hwid = str(UNDEFINED_WINDOWS_PLATFORM_UUID)
     return hwid
 
 
 def get_linux_hwid() -> str:
     try:
-        hw = subprocess.check_output(["cat", "/etc/machine-id"])
+        hw = subprocess.check_output(["cat", "/etc/machine-id"], stderr=subprocess.DEVNULL)
         hw = hw.decode().strip()
         hwid = str(uuid.UUID(hw))
     except Exception:  # not sure if this is the right exception, but I don't know right one. Vladimir Makhanov.
         hwid = str(UNDEFINED_LINUX_PLATFORM_UUID)
     return hwid
 
 
 def get_mac_hwid() -> str:
     try:
-        hw = subprocess.check_output(["cat", "/etc/machine-id"])
+        hw = subprocess.check_output(["cat", "/etc/machine-id"], stderr=subprocess.DEVNULL)
         hw = hw.decode().strip()
         hwid = str(uuid.UUID(hw))
     except Exception:  # not sure if this is the right exception, but I don't know right one. Vladimir Makhanov.
         hwid = str(UNDEFINED_MAC_PLATFORM_UUID)
     return hwid
 
 
@@ -48,13 +52,16 @@
 __platforms_HWID = defaultdict(default_factory=undefined_platform)
 __platforms_HWID["Windows"] = get_windows_hwid
 __platforms_HWID["Linux"] = get_linux_hwid
 __platforms_HWID["Darwin"] = get_mac_hwid
 
 
 def get_hwid() -> str:
-    os_name = platform.system()
-    hwid = __platforms_HWID[os_name]()
+    try:
+        os_name = platform.system()
+        hwid = __platforms_HWID[os_name]()
+    except Exception as e:
+        hwid = UNDEFINED_PLATFORM_UUID
     return hwid
 
 
 __all__ = ("get_hwid",)
```

### Comparing `retentioneering-3.0.0b2/retentioneering/backend/tracker/tracker.py` & `retentioneering-3.0.0rc1/retentioneering/backend/tracker/tracker.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,37 +29,55 @@
         return get_hwid()
 
     def __clean_params(self, params: dict[str, Any], allowed_params: list[str] | None = None) -> dict[str, Any]:
         if allowed_params is None:
             allowed_params = []
         return {key: value for key, value in params.items() if key in allowed_params}
 
+    def _track_action(
+        self, called_function_params: dict[str, Any], event_name: str, event_custom_name: str, suffix: str
+    ) -> None:
+        if self.enabled:
+            try:
+                _tracking_info_start = TrackingInfo(
+                    client_session_id=self.user_id,
+                    event_name=f"{event_name}_{suffix}",
+                    event_custom_name=event_custom_name,
+                    params=called_function_params,
+                )
+                self.connector.send_message(data=_tracking_info_start)
+            except Exception:
+                # Maximum suppression. Vladimir Makhanov
+                pass
+        else:
+            pass
+
     def track(self, tracking_info: dict[str, Any], allowed_params: list[str] | None = None) -> Callable:
         event_name = tracking_info["event_name"]
         event_custom_name = tracking_info.get("event_custom_name", tracking_info["event_name"])
 
         def tracker_decorator(func: Callable) -> Callable:
             @functools.wraps(func)
             def wrapper(*args: list[Any], **kwargs: dict[Any, Any]) -> Callable:
                 called_function_params = self.__clean_params(kwargs, allowed_params)
-                _tracking_info_start = TrackingInfo(
-                    client_session_id=self.user_id,
-                    event_name=f"{event_name}_start",
+
+                self._track_action(
+                    called_function_params=called_function_params,
+                    event_name=event_name,
                     event_custom_name=event_custom_name,
-                    params=called_function_params,
+                    suffix="start",
                 )
-                self.connector.send_message(data=_tracking_info_start)
+
                 res = func(*args, **kwargs)
 
-                _tracking_info_end = TrackingInfo(
-                    client_session_id=self.user_id,
-                    event_name=f"{event_name}_end",
+                self._track_action(
+                    called_function_params=called_function_params,
+                    event_name=event_name,
                     event_custom_name=event_custom_name,
-                    params=called_function_params,
+                    suffix="end",
                 )
-                self.connector.send_message(data=_tracking_info_end)
 
                 return res
 
             return wrapper
 
         return tracker_decorator
```

### Comparing `retentioneering-3.0.0b2/retentioneering/backend/tracker/tracking_info.py` & `retentioneering-3.0.0rc1/retentioneering/backend/tracker/tracking_info.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/data_processor/data_processor.py` & `retentioneering-3.0.0rc1/retentioneering/data_processor/data_processor.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/data_processor/registry.py` & `retentioneering-3.0.0rc1/retentioneering/data_processor/registry.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/data_processors_lib/__init__.py` & `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/data_processors_lib/add_negative_events.py` & `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/add_negative_events.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/data_processors_lib/add_positive_events.py` & `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/add_positive_events.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/data_processors_lib/add_start_end_events.py` & `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/add_start_end_events.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/data_processors_lib/collapse_loops.py` & `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/collapse_loops.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class CollapseLoopsParams(ParamsModel):
     """
     A class with parameters for :py:class:`.CollapseLoops` class.
     """
 
     suffix: Optional[Literal["loop", "count"]]
-    time_agg: Literal["max", "min", "mean"] = "max"
+    time_agg: Literal["max", "min", "mean"] = "min"
 
 
 class CollapseLoops(DataProcessor):
     """
     Find ``loops`` and create new synthetic events in the paths of all users having such sequences.
 
     A ``loop`` - is a sequence of repetitive events.
@@ -34,15 +34,15 @@
 
         - If ``loop``, event_name will be event_name_loop.\n
         For example *"event1 - event1 - event1"* --> event1_loop.
 
         - If ``count``, event_name will be event_name_loop_{number of events}.\n
         For example *"event1 - event1 - event1"* --> event1_loop_3.
 
-    time_agg : {"max", "min", "mean"}, default "max"
+    time_agg : {"max", "min", "mean"}, default "min"
         Aggregation method to calculate timestamp values for new groups.
 
     Returns
     -------
     Eventstream
         Eventstream with:
```

### Comparing `retentioneering-3.0.0b2/retentioneering/data_processors_lib/drop_paths.py` & `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/drop_paths.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/data_processors_lib/filter_events.py` & `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/filter_events.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/data_processors_lib/group_events.py` & `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/group_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     event_name : str
         Name of the created event.
     func : Callable[[DataFrame, EventstreamSchema], Any]
         Custom function that returns boolean mask with the same length as input eventstream.
 
         - If ``True`` - events will be grouped.
         - If ``False`` - events will be remained.
-    event_type : str, default="group_alias"
+    event_type : str, default "group_alias"
         Event_type name for the grouped events.
         If custom event_type is created, it should be added to the ``DEFAULT_INDEX_ORDER``.
 
     Returns
     -------
     Eventstream
         ``Eventstream`` with:
```

### Comparing `retentioneering-3.0.0b2/retentioneering/data_processors_lib/label_cropped_paths.py` & `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/label_cropped_paths.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/data_processors_lib/label_lost_users.py` & `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/label_lost_users.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/data_processors_lib/label_new_users.py` & `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/label_new_users.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/data_processors_lib/rename.py` & `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/rename.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/data_processors_lib/split_sessions.py` & `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/split_sessions.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/data_processors_lib/truncate_paths.py` & `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/truncate_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,27 +29,27 @@
 
     Parameters
     ----------
     drop_before : str, optional
         Event name before which part of the user's path is dropped. The specified event remains in the data.
     drop_after : str, optional
         Event name after which part of the user's path is dropped. The specified event remains in the data.
-    occurrence_before : {"first", "last"}, default="first"
+    occurrence_before : {"first", "last"}, default "first"
         This parameter is necessary when the specified event occurs more than once in one user's path.
 
         - when set to ``first``, the part of the user path before the first event occurrence is dropped;
         - when set to ``last``, the part of the user path before the last event occurrence is dropped;
 
-    occurrence_after : {"first", "last"}, default="first"
+    occurrence_after : {"first", "last"}, default "first"
         The same behavior as in the 'occurrence_before', but for the other part of the user path.
-    shift_before : int,  default=0
+    shift_before : int,  default 0
         Sets the number of steps by which the truncate point is shifted from the selected event.
         If the value is negative, then the offset occurs to the left along the timeline.
         If positive, then it occurs to the right.
-    shift_after : int,  default=0
+    shift_after : int,  default 0
         The same behavior as in the ``shift_before``, but for the other part of the user path.
 
     Returns
     -------
     Eventstream
         ``Eventstream`` with events that should be deleted from input ``eventstream``.
```

### Comparing `retentioneering-3.0.0b2/retentioneering/datasets/data/ab_test_demo.csv` & `retentioneering-3.0.0rc1/retentioneering/datasets/data/ab_test_demo.csv`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/datasets/data/simple-onlineshop.csv` & `retentioneering-3.0.0rc1/retentioneering/datasets/data/simple-onlineshop.csv`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/datasets/load.py` & `retentioneering-3.0.0rc1/retentioneering/datasets/load.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/edgelist/edgelist.py` & `retentioneering-3.0.0rc1/retentioneering/edgelist/edgelist.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/eventstream.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/eventstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # flake8: noqa
 from __future__ import annotations
 
 import uuid
 import warnings
 from collections.abc import Collection
-from typing import Any, Callable, List, Literal, MutableMapping, Optional, Tuple, Union
+from typing import Any, Callable, List, Literal, MutableMapping, Optional, Tuple
 
 import numpy as np
 import pandas as pd
 
 from retentioneering.backend.tracker import track
 from retentioneering.constants import DATETIME_UNITS
 from retentioneering.eventstream.schema import EventstreamSchema, RawDataSchema
@@ -61,15 +61,14 @@
 )
 
 IndexOrder = List[Optional[str]]
 FeatureType = Literal["tfidf", "count", "frequency", "binary", "time", "time_fraction", "external"]
 NgramRange = Tuple[int, int]
 Method = Literal["kmeans", "gmm"]
 
-
 DEFAULT_INDEX_ORDER: IndexOrder = [
     "profile",
     "path_start",
     "new_user",
     "existing_user",
     "cropped_left",
     "session_start",
@@ -156,15 +155,15 @@
 
 
     """
 
     schema: EventstreamSchema
     index_order: IndexOrder
     relations: List[Relation]
-    preprocessiong_graph: PreprocessingGraph | None = None
+    _preprocessing_graph: PreprocessingGraph | None = None
 
     __raw_data_schema: RawDataSchemaType
     __events: pd.DataFrame | pd.Series[Any]
     __clusters: Clusters | None = None
     __funnel: Funnel | None = None
     __cohorts: Cohorts | None = None
     __step_matrix: StepMatrix | None = None
@@ -211,15 +210,15 @@
         if not relations:
             self.relations = []
         else:
             self.relations = relations
         self.__events = self.__prepare_events(raw_data) if prepare else raw_data
         self.__events = self.__required_cleanup(events=self.__events)
         self.index_events()
-        self.preprocessiong_graph = None
+        self._preprocessing_graph = None
 
     def copy(self) -> Eventstream:
         """
         Make a copy of current ``eventstream``.
 
         Returns
         -------
@@ -634,23 +633,22 @@
 
         Returns
         -------
         Funnel
             A ``Funnel`` class instance fitted to the given parameters.
 
         """
-        self.__funnel = Funnel(
-            eventstream=self,
+        self.__funnel = Funnel(eventstream=self)
+        self.__funnel.fit(
             stages=stages,
             stage_names=stage_names,
             funnel_type=funnel_type,
             segments=segments,
             segment_names=segment_names,
         )
-        self.__funnel.fit()
         if show_plot:
             figure = self.__funnel.plot()
             figure.show()
         return self.__funnel
 
     @property
     def clusters(self) -> Clusters:
@@ -668,22 +666,22 @@
         if self.__clusters is None:
             self.__clusters = Clusters(eventstream=self)
         return self.__clusters
 
     def step_matrix(
         self,
         max_steps: int = 20,
-        weight_col: Optional[str] = None,
+        weight_col: str | None = None,
         precision: int = 2,
-        targets: Optional[list[str] | str] = None,
-        accumulated: Optional[Union[Literal["both", "only"], None]] = None,
-        sorting: Optional[list[str]] = None,
+        targets: list[str] | str | None = None,
+        accumulated: Literal["both", "only"] | None = None,
+        sorting: list | None = None,
         threshold: float = 0,
-        centered: Optional[dict] = None,
-        groups: Optional[Tuple[list, list]] = None,
+        centered: dict | None = None,
+        groups: Tuple[list, list] | None = None,
         show_plot: bool = True,
     ) -> StepMatrix:
         """
         Show a heatmap visualization of the step matrix.
 
         Parameters
         ----------
@@ -694,38 +692,37 @@
 
         Returns
         -------
         StepMatrix
             A ``StepMatrix`` class instance fitted to the given parameters.
 
         """
-        self.__step_matrix = StepMatrix(
-            eventstream=self,
+        self.__step_matrix = StepMatrix(eventstream=self)
+
+        self.__step_matrix.fit(
             max_steps=max_steps,
             weight_col=weight_col,
             precision=precision,
             targets=targets,
             accumulated=accumulated,
             sorting=sorting,
             threshold=threshold,
             centered=centered,
             groups=groups,
         )
-
-        self.__step_matrix.fit()
         if show_plot:
             self.__step_matrix.plot()
         return self.__step_matrix
 
     def step_sankey(
         self,
         max_steps: int = 10,
-        threshold: Union[int, float] = 0.05,
+        threshold: int | float = 0.05,
         sorting: list | None = None,
-        targets: Union[list[str], str] | None = None,
+        targets: list[str] | str | None = None,
         autosize: bool = True,
         width: int | None = None,
         height: int | None = None,
         show_plot: bool = True,
     ) -> StepSankey:
         """
         Show a Sankey diagram visualizing the user paths in stepwise manner.
@@ -739,28 +736,19 @@
 
         Returns
         -------
         StepSankey
             A ``StepSankey`` class instance fitted to the given parameters.
 
         """
-        self.__sankey = StepSankey(
-            eventstream=self,
-            max_steps=max_steps,
-            threshold=threshold,
-            sorting=sorting,
-            targets=targets,
-            autosize=autosize,
-            width=width,
-            height=height,
-        )
+        self.__sankey = StepSankey(eventstream=self)
 
-        self.__sankey.fit()
+        self.__sankey.fit(max_steps=max_steps, threshold=threshold, sorting=sorting, targets=targets)
         if show_plot:
-            figure = self.__sankey.plot()
+            figure = self.__sankey.plot(autosize=autosize, width=width, height=height)
             figure.show()
         return self.__sankey
 
     def cohorts(
         self,
         cohort_start_unit: DATETIME_UNITS,
         cohort_period: Tuple[int, DATETIME_UNITS],
@@ -784,25 +772,24 @@
 
         Returns
         -------
         Cohorts
             A ``Cohorts`` class instance fitted to the given parameters.
         """
 
-        self.__cohorts = Cohorts(
-            eventstream=self,
+        self.__cohorts = Cohorts(eventstream=self)
+
+        self.__cohorts.fit(
             cohort_start_unit=cohort_start_unit,
             cohort_period=cohort_period,
             average=average,
             cut_bottom=cut_bottom,
             cut_right=cut_right,
             cut_diagonal=cut_diagonal,
         )
-
-        self.__cohorts.fit()
         if show_plot:
             self.__cohorts.heatmap(width=width, height=height)
         return self.__cohorts
 
     def stattests(
         self,
         test: STATTEST_NAMES,
@@ -820,32 +807,30 @@
             :py:class:`.Stattests`
 
         Returns
         -------
         StatTests
             A ``StatTest`` class instance fitted to the given parameters.
         """
-        self.__stattests = StatTests(
-            eventstream=self, groups=groups, func=func, test=test, group_names=group_names, alpha=alpha
-        )
-        self.__stattests.fit()
+        self.__stattests = StatTests(eventstream=self)
+        self.__stattests.fit(groups=groups, func=func, test=test, group_names=group_names, alpha=alpha)
         self.__stattests.display_results()
         return self.__stattests
 
     def timedelta_hist(
         self,
         raw_events_only: bool = False,
-        event_pair: Optional[list[str | Literal[EVENTSTREAM_GLOBAL_EVENTS]]] = None,
+        event_pair: list[str | Literal[EVENTSTREAM_GLOBAL_EVENTS]] | None = None,
         adjacent_events_only: bool = True,
         weight_col: str | None = None,
-        time_agg: Optional[AGGREGATION_NAMES] = None,
+        time_agg: AGGREGATION_NAMES | None = None,
         timedelta_unit: DATETIME_UNITS = "s",
         log_scale: bool | tuple[bool, bool] | None = None,
-        lower_cutoff_quantile: Optional[float] = None,
-        upper_cutoff_quantile: Optional[float] = None,
+        lower_cutoff_quantile: float | None = None,
+        upper_cutoff_quantile: float | None = None,
         bins: int | Literal[BINS_ESTIMATORS] = 20,
         width: float = 6.0,
         height: float = 4.5,
         show_plot: bool = True,
     ) -> TimedeltaHist:
         """
         Plot the distribution of the time deltas between two events. Support various
@@ -863,40 +848,42 @@
         -------
         TimedeltaHist
             A ``TimedeltaHist`` class instance fitted with given parameters.
 
         """
         self.__timedelta_hist = TimedeltaHist(
             eventstream=self,
+        )
+
+        self.__timedelta_hist.fit(
             raw_events_only=raw_events_only,
             event_pair=event_pair,
             adjacent_events_only=adjacent_events_only,
             time_agg=time_agg,
             weight_col=weight_col,
             timedelta_unit=timedelta_unit,
             log_scale=log_scale,
             lower_cutoff_quantile=lower_cutoff_quantile,
             upper_cutoff_quantile=upper_cutoff_quantile,
             bins=bins,
-            width=width,
-            height=height,
         )
-
-        self.__timedelta_hist.fit()
         if show_plot:
-            self.__timedelta_hist.plot()
+            self.__timedelta_hist.plot(
+                width=width,
+                height=height,
+            )
 
         return self.__timedelta_hist
 
     def user_lifetime_hist(
         self,
         timedelta_unit: DATETIME_UNITS = "s",
         log_scale: bool | tuple[bool, bool] | None = None,
-        lower_cutoff_quantile: Optional[float] = None,
-        upper_cutoff_quantile: Optional[float] = None,
+        lower_cutoff_quantile: float | None = None,
+        upper_cutoff_quantile: float | None = None,
         bins: int | Literal[BINS_ESTIMATORS] = 20,
         width: float = 6.0,
         height: float = 4.5,
         show_plot: bool = True,
     ) -> UserLifetimeHist:
         """
         Plot the distribution of user lifetimes. A ``users lifetime`` is the timedelta between the first and the last
@@ -914,33 +901,32 @@
         UserLifetimeHist
             A ``UserLifetimeHist`` class instance with given parameters.
 
 
         """
         self.__user_lifetime_hist = UserLifetimeHist(
             eventstream=self,
+        )
+        self.__user_lifetime_hist.fit(
             timedelta_unit=timedelta_unit,
             log_scale=log_scale,
             lower_cutoff_quantile=lower_cutoff_quantile,
             upper_cutoff_quantile=upper_cutoff_quantile,
             bins=bins,
-            width=width,
-            height=height,
         )
-        self.__user_lifetime_hist.fit()
         if show_plot:
-            self.__user_lifetime_hist.plot()
+            self.__user_lifetime_hist.plot(width=width, height=height)
         return self.__user_lifetime_hist
 
     def event_timestamp_hist(
         self,
         event_list: list[str] | None = None,
         raw_events_only: bool = False,
-        lower_cutoff_quantile: Optional[float] = None,
-        upper_cutoff_quantile: Optional[float] = None,
+        lower_cutoff_quantile: float | None = None,
+        upper_cutoff_quantile: float | None = None,
         bins: int | Literal[BINS_ESTIMATORS] = 20,
         width: float = 6.0,
         height: float = 4.5,
         show_plot: bool = True,
     ) -> EventTimestampHist:
         """
         Plot distribution of events over time. Can be useful for detecting time-based anomalies, and visualising
@@ -957,26 +943,25 @@
         Returns
         -------
         EventTimestampHist
             A ``EventTimestampHist`` class instance with given parameters.
         """
         self.__event_timestamp_hist = EventTimestampHist(
             eventstream=self,
+        )
+
+        self.__event_timestamp_hist.fit(
             event_list=event_list,
             raw_events_only=raw_events_only,
             lower_cutoff_quantile=lower_cutoff_quantile,
             upper_cutoff_quantile=upper_cutoff_quantile,
             bins=bins,
-            width=width,
-            height=height,
         )
-
-        self.__event_timestamp_hist.fit()
         if show_plot:
-            self.__event_timestamp_hist.plot()
+            self.__event_timestamp_hist.plot(width=width, height=height)
         return self.__event_timestamp_hist
 
     def describe(self, session_col: str = "session_id", raw_events_only: bool = False) -> pd.DataFrame:
         """
         Display general eventstream information. If ``session_col`` is present in eventstream, also
         output session statistics.
 
@@ -1100,14 +1085,15 @@
             "width",
             "height",
         ],
     )
     def transition_graph(
         self,
         edges_norm_type: NormType = None,
+        nodes_norm_type: NormType = None,
         targets: MutableMapping[str, str | None] | None = None,
         nodes_threshold: Threshold | None = None,
         edges_threshold: Threshold | None = None,
         nodes_weight_col: str | None = None,
         edges_weight_col: str | None = None,
         custom_weight_cols: list[str] | None = None,
         width: int = 960,
@@ -1131,14 +1117,15 @@
             Rendered IFrame graph.
 
         """
         self.__transition_graph = TransitionGraph(eventstream=self)
         self.__transition_graph.plot(
             targets=targets,
             edges_norm_type=edges_norm_type,
+            nodes_norm_type=nodes_norm_type,
             edges_weight_col=edges_weight_col,
             nodes_threshold=nodes_threshold,
             edges_threshold=edges_threshold,
             nodes_weight_col=nodes_weight_col,
             custom_weight_cols=custom_weight_cols,
             width=width,
             height=height,
@@ -1150,18 +1137,18 @@
         )
         return self.__transition_graph
 
     def preprocessing_graph(self) -> PreprocessingGraph:
         """
         Display the preprocessing GUI tool.
         """
-        if self.preprocessiong_graph is None:
-            self.preprocessiong_graph = PreprocessingGraph(source_stream=self)
-        self.preprocessiong_graph.display()
-        return self.preprocessiong_graph
+        if self._preprocessing_graph is None:
+            self._preprocessing_graph = PreprocessingGraph(source_stream=self)
+        self._preprocessing_graph.display()
+        return self._preprocessing_graph
 
     @track(  # type: ignore
         tracking_info={"event_name": "transition_matrix", "event_custom_name": "transition_matrix_helper"},
         allowed_params=["weight_col", "norm_type"],
     )
     def transition_matrix(self, weight_col: str | None = None, norm_type: NormType = None) -> pd.DataFrame:
         """
```

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/__init__.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/add_negative_events_helper.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/add_negative_events_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,18 +26,16 @@
 
         """
         # avoid circular import
         from retentioneering.data_processors_lib import (
             AddNegativeEvents,
             AddNegativeEventsParams,
         )
+        from retentioneering.preprocessing_graph import PreprocessingGraph
         from retentioneering.preprocessing_graph.nodes import EventsNode
-        from retentioneering.preprocessing_graph.preprocessing_graph import (
-            PreprocessingGraph,
-        )
 
         p = PreprocessingGraph(source_stream=self)  # type: ignore
 
         params: dict[str, list[str] | Callable] = {"targets": targets}
         if func:
             params["func"] = func
```

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/add_positive_events_helper.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/add_positive_events_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,18 +25,16 @@
 
         """
         # avoid circular import
         from retentioneering.data_processors_lib import (
             AddPositiveEvents,
             AddPositiveEventsParams,
         )
+        from retentioneering.preprocessing_graph import PreprocessingGraph
         from retentioneering.preprocessing_graph.nodes import EventsNode
-        from retentioneering.preprocessing_graph.preprocessing_graph import (
-            PreprocessingGraph,
-        )
 
         p = PreprocessingGraph(source_stream=self)  # type: ignore
 
         params: dict[str, list[str] | Callable] = {"targets": targets}
         if func:
             params["func"] = func
```

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/add_start_end_events_helper.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/add_start_end_events_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,18 +17,16 @@
 
         """
         # avoid circular import
         from retentioneering.data_processors_lib import (
             AddStartEndEvents,
             AddStartEndEventsParams,
         )
+        from retentioneering.preprocessing_graph import PreprocessingGraph
         from retentioneering.preprocessing_graph.nodes import EventsNode
-        from retentioneering.preprocessing_graph.preprocessing_graph import (
-            PreprocessingGraph,
-        )
 
         p = PreprocessingGraph(source_stream=self)  # type: ignore
 
         node = EventsNode(processor=AddStartEndEvents(params=AddStartEndEventsParams(**{})))
         p.add_node(node=node, parents=[p.root])
         result = p.combine(node)
         del p
```

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/collapse_loops_helper.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/collapse_loops_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,18 +32,16 @@
         """
 
         # avoid circular import
         from retentioneering.data_processors_lib import (
             CollapseLoops,
             CollapseLoopsParams,
         )
+        from retentioneering.preprocessing_graph import PreprocessingGraph
         from retentioneering.preprocessing_graph.nodes import EventsNode
-        from retentioneering.preprocessing_graph.preprocessing_graph import (
-            PreprocessingGraph,
-        )
 
         p = PreprocessingGraph(source_stream=self)  # type: ignore
 
         node = EventsNode(
             processor=CollapseLoops(params=CollapseLoopsParams(suffix=suffix, time_agg=time_agg))  # type: ignore
         )
         p.add_node(node=node, parents=[p.root])
```

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/drop_paths_helper.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/drop_paths_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,18 +26,16 @@
              Input ``eventstream`` without the deleted short users' paths.
 
 
         """
 
         # avoid circular import
         from retentioneering.data_processors_lib import DropPaths, DropPathsParams
+        from retentioneering.preprocessing_graph import PreprocessingGraph
         from retentioneering.preprocessing_graph.nodes import EventsNode
-        from retentioneering.preprocessing_graph.preprocessing_graph import (
-            PreprocessingGraph,
-        )
 
         p = PreprocessingGraph(source_stream=self)  # type: ignore
 
         node = EventsNode(
             processor=DropPaths(params=DropPathsParams(min_steps=min_steps, min_time=min_time))  # type: ignore
         )
         p.add_node(node=node, parents=[p.root])
```

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/filter_events_helper.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/filter_events_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,16 @@
         Eventstream
             The filtered ``eventstream``.
 
 
         """
         # avoid circular import
         from retentioneering.data_processors_lib import FilterEvents, FilterEventsParams
+        from retentioneering.preprocessing_graph import PreprocessingGraph
         from retentioneering.preprocessing_graph.nodes import EventsNode
-        from retentioneering.preprocessing_graph.preprocessing_graph import (
-            PreprocessingGraph,
-        )
 
         p = PreprocessingGraph(source_stream=self)  # type: ignore
 
         node = EventsNode(processor=FilterEvents(params=FilterEventsParams(func=func)))  # type: ignore
         p.add_node(node=node, parents=[p.root])
         result = p.combine(node)
         del p
```

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/group_events_helper.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/group_events_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,18 +32,16 @@
 
 
 
         """
 
         # avoid circular import
         from retentioneering.data_processors_lib import GroupEvents, GroupEventsParams
+        from retentioneering.preprocessing_graph import PreprocessingGraph
         from retentioneering.preprocessing_graph.nodes import EventsNode
-        from retentioneering.preprocessing_graph.preprocessing_graph import (
-            PreprocessingGraph,
-        )
 
         p = PreprocessingGraph(source_stream=self)  # type: ignore
 
         node = EventsNode(
             processor=GroupEvents(
                 params=GroupEventsParams(event_name=event_name, func=func, event_type=event_type)  # type: ignore
             )
```

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/label_cropped_paths_helper.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/label_cropped_paths_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,18 +31,16 @@
 
         """
         # avoid circular import
         from retentioneering.data_processors_lib import (
             LabelCroppedPaths,
             LabelCroppedPathsParams,
         )
+        from retentioneering.preprocessing_graph import PreprocessingGraph
         from retentioneering.preprocessing_graph.nodes import EventsNode
-        from retentioneering.preprocessing_graph.preprocessing_graph import (
-            PreprocessingGraph,
-        )
 
         p = PreprocessingGraph(source_stream=self)  # type: ignore
 
         params = dict(left_cutoff=left_cutoff, right_cutoff=right_cutoff)
 
         node = EventsNode(processor=LabelCroppedPaths(params=LabelCroppedPathsParams(**params)))  # type: ignore
         p.add_node(node=node, parents=[p.root])
```

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/label_lost_users_helper.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/label_lost_users_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,18 +30,16 @@
         """
 
         # avoid circular import
         from retentioneering.data_processors_lib import (
             LabelLostUsers,
             LabelLostUsersParams,
         )
+        from retentioneering.preprocessing_graph import PreprocessingGraph
         from retentioneering.preprocessing_graph.nodes import EventsNode
-        from retentioneering.preprocessing_graph.preprocessing_graph import (
-            PreprocessingGraph,
-        )
 
         p = PreprocessingGraph(source_stream=self)  # type: ignore
 
         node = EventsNode(
             processor=LabelLostUsers(
                 params=LabelLostUsersParams(timeout=timeout, lost_users_list=lost_users_list)  # type: ignore
             )
```

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/label_new_users_helper.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/label_new_users_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,18 +24,16 @@
 
         """
         # avoid circular import
         from retentioneering.data_processors_lib import (
             LabelNewUsers,
             LabelNewUsersParams,
         )
+        from retentioneering.preprocessing_graph import PreprocessingGraph
         from retentioneering.preprocessing_graph.nodes import EventsNode
-        from retentioneering.preprocessing_graph.preprocessing_graph import (
-            PreprocessingGraph,
-        )
 
         p = PreprocessingGraph(source_stream=self)  # type: ignore
 
         node = EventsNode(
             processor=LabelNewUsers(params=LabelNewUsersParams(new_users_list=new_users_list))  # type: ignore
         )
         p.add_node(node=node, parents=[p.root])
```

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/rename_helper.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/rename_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 from ..types import EventstreamType
 
 
 class RenameHelperMixin:
     def rename(self, rules: list[dict[str, list[str] | str]]) -> EventstreamType:
         # avoid circular import
         from retentioneering.data_processors_lib import RenameParams, RenameProcessor
+        from retentioneering.preprocessing_graph import PreprocessingGraph
         from retentioneering.preprocessing_graph.nodes import EventsNode
-        from retentioneering.preprocessing_graph.preprocessing_graph import (
-            PreprocessingGraph,
-        )
 
         p = PreprocessingGraph(source_stream=self)  # type: ignore
 
         node = EventsNode(processor=RenameProcessor(params=RenameParams(rules=rules)))  # type: ignore
         p.add_node(node=node, parents=[p.root])
         result = p.combine(node)
         del p
```

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/split_sessions_helper.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/split_sessions_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,18 +35,16 @@
         """
 
         # avoid circular import
         from retentioneering.data_processors_lib import (
             SplitSessions,
             SplitSessionsParams,
         )
+        from retentioneering.preprocessing_graph import PreprocessingGraph
         from retentioneering.preprocessing_graph.nodes import EventsNode
-        from retentioneering.preprocessing_graph.preprocessing_graph import (
-            PreprocessingGraph,
-        )
 
         p = PreprocessingGraph(source_stream=self)  # type: ignore
         params = dict(timeout=timeout, session_col=session_col, mark_truncated=mark_truncated)
         node = EventsNode(processor=SplitSessions(params=SplitSessionsParams(**params)))  # type: ignore
         p.add_node(node=node, parents=[p.root])
         result = p.combine(node)
         del p
```

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/truncate_paths_helper.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/truncate_paths_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,16 @@
 
         """
         # avoid circular import
         from retentioneering.data_processors_lib import (
             TruncatePaths,
             TruncatePathsParams,
         )
+        from retentioneering.preprocessing_graph import PreprocessingGraph
         from retentioneering.preprocessing_graph.nodes import EventsNode
-        from retentioneering.preprocessing_graph.preprocessing_graph import (
-            PreprocessingGraph,
-        )
 
         p = PreprocessingGraph(source_stream=self)  # type: ignore
         params = {
             "drop_before": drop_before,
             "drop_after": drop_after,
             "occurrence_before": occurrence_before,
             "occurrence_after": occurrence_after,
```

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/schema.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/schema.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/eventstream/types.py` & `retentioneering-3.0.0rc1/retentioneering/eventstream/types.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/exceptions/server.py` & `retentioneering-3.0.0rc1/retentioneering/exceptions/server.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/nodelist/nodelist.py` & `retentioneering-3.0.0rc1/retentioneering/nodelist/nodelist.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/params_model/params_model.py` & `retentioneering-3.0.0rc1/retentioneering/params_model/params_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 from typing_extensions import TypedDict
 
 from retentioneering.exceptions.widget import WidgetParseError
 from retentioneering.params_model.registry import register_params_model
 from retentioneering.utils.dict import clear_dict
 from retentioneering.widget import WIDGET_MAPPING
 
-# disable warning for pydantic schema Callable type
-warnings.simplefilter(action="ignore", category=UserWarning)
-
 if TYPE_CHECKING:
     from pydantic.typing import AbstractSetIntStr, MappingIntStrAny
 
 
 class CustomWidgetProperties(TypedDict):
     widget: str
     serialize: Callable
@@ -69,15 +66,19 @@
 
     def __call__(self, **data: Dict[str, Any]) -> ParamsModel:
         ParamsModel.__init__(self, **data)
         return self
 
     @classmethod
     def _parse_schemas(cls) -> dict[str, str | dict | list]:
-        params_schema: dict[str, Any] = cls.schema()
+        with warnings.catch_warnings():
+            # disable warning for pydantic schema Callable type
+            warnings.simplefilter(action="ignore", category=UserWarning)
+            params_schema: dict[str, Any] = cls.schema()
+
         params_schema["required"] = params_schema.get("required", [])
 
         for field_name, field in cls.__fields__.items():
             field_type = getattr(field, "type_", None)
             # TODO: python3.8 fix
             field_type_classname_legacy = getattr(field_type, "_name", None)
             field_type_classname = getattr(field_type, "__name__", None)
```

### Comparing `retentioneering-3.0.0b2/retentioneering/params_model/registry.py` & `retentioneering-3.0.0rc1/retentioneering/params_model/registry.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/preprocessing_graph/nodes.py` & `retentioneering-3.0.0rc1/retentioneering/preprocessing_graph/nodes.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/preprocessing_graph/preprocessing_graph.py` & `retentioneering-3.0.0rc1/retentioneering/preprocessing_graph/preprocessing_graph.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/templates/preprocessing_graph/preprocessing_graph.html` & `retentioneering-3.0.0rc1/retentioneering/templates/preprocessing_graph/preprocessing_graph.html`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/templates/preprocessing_graph/show.py` & `retentioneering-3.0.0rc1/retentioneering/templates/preprocessing_graph/show.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/templates/transition_graph/full.html` & `retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/full.html`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/templates/transition_graph/init_template.py` & `retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/init_template.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/templates/transition_graph/inner_iframe.html` & `retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/inner_iframe.html`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/templates/transition_graph/show.py` & `retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/show.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/_describe/_describe.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/_describe/_describe.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/_describe_events/_describe_events.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/_describe_events/_describe_events.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/_transition_matrix/_transition_matrix.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/_transition_matrix/_transition_matrix.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/clusters/clusters.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/clusters/clusters.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from matplotlib import axes, rcParams
 from numpy import ndarray
 from sklearn.cluster import KMeans
 from sklearn.feature_extraction.text import CountVectorizer, TfidfVectorizer
 from sklearn.manifold import TSNE
 from sklearn.mixture import GaussianMixture
 
-from retentioneering.eventstream.types import EventstreamSchemaType, EventstreamType
+from retentioneering.eventstream.types import EventstreamType
 from retentioneering.tooling.clusters.segments import Segments
 
 FeatureType = Literal["tfidf", "count", "frequency", "binary", "time", "time_fraction", "markov"]
 SklearnFeatureType = Literal["count", "frequency", "tfidf", "binary"]
 NgramRange = Tuple[int, int]
 Method = Literal["kmeans", "gmm"]
 PlotType = Literal["cluster_bar"]
@@ -47,69 +47,56 @@
         self.__eventstream: EventstreamType = eventstream
         self.user_col = eventstream.schema.user_id
         self.event_col = eventstream.schema.event_name
         self.time_col = eventstream.schema.event_timestamp
         self.event_index_col = eventstream.schema.event_index
 
         self.__segments: Segments | None = None
-        self.__features: pd.DataFrame | None = None
         self.__cluster_result: pd.Series | None = None
         self.__projection: pd.DataFrame | None = None
         self.__is_fitted: bool = False
 
         self._method: Method | None = None
         self._n_clusters: int | None = None
         self._user_clusters: pd.Series | None = None
-        self._feature_type: FeatureType | None = None
-        self._ngram_range: NgramRange | None = None
         self._X: pd.DataFrame | None = None
 
     # public API
 
     def fit(
         self,
         method: Method,
         n_clusters: int,
-        feature_type: FeatureType | None = None,
-        ngram_range: NgramRange | None = None,
-        X: pd.DataFrame | None = None,
+        X: pd.DataFrame,
     ) -> Clusters:
         """
         Prepare features and compute clusters for the input eventstream data.
 
         Parameters
         ----------
         method : {"kmeans", "gmm"}
             - ``kmeans`` stands for the classic K-means algorithm.
               See details in :sklearn_kmeans:`sklearn documentation<>`.
             - ``gmm`` stands for Gaussian mixture model. See details in :sklearn_gmm:`sklearn documentation<>`.
 
         n_clusters : int
             The expected number of clusters to be passed to a clustering algorithm.
-        feature_type : {"tfidf", "count", "frequency", "binary", "markov", "time", "time_fraction"}, optional
-            See :py:func:`extract_features`.
-        ngram_range : Tuple(int, int), optional
-            See :py:func:`extract_features`.
-        X : pd.DataFrame, optional
+        X : pd.DataFrame
             ``pd.DataFrame`` representing a custom vectorization of the user paths. The index corresponds to user_ids,
-            the columns are vectorized values of the path.
+            the columns are vectorized values of the path. See :py:func:`extract_features`.
 
         Returns
         -------
         Clusters
             A fitted ``Clusters`` instance.
-
-
         """
 
-        self._method, self._n_clusters, self._feature_type, self._ngram_range, self._X = self.__validate_input(
-            method, n_clusters, feature_type, ngram_range, X
-        )
+        self._method, self._n_clusters, self._X = self.__validate_input(method, n_clusters, X)
 
-        self.__features, self.__cluster_result = self._prepare_clusters()
+        self.__cluster_result = self._prepare_clusters()
         self._user_clusters = self.__cluster_result.copy()
 
         self.__segments = Segments(
             eventstream=self.__eventstream,
             segments_df=self.__cluster_result.to_frame("segment").reset_index(),
         )
 
@@ -146,16 +133,14 @@
             (column name specified by parameter ``weight_col``) who have particular
             events will be plotted.
         targets : str or list of str, optional
             List of event names always to include for comparison, regardless
             of the parameter top_n_events value. Target events will appear in the same
             order as specified.
 
-
-
         Returns
         -------
         matplotlib.axes.Axes
             Plots the distribution barchart.
         """
         if not self.__is_fitted:
             raise RuntimeError("Clusters are not defined. Consider to run 'fit()' or `set_clusters()` methods.")
@@ -278,40 +263,20 @@
 
         df = self.__cluster_result.to_frame("cluster_id").reset_index()
         user_col, cluster_col = df.columns
         cluster_map = df.groupby(cluster_col)[user_col].apply(list)  # type: ignore
         return cluster_map.to_dict()
 
     @property
-    def features(self) -> pd.DataFrame | None:
-        """
-
-        Returns
-        -------
-        pd.DataFrame
-            The calculated features if the clusters are fitted. The index corresponds to user_ids,
-            the columns are values of the vectorized user's trajectory.
-        """
-        if self.__features is None:
-            raise RuntimeError("The features are not calculated. Consider to run 'extract_features()` method.")
-
-        return self.__features
-
-    @property
     def params(self) -> dict:
         """
         Returns the parameters used for the last fitting.
 
         """
-        return {
-            "method": self._method,
-            "n_clusters": self._n_clusters,
-            "ngram_range": self._ngram_range,
-            "feature_type": self._feature_type,
-        }
+        return {"method": self._method, "n_clusters": self._n_clusters, "X": self._X}
 
     def set_clusters(self, user_clusters: pd.Series) -> Clusters:
         """
         Set custom user-cluster mapping.
 
         Parameters
         ----------
@@ -323,17 +288,15 @@
         Clusters
             A fitted ``Clusters`` instance.
 
         """
         self._user_clusters = user_clusters
         self.__cluster_result = user_clusters.copy()
         self._n_clusters = user_clusters.nunique()
-        self._feature_type = None
         self._method = None
-        self._ngram_range = None
         self.__is_fitted = True
         return self
 
     def filter_cluster(self, cluster_id: int | str) -> EventstreamType:
         """
         Truncate the eventstream, leaving the trajectories of the users who belong to the selected cluster.
         Should be used after :py:func:`fit` or :py:func:`set_clusters`.
@@ -398,14 +361,15 @@
             and bigrams. Ignored for ``markov``, ``time``, ``time_fraction`` feature types.
 
         Returns
         -------
         pd.DataFrame
             A DataFrame with the vectorized values. Index contains user_ids, columns contain n-grams.
         """
+
         eventstream = self.__eventstream
         events = eventstream.to_dataframe()
         vec_data = None
 
         if feature_type in ["count", "frequency", "tfidf", "binary"] and ngram_range is not None:
             feature_type = cast(SklearnFeatureType, feature_type)
             events, vec_data = self._sklearn_vectorization(events, feature_type, ngram_range, self.user_col)
@@ -467,15 +431,15 @@
 
         Returns
         -------
         sns.scatterplot
             Plot in the low-dimensional space for user trajectories indexed by user IDs.
         """
 
-        if self.__features is None or self.__is_fitted is False:
+        if self._X is None or self.__is_fitted is False:
             raise RuntimeError("Clusters and features must be defined. Consider to run 'fit()' method.")
 
         if targets is None:
             targets = []
 
         if isinstance(targets, str):
             targets = [targets]
@@ -503,20 +467,18 @@
                     .to_frame()
                     .sort_index()[self.event_col]
                     .values
                 )
         else:
             raise ValueError("Unexpected plot type: %s. Allowed values: clusters, targets" % color_type)
 
-        features = self.__features
-
         if method == "tsne":
-            projection: pd.DataFrame = self._learn_tsne(features, **kwargs)
+            projection: pd.DataFrame = self._learn_tsne(self._X, **kwargs)
         elif method == "umap":
-            projection = self._learn_umap(features, **kwargs)
+            projection = self._learn_umap(self._X, **kwargs)
         else:
             raise ValueError("Unknown method: %s. Allowed methods: tsne, umap" % method)
 
         self.__projection = projection
 
         figure, _ = self._plot_projection(
             projection=projection.values,
@@ -527,71 +489,41 @@
         return figure
 
     # inner functions
     def __validate_input(
         self,
         method: Method,
         n_clusters: int,
-        feature_type: FeatureType | None = None,
-        ngram_range: NgramRange | None = None,
-        X: pd.DataFrame | None = None,
-    ) -> tuple[Method | None, int | None, FeatureType | None, NgramRange | None, pd.DataFrame | None]:
+        X: pd.DataFrame,
+    ) -> tuple[Method | None, int | None, pd.DataFrame]:
         _method = method or self._method
         _n_clusters = n_clusters or self._n_clusters
-        _user_clusters = None
 
-        if X is not None:
-            if not isinstance(X, pd.DataFrame):  # type: ignore
-                raise ValueError("Vector is not a DataFrame!")
-            if np.all(np.all(X.dtypes == "float") and X.isna().sum().sum() != 0):
-                raise ValueError(
-                    "Vector is wrong formatted! NaN should be replaced with 0 and all dtypes must be float!"
-                )
-            if feature_type:
-                raise ValueError("Both 'vector' and 'feature_type' are defined. 'feature_type' will be ignored.")
-            if ngram_range:
-                raise ValueError("Both 'vector' and 'ngram_range' are defined. 'ngram_range' will be ignored.")
-
-            _X = X
-            _feature_type = None
-            _ngram_range = None
-        else:
-            _feature_type = feature_type or self._feature_type
-            _ngram_range = ngram_range or self._ngram_range
-            _X = X or self._X
-
-            if _feature_type is None:
-                raise ValueError("'feature_type' must be defined for fitting.")
-
-            if _ngram_range is None:
-                raise ValueError("'ngram_range' must be defined for fitting.")
+        if not isinstance(X, pd.DataFrame):  # type: ignore
+            raise ValueError("X is not a DataFrame!")
+        if np.all(np.all(X.dtypes == "float") and X.isna().sum().sum() != 0):
+            raise ValueError("X is wrong formatted! NaN should be replaced with 0 and all dtypes must be float!")
 
-        return _method, _n_clusters, _feature_type, _ngram_range, _X
+        return _method, _n_clusters, X
 
-    def _prepare_clusters(self) -> tuple[pd.DataFrame, pd.Series]:
-        features = pd.DataFrame()
+    def _prepare_clusters(self) -> pd.Series:
         user_clusters = pd.Series(dtype=np.int64)
 
-        if self._X is not None:
-            features = self._X.copy()
-        else:
-            if self._feature_type is not None and self._ngram_range is not None:
-                features = self.extract_features(self._feature_type, self._ngram_range)
-
+        features = self._X.copy()  # type: ignore
         if self._n_clusters is not None:
             if self._method == "kmeans":
                 cluster_result = self._kmeans(features=features, n_clusters=self._n_clusters)
             elif self._method == "gmm":
                 cluster_result = self._gmm(features=features, n_clusters=self._n_clusters)
             else:
                 raise ValueError("Unknown method: %s" % self._method)
 
             user_clusters = pd.Series(cluster_result, index=features.index)
 
-        return features, user_clusters
+        return user_clusters
 
     @staticmethod
     def _plot_projection(projection: ndarray, targets: ndarray, legend_title: str) -> tuple:
         rcParams["figure.figsize"] = 8, 6
 
         scatter = sns.scatterplot(
             x=projection[:, 0],
```

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/clusters/segments.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/clusters/segments.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/clusters/userlist.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/clusters/userlist.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/cohorts/cohorts.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/cohorts/cohorts.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,111 +20,46 @@
     depending on the time of their first appearance in the eventstream; thus each user is
     associated with some ``cohort_group``. Retention rates of the active users
     belonging to each ``cohort_group`` are  calculated within each ``cohort_period``.
 
     Parameters
     ----------
     eventstream : EventstreamType
-    cohort_start_unit : :numpy_link:`DATETIME_UNITS<>`
-        The way of rounding and formatting of the moment from which the cohort count begins.
-        The minimum timestamp is rounded down to the selected datetime unit.
-
-        For example:
-        assume we have an eventstream with the following minimum timestamp - "2021-12-28 09:08:34.432456".
-        The result of roundings with different ``DATETIME_UNITS`` is shown in the table below:
-
-        +------------------------+-------------------------+
-        | **cohort_start_unit**  | **cohort_start_moment** |
-        +------------------------+-------------------------+
-        | Y                      |  2021-01-01 00:00:00    |
-        +------------------------+-------------------------+
-        | M                      |  2021-12-01 00:00:00    |
-        +------------------------+-------------------------+
-        | W                      |  2021-12-27 00:00:00    |
-        +------------------------+-------------------------+
-        | D                      |  2021-08-28 00:00:00    |
-        +------------------------+-------------------------+
-
-    cohort_period : Tuple(int, :numpy_link:`DATETIME_UNITS<>`)
-        The cohort_period size and its ``DATETIME_UNIT``. This parameter is used in calculating:
-
-        - Start moments for each cohort from the moment specified with the ``cohort_start_unit`` parameter
-        - Cohort periods for each cohort from its start moment.
-    average : bool, default True
-        - If ``True`` - calculating average for each cohort period.
-        - If ``False`` - averaged values aren't calculated.
-    cut_bottom : int, default 0
-        Drop 'n' rows from the bottom of the cohort matrix.
-        Average is recalculated.
-    cut_right : int, default 0
-        Drop 'n' columns from the right side of the cohort matrix.
-        Average is recalculated.
-    cut_diagonal : int, default 0
-        Replace values in 'n' diagonals (last period-group cells) with ``np.nan``.
-        Average is recalculated.
+
 
     See Also
     --------
     .Eventstream.cohorts : Call Cohorts tool as an eventstream method.
     .EventTimestampHist : Plot the distribution of events over time.
     .UserLifetimeHist : Plot the distribution of user lifetimes.
 
     Notes
     -----
-    Parameters ``cohort_start_unit`` and ``cohort_period`` should be consistent.
-    Due to "Y" and "M" being non-fixed types, it can be used only with each other
-    or if ``cohort_period_unit`` is more detailed than ``cohort_start_unit``.
-    More information - :numpy_timedelta_link:`about numpy timedelta<>`
-
-    Only cohorts with at least 1 user in some period are shown.
-
     See :doc:`Cohorts user guide</user_guides/cohorts>` for the details.
 
     """
 
     __eventstream: EventstreamType
+    cohort_start_unit: DATETIME_UNITS
     cohort_period: int
     cohort_period_unit: DATETIME_UNITS
-    cohort_start_unit: DATETIME_UNITS
 
-    def __init__(
-        self,
-        eventstream: EventstreamType,
-        cohort_start_unit: DATETIME_UNITS,
-        cohort_period: Tuple[int, DATETIME_UNITS],
-        average: bool = True,
-        cut_bottom: int = 0,
-        cut_right: int = 0,
-        cut_diagonal: int = 0,
-    ):
+    average: bool
+    cut_bottom: int
+    cut_right: int
+    cut_diagonal: int
+    _cohort_matrix_result: pd.DataFrame
+
+    def __init__(self, eventstream: EventstreamType):
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
-        self.average = average
-        self.cohort_start_unit = cohort_start_unit
-        self.cohort_period, self.cohort_period_unit = cohort_period
-        self.cut_bottom = cut_bottom
-        self.cut_right = cut_right
-        self.cut_diagonal = cut_diagonal
-
-        data = self.__eventstream.to_dataframe()
-        self.data = data
-        self._cohort_matrix_result: pd.DataFrame = pd.DataFrame()
-
-        if self.cohort_period <= 0:
-            raise ValueError("cohort_period should be positive integer!")
 
-        # @TODO добавить ссылку на numpy с объяснением. dpanina
-        if self.cohort_period_unit in ["Y", "M"] and self.cohort_start_unit not in ["Y", "M"]:
-            raise ValueError(
-                """Parameters ``cohort_start_unit`` and ``cohort_period`` should be consistent.
-                                 Due to "Y" and "M" are non-fixed types it can be used only with each other
-                                 or if ``cohort_period_unit`` is more detailed than ``cohort_start_unit``!"""
-            )
+        self._cohort_matrix_result = pd.DataFrame()
 
     def _add_min_date(
         self,
         data: pd.DataFrame,
         cohort_start_unit: DATETIME_UNITS,
         cohort_period: int,
         cohort_period_unit: DATETIME_UNITS,
@@ -177,24 +112,101 @@
         df: pd.DataFrame, cut_bottom: int = 0, cut_right: int = 0, cut_diagonal: int = 0
     ) -> pd.DataFrame:
         for row in df.index:
             df.loc[row, max(0, df.loc[row].notna()[::-1].idxmax() + 1 - cut_diagonal) :] = None  # type: ignore
 
         return df.iloc[: len(df) - cut_bottom, : len(df.columns) - cut_right]
 
-    def fit(self) -> None:
+    def fit(
+        self,
+        cohort_start_unit: DATETIME_UNITS,
+        cohort_period: Tuple[int, DATETIME_UNITS],
+        average: bool = True,
+        cut_bottom: int = 0,
+        cut_right: int = 0,
+        cut_diagonal: int = 0,
+    ) -> None:
         """
         Calculates the cohort internal values with the defined parameters.
         Applying ``fit`` method is necessary for the following usage
         of any visualization or descriptive ``Cohorts`` methods.
 
+        Parameters
+        ----------
+        cohort_start_unit : :numpy_link:`DATETIME_UNITS<>`
+            The way of rounding and formatting of the moment from which the cohort count begins.
+            The minimum timestamp is rounded down to the selected datetime unit.
+
+            For example:
+            assume we have an eventstream with the following minimum timestamp - "2021-12-28 09:08:34.432456".
+            The result of roundings with different ``DATETIME_UNITS`` is shown in the table below:
+
+            +------------------------+-------------------------+
+            | **cohort_start_unit**  | **cohort_start_moment** |
+            +------------------------+-------------------------+
+            | Y                      |  2021-01-01 00:00:00    |
+            +------------------------+-------------------------+
+            | M                      |  2021-12-01 00:00:00    |
+            +------------------------+-------------------------+
+            | W                      |  2021-12-27 00:00:00    |
+            +------------------------+-------------------------+
+            | D                      |  2021-08-28 00:00:00    |
+            +------------------------+-------------------------+
+
+        cohort_period : Tuple(int, :numpy_link:`DATETIME_UNITS<>`)
+            The cohort_period size and its ``DATETIME_UNIT``. This parameter is used in calculating:
+
+            - Start moments for each cohort from the moment specified with the ``cohort_start_unit`` parameter
+            - Cohort periods for each cohort from its start moment.
+        average : bool, default True
+            - If ``True`` - calculating average for each cohort period.
+            - If ``False`` - averaged values aren't calculated.
+        cut_bottom : int, default 0
+            Drop 'n' rows from the bottom of the cohort matrix.
+            Average is recalculated.
+        cut_right : int, default 0
+            Drop 'n' columns from the right side of the cohort matrix.
+            Average is recalculated.
+        cut_diagonal : int, default 0
+            Replace values in 'n' diagonals (last period-group cells) with ``np.nan``.
+            Average is recalculated.
+
+        Notes
+        -----
+        Parameters ``cohort_start_unit`` and ``cohort_period`` should be consistent.
+        Due to "Y" and "M" being non-fixed types, it can be used only with each other
+        or if ``cohort_period_unit`` is more detailed than ``cohort_start_unit``.
+        More information - :numpy_timedelta_link:`about numpy timedelta<>`
+
+        Only cohorts with at least 1 user in some period are shown.
+
+        See :doc:`Cohorts user guide</user_guides/cohorts>` for the details.
+
         """
+        data = self.__eventstream.to_dataframe()
+        self.average = average
+        self.cohort_start_unit = cohort_start_unit
+        self.cohort_period, self.cohort_period_unit = cohort_period
+        self.cut_bottom = cut_bottom
+        self.cut_right = cut_right
+        self.cut_diagonal = cut_diagonal
+
+        if self.cohort_period <= 0:
+            raise ValueError("cohort_period should be positive integer!")
+
+        # @TODO добавить ссылку на numpy с объяснением. dpanina
+        if self.cohort_period_unit in ["Y", "M"] and self.cohort_start_unit not in ["Y", "M"]:
+            raise ValueError(
+                """Parameters ``cohort_start_unit`` and ``cohort_period`` should be consistent.
+                                 Due to "Y" and "M" are non-fixed types it can be used only with each other
+                                 or if ``cohort_period_unit`` is more detailed than ``cohort_start_unit``!"""
+            )
 
         df = self._add_min_date(
-            data=self.data,
+            data=data,
             cohort_start_unit=self.cohort_start_unit,
             cohort_period=self.cohort_period,
             cohort_period_unit=self.cohort_period_unit,
         )
 
         cohorts = df.groupby(["CohortGroup", "CohortPeriod"])[[self.user_col]].nunique()
         cohorts.reset_index(inplace=True)
@@ -239,53 +251,53 @@
         df = self._cohort_matrix_result
         figsize = (width, height)
         figure, ax = plt.subplots(figsize=figsize)
         sns.heatmap(df, annot=True, fmt=".1%", linewidths=1, linecolor="gray", ax=ax)
         return ax
 
     def lineplot(
-        self, show_plot: Literal["cohorts", "average", "all"] = "cohorts", width: float = 7.0, height: float = 5.0
+        self, plot_type: Literal["cohorts", "average", "all"] = "cohorts", width: float = 7.0, height: float = 5.0
     ) -> matplotlib.axes.Axes:
         """
         Create a chart representing each cohort dynamics over time.
         Should be used after :py:func:`fit`.
 
         Parameters
         ----------
-        show_plot: 'cohorts', 'average' or 'all'
+        plot_type: 'cohorts', 'average' or 'all'
             - if ``cohorts`` - shows a lineplot for each cohort,
             - if ``average`` - shows a lineplot only for the average values over all the cohorts,
             - if ``all`` - shows a lineplot for each cohort and also for their average values.
         width : float, default 7.0
             Width of the figure in inches.
         height : float, default 5.0
             Height of the figure in inches.
 
         Returns
         -------
         matplotlib.axes.Axes
 
         """
-        if show_plot not in ["cohorts", "average", "all"]:
-            raise ValueError("show_plot parameter should be 'cohorts', 'average' or 'all'!")
+        if plot_type not in ["cohorts", "average", "all"]:
+            raise ValueError("plot_type parameter should be 'cohorts', 'average' or 'all'!")
         figsize = (width, height)
         df_matrix = self._cohort_matrix_result
         df_wo_average = df_matrix[df_matrix.index != "Average"]  # type: ignore
-        if show_plot in ["all", "average"] and "Average" not in df_matrix.index:  # type: ignore
+        if plot_type in ["all", "average"] and "Average" not in df_matrix.index:  # type: ignore
             df_matrix.loc["Average"] = df_matrix.mean()  # type: ignore
         df_average = df_matrix[df_matrix.index == "Average"]  # type: ignore
         figure, ax = plt.subplots(figsize=figsize)
-        if show_plot == "all":
+        if plot_type == "all":
             sns.lineplot(df_wo_average.T, lw=1.5, ax=ax)
             sns.lineplot(df_average.T, lw=2.5, palette=["red"], marker="X", markersize=8, alpha=0.6, ax=ax)
 
-        if show_plot == "average":
+        if plot_type == "average":
             sns.lineplot(df_average.T, lw=2.5, palette=["red"], marker="X", markersize=8, alpha=0.6, ax=ax)
 
-        if show_plot == "cohorts":
+        if plot_type == "cohorts":
             sns.lineplot(df_wo_average.T, lw=1.5, ax=ax)
 
         ax.legend(loc="upper left", bbox_to_anchor=(1, 1))
         ax.set_xlabel("Period from the start of observation")
         ax.set_ylabel("Share of active users")
         return ax
```

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/event_timestamp_hist/event_timestamp_hist.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/event_timestamp_hist/event_timestamp_hist.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import warnings
-from typing import Literal, Optional
+from typing import Literal
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 
@@ -16,99 +16,115 @@
 class EventTimestampHist:
     """
     Plot the distribution of events over time. Can be useful for detecting
     time-based anomalies, and visualising general timespan of the eventstream.
 
     Parameters
     ----------
-    raw_events_only : bool, default False
-        If ``True`` - statistics will only be shown for raw events.
-        If ``False`` - statistics will be shown for all events presented in your data.
-    event_list : list of str, optional
-        Specify events to be displayed.
-    lower_cutoff_quantile : float, optional
-        Specify time distance quantile as the lower boundary. The values below the boundary are truncated.
-    upper_cutoff_quantile : float, optional
-        Specify time distance quantile as the upper boundary. The values above the boundary are truncated.
-    bins : int or str, default 20
-        Generic bin parameter that can be the name of a reference rule or
-        the number of bins. Passed to :numpy_bins_link:`numpy.histogram_bin_edges<>`.
-    width : float, default 6.0
-        Width in inches.
-    height : float, default 4.5
-        Height in inches.
-
+    eventstream : EventstreamType
 
     See Also
     --------
     .TimedeltaHist : Plot the distribution of the time deltas between two events.
     .UserLifetimeHist : Plot the distribution of user lifetimes.
     .Eventstream.describe : Show general eventstream statistics.
     .Eventstream.describe_events : Show general eventstream events statistics.
 
     Notes
     -----
     See :ref:`Eventstream user guide<eventstream_events_timestamp>` for the details.
     """
 
-    def __init__(
-        self,
-        eventstream: EventstreamType,
-        raw_events_only: bool = False,
-        event_list: list[str] | None = None,
-        lower_cutoff_quantile: Optional[float] = None,
-        upper_cutoff_quantile: Optional[float] = None,
-        bins: int | Literal[BINS_ESTIMATORS] = 20,
-        width: float = 6.0,
-        height: float = 4.5,
-    ) -> None:
+    __eventstream: EventstreamType
+    raw_events_only: bool
+    event_list: list[str] | None
+    lower_cutoff_quantile: float | None
+    upper_cutoff_quantile: float | None
+    bins: int | Literal[BINS_ESTIMATORS]
+    bins_to_show: np.ndarray
+    values_to_plot: np.ndarray
+
+    def __init__(self, eventstream: EventstreamType) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
 
-        self.event_list = event_list
-        self.raw_events_only = raw_events_only
+        self.bins_to_show = np.array([])
+        self.values_to_plot = np.array([])
+
+    def _remove_cutoff_values(self, series: pd.Series) -> pd.Series:
+        idx = [True] * len(series)
+        if self.upper_cutoff_quantile is not None:
+            idx &= series <= series.quantile(self.upper_cutoff_quantile)
+        if self.lower_cutoff_quantile is not None:
+            idx &= series >= series.quantile(self.lower_cutoff_quantile)
+        return series[idx]
 
+    def __validate_input(
+        self,
+        lower_cutoff_quantile: float | None = None,
+        upper_cutoff_quantile: float | None = None,
+    ) -> tuple[float | None, float | None]:
         if lower_cutoff_quantile is not None:
             if not 0 < lower_cutoff_quantile < 1:
                 raise ValueError("lower_cutoff_quantile should be a fraction between 0 and 1.")
-        self.lower_cutoff_quantile = lower_cutoff_quantile
 
         if upper_cutoff_quantile is not None:
             if not 0 < upper_cutoff_quantile < 1:
                 raise ValueError("upper_cutoff_quantile should be a fraction between 0 and 1.")
-        self.upper_cutoff_quantile = upper_cutoff_quantile
 
         if lower_cutoff_quantile is not None and upper_cutoff_quantile is not None:
             if lower_cutoff_quantile > upper_cutoff_quantile:
                 warnings.warn("lower_cutoff_quantile exceeds upper_cutoff_quantile; no data passed to the histogram")
-        self.bins = bins
-        self.figsize = (width, height)
-        self.bins_to_show: np.ndarray = np.array([])
-        self.values_to_plot: np.ndarray = np.array([])
 
-    def _remove_cutoff_values(self, series: pd.Series) -> pd.Series:
-        idx = [True] * len(series)
-        if self.upper_cutoff_quantile is not None:
-            idx &= series <= series.quantile(self.upper_cutoff_quantile)
-        if self.lower_cutoff_quantile is not None:
-            idx &= series >= series.quantile(self.lower_cutoff_quantile)
-        return series[idx]
+        return upper_cutoff_quantile, lower_cutoff_quantile
 
-    def fit(self) -> None:
+    def fit(
+        self,
+        raw_events_only: bool = False,
+        event_list: list[str] | None = None,
+        lower_cutoff_quantile: float | None = None,
+        upper_cutoff_quantile: float | None = None,
+        bins: int | Literal[BINS_ESTIMATORS] = 20,
+    ) -> None:
         """
         Calculate values for the histplot.
 
+        Parameters
+        ----------
+        raw_events_only : bool, default False
+            If ``True`` - statistics will only be shown for raw events.
+            If ``False`` - statistics will be shown for all events presented in your data.
+        event_list : list of str, optional
+            Specify events to be displayed.
+        lower_cutoff_quantile : float, optional
+            Specify time distance quantile as the lower boundary. The values below the boundary are truncated.
+        upper_cutoff_quantile : float, optional
+            Specify time distance quantile as the upper boundary. The values above the boundary are truncated.
+        bins : int or str, default 20
+            Generic bin parameter that can be the name of a reference rule or
+            the number of bins. Passed to :numpy_bins_link:`numpy.histogram_bin_edges<>`.
+
         Returns
         -------
         None
 
         """
-        data = self.__eventstream.to_dataframe()
+
+        self.upper_cutoff_quantile, self.lower_cutoff_quantile = self.__validate_input(
+            lower_cutoff_quantile,
+            upper_cutoff_quantile,
+        )
+
+        self.event_list = event_list
+        self.raw_events_only = raw_events_only
+        self.bins = bins
+
+        data = self.__eventstream.to_dataframe(copy=True)
 
         if self.raw_events_only:
             data = data[data["event_type"].isin(["raw"])]
         if self.event_list:
             data = data[data[self.event_col].isin(self.event_list)]
 
         values_to_plot = data[self.time_col]
@@ -133,24 +149,32 @@
 
             1. The first array contains the values for histogram.
             2. The first array contains the bin edges.
 
         """
         return self.values_to_plot, self.bins_to_show
 
-    def plot(self) -> matplotlib.axes.Axesne:
+    def plot(self, width: float = 6.0, height: float = 4.5) -> matplotlib.axes.Axesne:
         """
         Create a sns.histplot based on the calculated values.
 
+        Parameters
+        ----------
+        width : float, default 6.0
+            Width in inches.
+        height : float, default 4.5
+            Height in inches.
+
         Returns
         -------
         :matplotlib_axes:`matplotlib.axes.Axes<>`
             The matplotlib axes containing the plot.
 
         """
 
-        plt.figure(figsize=self.figsize)
+        figsize = (width, height)
+        plt.figure(figsize=figsize)
 
         hist = sns.histplot(self.values_to_plot, bins=self.bins)
         hist.set_title("Event timestamp histogram")
 
         return hist
```

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/funnel/funnel.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/funnel/funnel.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,120 +5,102 @@
 
 import pandas as pd
 import plotly.graph_objects as go
 from pandas.core.common import flatten
 
 from retentioneering.eventstream.types import EventstreamType
 
+FunnelTypes = Literal["open", "closed", "hybrid"]
+
 
 class Funnel:
     """
     A class for the calculation and visualization of a conversion funnel.
 
     Parameters
     ----------
     eventstream : EventstreamType
-    stages: list of str
-        List of events used as stages for the funnel. Absolute and relative
-        number of users who reached specified events at least once will be
-        plotted. Multiple events can be grouped together as an individual state
-        by combining them as a sub list.
-    stage_names: list of str, optional
-        List of stage names, this is necessary for stages that include several events.
-    funnel_type: 'open', 'closed' or 'hybrid', default 'closed'
-        - if ``open`` - all users will be counted on each stage;
-        - if ``closed`` - each stage will include only users, that were present on all previous stages;
-        - if ``hybrid`` - combination of 2 previous types. The first stage is required
-          to go further. And for the second and subsequent stages it is important to have
-          all previous stages in their path, but the order of these events is not taken
-          into account.
-
-    segments: Collection[Collection[int]], optional
-        List of user_ids collections. Funnel for each user_id collection will be plotted.
-        If ``None`` - all users from the dataset will be plotted. A user can only belong to one segment at a time.
-    segment_names: list of str, optional
-        Names of segments. Should be a list from unique values of the ``segment_col``.
-        If ``None`` and ``segment_col`` is given - all values from ``segment_col`` will be used.
-
 
     See Also
     --------
     .Eventstream.funnel : Call Funnel tool as an eventstream method.
 
     Notes
     -----
     See :doc:`Funnel user guide</user_guides/funnel>` for the details.
 
     """
 
-    __eventstream: EventstreamType
     __default_layout = dict(
         margin={"l": 180, "r": 0, "t": 30, "b": 0, "pad": 0},
         funnelmode="stack",
         showlegend=True,
         hovermode="closest",
         legend=dict(orientation="v", bgcolor="#E2E2E2", xanchor="left", font=dict(size=12)),
     )
+    __eventstream: EventstreamType
+    stages: list[str]
+    stage_names: list[str] | None
+    funnel_type: FunnelTypes
+    segments: Collection[Collection[int]] | None
+    segment_names: list[str] | None
+    __res_dict: dict[str, dict]
 
-    def __init__(
-        self,
-        eventstream: EventstreamType,
-        stages: list[str],
-        stage_names: list[str] | None = None,
-        funnel_type: Literal["open", "closed", "hybrid"] = "closed",
-        segments: Collection[Collection[int]] | None = None,
-        segment_names: list[str] | None = None,
-    ) -> None:
+    def __init__(self, eventstream: EventstreamType) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
+        self.__res_dict = {}
 
-        self.stages = stages
-        self.funnel_type: Literal["open", "closed", "hybrid"] = funnel_type
-
-        data = self.__eventstream.to_dataframe()
+    def __validate_input(
+        self,
+        stages: list[str],
+        stage_names: list[str] | None = None,
+        funnel_type: FunnelTypes = "closed",
+        segments: Collection[Collection[int]] | None = None,
+        segment_names: list[str] | None = None,
+    ) -> tuple[pd.DataFrame, list[str], list[str], FunnelTypes, Collection[Collection[int]], list[str]]:
+        data = self.__eventstream.to_dataframe(copy=True)
         data = data[data[self.event_col].isin([i for i in flatten(stages)])]  # type: ignore
-        self.data = data
-        self.res_dict: dict = {}
 
-        if self.stages and stage_names and len(self.stages) != len(stage_names):
+        if stages and stage_names and len(stages) != len(stage_names):
             raise ValueError("stages and stage_names must be the same length!")
 
         if segments is None:
-            segments = [self.data[self.user_col].unique().tolist()]
+            segments = [data[self.user_col].unique().tolist()]
             segment_names = ["all users"]
         else:
             sets = [set(segment) for segment in segments]
             if len(set.intersection(*sets)) > 0:
                 raise ValueError("Check intersections of users in segments!")
 
         if segment_names is None:
             segment_names = [f"group {i}" for i in range(len(segments))]  # type: ignore
 
         if segments and segment_names and len(segments) != len(segment_names):  # type: ignore
             raise ValueError("segments and segment_names must be the same length!")
 
         # IDK why but pyright thinks this is Funnel!!!
-        self.segments = segments
-        self.segment_names = segment_names
 
         if funnel_type not in ["open", "closed", "hybrid"]:
             raise ValueError("funnel_type should be 'open', 'closed' or 'hybrid'!")
 
-        for idx, stage in enumerate(self.stages):
+        for idx, stage in enumerate(stages):
             if type(stage) is not list:
-                self.stages[idx] = [stage]  # type: ignore
+                stages[idx] = [stage]  # type: ignore
 
         if stage_names is None:
             stage_names = []
-            for t in self.stages:
+            for t in stages:
                 # get name
                 stage_names.append(" | ".join(t).strip(" | "))
-        self.stage_names = stage_names
+        stage_names = stage_names
+
+        return data, stages, stage_names, funnel_type, segments, segment_names
 
     def _plot_stacked_funnel(self, data: list[go.Funnel]) -> go.Figure:
         layout = go.Layout(**self.__default_layout)
         fig = go.Figure(data, layout)
         return fig
 
     @staticmethod
@@ -149,35 +131,35 @@
         data = data.merge(min_time_0stage, "left", on=self.user_col, suffixes=("", "_min"))
         data.rename(columns={data.columns[-1]: "min_date"}, inplace=True)
 
         # filtered NA and only events that occurred after the user entered the first funnel event remain
         data = data[(~data["min_date"].isna()) & (data["min_date"] <= data[self.time_col])]
         data.drop(columns="min_date", inplace=True)
 
-        res_dict = {}
+        __res_dict = {}
         for segment, name in zip(segments, segment_names):
             vals, _df = self._crop_df(data, stages, segment)
-            res_dict[name] = {"stages": stage_names, "values": vals}
-        return res_dict
+            __res_dict[name] = {"stages": stage_names, "values": vals}
+        return __res_dict
 
     def _prepare_data_for_open_funnel(
         self,
         data: pd.DataFrame,
         stages: list[str],
         stage_names: list[str],
         segments: Collection[Collection[int]],
         segment_names: list[str],
     ) -> dict[str, dict]:
-        res_dict = {}
+        __res_dict = {}
         for segment, name in zip(segments, segment_names):
             # isolate users from group
             group_data = data[data[self.user_col].isin(segment)]
             vals = [group_data[group_data[self.event_col].isin(stage)][self.user_col].nunique() for stage in stages]
-            res_dict[name] = {"stages": stage_names, "values": vals}
-        return res_dict
+            __res_dict[name] = {"stages": stage_names, "values": vals}
+        return __res_dict
 
     def _crop_df(self, df: pd.DataFrame, stages: list[str], segment: Collection[int]) -> tuple[list[int], pd.DataFrame]:
         first_stage = stages[0]
         next_stages = stages[1:]
 
         first_stage_users = set(
             (df[(df[self.event_col].isin(first_stage)) & (df[self.user_col].isin(segment))][self.user_col])
@@ -214,54 +196,91 @@
                 )
                 df.drop(columns="min_date", inplace=True)
             else:
                 df = df.drop(df[~df[self.user_col].isin(user_stage)].index.tolist())
 
         return vals, df
 
-    def fit(self) -> None:
+    def fit(
+        self,
+        stages: list[str],
+        stage_names: list[str] | None = None,
+        funnel_type: FunnelTypes = "closed",
+        segments: Collection[Collection[int]] | None = None,
+        segment_names: list[str] | None = None,
+    ) -> None:
         """
         Calculate the funnel internal values with the defined parameters.
         Applying ``fit`` method is necessary for the following usage
         of any visualization or descriptive ``Funnel`` methods.
 
+        Parameters
+        ----------
+        stages : list of str
+            List of events used as stages for the funnel. Absolute and relative
+            number of users who reached specified events at least once will be
+            plotted. Multiple events can be grouped together as an individual state
+            by combining them as a sub list.
+        stage_names : list of str, optional
+            List of stage names, this is necessary for stages that include several events.
+        funnel_type : 'open', 'closed' or 'hybrid', default 'closed'
+
+            - if ``open`` - all users will be counted on each stage;
+            - if ``closed`` - each stage will include only users, that were present on all previous stages;
+            - if ``hybrid`` - combination of 2 previous types. The first stage is required
+              to go further. And for the second and subsequent stages it is important to have
+              all previous stages in their path, but the order of these events is not taken
+              into account.
+
+        segments : Collection[Collection[int]], optional
+            List of user_ids collections. Funnel for each user_id collection will be plotted.
+            If ``None`` - all users from the dataset will be plotted. A user can only belong to one segment at a time.
+        segment_names : list of str, optional
+            Names of segments. Should be a list from unique values of the ``segment_col``.
+            If ``None`` and ``segment_col`` is given - all values from ``segment_col`` will be used.
         """
 
+        (
+            data,
+            self.stages,
+            self.stage_names,
+            self.funnel_type,
+            self.segments,
+            self.segment_names,
+        ) = self.__validate_input(stages, stage_names, funnel_type, segments, segment_names)
+
         if self.funnel_type in ["closed", "hybrid"]:
-            self.res_dict = self._prepare_data_for_closed_and_hybrid_funnel(
-                data=self.data,
+            self.__res_dict = self._prepare_data_for_closed_and_hybrid_funnel(
+                data=data,
                 stages=self.stages,
+                stage_names=self.stage_names,
                 segments=self.segments,
                 segment_names=self.segment_names,
-                stage_names=self.stage_names,
             )
 
         elif self.funnel_type == "open":
-            self.res_dict = self._prepare_data_for_open_funnel(
-                data=self.data,
+            self.__res_dict = self._prepare_data_for_open_funnel(
+                data=data,
                 stages=self.stages,
                 segments=self.segments,
                 segment_names=self.segment_names,
                 stage_names=self.stage_names,
             )
 
-        del self.data
-        self.data = pd.DataFrame()
-
     def plot(self) -> go.Figure:
         """
         Create a funnel plot based on the calculated funnel values.
         Should be used after :py:func:`fit`.
 
         Returns
         -------
         go.Figure
 
         """
-        result_dict = self.res_dict
+        result_dict = self.__res_dict
         data = self._calculate_plot_data(plot_params=result_dict)
         figure = self._plot_stacked_funnel(data=data)
         return figure
 
     @property
     def values(self) -> pd.DataFrame:
         """
@@ -276,15 +295,15 @@
             | **segment_name** |  **stages** | **unique_users**|  **%_of_initial** |  **%_of_total** |
             +------------------+-------------+-----------------+-------------------+-----------------+
             | segment_1        |  stage_1    |            2000 |            100.00 |          100.00 |
             +------------------+-------------+-----------------+-------------------+-----------------+
 
         """
 
-        result_dict = self.res_dict
+        result_dict = self.__res_dict
         result_list = []
         for key in result_dict:
             result_ = pd.DataFrame(result_dict[key])
             result_.columns = ["stages", "unique_users"]  # type: ignore
             result_["segment_name"] = key
             result_ = result_[["segment_name", "stages", "unique_users"]]
             result_["shift"] = result_["unique_users"].shift(periods=1, fill_value=result_["unique_users"][0])
```

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/mixins/ended_events.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/mixins/ended_events.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/stattests/stattests.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/stattests/stattests.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,90 +12,106 @@
 from statsmodels.stats.power import TTestIndPower
 from statsmodels.stats.weightstats import ttest_ind, ztest
 
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.tooling.stattests.constants import STATTEST_NAMES
 
 
-def _cohend(d1: list, d2: list) -> float:
-    n1, n2 = len(d1), len(d2)
-    s1, s2 = np.var(d1, ddof=1), np.var(d2, ddof=1)
-    s = float(math.sqrt(((n1 - 1) * s1 + (n2 - 1) * s2) / (n1 + n2 - 2)))
-    u1, u2 = float(np.mean(d1)), float(np.mean(d2))
-    return (u1 - u2) / s
+def _effect_size_cohend(sample1: list, sample2: list) -> float:
+    """
+    Calculate an effect size value using Cohen’s D measure (difference between two means).
+
+    Parameters
+    ----------
+    sample1 : list
+        First group's statistics.
+
+    sample2 : list
+        Second group's statistics.
+
+    Returns
+    -------
+    float
+        Calculated an effect size value.
 
+    """
+    sample_size1, sample_size2 = len(sample1), len(sample2)
+    standard_deviation1, standard_deviation2 = np.var(sample1, ddof=1), np.var(sample2, ddof=1)
+    pooled_standard_deviation = float(
+        math.sqrt(
+            ((sample_size1 - 1) * standard_deviation1 + (sample_size2 - 1) * standard_deviation2)
+            / (sample_size1 + sample_size2 - 2)
+        )
+    )
+    mean_sample1, mean_sample2 = float(np.mean(sample1)), float(np.mean(sample2))
+    return (mean_sample1 - mean_sample2) / pooled_standard_deviation
+
+
+def _effect_size_cohenh(sample1: list, sample2: list) -> float:
+    """
+    Calculate an effect size value using Cohen’s D measure (between proportions)
 
-def _cohenh(d1: list, d2: list) -> float:
-    u1, u2 = np.mean(d1), np.mean(d2)
-    return 2 * (math.asin(math.sqrt(u1)) - math.asin(math.sqrt(u2)))
+    Parameters
+    ----------
+    sample1 : list
+        First group's statistics.
+
+    sample2 : list
+        Second group's statistics.
+
+    Returns
+    -------
+    float
+        Calculated an effect size value.
+
+    """
+    mean_sample1, mean_sample2 = np.mean(sample1), np.mean(sample2)
+    return 2 * (math.asin(math.sqrt(mean_sample1)) - math.asin(math.sqrt(mean_sample2)))
 
 
 class StatTests:
     """
     A class for determining statistical difference between two groups of users.
 
     Parameters
     ----------
     eventstream : EventstreamType
-    test : {'mannwhitneyu', 'ttest', 'ztest', 'ks_2samp', 'chi2_contingency', 'fisher_exact'}
-        Test the null hypothesis that 2 independent samples are drawn from the same
-        distribution. Supported tests are:
-
-        - ``mannwhitneyu`` see :mannwhitneyu:`scipy documentation<>`.
-        - ``ttest`` see :statsmodel_ttest:`statsmodels documentation<>`.
-        - ``ztest`` see :statsmodel_ztest:`statsmodels documentation<>`.
-        - ``ks_2samp`` see :scipy_ks:`scipy documentation<>`.
-        - ``chi2_contingency`` see :scipy_chi2:`scipy documentation<>`.
-        - ``fisher_exact`` see :scipy_fisher:`scipy documentation<>`.
-
-    groups : tuple of list
-        Must contain a tuple of two elements (g_1, g_2): g_1 and g_2 are collections
-        of user_id`s.
-    func : Callable
-        Selected metrics. Must contain a function that takes a dataset as an argument for
-        a single user trajectory and returns a single numerical value.
-    group_names : tuple, default ('group_1', 'group_2')
-        Names for selected groups g_1 and g_2.
-    alpha : float, default 0.05
-        Selected level of significance.
-
 
     See Also
     --------
     .Eventstream.stattests : Call StatTests tool as an eventstream method.
 
     Notes
     -----
     See :doc:`StatTests user guide</user_guides/stattests>` for the details.
 
     """
 
-    def __init__(
-        self,
-        eventstream: EventstreamType,
-        test: STATTEST_NAMES,
-        groups: Tuple[list[str | int], list[str | int]],
-        func: Callable,
-        group_names: Tuple[str, str] = ("group_1", "group_2"),
-        alpha: float = 0.05,
-    ) -> None:
+    __eventstream: EventstreamType
+    test: STATTEST_NAMES
+    groups: Tuple[list[str | int], list[str | int]]
+    func: Callable
+    group_names: Tuple[str, str]
+    alpha: float
+    g1_data: list[str | int]
+    g2_data: list[str | int]
+
+    is_fitted: bool
+    output_template_numerical = "{0} (mean ± SD): {1:.3f} ± {2:.3f}, n = {3}"
+    output_template_categorical = "{0} (size): n = {1}"
+    p_val, power, label_min, label_max = 0.0, 0.0, "", ""
+
+    def __init__(self, eventstream: EventstreamType) -> None:
         self.__eventstream = eventstream
-        self.output_template_numerical = "{0} (mean ± SD): {1:.3f} ± {2:.3f}, n = {3}"
-        self.output_template_categorical = "{0} (size): n = {1}"
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
-        self.groups = groups
-        self.func = func
-        self.test = test
-        self.group_names = group_names
-        self.alpha = alpha
-        self.g1_data: list[str | int] = list()
-        self.g2_data: list[str | int] = list()
-        self.p_val, self.power, self.label_min, self.label_max = 0.0, 0.0, "", ""
+
+        self.g1_data = list()
+        self.g2_data = list()
         self.is_fitted = False
 
     def _get_group_values(self) -> Tuple[list, list]:
         data = self.__eventstream.to_dataframe()
         # obtain two populations for each group
         g1 = data[data[self.user_col].isin(self.groups[0])].copy()
         g2 = data[data[self.user_col].isin(self.groups[1])].copy()
@@ -117,18 +133,18 @@
         return crosstab(labels, values)[1]
 
     def _get_test_results(self, data_max: list, data_min: list) -> Tuple[float, float]:
         if self.test in ["ztest", "ttest", "mannwhitneyu", "ks_2samp"]:
             # calculate effect size
             if max(data_max) <= 1 and min(data_max) >= 0 and max(data_min) <= 1 and min(data_min) >= 0:
                 # if analyze proportions use Cohen's h:
-                effect_size = _cohenh(data_max, data_min)
+                effect_size = _effect_size_cohenh(data_max, data_min)
             else:
                 # for other variables use Cohen's d:
-                effect_size = _cohend(data_max, data_min)
+                effect_size = _effect_size_cohend(data_max, data_min)
 
             # calculate power
             power = TTestIndPower().power(
                 effect_size=effect_size,
                 nobs1=len(data_max),
                 ratio=len(data_min) / len(data_max),
                 alpha=self.alpha,
@@ -148,15 +164,15 @@
             if self.test == "chi2_contingency":
                 freq_table = self._get_freq_table(data_max, data_min)
                 p_val = chi2_contingency(freq_table)[1]
             elif self.test == "fisher_exact":
                 freq_table = self._get_freq_table(data_max, data_min)
                 p_val = fisher_exact(freq_table, alternative="greater")[1]
         else:
-            raise ValueError("The argument test is not supported. Supported tests are: {}".format(*STATTEST_NAMES))  # type: ignore
+            raise ValueError(f"The argument test is not supported. Supported tests are: {STATTEST_NAMES}")
         return p_val, power  # type: ignore
 
     def _get_sorted_test_results(self) -> Tuple[float, float, str, str]:
         p_val_norm, power_norm = self._get_test_results(self.g1_data, self.g2_data)
         p_val_rev, power_rev = self._get_test_results(self.g2_data, self.g1_data)
         if p_val_norm < p_val_rev:
             p_val = p_val_norm
@@ -166,21 +182,58 @@
         else:
             p_val = p_val_rev
             power = power_rev
             label_max = self.group_names[1]
             label_min = self.group_names[0]
         return p_val, power, label_max, label_min
 
-    def fit(self) -> None:
+    def fit(
+        self,
+        test: STATTEST_NAMES,
+        groups: Tuple[list[str | int], list[str | int]],
+        func: Callable,
+        group_names: Tuple[str, str] = ("group_1", "group_2"),
+        alpha: float = 0.05,
+    ) -> None:
         """
         Calculates the stattests internal values with the defined parameters.
         Applying ``fit`` method is necessary for the following usage
         of any visualization or descriptive ``StatTests`` methods.
 
+        Parameters
+        ----------
+        test : {'mannwhitneyu', 'ttest', 'ztest', 'ks_2samp', 'chi2_contingency', 'fisher_exact'}
+            Test the null hypothesis that 2 independent samples are drawn from the same
+            distribution. Supported tests are:
+
+            - ``mannwhitneyu`` see :mannwhitneyu:`scipy documentation<>`.
+            - ``ttest`` see :statsmodel_ttest:`statsmodels documentation<>`.
+            - ``ztest`` see :statsmodel_ztest:`statsmodels documentation<>`.
+            - ``ks_2samp`` see :scipy_ks:`scipy documentation<>`.
+            - ``chi2_contingency`` see :scipy_chi2:`scipy documentation<>`.
+            - ``fisher_exact`` see :scipy_fisher:`scipy documentation<>`.
+
+        groups : tuple of list
+            Must contain a tuple of two elements (g_1, g_2): g_1 and g_2 are collections
+            of user_id`s.
+        func : Callable
+            Selected metrics. Must contain a function that takes a dataset as an argument for
+            a single user trajectory and returns a single numerical value.
+        group_names : tuple, default ('group_1', 'group_2')
+            Names for selected groups g_1 and g_2.
+        alpha : float, default 0.05
+            Selected level of significance.
+
         """
+        self.groups = groups
+        self.func = func
+        self.test = test
+        self.group_names = group_names
+        self.alpha = alpha
+
         self.g1_data, self.g2_data = self._get_group_values()
         self.p_val, self.power, self.label_min, self.label_max = self._get_sorted_test_results()
         self.is_fitted = True
 
     def plot(self) -> Tuple[go.Figure, str]:
         """
         Plots a barplot comparing the metric values between two groups.
```

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/step_matrix/step_matrix.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/step_matrix/step_matrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import itertools
 from copy import deepcopy
 from dataclasses import dataclass
-from typing import Literal, Optional, Tuple, Union
+from typing import Literal, Tuple
 
 import matplotlib
 import pandas as pd
 import seaborn as sns
 
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.tooling.mixins.ended_events import EndedEventsMixin
@@ -31,120 +31,57 @@
     Step matrix is a matrix where its ``(i, j)`` element shows the frequency
     of event ``i`` occurring as ``j``-th step in user trajectories. This class
     provides methods for step matrix calculation and visualization.
 
     Parameters
     ----------
     eventstream : EventstreamType
-    max_steps : int, default=20
-        Maximum number of steps in ``user path`` to include.
-    weight_col : str, optional
-        Aggregation column for edge weighting. If ``None``, specified ``user_id``
-        from ``eventstream.schema`` will be used. For example, can be specified as
-        ``session_id`` if ``eventstream`` has such ``custom_col``.
-    precision : int, default=2
-        Number of decimal digits after 0 to show as fractions in the ``heatmap``.
-    targets : list of str or str, optional
-        List of event names to include in the bottom of ``step_matrix`` as individual rows.
-        Each specified target will have separate color-coding space for clear visualization.
-        `Example: ['product_page', 'cart', 'payment']`
-
-        If multiple targets need to be compared and plotted using the same color-coding scale,
-        such targets must be combined in a sub-list.
-        `Example: ['product_page', ['cart', 'payment']]`
-    accumulated : {"both", "only"}, optional
-        Option to include accumulated values for targets.
-
-        - If ``None``, accumulated tartes are not shown.
-        - If ``both``, show step values and accumulated values.
-        - If ``only``, show targets only as accumulated.
-    sorting : list of str, optional
-        - If list of event names specified - lines in the heatmap will be shown in
-          the passed order.
-        - If ``None`` - rows will be ordered according to i`th value (first row,
-          where 1st element is max; second row, where second element is max; etc)
-    threshold : float, default=0
-        Used to remove rare events. Aggregates all rows where all values are
-        less than the specified threshold.
-    centered : dict, optional
-        Parameter used to align user paths at a specific event at a specific step.
-        Has to contain three keys:
-        - ``event``: str, name of event to align.
-        - ``left_gap``: int, number of events to include before specified event.
-        - ``occurrence`` : int which occurrence of event to align (typical 1).
-
-        If not ``None`` - only users who have selected events with the specified
-        ``occurrence`` in their paths will be included.
-        ``Fraction`` of such remaining users is specified in the title of centered
-        step_matrix.
-        `Example: {'event': 'cart', 'left_gap': 8, 'occurrence': 1}`
-    groups : tuple[list, list], optional
-        Can be specified to plot differential step_matrix. Must contain
-        a tuple of two elements (g_1, g_2): where g_1 and g_2 are collections
-        of user_id`s. Two separate step_matrices M1 and M2 will be calculated
-        for users from g_1 and g_2, respectively. Resulting matrix will be the matrix
-        M = M1-M2.
-
-    Notes
-    -----
-    During step matrix calculation an artificial ``ENDED`` event is created. If a path already
-    contains ``path_end`` event (See :py:class:`.AddStartEndEvents`), it
-    will be temporarily replaced with ``ENDED`` (within step matrix only). Otherwise, ``ENDED``
-    event will be explicitly added to the end of each path.
-
-    Event ``ENDED`` is cumulated so that the values in its row are summed up from
-    the first step to the last. ``ENDED`` row is always placed at the last line of step matrix.
-    This design guarantees that the sum of any step matrix's column is 1
-    (0 for a differential step matrix).
-
-    See :doc:`StepMatrix user guide</user_guides/step_matrix>` for the details.
 
     See Also
     --------
     .Eventstream.step_matrix : Call StepMatrix tool as an eventstream method.
     .StepSankey : A class for the visualization of user paths in stepwise manner using Sankey diagram.
     .CollapseLoops : Find loops and create new synthetic events in the paths of all users having such sequences.
+
+    Notes
+    -----
+    See :doc:`StepMatrix user guide</user_guides/step_matrix>` for the details.
     """
 
     __eventstream: EventstreamType
     ENDED_EVENT = "ENDED"
+    max_steps: int
+    weight_col: str
+    precision: int
+    targets: list[str] | str | None = None
+    accumulated: Literal["both", "only"] | None = None
+    sorting: list | None = None
+    threshold: float
+    centered: CenteredParams | None = None
+    groups: Tuple[list, list] | None = None
+
+    __result_data: pd.DataFrame
+    __result_targets: pd.DataFrame | None
+    _fraction_title: str | None
+    _targets_list: list[list[str]] | None
 
     def __init__(
         self,
         eventstream: EventstreamType,
-        max_steps: int = 20,
-        weight_col: Optional[str] = None,
-        precision: int = 2,
-        targets: Optional[list[str] | str] = None,
-        accumulated: Optional[Union[Literal["both", "only"], None]] = None,
-        sorting: Optional[list[str]] = None,
-        threshold: float = 0,
-        centered: Optional[dict] = None,
-        groups: Optional[Tuple[list, list]] = None,
     ) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
         self.event_index_col = self.__eventstream.schema.event_index
-        self.data = self.__eventstream.to_dataframe()
-        self.max_steps = max_steps
-        self.weight_col = weight_col or self.__eventstream.schema.user_id
-        self.precision = precision
-        self.targets = targets
-        self.accumulated = accumulated
-        self.sorting = sorting
-        self.threshold = threshold
-        self.centered: CenteredParams | None = CenteredParams(**centered) if centered else None
-        self.groups = groups
 
-        self.result_data: pd.DataFrame = pd.DataFrame()
-        self.result_targets: pd.DataFrame | None = None
-        self.fraction_title: str | None = None
-        self.targets_list: list[list[str]] | None = None
+        self.__result_data = pd.DataFrame()
+        self.__result_targets = None
+        self._fraction_title = None
+        self._targets_list = None
 
     def _pad_to_center(self, df_: pd.DataFrame) -> pd.DataFrame | None:
         if self.centered is None:
             return None
 
         center_event = self.centered.event
         occurrence = self.centered.occurrence
@@ -167,15 +104,15 @@
         Parameters
         ----------
         df : pd.Dataframe
 
         Returns
         -------
         pd.Dataframe
-            With columns from 0 to ``max_steps``
+            With columns from 0 to ``max_steps``.
         """
         df = df.copy()
         if max(df.columns) < self.max_steps:  # type: ignore
             for col in range(max(df.columns) + 1, self.max_steps + 1):  # type: ignore
                 df[col] = 0
         # add missing cols if needed:
         if min(df.columns) > 1:  # type: ignore
@@ -391,23 +328,107 @@
             if self.centered is not None:
                 centered_position = self.centered.left_gap
                 axs.vlines(
                     [centered_position - 0.02, centered_position + 0.98], *axs.get_ylim(), colors="Black", linewidth=0.7
                 )
         return axs
 
-    def fit(self) -> None:
+    def fit(
+        self,
+        max_steps: int = 20,
+        weight_col: str | None = None,
+        precision: int = 2,
+        targets: list[str] | str | None = None,
+        accumulated: Literal["both", "only"] | None = None,
+        sorting: list | None = None,
+        threshold: float = 0,
+        centered: dict | None = None,
+        groups: Tuple[list, list] | None = None,
+    ) -> None:
         """
         Calculates the step matrix internal values with the defined parameters.
         Applying ``fit`` method is necessary for the following usage
         of any visualization or descriptive ``StepMatrix`` methods.
 
+        Parameters
+        ----------
+        max_steps : int, default 20
+            Maximum number of steps in ``user path`` to include.
+        weight_col : str, optional
+            Aggregation column for edge weighting. If ``None``, specified ``user_id``
+            from ``eventstream.schema`` will be used. For example, can be specified as
+            ``session_id`` if ``eventstream`` has such ``custom_col``.
+        precision : int, default 2
+            Number of decimal digits after 0 to show as fractions in the ``heatmap``.
+        targets : list of str or str, optional
+            List of event names to include in the bottom of ``step_matrix`` as individual rows.
+            Each specified target will have separate color-coding space for clear visualization.
+            `Example: ['product_page', 'cart', 'payment']`
+
+            If multiple targets need to be compared and plotted using the same color-coding scale,
+            such targets must be combined in a sub-list.
+            `Example: ['product_page', ['cart', 'payment']]`
+        accumulated : {"both", "only"}, optional
+            Option to include accumulated values for targets.
+
+            - If ``None``, accumulated tartes are not shown.
+            - If ``both``, show step values and accumulated values.
+            - If ``only``, show targets only as accumulated.
+        sorting : list of str, optional
+            - If list of event names specified - lines in the heatmap will be shown in
+              the passed order.
+            - If ``None`` - rows will be ordered according to i`th value (first row,
+              where 1st element is max; second row, where second element is max; etc)
+        threshold : float, default 0
+            Used to remove rare events. Aggregates all rows where all values are
+            less than the specified threshold.
+        centered : dict, optional
+            Parameter used to align user paths at a specific event at a specific step.
+            Has to contain three keys:
+            - ``event``: str, name of event to align.
+            - ``left_gap``: int, number of events to include before specified event.
+            - ``occurrence`` : int which occurrence of event to align (typical 1).
+
+            If not ``None`` - only users who have selected events with the specified
+            ``occurrence`` in their paths will be included.
+            ``Fraction`` of such remaining users is specified in the title of centered
+            step_matrix.
+            `Example: {'event': 'cart', 'left_gap': 8, 'occurrence': 1}`
+        groups : tuple[list, list], optional
+            Can be specified to plot differential step_matrix. Must contain
+            a tuple of two elements (g_1, g_2): where g_1 and g_2 are collections
+            of user_id`s. Two separate step_matrices M1 and M2 will be calculated
+            for users from g_1 and g_2, respectively. Resulting matrix will be the matrix
+            M = M1-M2.
+
+        Notes
+        -----
+        During step matrix calculation an artificial ``ENDED`` event is created. If a path already
+        contains ``path_end`` event (See :py:class:`.AddStartEndEvents`), it
+        will be temporarily replaced with ``ENDED`` (within step matrix only). Otherwise, ``ENDED``
+        event will be explicitly added to the end of each path.
+
+        Event ``ENDED`` is cumulated so that the values in its row are summed up from
+        the first step to the last. ``ENDED`` row is always placed at the last line of step matrix.
+        This design guarantees that the sum of any step matrix's column is 1
+        (0 for a differential step matrix).
+
         """
+        self.max_steps = max_steps
+        self.precision = precision
+        self.targets = targets
+        self.accumulated = accumulated
+        self.sorting = sorting
+        self.threshold = threshold
+        self.centered = CenteredParams(**centered) if centered else None
+        self.groups = groups
+        self.weight_col = weight_col or self.__eventstream.schema.user_id
         weight_col = self.weight_col or self.user_col
         data = self.__eventstream.to_dataframe()
+
         data = self._add_ended_events(data=data, schema=self.__eventstream.schema, weight_col=self.weight_col)
         data["event_rank"] = data.groupby(weight_col).cumcount() + 1
 
         # BY HERE WE NEED TO OBTAIN FINAL DIFF piv and piv_targets before sorting, thresholding and plotting:
 
         if self.groups:
             data_pos = data[data[weight_col].isin(self.groups[0])].copy()
@@ -463,45 +484,45 @@
 
         if self.centered:
             window = self.centered.left_gap
             piv.columns = [f"{int(i) - window - 1}" for i in piv.columns]  # type: ignore
             if self.targets and piv_targets is not None:
                 piv_targets.columns = [f"{int(i) - window - 1}" for i in piv_targets.columns]  # type: ignore
 
-        self.result_data = piv
-        self.result_targets = piv_targets
-        self.fraction_title = fraction_title
-        self.targets_list = targets_plot
+        self.__result_data = piv
+        self.__result_targets = piv_targets
+        self._fraction_title = fraction_title
+        self._targets_list = targets_plot
 
     def plot(self) -> matplotlib.axes.Axes:
         """
         Create a heatmap plot based on the calculated step matrix values.
         Should be used after :py:func:`fit`.
 
         Returns
         -------
         matplotlib.axes.Axes
 
         """
-        axes = self._render_plot(self.result_data, self.result_targets, self.targets_list, self.fraction_title)
+        axes = self._render_plot(self.__result_data, self.__result_targets, self._targets_list, self._fraction_title)
         return axes
 
     @property
     def values(self) -> tuple[pd.DataFrame, pd.DataFrame | None]:
         """
         Returns the calculated step matrix as a pd.DataFrame.
         Should be used after :py:func:`fit`.
 
         Returns
         -------
         tuple[pd.DataFrame, pd.DataFrame | None]
             1. Stands for the step matrix.
             2. Stands for a separate step matrix related for target events only.
         """
-        return self.result_data, self.result_targets
+        return self.__result_data, self.__result_targets
 
     @property
     def params(self) -> dict:
         """
         Returns the parameters used for the last fitting.
         Should be used after :py:func:`fit`.
```

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/step_sankey/step_sankey.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/step_sankey/step_sankey.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, Dict, Union
+from typing import Any, Dict
 
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 import seaborn as sns
 
 from retentioneering.eventstream.types import EventstreamType
@@ -14,85 +14,52 @@
 class StepSankey(EndedEventsMixin):
     """
     A class for the visualization of user paths in stepwise manner using Sankey diagram.
 
     Parameters
     ----------
     eventstream : EventstreamType
-    max_steps : int, default 10
-        Maximum number of steps in trajectories to include. Should be > 1.
-    threshold : float | int, default 0.05
-        Used to remove rare events from the plot. An event is collapsed to ``thresholded_N`` artificial event if
-        its maximum frequency across all the steps is less than or equal to ``threshold``. The frequency is set
-        with respect to ``threshold`` type:
-
-        - If ``int`` - the frequency is the number of unique users who had given event at given step.
-        - If ``float`` - percentage of users: the same as for ``int``, but divided by the number of unique users.
-
-        The events which are prohibited for collapsing could be enlisted in ``target`` parameter.
-    sorting : list of str, optional
-        Define the order of the events visualized at each step. The events that are not represented in the list
-        will follow after the events from the list.
-    targets : str or list of str, optional
-        Contain events that are prohibited for collapsing with ``threshold`` parameter.
-    autosize : bool, default True
-        Plotly autosize parameter. See :plotly_autosize:`plotly documentation<>`.
-    width : int, optional
-        Plot's width (in px). See :plotly_width:`plotly documentation<>`.
-    height : int, optional
-        Plot's height (in px). See :plotly_height:`plotly documentation<>`.
-
-    Raises
-    ------
-    ValueError
-        If ``max_steps`` parameter is <= 1.
+
 
     See Also
     --------
     .Eventstream.step_sankey : Call StepSankey tool as an eventstream method.
     .CollapseLoops : Find loops and create new synthetic events in the paths of all users having such sequences.
     .StepMatrix : This class provides methods for step matrix calculation and visualization.
 
     Notes
     -----
     See :doc:`StepSankey user guide</user_guides/step_sankey>` for the details.
 
     """
 
-    def __init__(
-        self,
-        eventstream: EventstreamType,
-        max_steps: int = 10,
-        threshold: Union[int, float] = 0.05,
-        sorting: list | None = None,
-        targets: Union[list[str], str] | None = None,
-        autosize: bool = True,
-        width: int | None = None,
-        height: int | None = None,
-    ) -> None:
+    max_steps: int
+    threshold: int | float
+    sorting: list | None
+    targets: list[str] | str | None
+    autosize: bool
+    width: int | None
+    height: int | None
+
+    data_grp_nodes: pd.DataFrame
+    data: pd.DataFrame
+    data_grp_links: pd.DataFrame
+    data_for_plot: dict
+
+    def __init__(self, eventstream: EventstreamType) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
         self.event_index_col = self.__eventstream.schema.event_index
 
-        self.max_steps = max_steps
-        self.threshold = threshold
-        self.sorting = sorting
-        self.targets = targets
-        self.autosize = autosize
-        self.width = width
-        self.height = height
-
-        self.data_grp_nodes: pd.DataFrame = pd.DataFrame()
-        self.data: pd.DataFrame = pd.DataFrame()
-        self.data_grp_links: pd.DataFrame = pd.DataFrame()
-        self.data_for_plot: dict = {}
-        if max_steps <= 1:
-            raise ValueError("max_steps parameter must be > 1!")
+        self.data_grp_nodes = pd.DataFrame()
+        self.data = pd.DataFrame()
+        self.data_grp_links = pd.DataFrame()
+        self.data_for_plot = {}
 
     @staticmethod
     def _make_color(
         event: str,
         all_events: list,
         palette: list,
     ) -> tuple[int, int, int]:
@@ -535,38 +502,88 @@
         grouped = data.groupby(self.user_col)
         data["next_event"] = grouped[self.event_col].shift(-1)
         data["next_timestamp"] = grouped[self.time_col].shift(-1)
         data["time_to_next"] = data["next_timestamp"] - data[self.time_col]
         data = data.drop("next_timestamp", axis=1)
         return data
 
-    def fit(self) -> None:
+    def fit(
+        self,
+        max_steps: int = 10,
+        threshold: int | float = 0.05,
+        sorting: list | None = None,
+        targets: list[str] | str | None = None,
+    ) -> None:
         """
         Calculate the sankey diagram internal values with the defined parameters.
         Applying ``fit`` method is necessary for the following usage
         of any visualization or descriptive ``StepSankey`` methods.
 
+        Parameters
+        ----------
+        max_steps : int, default 10
+            Maximum number of steps in trajectories to include. Should be > 1.
+        threshold : float | int, default 0.05
+            Used to remove rare events from the plot. An event is collapsed to ``thresholded_N`` artificial event if
+            its maximum frequency across all the steps is less than or equal to ``threshold``. The frequency is set
+            with respect to ``threshold`` type:
+
+            - If ``int`` - the frequency is the number of unique users who had given event at given step.
+            - If ``float`` - percentage of users: the same as for ``int``, but divided by the number of unique users.
+
+            The events which are prohibited for collapsing could be enlisted in ``target`` parameter.
+        sorting : list of str, optional
+            Define the order of the events visualized at each step. The events that are not represented in the list
+            will follow after the events from the list.
+        targets : str or list of str, optional
+            Contain events that are prohibited for collapsing with ``threshold`` parameter.
+
+        Raises
+        ------
+        ValueError
+            If ``max_steps`` parameter is <= 1.
         """
-        data = self.__eventstream.to_dataframe().copy()[
+        data = self.__eventstream.to_dataframe(copy=True)[
             [self.user_col, self.event_col, self.time_col, self.event_index_col]
         ]
+        if max_steps <= 1:
+            raise ValueError("max_steps parameter must be > 1!")
+
+        self.max_steps = max_steps
+        self.threshold = threshold
+        self.sorting = sorting
+        self.targets = targets
+
         self.data = self._prepare_data(data)
         data_for_plot, self.data_grp_nodes = self._get_nodes(self.data)
         self.data_for_plot, self.data_grp_links = self._get_links(self.data, data_for_plot, self.data_grp_nodes)
 
-    def plot(self) -> go.Figure:
+    def plot(self, autosize: bool = True, width: int | None = None, height: int | None = None) -> go.Figure:
         """
         Create a Sankey interactive plot based on the calculated values.
         Should be used after :py:func:`fit`.
 
+        Parameters
+        ----------
+        autosize : bool, default True
+            Plotly autosize parameter. See :plotly_autosize:`plotly documentation<>`.
+        width : int, optional
+            Plot's width (in px). See :plotly_width:`plotly documentation<>`.
+        height : int, optional
+            Plot's height (in px). See :plotly_height:`plotly documentation<>`.
+
         Returns
         -------
         plotly.graph_objects.Figure
 
         """
+
+        self.autosize = autosize
+        self.width = width
+        self.height = height
         figure = self._render_plot(self.data_for_plot, self.data_grp_nodes)
         return figure
 
     @property
     def values(self) -> tuple[pd.DataFrame, pd.DataFrame]:
         """
         Returns two pd.DataFrames which the Sankey diagram is based on.
```

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/timedelta_hist/timedelta_hist.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/timedelta_hist/timedelta_hist.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,73 +22,17 @@
     """
     Plot the distribution of the time deltas between two events. Support various
     distribution types, such as distribution of time for adjacent consecutive events, or
     for a pair of pre-defined events, or median transition time from event to event per user/session.
 
     Parameters
     ----------
-    raw_events_only : bool, default True
-        If ``True`` - statistics will be shown only for raw events.
-        If ``False`` - statistics will be shown for all events presented in your data.
-    event_pair : tuple of str, optional
-        Specify an event pair to plot the time distance between. The first
-        item corresponds to chronologically first event, the second item corresponds to the second event. If
-        ``event_pair=None``, plot distribution of timedelta for all adjacent events.
-
-        Examples: ('login', 'purchase'); ['start', 'cabinet']
-
-        Besides the generic eventstream events, ``event_pair`` can accept special ``eventstream_start`` and
-        ``eventstream_end`` events which denote the first and the last event in the entire eventstream correspondingly.
-
-        Note that the sequence of events and ``weight_col`` is important.
-
-    adjacent_events_only : bool, default True
-        Is used only when ``event_pair`` is not ``None``; specifies whether events need to be
-        adjacent to be included.
-
-        For example, if ``event_pair=("login", "purchase")`` and ``adjacent_events_only=False``,
-        then the sequence ("login", "main", "trading", "purchase") will contain a valid pair
-        (which is not the case with ``adjacent_events_only=True``).
-
-    weight_col : str, default None
-        Specify a unit of observation, inside which time differences will be computed.
-        By default, the values from ``user_id`` column in :py:class:`.EventstreamSchema` is taken.
-
-        For example:
-
-        - If ``user_id`` - time deltas will be computed only for events inside each user path.
-        - If ``session_id`` - the same, but inside each session.
-
-    time_agg : {None, "mean", "median"}, default None
-        Specify the aggregation policy for the time distances. Aggregate based on passed ``weight_col``.
-
-        - If ``None`` - no aggregation;
-        - ``mean`` and ``median`` plot distributions of ``weight_col`` unit mean or unit ``median`` timedeltas.
-
-        For example, if session id is specified in ``weight_col``, one observation per
-        session (for example, session median) will be provided for the histogram.
-    timedelta_unit : :numpy_link:`DATETIME_UNITS<>`, default 's'
-        Specify units of time differences the histogram should use. Use "s" for seconds, "m" for minutes,
-        "h" for hours and "D" for days.
-    log_scale: bool | tuple of bool | None, optional
-
-         - If ``True`` - apply log scaling to the ``x`` axis.
-         - If tuple of bool - apply log scaling to the (``x``,``y``) axes correspondingly.
-
-    lower_cutoff_quantile : float, optional
-        Specify time distance quantile as the lower boundary. The values below the boundary are truncated.
-    upper_cutoff_quantile : float, optional
-        Specify time distance quantile as the upper boundary. The values above the boundary are truncated.
-    bins : int or {"auto", "fd", "doane", "scott", "stone", "rice", "sturges", "sqrt"}, default 20
-        Generic bin parameter that can be the name of a reference rule or
-        the number of bins. Passed to :numpy_bins_link:`numpy.histogram_bin_edges<>`.
-    width : float, default 6.0
-        Width in inches.
-    height : float, default 4.5
-        Height in inches.
+    eventstream : EventstreamType
+
+
 
     See Also
     --------
     .UserLifetimeHist : Plot the distribution of user lifetimes.
     .EventTimestampHist : Plot the distribution of events over time.
     .Eventstream.describe : Show general eventstream statistics.
     .Eventstream.describe_events : Show general eventstream events statistics.
@@ -103,85 +47,36 @@
     -----
     See :ref:`Eventstream user guide<eventstream_timedelta_hist>` for the details.
     """
 
     EVENTSTREAM_START = "eventstream_start"
     EVENTSTREAM_END = "eventstream_end"
 
-    def __init__(
-        self,
-        eventstream: EventstreamType,
-        raw_events_only: bool = False,
-        event_pair: Optional[list[str | EVENTSTREAM_GLOBAL_EVENTS]] = None,
-        adjacent_events_only: bool = True,
-        weight_col: str | None = None,
-        time_agg: Optional[AGGREGATION_NAMES] = None,
-        timedelta_unit: DATETIME_UNITS = "s",
-        log_scale: bool | tuple[bool, bool] | None = None,
-        lower_cutoff_quantile: Optional[float] = None,
-        upper_cutoff_quantile: Optional[float] = None,
-        bins: int | Literal[BINS_ESTIMATORS] = 20,
-        width: float = 6.0,
-        height: float = 4.5,
-    ) -> None:
+    __eventstream: EventstreamType
+    raw_events_only: bool
+    event_pair: list[str | EVENTSTREAM_GLOBAL_EVENTS] | None
+    adjacent_events_only: bool
+    weight_col: str | None
+    time_agg: AGGREGATION_NAMES | None
+    timedelta_unit: DATETIME_UNITS
+    log_scale: bool | tuple[bool, bool] | None
+    lower_cutoff_quantile: float | None
+    upper_cutoff_quantile: float | None
+    bins: int | Literal[BINS_ESTIMATORS]
+    bins_to_show: np.ndarray
+    values_to_plot: np.ndarray
+
+    def __init__(self, eventstream: EventstreamType) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
         self.type_col = self.__eventstream.schema.event_type
-        self.raw_events_only = raw_events_only
-
-        if event_pair is not None:
-            if type(event_pair) not in (list, tuple):
-                raise TypeError("event_pair should be a tuple or a list of length 2.")
-            if len(event_pair) != 2:
-                raise ValueError("event_pair should be a tuple or a list of length 2.")
-
-            if set(event_pair) == {self.EVENTSTREAM_START, self.EVENTSTREAM_END}:
-                raise ValueError(
-                    f"event_pair = ['{self.EVENTSTREAM_START}', '{self.EVENTSTREAM_END}'] "
-                    f"is invalid. Only one event of these two events can be a member of the event_pair."
-                )
-            if set(event_pair) in [{self.EVENTSTREAM_START}, {self.EVENTSTREAM_END}]:
-                raise ValueError(
-                    f"event_pair = ['{self.EVENTSTREAM_START}', '{self.EVENTSTREAM_END}'] and "
-                    f"event_pair = ['{self.EVENTSTREAM_START}', '{self.EVENTSTREAM_END}'] "
-                    f"are invalid. Events '{self.EVENTSTREAM_START}' "
-                    f"and '{self.EVENTSTREAM_END}' couldn't be doubled."
-                )
-
-        self.event_pair = event_pair
-        self.adjacent_events_only = adjacent_events_only
-        self.weight_col = weight_col or self.__eventstream.schema.user_id
-
-        self.time_agg = time_agg
-        self.timedelta_unit = timedelta_unit
-        if lower_cutoff_quantile is not None:
-            if not 0 < lower_cutoff_quantile < 1:
-                raise ValueError("lower_cutoff_quantile should be a fraction between 0 and 1.")
-        self.lower_cutoff_quantile = lower_cutoff_quantile
-        if upper_cutoff_quantile is not None:
-            if not 0 < upper_cutoff_quantile < 1:
-                raise ValueError("upper_cutoff_quantile should be a fraction between 0 and 1.")
-        self.upper_cutoff_quantile = upper_cutoff_quantile
-        if lower_cutoff_quantile is not None and upper_cutoff_quantile is not None:
-            if lower_cutoff_quantile > upper_cutoff_quantile:
-                warnings.warn("lower_cutoff_quantile exceeds upper_cutoff_quantile; no data passed to the histogram")
-
-        if log_scale:
-            if isinstance(log_scale, bool):
-                self.log_scale = (log_scale, False)
-            else:
-                self.log_scale = log_scale
-        else:
-            self.log_scale = (False, False)
-        self.bins = bins
-        self.figsize = (width, height)
-        self.bins_to_show: np.ndarray = np.array([])
-        self.values_to_plot: np.ndarray = np.array([])
+        self.bins_to_show = np.array([])
+        self.values_to_plot = np.array([])
 
     def _prepare_time_diff(self, data: pd.DataFrame) -> pd.DataFrame:
         if not self.adjacent_events_only:
             data = data[data[self.event_col].isin(self.event_pair)]  # type: ignore
 
         weight_col_group = data.groupby([self.weight_col])
         with pd.option_context("mode.chained_assignment", None):
@@ -214,26 +109,136 @@
             global_event = self.EVENTSTREAM_END
 
         global_events = data.groupby([self.weight_col]).first().reset_index().copy()
         global_events[self.time_col] = global_event_time
         global_events[self.event_col] = global_event
 
         data = data[data[self.event_col].isin(self.event_pair)].copy()  # type: ignore
-        data = pd.concat([data, global_events]).sort_values([self.weight_col, self.time_col]).reset_index(drop=True)
+        data = pd.concat([data, global_events]).sort_values([self.weight_col, self.time_col]).reset_index(drop=True)  # type: ignore
         return data
 
-    def fit(self) -> None:
+    def __validate_input(
+        self,
+        log_scale: bool | tuple[bool, bool] | None = None,
+        lower_cutoff_quantile: float | None = None,
+        upper_cutoff_quantile: float | None = None,
+    ) -> tuple[tuple[bool, bool], float | None, float | None]:
+        if lower_cutoff_quantile is not None:
+            if not 0 < lower_cutoff_quantile < 1:
+                raise ValueError("lower_cutoff_quantile should be a fraction between 0 and 1.")
+
+        if upper_cutoff_quantile is not None:
+            if not 0 < upper_cutoff_quantile < 1:
+                raise ValueError("upper_cutoff_quantile should be a fraction between 0 and 1.")
+
+        if lower_cutoff_quantile is not None and upper_cutoff_quantile is not None:
+            if lower_cutoff_quantile > upper_cutoff_quantile:
+                warnings.warn("lower_cutoff_quantile exceeds upper_cutoff_quantile; no data passed to the histogram")
+
+        if log_scale:
+            if isinstance(log_scale, bool):
+                log_scale = (log_scale, False)
+            else:
+                log_scale = log_scale
+        else:
+            log_scale = (False, False)
+
+        return log_scale, upper_cutoff_quantile, lower_cutoff_quantile
+
+    def fit(
+        self,
+        raw_events_only: bool = False,
+        event_pair: Optional[list[str | EVENTSTREAM_GLOBAL_EVENTS]] = None,
+        adjacent_events_only: bool = True,
+        weight_col: str | None = None,
+        time_agg: Optional[AGGREGATION_NAMES] = None,
+        timedelta_unit: DATETIME_UNITS = "s",
+        log_scale: bool | tuple[bool, bool] | None = None,
+        lower_cutoff_quantile: Optional[float] = None,
+        upper_cutoff_quantile: Optional[float] = None,
+        bins: int | Literal[BINS_ESTIMATORS] = 20,
+    ) -> None:
         """
         Calculate values and bins for the histplot.
 
+        Parameters
+        ----------
+        raw_events_only : bool, default True
+            If ``True`` - statistics will be shown only for raw events.
+            If ``False`` - statistics will be shown for all events presented in your data.
+        event_pair : tuple of str, optional
+            Specify an event pair to plot the time distance between. The first
+            item corresponds to chronologically first event, the second item corresponds to the second event. If
+            ``event_pair=None``, plot distribution of timedelta for all adjacent events.
+
+            Examples: ('login', 'purchase'); ['start', 'cabinet']
+
+            Besides the generic eventstream events, ``event_pair`` can accept special ``eventstream_start`` and
+            ``eventstream_end`` events which denote the first and the last event in the entire eventstream correspondingly.
+
+            Note that the sequence of events and ``weight_col`` is important.
+
+        adjacent_events_only : bool, default True
+            Is used only when ``event_pair`` is not ``None``; specifies whether events need to be
+            adjacent to be included.
+
+            For example, if ``event_pair=("login", "purchase")`` and ``adjacent_events_only=False``,
+            then the sequence ("login", "main", "trading", "purchase") will contain a valid pair
+            (which is not the case with ``adjacent_events_only=True``).
+
+        weight_col : str, default None
+            Specify a unit of observation, inside which time differences will be computed.
+            By default, the values from ``user_id`` column in :py:class:`.EventstreamSchema` is taken.
+
+            For example:
+
+            - If ``user_id`` - time deltas will be computed only for events inside each user path.
+            - If ``session_id`` - the same, but inside each session.
+
+        time_agg : {None, "mean", "median"}, default None
+            Specify the aggregation policy for the time distances. Aggregate based on passed ``weight_col``.
+
+            - If ``None`` - no aggregation;
+            - ``mean`` and ``median`` plot distributions of ``weight_col`` unit mean or unit ``median`` timedeltas.
+
+            For example, if session id is specified in ``weight_col``, one observation per
+            session (for example, session median) will be provided for the histogram.
+        timedelta_unit : :numpy_link:`DATETIME_UNITS<>`, default 's'
+            Specify units of time differences the histogram should use. Use "s" for seconds, "m" for minutes,
+            "h" for hours and "D" for days.
+        log_scale: bool | tuple of bool | None, optional
+
+             - If ``True`` - apply log scaling to the ``x`` axis.
+             - If tuple of bool - apply log scaling to the (``x``,``y``) axes correspondingly.
+
+        lower_cutoff_quantile : float, optional
+            Specify time distance quantile as the lower boundary. The values below the boundary are truncated.
+        upper_cutoff_quantile : float, optional
+            Specify time distance quantile as the upper boundary. The values above the boundary are truncated.
+        bins : int or {"auto", "fd", "doane", "scott", "stone", "rice", "sturges", "sqrt"}, default 20
+            Generic bin parameter that can be the name of a reference rule or
+            the number of bins. Passed to :numpy_bins_link:`numpy.histogram_bin_edges<>`.
+
         Returns
         -------
         None
         """
 
+        self.log_scale, self.upper_cutoff_quantile, self.lower_cutoff_quantile = self.__validate_input(
+            log_scale, lower_cutoff_quantile, upper_cutoff_quantile
+        )
+
+        self.raw_events_only = raw_events_only
+        self.event_pair = event_pair
+        self.adjacent_events_only = adjacent_events_only
+        self.weight_col = weight_col or self.__eventstream.schema.user_id
+        self.time_agg = time_agg
+        self.timedelta_unit = timedelta_unit
+        self.bins = bins
+
         data = self.__eventstream.to_dataframe(copy=True)
 
         if self.raw_events_only:
             data = data[data[self.type_col].isin(["raw"])]
         data = data.sort_values([self.weight_col, self.time_col])
 
         if self.event_pair is not None and set([self.EVENTSTREAM_START, self.EVENTSTREAM_END]).intersection(
@@ -267,25 +272,32 @@
         tuple(np.ndarray, np.ndarray)
 
             1. The first array contains the values for histogram.
             2. The first array contains the bin edges.
         """
         return self.values_to_plot, self.bins_to_show
 
-    def plot(self) -> matplotlib.axes.Axes:
+    def plot(self, width: float = 6.0, height: float = 4.5) -> matplotlib.axes.Axes:
         """
         Create a sns.histplot based on the calculated values.
 
+        Parameters
+        ----------
+
+        width : float, default 6.0
+            Width in inches.
+        height : float, default 4.5
+            Height in inches.
         Returns
         -------
         :matplotlib_axes:`matplotlib.axes.Axes<>`
             The matplotlib axes containing the plot.
         """
-
-        plt.subplots(figsize=self.figsize)
+        figsize = (width, height)
+        plt.subplots(figsize=figsize)
 
         hist = sns.histplot(self.values_to_plot, bins=self.bins, log_scale=self.log_scale)
         hist.set_title(
             f"Timedelta histogram, event pair - {self.event_pair}, weight column - {self.weight_col}"
             f"{', group - ' + self.time_agg if self.time_agg is not None else ''}"
         )
         hist.set_xlabel(f"Time units: {self.timedelta_unit}")
```

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/transition_graph/transition_graph.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/transition_graph/transition_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import copy
 import json
 import random
 import string
+import warnings
 from typing import Any, Dict, List, MutableMapping, MutableSequence, Union, cast
 
 import networkx as nx
 import pandas as pd
 from IPython.core.display import HTML, display
 
 from retentioneering.backend import ServerManager
@@ -55,46 +56,43 @@
     -----
     See :doc:`transition graph user guide</user_guides/transition_graph>` for the details.
 
     """
 
     _weights: MutableMapping[str, str] | None = None
     _edges_norm_type: NormType = None
+    _nodes_norm_type: NormType = None
     _nodes_threshold: Threshold
     _edges_threshold: Threshold
 
     @property
     def nodes_thresholds(self) -> Threshold:
         return self._nodes_threshold
 
     @nodes_thresholds.setter
     def nodes_thresholds(self, value: Threshold) -> None:
-        if self._check_thresholds_for_norm_type(value):
+        if self._check_thresholds_for_norm_type(value=value, norm_type=self.nodes_norm_type):
             self._nodes_threshold = value
 
     @property
     def edges_thresholds(self) -> Threshold:
         return self._edges_threshold
 
     @edges_thresholds.setter
     def edges_thresholds(self, value: Threshold) -> None:
-        if self._check_thresholds_for_norm_type(value):
+        if self._check_thresholds_for_norm_type(value=value, norm_type=self.edges_norm_type):
             self._edges_threshold = value
 
-    def _check_thresholds_for_norm_type(self, value: Threshold) -> bool:
-        if self.edges_norm_type is None:
+    def _check_thresholds_for_norm_type(self, value: Threshold, norm_type: NormType) -> bool:
+        if norm_type is None:
             if not all(map(lambda x: x is None or x >= 0, value.values())):
-                raise ValueError(
-                    f"For normalization type {self.edges_norm_type} all thresholds must be positive or None"
-                )
+                raise ValueError(f"For normalization type {norm_type} all thresholds must be positive or None")
         else:
             if not all(map(lambda x: x is None or 0 <= x <= 1, value.values())):
-                raise ValueError(
-                    f"For normalization type {self.edges_norm_type} all thresholds must be between 0 and 1 or None"
-                )
+                raise ValueError(f"For normalization type {norm_type} all thresholds must be between 0 and 1 or None")
 
         return True
 
     @track(  # type: ignore
         tracking_info={"event_name": "transition_graph", "event_custom_name": "transition_graph_init"},
     )
     def __init__(
@@ -164,14 +162,24 @@
     def edges_norm_type(self, edges_norm_type: NormType) -> None:  # type: ignore
         allowed_edges_norm_types: list[str | None] = [None, "full", "node"]
         if edges_norm_type in allowed_edges_norm_types:
             self._edges_norm_type = edges_norm_type
         else:
             raise ValueError("Norm type should be one of: %s" % allowed_edges_norm_types)
 
+    @property
+    def nodes_norm_type(self) -> NormType:  # type: ignore
+        return self._nodes_norm_type
+
+    @nodes_norm_type.setter
+    def nodes_norm_type(self, nodes_norm_type: NormType) -> None:  # type: ignore
+        if nodes_norm_type is not None:
+            warnings.warn(f"Currently nodes_norm_type allowed to be None only")
+        self._nodes_norm_type = None
+
     def _on_recalc_request(
         self, rename_rules: list[RenameRule]
     ) -> dict[str, MutableSequence[PreparedNode] | MutableSequence[PreparedLink] | list]:
         try:
             self._recalculate(rename_rules=rename_rules)
 
             nodes, nodes_set = self._prepare_nodes(
@@ -557,14 +565,15 @@
         ],
     )
     def plot(
         self,
         targets: MutableMapping[str, str | None] | None = None,
         edges_norm_type: NormType | None = None,
         nodes_threshold: Threshold | None = None,
+        nodes_norm_type: NormType | None = None,
         edges_threshold: Threshold | None = None,
         nodes_weight_col: str | None = None,
         edges_weight_col: str | None = None,
         custom_weight_cols: list[str] | None = None,
         width: int = 960,
         height: int = 900,
         show_weights: bool = True,
@@ -584,14 +593,17 @@
 
             - If ``None``, normalization is not used, the absolute values are taken.
             - If ``full``, normalization across the whole eventstream.
             - If ``node``, normalization across each node (or outgoing transitions from each node).
 
             See :ref:`Transition graph user guide <transition_graph_weights>` for the details.
 
+        nodes_norm_type: {"full", "node", None}, default None
+            Currently not implemented. Always None.
+
         edges_weight_col: str, optional
             A column name from the :py:class:`.EventstreamSchema` which values will control the final
             edges' weights and displayed width as well.
 
             For each edge is calculated:
 
             - If ``None`` or ``event_id`` - the number of transitions.
@@ -682,21 +694,22 @@
         1. If all the edges connected to a node are hidden, the node becomes hidden as well.
            In order to avoid it - use ``show_nodes_without_links=True`` parameter in code or in the interface.
         2. The thresholds may use their own weighting columns both for nodes and for edges independently
            of weighting columns defined in ``edges_weight_col`` and ``nodes_weight_col`` arguments.
 
         See :doc:`TransitionGraph user guide </user_guides/transition_graph>` for the details.
         """
-        if not edges_norm_type and show_percents:
+        if edges_norm_type is None and show_percents:
             raise ValueError("If show_percents=True, edges_norm_type should be 'full' or 'node'!")
 
         self.__prepare_graph_for_plot(
             edges_weight_col=edges_weight_col,
             edges_threshold=edges_threshold,
             edges_norm_type=edges_norm_type,
+            nodes_norm_type=nodes_norm_type,
             nodes_weight_col=nodes_weight_col,
             nodes_threshold=nodes_threshold,
             targets=targets,
             custom_weight_cols=custom_weight_cols,
         )
 
         norm_nodes_threshold = (
@@ -723,15 +736,14 @@
             height=height,
         )
 
         shown_nodes_col = self.nodes_weight_col
         shown_links_weight = self.edges_weight_col
         selected_nodes_col_for_thresholds = shown_nodes_col
         selected_links_weight_for_thresholds = shown_links_weight
-
         init_graph_js = self.render.init(
             **dict(
                 server_id=self.server.pk,
                 env=self.env,
                 norm_type=self._edges_norm_type_to_json_value(self.edges_norm_type),
                 links=self._to_json_links(links),
                 nodes=self._to_json(nodes),
@@ -819,14 +831,15 @@
     def __prepare_graph_for_plot(
         self,
         edges_weight_col: str | None = None,
         edges_threshold: Threshold | None = None,
         nodes_weight_col: str | None = None,
         nodes_threshold: Threshold | None = None,
         edges_norm_type: NormType | None = None,
+        nodes_norm_type: NormType | None = None,
         targets: MutableMapping[str, str | None] | None = None,
         custom_weight_cols: list[str] | None = None,
     ) -> None:
         if targets:
             self.targets = targets
         self.edges_norm_type = edges_norm_type
         if nodes_threshold is None:
@@ -838,22 +851,22 @@
         self.nodelist_default_col = self.eventstream.schema.event_id
         self.edgelist_default_col = self.eventstream.schema.event_id
         self.targets = targets if targets else {"positive": None, "negative": None, "source": None}
         self.weight_cols = self._define_weight_cols(custom_weight_cols)
         self.nodes_weight_col = nodes_weight_col if nodes_weight_col else self.eventstream.schema.event_id
         self.edges_weight_col = edges_weight_col if edges_weight_col else self.eventstream.schema.event_id
 
-        self.edges_weight_col = self.eventstream.schema.event_id
-        self.edges_norm_type: NormType | None = edges_norm_type
+        self.nodes_norm_type = nodes_norm_type
         self.nodelist: Nodelist = Nodelist(
             weight_cols=self.weight_cols,
             time_col=self.event_time_col,
             event_col=self.event_col,
         )
         self.nodelist.calculate_nodelist(data=self.eventstream.to_dataframe())
+        self.edges_norm_type: NormType | None = edges_norm_type
         self.edgelist: Edgelist = Edgelist(eventstream=self.eventstream)
         self.edgelist.calculate_edgelist(
             weight_cols=self.weight_cols,
             norm_type=self.edges_norm_type,
         )
 
     def _get_option(self, name: str, settings: dict[str, Any]) -> str:
```

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/typing/transition_graph/graph_types.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/typing/transition_graph/graph_types.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/tooling/user_lifetime_hist/user_lifetime_hist.py` & `retentioneering-3.0.0rc1/retentioneering/tooling/user_lifetime_hist/user_lifetime_hist.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import warnings
-from typing import Literal, Optional
+from typing import Literal
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 
@@ -18,34 +18,15 @@
     """
 
     Plot the distribution of user lifetimes. A ``users lifetime`` is the timedelta between
     the first and the last events of the user.
 
     Parameters
     ----------
-    timedelta_unit : :numpy_link:`DATETIME_UNITS<>`, default 's'
-        Specify units of time differences the histogram should use. Use "s" for seconds, "m" for minutes,
-        "h" for hours and "D" for days.
-    log_scale : bool or tuple of bool, optional
-
-        - If ``True`` - apply log scaling to the ``x`` axis.
-        - If tuple of bool - apply log scaling to the (``x``,``y``) axes correspondingly.
-    lower_cutoff_quantile : float, optional
-        Specify time distance quantile as the lower boundary. The values below the boundary are truncated.
-    upper_cutoff_quantile : float, optional
-        Specify time distance quantile as the upper boundary. The values above the boundary are truncated.
-    bins : int or str, default 20
-        Generic bin parameter that can be the name of a reference rule or
-        the number of bins. Passed to :numpy_bins_link:`numpy.histogram_bin_edges<>`.
-    width : float, default 6.0
-        Width in inches.
-    height : float, default 4.5
-        Height in inches.
-
-
+    eventstream : EventstreamType
 
     See Also
     --------
     .EventTimestampHist : Plot the distribution of events over time.
     .TimedeltaHist : Plot the distribution of the time deltas between two events.
     .Eventstream.describe : Show general eventstream statistics.
     .Eventstream.describe_events : Show general eventstream events statistics.
@@ -54,72 +35,110 @@
 
     Notes
     -----
     See :ref:`Eventstream user guide<eventstream_user_lifetime>` for the details.
 
     """
 
-    def __init__(
-        self,
-        eventstream: EventstreamType,
-        timedelta_unit: DATETIME_UNITS = "s",
-        log_scale: bool | tuple[bool, bool] | None = None,
-        lower_cutoff_quantile: Optional[float] = None,
-        upper_cutoff_quantile: Optional[float] = None,
-        bins: int | Literal[BINS_ESTIMATORS] = 20,
-        width: float = 6.0,
-        height: float = 4.5,
-    ) -> None:
+    __eventstream: EventstreamType
+    timedelta_unit: DATETIME_UNITS
+    log_scale: bool | tuple[bool, bool] | None
+    lower_cutoff_quantile: float | None
+    upper_cutoff_quantile: float | None
+    bins: int | Literal[BINS_ESTIMATORS]
+    bins_to_show: np.ndarray
+    values_to_plot: np.ndarray
+
+    def __init__(self, eventstream: EventstreamType) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
-        self.timedelta_unit = timedelta_unit
+
+        self.bins_to_show = np.array([])
+        self.values_to_plot = np.array([])
+
+    def _remove_cutoff_values(self, series: pd.Series) -> pd.Series:
+        idx = [True] * len(series)
+        if self.upper_cutoff_quantile is not None:
+            idx &= series <= series.quantile(self.upper_cutoff_quantile)
+        if self.lower_cutoff_quantile is not None:
+            idx &= series >= series.quantile(self.lower_cutoff_quantile)
+        return series[idx]
+
+    def __validate_input(
+        self,
+        log_scale: bool | tuple[bool, bool] | None = None,
+        lower_cutoff_quantile: float | None = None,
+        upper_cutoff_quantile: float | None = None,
+    ) -> tuple[tuple[bool, bool], float | None, float | None]:
         if lower_cutoff_quantile is not None:
             if not 0 < lower_cutoff_quantile < 1:
                 raise ValueError("lower_cutoff_quantile should be a fraction between 0 and 1.")
-        self.lower_cutoff_quantile = lower_cutoff_quantile
+
         if upper_cutoff_quantile is not None:
             if not 0 < upper_cutoff_quantile < 1:
                 raise ValueError("upper_cutoff_quantile should be a fraction between 0 and 1.")
-        self.upper_cutoff_quantile = upper_cutoff_quantile
+
         if lower_cutoff_quantile is not None and upper_cutoff_quantile is not None:
             if lower_cutoff_quantile > upper_cutoff_quantile:
                 warnings.warn("lower_cutoff_quantile exceeds upper_cutoff_quantile; no data passed to the histogram")
 
         if log_scale:
             if isinstance(log_scale, bool):
-                self.log_scale = (log_scale, False)
+                log_scale = (log_scale, False)
             else:
-                self.log_scale = log_scale
+                log_scale = log_scale
         else:
-            self.log_scale = (False, False)
+            log_scale = (False, False)
 
-        self.bins = bins
-        self.figsize = (width, height)
-        self.bins_to_show: np.ndarray = np.array([])
-        self.values_to_plot: np.ndarray = np.array([])
+        return log_scale, upper_cutoff_quantile, lower_cutoff_quantile
 
-    def _remove_cutoff_values(self, series: pd.Series) -> pd.Series:
-        idx = [True] * len(series)
-        if self.upper_cutoff_quantile is not None:
-            idx &= series <= series.quantile(self.upper_cutoff_quantile)
-        if self.lower_cutoff_quantile is not None:
-            idx &= series >= series.quantile(self.lower_cutoff_quantile)
-        return series[idx]
-
-    def fit(self) -> None:
+    def fit(
+        self,
+        timedelta_unit: DATETIME_UNITS = "s",
+        log_scale: bool | tuple[bool, bool] | None = None,
+        lower_cutoff_quantile: float | None = None,
+        upper_cutoff_quantile: float | None = None,
+        bins: int | Literal[BINS_ESTIMATORS] = 20,
+    ) -> None:
         """
         Calculate values for the histplot.
 
+        Parameters
+        ----------
+        timedelta_unit : :numpy_link:`DATETIME_UNITS<>`, default 's'
+            Specify units of time differences the histogram should use. Use "s" for seconds, "m" for minutes,
+            "h" for hours and "D" for days.
+        log_scale : bool or tuple of bool, optional
+
+            - If ``True`` - apply log scaling to the ``x`` axis.
+            - If tuple of bool - apply log scaling to the (``x``,``y``) axes correspondingly.
+        lower_cutoff_quantile : float, optional
+            Specify time distance quantile as the lower boundary. The values below the boundary are truncated.
+        upper_cutoff_quantile : float, optional
+            Specify time distance quantile as the upper boundary. The values above the boundary are truncated.
+        bins : int or str, default 20
+            Generic bin parameter that can be the name of a reference rule or
+            the number of bins. Passed to :numpy_bins_link:`numpy.histogram_bin_edges<>`.
+
         Returns
         -------
         None
         """
-        data = self.__eventstream.to_dataframe().groupby(self.user_col)[self.time_col].agg(["min", "max"])
+        self.log_scale, self.upper_cutoff_quantile, self.lower_cutoff_quantile = self.__validate_input(
+            log_scale,
+            lower_cutoff_quantile,
+            upper_cutoff_quantile,
+        )
+
+        self.timedelta_unit = timedelta_unit
+        self.bins = bins
+
+        data = self.__eventstream.to_dataframe(copy=True).groupby(self.user_col)[self.time_col].agg(["min", "max"])
         data["time_passed"] = data["max"] - data["min"]
         values_to_plot = (data["time_passed"] / np.timedelta64(1, self.timedelta_unit)).reset_index(  # type: ignore
             drop=True
         )
 
         if self._remove_cutoff_values:  # type: ignore
             values_to_plot = self._remove_cutoff_values(values_to_plot).to_numpy()
@@ -144,24 +163,33 @@
         tuple(np.ndarray, np.ndarray)
             1. The first array contains the values for histogram.
             2. The first array contains the bin edges.
 
         """
         return self.values_to_plot, self.bins_to_show
 
-    def plot(self) -> matplotlib.axes.Axes:
+    def plot(self, width: float = 6.0, height: float = 4.5) -> matplotlib.axes.Axes:
         """
         Create a sns.histplot based on the calculated values.
 
+        Parameters
+        ----------
+        width : float, default 6.0
+            Width in inches.
+        height : float, default 4.5
+            Height in inches.
+
         Returns
         -------
         :matplotlib_axes:`matplotlib.axes.Axes<>`
             The matplotlib axes containing the plot.
 
         """
-        plt.subplots(figsize=self.figsize)
+
+        figsize = (width, height)
+        plt.subplots(figsize=figsize)
 
         hist = sns.histplot(self.values_to_plot, bins=self.bins, log_scale=self.log_scale)
         hist.set_title("User lifetime histogram")
         hist.set_xlabel(f"Time units: {self.timedelta_unit}")
 
         return hist
```

### Comparing `retentioneering-3.0.0b2/retentioneering/utils/registry.py` & `retentioneering-3.0.0rc1/retentioneering/utils/registry.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/retentioneering/widget/widgets.py` & `retentioneering-3.0.0rc1/retentioneering/widget/widgets.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b2/PKG-INFO` & `retentioneering-3.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retentioneering
-Version: 3.0.0b2
+Version: 3.0.0rc1
 Summary: universal framework for data processing
 Author: Retentioneering User Trajectory Analysis Lab
 Author-email: you@example.com
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

