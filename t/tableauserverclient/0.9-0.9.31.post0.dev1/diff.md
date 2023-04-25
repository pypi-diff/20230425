# Comparing `tmp/tableauserverclient-0.9.tar.gz` & `tmp/tableauserverclient-0.9.31.post0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tableauserverclient-0.9.tar", last modified: Fri Oct  4 21:26:13 2019, max compression
+gzip compressed data, was "tableauserverclient-0.9.31.post0.dev1.tar", last modified: Tue Mar 29 23:49:06 2022, max compression
```

## Comparing `tableauserverclient-0.9.tar` & `tableauserverclient-0.9.31.post0.dev1.tar`

### file list

```diff
@@ -1,116 +1,330 @@
-drwxr-xr-x   0 rhay     (1469294935) TSI\Domain Users (62064481)        0 2019-10-04 21:26:13.000000 tableauserverclient-0.9/
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      292 2019-10-04 21:26:13.000000 tableauserverclient-0.9/PKG-INFO
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     1074 2019-04-08 17:10:19.000000 tableauserverclient-0.9/LICENSE
-drwxr-xr-x   0 rhay     (1469294935) TSI\Domain Users (62064481)        0 2019-10-04 21:26:13.000000 tableauserverclient-0.9/test/
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     2246 2019-04-08 17:10:19.000000 tableauserverclient-0.9/test/test_site_model.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     2019 2019-04-08 17:10:19.000000 tableauserverclient-0.9/test/test_job.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      705 2019-04-08 17:10:19.000000 tableauserverclient-0.9/test/test_regression_tests.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4200 2019-10-04 21:26:02.000000 tableauserverclient-0.9/test/test_database.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     3278 2019-04-08 17:10:19.000000 tableauserverclient-0.9/test/test_task.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     7219 2019-04-08 17:10:19.000000 tableauserverclient-0.9/test/test_user.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     3849 2019-04-08 17:10:19.000000 tableauserverclient-0.9/test/test_pager.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     2880 2019-04-08 17:10:19.000000 tableauserverclient-0.9/test/test_server_info.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     9833 2019-04-08 17:10:19.000000 tableauserverclient-0.9/test/test_group.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4546 2019-10-04 21:26:02.000000 tableauserverclient-0.9/test/test_auth.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      427 2019-04-08 17:10:19.000000 tableauserverclient-0.9/test/test_group_model.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     2687 2019-10-04 21:26:02.000000 tableauserverclient-0.9/test/test_table.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     6237 2019-10-04 21:26:02.000000 tableauserverclient-0.9/test/test_flow.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)    27849 2019-10-04 21:26:02.000000 tableauserverclient-0.9/test/test_workbook.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)    20625 2019-10-04 21:26:02.000000 tableauserverclient-0.9/test/test_datasource.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     2752 2019-10-04 21:26:02.000000 tableauserverclient-0.9/test/test_metadata.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      785 2019-04-08 17:10:19.000000 tableauserverclient-0.9/test/test_project_model.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     5237 2019-10-04 21:26:02.000000 tableauserverclient-0.9/test/test_sort.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)    13059 2019-04-08 17:32:53.000000 tableauserverclient-0.9/test/test_schedule.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     2852 2019-04-08 17:32:53.000000 tableauserverclient-0.9/test/test_requests.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     9672 2019-10-04 21:26:02.000000 tableauserverclient-0.9/test/test_view.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     7069 2019-10-04 21:26:02.000000 tableauserverclient-0.9/test/test_site.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     5554 2019-04-08 17:10:19.000000 tableauserverclient-0.9/test/test_request_option.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     7998 2019-10-04 21:26:02.000000 tableauserverclient-0.9/test/test_project.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      349 2019-04-08 17:10:19.000000 tableauserverclient-0.9/test/test_datasource_model.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      572 2019-04-08 17:10:19.000000 tableauserverclient-0.9/test/test_workbook_model.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      883 2019-04-08 17:10:19.000000 tableauserverclient-0.9/test/test_user_model.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      867 2019-04-08 17:10:19.000000 tableauserverclient-0.9/test/test_tableauauth_model.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     3764 2019-04-08 17:32:53.000000 tableauserverclient-0.9/test/test_subscription.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      334 2019-04-08 17:10:19.000000 tableauserverclient-0.9/LICENSE.versioneer
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      105 2019-04-08 17:10:19.000000 tableauserverclient-0.9/MANIFEST.in
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      711 2019-04-08 17:10:19.000000 tableauserverclient-0.9/README.md
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     1091 2019-10-04 21:26:02.000000 tableauserverclient-0.9/setup.py
-drwxr-xr-x   0 rhay     (1469294935) TSI\Domain Users (62064481)        0 2019-10-04 21:26:13.000000 tableauserverclient-0.9/tableauserverclient/
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      195 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/filesys_helpers.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      689 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/datetime_helpers.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      495 2019-10-04 21:26:13.000000 tableauserverclient-0.9/tableauserverclient/_version.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      845 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/__init__.py
-drwxr-xr-x   0 rhay     (1469294935) TSI\Domain Users (62064481)        0 2019-10-04 21:26:13.000000 tableauserverclient-0.9/tableauserverclient/server/
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4862 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/server.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      208 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/server/sort.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      797 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/__init__.py
-drwxr-xr-x   0 rhay     (1469294935) TSI\Domain Users (62064481)        0 2019-10-04 21:26:13.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4592 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/projects_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     9589 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/flows_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)    11213 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/datasources_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)    14145 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/workbooks_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     1811 2019-04-08 17:32:53.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/jobs_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     3815 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/users_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      788 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/__init__.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4417 2019-04-08 17:32:53.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/sites_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     2299 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/subscriptions_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     2151 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/auth_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     6253 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4417 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/databases_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     3405 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/default_permissions_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4534 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/tables_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     1006 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/metadata_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     3375 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/permissions_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     2092 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/resource_tagger.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4625 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/groups_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     1569 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/exceptions.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      949 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/server_info_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     2526 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/fileuploads_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     1738 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/tasks_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4004 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/schedules_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4673 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/server/endpoint/views_endpoint.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     2747 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/pager.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)    26292 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/request_factory.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)       44 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/server/exceptions.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      865 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/server/filter.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4890 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/server/request_options.py
-drwxr-xr-x   0 rhay     (1469294935) TSI\Domain Users (62064481)        0 2019-10-04 21:26:13.000000 tableauserverclient-0.9/tableauserverclient/models/
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     1317 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/models/connection_credentials.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4893 2019-04-08 17:32:53.000000 tableauserverclient-0.9/tableauserverclient/models/property_decorators.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4770 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/view_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     5295 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/flow_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     2114 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/models/task_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      509 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/models/tag_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     1119 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/tableau_auth.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4500 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/models/job_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     1042 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/models/server_info_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     7508 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/database_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     9618 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/workbook_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     9938 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/site_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     3030 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/permissions_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4590 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/project_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     5033 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/models/interval_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     1094 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/__init__.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      503 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/personal_access_token_auth.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     5642 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/user_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     8484 2019-04-08 17:32:53.000000 tableauserverclient-0.9/tableauserverclient/models/schedule_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4061 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/table_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      105 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/exceptions.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      265 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/models/target.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      730 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/models/fileupload_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     1882 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/group_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     1964 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/models/subscription_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     1918 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/column_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     3437 2019-04-08 17:32:53.000000 tableauserverclient-0.9/tableauserverclient/models/connection_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      967 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/models/pagination_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      404 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/reference_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     6371 2019-10-04 21:26:02.000000 tableauserverclient-0.9/tableauserverclient/models/datasource_item.py
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      967 2019-04-08 17:10:19.000000 tableauserverclient-0.9/tableauserverclient/namespace.py
-drwxr-xr-x   0 rhay     (1469294935) TSI\Domain Users (62064481)        0 2019-10-04 21:26:13.000000 tableauserverclient-0.9/tableauserverclient.egg-info/
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      292 2019-10-04 21:26:12.000000 tableauserverclient-0.9/tableauserverclient.egg-info/PKG-INFO
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)     4098 2019-10-04 21:26:12.000000 tableauserverclient-0.9/tableauserverclient.egg-info/SOURCES.txt
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)       36 2019-10-04 21:26:12.000000 tableauserverclient-0.9/tableauserverclient.egg-info/requires.txt
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)       20 2019-10-04 21:26:12.000000 tableauserverclient-0.9/tableauserverclient.egg-info/top_level.txt
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)        1 2019-10-04 21:26:12.000000 tableauserverclient-0.9/tableauserverclient.egg-info/dependency_links.txt
--rw-r--r--   0 rhay     (1469294935) TSI\Domain Users (62064481)      399 2019-10-04 21:26:13.000000 tableauserverclient-0.9/setup.cfg
--rwxr-xr-x   0 rhay     (1469294935) TSI\Domain Users (62064481)    68632 2019-04-08 17:10:19.000000 tableauserverclient-0.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 23:49:06.810418 tableauserverclient-0.9.31.post0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (121)     9886 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/LICENSE.versioneer
+-rw-r--r--   0 runner    (1001) docker     (121)      542 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-03-29 23:49:06.810418 tableauserverclient-0.9.31.post0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      921 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 23:49:06.782417 tableauserverclient-0.9.31.post0.dev1/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 23:49:06.786417 tableauserverclient-0.9.31.post0.dev1/samples/
+-rw-r--r--   0 runner    (1001) docker     (121)     3763 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/add_default_permission.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1742 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/create_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2943 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/create_project.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4964 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/create_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2989 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/download_view_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4141 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/explore_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3005 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/explore_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5640 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/explore_workbook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3600 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/export.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3218 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/export_wb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4152 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/filter_sort_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4028 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/filter_sort_projects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5454 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/initialize_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/kill_all_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3341 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/login.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/metadata_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2703 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/move_workbook_projects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4276 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/move_workbook_sites.py
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/name.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4776 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/pagination_sample.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5158 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/publish_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4453 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/publish_workbook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2927 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/query_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2585 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2420 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/refresh_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/set_refresh_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/update_connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3709 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/samples/update_datasource_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2022-03-29 23:49:06.810418 tableauserverclient-0.9.31.post0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 23:49:06.786417 tableauserverclient-0.9.31.post0.dev1/smoke/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/smoke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 23:49:06.810418 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/
+-rw-r--r--   0 runner    (1001) docker     (121)     1123 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2022-03-29 23:49:06.810418 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      790 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/datetime_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/exponential_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1667 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/filesys_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 23:49:06.790417 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/column_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1317 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/connection_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3457 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/connection_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3283 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/data_acceleration_report_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6504 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/data_alert_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7927 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/database_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13317 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/datasource_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3700 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/dqw_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/favorites_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/fileupload_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7054 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/flow_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3167 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/flow_run_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3650 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/group_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5249 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/interval_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7044 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/job_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5102 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/metric_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/pagination_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3511 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/permissions_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/personal_access_token_auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5668 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/project_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4709 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/property_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/reference_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2796 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/revision_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10496 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/schedule_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/server_info_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40754 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/site_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4421 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/subscription_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4356 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/table_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/tableau_auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/tag_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/target.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3420 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/task_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7609 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/user_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/view_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2650 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/webhook_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13542 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/workbook_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 23:49:06.790417 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/
+-rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 23:49:06.794417 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3560 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/auth_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/data_acceleration_report_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5299 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/data_alert_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5335 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/databases_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19282 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/datasources_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4066 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/default_permissions_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/dqw_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8256 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2240 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4869 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/favorites_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2288 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/fileuploads_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3298 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/flow_runs_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10475 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/flows_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6507 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/groups_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3169 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/jobs_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5204 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/metadata_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3247 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/metrics_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3720 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/permissions_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5658 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/projects_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2215 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/resource_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5497 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/schedules_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)      965 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/server_info_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5773 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/sites_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3224 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/subscriptions_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5313 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/tables_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3017 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/tasks_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5382 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/users_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7050 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/views_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2795 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/webhooks_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21564 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/workbooks_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      864 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2726 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/pager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5333 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/query.py
+-rw-r--r--   0 runner    (1001) docker     (121)    54187 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/request_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6197 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/request_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5500 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 23:49:06.786417 tableauserverclient-0.9.31.post0.dev1/tableauserverclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-03-29 23:49:06.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    11488 2022-03-29 23:49:06.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-29 23:49:06.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-29 23:49:05.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-03-29 23:49:06.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-03-29 23:49:06.000000 tableauserverclient-0.9.31.post0.dev1/tableauserverclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 23:49:06.798417 tableauserverclient-0.9.31.post0.dev1/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 23:49:06.810418 tableauserverclient-0.9.31.post0.dev1/test/assets/
+-rw-r--r--   0 runner    (1001) docker     (121)    18670 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/RESTAPISample Image.png
+-rw-r--r--   0 runner    (1001) docker     (121)    39415 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/Sample View Image.png
+-rw-r--r--   0 runner    (1001) docker     (121)   196608 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/World Indicators.hyper
+-rw-r--r--   0 runner    (1001) docker     (121)      449 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/auth_sign_in.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/auth_sign_in_error.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/auth_sign_in_impersonate.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      787 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/data_acceleration_report.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/data_alerts_add_user.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/data_alerts_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/data_alerts_get_by_id.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/data_alerts_update.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     2244 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/database_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      982 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/database_populate_permissions.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/database_update.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/datasource_add_tags.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/datasource_connection_update.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/datasource_data_update.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/datasource_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      803 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/datasource_get_by_id.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/datasource_get_empty.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/datasource_populate_connections.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/datasource_populate_permissions.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/datasource_publish.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      389 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/datasource_publish_async.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/datasource_refresh.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      773 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/datasource_revision.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      635 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/datasource_update.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      758 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/dqw_by_content_type.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      743 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/favorites_add_datasource.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/favorites_add_project.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/favorites_add_view.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      849 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/favorites_add_workbook.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/favorites_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/fileupload_append.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/fileupload_initialize.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/flow_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      722 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/flow_populate_connections.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      719 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/flow_populate_permissions.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/flow_refresh.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      926 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/flow_runs_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/flow_runs_get_by_id.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/flow_runs_get_by_id_failed.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/flow_runs_get_by_id_inprogress.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/flow_update.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/group_add_user.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      401 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/group_create.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/group_create_ad.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      367 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/group_create_async.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      720 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/group_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      473 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/group_populate_users.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/group_populate_users_empty.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      444 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/group_update.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/group_users_added.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/job_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      846 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/job_get_by_id.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      737 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/job_get_by_id_failed.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      685 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/job_get_by_id_inprogress.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/metadata_paged_1.json
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/metadata_paged_2.json
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/metadata_paged_3.json
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/metadata_query_error.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/metadata_query_expected_dict.dict
+-rw-r--r--   0 runner    (1001) docker     (121)      549 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/metadata_query_success.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/metrics_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/metrics_get_by_id.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/metrics_update.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1997 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/populate_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (121)   152314 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/populate_pdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/project_content_permission.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      444 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/project_create.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/project_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      722 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/project_populate_permissions.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/project_populate_workbook_default_permissions.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/project_update.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      833 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/project_update_datasource_default_permissions.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/request_option_filter_equals.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/request_option_filter_tags_in.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     2990 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/request_option_page_number.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/request_option_page_size.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     2988 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/request_option_pagination.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     2988 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/request_option_slicing_queryset.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/schedule_add_datasource.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/schedule_add_workbook.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      430 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/schedule_add_workbook_with_warnings.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/schedule_create_daily.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      693 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/schedule_create_hourly.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/schedule_create_monthly.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      889 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/schedule_create_weekly.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/schedule_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/schedule_get_by_id.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/schedule_get_empty.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/schedule_update.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/server_info_25.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/server_info_404.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      391 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/server_info_auth_info.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/server_info_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/site_create.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/site_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/site_get_by_id.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/site_get_by_name.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/site_update.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/subscription_create.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/subscription_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      652 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/subscription_get_by_id.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/table_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/table_update.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1707 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/tasks_no_workbook_or_datasource.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/tasks_run_now_response.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/tasks_with_dataacceleration_task.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      820 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/tasks_with_datasource.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      818 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/tasks_with_workbook.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/tasks_with_workbook_and_datasource.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/user_add.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/user_add_favorite.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      678 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/user_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/user_get_by_id.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/user_get_empty.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/user_populate_groups.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      815 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/user_populate_workbooks.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/user_update.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/view_add_tags.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/view_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/view_get_id.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/view_get_usage.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/view_populate_permissions.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      858 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/view_update_permissions.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      549 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/webhook_create.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/webhook_create_request.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/webhook_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_add_tags.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_get.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_get_by_id.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_get_by_id_personal.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_get_empty.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      714 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_get_invalid_date.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      719 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_get_page_1.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      816 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_get_page_2.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      699 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_get_page_3.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_populate_connections.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_populate_permissions.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      641 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_populate_views.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      807 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_populate_views_usage.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_publish.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_publish_async.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_refresh.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      773 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_revision.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      684 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_update.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/assets/workbook_update_permissions.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     6130 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2072 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_data_acceleration_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5720 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_dataalert.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5318 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37148 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_datasource_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_exponential_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5554 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_favorites.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3750 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_filesys_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2568 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_fileuploads.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7281 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_flow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5037 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_flowruns.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11948 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)      766 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4699 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4103 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5644 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3858 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_pager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16369 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (121)      954 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_project_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_regression_tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12928 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_request_option.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16907 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2889 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_server_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11893 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_site.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2247 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_site_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4345 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_sort.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5149 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2413 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)      674 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_tableauauth_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6665 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10266 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)      884 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_user_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15414 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3333 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46402 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_workbook.py
+-rw-r--r--   0 runner    (1001) docker     (121)      573 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/test/test_workbook_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    68632 2022-03-29 23:48:57.000000 tableauserverclient-0.9.31.post0.dev1/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tableauserverclient-0.9/LICENSE` & `tableauserverclient-0.9.31.post0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `tableauserverclient-0.9/test/test_site_model.py` & `tableauserverclient-0.9.31.post0.dev1/test/test_site_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # coding=utf-8
 
 import unittest
+
 import tableauserverclient as TSC
 
 
 class SiteModelTests(unittest.TestCase):
     def test_invalid_name(self):
         self.assertRaises(ValueError, TSC.SiteItem, None, "url")
         self.assertRaises(ValueError, TSC.SiteItem, "", "url")
```

### Comparing `tableauserverclient-0.9/test/test_database.py` & `tableauserverclient-0.9.31.post0.dev1/test/test_database.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,113 @@
 import unittest
-import os
+
 import requests_mock
-import xml.etree.ElementTree as ET
+
 import tableauserverclient as TSC
-from tableauserverclient.datetime_helpers import format_datetime
-from tableauserverclient.server.endpoint.exceptions import InternalServerError
-from tableauserverclient.server.request_factory import RequestFactory
-from ._utils import read_xml_asset, read_xml_assets, asset
-
-GET_XML = 'database_get.xml'
-POPULATE_PERMISSIONS_XML = 'database_populate_permissions.xml'
-UPDATE_XML = 'database_update.xml'
+from ._utils import read_xml_asset, asset
+
+GET_XML = "database_get.xml"
+POPULATE_PERMISSIONS_XML = "database_populate_permissions.xml"
+UPDATE_XML = "database_update.xml"
+GET_DQW_BY_CONTENT = "dqw_by_content_type.xml"
 
 
 class DatabaseTests(unittest.TestCase):
     def setUp(self):
-        self.server = TSC.Server('http://test')
-
+        self.server = TSC.Server("http://test", False)
         # Fake signin
-        self.server._site_id = 'dad65087-b08b-4603-af4e-2887b8aafc67'
-        self.server._auth_token = 'j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM'
+        self.server._site_id = "dad65087-b08b-4603-af4e-2887b8aafc67"
+        self.server._auth_token = "j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM"
         self.server.version = "3.5"
 
         self.baseurl = self.server.databases.baseurl
 
     def test_get(self):
         response_xml = read_xml_asset(GET_XML)
         with requests_mock.mock() as m:
             m.get(self.baseurl, text=response_xml)
             all_databases, pagination_item = self.server.databases.get()
 
         self.assertEqual(5, pagination_item.total_available)
-        self.assertEqual('5ea59b45-e497-4827-8809-bfe213236f75', all_databases[0].id)
-        self.assertEqual('hyper', all_databases[0].connection_type)
-        self.assertEqual('hyper_0.hyper', all_databases[0].name)
-
-        self.assertEqual('23591f2c-4802-4d6a-9e28-574a8ea9bc4c', all_databases[1].id)
-        self.assertEqual('sqlserver', all_databases[1].connection_type)
-        self.assertEqual('testv1', all_databases[1].name)
-        self.assertEqual('9324cf6b-ba72-4b8e-b895-ac3f28d2f0e0', all_databases[1].contact_id)
+        self.assertEqual("5ea59b45-e497-4827-8809-bfe213236f75", all_databases[0].id)
+        self.assertEqual("hyper", all_databases[0].connection_type)
+        self.assertEqual("hyper_0.hyper", all_databases[0].name)
+
+        self.assertEqual("23591f2c-4802-4d6a-9e28-574a8ea9bc4c", all_databases[1].id)
+        self.assertEqual("sqlserver", all_databases[1].connection_type)
+        self.assertEqual("testv1", all_databases[1].name)
+        self.assertEqual("9324cf6b-ba72-4b8e-b895-ac3f28d2f0e0", all_databases[1].contact_id)
         self.assertEqual(True, all_databases[1].certified)
 
     def test_update(self):
         response_xml = read_xml_asset(UPDATE_XML)
         with requests_mock.mock() as m:
-            m.put(self.baseurl + '/23591f2c-4802-4d6a-9e28-574a8ea9bc4c', text=response_xml)
-            single_database = TSC.DatabaseItem('test')
-            single_database.contact_id = '9324cf6b-ba72-4b8e-b895-ac3f28d2f0e0'
-            single_database._id = '23591f2c-4802-4d6a-9e28-574a8ea9bc4c'
+            m.put(self.baseurl + "/23591f2c-4802-4d6a-9e28-574a8ea9bc4c", text=response_xml)
+            single_database = TSC.DatabaseItem("test")
+            single_database.contact_id = "9324cf6b-ba72-4b8e-b895-ac3f28d2f0e0"
+            single_database._id = "23591f2c-4802-4d6a-9e28-574a8ea9bc4c"
             single_database.certified = True
             single_database.certification_note = "Test"
             single_database = self.server.databases.update(single_database)
 
-        self.assertEqual('23591f2c-4802-4d6a-9e28-574a8ea9bc4c', single_database.id)
-        self.assertEqual('9324cf6b-ba72-4b8e-b895-ac3f28d2f0e0', single_database.contact_id)
+        self.assertEqual("23591f2c-4802-4d6a-9e28-574a8ea9bc4c", single_database.id)
+        self.assertEqual("9324cf6b-ba72-4b8e-b895-ac3f28d2f0e0", single_database.contact_id)
         self.assertEqual(True, single_database.certified)
         self.assertEqual("Test", single_database.certification_note)
 
     def test_populate_permissions(self):
-        with open(asset(POPULATE_PERMISSIONS_XML), 'rb') as f:
-            response_xml = f.read().decode('utf-8')
+        with open(asset(POPULATE_PERMISSIONS_XML), "rb") as f:
+            response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
-            m.get(self.baseurl + '/0448d2ed-590d-4fa0-b272-a2a8a24555b5/permissions', text=response_xml)
-            single_database = TSC.DatabaseItem('test')
-            single_database._id = '0448d2ed-590d-4fa0-b272-a2a8a24555b5'
+            m.get(self.baseurl + "/0448d2ed-590d-4fa0-b272-a2a8a24555b5/permissions", text=response_xml)
+            single_database = TSC.DatabaseItem("test")
+            single_database._id = "0448d2ed-590d-4fa0-b272-a2a8a24555b5"
 
             self.server.databases.populate_permissions(single_database)
             permissions = single_database.permissions
 
-            self.assertEqual(permissions[0].grantee.tag_name, 'group')
-            self.assertEqual(permissions[0].grantee.id, '5e5e1978-71fa-11e4-87dd-7382f5c437af')
-            self.assertDictEqual(permissions[0].capabilities, {
-                TSC.Permission.Capability.ChangePermissions: TSC.Permission.Mode.Deny,
-                TSC.Permission.Capability.Read: TSC.Permission.Mode.Allow,
-            })
-
-            self.assertEqual(permissions[1].grantee.tag_name, 'user')
-            self.assertEqual(permissions[1].grantee.id, '7c37ee24-c4b1-42b6-a154-eaeab7ee330a')
-            self.assertDictEqual(permissions[1].capabilities, {
-                TSC.Permission.Capability.Write: TSC.Permission.Mode.Allow,
-            })
+            self.assertEqual(permissions[0].grantee.tag_name, "group")
+            self.assertEqual(permissions[0].grantee.id, "5e5e1978-71fa-11e4-87dd-7382f5c437af")
+            self.assertDictEqual(
+                permissions[0].capabilities,
+                {
+                    TSC.Permission.Capability.ChangePermissions: TSC.Permission.Mode.Deny,
+                    TSC.Permission.Capability.Read: TSC.Permission.Mode.Allow,
+                },
+            )
+
+            self.assertEqual(permissions[1].grantee.tag_name, "user")
+            self.assertEqual(permissions[1].grantee.id, "7c37ee24-c4b1-42b6-a154-eaeab7ee330a")
+            self.assertDictEqual(
+                permissions[1].capabilities,
+                {
+                    TSC.Permission.Capability.Write: TSC.Permission.Mode.Allow,
+                },
+            )
+
+    def test_populate_data_quality_warning(self):
+        with open(asset(GET_DQW_BY_CONTENT), "rb") as f:
+            response_xml = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            m.get(
+                self.server.databases._data_quality_warnings.baseurl + "/94441d26-9a52-4a42-b0fb-3f94792d1aac",
+                text=response_xml,
+            )
+            single_database = TSC.DatabaseItem("test")
+            single_database._id = "94441d26-9a52-4a42-b0fb-3f94792d1aac"
+
+            self.server.databases.populate_dqw(single_database)
+            dqws = single_database.dqws
+            first_dqw = dqws.pop()
+            self.assertEqual(first_dqw.id, "c2e0e406-84fb-4f4e-9998-f20dd9306710")
+            self.assertEqual(first_dqw.warning_type, "WARNING")
+            self.assertEqual(first_dqw.message, "Hello, World!")
+            self.assertEqual(first_dqw.owner_id, "eddc8c5f-6af0-40be-b6b0-2c790290a43f")
+            self.assertEqual(first_dqw.active, True)
+            self.assertEqual(first_dqw.severe, True)
+            self.assertEqual(str(first_dqw.created_at), "2021-04-09 18:39:54+00:00")
+            self.assertEqual(str(first_dqw.updated_at), "2021-04-09 18:39:54+00:00")
 
     def test_delete(self):
         with requests_mock.mock() as m:
-            m.delete(self.baseurl + '/0448d2ed-590d-4fa0-b272-a2a8a24555b5', status_code=204)
-            self.server.databases.delete('0448d2ed-590d-4fa0-b272-a2a8a24555b5')
+            m.delete(self.baseurl + "/0448d2ed-590d-4fa0-b272-a2a8a24555b5", status_code=204)
+            self.server.databases.delete("0448d2ed-590d-4fa0-b272-a2a8a24555b5")
```

### Comparing `tableauserverclient-0.9/test/test_user.py` & `tableauserverclient-0.9.31.post0.dev1/test/test_flow.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,148 +1,135 @@
 import unittest
-import os
+
 import requests_mock
+
 import tableauserverclient as TSC
 from tableauserverclient.datetime_helpers import format_datetime
+from ._utils import read_xml_asset, asset
 
-TEST_ASSET_DIR = os.path.join(os.path.dirname(__file__), 'assets')
-
-GET_XML = os.path.join(TEST_ASSET_DIR, 'user_get.xml')
-GET_EMPTY_XML = os.path.join(TEST_ASSET_DIR, 'user_get_empty.xml')
-GET_BY_ID_XML = os.path.join(TEST_ASSET_DIR, 'user_get_by_id.xml')
-UPDATE_XML = os.path.join(TEST_ASSET_DIR, 'user_update.xml')
-ADD_XML = os.path.join(TEST_ASSET_DIR, 'user_add.xml')
-POPULATE_WORKBOOKS_XML = os.path.join(TEST_ASSET_DIR, 'user_populate_workbooks.xml')
-ADD_FAVORITE_XML = os.path.join(TEST_ASSET_DIR, 'user_add_favorite.xml')
+GET_XML = "flow_get.xml"
+POPULATE_CONNECTIONS_XML = "flow_populate_connections.xml"
+POPULATE_PERMISSIONS_XML = "flow_populate_permissions.xml"
+UPDATE_XML = "flow_update.xml"
+REFRESH_XML = "flow_refresh.xml"
 
 
-class UserTests(unittest.TestCase):
-    def setUp(self):
-        self.server = TSC.Server('http://test')
+class FlowTests(unittest.TestCase):
+    def setUp(self) -> None:
+        self.server = TSC.Server("http://test", False)
 
         # Fake signin
-        self.server._site_id = 'dad65087-b08b-4603-af4e-2887b8aafc67'
-        self.server._auth_token = 'j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM'
+        self.server._site_id = "dad65087-b08b-4603-af4e-2887b8aafc67"
+        self.server._auth_token = "j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM"
+        self.server.version = "3.5"
 
-        self.baseurl = self.server.users.baseurl
+        self.baseurl = self.server.flows.baseurl
 
-    def test_get(self):
-        with open(GET_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
+    def test_get(self) -> None:
+        response_xml = read_xml_asset(GET_XML)
         with requests_mock.mock() as m:
             m.get(self.baseurl, text=response_xml)
-            all_users, pagination_item = self.server.users.get()
+            all_flows, pagination_item = self.server.flows.get()
 
-        self.assertEqual(2, pagination_item.total_available)
-        self.assertEqual(2, len(all_users))
-
-        self.assertTrue(any(user.id == 'dd2239f6-ddf1-4107-981a-4cf94e415794' for user in all_users))
-        single_user = next(user for user in all_users if user.id == 'dd2239f6-ddf1-4107-981a-4cf94e415794')
-        self.assertEqual('alice', single_user.name)
-        self.assertEqual('Publisher', single_user.site_role)
-        self.assertEqual('2016-08-16T23:17:06Z', format_datetime(single_user.last_login))
-
-        self.assertTrue(any(user.id == '2a47bbf8-8900-4ebb-b0a4-2723bd7c46c3' for user in all_users))
-        single_user = next(user for user in all_users if user.id == '2a47bbf8-8900-4ebb-b0a4-2723bd7c46c3')
-        self.assertEqual('Bob', single_user.name)
-        self.assertEqual('Interactor', single_user.site_role)
-
-    def test_get_empty(self):
-        with open(GET_EMPTY_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
-        with requests_mock.mock() as m:
-            m.get(self.baseurl, text=response_xml)
-            all_users, pagination_item = self.server.users.get()
-
-        self.assertEqual(0, pagination_item.total_available)
-        self.assertEqual([], all_users)
-
-    def test_get_before_signin(self):
-        self.server._auth_token = None
-        self.assertRaises(TSC.NotSignedInError, self.server.users.get)
-
-    def test_get_by_id(self):
-        with open(GET_BY_ID_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
-        with requests_mock.mock() as m:
-            m.get(self.baseurl + '/dd2239f6-ddf1-4107-981a-4cf94e415794', text=response_xml)
-            single_user = self.server.users.get_by_id('dd2239f6-ddf1-4107-981a-4cf94e415794')
-
-        self.assertEqual('dd2239f6-ddf1-4107-981a-4cf94e415794', single_user.id)
-        self.assertEqual('alice', single_user.name)
-        self.assertEqual('Alice', single_user.fullname)
-        self.assertEqual('Publisher', single_user.site_role)
-        self.assertEqual('ServerDefault', single_user.auth_setting)
-        self.assertEqual('2016-08-16T23:17:06Z', format_datetime(single_user.last_login))
-        self.assertEqual('local', single_user.domain_name)
-
-    def test_get_by_id_missing_id(self):
-        self.assertRaises(ValueError, self.server.users.get_by_id, '')
-
-    def test_update(self):
-        with open(UPDATE_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
-        with requests_mock.mock() as m:
-            m.put(self.baseurl + '/dd2239f6-ddf1-4107-981a-4cf94e415794', text=response_xml)
-            single_user = TSC.UserItem('test', 'Viewer')
-            single_user._id = 'dd2239f6-ddf1-4107-981a-4cf94e415794'
-            single_user.name = 'Cassie'
-            single_user.fullname = 'Cassie'
-            single_user.email = 'cassie@email.com'
-            single_user = self.server.users.update(single_user)
-
-        self.assertEqual('Cassie', single_user.name)
-        self.assertEqual('Cassie', single_user.fullname)
-        self.assertEqual('cassie@email.com', single_user.email)
-        self.assertEqual('Viewer', single_user.site_role)
-
-    def test_update_missing_id(self):
-        single_user = TSC.UserItem('test', 'Interactor')
-        self.assertRaises(TSC.MissingRequiredFieldError, self.server.users.update, single_user)
-
-    def test_remove(self):
-        with requests_mock.mock() as m:
-            m.delete(self.baseurl + '/dd2239f6-ddf1-4107-981a-4cf94e415794', status_code=204)
-            self.server.users.remove('dd2239f6-ddf1-4107-981a-4cf94e415794')
-
-    def test_remove_missing_id(self):
-        self.assertRaises(ValueError, self.server.users.remove, '')
-
-    def test_add(self):
-        with open(ADD_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
-        with requests_mock.mock() as m:
-            m.post(self.baseurl + '', text=response_xml)
-            new_user = TSC.UserItem(name='Cassie', site_role='Viewer', auth_setting='ServerDefault')
-            new_user = self.server.users.add(new_user)
-
-        self.assertEqual('4cc4c17f-898a-4de4-abed-a1681c673ced', new_user.id)
-        self.assertEqual('Cassie', new_user.name)
-        self.assertEqual('Viewer', new_user.site_role)
-        self.assertEqual('ServerDefault', new_user.auth_setting)
-
-    def test_populate_workbooks(self):
-        with open(POPULATE_WORKBOOKS_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
-        with requests_mock.mock() as m:
-            m.get(self.baseurl + '/dd2239f6-ddf1-4107-981a-4cf94e415794/workbooks',
-                  text=response_xml)
-            single_user = TSC.UserItem('test', 'Interactor')
-            single_user._id = 'dd2239f6-ddf1-4107-981a-4cf94e415794'
-            self.server.users.populate_workbooks(single_user)
-
-            workbook_list = list(single_user.workbooks)
-            self.assertEqual('3cc6cd06-89ce-4fdc-b935-5294135d6d42', workbook_list[0].id)
-            self.assertEqual('SafariSample', workbook_list[0].name)
-            self.assertEqual('SafariSample', workbook_list[0].content_url)
-            self.assertEqual(False, workbook_list[0].show_tabs)
-            self.assertEqual(26, workbook_list[0].size)
-            self.assertEqual('2016-07-26T20:34:56Z', format_datetime(workbook_list[0].created_at))
-            self.assertEqual('2016-07-26T20:35:05Z', format_datetime(workbook_list[0].updated_at))
-            self.assertEqual('ee8c6e70-43b6-11e6-af4f-f7b0d8e20760', workbook_list[0].project_id)
-            self.assertEqual('default', workbook_list[0].project_name)
-            self.assertEqual('5de011f8-5aa9-4d5b-b991-f462c8dd6bb7', workbook_list[0].owner_id)
-            self.assertEqual(set(['Safari', 'Sample']), workbook_list[0].tags)
-
-    def test_populate_workbooks_missing_id(self):
-        single_user = TSC.UserItem('test', 'Interactor')
-        self.assertRaises(TSC.MissingRequiredFieldError, self.server.users.populate_workbooks, single_user)
+        self.assertEqual(5, pagination_item.total_available)
+        self.assertEqual("587daa37-b84d-4400-a9a2-aa90e0be7837", all_flows[0].id)
+        self.assertEqual("http://tableauserver/#/flows/1", all_flows[0].webpage_url)
+        self.assertEqual("2019-06-16T21:43:28Z", format_datetime(all_flows[0].created_at))
+        self.assertEqual("2019-06-16T21:43:28Z", format_datetime(all_flows[0].updated_at))
+        self.assertEqual("Default", all_flows[0].project_name)
+        self.assertEqual("FlowOne", all_flows[0].name)
+        self.assertEqual("aa23f4ac-906f-11e9-86fb-3f0f71412e77", all_flows[0].project_id)
+        self.assertEqual("7ebb3f20-0fd2-4f27-a2f6-c539470999e2", all_flows[0].owner_id)
+        self.assertEqual({"i_love_tags"}, all_flows[0].tags)
+        self.assertEqual("Descriptive", all_flows[0].description)
+
+        self.assertEqual("5c36be69-eb30-461b-b66e-3e2a8e27cc35", all_flows[1].id)
+        self.assertEqual("http://tableauserver/#/flows/4", all_flows[1].webpage_url)
+        self.assertEqual("2019-06-18T03:08:19Z", format_datetime(all_flows[1].created_at))
+        self.assertEqual("2019-06-18T03:08:19Z", format_datetime(all_flows[1].updated_at))
+        self.assertEqual("Default", all_flows[1].project_name)
+        self.assertEqual("FlowTwo", all_flows[1].name)
+        self.assertEqual("aa23f4ac-906f-11e9-86fb-3f0f71412e77", all_flows[1].project_id)
+        self.assertEqual("9127d03f-d996-405f-b392-631b25183a0f", all_flows[1].owner_id)
+
+    def test_update(self) -> None:
+        response_xml = read_xml_asset(UPDATE_XML)
+        with requests_mock.mock() as m:
+            m.put(self.baseurl + "/587daa37-b84d-4400-a9a2-aa90e0be7837", text=response_xml)
+            single_datasource = TSC.FlowItem("test", "aa23f4ac-906f-11e9-86fb-3f0f71412e77")
+            single_datasource.owner_id = "7ebb3f20-0fd2-4f27-a2f6-c539470999e2"
+            single_datasource._id = "587daa37-b84d-4400-a9a2-aa90e0be7837"
+            single_datasource.description = "So fun to see"
+            single_datasource = self.server.flows.update(single_datasource)
+
+        self.assertEqual("587daa37-b84d-4400-a9a2-aa90e0be7837", single_datasource.id)
+        self.assertEqual("aa23f4ac-906f-11e9-86fb-3f0f71412e77", single_datasource.project_id)
+        self.assertEqual("7ebb3f20-0fd2-4f27-a2f6-c539470999e2", single_datasource.owner_id)
+        self.assertEqual("So fun to see", single_datasource.description)
+
+    def test_populate_connections(self) -> None:
+        response_xml = read_xml_asset(POPULATE_CONNECTIONS_XML)
+        with requests_mock.mock() as m:
+            m.get(self.baseurl + "/9dbd2263-16b5-46e1-9c43-a76bb8ab65fb/connections", text=response_xml)
+            single_datasource = TSC.FlowItem("test", "aa23f4ac-906f-11e9-86fb-3f0f71412e77")
+            single_datasource.owner_id = "dd2239f6-ddf1-4107-981a-4cf94e415794"
+            single_datasource._id = "9dbd2263-16b5-46e1-9c43-a76bb8ab65fb"
+            self.server.flows.populate_connections(single_datasource)
+            self.assertEqual("9dbd2263-16b5-46e1-9c43-a76bb8ab65fb", single_datasource.id)
+            connections = single_datasource.connections
+
+        self.assertTrue(connections)
+        conn1, conn2, conn3 = connections
+        self.assertEqual("405c1e4b-60c9-499f-9c47-a4ef1af69359", conn1.id)
+        self.assertEqual("excel-direct", conn1.connection_type)
+        self.assertEqual("", conn1.server_address)
+        self.assertEqual("", conn1.username)
+        self.assertEqual(False, conn1.embed_password)
+        self.assertEqual("b47f41b1-2c47-41a3-8b17-a38ebe8b340c", conn2.id)
+        self.assertEqual("sqlserver", conn2.connection_type)
+        self.assertEqual("test.database.com", conn2.server_address)
+        self.assertEqual("bob", conn2.username)
+        self.assertEqual(False, conn2.embed_password)
+        self.assertEqual("4f4a3b78-0554-43a7-b327-9605e9df9dd2", conn3.id)
+        self.assertEqual("tableau-server-site", conn3.connection_type)
+        self.assertEqual("http://tableauserver", conn3.server_address)
+        self.assertEqual("sally", conn3.username)
+        self.assertEqual(True, conn3.embed_password)
+
+    def test_populate_permissions(self) -> None:
+        with open(asset(POPULATE_PERMISSIONS_XML), "rb") as f:
+            response_xml = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            m.get(self.baseurl + "/0448d2ed-590d-4fa0-b272-a2a8a24555b5/permissions", text=response_xml)
+            single_datasource = TSC.FlowItem("test")
+            single_datasource._id = "0448d2ed-590d-4fa0-b272-a2a8a24555b5"
+
+            self.server.flows.populate_permissions(single_datasource)
+            permissions = single_datasource.permissions
+
+            self.assertEqual(permissions[0].grantee.tag_name, "group")
+            self.assertEqual(permissions[0].grantee.id, "aa42f384-906f-11e9-86fc-bb24278874b9")
+            self.assertDictEqual(
+                permissions[0].capabilities,
+                {
+                    TSC.Permission.Capability.Write: TSC.Permission.Mode.Allow,
+                    TSC.Permission.Capability.Read: TSC.Permission.Mode.Allow,
+                },
+            )
+
+    def test_refresh(self):
+        with open(asset(REFRESH_XML), "rb") as f:
+            response_xml = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            m.post(self.baseurl + "/92967d2d-c7e2-46d0-8847-4802df58f484/run", text=response_xml)
+            flow_item = TSC.FlowItem("test")
+            flow_item._id = "92967d2d-c7e2-46d0-8847-4802df58f484"
+            refresh_job = self.server.flows.refresh(flow_item)
+
+            self.assertEqual(refresh_job.id, "d1b2ccd0-6dfa-444a-aee4-723dbd6b7c9d")
+            self.assertEqual(refresh_job.mode, "Asynchronous")
+            self.assertEqual(refresh_job.type, "RunFlow")
+            self.assertEqual(format_datetime(refresh_job.created_at), "2018-05-22T13:00:29Z")
+            self.assertIsInstance(refresh_job.flow_run, TSC.FlowRunItem)
+            self.assertEqual(refresh_job.flow_run.id, "e0c3067f-2333-4eee-8028-e0a56ca496f6")
+            self.assertEqual(refresh_job.flow_run.flow_id, "92967d2d-c7e2-46d0-8847-4802df58f484")
+            self.assertEqual(format_datetime(refresh_job.flow_run.started_at), "2018-05-22T13:00:29Z")
```

### Comparing `tableauserverclient-0.9/test/test_pager.py` & `tableauserverclient-0.9.31.post0.dev1/test/test_pager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-import unittest
 import os
+import unittest
+
 import requests_mock
+
 import tableauserverclient as TSC
 
-TEST_ASSET_DIR = os.path.join(os.path.dirname(__file__), 'assets')
+TEST_ASSET_DIR = os.path.join(os.path.dirname(__file__), "assets")
 
-GET_XML_PAGE1 = os.path.join(TEST_ASSET_DIR, 'workbook_get_page_1.xml')
-GET_XML_PAGE2 = os.path.join(TEST_ASSET_DIR, 'workbook_get_page_2.xml')
-GET_XML_PAGE3 = os.path.join(TEST_ASSET_DIR, 'workbook_get_page_3.xml')
+GET_XML_PAGE1 = os.path.join(TEST_ASSET_DIR, "workbook_get_page_1.xml")
+GET_XML_PAGE2 = os.path.join(TEST_ASSET_DIR, "workbook_get_page_2.xml")
+GET_XML_PAGE3 = os.path.join(TEST_ASSET_DIR, "workbook_get_page_3.xml")
 
 
 class PagerTests(unittest.TestCase):
     def setUp(self):
-        self.server = TSC.Server('http://test')
+        self.server = TSC.Server("http://test", False)
 
         # Fake sign in
-        self.server._site_id = 'dad65087-b08b-4603-af4e-2887b8aafc67'
-        self.server._auth_token = 'j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM'
+        self.server._site_id = "dad65087-b08b-4603-af4e-2887b8aafc67"
+        self.server._auth_token = "j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM"
 
         self.baseurl = self.server.workbooks.baseurl
 
     def test_pager_with_no_options(self):
-        with open(GET_XML_PAGE1, 'rb') as f:
-            page_1 = f.read().decode('utf-8')
-        with open(GET_XML_PAGE2, 'rb') as f:
-            page_2 = f.read().decode('utf-8')
-        with open(GET_XML_PAGE3, 'rb') as f:
-            page_3 = f.read().decode('utf-8')
+        with open(GET_XML_PAGE1, "rb") as f:
+            page_1 = f.read().decode("utf-8")
+        with open(GET_XML_PAGE2, "rb") as f:
+            page_2 = f.read().decode("utf-8")
+        with open(GET_XML_PAGE3, "rb") as f:
+            page_3 = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             # Register Pager with default request options
             m.get(self.baseurl, text=page_1)
 
             # Register Pager with some pages
             m.get(self.baseurl + "?pageNumber=1&pageSize=1", text=page_1)
             m.get(self.baseurl + "?pageNumber=2&pageSize=1", text=page_2)
@@ -38,51 +40,51 @@
 
             # No options should get all 3
             workbooks = list(TSC.Pager(self.server.workbooks))
             self.assertTrue(len(workbooks) == 3)
 
             # Let's check that workbook items aren't duplicates
             wb1, wb2, wb3 = workbooks
-            self.assertEqual(wb1.name, 'Page1Workbook')
-            self.assertEqual(wb2.name, 'Page2Workbook')
-            self.assertEqual(wb3.name, 'Page3Workbook')
+            self.assertEqual(wb1.name, "Page1Workbook")
+            self.assertEqual(wb2.name, "Page2Workbook")
+            self.assertEqual(wb3.name, "Page3Workbook")
 
     def test_pager_with_options(self):
-        with open(GET_XML_PAGE1, 'rb') as f:
-            page_1 = f.read().decode('utf-8')
-        with open(GET_XML_PAGE2, 'rb') as f:
-            page_2 = f.read().decode('utf-8')
-        with open(GET_XML_PAGE3, 'rb') as f:
-            page_3 = f.read().decode('utf-8')
+        with open(GET_XML_PAGE1, "rb") as f:
+            page_1 = f.read().decode("utf-8")
+        with open(GET_XML_PAGE2, "rb") as f:
+            page_2 = f.read().decode("utf-8")
+        with open(GET_XML_PAGE3, "rb") as f:
+            page_3 = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             # Register Pager with some pages
             m.get(self.baseurl + "?pageNumber=1&pageSize=1", complete_qs=True, text=page_1)
             m.get(self.baseurl + "?pageNumber=2&pageSize=1", complete_qs=True, text=page_2)
             m.get(self.baseurl + "?pageNumber=3&pageSize=1", complete_qs=True, text=page_3)
             m.get(self.baseurl + "?pageNumber=1&pageSize=3", complete_qs=True, text=page_1)
 
             # Starting on page 2 should get 2 out of 3
             opts = TSC.RequestOptions(2, 1)
             workbooks = list(TSC.Pager(self.server.workbooks, opts))
             self.assertTrue(len(workbooks) == 2)
 
             # Check that the workbooks are the 2 we think they should be
             wb2, wb3 = workbooks
-            self.assertEqual(wb2.name, 'Page2Workbook')
-            self.assertEqual(wb3.name, 'Page3Workbook')
+            self.assertEqual(wb2.name, "Page2Workbook")
+            self.assertEqual(wb3.name, "Page3Workbook")
 
             # Starting on 1 with pagesize of 3 should get all 3
             opts = TSC.RequestOptions(1, 3)
             workbooks = list(TSC.Pager(self.server.workbooks, opts))
             self.assertTrue(len(workbooks) == 3)
             wb1, wb2, wb3 = workbooks
-            self.assertEqual(wb1.name, 'Page1Workbook')
-            self.assertEqual(wb2.name, 'Page2Workbook')
-            self.assertEqual(wb3.name, 'Page3Workbook')
+            self.assertEqual(wb1.name, "Page1Workbook")
+            self.assertEqual(wb2.name, "Page2Workbook")
+            self.assertEqual(wb3.name, "Page3Workbook")
 
             # Starting on 3 with pagesize of 1 should get the last item
             opts = TSC.RequestOptions(3, 1)
             workbooks = list(TSC.Pager(self.server.workbooks, opts))
             self.assertTrue(len(workbooks) == 1)
             # Should have the last workbook
             wb3 = workbooks.pop()
-            self.assertEqual(wb3.name, 'Page3Workbook')
+            self.assertEqual(wb3.name, "Page3Workbook")
```

### Comparing `tableauserverclient-0.9/test/test_server_info.py` & `tableauserverclient-0.9.31.post0.dev1/test/test_server_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,62 +1,64 @@
-import unittest
 import os.path
+import unittest
+
 import requests_mock
+
 import tableauserverclient as TSC
 
-TEST_ASSET_DIR = os.path.join(os.path.dirname(__file__), 'assets')
+TEST_ASSET_DIR = os.path.join(os.path.dirname(__file__), "assets")
 
-SERVER_INFO_GET_XML = os.path.join(TEST_ASSET_DIR, 'server_info_get.xml')
-SERVER_INFO_25_XML = os.path.join(TEST_ASSET_DIR, 'server_info_25.xml')
-SERVER_INFO_404 = os.path.join(TEST_ASSET_DIR, 'server_info_404.xml')
-SERVER_INFO_AUTH_INFO_XML = os.path.join(TEST_ASSET_DIR, 'server_info_auth_info.xml')
+SERVER_INFO_GET_XML = os.path.join(TEST_ASSET_DIR, "server_info_get.xml")
+SERVER_INFO_25_XML = os.path.join(TEST_ASSET_DIR, "server_info_25.xml")
+SERVER_INFO_404 = os.path.join(TEST_ASSET_DIR, "server_info_404.xml")
+SERVER_INFO_AUTH_INFO_XML = os.path.join(TEST_ASSET_DIR, "server_info_auth_info.xml")
 
 
 class ServerInfoTests(unittest.TestCase):
     def setUp(self):
-        self.server = TSC.Server('http://test')
+        self.server = TSC.Server("http://test", False)
         self.baseurl = self.server.server_info.baseurl
         self.server.version = "2.4"
 
     def test_server_info_get(self):
-        with open(SERVER_INFO_GET_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
+        with open(SERVER_INFO_GET_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             m.get(self.server.server_info.baseurl, text=response_xml)
             actual = self.server.server_info.get()
 
-            self.assertEqual('10.1.0', actual.product_version)
-            self.assertEqual('10100.16.1024.2100', actual.build_number)
-            self.assertEqual('2.4', actual.rest_api_version)
+            self.assertEqual("10.1.0", actual.product_version)
+            self.assertEqual("10100.16.1024.2100", actual.build_number)
+            self.assertEqual("2.4", actual.rest_api_version)
 
     def test_server_info_use_highest_version_downgrades(self):
-        with open(SERVER_INFO_AUTH_INFO_XML, 'rb') as f:
+        with open(SERVER_INFO_AUTH_INFO_XML, "rb") as f:
             # This is the auth.xml endpoint present back to 9.0 Servers
-            auth_response_xml = f.read().decode('utf-8')
-        with open(SERVER_INFO_404, 'rb') as f:
+            auth_response_xml = f.read().decode("utf-8")
+        with open(SERVER_INFO_404, "rb") as f:
             # 10.1 serverInfo response
-            si_response_xml = f.read().decode('utf-8')
+            si_response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             # Return a 404 for serverInfo so we can pretend this is an old Server
             m.get(self.server.server_address + "/api/2.4/serverInfo", text=si_response_xml, status_code=404)
             m.get(self.server.server_address + "/auth?format=xml", text=auth_response_xml)
             self.server.use_server_version()
-            self.assertEqual(self.server.version, '2.2')
+            self.assertEqual(self.server.version, "2.2")
 
     def test_server_info_use_highest_version_upgrades(self):
-        with open(SERVER_INFO_GET_XML, 'rb') as f:
-            si_response_xml = f.read().decode('utf-8')
+        with open(SERVER_INFO_GET_XML, "rb") as f:
+            si_response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             m.get(self.server.server_address + "/api/2.4/serverInfo", text=si_response_xml)
             # Pretend we're old
-            self.server.version = '2.0'
+            self.server.version = "2.0"
             self.server.use_server_version()
             # Did we upgrade to 2.4?
-            self.assertEqual(self.server.version, '2.4')
+            self.assertEqual(self.server.version, "2.4")
 
     def test_server_use_server_version_flag(self):
-        with open(SERVER_INFO_25_XML, 'rb') as f:
-            si_response_xml = f.read().decode('utf-8')
+        with open(SERVER_INFO_25_XML, "rb") as f:
+            si_response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
-            m.get('http://test/api/2.4/serverInfo', text=si_response_xml)
-            server = TSC.Server('http://test', use_server_version=True)
-            self.assertEqual(server.version, '2.5')
+            m.get("http://test/api/2.4/serverInfo", text=si_response_xml)
+            server = TSC.Server("http://test", use_server_version=True)
+            self.assertEqual(server.version, "2.5")
```

### Comparing `tableauserverclient-0.9/test/test_group.py` & `tableauserverclient-0.9.31.post0.dev1/test/test_group.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,199 +1,251 @@
 # encoding=utf-8
-import unittest
 import os
+import unittest
+
 import requests_mock
+
 import tableauserverclient as TSC
 from tableauserverclient.datetime_helpers import format_datetime
 
-TEST_ASSET_DIR = os.path.join(os.path.dirname(__file__), 'assets')
+TEST_ASSET_DIR = os.path.join(os.path.dirname(__file__), "assets")
 
-GET_XML = os.path.join(TEST_ASSET_DIR, 'group_get.xml')
-POPULATE_USERS = os.path.join(TEST_ASSET_DIR, 'group_populate_users.xml')
-POPULATE_USERS_EMPTY = os.path.join(TEST_ASSET_DIR, 'group_populate_users_empty.xml')
-ADD_USER = os.path.join(TEST_ASSET_DIR, 'group_add_user.xml')
-ADD_USER_POPULATE = os.path.join(TEST_ASSET_DIR, 'group_users_added.xml')
-CREATE_GROUP = os.path.join(TEST_ASSET_DIR, 'group_create.xml')
-CREATE_GROUP_ASYNC = os.path.join(TEST_ASSET_DIR, 'group_create_async.xml')
-UPDATE_XML = os.path.join(TEST_ASSET_DIR, 'group_update.xml')
+GET_XML = os.path.join(TEST_ASSET_DIR, "group_get.xml")
+POPULATE_USERS = os.path.join(TEST_ASSET_DIR, "group_populate_users.xml")
+POPULATE_USERS_EMPTY = os.path.join(TEST_ASSET_DIR, "group_populate_users_empty.xml")
+ADD_USER = os.path.join(TEST_ASSET_DIR, "group_add_user.xml")
+ADD_USER_POPULATE = os.path.join(TEST_ASSET_DIR, "group_users_added.xml")
+CREATE_GROUP = os.path.join(TEST_ASSET_DIR, "group_create.xml")
+CREATE_GROUP_AD = os.path.join(TEST_ASSET_DIR, "group_create_ad.xml")
+CREATE_GROUP_ASYNC = os.path.join(TEST_ASSET_DIR, "group_create_async.xml")
+UPDATE_XML = os.path.join(TEST_ASSET_DIR, "group_update.xml")
 
 
 class GroupTests(unittest.TestCase):
-    def setUp(self):
-        self.server = TSC.Server('http://test')
+    def setUp(self) -> None:
+        self.server = TSC.Server("http://test", False)
 
         # Fake signin
-        self.server._site_id = 'dad65087-b08b-4603-af4e-2887b8aafc67'
-        self.server._auth_token = 'j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM'
+        self.server._site_id = "dad65087-b08b-4603-af4e-2887b8aafc67"
+        self.server._auth_token = "j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM"
 
         self.baseurl = self.server.groups.baseurl
 
-    def test_get(self):
-        with open(GET_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
+    def test_get(self) -> None:
+        with open(GET_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             m.get(self.baseurl, text=response_xml)
             all_groups, pagination_item = self.server.groups.get()
 
         self.assertEqual(3, pagination_item.total_available)
-        self.assertEqual('ef8b19c0-43b6-11e6-af50-63f5805dbe3c', all_groups[0].id)
-        self.assertEqual('All Users', all_groups[0].name)
-        self.assertEqual('local', all_groups[0].domain_name)
-
-        self.assertEqual('e7833b48-c6f7-47b5-a2a7-36e7dd232758', all_groups[1].id)
-        self.assertEqual('Another group', all_groups[1].name)
-        self.assertEqual('local', all_groups[1].domain_name)
-
-        self.assertEqual('86a66d40-f289-472a-83d0-927b0f954dc8', all_groups[2].id)
-        self.assertEqual('TableauExample', all_groups[2].name)
-        self.assertEqual('local', all_groups[2].domain_name)
+        self.assertEqual("ef8b19c0-43b6-11e6-af50-63f5805dbe3c", all_groups[0].id)
+        self.assertEqual("All Users", all_groups[0].name)
+        self.assertEqual("local", all_groups[0].domain_name)
+
+        self.assertEqual("e7833b48-c6f7-47b5-a2a7-36e7dd232758", all_groups[1].id)
+        self.assertEqual("Another group", all_groups[1].name)
+        self.assertEqual("local", all_groups[1].domain_name)
+
+        self.assertEqual("86a66d40-f289-472a-83d0-927b0f954dc8", all_groups[2].id)
+        self.assertEqual("TableauExample", all_groups[2].name)
+        self.assertEqual("local", all_groups[2].domain_name)
 
-    def test_get_before_signin(self):
+    def test_get_before_signin(self) -> None:
         self.server._auth_token = None
         self.assertRaises(TSC.NotSignedInError, self.server.groups.get)
 
-    def test_populate_users(self):
-        with open(POPULATE_USERS, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
-        with requests_mock.mock() as m:
-            m.get(self.baseurl + '/e7833b48-c6f7-47b5-a2a7-36e7dd232758/users?pageNumber=1&pageSize=100',
-                  text=response_xml, complete_qs=True)
-            single_group = TSC.GroupItem(name='Test Group')
-            single_group._id = 'e7833b48-c6f7-47b5-a2a7-36e7dd232758'
+    def test_populate_users(self) -> None:
+        with open(POPULATE_USERS, "rb") as f:
+            response_xml = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            m.get(
+                self.baseurl + "/e7833b48-c6f7-47b5-a2a7-36e7dd232758/users?pageNumber=1&pageSize=100",
+                text=response_xml,
+                complete_qs=True,
+            )
+            single_group = TSC.GroupItem(name="Test Group")
+            single_group._id = "e7833b48-c6f7-47b5-a2a7-36e7dd232758"
             self.server.groups.populate_users(single_group)
 
             self.assertEqual(1, len(list(single_group.users)))
             user = list(single_group.users).pop()
-            self.assertEqual('dd2239f6-ddf1-4107-981a-4cf94e415794', user.id)
-            self.assertEqual('alice', user.name)
-            self.assertEqual('Publisher', user.site_role)
-            self.assertEqual('2016-08-16T23:17:06Z', format_datetime(user.last_login))
+            self.assertEqual("dd2239f6-ddf1-4107-981a-4cf94e415794", user.id)
+            self.assertEqual("alice", user.name)
+            self.assertEqual("Publisher", user.site_role)
+            self.assertEqual("2016-08-16T23:17:06Z", format_datetime(user.last_login))
 
-    def test_delete(self):
+    def test_delete(self) -> None:
         with requests_mock.mock() as m:
-            m.delete(self.baseurl + '/e7833b48-c6f7-47b5-a2a7-36e7dd232758', status_code=204)
-            self.server.groups.delete('e7833b48-c6f7-47b5-a2a7-36e7dd232758')
+            m.delete(self.baseurl + "/e7833b48-c6f7-47b5-a2a7-36e7dd232758", status_code=204)
+            self.server.groups.delete("e7833b48-c6f7-47b5-a2a7-36e7dd232758")
 
-    def test_remove_user(self):
-        with open(POPULATE_USERS, 'rb') as f:
-            response_xml_populate = f.read().decode('utf-8')
+    def test_remove_user(self) -> None:
+        with open(POPULATE_USERS, "rb") as f:
+            response_xml_populate = f.read().decode("utf-8")
 
-        with open(POPULATE_USERS_EMPTY, 'rb') as f:
-            response_xml_empty = f.read().decode('utf-8')
+        with open(POPULATE_USERS_EMPTY, "rb") as f:
+            response_xml_empty = f.read().decode("utf-8")
 
         with requests_mock.mock() as m:
-            url = self.baseurl + '/e7833b48-c6f7-47b5-a2a7-36e7dd232758/users' \
-                                 '/dd2239f6-ddf1-4107-981a-4cf94e415794'
+            url = self.baseurl + "/e7833b48-c6f7-47b5-a2a7-36e7dd232758/users" "/dd2239f6-ddf1-4107-981a-4cf94e415794"
 
             m.delete(url, status_code=204)
             #  We register the get endpoint twice. The first time we have 1 user, the second we have 'removed' them.
-            m.get(self.baseurl + '/e7833b48-c6f7-47b5-a2a7-36e7dd232758/users', text=response_xml_populate)
+            m.get(self.baseurl + "/e7833b48-c6f7-47b5-a2a7-36e7dd232758/users", text=response_xml_populate)
 
-            single_group = TSC.GroupItem('test')
-            single_group._id = 'e7833b48-c6f7-47b5-a2a7-36e7dd232758'
+            single_group = TSC.GroupItem("test")
+            single_group._id = "e7833b48-c6f7-47b5-a2a7-36e7dd232758"
             self.server.groups.populate_users(single_group)
             self.assertEqual(1, len(list(single_group.users)))
-            self.server.groups.remove_user(single_group, 'dd2239f6-ddf1-4107-981a-4cf94e415794')
+            self.server.groups.remove_user(single_group, "dd2239f6-ddf1-4107-981a-4cf94e415794")
 
-            m.get(self.baseurl + '/e7833b48-c6f7-47b5-a2a7-36e7dd232758/users', text=response_xml_empty)
+            m.get(self.baseurl + "/e7833b48-c6f7-47b5-a2a7-36e7dd232758/users", text=response_xml_empty)
             self.assertEqual(0, len(list(single_group.users)))
 
-    def test_add_user(self):
-        with open(ADD_USER, 'rb') as f:
-            response_xml_add = f.read().decode('utf-8')
-        with open(ADD_USER_POPULATE, 'rb') as f:
-            response_xml_populate = f.read().decode('utf-8')
-        with requests_mock.mock() as m:
-            m.post(self.baseurl + '/e7833b48-c6f7-47b5-a2a7-36e7dd232758/users', text=response_xml_add)
-            m.get(self.baseurl + '/e7833b48-c6f7-47b5-a2a7-36e7dd232758/users', text=response_xml_populate)
-            single_group = TSC.GroupItem('test')
-            single_group._id = 'e7833b48-c6f7-47b5-a2a7-36e7dd232758'
+    def test_add_user(self) -> None:
+        with open(ADD_USER, "rb") as f:
+            response_xml_add = f.read().decode("utf-8")
+        with open(ADD_USER_POPULATE, "rb") as f:
+            response_xml_populate = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            m.post(self.baseurl + "/e7833b48-c6f7-47b5-a2a7-36e7dd232758/users", text=response_xml_add)
+            m.get(self.baseurl + "/e7833b48-c6f7-47b5-a2a7-36e7dd232758/users", text=response_xml_populate)
+            single_group = TSC.GroupItem("test")
+            single_group._id = "e7833b48-c6f7-47b5-a2a7-36e7dd232758"
 
-            self.server.groups.add_user(single_group, '5de011f8-5aa9-4d5b-b991-f462c8dd6bb7')
+            self.server.groups.add_user(single_group, "5de011f8-5aa9-4d5b-b991-f462c8dd6bb7")
             self.server.groups.populate_users(single_group)
             self.assertEqual(1, len(list(single_group.users)))
             user = list(single_group.users).pop()
-            self.assertEqual('5de011f8-5aa9-4d5b-b991-f462c8dd6bb7', user.id)
-            self.assertEqual('testuser', user.name)
-            self.assertEqual('ServerAdministrator', user.site_role)
-
-    def test_add_user_before_populating(self):
-        with open(GET_XML, 'rb') as f:
-            get_xml_response = f.read().decode('utf-8')
-        with open(ADD_USER, 'rb') as f:
-            add_user_response = f.read().decode('utf-8')
+            self.assertEqual("5de011f8-5aa9-4d5b-b991-f462c8dd6bb7", user.id)
+            self.assertEqual("testuser", user.name)
+            self.assertEqual("ServerAdministrator", user.site_role)
+
+    def test_add_user_before_populating(self) -> None:
+        with open(GET_XML, "rb") as f:
+            get_xml_response = f.read().decode("utf-8")
+        with open(ADD_USER, "rb") as f:
+            add_user_response = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             m.get(self.baseurl, text=get_xml_response)
-            m.post('http://test/api/2.3/sites/dad65087-b08b-4603-af4e-2887b8aafc67/groups/ef8b19c0-43b6-11e6-af50'
-                   '-63f5805dbe3c/users', text=add_user_response)
+            m.post(
+                "http://test/api/2.3/sites/dad65087-b08b-4603-af4e-2887b8aafc67/groups/ef8b19c0-43b6-11e6-af50"
+                "-63f5805dbe3c/users",
+                text=add_user_response,
+            )
             all_groups, pagination_item = self.server.groups.get()
             single_group = all_groups[0]
-            self.server.groups.add_user(single_group, '5de011f8-5aa9-4d5b-b991-f462c8dd6bb7')
+            self.server.groups.add_user(single_group, "5de011f8-5aa9-4d5b-b991-f462c8dd6bb7")
 
-    def test_add_user_missing_user_id(self):
-        with open(POPULATE_USERS, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
-        with requests_mock.mock() as m:
-            m.get(self.baseurl + '/e7833b48-c6f7-47b5-a2a7-36e7dd232758/users', text=response_xml)
-            single_group = TSC.GroupItem(name='Test Group')
-            single_group._id = 'e7833b48-c6f7-47b5-a2a7-36e7dd232758'
+    def test_add_user_missing_user_id(self) -> None:
+        with open(POPULATE_USERS, "rb") as f:
+            response_xml = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            m.get(self.baseurl + "/e7833b48-c6f7-47b5-a2a7-36e7dd232758/users", text=response_xml)
+            single_group = TSC.GroupItem(name="Test Group")
+            single_group._id = "e7833b48-c6f7-47b5-a2a7-36e7dd232758"
             self.server.groups.populate_users(single_group)
 
-        self.assertRaises(ValueError, self.server.groups.add_user, single_group, '')
+        self.assertRaises(ValueError, self.server.groups.add_user, single_group, "")
 
-    def test_add_user_missing_group_id(self):
-        single_group = TSC.GroupItem('test')
-        single_group._users = []
-        self.assertRaises(TSC.MissingRequiredFieldError, self.server.groups.add_user, single_group,
-                          '5de011f8-5aa9-4d5b-b991-f462c8dd6bb7')
-
-    def test_remove_user_before_populating(self):
-        with open(GET_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
+    def test_add_user_missing_group_id(self) -> None:
+        single_group = TSC.GroupItem("test")
+        self.assertRaises(
+            TSC.MissingRequiredFieldError,
+            self.server.groups.add_user,
+            single_group,
+            "5de011f8-5aa9-4d5b-b991-f462c8dd6bb7",
+        )
+
+    def test_remove_user_before_populating(self) -> None:
+        with open(GET_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             m.get(self.baseurl, text=response_xml)
-            m.delete('http://test/api/2.3/sites/dad65087-b08b-4603-af4e-2887b8aafc67/groups/ef8b19c0-43b6-11e6-af50'
-                     '-63f5805dbe3c/users/5de011f8-5aa9-4d5b-b991-f462c8dd6bb7',
-                     text='ok')
+            m.delete(
+                "http://test/api/2.3/sites/dad65087-b08b-4603-af4e-2887b8aafc67/groups/ef8b19c0-43b6-11e6-af50"
+                "-63f5805dbe3c/users/5de011f8-5aa9-4d5b-b991-f462c8dd6bb7",
+                text="ok",
+            )
             all_groups, pagination_item = self.server.groups.get()
             single_group = all_groups[0]
-            self.server.groups.remove_user(single_group, '5de011f8-5aa9-4d5b-b991-f462c8dd6bb7')
+            self.server.groups.remove_user(single_group, "5de011f8-5aa9-4d5b-b991-f462c8dd6bb7")
 
-    def test_remove_user_missing_user_id(self):
-        with open(POPULATE_USERS, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
-        with requests_mock.mock() as m:
-            m.get(self.baseurl + '/e7833b48-c6f7-47b5-a2a7-36e7dd232758/users', text=response_xml)
-            single_group = TSC.GroupItem(name='Test Group')
-            single_group._id = 'e7833b48-c6f7-47b5-a2a7-36e7dd232758'
+    def test_remove_user_missing_user_id(self) -> None:
+        with open(POPULATE_USERS, "rb") as f:
+            response_xml = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            m.get(self.baseurl + "/e7833b48-c6f7-47b5-a2a7-36e7dd232758/users", text=response_xml)
+            single_group = TSC.GroupItem(name="Test Group")
+            single_group._id = "e7833b48-c6f7-47b5-a2a7-36e7dd232758"
             self.server.groups.populate_users(single_group)
 
-        self.assertRaises(ValueError, self.server.groups.remove_user, single_group, '')
+        self.assertRaises(ValueError, self.server.groups.remove_user, single_group, "")
 
-    def test_remove_user_missing_group_id(self):
-        single_group = TSC.GroupItem('test')
-        single_group._users = []
-        self.assertRaises(TSC.MissingRequiredFieldError, self.server.groups.remove_user, single_group,
-                          '5de011f8-5aa9-4d5b-b991-f462c8dd6bb7')
-
-    def test_create_group(self):
-        with open(CREATE_GROUP, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
+    def test_remove_user_missing_group_id(self) -> None:
+        single_group = TSC.GroupItem("test")
+        self.assertRaises(
+            TSC.MissingRequiredFieldError,
+            self.server.groups.remove_user,
+            single_group,
+            "5de011f8-5aa9-4d5b-b991-f462c8dd6bb7",
+        )
+
+    def test_create_group(self) -> None:
+        with open(CREATE_GROUP, "rb") as f:
+            response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             m.post(self.baseurl, text=response_xml)
-            group_to_create = TSC.GroupItem(u'試供品')
+            group_to_create = TSC.GroupItem("試供品")
             group = self.server.groups.create(group_to_create)
-            self.assertEqual(group.name, u'試供品')
-            self.assertEqual(group.id, '3e4a9ea0-a07a-4fe6-b50f-c345c8c81034')
+            self.assertEqual(group.name, "試供品")
+            self.assertEqual(group.id, "3e4a9ea0-a07a-4fe6-b50f-c345c8c81034")
 
-    def test_update(self):
-        with open(UPDATE_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
-        with requests_mock.mock() as m:
-            m.put(self.baseurl + '/ef8b19c0-43b6-11e6-af50-63f5805dbe3c', text=response_xml)
-            group = TSC.GroupItem(name='Test Group')
-            group._domain_name = 'local'
-            group._id = 'ef8b19c0-43b6-11e6-af50-63f5805dbe3c'
+    def test_create_ad_group(self) -> None:
+        with open(CREATE_GROUP_AD, "rb") as f:
+            response_xml = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            m.post(self.baseurl, text=response_xml)
+            group_to_create = TSC.GroupItem("試供品")
+            group_to_create.domain_name = "just-has-to-exist"
+            group = self.server.groups.create_AD_group(group_to_create, False)
+            self.assertEqual(group.name, "試供品")
+            self.assertEqual(group.license_mode, "onLogin")
+            self.assertEqual(group.minimum_site_role, "Creator")
+            self.assertEqual(group.domain_name, "active-directory-domain-name")
+
+    def test_create_group_async(self) -> None:
+        with open(CREATE_GROUP_ASYNC, "rb") as f:
+            response_xml = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            m.post(self.baseurl, text=response_xml)
+            group_to_create = TSC.GroupItem("試供品")
+            group_to_create.domain_name = "woohoo"
+            job = self.server.groups.create_AD_group(group_to_create, True)
+            self.assertEqual(job.mode, "Asynchronous")
+            self.assertEqual(job.type, "GroupImport")
+
+    def test_update(self) -> None:
+        with open(UPDATE_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            m.put(self.baseurl + "/ef8b19c0-43b6-11e6-af50-63f5805dbe3c", text=response_xml)
+            group = TSC.GroupItem(name="Test Group")
+            group._domain_name = "local"
+            group._id = "ef8b19c0-43b6-11e6-af50-63f5805dbe3c"
             group = self.server.groups.update(group)
 
-        self.assertEqual('ef8b19c0-43b6-11e6-af50-63f5805dbe3c', group.id)
-        self.assertEqual('Group updated name', group.name)
+        self.assertEqual("ef8b19c0-43b6-11e6-af50-63f5805dbe3c", group.id)
+        self.assertEqual("Group updated name", group.name)
+        self.assertEqual("ExplorerCanPublish", group.minimum_site_role)
+        self.assertEqual("onLogin", group.license_mode)
+
+    # async update is not supported for local groups
+    def test_update_local_async(self) -> None:
+        group = TSC.GroupItem("myGroup")
+        group._id = "ef8b19c0-43b6-11e6-af50-63f5805dbe3c"
+        self.assertRaises(ValueError, self.server.groups.update, group, as_job=True)
+
+        # mimic group returned from server where domain name is set to 'local'
+        group.domain_name = "local"
+        self.assertRaises(ValueError, self.server.groups.update, group, as_job=True)
```

### Comparing `tableauserverclient-0.9/test/test_auth.py` & `tableauserverclient-0.9.31.post0.dev1/test/test_auth.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,128 @@
-import unittest
 import os.path
+import unittest
+
 import requests_mock
+
 import tableauserverclient as TSC
 
-TEST_ASSET_DIR = os.path.join(os.path.dirname(__file__), 'assets')
+TEST_ASSET_DIR = os.path.join(os.path.dirname(__file__), "assets")
 
-SIGN_IN_XML = os.path.join(TEST_ASSET_DIR, 'auth_sign_in.xml')
-SIGN_IN_IMPERSONATE_XML = os.path.join(TEST_ASSET_DIR, 'auth_sign_in_impersonate.xml')
-SIGN_IN_ERROR_XML = os.path.join(TEST_ASSET_DIR, 'auth_sign_in_error.xml')
+SIGN_IN_XML = os.path.join(TEST_ASSET_DIR, "auth_sign_in.xml")
+SIGN_IN_IMPERSONATE_XML = os.path.join(TEST_ASSET_DIR, "auth_sign_in_impersonate.xml")
+SIGN_IN_ERROR_XML = os.path.join(TEST_ASSET_DIR, "auth_sign_in_error.xml")
 
 
 class AuthTests(unittest.TestCase):
     def setUp(self):
-        self.server = TSC.Server('http://test')
+        self.server = TSC.Server("http://test", False)
         self.baseurl = self.server.auth.baseurl
 
     def test_sign_in(self):
-        with open(SIGN_IN_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
+        with open(SIGN_IN_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
-            m.post(self.baseurl + '/signin', text=response_xml)
-            tableau_auth = TSC.TableauAuth('testuser', 'password', site_id='Samples')
+            m.post(self.baseurl + "/signin", text=response_xml)
+            tableau_auth = TSC.TableauAuth("testuser", "password", site_id="Samples")
             self.server.auth.sign_in(tableau_auth)
 
-        self.assertEqual('eIX6mvFsqyansa4KqEI1UwOpS8ggRs2l', self.server.auth_token)
-        self.assertEqual('6b7179ba-b82b-4f0f-91ed-812074ac5da6', self.server.site_id)
-        self.assertEqual('1a96d216-e9b8-497b-a82a-0b899a965e01', self.server.user_id)
+        self.assertEqual("eIX6mvFsqyansa4KqEI1UwOpS8ggRs2l", self.server.auth_token)
+        self.assertEqual("6b7179ba-b82b-4f0f-91ed-812074ac5da6", self.server.site_id)
+        self.assertEqual("1a96d216-e9b8-497b-a82a-0b899a965e01", self.server.user_id)
 
     def test_sign_in_with_personal_access_tokens(self):
-        with open(SIGN_IN_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
+        with open(SIGN_IN_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
-            m.post(self.baseurl + '/signin', text=response_xml)
-            tableau_auth = TSC.PersonalAccessTokenAuth(token_name='mytoken',
-                                                       personal_access_token='Random123Generated', site_id='Samples')
+            m.post(self.baseurl + "/signin", text=response_xml)
+            tableau_auth = TSC.PersonalAccessTokenAuth(
+                token_name="mytoken", personal_access_token="Random123Generated", site_id="Samples"
+            )
             self.server.auth.sign_in(tableau_auth)
 
-        self.assertEqual('eIX6mvFsqyansa4KqEI1UwOpS8ggRs2l', self.server.auth_token)
-        self.assertEqual('6b7179ba-b82b-4f0f-91ed-812074ac5da6', self.server.site_id)
-        self.assertEqual('1a96d216-e9b8-497b-a82a-0b899a965e01', self.server.user_id)
+        self.assertEqual("eIX6mvFsqyansa4KqEI1UwOpS8ggRs2l", self.server.auth_token)
+        self.assertEqual("6b7179ba-b82b-4f0f-91ed-812074ac5da6", self.server.site_id)
+        self.assertEqual("1a96d216-e9b8-497b-a82a-0b899a965e01", self.server.user_id)
 
     def test_sign_in_impersonate(self):
-        with open(SIGN_IN_IMPERSONATE_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
+        with open(SIGN_IN_IMPERSONATE_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
-            m.post(self.baseurl + '/signin', text=response_xml)
-            tableau_auth = TSC.TableauAuth('testuser', 'password',
-                                           user_id_to_impersonate='dd2239f6-ddf1-4107-981a-4cf94e415794')
+            m.post(self.baseurl + "/signin", text=response_xml)
+            tableau_auth = TSC.TableauAuth(
+                "testuser", "password", user_id_to_impersonate="dd2239f6-ddf1-4107-981a-4cf94e415794"
+            )
             self.server.auth.sign_in(tableau_auth)
 
-        self.assertEqual('MJonFA6HDyy2C3oqR13fRGqE6cmgzwq3', self.server.auth_token)
-        self.assertEqual('dad65087-b08b-4603-af4e-2887b8aafc67', self.server.site_id)
-        self.assertEqual('dd2239f6-ddf1-4107-981a-4cf94e415794', self.server.user_id)
+        self.assertEqual("MJonFA6HDyy2C3oqR13fRGqE6cmgzwq3", self.server.auth_token)
+        self.assertEqual("dad65087-b08b-4603-af4e-2887b8aafc67", self.server.site_id)
+        self.assertEqual("dd2239f6-ddf1-4107-981a-4cf94e415794", self.server.user_id)
 
     def test_sign_in_error(self):
-        with open(SIGN_IN_ERROR_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
+        with open(SIGN_IN_ERROR_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
-            m.post(self.baseurl + '/signin', text=response_xml, status_code=401)
-            tableau_auth = TSC.TableauAuth('testuser', 'wrongpassword')
+            m.post(self.baseurl + "/signin", text=response_xml, status_code=401)
+            tableau_auth = TSC.TableauAuth("testuser", "wrongpassword")
             self.assertRaises(TSC.ServerResponseError, self.server.auth.sign_in, tableau_auth)
 
     def test_sign_in_invalid_token(self):
-        with open(SIGN_IN_ERROR_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
+        with open(SIGN_IN_ERROR_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
-            m.post(self.baseurl + '/signin', text=response_xml, status_code=401)
-            tableau_auth = TSC.PersonalAccessTokenAuth(token_name='mytoken', personal_access_token='invalid')
+            m.post(self.baseurl + "/signin", text=response_xml, status_code=401)
+            tableau_auth = TSC.PersonalAccessTokenAuth(token_name="mytoken", personal_access_token="invalid")
             self.assertRaises(TSC.ServerResponseError, self.server.auth.sign_in, tableau_auth)
 
     def test_sign_in_without_auth(self):
-        with open(SIGN_IN_ERROR_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
+        with open(SIGN_IN_ERROR_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
-            m.post(self.baseurl + '/signin', text=response_xml, status_code=401)
-            tableau_auth = TSC.TableauAuth('', '')
+            m.post(self.baseurl + "/signin", text=response_xml, status_code=401)
+            tableau_auth = TSC.TableauAuth("", "")
             self.assertRaises(TSC.ServerResponseError, self.server.auth.sign_in, tableau_auth)
 
     def test_sign_out(self):
-        with open(SIGN_IN_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
+        with open(SIGN_IN_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
-            m.post(self.baseurl + '/signin', text=response_xml)
-            m.post(self.baseurl + '/signout', text='')
-            tableau_auth = TSC.TableauAuth('testuser', 'password')
+            m.post(self.baseurl + "/signin", text=response_xml)
+            m.post(self.baseurl + "/signout", text="")
+            tableau_auth = TSC.TableauAuth("testuser", "password")
             self.server.auth.sign_in(tableau_auth)
             self.server.auth.sign_out()
 
         self.assertIsNone(self.server._auth_token)
         self.assertIsNone(self.server._site_id)
         self.assertIsNone(self.server._user_id)
+
+    def test_switch_site(self):
+        self.server.version = "2.6"
+        baseurl = self.server.auth.baseurl
+        site_id, user_id, auth_token = list("123")
+        self.server._set_auth(site_id, user_id, auth_token)
+        with open(SIGN_IN_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            m.post(baseurl + "/switchSite", text=response_xml)
+            site = TSC.SiteItem("Samples", "Samples")
+            self.server.auth.switch_site(site)
+
+        self.assertEqual("eIX6mvFsqyansa4KqEI1UwOpS8ggRs2l", self.server.auth_token)
+        self.assertEqual("6b7179ba-b82b-4f0f-91ed-812074ac5da6", self.server.site_id)
+        self.assertEqual("1a96d216-e9b8-497b-a82a-0b899a965e01", self.server.user_id)
+
+    def test_revoke_all_server_admin_tokens(self):
+        self.server.version = "3.10"
+        baseurl = self.server.auth.baseurl
+        with open(SIGN_IN_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            m.post(baseurl + "/signin", text=response_xml)
+            m.post(baseurl + "/revokeAllServerAdminTokens", text="")
+            tableau_auth = TSC.TableauAuth("testuser", "password")
+            self.server.auth.sign_in(tableau_auth)
+            self.server.auth.revoke_all_server_admin_tokens()
+
+        self.assertEqual("eIX6mvFsqyansa4KqEI1UwOpS8ggRs2l", self.server.auth_token)
+        self.assertEqual("6b7179ba-b82b-4f0f-91ed-812074ac5da6", self.server.site_id)
+        self.assertEqual("1a96d216-e9b8-497b-a82a-0b899a965e01", self.server.user_id)
```

### Comparing `tableauserverclient-0.9/test/test_project_model.py` & `tableauserverclient-0.9.31.post0.dev1/test/test_project_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+
 import tableauserverclient as TSC
 
 
 class ProjectModelTests(unittest.TestCase):
     def test_invalid_name(self):
         self.assertRaises(ValueError, TSC.ProjectItem, None)
         self.assertRaises(ValueError, TSC.ProjectItem, "")
@@ -18,7 +19,12 @@
         with self.assertRaises(ValueError):
             project.content_permissions = "Hello"
 
     def test_parent_id(self):
         project = TSC.ProjectItem("proj")
         project.parent_id = "foo"
         self.assertEqual(project.parent_id, "foo")
+
+    def test_owner_id(self):
+        project = TSC.ProjectItem("proj")
+        with self.assertRaises(NotImplementedError):
+            project.owner_id = "new_owner"
```

### Comparing `tableauserverclient-0.9/test/test_sort.py` & `tableauserverclient-0.9.31.post0.dev1/test/test_sort.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,103 @@
+import re
 import unittest
-import os
-import requests
+
 import requests_mock
+
 import tableauserverclient as TSC
 
 
 class SortTests(unittest.TestCase):
     def setUp(self):
-        self.server = TSC.Server('http://test')
-        self.server._site_id = 'dad65087-b08b-4603-af4e-2887b8aafc67'
-        self.server._auth_token = 'j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM'
+        self.server = TSC.Server("http://test", False)
+        self.server.version = "3.10"
+        self.server._site_id = "dad65087-b08b-4603-af4e-2887b8aafc67"
+        self.server._auth_token = "j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM"
         self.baseurl = self.server.workbooks.baseurl
 
     def test_empty_filter(self):
         self.assertRaises(TypeError, TSC.Filter, "")
 
     def test_filter_equals(self):
         with requests_mock.mock() as m:
             m.get(requests_mock.ANY)
             url = "http://test/api/2.3/sites/dad65087-b08b-4603-af4e-2887b8aafc67/workbooks"
             opts = TSC.RequestOptions(pagesize=13, pagenumber=13)
-            opts.filter.add(TSC.Filter(TSC.RequestOptions.Field.Name,
-                                       TSC.RequestOptions.Operator.Equals,
-                                       'Superstore'))
-
-            resp = self.server.workbooks._make_request(requests.get,
-                                                       url,
-                                                       content=None,
-                                                       request_object=opts,
-                                                       auth_token='j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM',
-                                                       content_type='text/xml')
+            opts.filter.add(TSC.Filter(TSC.RequestOptions.Field.Name, TSC.RequestOptions.Operator.Equals, "Superstore"))
 
-            self.assertEqual(resp.request.query, 'pagenumber=13&pagesize=13&filter=name:eq:superstore')
+            resp = self.server.workbooks.get_request(url, request_object=opts)
+
+            self.assertTrue(re.search("pagenumber=13", resp.request.query))
+            self.assertTrue(re.search("pagesize=13", resp.request.query))
+            self.assertTrue(re.search("filter=name%3aeq%3asuperstore", resp.request.query))
 
     def test_filter_equals_list(self):
         with self.assertRaises(ValueError) as cm:
-            TSC.Filter(TSC.RequestOptions.Field.Tags,
-                       TSC.RequestOptions.Operator.Equals,
-                       ['foo', 'bar'])
+            TSC.Filter(TSC.RequestOptions.Field.Tags, TSC.RequestOptions.Operator.Equals, ["foo", "bar"])
 
         self.assertEqual("Filter values can only be a list if the operator is 'in'.", str(cm.exception)),
 
     def test_filter_in(self):
         with requests_mock.mock() as m:
             m.get(requests_mock.ANY)
             url = "http://test/api/2.3/sites/dad65087-b08b-4603-af4e-2887b8aafc67/workbooks"
             opts = TSC.RequestOptions(pagesize=13, pagenumber=13)
 
-            opts.filter.add(TSC.Filter(TSC.RequestOptions.Field.Tags,
-                                       TSC.RequestOptions.Operator.In,
-                                       ['stocks', 'market']))
-
-            resp = self.server.workbooks._make_request(requests.get,
-                                                       url,
-                                                       content=None,
-                                                       request_object=opts,
-                                                       auth_token='j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM',
-                                                       content_type='text/xml')
-            self.assertEqual(resp.request.query, 'pagenumber=13&pagesize=13&filter=tags:in:[stocks,market]')
+            opts.filter.add(
+                TSC.Filter(TSC.RequestOptions.Field.Tags, TSC.RequestOptions.Operator.In, ["stocks", "market"])
+            )
+
+            resp = self.server.workbooks.get_request(url, request_object=opts)
+            self.assertTrue(re.search("pagenumber=13", resp.request.query))
+            self.assertTrue(re.search("pagesize=13", resp.request.query))
+            self.assertTrue(re.search("filter=tags%3ain%3a%5bstocks%2cmarket%5d", resp.request.query))
 
     def test_sort_asc(self):
         with requests_mock.mock() as m:
             m.get(requests_mock.ANY)
             url = "http://test/api/2.3/sites/dad65087-b08b-4603-af4e-2887b8aafc67/workbooks"
             opts = TSC.RequestOptions(pagesize=13, pagenumber=13)
-            opts.sort.add(TSC.Sort(TSC.RequestOptions.Field.Name,
-                                   TSC.RequestOptions.Direction.Asc))
+            opts.sort.add(TSC.Sort(TSC.RequestOptions.Field.Name, TSC.RequestOptions.Direction.Asc))
 
-            resp = self.server.workbooks._make_request(requests.get,
-                                                       url,
-                                                       content=None,
-                                                       request_object=opts,
-                                                       auth_token='j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM',
-                                                       content_type='text/xml')
+            resp = self.server.workbooks.get_request(url, request_object=opts)
 
-            self.assertEqual(resp.request.query, 'pagenumber=13&pagesize=13&sort=name:asc')
+            self.assertTrue(re.search("pagenumber=13", resp.request.query))
+            self.assertTrue(re.search("pagesize=13", resp.request.query))
+            self.assertTrue(re.search("sort=name%3aasc", resp.request.query))
 
     def test_filter_combo(self):
         with requests_mock.mock() as m:
             m.get(requests_mock.ANY)
             url = "http://test/api/2.3/sites/dad65087-b08b-4603-af4e-2887b8aafc67/users"
             opts = TSC.RequestOptions(pagesize=13, pagenumber=13)
 
-            opts.filter.add(TSC.Filter(TSC.RequestOptions.Field.LastLogin,
-                                       TSC.RequestOptions.Operator.GreaterThanOrEqual,
-                                       '2017-01-15T00:00:00:00Z'))
-
-            opts.filter.add(TSC.Filter(TSC.RequestOptions.Field.SiteRole,
-                                       TSC.RequestOptions.Operator.Equals,
-                                       'Publisher'))
-
-            resp = self.server.workbooks._make_request(requests.get,
-                                                       url,
-                                                       content=None,
-                                                       request_object=opts,
-                                                       auth_token='j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM',
-                                                       content_type='text/xml')
-
-            expected = 'pagenumber=13&pagesize=13&filter=lastlogin:gte:2017-01-15t00:00:00:00z,siterole:eq:publisher'
-
-            self.assertEqual(resp.request.query, expected)
+            opts.filter.add(
+                TSC.Filter(
+                    TSC.RequestOptions.Field.LastLogin,
+                    TSC.RequestOptions.Operator.GreaterThanOrEqual,
+                    "2017-01-15T00:00:00:00Z",
+                )
+            )
+
+            opts.filter.add(
+                TSC.Filter(TSC.RequestOptions.Field.SiteRole, TSC.RequestOptions.Operator.Equals, "Publisher")
+            )
+
+            resp = self.server.workbooks.get_request(url, request_object=opts)
+
+            expected = (
+                "pagenumber=13&pagesize=13&filter=lastlogin%3agte%3a"
+                "2017-01-15t00%3a00%3a00%3a00z%2csiterole%3aeq%3apublisher"
+            )
+
+            self.assertTrue(re.search("pagenumber=13", resp.request.query))
+            self.assertTrue(re.search("pagesize=13", resp.request.query))
+            self.assertTrue(
+                re.search(
+                    "filter=lastlogin%3agte%3a2017-01-15t00%3a00%3a00%3a00z%2csiterole%3aeq%3apublisher",
+                    resp.request.query,
+                )
+            )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `tableauserverclient-0.9/test/test_schedule.py` & `tableauserverclient-0.9.31.post0.dev1/test/test_schedule.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,45 @@
-from datetime import time
-import unittest
 import os
+import unittest
+from datetime import time
+
 import requests_mock
+
 import tableauserverclient as TSC
 from tableauserverclient.datetime_helpers import format_datetime
 
 TEST_ASSET_DIR = os.path.join(os.path.dirname(__file__), "assets")
 
 GET_XML = os.path.join(TEST_ASSET_DIR, "schedule_get.xml")
+GET_BY_ID_XML = os.path.join(TEST_ASSET_DIR, "schedule_get_by_id.xml")
 GET_EMPTY_XML = os.path.join(TEST_ASSET_DIR, "schedule_get_empty.xml")
 CREATE_HOURLY_XML = os.path.join(TEST_ASSET_DIR, "schedule_create_hourly.xml")
 CREATE_DAILY_XML = os.path.join(TEST_ASSET_DIR, "schedule_create_daily.xml")
 CREATE_WEEKLY_XML = os.path.join(TEST_ASSET_DIR, "schedule_create_weekly.xml")
 CREATE_MONTHLY_XML = os.path.join(TEST_ASSET_DIR, "schedule_create_monthly.xml")
 UPDATE_XML = os.path.join(TEST_ASSET_DIR, "schedule_update.xml")
+ADD_WORKBOOK_TO_SCHEDULE = os.path.join(TEST_ASSET_DIR, "schedule_add_workbook.xml")
+ADD_WORKBOOK_TO_SCHEDULE_WITH_WARNINGS = os.path.join(TEST_ASSET_DIR, "schedule_add_workbook_with_warnings.xml")
+ADD_DATASOURCE_TO_SCHEDULE = os.path.join(TEST_ASSET_DIR, "schedule_add_datasource.xml")
 
-WORKBOOK_GET_BY_ID_XML = os.path.join(TEST_ASSET_DIR, 'workbook_get_by_id.xml')
-DATASOURCE_GET_BY_ID_XML = os.path.join(TEST_ASSET_DIR, 'datasource_get_by_id.xml')
+WORKBOOK_GET_BY_ID_XML = os.path.join(TEST_ASSET_DIR, "workbook_get_by_id.xml")
+DATASOURCE_GET_BY_ID_XML = os.path.join(TEST_ASSET_DIR, "datasource_get_by_id.xml")
 
 
 class ScheduleTests(unittest.TestCase):
-    def setUp(self):
-        self.server = TSC.Server("http://test")
+    def setUp(self) -> None:
+        self.server = TSC.Server("http://test", False)
 
         # Fake Signin
         self.server._site_id = "dad65087-b08b-4603-af4e-2887b8aafc67"
         self.server._auth_token = "j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM"
 
         self.baseurl = self.server.schedules.baseurl
 
-    def test_get(self):
+    def test_get(self) -> None:
         with open(GET_XML, "rb") as f:
             response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             m.get(self.baseurl, text=response_xml)
             all_schedules, pagination_item = self.server.schedules.get()
 
         extract = all_schedules[0]
@@ -64,165 +70,247 @@
         self.assertEqual("Active", flow.state)
         self.assertEqual(50, flow.priority)
         self.assertEqual("2019-02-19T18:52:19Z", format_datetime(flow.created_at))
         self.assertEqual("2019-02-19T18:55:51Z", format_datetime(flow.updated_at))
         self.assertEqual("Flow", flow.schedule_type)
         self.assertEqual("2019-03-01T09:00:00Z", format_datetime(flow.next_run_at))
 
-    def test_get_empty(self):
+    def test_get_empty(self) -> None:
         with open(GET_EMPTY_XML, "rb") as f:
             response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             m.get(self.baseurl, text=response_xml)
             all_schedules, pagination_item = self.server.schedules.get()
 
         self.assertEqual(0, pagination_item.total_available)
         self.assertEqual([], all_schedules)
 
-    def test_delete(self):
+    def test_get_by_id(self) -> None:
+        self.server.version = "3.8"
+        with open(GET_BY_ID_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            schedule_id = "c9cff7f9-309c-4361-99ff-d4ba8c9f5467"
+            baseurl = "{}/schedules/{}".format(self.server.baseurl, schedule_id)
+            m.get(baseurl, text=response_xml)
+            schedule = self.server.schedules.get_by_id(schedule_id)
+            self.assertIsNotNone(schedule)
+            self.assertEqual(schedule_id, schedule.id)
+            self.assertEqual("Weekday early mornings", schedule.name)
+            self.assertEqual("Active", schedule.state)
+
+    def test_delete(self) -> None:
         with requests_mock.mock() as m:
             m.delete(self.baseurl + "/c9cff7f9-309c-4361-99ff-d4ba8c9f5467", status_code=204)
             self.server.schedules.delete("c9cff7f9-309c-4361-99ff-d4ba8c9f5467")
 
-    def test_create_hourly(self):
+    def test_create_hourly(self) -> None:
         with open(CREATE_HOURLY_XML, "rb") as f:
             response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             m.post(self.baseurl, text=response_xml)
-            hourly_interval = TSC.HourlyInterval(start_time=time(2, 30),
-                                                 end_time=time(23, 0),
-                                                 interval_value=2)
-            new_schedule = TSC.ScheduleItem("hourly-schedule-1", 50, TSC.ScheduleItem.Type.Extract,
-                                            TSC.ScheduleItem.ExecutionOrder.Parallel, hourly_interval)
+            hourly_interval = TSC.HourlyInterval(start_time=time(2, 30), end_time=time(23, 0), interval_value=2)
+            new_schedule = TSC.ScheduleItem(
+                "hourly-schedule-1",
+                50,
+                TSC.ScheduleItem.Type.Extract,
+                TSC.ScheduleItem.ExecutionOrder.Parallel,
+                hourly_interval,
+            )
             new_schedule = self.server.schedules.create(new_schedule)
 
         self.assertEqual("5f42be25-8a43-47ba-971a-63f2d4e7029c", new_schedule.id)
         self.assertEqual("hourly-schedule-1", new_schedule.name)
         self.assertEqual("Active", new_schedule.state)
         self.assertEqual(50, new_schedule.priority)
         self.assertEqual("2016-09-15T20:47:33Z", format_datetime(new_schedule.created_at))
         self.assertEqual("2016-09-15T20:47:33Z", format_datetime(new_schedule.updated_at))
         self.assertEqual(TSC.ScheduleItem.Type.Extract, new_schedule.schedule_type)
         self.assertEqual("2016-09-16T01:30:00Z", format_datetime(new_schedule.next_run_at))
         self.assertEqual(TSC.ScheduleItem.ExecutionOrder.Parallel, new_schedule.execution_order)
         self.assertEqual(time(2, 30), new_schedule.interval_item.start_time)
-        self.assertEqual(time(23), new_schedule.interval_item.end_time)
-        self.assertEqual("8", new_schedule.interval_item.interval)
+        self.assertEqual(time(23), new_schedule.interval_item.end_time)  # type: ignore[union-attr]
+        self.assertEqual("8", new_schedule.interval_item.interval)  # type: ignore[union-attr]
 
-    def test_create_daily(self):
+    def test_create_daily(self) -> None:
         with open(CREATE_DAILY_XML, "rb") as f:
             response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             m.post(self.baseurl, text=response_xml)
             daily_interval = TSC.DailyInterval(time(4, 50))
-            new_schedule = TSC.ScheduleItem("daily-schedule-1", 90, TSC.ScheduleItem.Type.Subscription,
-                                            TSC.ScheduleItem.ExecutionOrder.Serial, daily_interval)
+            new_schedule = TSC.ScheduleItem(
+                "daily-schedule-1",
+                90,
+                TSC.ScheduleItem.Type.Subscription,
+                TSC.ScheduleItem.ExecutionOrder.Serial,
+                daily_interval,
+            )
             new_schedule = self.server.schedules.create(new_schedule)
 
         self.assertEqual("907cae38-72fd-417c-892a-95540c4664cd", new_schedule.id)
         self.assertEqual("daily-schedule-1", new_schedule.name)
         self.assertEqual("Active", new_schedule.state)
         self.assertEqual(90, new_schedule.priority)
         self.assertEqual("2016-09-15T21:01:09Z", format_datetime(new_schedule.created_at))
         self.assertEqual("2016-09-15T21:01:09Z", format_datetime(new_schedule.updated_at))
         self.assertEqual(TSC.ScheduleItem.Type.Subscription, new_schedule.schedule_type)
         self.assertEqual("2016-09-16T11:45:00Z", format_datetime(new_schedule.next_run_at))
         self.assertEqual(TSC.ScheduleItem.ExecutionOrder.Serial, new_schedule.execution_order)
         self.assertEqual(time(4, 45), new_schedule.interval_item.start_time)
 
-    def test_create_weekly(self):
+    def test_create_weekly(self) -> None:
         with open(CREATE_WEEKLY_XML, "rb") as f:
             response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             m.post(self.baseurl, text=response_xml)
-            weekly_interval = TSC.WeeklyInterval(time(9, 15), TSC.IntervalItem.Day.Monday,
-                                                 TSC.IntervalItem.Day.Wednesday,
-                                                 TSC.IntervalItem.Day.Friday)
-            new_schedule = TSC.ScheduleItem("weekly-schedule-1", 80, TSC.ScheduleItem.Type.Extract,
-                                            TSC.ScheduleItem.ExecutionOrder.Parallel, weekly_interval)
+            weekly_interval = TSC.WeeklyInterval(
+                time(9, 15), TSC.IntervalItem.Day.Monday, TSC.IntervalItem.Day.Wednesday, TSC.IntervalItem.Day.Friday
+            )
+            new_schedule = TSC.ScheduleItem(
+                "weekly-schedule-1",
+                80,
+                TSC.ScheduleItem.Type.Extract,
+                TSC.ScheduleItem.ExecutionOrder.Parallel,
+                weekly_interval,
+            )
             new_schedule = self.server.schedules.create(new_schedule)
 
         self.assertEqual("1adff386-6be0-4958-9f81-a35e676932bf", new_schedule.id)
         self.assertEqual("weekly-schedule-1", new_schedule.name)
         self.assertEqual("Active", new_schedule.state)
         self.assertEqual(80, new_schedule.priority)
         self.assertEqual("2016-09-15T21:12:50Z", format_datetime(new_schedule.created_at))
         self.assertEqual("2016-09-15T21:12:50Z", format_datetime(new_schedule.updated_at))
         self.assertEqual(TSC.ScheduleItem.Type.Extract, new_schedule.schedule_type)
         self.assertEqual("2016-09-16T16:15:00Z", format_datetime(new_schedule.next_run_at))
         self.assertEqual(TSC.ScheduleItem.ExecutionOrder.Parallel, new_schedule.execution_order)
         self.assertEqual(time(9, 15), new_schedule.interval_item.start_time)
-        self.assertEqual(("Monday", "Wednesday", "Friday"),
-                         new_schedule.interval_item.interval)
+        self.assertEqual(("Monday", "Wednesday", "Friday"), new_schedule.interval_item.interval)
+        self.assertEqual(2, len(new_schedule.warnings))
+        self.assertEqual("warning 1", new_schedule.warnings[0])
+        self.assertEqual("warning 2", new_schedule.warnings[1])
 
-    def test_create_monthly(self):
+    def test_create_monthly(self) -> None:
         with open(CREATE_MONTHLY_XML, "rb") as f:
             response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             m.post(self.baseurl, text=response_xml)
             monthly_interval = TSC.MonthlyInterval(time(7), 12)
-            new_schedule = TSC.ScheduleItem("monthly-schedule-1", 20, TSC.ScheduleItem.Type.Extract,
-                                            TSC.ScheduleItem.ExecutionOrder.Serial, monthly_interval)
+            new_schedule = TSC.ScheduleItem(
+                "monthly-schedule-1",
+                20,
+                TSC.ScheduleItem.Type.Extract,
+                TSC.ScheduleItem.ExecutionOrder.Serial,
+                monthly_interval,
+            )
             new_schedule = self.server.schedules.create(new_schedule)
 
         self.assertEqual("e06a7c75-5576-4f68-882d-8909d0219326", new_schedule.id)
         self.assertEqual("monthly-schedule-1", new_schedule.name)
         self.assertEqual("Active", new_schedule.state)
         self.assertEqual(20, new_schedule.priority)
         self.assertEqual("2016-09-15T21:16:56Z", format_datetime(new_schedule.created_at))
         self.assertEqual("2016-09-15T21:16:56Z", format_datetime(new_schedule.updated_at))
         self.assertEqual(TSC.ScheduleItem.Type.Extract, new_schedule.schedule_type)
         self.assertEqual("2016-10-12T14:00:00Z", format_datetime(new_schedule.next_run_at))
         self.assertEqual(TSC.ScheduleItem.ExecutionOrder.Serial, new_schedule.execution_order)
         self.assertEqual(time(7), new_schedule.interval_item.start_time)
-        self.assertEqual("12", new_schedule.interval_item.interval)
+        self.assertEqual("12", new_schedule.interval_item.interval)  # type: ignore[union-attr]
 
-    def test_update(self):
+    def test_update(self) -> None:
         with open(UPDATE_XML, "rb") as f:
             response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
-            m.put(self.baseurl + '/7bea1766-1543-4052-9753-9d224bc069b5', text=response_xml)
-            new_interval = TSC.WeeklyInterval(time(7), TSC.IntervalItem.Day.Monday,
-                                              TSC.IntervalItem.Day.Friday)
-            single_schedule = TSC.ScheduleItem("weekly-schedule-1", 90, TSC.ScheduleItem.Type.Extract,
-                                               TSC.ScheduleItem.ExecutionOrder.Parallel, new_interval)
+            m.put(self.baseurl + "/7bea1766-1543-4052-9753-9d224bc069b5", text=response_xml)
+            new_interval = TSC.WeeklyInterval(time(7), TSC.IntervalItem.Day.Monday, TSC.IntervalItem.Day.Friday)
+            single_schedule = TSC.ScheduleItem(
+                "weekly-schedule-1",
+                90,
+                TSC.ScheduleItem.Type.Extract,
+                TSC.ScheduleItem.ExecutionOrder.Parallel,
+                new_interval,
+            )
             single_schedule._id = "7bea1766-1543-4052-9753-9d224bc069b5"
+            single_schedule.state = TSC.ScheduleItem.State.Suspended
             single_schedule = self.server.schedules.update(single_schedule)
 
         self.assertEqual("7bea1766-1543-4052-9753-9d224bc069b5", single_schedule.id)
         self.assertEqual("weekly-schedule-1", single_schedule.name)
         self.assertEqual(90, single_schedule.priority)
         self.assertEqual("2016-09-15T23:50:02Z", format_datetime(single_schedule.updated_at))
         self.assertEqual(TSC.ScheduleItem.Type.Extract, single_schedule.schedule_type)
         self.assertEqual("2016-09-16T14:00:00Z", format_datetime(single_schedule.next_run_at))
         self.assertEqual(TSC.ScheduleItem.ExecutionOrder.Parallel, single_schedule.execution_order)
         self.assertEqual(time(7), single_schedule.interval_item.start_time)
-        self.assertEqual(("Monday", "Friday"),
-                         single_schedule.interval_item.interval)
+        self.assertEqual(("Monday", "Friday"), single_schedule.interval_item.interval)  # type: ignore[union-attr]
+        self.assertEqual(TSC.ScheduleItem.State.Suspended, single_schedule.state)
+
+    # Tests calling update with a schedule item returned from the server
+    def test_update_after_get(self) -> None:
+        with open(GET_XML, "rb") as f:
+            get_response_xml = f.read().decode("utf-8")
+        with open(UPDATE_XML, "rb") as f:
+            update_response_xml = f.read().decode("utf-8")
+
+        # Get a schedule
+        with requests_mock.mock() as m:
+            m.get(self.baseurl, text=get_response_xml)
+            all_schedules, pagination_item = self.server.schedules.get()
+        schedule_item = all_schedules[0]
+        self.assertEqual(TSC.ScheduleItem.State.Active, schedule_item.state)
+        self.assertEqual("Weekday early mornings", schedule_item.name)
+
+        # Update the schedule
+        with requests_mock.mock() as m:
+            m.put(self.baseurl + "/c9cff7f9-309c-4361-99ff-d4ba8c9f5467", text=update_response_xml)
+            schedule_item.state = TSC.ScheduleItem.State.Suspended
+            schedule_item.name = "newName"
+            schedule_item = self.server.schedules.update(schedule_item)
 
-    def test_add_workbook(self):
+        self.assertEqual(TSC.ScheduleItem.State.Suspended, schedule_item.state)
+        self.assertEqual("weekly-schedule-1", schedule_item.name)
+
+    def test_add_workbook(self) -> None:
         self.server.version = "2.8"
         baseurl = "{}/sites/{}/schedules".format(self.server.baseurl, self.server.site_id)
 
         with open(WORKBOOK_GET_BY_ID_XML, "rb") as f:
             workbook_response = f.read().decode("utf-8")
+        with open(ADD_WORKBOOK_TO_SCHEDULE, "rb") as f:
+            add_workbook_response = f.read().decode("utf-8")
         with requests_mock.mock() as m:
-            #  TODO: Replace with real response
-            m.get(self.server.workbooks.baseurl + '/bar', text=workbook_response)
-            m.put(baseurl + '/foo/workbooks', text="OK")
+            m.get(self.server.workbooks.baseurl + "/bar", text=workbook_response)
+            m.put(baseurl + "/foo/workbooks", text=add_workbook_response)
             workbook = self.server.workbooks.get_by_id("bar")
-            result = self.server.schedules.add_to_schedule('foo', workbook=workbook)
+            result = self.server.schedules.add_to_schedule("foo", workbook=workbook)
         self.assertEqual(0, len(result), "Added properly")
 
-    def test_add_datasource(self):
+    def test_add_workbook_with_warnings(self) -> None:
+        self.server.version = "2.8"
+        baseurl = "{}/sites/{}/schedules".format(self.server.baseurl, self.server.site_id)
+
+        with open(WORKBOOK_GET_BY_ID_XML, "rb") as f:
+            workbook_response = f.read().decode("utf-8")
+        with open(ADD_WORKBOOK_TO_SCHEDULE_WITH_WARNINGS, "rb") as f:
+            add_workbook_response = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            m.get(self.server.workbooks.baseurl + "/bar", text=workbook_response)
+            m.put(baseurl + "/foo/workbooks", text=add_workbook_response)
+            workbook = self.server.workbooks.get_by_id("bar")
+            result = self.server.schedules.add_to_schedule("foo", workbook=workbook)
+        self.assertEqual(1, len(result), "Not added properly")
+        self.assertEqual(2, len(result[0].warnings))
+
+    def test_add_datasource(self) -> None:
         self.server.version = "2.8"
         baseurl = "{}/sites/{}/schedules".format(self.server.baseurl, self.server.site_id)
 
         with open(DATASOURCE_GET_BY_ID_XML, "rb") as f:
             datasource_response = f.read().decode("utf-8")
+        with open(ADD_DATASOURCE_TO_SCHEDULE, "rb") as f:
+            add_datasource_response = f.read().decode("utf-8")
         with requests_mock.mock() as m:
-            #  TODO: Replace with real response
-            m.get(self.server.datasources.baseurl + '/bar', text=datasource_response)
-            m.put(baseurl + '/foo/datasources', text="OK")
+            m.get(self.server.datasources.baseurl + "/bar", text=datasource_response)
+            m.put(baseurl + "/foo/datasources", text=add_datasource_response)
             datasource = self.server.datasources.get_by_id("bar")
-            result = self.server.schedules.add_to_schedule('foo', datasource=datasource)
+            result = self.server.schedules.add_to_schedule("foo", datasource=datasource)
         self.assertEqual(0, len(result), "Added properly")
```

### Comparing `tableauserverclient-0.9/test/test_requests.py` & `tableauserverclient-0.9.31.post0.dev1/test/test_requests.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,60 @@
+import re
 import unittest
 
 import requests
 import requests_mock
 
 import tableauserverclient as TSC
-
-from tableauserverclient.server.endpoint.exceptions import InternalServerError
+from tableauserverclient.server.endpoint.exceptions import InternalServerError, NonXMLResponseError
 
 
 class RequestTests(unittest.TestCase):
     def setUp(self):
-        self.server = TSC.Server('http://test')
+        self.server = TSC.Server("http://test", False)
 
         # Fake sign in
-        self.server._site_id = 'dad65087-b08b-4603-af4e-2887b8aafc67'
-        self.server._auth_token = 'j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM'
+        self.server._site_id = "dad65087-b08b-4603-af4e-2887b8aafc67"
+        self.server._auth_token = "j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM"
 
         self.baseurl = self.server.workbooks.baseurl
 
     def test_make_get_request(self):
         with requests_mock.mock() as m:
             m.get(requests_mock.ANY)
             url = "http://test/api/2.3/sites/dad65087-b08b-4603-af4e-2887b8aafc67/workbooks"
-            opts = TSC.RequestOptions(pagesize=13, pagenumber=13)
-            resp = self.server.workbooks._make_request(requests.get,
-                                                       url,
-                                                       content=None,
-                                                       request_object=opts,
-                                                       auth_token='j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM',
-                                                       content_type='text/xml')
-
-            self.assertEqual(resp.request.query, 'pagenumber=13&pagesize=13')
-            self.assertEqual(resp.request.headers['x-tableau-auth'], 'j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM')
-            self.assertEqual(resp.request.headers['content-type'], 'text/xml')
+            opts = TSC.RequestOptions(pagesize=13, pagenumber=15)
+            resp = self.server.workbooks.get_request(url, request_object=opts)
+
+            self.assertTrue(re.search("pagesize=13", resp.request.query))
+            self.assertTrue(re.search("pagenumber=15", resp.request.query))
 
     def test_make_post_request(self):
         with requests_mock.mock() as m:
             m.post(requests_mock.ANY)
             url = "http://test/api/2.3/sites/dad65087-b08b-4603-af4e-2887b8aafc67/workbooks"
-            resp = self.server.workbooks._make_request(requests.post,
-                                                       url,
-                                                       content=b'1337',
-                                                       request_object=None,
-                                                       auth_token='j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM',
-                                                       content_type='multipart/mixed')
-            self.assertEqual(resp.request.headers['x-tableau-auth'], 'j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM')
-            self.assertEqual(resp.request.headers['content-type'], 'multipart/mixed')
-            self.assertEqual(resp.request.body, b'1337')
+            resp = self.server.workbooks._make_request(
+                requests.post,
+                url,
+                content=b"1337",
+                auth_token="j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM",
+                content_type="multipart/mixed",
+            )
+            self.assertEqual(resp.request.headers["x-tableau-auth"], "j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM")
+            self.assertEqual(resp.request.headers["content-type"], "multipart/mixed")
+            self.assertEqual(resp.request.body, b"1337")
 
     # Test that 500 server errors are handled properly
     def test_internal_server_error(self):
         self.server.version = "3.2"
         server_response = "500: Internal Server Error"
         with requests_mock.mock() as m:
-            m.register_uri('GET', self.server.server_info.baseurl, status_code=500, text=server_response)
-            self.assertRaisesRegexp(InternalServerError, server_response, self.server.server_info.get)
+            m.register_uri("GET", self.server.server_info.baseurl, status_code=500, text=server_response)
+            self.assertRaisesRegex(InternalServerError, server_response, self.server.server_info.get)
+
+    # Test that non-xml server errors are handled properly
+    def test_non_xml_error(self):
+        self.server.version = "3.2"
+        server_response = "this is not xml"
+        with requests_mock.mock() as m:
+            m.register_uri("GET", self.server.server_info.baseurl, status_code=499, text=server_response)
+            self.assertRaisesRegex(NonXMLResponseError, server_response, self.server.server_info.get)
```

### Comparing `tableauserverclient-0.9/test/test_site.py` & `tableauserverclient-0.9.31.post0.dev1/test/test_site.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,142 +1,231 @@
-import unittest
 import os.path
+import unittest
+
 import requests_mock
+
 import tableauserverclient as TSC
 
-TEST_ASSET_DIR = os.path.join(os.path.dirname(__file__), 'assets')
+TEST_ASSET_DIR = os.path.join(os.path.dirname(__file__), "assets")
 
-GET_XML = os.path.join(TEST_ASSET_DIR, 'site_get.xml')
-GET_BY_ID_XML = os.path.join(TEST_ASSET_DIR, 'site_get_by_id.xml')
-GET_BY_NAME_XML = os.path.join(TEST_ASSET_DIR, 'site_get_by_name.xml')
-UPDATE_XML = os.path.join(TEST_ASSET_DIR, 'site_update.xml')
-CREATE_XML = os.path.join(TEST_ASSET_DIR, 'site_create.xml')
+GET_XML = os.path.join(TEST_ASSET_DIR, "site_get.xml")
+GET_BY_ID_XML = os.path.join(TEST_ASSET_DIR, "site_get_by_id.xml")
+GET_BY_NAME_XML = os.path.join(TEST_ASSET_DIR, "site_get_by_name.xml")
+UPDATE_XML = os.path.join(TEST_ASSET_DIR, "site_update.xml")
+CREATE_XML = os.path.join(TEST_ASSET_DIR, "site_create.xml")
 
 
 class SiteTests(unittest.TestCase):
-    def setUp(self):
-        self.server = TSC.Server('http://test')
+    def setUp(self) -> None:
+        self.server = TSC.Server("http://test", False)
+        self.server.version = "3.10"
 
         # Fake signin
-        self.server._auth_token = 'j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM'
-        self.server._site_id = '0626857c-1def-4503-a7d8-7907c3ff9d9f'
+        self.server._auth_token = "j80k54ll2lfMZ0tv97mlPvvSCRyD0DOM"
+        self.server._site_id = "0626857c-1def-4503-a7d8-7907c3ff9d9f"
         self.baseurl = self.server.sites.baseurl
 
-    def test_get(self):
-        with open(GET_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
+    def test_get(self) -> None:
+        with open(GET_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             m.get(self.baseurl, text=response_xml)
             all_sites, pagination_item = self.server.sites.get()
 
         self.assertEqual(2, pagination_item.total_available)
-        self.assertEqual('dad65087-b08b-4603-af4e-2887b8aafc67', all_sites[0].id)
-        self.assertEqual('Active', all_sites[0].state)
-        self.assertEqual('Default', all_sites[0].name)
-        self.assertEqual('ContentOnly', all_sites[0].admin_mode)
+        self.assertEqual("dad65087-b08b-4603-af4e-2887b8aafc67", all_sites[0].id)
+        self.assertEqual("Active", all_sites[0].state)
+        self.assertEqual("Default", all_sites[0].name)
+        self.assertEqual("ContentOnly", all_sites[0].admin_mode)
         self.assertEqual(False, all_sites[0].revision_history_enabled)
         self.assertEqual(True, all_sites[0].subscribe_others_enabled)
-
-        self.assertEqual('6b7179ba-b82b-4f0f-91ed-812074ac5da6', all_sites[1].id)
-        self.assertEqual('Active', all_sites[1].state)
-        self.assertEqual('Samples', all_sites[1].name)
-        self.assertEqual('ContentOnly', all_sites[1].admin_mode)
+        self.assertEqual(25, all_sites[0].revision_limit)
+        self.assertEqual(None, all_sites[0].num_users)
+        self.assertEqual(None, all_sites[0].storage)
+        self.assertEqual(True, all_sites[0].cataloging_enabled)
+        self.assertEqual(False, all_sites[0].editing_flows_enabled)
+        self.assertEqual(False, all_sites[0].scheduling_flows_enabled)
+        self.assertEqual(True, all_sites[0].allow_subscription_attachments)
+        self.assertEqual("6b7179ba-b82b-4f0f-91ed-812074ac5da6", all_sites[1].id)
+        self.assertEqual("Active", all_sites[1].state)
+        self.assertEqual("Samples", all_sites[1].name)
+        self.assertEqual("ContentOnly", all_sites[1].admin_mode)
         self.assertEqual(False, all_sites[1].revision_history_enabled)
         self.assertEqual(True, all_sites[1].subscribe_others_enabled)
+        self.assertEqual(False, all_sites[1].guest_access_enabled)
+        self.assertEqual(True, all_sites[1].cache_warmup_enabled)
+        self.assertEqual(True, all_sites[1].commenting_enabled)
+        self.assertEqual(True, all_sites[1].cache_warmup_enabled)
+        self.assertEqual(False, all_sites[1].request_access_enabled)
+        self.assertEqual(True, all_sites[1].run_now_enabled)
+        self.assertEqual(1, all_sites[1].tier_explorer_capacity)
+        self.assertEqual(2, all_sites[1].tier_creator_capacity)
+        self.assertEqual(1, all_sites[1].tier_viewer_capacity)
+        self.assertEqual(False, all_sites[1].flows_enabled)
+        self.assertEqual(None, all_sites[1].data_acceleration_mode)
 
-    def test_get_before_signin(self):
+    def test_get_before_signin(self) -> None:
         self.server._auth_token = None
         self.assertRaises(TSC.NotSignedInError, self.server.sites.get)
 
-    def test_get_by_id(self):
-        with open(GET_BY_ID_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
-        with requests_mock.mock() as m:
-            m.get(self.baseurl + '/dad65087-b08b-4603-af4e-2887b8aafc67', text=response_xml)
-            single_site = self.server.sites.get_by_id('dad65087-b08b-4603-af4e-2887b8aafc67')
-
-        self.assertEqual('dad65087-b08b-4603-af4e-2887b8aafc67', single_site.id)
-        self.assertEqual('Active', single_site.state)
-        self.assertEqual('Default', single_site.name)
-        self.assertEqual('ContentOnly', single_site.admin_mode)
+    def test_get_by_id(self) -> None:
+        with open(GET_BY_ID_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            m.get(self.baseurl + "/dad65087-b08b-4603-af4e-2887b8aafc67", text=response_xml)
+            single_site = self.server.sites.get_by_id("dad65087-b08b-4603-af4e-2887b8aafc67")
+
+        self.assertEqual("dad65087-b08b-4603-af4e-2887b8aafc67", single_site.id)
+        self.assertEqual("Active", single_site.state)
+        self.assertEqual("Default", single_site.name)
+        self.assertEqual("ContentOnly", single_site.admin_mode)
         self.assertEqual(False, single_site.revision_history_enabled)
         self.assertEqual(True, single_site.subscribe_others_enabled)
         self.assertEqual(False, single_site.disable_subscriptions)
-
-    def test_get_by_id_missing_id(self):
-        self.assertRaises(ValueError, self.server.sites.get_by_id, '')
-
-    def test_get_by_name(self):
-        with open(GET_BY_NAME_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
-        with requests_mock.mock() as m:
-            m.get(self.baseurl + '/testsite?key=name', text=response_xml)
-            single_site = self.server.sites.get_by_name('testsite')
-
-        self.assertEqual('dad65087-b08b-4603-af4e-2887b8aafc67', single_site.id)
-        self.assertEqual('Active', single_site.state)
-        self.assertEqual('testsite', single_site.name)
-        self.assertEqual('ContentOnly', single_site.admin_mode)
+        self.assertEqual(False, single_site.data_alerts_enabled)
+        self.assertEqual(False, single_site.commenting_mentions_enabled)
+        self.assertEqual(True, single_site.catalog_obfuscation_enabled)
+
+    def test_get_by_id_missing_id(self) -> None:
+        self.assertRaises(ValueError, self.server.sites.get_by_id, "")
+
+    def test_get_by_name(self) -> None:
+        with open(GET_BY_NAME_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            m.get(self.baseurl + "/testsite?key=name", text=response_xml)
+            single_site = self.server.sites.get_by_name("testsite")
+
+        self.assertEqual("dad65087-b08b-4603-af4e-2887b8aafc67", single_site.id)
+        self.assertEqual("Active", single_site.state)
+        self.assertEqual("testsite", single_site.name)
+        self.assertEqual("ContentOnly", single_site.admin_mode)
         self.assertEqual(False, single_site.revision_history_enabled)
         self.assertEqual(True, single_site.subscribe_others_enabled)
         self.assertEqual(False, single_site.disable_subscriptions)
 
-    def test_get_by_name_missing_name(self):
-        self.assertRaises(ValueError, self.server.sites.get_by_name, '')
+    def test_get_by_name_missing_name(self) -> None:
+        self.assertRaises(ValueError, self.server.sites.get_by_name, "")
 
-    def test_update(self):
-        with open(UPDATE_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
-        with requests_mock.mock() as m:
-            m.put(self.baseurl + '/6b7179ba-b82b-4f0f-91ed-812074ac5da6', text=response_xml)
-            single_site = TSC.SiteItem(name='Tableau', content_url='tableau',
-                                       admin_mode=TSC.SiteItem.AdminMode.ContentAndUsers,
-                                       user_quota=15, storage_quota=1000,
-                                       disable_subscriptions=True, revision_history_enabled=False,
-                                       materialized_views_mode='disable')
-            single_site._id = '6b7179ba-b82b-4f0f-91ed-812074ac5da6'
+    def test_update(self) -> None:
+        with open(UPDATE_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
+        with requests_mock.mock() as m:
+            m.put(self.baseurl + "/6b7179ba-b82b-4f0f-91ed-812074ac5da6", text=response_xml)
+            single_site = TSC.SiteItem(
+                name="Tableau",
+                content_url="tableau",
+                admin_mode=TSC.SiteItem.AdminMode.ContentAndUsers,
+                user_quota=15,
+                storage_quota=1000,
+                disable_subscriptions=True,
+                revision_history_enabled=False,
+                data_acceleration_mode="disable",
+                flow_auto_save_enabled=True,
+                web_extraction_enabled=False,
+                metrics_content_type_enabled=True,
+                notify_site_admins_on_throttle=False,
+                authoring_enabled=True,
+                custom_subscription_email_enabled=True,
+                custom_subscription_email="test@test.com",
+                custom_subscription_footer_enabled=True,
+                custom_subscription_footer="example_footer",
+                ask_data_mode="EnabledByDefault",
+                named_sharing_enabled=False,
+                mobile_biometrics_enabled=True,
+                sheet_image_enabled=False,
+                derived_permissions_enabled=True,
+                user_visibility_mode="FULL",
+                use_default_time_zone=False,
+                time_zone="America/Los_Angeles",
+                auto_suspend_refresh_enabled=True,
+                auto_suspend_refresh_inactivity_window=55,
+            )
+            single_site._id = "6b7179ba-b82b-4f0f-91ed-812074ac5da6"
             single_site = self.server.sites.update(single_site)
 
-        self.assertEqual('6b7179ba-b82b-4f0f-91ed-812074ac5da6', single_site.id)
-        self.assertEqual('tableau', single_site.content_url)
-        self.assertEqual('Suspended', single_site.state)
-        self.assertEqual('Tableau', single_site.name)
-        self.assertEqual('ContentAndUsers', single_site.admin_mode)
+        self.assertEqual("6b7179ba-b82b-4f0f-91ed-812074ac5da6", single_site.id)
+        self.assertEqual("tableau", single_site.content_url)
+        self.assertEqual("Suspended", single_site.state)
+        self.assertEqual("Tableau", single_site.name)
+        self.assertEqual("ContentAndUsers", single_site.admin_mode)
         self.assertEqual(True, single_site.revision_history_enabled)
         self.assertEqual(13, single_site.revision_limit)
         self.assertEqual(True, single_site.disable_subscriptions)
         self.assertEqual(15, single_site.user_quota)
-        self.assertEqual('disable', single_site.materialized_views_mode)
+        self.assertEqual("disable", single_site.data_acceleration_mode)
         self.assertEqual(True, single_site.flows_enabled)
         self.assertEqual(True, single_site.cataloging_enabled)
+        self.assertEqual(True, single_site.flow_auto_save_enabled)
+        self.assertEqual(False, single_site.web_extraction_enabled)
+        self.assertEqual(True, single_site.metrics_content_type_enabled)
+        self.assertEqual(False, single_site.notify_site_admins_on_throttle)
+        self.assertEqual(True, single_site.authoring_enabled)
+        self.assertEqual(True, single_site.custom_subscription_email_enabled)
+        self.assertEqual("test@test.com", single_site.custom_subscription_email)
+        self.assertEqual(True, single_site.custom_subscription_footer_enabled)
+        self.assertEqual("example_footer", single_site.custom_subscription_footer)
+        self.assertEqual("EnabledByDefault", single_site.ask_data_mode)
+        self.assertEqual(False, single_site.named_sharing_enabled)
+        self.assertEqual(True, single_site.mobile_biometrics_enabled)
+        self.assertEqual(False, single_site.sheet_image_enabled)
+        self.assertEqual(True, single_site.derived_permissions_enabled)
+        self.assertEqual("FULL", single_site.user_visibility_mode)
+        self.assertEqual(False, single_site.use_default_time_zone)
+        self.assertEqual("America/Los_Angeles", single_site.time_zone)
+        self.assertEqual(True, single_site.auto_suspend_refresh_enabled)
+        self.assertEqual(55, single_site.auto_suspend_refresh_inactivity_window)
 
-    def test_update_missing_id(self):
-        single_site = TSC.SiteItem('test', 'test')
+    def test_update_missing_id(self) -> None:
+        single_site = TSC.SiteItem("test", "test")
         self.assertRaises(TSC.MissingRequiredFieldError, self.server.sites.update, single_site)
 
-    def test_create(self):
-        with open(CREATE_XML, 'rb') as f:
-            response_xml = f.read().decode('utf-8')
+    def test_create(self) -> None:
+        with open(CREATE_XML, "rb") as f:
+            response_xml = f.read().decode("utf-8")
         with requests_mock.mock() as m:
             m.post(self.baseurl, text=response_xml)
-            new_site = TSC.SiteItem(name='Tableau', content_url='tableau',
-                                    admin_mode=TSC.SiteItem.AdminMode.ContentAndUsers, user_quota=15,
-                                    storage_quota=1000, disable_subscriptions=True)
+            new_site = TSC.SiteItem(
+                name="Tableau",
+                content_url="tableau",
+                admin_mode=TSC.SiteItem.AdminMode.ContentAndUsers,
+                user_quota=15,
+                storage_quota=1000,
+                disable_subscriptions=True,
+            )
             new_site = self.server.sites.create(new_site)
 
-        self.assertEqual('0626857c-1def-4503-a7d8-7907c3ff9d9f', new_site.id)
-        self.assertEqual('tableau', new_site.content_url)
-        self.assertEqual('Tableau', new_site.name)
-        self.assertEqual('Active', new_site.state)
-        self.assertEqual('ContentAndUsers', new_site.admin_mode)
+        new_site._tier_viewer_capacity = None
+        new_site._tier_creator_capacity = None
+        new_site._tier_explorer_capacity = None
+        self.assertEqual("0626857c-1def-4503-a7d8-7907c3ff9d9f", new_site.id)
+        self.assertEqual("tableau", new_site.content_url)
+        self.assertEqual("Tableau", new_site.name)
+        self.assertEqual("Active", new_site.state)
+        self.assertEqual("ContentAndUsers", new_site.admin_mode)
         self.assertEqual(False, new_site.revision_history_enabled)
         self.assertEqual(True, new_site.subscribe_others_enabled)
         self.assertEqual(True, new_site.disable_subscriptions)
         self.assertEqual(15, new_site.user_quota)
 
-    def test_delete(self):
+    def test_delete(self) -> None:
         with requests_mock.mock() as m:
-            m.delete(self.baseurl + '/0626857c-1def-4503-a7d8-7907c3ff9d9f', status_code=204)
-            self.server.sites.delete('0626857c-1def-4503-a7d8-7907c3ff9d9f')
+            m.delete(self.baseurl + "/0626857c-1def-4503-a7d8-7907c3ff9d9f", status_code=204)
+            self.server.sites.delete("0626857c-1def-4503-a7d8-7907c3ff9d9f")
 
-    def test_delete_missing_id(self):
-        self.assertRaises(ValueError, self.server.sites.delete, '')
+    def test_delete_missing_id(self) -> None:
+        self.assertRaises(ValueError, self.server.sites.delete, "")
+
+    def test_encrypt(self) -> None:
+        with requests_mock.mock() as m:
+            m.post(self.baseurl + "/0626857c-1def-4503-a7d8-7907c3ff9d9f/encrypt-extracts", status_code=200)
+            self.server.sites.encrypt_extracts("0626857c-1def-4503-a7d8-7907c3ff9d9f")
+
+    def test_recrypt(self) -> None:
+        with requests_mock.mock() as m:
+            m.post(self.baseurl + "/0626857c-1def-4503-a7d8-7907c3ff9d9f/reencrypt-extracts", status_code=200)
+            self.server.sites.re_encrypt_extracts("0626857c-1def-4503-a7d8-7907c3ff9d9f")
+
+    def test_decrypt(self) -> None:
+        with requests_mock.mock() as m:
+            m.post(self.baseurl + "/0626857c-1def-4503-a7d8-7907c3ff9d9f/decrypt-extracts", status_code=200)
+            self.server.sites.decrypt_extracts("0626857c-1def-4503-a7d8-7907c3ff9d9f")
```

### Comparing `tableauserverclient-0.9/test/test_workbook_model.py` & `tableauserverclient-0.9.31.post0.dev1/test/test_workbook_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+
 import tableauserverclient as TSC
 
 
 class WorkbookModelTests(unittest.TestCase):
     def test_invalid_project_id(self):
         self.assertRaises(ValueError, TSC.WorkbookItem, None)
         workbook = TSC.WorkbookItem("10")
```

### Comparing `tableauserverclient-0.9/test/test_user_model.py` & `tableauserverclient-0.9.31.post0.dev1/test/test_user_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+
 import tableauserverclient as TSC
 
 
 class UserModelTests(unittest.TestCase):
     def test_invalid_name(self):
         self.assertRaises(ValueError, TSC.UserItem, None, TSC.UserItem.Roles.Publisher)
         self.assertRaises(ValueError, TSC.UserItem, "", TSC.UserItem.Roles.Publisher)
```

### Comparing `tableauserverclient-0.9/tableauserverclient/datetime_helpers.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/datetime_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import datetime
 
-# This code below is from the python documentation for tzinfo: https://docs.python.org/2.3/lib/datetime-tzinfo.html
+# This code below is from the python documentation for
+# tzinfo: https://docs.python.org/2.3/lib/datetime-tzinfo.html
+
 ZERO = datetime.timedelta(0)
 HOUR = datetime.timedelta(hours=1)
 
 
 class UTC(datetime.tzinfo):
     """UTC"""
 
@@ -22,12 +24,18 @@
 TABLEAU_DATE_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
 
 
 def parse_datetime(date):
     if date is None:
         return None
 
-    return datetime.datetime.strptime(date, TABLEAU_DATE_FORMAT).replace(tzinfo=utc)
+    try:
+        return datetime.datetime.strptime(date, TABLEAU_DATE_FORMAT).replace(tzinfo=utc)
+    except ValueError:
+        return None
 
 
 def format_datetime(date):
+    if date is None:
+        return None
+
     return date.astimezone(tz=utc).strftime(TABLEAU_DATE_FORMAT)
```

### Comparing `tableauserverclient-0.9/tableauserverclient/server/endpoint/flows_endpoint.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/flows_endpoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,215 +1,239 @@
-from .endpoint import Endpoint, api, parameter_added_in
+import cgi
+import copy
+import logging
+import os
+from contextlib import closing
+from typing import Iterable, List, Optional, TYPE_CHECKING, Tuple, Union
+
+from .dqw_endpoint import _DataQualityWarningEndpoint
+from .endpoint import Endpoint, QuerysetEndpoint, api
 from .exceptions import InternalServerError, MissingRequiredFieldError
-from .endpoint import api, parameter_added_in, Endpoint
 from .permissions_endpoint import _PermissionsEndpoint
-from .exceptions import MissingRequiredFieldError
-from .fileuploads_endpoint import Fileuploads
 from .resource_tagger import _ResourceTagger
 from .. import RequestFactory, FlowItem, PaginationItem, ConnectionItem
-from ...filesys_helpers import to_filename
-from ...models.tag_item import TagItem
+from ...filesys_helpers import to_filename, make_download_path
 from ...models.job_item import JobItem
-import os
-import logging
-import copy
-import cgi
-from contextlib import closing
 
 # The maximum size of a file that can be published in a single request is 64MB
-FILESIZE_LIMIT = 1024 * 1024 * 64   # 64MB
+FILESIZE_LIMIT = 1024 * 1024 * 64  # 64MB
+
+ALLOWED_FILE_EXTENSIONS = ["tfl", "tflx"]
 
-ALLOWED_FILE_EXTENSIONS = ['tfl', 'tflx']
+logger = logging.getLogger("tableau.endpoint.flows")
 
-logger = logging.getLogger('tableau.endpoint.flows')
+if TYPE_CHECKING:
+    from .. import DQWItem
+    from ..request_options import RequestOptions
+    from ...models.permissions_item import PermissionsRule
 
 
-class Flows(Endpoint):
+FilePath = Union[str, os.PathLike]
+
+
+class Flows(QuerysetEndpoint):
     def __init__(self, parent_srv):
         super(Flows, self).__init__(parent_srv)
         self._resource_tagger = _ResourceTagger(parent_srv)
         self._permissions = _PermissionsEndpoint(parent_srv, lambda: self.baseurl)
+        self._data_quality_warnings = _DataQualityWarningEndpoint(self.parent_srv, "flow")
 
     @property
-    def baseurl(self):
+    def baseurl(self) -> str:
         return "{0}/sites/{1}/flows".format(self.parent_srv.baseurl, self.parent_srv.site_id)
 
     # Get all flows
     @api(version="3.3")
-    def get(self, req_options=None):
-        logger.info('Querying all flows on site')
+    def get(self, req_options: Optional["RequestOptions"] = None) -> Tuple[List[FlowItem], PaginationItem]:
+        logger.info("Querying all flows on site")
         url = self.baseurl
         server_response = self.get_request(url, req_options)
         pagination_item = PaginationItem.from_response(server_response.content, self.parent_srv.namespace)
         all_flow_items = FlowItem.from_response(server_response.content, self.parent_srv.namespace)
         return all_flow_items, pagination_item
 
     # Get 1 flow by id
     @api(version="3.3")
-    def get_by_id(self, flow_id):
+    def get_by_id(self, flow_id: str) -> FlowItem:
         if not flow_id:
             error = "Flow ID undefined."
             raise ValueError(error)
-        logger.info('Querying single flow (ID: {0})'.format(flow_id))
+        logger.info("Querying single flow (ID: {0})".format(flow_id))
         url = "{0}/{1}".format(self.baseurl, flow_id)
         server_response = self.get_request(url)
         return FlowItem.from_response(server_response.content, self.parent_srv.namespace)[0]
 
     # Populate flow item's connections
     @api(version="3.3")
-    def populate_connections(self, flow_item):
+    def populate_connections(self, flow_item: FlowItem) -> None:
         if not flow_item.id:
-            error = 'Flow item missing ID. Flow must be retrieved from server first.'
+            error = "Flow item missing ID. Flow must be retrieved from server first."
             raise MissingRequiredFieldError(error)
 
         def connections_fetcher():
             return self._get_flow_connections(flow_item)
 
         flow_item._set_connections(connections_fetcher)
-        logger.info('Populated connections for flow (ID: {0})'.format(flow_item.id))
+        logger.info("Populated connections for flow (ID: {0})".format(flow_item.id))
 
-    def _get_flow_connections(self, flow_item, req_options=None):
-        url = '{0}/{1}/connections'.format(self.baseurl, flow_item.id)
+    def _get_flow_connections(self, flow_item, req_options: Optional["RequestOptions"] = None) -> List[ConnectionItem]:
+        url = "{0}/{1}/connections".format(self.baseurl, flow_item.id)
         server_response = self.get_request(url, req_options)
         connections = ConnectionItem.from_response(server_response.content, self.parent_srv.namespace)
         return connections
 
     # Delete 1 flow by id
     @api(version="3.3")
-    def delete(self, flow_id):
+    def delete(self, flow_id: str) -> None:
         if not flow_id:
             error = "Flow ID undefined."
             raise ValueError(error)
         url = "{0}/{1}".format(self.baseurl, flow_id)
         self.delete_request(url)
-        logger.info('Deleted single flow (ID: {0})'.format(flow_id))
+        logger.info("Deleted single flow (ID: {0})".format(flow_id))
 
     # Download 1 flow by id
     @api(version="3.3")
-    def download(self, flow_id, filepath=None):
+    def download(self, flow_id: str, filepath: FilePath = None) -> str:
         if not flow_id:
             error = "Flow ID undefined."
             raise ValueError(error)
         url = "{0}/{1}/content".format(self.baseurl, flow_id)
 
-        with closing(self.get_request(url, parameters={'stream': True})) as server_response:
-            _, params = cgi.parse_header(server_response.headers['Content-Disposition'])
-            filename = to_filename(os.path.basename(params['filename']))
-            if filepath is None:
-                filepath = filename
-            elif os.path.isdir(filepath):
-                filepath = os.path.join(filepath, filename)
+        with closing(self.get_request(url, parameters={"stream": True})) as server_response:
+            _, params = cgi.parse_header(server_response.headers["Content-Disposition"])
+            filename = to_filename(os.path.basename(params["filename"]))
+
+            download_path = make_download_path(filepath, filename)
 
-            with open(filepath, 'wb') as f:
+            with open(download_path, "wb") as f:
                 for chunk in server_response.iter_content(1024):  # 1KB
                     f.write(chunk)
 
-        logger.info('Downloaded flow to {0} (ID: {1})'.format(filepath, flow_id))
-        return os.path.abspath(filepath)
+        logger.info("Downloaded flow to {0} (ID: {1})".format(download_path, flow_id))
+        return os.path.abspath(download_path)
 
     # Update flow
     @api(version="3.3")
-    def update(self, flow_item):
+    def update(self, flow_item: FlowItem) -> FlowItem:
         if not flow_item.id:
-            error = 'Flow item missing ID. Flow must be retrieved from server first.'
+            error = "Flow item missing ID. Flow must be retrieved from server first."
             raise MissingRequiredFieldError(error)
 
         self._resource_tagger.update_tags(self.baseurl, flow_item)
 
         # Update the flow itself
         url = "{0}/{1}".format(self.baseurl, flow_item.id)
         update_req = RequestFactory.Flow.update_req(flow_item)
         server_response = self.put_request(url, update_req)
-        logger.info('Updated flow item (ID: {0})'.format(flow_item.id))
+        logger.info("Updated flow item (ID: {0})".format(flow_item.id))
         updated_flow = copy.copy(flow_item)
         return updated_flow._parse_common_elements(server_response.content, self.parent_srv.namespace)
 
     # Update flow connections
     @api(version="3.3")
-    def update_connection(self, flow_item, connection_item):
+    def update_connection(self, flow_item: FlowItem, connection_item: ConnectionItem) -> ConnectionItem:
         url = "{0}/{1}/connections/{2}".format(self.baseurl, flow_item.id, connection_item.id)
 
         update_req = RequestFactory.Connection.update_req(connection_item)
         server_response = self.put_request(url, update_req)
         connection = ConnectionItem.from_response(server_response.content, self.parent_srv.namespace)[0]
 
-        logger.info('Updated flow item (ID: {0} & connection item {1}'.format(flow_item.id,
-                                                                              connection_item.id))
+        logger.info("Updated flow item (ID: {0} & connection item {1}".format(flow_item.id, connection_item.id))
         return connection
 
     @api(version="3.3")
-    def refresh(self, flow_item):
+    def refresh(self, flow_item: FlowItem) -> JobItem:
         url = "{0}/{1}/run".format(self.baseurl, flow_item.id)
         empty_req = RequestFactory.Empty.empty_req()
         server_response = self.post_request(url, empty_req)
         new_job = JobItem.from_response(server_response.content, self.parent_srv.namespace)[0]
         return new_job
 
     # Publish flow
     @api(version="3.3")
-    def publish(self, flow_item, file_path, mode, connections=None):
+    def publish(
+        self, flow_item: FlowItem, file_path: FilePath, mode: str, connections: Optional[List[ConnectionItem]] = None
+    ) -> FlowItem:
         if not os.path.isfile(file_path):
             error = "File path does not lead to an existing file."
             raise IOError(error)
         if not mode or not hasattr(self.parent_srv.PublishMode, mode):
-            error = 'Invalid mode defined.'
+            error = "Invalid mode defined."
             raise ValueError(error)
 
         filename = os.path.basename(file_path)
         file_extension = os.path.splitext(filename)[1][1:]
 
         # If name is not defined, grab the name from the file to publish
         if not flow_item.name:
             flow_item.name = os.path.splitext(filename)[0]
         if file_extension not in ALLOWED_FILE_EXTENSIONS:
-            error = "Only {} files can be published as flows.".format(', '.join(ALLOWED_FILE_EXTENSIONS))
+            error = "Only {} files can be published as flows.".format(", ".join(ALLOWED_FILE_EXTENSIONS))
             raise ValueError(error)
 
         # Construct the url with the defined mode
         url = "{0}?flowType={1}".format(self.baseurl, file_extension)
         if mode == self.parent_srv.PublishMode.Overwrite or mode == self.parent_srv.PublishMode.Append:
-            url += '&{0}=true'.format(mode.lower())
+            url += "&{0}=true".format(mode.lower())
 
         # Determine if chunking is required (64MB is the limit for single upload method)
         if os.path.getsize(file_path) >= FILESIZE_LIMIT:
-            logger.info('Publishing {0} to server with chunking method (flow over 64MB)'.format(filename))
-            upload_session_id = Fileuploads.upload_chunks(self.parent_srv, file_path)
+            logger.info("Publishing {0} to server with chunking method (flow over 64MB)".format(filename))
+            upload_session_id = self.parent_srv.fileuploads.upload(file_path)
             url = "{0}&uploadSessionId={1}".format(url, upload_session_id)
-            xml_request, content_type = RequestFactory.Flow.publish_req_chunked(flow_item,
-                                                                                connections)
+            xml_request, content_type = RequestFactory.Flow.publish_req_chunked(flow_item, connections)
         else:
-            logger.info('Publishing {0} to server'.format(filename))
-            with open(file_path, 'rb') as f:
+            logger.info("Publishing {0} to server".format(filename))
+            with open(file_path, "rb") as f:
                 file_contents = f.read()
-            xml_request, content_type = RequestFactory.Flow.publish_req(flow_item,
-                                                                        filename,
-                                                                        file_contents,
-                                                                        connections)
+            xml_request, content_type = RequestFactory.Flow.publish_req(flow_item, filename, file_contents, connections)
 
         # Send the publishing request to server
         try:
             server_response = self.post_request(url, xml_request, content_type)
         except InternalServerError as err:
             if err.code == 504:
                 err.content = "Timeout error while publishing. Please use asynchronous publishing to avoid timeouts."
             raise err
         else:
             new_flow = FlowItem.from_response(server_response.content, self.parent_srv.namespace)[0]
-            logger.info('Published {0} (ID: {1})'.format(filename, new_flow.id))
+            logger.info("Published {0} (ID: {1})".format(filename, new_flow.id))
             return new_flow
 
-        server_response = self.post_request(url, xml_request, content_type)
-        new_flow = FlowItem.from_response(server_response.content, self.parent_srv.namespace)[0]
-        logger.info('Published {0} (ID: {1})'.format(filename, new_flow.id))
-        return new_flow
-
-    @api(version='3.3')
-    def populate_permissions(self, item):
+    @api(version="3.3")
+    def populate_permissions(self, item: FlowItem) -> None:
         self._permissions.populate(item)
 
-    @api(version='3.3')
+    @api(version="3.3")
     def update_permission(self, item, permission_item):
+        import warnings
+
+        warnings.warn(
+            "Server.flows.update_permission is deprecated, " "please use Server.flows.update_permissions instead.",
+            DeprecationWarning,
+        )
+        self._permissions.update(item, permission_item)
+
+    @api(version="3.3")
+    def update_permissions(self, item: FlowItem, permission_item: Iterable["PermissionsRule"]) -> None:
         self._permissions.update(item, permission_item)
 
-    @api(version='3.3')
-    def delete_permission(self, item, capability_item):
+    @api(version="3.3")
+    def delete_permission(self, item: FlowItem, capability_item: "PermissionsRule") -> None:
         self._permissions.delete(item, capability_item)
+
+    @api(version="3.5")
+    def populate_dqw(self, item: FlowItem) -> None:
+        self._data_quality_warnings.populate(item)
+
+    @api(version="3.5")
+    def update_dqw(self, item: FlowItem, warning: "DQWItem") -> None:
+        return self._data_quality_warnings.update(item, warning)
+
+    @api(version="3.5")
+    def add_dqw(self, item: FlowItem, warning: "DQWItem") -> None:
+        return self._data_quality_warnings.add(item, warning)
+
+    @api(version="3.5")
+    def delete_dqw(self, item: FlowItem) -> None:
+        self._data_quality_warnings.clear(item)
```

### Comparing `tableauserverclient-0.9/tableauserverclient/server/endpoint/jobs_endpoint.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/fileuploads_endpoint.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,62 @@
-from .endpoint import Endpoint, api
-from .. import JobItem, BackgroundJobItem, PaginationItem
-from ..request_options import RequestOptionsBase
 import logging
 
-try:
-    basestring
-except NameError:
-    # In case we are in python 3 the string check is different
-    basestring = str
+from .endpoint import Endpoint, api
+from .. import RequestFactory
+from ...models.fileupload_item import FileuploadItem
+
+# For when a datasource is over 64MB, break it into 5MB(standard chunk size) chunks
+CHUNK_SIZE = 1024 * 1024 * 5  # 5MB
+
+logger = logging.getLogger("tableau.endpoint.fileuploads")
 
-logger = logging.getLogger('tableau.endpoint.jobs')
 
+class Fileuploads(Endpoint):
+    def __init__(self, parent_srv):
+        super(Fileuploads, self).__init__(parent_srv)
 
-class Jobs(Endpoint):
     @property
     def baseurl(self):
-        return "{0}/sites/{1}/jobs".format(self.parent_srv.baseurl, self.parent_srv.site_id)
+        return "{0}/sites/{1}/fileUploads".format(self.parent_srv.baseurl, self.parent_srv.site_id)
 
-    @api(version='2.6')
-    def get(self, job_id=None, req_options=None):
-        # Backwards Compatibility fix until we rev the major version
-        if job_id is not None and isinstance(job_id, basestring):
-            import warnings
-            warnings.warn("Jobs.get(job_id) is deprecated, update code to use Jobs.get_by_id(job_id)")
-            return self.get_by_id(job_id)
-        if isinstance(job_id, RequestOptionsBase):
-            req_options = job_id
-
-        self.parent_srv.assert_at_least_version('3.1')
-        server_response = self.get_request(self.baseurl, req_options)
-        pagination_item = PaginationItem.from_response(server_response.content, self.parent_srv.namespace)
-        jobs = BackgroundJobItem.from_response(server_response.content, self.parent_srv.namespace)
-        return jobs, pagination_item
-
-    @api(version='3.1')
-    def cancel(self, job_id):
-        url = '{0}/{1}'.format(self.baseurl, job_id)
-        return self.put_request(url)
-
-    @api(version='2.6')
-    def get_by_id(self, job_id):
-        logger.info('Query for information about job ' + job_id)
-        url = "{0}/{1}".format(self.baseurl, job_id)
-        server_response = self.get_request(url)
-        new_job = JobItem.from_response(server_response.content, self.parent_srv.namespace)[0]
-        return new_job
+    @api(version="2.0")
+    def initiate(self):
+        url = self.baseurl
+        server_response = self.post_request(url, "")
+        fileupload_item = FileuploadItem.from_response(server_response.content, self.parent_srv.namespace)
+        upload_id = fileupload_item.upload_session_id
+        logger.info("Initiated file upload session (ID: {0})".format(upload_id))
+        return upload_id
+
+    @api(version="2.0")
+    def append(self, upload_id, data, content_type):
+        url = "{0}/{1}".format(self.baseurl, upload_id)
+        server_response = self.put_request(url, data, content_type)
+        logger.info("Uploading a chunk to session (ID: {0})".format(upload_id))
+        return FileuploadItem.from_response(server_response.content, self.parent_srv.namespace)
+
+    def _read_chunks(self, file):
+        file_opened = False
+        try:
+            file_content = open(file, "rb")
+            file_opened = True
+        except TypeError:
+            file_content = file
+
+        try:
+            while True:
+                chunked_content = file_content.read(CHUNK_SIZE)
+                if not chunked_content:
+                    break
+                yield chunked_content
+        finally:
+            if file_opened:
+                file_content.close()
+
+    def upload(self, file):
+        upload_id = self.initiate()
+        for chunk in self._read_chunks(file):
+            request, content_type = RequestFactory.Fileupload.chunk_req(chunk)
+            fileupload_item = self.append(upload_id, request, content_type)
+            logger.info("\tPublished {0}MB".format(fileupload_item.file_size))
+        logger.info("File upload finished (ID: {0})".format(upload_id))
+        return upload_id
```

### Comparing `tableauserverclient-0.9/tableauserverclient/server/endpoint/users_endpoint.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/auth_endpoint.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,82 @@
-from .endpoint import Endpoint, api
-from .exceptions import MissingRequiredFieldError
-from .. import RequestFactory, UserItem, WorkbookItem, PaginationItem
-from ..pager import Pager
 import logging
-import copy
 
-logger = logging.getLogger('tableau.endpoint.users')
+from defusedxml.ElementTree import fromstring
 
+from .endpoint import Endpoint, api
+from .exceptions import ServerResponseError
+from ..request_factory import RequestFactory
 
-class Users(Endpoint):
-    @property
-    def baseurl(self):
-        return "{0}/sites/{1}/users".format(self.parent_srv.baseurl, self.parent_srv.site_id)
+logger = logging.getLogger("tableau.endpoint.auth")
 
-    # Gets all users
-    @api(version="2.0")
-    def get(self, req_options=None):
-        logger.info('Querying all users on site')
-        url = self.baseurl
-        server_response = self.get_request(url, req_options)
-        pagination_item = PaginationItem.from_response(server_response.content, self.parent_srv.namespace)
-        all_user_items = UserItem.from_response(server_response.content, self.parent_srv.namespace)
-        return all_user_items, pagination_item
 
-    # Gets 1 user by id
-    @api(version="2.0")
-    def get_by_id(self, user_id):
-        if not user_id:
-            error = "User ID undefined."
-            raise ValueError(error)
-        logger.info('Querying single user (ID: {0})'.format(user_id))
-        url = "{0}/{1}".format(self.baseurl, user_id)
-        server_response = self.get_request(url)
-        return UserItem.from_response(server_response.content, self.parent_srv.namespace).pop()
+class Auth(Endpoint):
+    class contextmgr(object):
+        def __init__(self, callback):
+            self._callback = callback
 
-    # Update user
-    @api(version="2.0")
-    def update(self, user_item, password=None):
-        if not user_item.id:
-            error = "User item missing ID."
-            raise MissingRequiredFieldError(error)
-
-        url = "{0}/{1}".format(self.baseurl, user_item.id)
-        update_req = RequestFactory.User.update_req(user_item, password)
-        server_response = self.put_request(url, update_req)
-        logger.info('Updated user item (ID: {0})'.format(user_item.id))
-        updated_item = copy.copy(user_item)
-        return updated_item._parse_common_tags(server_response.content, self.parent_srv.namespace)
+        def __enter__(self):
+            return self
 
-    # Delete 1 user by id
-    @api(version="2.0")
-    def remove(self, user_id):
-        if not user_id:
-            error = "User ID undefined."
-            raise ValueError(error)
-        url = "{0}/{1}".format(self.baseurl, user_id)
-        self.delete_request(url)
-        logger.info('Removed single user (ID: {0})'.format(user_id))
+        def __exit__(self, exc_type, exc_val, exc_tb):
+            self._callback()
 
-    # Add new user to site
-    @api(version="2.0")
-    def add(self, user_item):
-        url = self.baseurl
-        add_req = RequestFactory.User.add_req(user_item)
-        server_response = self.post_request(url, add_req)
-        new_user = UserItem.from_response(server_response.content, self.parent_srv.namespace).pop()
-        logger.info('Added new user (ID: {0})'.format(user_item.id))
-        return new_user
+    @property
+    def baseurl(self):
+        return "{0}/auth".format(self.parent_srv.baseurl)
 
-    # Get workbooks for user
     @api(version="2.0")
-    def populate_workbooks(self, user_item, req_options=None):
-        if not user_item.id:
-            error = "User item missing ID."
-            raise MissingRequiredFieldError(error)
-
-        def wb_pager():
-            return Pager(lambda options: self._get_wbs_for_user(user_item, options), req_options)
-
-        user_item._set_workbooks(wb_pager)
-
-    def _get_wbs_for_user(self, user_item, req_options=None):
-        url = "{0}/{1}/workbooks".format(self.baseurl, user_item.id)
-        server_response = self.get_request(url, req_options)
-        logger.info('Populated workbooks for user (ID: {0})'.format(user_item.id))
-        workbook_item = WorkbookItem.from_response(server_response.content, self.parent_srv.namespace)
-        pagination_item = PaginationItem.from_response(server_response.content, self.parent_srv.namespace)
-        return workbook_item, pagination_item
-
-    def populate_favorites(self, user_item):
-        raise NotImplementedError('REST API currently does not support the ability to query favorites')
+    def sign_in(self, auth_req):
+        url = "{0}/{1}".format(self.baseurl, "signin")
+        signin_req = RequestFactory.Auth.signin_req(auth_req)
+        server_response = self.parent_srv.session.post(url, data=signin_req, **self.parent_srv.http_options)
+        self.parent_srv._namespace.detect(server_response.content)
+        self._check_status(server_response)
+        parsed_response = fromstring(server_response.content)
+        site_id = parsed_response.find(".//t:site", namespaces=self.parent_srv.namespace).get("id", None)
+        user_id = parsed_response.find(".//t:user", namespaces=self.parent_srv.namespace).get("id", None)
+        auth_token = parsed_response.find("t:credentials", namespaces=self.parent_srv.namespace).get("token", None)
+        self.parent_srv._set_auth(site_id, user_id, auth_token)
+        logger.info("Signed into {0} as user with id {1}".format(self.parent_srv.server_address, user_id))
+        return Auth.contextmgr(self.sign_out)
+
+    @api(version="3.6")
+    def sign_in_with_personal_access_token(self, auth_req):
+        # We use the same request that username/password login uses.
+        return self.sign_in(auth_req)
+
+    @api(version="2.0")
+    def sign_out(self):
+        url = "{0}/{1}".format(self.baseurl, "signout")
+        # If there are no auth tokens you're already signed out. No-op
+        if not self.parent_srv.is_signed_in():
+            return
+        self.post_request(url, "")
+        self.parent_srv._clear_auth()
+        logger.info("Signed out")
+
+    @api(version="2.6")
+    def switch_site(self, site_item):
+        url = "{0}/{1}".format(self.baseurl, "switchSite")
+        switch_req = RequestFactory.Auth.switch_req(site_item.content_url)
+        try:
+            server_response = self.post_request(url, switch_req)
+        except ServerResponseError as e:
+            if e.code == "403070":
+                return Auth.contextmgr(self.sign_out)
+            else:
+                raise e
+        self.parent_srv._namespace.detect(server_response.content)
+        self._check_status(server_response)
+        parsed_response = fromstring(server_response.content)
+        site_id = parsed_response.find(".//t:site", namespaces=self.parent_srv.namespace).get("id", None)
+        user_id = parsed_response.find(".//t:user", namespaces=self.parent_srv.namespace).get("id", None)
+        auth_token = parsed_response.find("t:credentials", namespaces=self.parent_srv.namespace).get("token", None)
+        self.parent_srv._set_auth(site_id, user_id, auth_token)
+        logger.info("Signed into {0} as user with id {1}".format(self.parent_srv.server_address, user_id))
+        return Auth.contextmgr(self.sign_out)
+
+    @api(version="3.10")
+    def revoke_all_server_admin_tokens(self):
+        url = "{0}/{1}".format(self.baseurl, "revokeAllServerAdminTokens")
+        self.post_request(url, "")
+        logger.info("Revoked all tokens for all server admins")
```

### Comparing `tableauserverclient-0.9/tableauserverclient/server/endpoint/__init__.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 from .auth_endpoint import Auth
-from .datasources_endpoint import Datasources
+from .data_acceleration_report_endpoint import DataAccelerationReport
+from .data_alert_endpoint import DataAlerts
 from .databases_endpoint import Databases
-from .endpoint import Endpoint
+from .datasources_endpoint import Datasources
+from .endpoint import Endpoint, QuerysetEndpoint
+from .exceptions import (
+    ServerResponseError,
+    MissingRequiredFieldError,
+    ServerInfoEndpointNotFoundError,
+)
+from .favorites_endpoint import Favorites
+from .fileuploads_endpoint import Fileuploads
+from .flow_runs_endpoint import FlowRuns
 from .flows_endpoint import Flows
-from .exceptions import ServerResponseError, MissingRequiredFieldError, ServerInfoEndpointNotFoundError
 from .groups_endpoint import Groups
 from .jobs_endpoint import Jobs
 from .metadata_endpoint import Metadata
+from .metrics_endpoint import Metrics
 from .projects_endpoint import Projects
 from .schedules_endpoint import Schedules
 from .server_info_endpoint import ServerInfo
 from .sites_endpoint import Sites
+from .subscriptions_endpoint import Subscriptions
 from .tables_endpoint import Tables
 from .tasks_endpoint import Tasks
 from .users_endpoint import Users
 from .views_endpoint import Views
+from .webhooks_endpoint import Webhooks
 from .workbooks_endpoint import Workbooks
-from .subscriptions_endpoint import Subscriptions
```

### Comparing `tableauserverclient-0.9/tableauserverclient/server/endpoint/sites_endpoint.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/sites_endpoint.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,138 @@
+import copy
+import logging
+
 from .endpoint import Endpoint, api
 from .exceptions import MissingRequiredFieldError
 from .. import RequestFactory, SiteItem, PaginationItem
-import logging
-import copy
 
-logger = logging.getLogger('tableau.endpoint.sites')
+logger = logging.getLogger("tableau.endpoint.sites")
+
+from typing import TYPE_CHECKING, List, Optional, Tuple
+
+if TYPE_CHECKING:
+    from ..request_options import RequestOptions
 
 
 class Sites(Endpoint):
     @property
-    def baseurl(self):
+    def baseurl(self) -> str:
         return "{0}/sites".format(self.parent_srv.baseurl)
 
     # Gets all sites
     @api(version="2.0")
-    def get(self, req_options=None):
-        logger.info('Querying all sites on site')
+    def get(self, req_options: Optional["RequestOptions"] = None) -> Tuple[List[SiteItem], PaginationItem]:
+        logger.info("Querying all sites on site")
         url = self.baseurl
         server_response = self.get_request(url, req_options)
         pagination_item = PaginationItem.from_response(server_response.content, self.parent_srv.namespace)
         all_site_items = SiteItem.from_response(server_response.content, self.parent_srv.namespace)
         return all_site_items, pagination_item
 
     # Gets 1 site by id
     @api(version="2.0")
-    def get_by_id(self, site_id):
+    def get_by_id(self, site_id: str) -> SiteItem:
         if not site_id:
             error = "Site ID undefined."
             raise ValueError(error)
-        logger.info('Querying single site (ID: {0})'.format(site_id))
+        logger.info("Querying single site (ID: {0})".format(site_id))
         url = "{0}/{1}".format(self.baseurl, site_id)
         server_response = self.get_request(url)
         return SiteItem.from_response(server_response.content, self.parent_srv.namespace)[0]
 
     # Gets 1 site by name
     @api(version="2.0")
-    def get_by_name(self, site_name):
+    def get_by_name(self, site_name: str) -> SiteItem:
         if not site_name:
             error = "Site Name undefined."
             raise ValueError(error)
-        logger.info('Querying single site (Name: {0})'.format(site_name))
+        logger.info("Querying single site (Name: {0})".format(site_name))
         url = "{0}/{1}?key=name".format(self.baseurl, site_name)
         server_response = self.get_request(url)
         return SiteItem.from_response(server_response.content, self.parent_srv.namespace)[0]
 
     # Gets 1 site by content url
     @api(version="2.0")
-    def get_by_content_url(self, content_url):
+    def get_by_content_url(self, content_url: str) -> SiteItem:
         if content_url is None:
             error = "Content URL undefined."
             raise ValueError(error)
-        logger.info('Querying single site (Content URL: {0})'.format(content_url))
+        logger.info("Querying single site (Content URL: {0})".format(content_url))
         url = "{0}/{1}?key=contentUrl".format(self.baseurl, content_url)
         server_response = self.get_request(url)
         return SiteItem.from_response(server_response.content, self.parent_srv.namespace)[0]
 
     # Update site
     @api(version="2.0")
-    def update(self, site_item):
+    def update(self, site_item: SiteItem) -> SiteItem:
         if not site_item.id:
             error = "Site item missing ID."
             raise MissingRequiredFieldError(error)
         if site_item.admin_mode:
             if site_item.admin_mode == SiteItem.AdminMode.ContentOnly and site_item.user_quota:
-                error = 'You cannot set admin_mode to ContentOnly and also set a user quota'
+                error = "You cannot set admin_mode to ContentOnly and also set a user quota"
                 raise ValueError(error)
 
         url = "{0}/{1}".format(self.baseurl, site_item.id)
         update_req = RequestFactory.Site.update_req(site_item)
         server_response = self.put_request(url, update_req)
-        logger.info('Updated site item (ID: {0})'.format(site_item.id))
+        logger.info("Updated site item (ID: {0})".format(site_item.id))
         update_site = copy.copy(site_item)
         return update_site._parse_common_tags(server_response.content, self.parent_srv.namespace)
 
     # Delete 1 site object
     @api(version="2.0")
-    def delete(self, site_id):
+    def delete(self, site_id: str) -> None:
         if not site_id:
             error = "Site ID undefined."
             raise ValueError(error)
         url = "{0}/{1}".format(self.baseurl, site_id)
         self.delete_request(url)
         # If we deleted the site we are logged into
         # then we are automatically logged out
         if site_id == self.parent_srv.site_id:
-            logger.info('Deleting current site and clearing auth tokens')
+            logger.info("Deleting current site and clearing auth tokens")
             self.parent_srv._clear_auth()
-        logger.info('Deleted single site (ID: {0}) and signed out'.format(site_id))
+        logger.info("Deleted single site (ID: {0}) and signed out".format(site_id))
 
     # Create new site
     @api(version="2.0")
-    def create(self, site_item):
+    def create(self, site_item: SiteItem) -> SiteItem:
         if site_item.admin_mode:
             if site_item.admin_mode == SiteItem.AdminMode.ContentOnly and site_item.user_quota:
-                error = 'You cannot set admin_mode to ContentOnly and also set a user quota'
+                error = "You cannot set admin_mode to ContentOnly and also set a user quota"
                 raise ValueError(error)
 
         url = self.baseurl
         create_req = RequestFactory.Site.create_req(site_item)
         server_response = self.post_request(url, create_req)
         new_site = SiteItem.from_response(server_response.content, self.parent_srv.namespace)[0]
-        logger.info('Created new site (ID: {0})'.format(new_site.id))
+        logger.info("Created new site (ID: {0})".format(new_site.id))
         return new_site
+
+    @api(version="3.5")
+    def encrypt_extracts(self, site_id: str) -> None:
+        if not site_id:
+            error = "Site ID undefined."
+            raise ValueError(error)
+        url = "{0}/{1}/encrypt-extracts".format(self.baseurl, site_id)
+        empty_req = RequestFactory.Empty.empty_req()
+        self.post_request(url, empty_req)
+
+    @api(version="3.5")
+    def decrypt_extracts(self, site_id: str) -> None:
+        if not site_id:
+            error = "Site ID undefined."
+            raise ValueError(error)
+        url = "{0}/{1}/decrypt-extracts".format(self.baseurl, site_id)
+        empty_req = RequestFactory.Empty.empty_req()
+        self.post_request(url, empty_req)
+
+    @api(version="3.5")
+    def re_encrypt_extracts(self, site_id: str) -> None:
+        if not site_id:
+            error = "Site ID undefined."
+            raise ValueError(error)
+        url = "{0}/{1}/reencrypt-extracts".format(self.baseurl, site_id)
+
+        empty_req = RequestFactory.Empty.empty_req()
+        self.post_request(url, empty_req)
```

### Comparing `tableauserverclient-0.9/tableauserverclient/server/endpoint/subscriptions_endpoint.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/subscriptions_endpoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,69 @@
+import logging
+
 from .endpoint import Endpoint, api
 from .exceptions import MissingRequiredFieldError
 from .. import RequestFactory, SubscriptionItem, PaginationItem
-import logging
 
-logger = logging.getLogger('tableau.endpoint.subscriptions')
+logger = logging.getLogger("tableau.endpoint.subscriptions")
+
+from typing import List, Optional, TYPE_CHECKING, Tuple
+
+if TYPE_CHECKING:
+    from ..request_options import RequestOptions
 
 
 class Subscriptions(Endpoint):
     @property
-    def baseurl(self):
-        return "{0}/sites/{1}/subscriptions".format(self.parent_srv.baseurl,
-                                                    self.parent_srv.site_id)
-
-    @api(version='2.3')
-    def get(self, req_options=None):
-        logger.info('Querying all subscriptions for the site')
+    def baseurl(self) -> str:
+        return "{0}/sites/{1}/subscriptions".format(self.parent_srv.baseurl, self.parent_srv.site_id)
+
+    @api(version="2.3")
+    def get(self, req_options: Optional["RequestOptions"] = None) -> Tuple[List[SubscriptionItem], PaginationItem]:
+        logger.info("Querying all subscriptions for the site")
         url = self.baseurl
         server_response = self.get_request(url, req_options)
 
         pagination_item = PaginationItem.from_response(server_response.content, self.parent_srv.namespace)
         all_subscriptions = SubscriptionItem.from_response(server_response.content, self.parent_srv.namespace)
         return all_subscriptions, pagination_item
 
-    @api(version='2.3')
-    def get_by_id(self, subscription_id):
+    @api(version="2.3")
+    def get_by_id(self, subscription_id: str) -> SubscriptionItem:
         if not subscription_id:
             error = "No Subscription ID provided"
             raise ValueError(error)
         logger.info("Querying a single subscription by id ({})".format(subscription_id))
         url = "{}/{}".format(self.baseurl, subscription_id)
         server_response = self.get_request(url)
         return SubscriptionItem.from_response(server_response.content, self.parent_srv.namespace)[0]
 
-    @api(version='2.3')
-    def create(self, subscription_item):
+    @api(version="2.3")
+    def create(self, subscription_item: SubscriptionItem) -> SubscriptionItem:
         if not subscription_item:
             error = "No Susbcription provided"
             raise ValueError(error)
         logger.info("Creating a subscription ({})".format(subscription_item))
         url = self.baseurl
         create_req = RequestFactory.Subscription.create_req(subscription_item)
         server_response = self.post_request(url, create_req)
         return SubscriptionItem.from_response(server_response.content, self.parent_srv.namespace)[0]
 
-    @api(version='2.3')
-    def delete(self, subscription_id):
+    @api(version="2.3")
+    def delete(self, subscription_id: str) -> None:
         if not subscription_id:
             error = "Subscription ID undefined."
             raise ValueError(error)
         url = "{0}/{1}".format(self.baseurl, subscription_id)
         self.delete_request(url)
-        logger.info('Deleted subscription (ID: {0})'.format(subscription_id))
+        logger.info("Deleted subscription (ID: {0})".format(subscription_id))
+
+    @api(version="2.3")
+    def update(self, subscription_item: SubscriptionItem) -> SubscriptionItem:
+        if not subscription_item.id:
+            error = "Subscription item missing ID. Subscription must be retrieved from server first."
+            raise MissingRequiredFieldError(error)
+        url = "{0}/{1}".format(self.baseurl, subscription_item.id)
+        update_req = RequestFactory.Subscription.update_req(subscription_item)
+        server_response = self.put_request(url, update_req)
+        logger.info("Updated subscription item (ID: {0})".format(subscription_item.id))
+        return SubscriptionItem.from_response(server_response.content, self.parent_srv.namespace)[0]
```

### Comparing `tableauserverclient-0.9/tableauserverclient/server/endpoint/tables_endpoint.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/tables_endpoint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,135 @@
+import logging
+
+from .dqw_endpoint import _DataQualityWarningEndpoint
 from .endpoint import api, Endpoint
 from .exceptions import MissingRequiredFieldError
 from .permissions_endpoint import _PermissionsEndpoint
-from .default_permissions_endpoint import _DefaultPermissionsEndpoint
+from .. import RequestFactory, TableItem, ColumnItem, PaginationItem
 from ..pager import Pager
 
-from .. import RequestFactory, TableItem, ColumnItem, PaginationItem, PermissionsRule, Permission
-
-import logging
-
-logger = logging.getLogger('tableau.endpoint.tables')
+logger = logging.getLogger("tableau.endpoint.tables")
 
 
 class Tables(Endpoint):
     def __init__(self, parent_srv):
         super(Tables, self).__init__(parent_srv)
 
         self._permissions = _PermissionsEndpoint(parent_srv, lambda: self.baseurl)
+        self._data_quality_warnings = _DataQualityWarningEndpoint(self.parent_srv, "table")
 
     @property
     def baseurl(self):
         return "{0}/sites/{1}/tables".format(self.parent_srv.baseurl, self.parent_srv.site_id)
 
     @api(version="3.5")
     def get(self, req_options=None):
-        logger.info('Querying all tables on site')
+        logger.info("Querying all tables on site")
         url = self.baseurl
         server_response = self.get_request(url, req_options)
         pagination_item = PaginationItem.from_response(server_response.content, self.parent_srv.namespace)
         all_table_items = TableItem.from_response(server_response.content, self.parent_srv.namespace)
         return all_table_items, pagination_item
 
     # Get 1 table
     @api(version="3.5")
     def get_by_id(self, table_id):
         if not table_id:
             error = "table ID undefined."
             raise ValueError(error)
-        logger.info('Querying single table (ID: {0})'.format(table_id))
+        logger.info("Querying single table (ID: {0})".format(table_id))
         url = "{0}/{1}".format(self.baseurl, table_id)
         server_response = self.get_request(url)
         return TableItem.from_response(server_response.content, self.parent_srv.namespace)[0]
 
     @api(version="3.5")
     def delete(self, table_id):
         if not table_id:
             error = "Database ID undefined."
             raise ValueError(error)
         url = "{0}/{1}".format(self.baseurl, table_id)
         self.delete_request(url)
-        logger.info('Deleted single table (ID: {0})'.format(table_id))
+        logger.info("Deleted single table (ID: {0})".format(table_id))
 
     @api(version="3.5")
     def update(self, table_item):
         if not table_item.id:
             error = "table item missing ID."
             raise MissingRequiredFieldError(error)
 
         url = "{0}/{1}".format(self.baseurl, table_item.id)
         update_req = RequestFactory.Table.update_req(table_item)
         server_response = self.put_request(url, update_req)
-        logger.info('Updated table item (ID: {0})'.format(table_item.id))
+        logger.info("Updated table item (ID: {0})".format(table_item.id))
         updated_table = TableItem.from_response(server_response.content, self.parent_srv.namespace)[0]
         return updated_table
 
     # Get all columns of the table
     @api(version="3.5")
     def populate_columns(self, table_item, req_options=None):
         if not table_item.id:
             error = "Table item missing ID. table must be retrieved from server first."
             raise MissingRequiredFieldError(error)
 
         def column_fetcher():
-            return Pager(lambda options: self._get_columns_for_table(table_item, options), req_options)
+            return Pager(
+                lambda options: self._get_columns_for_table(table_item, options),
+                req_options,
+            )
 
         table_item._set_columns(column_fetcher)
-        logger.info('Populated columns for table (ID: {0}'.format(table_item.id))
+        logger.info("Populated columns for table (ID: {0}".format(table_item.id))
 
     def _get_columns_for_table(self, table_item, req_options=None):
         url = "{0}/{1}/columns".format(self.baseurl, table_item.id)
         server_response = self.get_request(url, req_options)
-        columns = ColumnItem.from_response(server_response.content,
-                                           self.parent_srv.namespace)
+        columns = ColumnItem.from_response(server_response.content, self.parent_srv.namespace)
         pagination_item = PaginationItem.from_response(server_response.content, self.parent_srv.namespace)
         return columns, pagination_item
 
     @api(version="3.5")
     def update_column(self, table_item, column_item):
         url = "{0}/{1}/columns/{2}".format(self.baseurl, table_item.id, column_item.id)
         update_req = RequestFactory.Column.update_req(column_item)
         server_response = self.put_request(url, update_req)
         column = ColumnItem.from_response(server_response.content, self.parent_srv.namespace)[0]
 
-        logger.info('Updated table item (ID: {0} & column item {1}'.format(table_item.id,
-                                                                           column_item.id))
+        logger.info("Updated table item (ID: {0} & column item {1}".format(table_item.id, column_item.id))
         return column
 
-    @api(version='3.5')
+    @api(version="3.5")
     def populate_permissions(self, item):
         self._permissions.populate(item)
 
-    @api(version='3.5')
+    @api(version="3.5")
     def update_permission(self, item, rules):
+        import warnings
+
+        warnings.warn(
+            "Server.tables.update_permission is deprecated, " "please use Server.tables.update_permissions instead.",
+            DeprecationWarning,
+        )
+        return self._permissions.update(item, rules)
+
+    @api(version="3.5")
+    def update_permissions(self, item, rules):
         return self._permissions.update(item, rules)
 
-    @api(version='3.5')
+    @api(version="3.5")
     def delete_permission(self, item, rules):
         return self._permissions.delete(item, rules)
+
+    @api(version="3.5")
+    def populate_dqw(self, item):
+        self._data_quality_warnings.populate(item)
+
+    @api(version="3.5")
+    def update_dqw(self, item, warning):
+        return self._data_quality_warnings.update(item, warning)
+
+    @api(version="3.5")
+    def add_dqw(self, item, warning):
+        return self._data_quality_warnings.add(item, warning)
+
+    @api(version="3.5")
+    def delete_dqw(self, item):
+        self._data_quality_warnings.clear(item)
```

### Comparing `tableauserverclient-0.9/tableauserverclient/server/endpoint/permissions_endpoint.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/permissions_endpoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,89 @@
 import logging
 
 from .. import RequestFactory, PermissionsRule
 
-from .endpoint import Endpoint, api
+from .endpoint import Endpoint
 from .exceptions import MissingRequiredFieldError
 
+from typing import Callable, TYPE_CHECKING, List, Union
 
 logger = logging.getLogger(__name__)
 
+if TYPE_CHECKING:
+    from ...models import DatasourceItem, ProjectItem, WorkbookItem, ViewItem
+    from ..server import Server
+    from ..request_options import RequestOptions
+
+TableauItem = Union["DatasourceItem", "ProjectItem", "WorkbookItem", "ViewItem"]
+
 
 class _PermissionsEndpoint(Endpoint):
-    ''' Adds permission model to another endpoint
+    """Adds permission model to another endpoint
 
-    Tableau permissions model is identical between objects but they are nested under
+    Tableau permissions model is identical between objects, but they are nested under
     the parent object endpoint (i.e. permissions for workbooks are under
-    /workbooks/:id/permission).  This class is meant to be instantated inside a
+    /workbooks/:id/permission).  This class is meant to be instantiated inside a
     parent endpoint which has these supported endpoints
-    '''
-    def __init__(self, parent_srv, owner_baseurl):
+    """
+
+    def __init__(self, parent_srv: "Server", owner_baseurl: Callable[[], str]) -> None:
         super(_PermissionsEndpoint, self).__init__(parent_srv)
 
         # owner_baseurl is the baseurl of the parent.  The MUST be a lambda
         # since we don't know the full site URL until we sign in.  If
         # populated without, we will get a sign-in error
         self.owner_baseurl = owner_baseurl
 
-    def update(self, resource, permissions):
-        url = '{0}/{1}/permissions'.format(self.owner_baseurl(), resource.id)
+    def update(self, resource: TableauItem, permissions: List[PermissionsRule]) -> List[PermissionsRule]:
+        url = "{0}/{1}/permissions".format(self.owner_baseurl(), resource.id)
         update_req = RequestFactory.Permission.add_req(permissions)
         response = self.put_request(url, update_req)
-        permissions = PermissionsRule.from_response(response.content,
-                                                    self.parent_srv.namespace)
-        logger.info('Updated permissions for resource {0}'.format(resource.id))
+        permissions = PermissionsRule.from_response(response.content, self.parent_srv.namespace)
+        logger.info("Updated permissions for resource {0}".format(resource.id))
 
         return permissions
 
-    def delete(self, resource, rules):
+    def delete(self, resource: TableauItem, rules: Union[PermissionsRule, List[PermissionsRule]]):
         # Delete is the only endpoint that doesn't take a list of rules
         # so let's fake it to keep it consistent
         # TODO that means we need error handling around the call
         if isinstance(rules, PermissionsRule):
             rules = [rules]
 
         for rule in rules:
             for capability, mode in rule.capabilities.items():
-                "              /permissions/groups/group-id/capability-name/capability-mode"
-                url = '{0}/{1}/permissions/{2}/{3}/{4}/{5}'.format(
+                "/permissions/groups/group-id/capability-name/capability-mode"
+                url = "{0}/{1}/permissions/{2}/{3}/{4}/{5}".format(
                     self.owner_baseurl(),
                     resource.id,
-                    rule.grantee.permissions_grantee_type + 's',
+                    rule.grantee.tag_name + "s",
                     rule.grantee.id,
                     capability,
-                    mode)
+                    mode,
+                )
 
-                logger.debug('Removing {0} permission for capabilty {1}'.format(
-                    mode, capability))
+                logger.debug("Removing {0} permission for capabilty {1}".format(mode, capability))
 
                 self.delete_request(url)
 
-            logger.info('Deleted permission for {0} {1} item {2}'.format(
-                rule.grantee.permissions_grantee_type,
-                rule.grantee.id,
-                resource.id))
+            logger.info(
+                "Deleted permission for {0} {1} item {2}".format(rule.grantee.tag_name, rule.grantee.id, resource.id)
+            )
 
-    def populate(self, item):
+    def populate(self, item: TableauItem):
         if not item.id:
             error = "Server item is missing ID. Item must be retrieved from server first."
             raise MissingRequiredFieldError(error)
 
         def permission_fetcher():
             return self._get_permissions(item)
 
         item._set_permissions(permission_fetcher)
-        logger.info('Populated permissions for item (ID: {0})'.format(item.id))
+        logger.info("Populated permissions for item (ID: {0})".format(item.id))
 
-    def _get_permissions(self, item, req_options=None):
+    def _get_permissions(self, item: TableauItem, req_options: "RequestOptions" = None):
         url = "{0}/{1}/permissions".format(self.owner_baseurl(), item.id)
         server_response = self.get_request(url, req_options)
-        permissions = PermissionsRule.from_response(server_response.content,
-                                                    self.parent_srv.namespace)
+        permissions = PermissionsRule.from_response(server_response.content, self.parent_srv.namespace)
 
         return permissions
```

### Comparing `tableauserverclient-0.9/tableauserverclient/server/endpoint/resource_tagger.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/resource_tagger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,51 @@
+import copy
+import logging
+import urllib.parse
+
 from .endpoint import Endpoint
 from .exceptions import EndpointUnavailableError, ServerResponseError
 from .. import RequestFactory
 from ...models.tag_item import TagItem
-import logging
-import copy
 
-logger = logging.getLogger('tableau.endpoint.resource_tagger')
+logger = logging.getLogger("tableau.endpoint.resource_tagger")
 
 
 class _ResourceTagger(Endpoint):
     # Add new tags to resource
     def _add_tags(self, baseurl, resource_id, tag_set):
         url = "{0}/{1}/tags".format(baseurl, resource_id)
         add_req = RequestFactory.Tag.add_req(tag_set)
 
         try:
             server_response = self.put_request(url, add_req)
             return TagItem.from_response(server_response.content, self.parent_srv.namespace)
         except ServerResponseError as e:
-            if e.code == "404003":
+            if e.code == "404008":
                 error = "Adding tags to this resource type is only available with REST API version 2.6 and later."
                 raise EndpointUnavailableError(error)
             raise  # Some other error
 
     # Delete a resource's tag by name
     def _delete_tag(self, baseurl, resource_id, tag_name):
-        url = "{0}/{1}/tags/{2}".format(baseurl, resource_id, tag_name)
+        encoded_tag_name = urllib.parse.quote(tag_name)
+        url = "{0}/{1}/tags/{2}".format(baseurl, resource_id, encoded_tag_name)
 
         try:
             self.delete_request(url)
         except ServerResponseError as e:
-            if e.code == "404003":
+            if e.code == "404008":
                 error = "Deleting tags from this resource type is only available with REST API version 2.6 and later."
                 raise EndpointUnavailableError(error)
+            raise  # Some other error
 
     # Remove and add tags to match the resource item's tag set
     def update_tags(self, baseurl, resource_item):
         if resource_item.tags != resource_item._initial_tags:
             add_set = resource_item.tags - resource_item._initial_tags
             remove_set = resource_item._initial_tags - resource_item.tags
             for tag in remove_set:
                 self._delete_tag(baseurl, resource_item.id, tag)
             if add_set:
                 resource_item.tags = self._add_tags(baseurl, resource_item.id, add_set)
             resource_item._initial_tags = copy.copy(resource_item.tags)
-        logger.info('Updated tags to {0}'.format(resource_item.tags))
+        logger.info("Updated tags to {0}".format(resource_item.tags))
```

### Comparing `tableauserverclient-0.9/tableauserverclient/server/endpoint/groups_endpoint.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/users_endpoint.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,106 +1,133 @@
-from .endpoint import Endpoint, api
-from .exceptions import MissingRequiredFieldError
-from ...models.exceptions import UnpopulatedPropertyError
-from .. import RequestFactory, GroupItem, UserItem, PaginationItem
-from ..pager import Pager
+import copy
 import logging
+from typing import List, Tuple
 
-logger = logging.getLogger('tableau.endpoint.groups')
+from .endpoint import QuerysetEndpoint, api
+from .exceptions import MissingRequiredFieldError
+from .. import (
+    RequestFactory,
+    RequestOptions,
+    UserItem,
+    WorkbookItem,
+    PaginationItem,
+    GroupItem,
+)
+from ..pager import Pager
 
-UNLICENSED_USER = UserItem.Roles.Unlicensed
+logger = logging.getLogger("tableau.endpoint.users")
 
 
-class Groups(Endpoint):
+class Users(QuerysetEndpoint):
     @property
-    def baseurl(self):
-        return "{0}/sites/{1}/groups".format(self.parent_srv.baseurl, self.parent_srv.site_id)
-
-    # Gets all groups
-    @api(version="2.0")
-    def get(self, req_options=None):
-        logger.info('Querying all groups on site')
-        url = self.baseurl
-        server_response = self.get_request(url, req_options)
-        pagination_item = PaginationItem.from_response(server_response.content, self.parent_srv.namespace)
-        all_group_items = GroupItem.from_response(server_response.content, self.parent_srv.namespace)
-        return all_group_items, pagination_item
+    def baseurl(self) -> str:
+        return "{0}/sites/{1}/users".format(self.parent_srv.baseurl, self.parent_srv.site_id)
 
-    # Gets all users in a given group
+    # Gets all users
     @api(version="2.0")
-    def populate_users(self, group_item, req_options=None):
-        if not group_item.id:
-            error = "Group item missing ID. Group must be retrieved from server first."
-            raise MissingRequiredFieldError(error)
+    def get(self, req_options: RequestOptions = None) -> Tuple[List[UserItem], PaginationItem]:
+        logger.info("Querying all users on site")
 
-        # Define an inner function that we bind to the model_item's `.user` property.
+        if req_options is None:
+            req_options = RequestOptions()
+        req_options._all_fields = True
 
-        def user_pager():
-            return Pager(lambda options: self._get_users_for_group(group_item, options), req_options)
-
-        group_item._set_users(user_pager)
-
-    def _get_users_for_group(self, group_item, req_options=None):
-        url = "{0}/{1}/users".format(self.baseurl, group_item.id)
+        url = self.baseurl
         server_response = self.get_request(url, req_options)
-        user_item = UserItem.from_response(server_response.content, self.parent_srv.namespace)
         pagination_item = PaginationItem.from_response(server_response.content, self.parent_srv.namespace)
-        logger.info('Populated users for group (ID: {0})'.format(group_item.id))
-        return user_item, pagination_item
+        all_user_items = UserItem.from_response(server_response.content, self.parent_srv.namespace)
+        return all_user_items, pagination_item
 
-    # Deletes 1 group by id
+    # Gets 1 user by id
     @api(version="2.0")
-    def delete(self, group_id):
-        if not group_id:
-            error = "Group ID undefined."
+    def get_by_id(self, user_id: str) -> UserItem:
+        if not user_id:
+            error = "User ID undefined."
             raise ValueError(error)
-        url = "{0}/{1}".format(self.baseurl, group_id)
-        self.delete_request(url)
-        logger.info('Deleted single group (ID: {0})'.format(group_id))
+        logger.info("Querying single user (ID: {0})".format(user_id))
+        url = "{0}/{1}".format(self.baseurl, user_id)
+        server_response = self.get_request(url)
+        return UserItem.from_response(server_response.content, self.parent_srv.namespace).pop()
 
+    # Update user
     @api(version="2.0")
-    def update(self, group_item, default_site_role=UNLICENSED_USER):
-        if not group_item.id:
-            error = "Group item missing ID."
+    def update(self, user_item: UserItem, password: str = None) -> UserItem:
+        if not user_item.id:
+            error = "User item missing ID."
             raise MissingRequiredFieldError(error)
-        url = "{0}/{1}".format(self.baseurl, group_item.id)
-        update_req = RequestFactory.Group.update_req(group_item, default_site_role)
+
+        url = "{0}/{1}".format(self.baseurl, user_item.id)
+        update_req = RequestFactory.User.update_req(user_item, password)
         server_response = self.put_request(url, update_req)
-        logger.info('Updated group item (ID: {0})'.format(group_item.id))
-        updated_group = GroupItem.from_response(server_response.content, self.parent_srv.namespace)[0]
-        return updated_group
+        logger.info("Updated user item (ID: {0})".format(user_item.id))
+        updated_item = copy.copy(user_item)
+        return updated_item._parse_common_tags(server_response.content, self.parent_srv.namespace)
 
-    # Create a 'local' Tableau group
+    # Delete 1 user by id
     @api(version="2.0")
-    def create(self, group_item):
-        url = self.baseurl
-        create_req = RequestFactory.Group.create_req(group_item)
-        server_response = self.post_request(url, create_req)
-        return GroupItem.from_response(server_response.content, self.parent_srv.namespace)[0]
-
-    # Removes 1 user from 1 group
-    @api(version="2.0")
-    def remove_user(self, group_item, user_id):
-        if not group_item.id:
-            error = "Group item missing ID."
-            raise MissingRequiredFieldError(error)
+    def remove(self, user_id: str) -> None:
         if not user_id:
             error = "User ID undefined."
             raise ValueError(error)
-        url = "{0}/{1}/users/{2}".format(self.baseurl, group_item.id, user_id)
+        url = "{0}/{1}".format(self.baseurl, user_id)
         self.delete_request(url)
-        logger.info('Removed user (id: {0}) from group (ID: {1})'.format(user_id, group_item.id))
+        logger.info("Removed single user (ID: {0})".format(user_id))
 
-    # Adds 1 user to 1 group
+    # Add new user to site
     @api(version="2.0")
-    def add_user(self, group_item, user_id):
-        if not group_item.id:
-            error = "Group item missing ID."
-            raise MissingRequiredFieldError(error)
-        if not user_id:
-            error = "User ID undefined."
-            raise ValueError(error)
-        url = "{0}/{1}/users".format(self.baseurl, group_item.id)
-        add_req = RequestFactory.Group.add_user_req(user_id)
+    def add(self, user_item: UserItem) -> UserItem:
+        url = self.baseurl
+        add_req = RequestFactory.User.add_req(user_item)
         server_response = self.post_request(url, add_req)
-        return UserItem.from_response(server_response.content, self.parent_srv.namespace).pop()
-        logger.info('Added user (id: {0}) to group (ID: {1})'.format(user_id, group_item.id))
+        new_user = UserItem.from_response(server_response.content, self.parent_srv.namespace).pop()
+        logger.info("Added new user (ID: {0})".format(new_user.id))
+        return new_user
+
+    # Get workbooks for user
+    @api(version="2.0")
+    def populate_workbooks(self, user_item: UserItem, req_options: RequestOptions = None) -> None:
+        if not user_item.id:
+            error = "User item missing ID."
+            raise MissingRequiredFieldError(error)
+
+        def wb_pager():
+            return Pager(lambda options: self._get_wbs_for_user(user_item, options), req_options)
+
+        user_item._set_workbooks(wb_pager)
+
+    def _get_wbs_for_user(
+        self, user_item: UserItem, req_options: RequestOptions = None
+    ) -> Tuple[List[WorkbookItem], PaginationItem]:
+        url = "{0}/{1}/workbooks".format(self.baseurl, user_item.id)
+        server_response = self.get_request(url, req_options)
+        logger.info("Populated workbooks for user (ID: {0})".format(user_item.id))
+        workbook_item = WorkbookItem.from_response(server_response.content, self.parent_srv.namespace)
+        pagination_item = PaginationItem.from_response(server_response.content, self.parent_srv.namespace)
+        return workbook_item, pagination_item
+
+    def populate_favorites(self, user_item: UserItem) -> None:
+        self.parent_srv.favorites.get(user_item)
+
+    # Get groups for user
+    @api(version="3.7")
+    def populate_groups(self, user_item: UserItem, req_options: RequestOptions = None) -> None:
+        if not user_item.id:
+            error = "User item missing ID."
+            raise MissingRequiredFieldError(error)
+
+        def groups_for_user_pager():
+            return Pager(
+                lambda options: self._get_groups_for_user(user_item, options),
+                req_options,
+            )
+
+        user_item._set_groups(groups_for_user_pager)
+
+    def _get_groups_for_user(
+        self, user_item: UserItem, req_options: RequestOptions = None
+    ) -> Tuple[List[GroupItem], PaginationItem]:
+        url = "{0}/{1}/groups".format(self.baseurl, user_item.id)
+        server_response = self.get_request(url, req_options)
+        logger.info("Populated groups for user (ID: {0})".format(user_item.id))
+        group_item = GroupItem.from_response(server_response.content, self.parent_srv.namespace)
+        pagination_item = PaginationItem.from_response(server_response.content, self.parent_srv.namespace)
+        return group_item, pagination_item
```

### Comparing `tableauserverclient-0.9/tableauserverclient/server/endpoint/exceptions.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import xml.etree.ElementTree as ET
+from defusedxml.ElementTree import fromstring
 
 
 class ServerResponseError(Exception):
     def __init__(self, code, summary, detail):
         self.code = code
         self.summary = summary
         self.detail = detail
@@ -10,18 +10,20 @@
 
     def __str__(self):
         return "\n\n\t{0}: {1}\n\t\t{2}".format(self.code, self.summary, self.detail)
 
     @classmethod
     def from_response(cls, resp, ns):
         # Check elements exist before .text
-        parsed_response = ET.fromstring(resp)
-        error_response = cls(parsed_response.find('t:error', namespaces=ns).get('code', ''),
-                             parsed_response.find('.//t:summary', namespaces=ns).text,
-                             parsed_response.find('.//t:detail', namespaces=ns).text)
+        parsed_response = fromstring(resp)
+        error_response = cls(
+            parsed_response.find("t:error", namespaces=ns).get("code", ""),
+            parsed_response.find(".//t:summary", namespaces=ns).text,
+            parsed_response.find(".//t:detail", namespaces=ns).text,
+        )
         return error_response
 
 
 class InternalServerError(Exception):
     def __init__(self, server_response):
         self.code = server_response.status_code
         self.content = server_response.content
@@ -46,14 +48,45 @@
     pass
 
 
 class NonXMLResponseError(Exception):
     pass
 
 
+class InvalidGraphQLQuery(Exception):
+    pass
+
+
 class GraphQLError(Exception):
     def __init__(self, error_payload):
         self.error = error_payload
 
     def __str__(self):
         from pprint import pformat
+
         return pformat(self.error)
+
+
+class JobFailedException(Exception):
+    def __init__(self, job):
+        self.notes = job.notes
+        self.job = job
+
+    def __str__(self):
+        return f"Job {self.job.id} failed with notes {self.notes}"
+
+
+class JobCancelledException(JobFailedException):
+    pass
+
+
+class FlowRunFailedException(Exception):
+    def __init__(self, flow_run):
+        self.background_job_id = flow_run.background_job_id
+        self.flow_run = flow_run
+
+    def __str__(self):
+        return f"FlowRun {self.flow_run.id} failed with job id {self.background_job_id}"
+
+
+class FlowRunCancelledException(FlowRunFailedException):
+    pass
```

### Comparing `tableauserverclient-0.9/tableauserverclient/server/endpoint/server_info_endpoint.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/server_info_endpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+import logging
+
 from .endpoint import Endpoint, api
-from .exceptions import ServerResponseError, ServerInfoEndpointNotFoundError, EndpointUnavailableError
+from .exceptions import (
+    ServerResponseError,
+    ServerInfoEndpointNotFoundError,
+    EndpointUnavailableError,
+)
 from ...models import ServerInfoItem
-import logging
 
-logger = logging.getLogger('tableau.endpoint.server_info')
+logger = logging.getLogger("tableau.endpoint.server_info")
 
 
 class ServerInfo(Endpoint):
     @property
     def baseurl(self):
         return "{0}/serverInfo".format(self.parent_srv.baseurl)
 
     @api(version="2.4")
     def get(self):
-        """ Retrieve the server info for the server.  This is an unauthenticated call """
+        """Retrieve the server info for the server.  This is an unauthenticated call"""
         try:
             server_response = self.get_unauthenticated_request(self.baseurl)
         except ServerResponseError as e:
             if e.code == "404003":
                 raise ServerInfoEndpointNotFoundError
             if e.code == "404001":
                 raise EndpointUnavailableError
```

### Comparing `tableauserverclient-0.9/tableauserverclient/server/endpoint/schedules_endpoint.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/endpoint/schedules_endpoint.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,93 +1,134 @@
-from .endpoint import Endpoint, api
-from .exceptions import MissingRequiredFieldError
-from .. import RequestFactory, PaginationItem, ScheduleItem, WorkbookItem, DatasourceItem
-import logging
 import copy
+import logging
 from collections import namedtuple
+from typing import TYPE_CHECKING, Callable, List, Optional, Tuple, Union
 
-logger = logging.getLogger('tableau.endpoint.schedules')
+from .endpoint import Endpoint, api
+from .exceptions import MissingRequiredFieldError
+from .. import RequestFactory, PaginationItem, ScheduleItem, TaskItem
+
+logger = logging.getLogger("tableau.endpoint.schedules")
 # Oh to have a first class Result concept in Python...
-AddResponse = namedtuple('AddResponse', ('result', 'error'))
-OK = AddResponse(result=True, error=None)
+AddResponse = namedtuple("AddResponse", ("result", "error", "warnings", "task_created"))
+OK = AddResponse(result=True, error=None, warnings=None, task_created=None)
+
+if TYPE_CHECKING:
+    from ..request_options import RequestOptions
+    from ...models import DatasourceItem, WorkbookItem
 
 
 class Schedules(Endpoint):
     @property
-    def baseurl(self):
+    def baseurl(self) -> str:
         return "{0}/schedules".format(self.parent_srv.baseurl)
 
     @property
-    def siteurl(self):
+    def siteurl(self) -> str:
         return "{0}/sites/{1}/schedules".format(self.parent_srv.baseurl, self.parent_srv.site_id)
 
     @api(version="2.3")
-    def get(self, req_options=None):
+    def get(self, req_options: Optional["RequestOptions"] = None) -> Tuple[List[ScheduleItem], PaginationItem]:
         logger.info("Querying all schedules")
         url = self.baseurl
         server_response = self.get_request(url, req_options)
         pagination_item = PaginationItem.from_response(server_response.content, self.parent_srv.namespace)
         all_schedule_items = ScheduleItem.from_response(server_response.content, self.parent_srv.namespace)
         return all_schedule_items, pagination_item
 
+    @api(version="3.8")
+    def get_by_id(self, schedule_id):
+        if not schedule_id:
+            error = "No Schedule ID provided"
+            raise ValueError(error)
+        logger.info("Querying a single schedule by id ({})".format(schedule_id))
+        url = "{0}/{1}".format(self.baseurl, schedule_id)
+        server_response = self.get_request(url)
+        return ScheduleItem.from_response(server_response.content, self.parent_srv.namespace)[0]
+
     @api(version="2.3")
-    def delete(self, schedule_id):
+    def delete(self, schedule_id: str) -> None:
         if not schedule_id:
             error = "Schedule ID undefined"
             raise ValueError(error)
         url = "{0}/{1}".format(self.baseurl, schedule_id)
         self.delete_request(url)
         logger.info("Deleted single schedule (ID: {0})".format(schedule_id))
 
     @api(version="2.3")
-    def update(self, schedule_item):
+    def update(self, schedule_item: ScheduleItem) -> ScheduleItem:
         if not schedule_item.id:
             error = "Schedule item missing ID."
             raise MissingRequiredFieldError(error)
-        if schedule_item.interval_item is None:
-            error = "Interval item must be defined."
-            raise MissingRequiredFieldError(error)
 
         url = "{0}/{1}".format(self.baseurl, schedule_item.id)
         update_req = RequestFactory.Schedule.update_req(schedule_item)
         server_response = self.put_request(url, update_req)
         logger.info("Updated schedule item (ID: {})".format(schedule_item.id))
         updated_schedule = copy.copy(schedule_item)
         return updated_schedule._parse_common_tags(server_response.content, self.parent_srv.namespace)
 
     @api(version="2.3")
-    def create(self, schedule_item):
+    def create(self, schedule_item: ScheduleItem) -> ScheduleItem:
         if schedule_item.interval_item is None:
             error = "Interval item must be defined."
             raise MissingRequiredFieldError(error)
 
         url = self.baseurl
         create_req = RequestFactory.Schedule.create_req(schedule_item)
         server_response = self.post_request(url, create_req)
         new_schedule = ScheduleItem.from_response(server_response.content, self.parent_srv.namespace)[0]
         logger.info("Created new schedule (ID: {})".format(new_schedule.id))
         return new_schedule
 
     @api(version="2.8")
-    def add_to_schedule(self, schedule_id, workbook=None, datasource=None):
-
-        def add_to(resource, type_, req_factory):
+    def add_to_schedule(
+        self,
+        schedule_id: str,
+        workbook: "WorkbookItem" = None,
+        datasource: "DatasourceItem" = None,
+        task_type: str = TaskItem.Type.ExtractRefresh,
+    ) -> List[AddResponse]:
+        def add_to(
+            resource: Union["DatasourceItem", "WorkbookItem"],
+            type_: str,
+            req_factory: Callable[
+                [
+                    str,
+                    str,
+                ],
+                bytes,
+            ],
+        ) -> AddResponse:
             id_ = resource.id
             url = "{0}/{1}/{2}s".format(self.siteurl, schedule_id, type_)
-            add_req = req_factory(id_)
+            add_req = req_factory(id_, task_type=task_type)  # type: ignore[call-arg, arg-type]
             response = self.put_request(url, add_req)
-            if response.status_code < 200 or response.status_code >= 300:
-                return AddResponse(result=False,
-                                   error="Status {}: {}".format(response.status_code, response.reason))
-            logger.info("Added {} to {} to schedule {}".format(type_, id_, schedule_id))
-            return OK
+
+            error, warnings, task_created = ScheduleItem.parse_add_to_schedule_response(
+                response, self.parent_srv.namespace
+            )
+            if task_created:
+                logger.info("Added {} to {} to schedule {}".format(type_, id_, schedule_id))
+
+            if error is not None or warnings is not None:
+                return AddResponse(
+                    result=False,
+                    error=error,
+                    warnings=warnings,
+                    task_created=task_created,
+                )
+            else:
+                return OK
 
         items = []
 
         if workbook is not None:
             items.append((workbook, "workbook", RequestFactory.Schedule.add_workbook_req))
         if datasource is not None:
-            items.append((datasource, "datasource", RequestFactory.Schedule.add_datasource_req))
+            items.append(
+                (datasource, "datasource", RequestFactory.Schedule.add_datasource_req)  # type:ignore[arg-type]
+            )
 
         results = (add_to(*x) for x in items)
         # list() is needed for python 3.x compatibility
-        return list(filter(lambda x: not x.result, results))
+        return list(filter(lambda x: not x.result, results))  # type:ignore[arg-type]
```

### Comparing `tableauserverclient-0.9/tableauserverclient/server/pager.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/pager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from functools import partial
 
 from . import RequestOptions
-from . import Sort
 
 
 class Pager(object):
     """
     Generator that takes an endpoint (top level endpoints with `.get)` and lazily loads items from Server.
     Supports all `RequestOptions` including starting on any page. Also used by models to load sub-models
     (users in a group, views in a workbook, etc) by passing a different endpoint.
 
     Will loop over anything that returns (List[ModelItem], PaginationItem).
     """
 
     def __init__(self, endpoint, request_opts=None, **kwargs):
 
-        if hasattr(endpoint, 'get'):
+        if hasattr(endpoint, "get"):
             # The simpliest case is to take an Endpoint and call its get
             endpoint = partial(endpoint.get, **kwargs)
             self._endpoint = endpoint
         elif callable(endpoint):
             # but if they pass a callable then use that instead (used internally)
             endpoint = partial(endpoint, **kwargs)
             self._endpoint = endpoint
@@ -27,15 +26,15 @@
             # Didn't get something we can page over
             raise ValueError("Pager needs a server endpoint to page through.")
 
         self._options = request_opts
 
         # If we have options we could be starting on any page, backfill the count
         if self._options:
-            self._count = ((self._options.pagenumber - 1) * self._options.pagesize)
+            self._count = (self._options.pagenumber - 1) * self._options.pagesize
         else:
             self._count = 0
             self._options = RequestOptions()
 
     def __iter__(self):
         # Fetch the first page
         current_item_list, last_pagination_item = self._endpoint(self._options)
```

### Comparing `tableauserverclient-0.9/tableauserverclient/server/filter.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/server/filter.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,16 +7,16 @@
         self.operator = operator
         self._value = None
         self.value = value
 
     def __str__(self):
         value_string = str(self._value)
         if isinstance(self._value, list):
-            value_string = value_string.replace(' ', '').replace('\'', '')
-        return '{0}:{1}:{2}'.format(self.field, self.operator, value_string)
+            value_string = value_string.replace(" ", "").replace("'", "")
+        return "{0}:{1}:{2}".format(self.field, self.operator, value_string)
 
     @property
     def value(self):
         return self._value
 
     @value.setter
     def value(self, filter_value):
```

### Comparing `tableauserverclient-0.9/tableauserverclient/models/connection_credentials.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/connection_credentials.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     @oauth.setter
     @property_is_boolean
     def oauth(self, value):
         self._oauth = value
 
     @classmethod
     def from_xml_element(cls, parsed_response, ns):
-        connection_creds_xml = parsed_response.find('.//t:connectionCredentials', namespaces=ns)
+        connection_creds_xml = parsed_response.find(".//t:connectionCredentials", namespaces=ns)
 
-        name = connection_creds_xml.get('name', None)
-        password = connection_creds_xml.get('password', None)
-        embed = connection_creds_xml.get('embed', None)
-        oAuth = connection_creds_xml.get('oAuth', None)
+        name = connection_creds_xml.get("name", None)
+        password = connection_creds_xml.get("password", None)
+        embed = connection_creds_xml.get("embed", None)
+        oAuth = connection_creds_xml.get("oAuth", None)
 
         connection_creds = cls(name, password, embed, oAuth)
         return connection_creds
```

### Comparing `tableauserverclient-0.9/tableauserverclient/models/property_decorators.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/property_decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import datetime
 import re
 from functools import wraps
+
 from ..datetime_helpers import parse_datetime
-try:
-    basestring
-except NameError:
-    # In case we are in python 3 the string check is different
-    basestring = str
 
 
 def property_is_enum(enum_type):
     def property_type_decorator(func):
         @wraps(func)
         def wrapper(self, value):
             if value is not None and not hasattr(enum_type, value):
@@ -66,89 +62,102 @@
             raise ValueError(error)
         return func(self, value)
 
     return wrapper
 
 
 def property_is_int(range, allowed=None):
-    '''Takes a range of ints and a list of exemptions to check against
+    """Takes a range of ints and a list of exemptions to check against
     when setting a property on a model. The range is a tuple of (min, max) and the
     allowed list (empty by default) allows values outside that range.
     This is useful for when we use sentinel values.
 
     Example: Revisions allow a range of 2-10000, but use -1 as a sentinel for 'unlimited'.
-    '''
+    """
 
     if allowed is None:
         allowed = ()  # Empty tuple for fast no-op testing.
 
     def property_type_decorator(func):
         @wraps(func)
         def wrapper(self, value):
-            error = "Invalid priority defined: {}.".format(value)
+            error = "Invalid property defined: '{}'. Integer value expected.".format(value)
 
             if range is None:
                 if isinstance(value, int):
                     return func(self, value)
                 else:
                     raise ValueError(error)
 
             min, max = range
 
             if (value < min or value > max) and (value not in allowed):
                 raise ValueError(error)
 
             return func(self, value)
+
         return wrapper
+
     return property_type_decorator
 
 
 def property_matches(regex_to_match, error):
 
     compiled_re = re.compile(regex_to_match)
 
     def wrapper(func):
         @wraps(func)
         def validate_regex_decorator(self, value):
             if not compiled_re.match(value):
                 raise ValueError(error)
             return func(self, value)
+
         return validate_regex_decorator
+
     return wrapper
 
 
 def property_is_datetime(func):
-    """ Takes the following datetime format and turns it into a datetime object:
+    """Takes the following datetime format and turns it into a datetime object:
 
     2016-08-18T18:25:36Z
 
     Because we return everything with Z as the timezone, we assume everything is in UTC and create
     a timezone aware datetime.
     """
 
     @wraps(func)
     def wrapper(self, value):
         if isinstance(value, datetime.datetime):
             return func(self, value)
-        if not isinstance(value, basestring):
-            raise ValueError("Cannot convert {} into a datetime, cannot update {}".format(value.__class__.__name__,
-                                                                                          func.__name__))
+        if not isinstance(value, str):
+            raise ValueError(
+                "Cannot convert {} into a datetime, cannot update {}".format(value.__class__.__name__, func.__name__)
+            )
 
         dt = parse_datetime(value)
         return func(self, dt)
+
     return wrapper
 
 
-def property_is_materialized_views_config(func):
+def property_is_data_acceleration_config(func):
     @wraps(func)
     def wrapper(self, value):
         if not isinstance(value, dict):
-            raise ValueError("{} is not type 'dict', cannot update {})".format(value.__class__.__name__,
-                                                                               func.__name__))
-        if len(value) != 2 or not all(attr in value.keys() for attr in ('materialized_views_enabled',
-                                                                        'run_materialization_now')):
+            raise ValueError("{} is not type 'dict', cannot update {})".format(value.__class__.__name__, func.__name__))
+        if len(value) != 4 or not all(
+            attr in value.keys()
+            for attr in (
+                "acceleration_enabled",
+                "accelerate_now",
+                "last_updated_at",
+                "acceleration_status",
+            )
+        ):
             error = "{} should have 2 keys ".format(func.__name__)
-            error += "'materialized_views_enabled' and 'run_materialization_now'"
+            error += "'acceleration_enabled' and 'accelerate_now'"
             error += "instead you have {}".format(value.keys())
             raise ValueError(error)
         return func(self, value)
+
     return wrapper
```

### Comparing `tableauserverclient-0.9/tableauserverclient/models/view_item.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/subscription_item.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,153 +1,136 @@
-import xml.etree.ElementTree as ET
-from ..datetime_helpers import parse_datetime
-from .exceptions import UnpopulatedPropertyError
-from .tag_item import TagItem
+from typing import List, Type, TYPE_CHECKING
 
+from defusedxml.ElementTree import fromstring
 
-class ViewItem(object):
-    def __init__(self):
-        self._content_url = None
-        self._created_at = None
-        self._id = None
-        self._image = None
-        self._initial_tags = set()
-        self._name = None
-        self._owner_id = None
-        self._preview_image = None
-        self._project_id = None
-        self._pdf = None
-        self._csv = None
-        self._total_views = None
-        self._sheet_type = None
-        self._updated_at = None
-        self._workbook_id = None
-        self.tags = set()
-
-    def _set_preview_image(self, preview_image):
-        self._preview_image = preview_image
-
-    def _set_image(self, image):
-        self._image = image
+from .property_decorators import property_is_boolean
+from .target import Target
 
-    def _set_pdf(self, pdf):
-        self._pdf = pdf
+if TYPE_CHECKING:
+    from .target import Target
 
-    def _set_csv(self, csv):
-        self._csv = csv
 
-    @property
-    def content_url(self):
-        return self._content_url
-
-    @property
-    def created_at(self):
-        return self._created_at
+class SubscriptionItem(object):
+    def __init__(self, subject: str, schedule_id: str, user_id: str, target: "Target") -> None:
+        self._id = None
+        self.attach_image = True
+        self.attach_pdf = False
+        self.message = None
+        self.page_orientation = None
+        self.page_size_option = None
+        self.schedule_id = schedule_id
+        self.send_if_view_empty = True
+        self.subject = subject
+        self.suspended = False
+        self.target = target
+        self.user_id = user_id
+
+    def __repr__(self) -> str:
+        if self.id is not None:
+            return "<Subscription#{_id} subject({subject}) schedule_id({schedule_id}) user_id({user_id}) \
+                target({target})".format(
+                **self.__dict__
+            )
+        else:
+            return "<Subscription subject({subject}) schedule_id({schedule_id}) user_id({user_id}) \
+                target({target})".format(
+                **self.__dict__
+            )
 
     @property
     def id(self):
         return self._id
 
     @property
-    def image(self):
-        if self._image is None:
-            error = "View item must be populated with its png image first."
-            raise UnpopulatedPropertyError(error)
-        return self._image()
-
-    @property
-    def name(self):
-        return self._name
-
-    @property
-    def owner_id(self):
-        return self._owner_id
+    def attach_image(self) -> bool:
+        return self._attach_image
 
-    @property
-    def preview_image(self):
-        if self._preview_image is None:
-            error = "View item must be populated with its preview image first."
-            raise UnpopulatedPropertyError(error)
-        return self._preview_image()
+    @attach_image.setter
+    @property_is_boolean
+    def attach_image(self, value: bool):
+        self._attach_image = value
 
     @property
-    def project_id(self):
-        return self._project_id
+    def attach_pdf(self) -> bool:
+        return self._attach_pdf
 
-    @property
-    def pdf(self):
-        if self._pdf is None:
-            error = "View item must be populated with its pdf first."
-            raise UnpopulatedPropertyError(error)
-        return self._pdf()
+    @attach_pdf.setter
+    @property_is_boolean
+    def attach_pdf(self, value: bool) -> None:
+        self._attach_pdf = value
 
     @property
-    def csv(self):
-        if self._csv is None:
-            error = "View item must be populated with its csv first."
-            raise UnpopulatedPropertyError(error)
-        return self._csv()
+    def send_if_view_empty(self) -> bool:
+        return self._send_if_view_empty
 
-    @property
-    def sheet_type(self):
-        return self._sheet_type
+    @send_if_view_empty.setter
+    @property_is_boolean
+    def send_if_view_empty(self, value: bool) -> None:
+        self._send_if_view_empty = value
 
     @property
-    def total_views(self):
-        if self._total_views is None:
-            error = "Usage statistics must be requested when querying for view."
-            raise UnpopulatedPropertyError(error)
-        return self._total_views
+    def suspended(self) -> bool:
+        return self._suspended
 
-    @property
-    def updated_at(self):
-        return self._updated_at
-
-    @property
-    def workbook_id(self):
-        return self._workbook_id
+    @suspended.setter
+    @property_is_boolean
+    def suspended(self, value: bool) -> None:
+        self._suspended = value
 
     @classmethod
-    def from_response(cls, resp, ns, workbook_id=''):
-        return cls.from_xml_element(ET.fromstring(resp), ns, workbook_id)
+    def from_response(cls: Type, xml: bytes, ns) -> List["SubscriptionItem"]:
+        parsed_response = fromstring(xml)
+        all_subscriptions_xml = parsed_response.findall(".//t:subscription", namespaces=ns)
 
-    @classmethod
-    def from_xml_element(cls, parsed_response, ns, workbook_id=''):
-        all_view_items = list()
-        all_view_xml = parsed_response.findall('.//t:view', namespaces=ns)
-        for view_xml in all_view_xml:
-            view_item = cls()
-            usage_elem = view_xml.find('.//t:usage', namespaces=ns)
-            workbook_elem = view_xml.find('.//t:workbook', namespaces=ns)
-            owner_elem = view_xml.find('.//t:owner', namespaces=ns)
-            project_elem = view_xml.find('.//t:project', namespaces=ns)
-            tags_elem = view_xml.find('.//t:tags', namespaces=ns)
-            view_item._created_at = parse_datetime(view_xml.get('createdAt', None))
-            view_item._updated_at = parse_datetime(view_xml.get('updatedAt', None))
-            view_item._id = view_xml.get('id', None)
-            view_item._name = view_xml.get('name', None)
-            view_item._content_url = view_xml.get('contentUrl', None)
-            view_item._sheet_type = view_xml.get('sheetType', None)
-
-            if usage_elem is not None:
-                total_view = usage_elem.get('totalViewCount', None)
-                if total_view:
-                    view_item._total_views = int(total_view)
-
-            if owner_elem is not None:
-                view_item._owner_id = owner_elem.get('id', None)
-
-            if project_elem is not None:
-                view_item._project_id = project_elem.get('id', None)
-
-            if workbook_id:
-                view_item._workbook_id = workbook_id
-            elif workbook_elem is not None:
-                view_item._workbook_id = workbook_elem.get('id', None)
-
-            if tags_elem is not None:
-                tags = TagItem.from_xml_element(tags_elem, ns)
-                view_item.tags = tags
-                view_item._initial_tags = tags
+        all_subscriptions = [SubscriptionItem._parse_element(x, ns) for x in all_subscriptions_xml]
+        return all_subscriptions
 
-            all_view_items.append(view_item)
-        return all_view_items
+    @classmethod
+    def _parse_element(cls, element, ns):
+        schedule_element = element.find(".//t:schedule", namespaces=ns)
+        content_element = element.find(".//t:content", namespaces=ns)
+        user_element = element.find(".//t:user", namespaces=ns)
+
+        # Schedule element
+        schedule_id = None
+        if schedule_element is not None:
+            schedule_id = schedule_element.get("id", None)
+
+        # Content element
+        target = None
+        send_if_view_empty = None
+        if content_element is not None:
+            target = Target(content_element.get("id", None), content_element.get("type"))
+            send_if_view_empty = string_to_bool(content_element.get("sendIfViewEmpty", ""))
+
+        # User element
+        user_id = None
+        if user_element is not None:
+            user_id = user_element.get("id", None)
+
+        # Main attributes
+        id_ = element.get("id", None)
+        subject = element.get("subject", None)
+        attach_image = string_to_bool(element.get("attachImage", ""))
+        attach_pdf = string_to_bool(element.get("attachPdf", ""))
+        message = element.get("message", None)
+        page_orientation = element.get("pageOrientation", None)
+        page_size_option = element.get("pageSizeOption", None)
+        suspended = string_to_bool(element.get("suspended", ""))
+
+        # Create SubscriptionItem and set fields
+        sub = cls(subject, schedule_id, user_id, target)
+        sub._id = id_
+        sub.attach_image = attach_image
+        sub.attach_pdf = attach_pdf
+        sub.message = message
+        sub.page_orientation = page_orientation
+        sub.page_size_option = page_size_option
+        sub.send_if_view_empty = send_if_view_empty
+        sub.suspended = suspended
+
+        return sub
+
+
+# Used to convert string represented boolean to a boolean type
+def string_to_bool(s: str) -> bool:
+    return s.lower() == "true"
```

### Comparing `tableauserverclient-0.9/tableauserverclient/models/tableau_auth.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/tableau_auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 class TableauAuth(object):
-    def __init__(self, username, password, site=None, site_id='', user_id_to_impersonate=None):
+    def __init__(self, username, password, site=None, site_id=None, user_id_to_impersonate=None):
         if site is not None:
             import warnings
-            warnings.warn('TableauAuth(...site=""...) is deprecated, '
-                          'please use TableauAuth(...site_id=""...) instead.',
-                          DeprecationWarning)
+
+            warnings.warn(
+                "TableauAuth(..., site=...) is deprecated, " "please use TableauAuth(..., site_id=...) instead.",
+                DeprecationWarning,
+            )
             site_id = site
+        if password is None:
+            raise TabError("Must provide a password when using traditional authentication")
 
         self.user_id_to_impersonate = user_id_to_impersonate
         self.password = password
-        self.site_id = site_id
+        self.site_id = site_id if site_id is not None else ""
         self.username = username
 
     @property
     def site(self):
         import warnings
-        warnings.warn('TableauAuth.site is deprecated, use TableauAuth.site_id instead.',
-                      DeprecationWarning)
+
+        warnings.warn(
+            "TableauAuth.site is deprecated, use TableauAuth.site_id instead.",
+            DeprecationWarning,
+        )
         return self.site_id
 
     @site.setter
     def site(self, value):
         import warnings
-        warnings.warn('TableauAuth.site is deprecated, use TableauAuth.site_id instead.',
-                      DeprecationWarning)
+
+        warnings.warn(
+            "TableauAuth.site is deprecated, use TableauAuth.site_id instead.",
+            DeprecationWarning,
+        )
         self.site_id = value
 
     @property
     def credentials(self):
-        return {'name': self.username, 'password': self.password}
+        return {"name": self.username, "password": self.password}
```

### Comparing `tableauserverclient-0.9/tableauserverclient/models/database_item.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/database_item.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-import xml.etree.ElementTree as ET
+from defusedxml.ElementTree import fromstring
 
-from .permissions_item import Permission
-
-from .property_decorators import property_is_enum, property_not_empty, property_is_boolean
 from .exceptions import UnpopulatedPropertyError
+from .property_decorators import (
+    property_is_enum,
+    property_not_empty,
+    property_is_boolean,
+)
 
 
 class DatabaseItem(object):
     class ContentPermissions:
-        LockedToProject = 'LockedToDatabase'
-        ManagedByOwner = 'ManagedByOwner'
+        LockedToProject = "LockedToDatabase"
+        ManagedByOwner = "ManagedByOwner"
 
     def __init__(self, name, description=None, content_permissions=None):
         self._id = None
         self.name = name
         self.description = description
         self.content_permissions = content_permissions
         self._certified = None
@@ -32,39 +34,48 @@
         self._port = None
         self._provider = None
         self._request_url = None
 
         self._permissions = None
         self._default_table_permissions = None
 
+        self._data_quality_warnings = None
+
         self._tables = None  # Not implemented yet
 
     @property
+    def dqws(self):
+        if self._data_quality_warnings is None:
+            error = "Project item must be populated with permissions first."
+            raise UnpopulatedPropertyError(error)
+        return self._data_quality_warnings()
+
+    @property
     def content_permissions(self):
         return self._content_permissions
 
+    @content_permissions.setter
+    @property_is_enum(ContentPermissions)
+    def content_permissions(self, value):
+        self._content_permissions = value
+
     @property
     def permissions(self):
         if self._permissions is None:
             error = "Project item must be populated with permissions first."
             raise UnpopulatedPropertyError(error)
         return self._permissions()
 
     @property
     def default_table_permissions(self):
         if self._default_table_permissions is None:
             error = "Project item must be populated with permissions first."
             raise UnpopulatedPropertyError(error)
         return self._default_table_permissions()
 
-    @content_permissions.setter
-    @property_is_enum(ContentPermissions)
-    def content_permissions(self, value):
-        self._content_permissions = value
-
     @property
     def id(self):
         return self._id
 
     @property
     def name(self):
         return self._name
@@ -161,100 +172,107 @@
             error = "Database must be populated with tables first."
             raise UnpopulatedPropertyError(error)
         #  Each call to `.tables` should create a new pager, this just runs the callable
         return self._tables()
 
     def _set_values(self, database_values):
         # ID & Settable
-        if 'id' in database_values:
-            self._id = database_values['id']
+        if "id" in database_values:
+            self._id = database_values["id"]
 
-        if 'contact' in database_values:
-            self._contact_id = database_values['contact']['id']
+        if "contact" in database_values:
+            self._contact_id = database_values["contact"]["id"]
 
-        if 'name' in database_values:
-            self._name = database_values['name']
+        if "name" in database_values:
+            self._name = database_values["name"]
 
-        if 'description' in database_values:
-            self._description = database_values['description']
+        if "description" in database_values:
+            self._description = database_values["description"]
 
-        if 'isCertified' in database_values:
-            self._certified = string_to_bool(database_values['isCertified'])
+        if "isCertified" in database_values:
+            self._certified = string_to_bool(database_values["isCertified"])
 
-        if 'certificationNote' in database_values:
-            self._certification_note = database_values['certificationNote']
+        if "certificationNote" in database_values:
+            self._certification_note = database_values["certificationNote"]
 
         # Not settable, alphabetical
 
-        if 'connectionType' in database_values:
-            self._connection_type = database_values['connectionType']
+        if "connectionType" in database_values:
+            self._connection_type = database_values["connectionType"]
 
-        if 'connectorUrl' in database_values:
-            self._connector_url = database_values['connectorUrl']
+        if "connectorUrl" in database_values:
+            self._connector_url = database_values["connectorUrl"]
 
-        if 'contentPermissions' in database_values:
-            self._content_permissions = database_values['contentPermissions']
+        if "contentPermissions" in database_values:
+            self._content_permissions = database_values["contentPermissions"]
 
-        if 'isEmbedded' in database_values:
-            self._embedded = string_to_bool(database_values['isEmbedded'])
+        if "isEmbedded" in database_values:
+            self._embedded = string_to_bool(database_values["isEmbedded"])
 
-        if 'fileExtension' in database_values:
-            self._file_extension = database_values['fileExtension']
+        if "fileExtension" in database_values:
+            self._file_extension = database_values["fileExtension"]
 
-        if 'fileId' in database_values:
-            self._file_id = database_values['fileId']
+        if "fileId" in database_values:
+            self._file_id = database_values["fileId"]
 
-        if 'filePath' in database_values:
-            self._file_path = database_values['filePath']
+        if "filePath" in database_values:
+            self._file_path = database_values["filePath"]
 
-        if 'hostName' in database_values:
-            self._host_name = database_values['hostName']
+        if "hostName" in database_values:
+            self._host_name = database_values["hostName"]
 
-        if 'mimeType' in database_values:
-            self._mime_type = database_values['mimeType']
+        if "mimeType" in database_values:
+            self._mime_type = database_values["mimeType"]
 
-        if 'port' in database_values:
-            self._port = int(database_values['port'])
+        if "port" in database_values:
+            self._port = int(database_values["port"])
 
-        if 'provider' in database_values:
-            self._provider = database_values['provider']
+        if "provider" in database_values:
+            self._provider = database_values["provider"]
 
-        if 'requestUrl' in database_values:
-            self._request_url = database_values['requestUrl']
+        if "requestUrl" in database_values:
+            self._request_url = database_values["requestUrl"]
 
-        if 'type' in database_values:
-            self._metadata_type = database_values['type']
+        if "type" in database_values:
+            self._metadata_type = database_values["type"]
 
     def _set_permissions(self, permissions):
         self._permissions = permissions
 
     def _set_tables(self, tables):
         self._tables = tables
 
     def _set_default_permissions(self, permissions, content_type):
-        setattr(self, "_default_{content}_permissions".format(content=content_type), permissions)
+        setattr(
+            self,
+            "_default_{content}_permissions".format(content=content_type),
+            permissions,
+        )
+
+    def _set_data_quality_warnings(self, dqw):
+        self._data_quality_warnings = dqw
 
     @classmethod
     def from_response(cls, resp, ns):
         all_database_items = list()
-        parsed_response = ET.fromstring(resp)
-        all_database_xml = parsed_response.findall('.//t:database', namespaces=ns)
+        parsed_response = fromstring(resp)
+        all_database_xml = parsed_response.findall(".//t:database", namespaces=ns)
 
         for database_xml in all_database_xml:
             parsed_database = cls._parse_element(database_xml, ns)
-            database_item = cls(parsed_database['name'])
+            database_item = cls(parsed_database["name"])
             database_item._set_values(parsed_database)
             all_database_items.append(database_item)
         return all_database_items
 
     @staticmethod
     def _parse_element(database_xml, ns):
         database_values = database_xml.attrib.copy()
-        contact = database_xml.find('.//t:contact', namespaces=ns)
+        contact = database_xml.find(".//t:contact", namespaces=ns)
         if contact is not None:
-            database_values['contact'] = contact.attrib.copy()
+            database_values["contact"] = contact.attrib.copy()
         return database_values
 
 
 # Used to convert string represented boolean to a boolean type
 def string_to_bool(s):
-    return s.lower() == 'true'
+    return s.lower() == "true"
```

### Comparing `tableauserverclient-0.9/tableauserverclient/models/permissions_item.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/permissions_item.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,95 +1,102 @@
-import xml.etree.ElementTree as ET
 import logging
+import xml.etree.ElementTree as ET
 
-from .exceptions import UnknownGranteeTypeError
-from .user_item import UserItem
+from defusedxml.ElementTree import fromstring
+from .exceptions import UnknownGranteeTypeError, UnpopulatedPropertyError
 from .group_item import GroupItem
+from .user_item import UserItem
 
-logger = logging.getLogger('tableau.models.permissions_item')
+logger = logging.getLogger("tableau.models.permissions_item")
 
+from typing import Dict, List, Optional, TYPE_CHECKING
 
-class Permission:
+if TYPE_CHECKING:
+    from .reference_item import ResourceReference
 
+
+class Permission:
     class Mode:
-        Allow = 'Allow'
-        Deny = 'Deny'
+        Allow = "Allow"
+        Deny = "Deny"
 
     class Capability:
-        AddComment = 'AddComment'
-        ChangeHierarchy = 'ChangeHierarchy'
-        ChangePermissions = 'ChangePermissions'
-        Connect = 'Connect'
-        Delete = 'Delete'
-        ExportData = 'ExportData'
-        ExportImage = 'ExportImage'
-        ExportXml = 'ExportXml'
-        Filter = 'Filter'
-        ProjectLeader = 'ProjectLeader'
-        Read = 'Read'
-        ShareView = 'ShareView'
-        ViewComments = 'ViewComments'
-        ViewUnderlyingData = 'ViewUnderlyingData'
-        WebAuthoring = 'WebAuthoring'
-        Write = 'Write'
+        AddComment = "AddComment"
+        ChangeHierarchy = "ChangeHierarchy"
+        ChangePermissions = "ChangePermissions"
+        Connect = "Connect"
+        Delete = "Delete"
+        Execute = "Execute"
+        ExportData = "ExportData"
+        ExportImage = "ExportImage"
+        ExportXml = "ExportXml"
+        Filter = "Filter"
+        ProjectLeader = "ProjectLeader"
+        Read = "Read"
+        ShareView = "ShareView"
+        ViewComments = "ViewComments"
+        ViewUnderlyingData = "ViewUnderlyingData"
+        WebAuthoring = "WebAuthoring"
+        Write = "Write"
 
     class Resource:
-        Workbook = 'workbook'
-        Datasource = 'datasource'
-        Flow = 'flow'
-        Table = 'table'
-        Database = 'database'
+        Workbook = "workbook"
+        Datasource = "datasource"
+        Flow = "flow"
+        Table = "table"
+        Database = "database"
+        View = "view"
 
 
 class PermissionsRule(object):
-
-    def __init__(self, grantee, capabilities):
+    def __init__(self, grantee: "ResourceReference", capabilities: Dict[str, str]) -> None:
         self.grantee = grantee
         self.capabilities = capabilities
 
     @classmethod
-    def from_response(cls, resp, ns=None):
-        parsed_response = ET.fromstring(resp)
+    def from_response(cls, resp, ns=None) -> List["PermissionsRule"]:
+        parsed_response = fromstring(resp)
 
         rules = []
-        permissions_rules_list_xml = parsed_response.findall('.//t:granteeCapabilities',
-                                                             namespaces=ns)
+        permissions_rules_list_xml = parsed_response.findall(".//t:granteeCapabilities", namespaces=ns)
 
         for grantee_capability_xml in permissions_rules_list_xml:
-            capability_dict = {}
+            capability_dict: Dict[str, str] = {}
 
             grantee = PermissionsRule._parse_grantee_element(grantee_capability_xml, ns)
 
-            for capability_xml in grantee_capability_xml.findall(
-                    './/t:capabilities/t:capability', namespaces=ns):
-                name = capability_xml.get('name')
-                mode = capability_xml.get('mode')
-
-                capability_dict[name] = mode
+            for capability_xml in grantee_capability_xml.findall(".//t:capabilities/t:capability", namespaces=ns):
+                name = capability_xml.get("name")
+                mode = capability_xml.get("mode")
+
+                if name is None or mode is None:
+                    logger.error("Capability was not valid: ", capability_xml)
+                    raise UnpopulatedPropertyError()
+                else:
+                    capability_dict[name] = mode
 
-            rule = PermissionsRule(grantee,
-                                   capability_dict)
+            rule = PermissionsRule(grantee, capability_dict)
             rules.append(rule)
 
         return rules
 
     @staticmethod
-    def _parse_grantee_element(grantee_capability_xml, ns):
+    def _parse_grantee_element(grantee_capability_xml: ET.Element, ns: Optional[Dict[str, str]]) -> "ResourceReference":
         """Use Xpath magic and some string splitting to get the right object type from the xml"""
 
         # Get the first element in the tree with an 'id' attribute
-        grantee_element = grantee_capability_xml.findall('.//*[@id]', namespaces=ns).pop()
-        grantee_id = grantee_element.get('id', None)
-        grantee_type = grantee_element.tag.split('}').pop()
+        grantee_element = grantee_capability_xml.findall(".//*[@id]", namespaces=ns).pop()
+        grantee_id = grantee_element.get("id", None)
+        grantee_type = grantee_element.tag.split("}").pop()
 
         if grantee_id is None:
-            logger.error('Cannot find grantee type in response')
+            logger.error("Cannot find grantee type in response")
             raise UnknownGranteeTypeError()
 
-        if grantee_type == 'user':
+        if grantee_type == "user":
             grantee = UserItem.as_reference(grantee_id)
-        elif grantee_type == 'group':
+        elif grantee_type == "group":
             grantee = GroupItem.as_reference(grantee_id)
         else:
             raise UnknownGranteeTypeError("No support for grantee type of {}".format(grantee_type))
 
         return grantee
```

### Comparing `tableauserverclient-0.9/tableauserverclient/models/interval_item.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/interval_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,38 +58,39 @@
 
     @property
     def interval(self):
         return self._interval
 
     @interval.setter
     def interval(self, interval):
-        VALID_INTERVALS = {.25, .5, 1, 2, 4, 6, 8, 12}
+        VALID_INTERVALS = {0.25, 0.5, 1, 2, 4, 6, 8, 12}
         if float(interval) not in VALID_INTERVALS:
             error = "Invalid interval {} not in {}".format(interval, str(VALID_INTERVALS))
             raise ValueError(error)
 
         self._interval = interval
 
     def _interval_type_pairs(self):
 
         # We use fractional hours for the two minute-based intervals.
         # Need to convert to minutes from hours here
-        if self.interval in {.25, .5}:
+        if self.interval in {0.25, 0.5}:
             calculated_interval = int(self.interval * 60)
             interval_type = IntervalItem.Occurrence.Minutes
         else:
             calculated_interval = self.interval
             interval_type = IntervalItem.Occurrence.Hours
 
         return [(interval_type, str(calculated_interval))]
 
 
 class DailyInterval(object):
-    def __init__(self, start_time):
+    def __init__(self, start_time, *interval_values):
         self.start_time = start_time
+        self.interval = interval_values
 
     @property
     def _frequency(self):
         return IntervalItem.Frequency.Daily
 
     @property
     def start_time(self):
@@ -97,14 +98,22 @@
 
     @start_time.setter
     @property_is_valid_time
     @property_not_nullable
     def start_time(self, value):
         self._start_time = value
 
+    @property
+    def interval(self):
+        return self._interval
+
+    @interval.setter
+    def interval(self, interval):
+        self._interval = interval
+
 
 class WeeklyInterval(object):
     def __init__(self, start_time, *interval_values):
         self.start_time = start_time
         self.interval = interval_values
 
     @property
@@ -169,15 +178,15 @@
         # like 'badstring' we catch and re-raise. Otherwise we convert to int and check
         # that it's in range 1-31
 
         if interval_value != "LastDay":
             try:
                 if not (1 <= int(interval_value) <= 31):
                     raise ValueError(error)
-            except ValueError as e:
+            except ValueError:
                 if interval_value != "LastDay":
                     raise ValueError(error)
 
         self._interval = str(interval_value)
 
     def _interval_type_pairs(self):
         return [(IntervalItem.Occurrence.MonthDay, self.interval)]
```

### Comparing `tableauserverclient-0.9/tableauserverclient/models/__init__.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,40 @@
+from .column_item import ColumnItem
 from .connection_credentials import ConnectionCredentials
 from .connection_item import ConnectionItem
-from .column_item import ColumnItem
-from .datasource_item import DatasourceItem
+from .data_acceleration_report_item import DataAccelerationReportItem
+from .data_alert_item import DataAlertItem
 from .database_item import DatabaseItem
+from .datasource_item import DatasourceItem
+from .dqw_item import DQWItem
 from .exceptions import UnpopulatedPropertyError
-from .group_item import GroupItem
+from .favorites_item import FavoriteItem
 from .flow_item import FlowItem
-from .interval_item import IntervalItem, DailyInterval, WeeklyInterval, MonthlyInterval, HourlyInterval
+from .flow_run_item import FlowRunItem
+from .group_item import GroupItem
+from .interval_item import (
+    IntervalItem,
+    DailyInterval,
+    WeeklyInterval,
+    MonthlyInterval,
+    HourlyInterval,
+)
 from .job_item import JobItem, BackgroundJobItem
+from .metric_item import MetricItem
 from .pagination_item import PaginationItem
+from .permissions_item import PermissionsRule, Permission
+from .personal_access_token_auth import PersonalAccessTokenAuth
+from .personal_access_token_auth import PersonalAccessTokenAuth
 from .project_item import ProjectItem
+from .revision_item import RevisionItem
 from .schedule_item import ScheduleItem
 from .server_info_item import ServerInfoItem
 from .site_item import SiteItem
+from .subscription_item import SubscriptionItem
+from .table_item import TableItem
 from .tableau_auth import TableauAuth
-from .personal_access_token_auth import PersonalAccessTokenAuth
 from .target import Target
-from .table_item import TableItem
 from .task_item import TaskItem
 from .user_item import UserItem
 from .view_item import ViewItem
+from .webhook_item import WebhookItem
 from .workbook_item import WorkbookItem
-from .subscription_item import SubscriptionItem
-from .permissions_item import PermissionsRule, Permission
```

### Comparing `tableauserverclient-0.9/tableauserverclient/models/table_item.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/table_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import xml.etree.ElementTree as ET
+from defusedxml.ElementTree import fromstring
 
-from .permissions_item import Permission
-from .column_item import ColumnItem
-
-from .property_decorators import property_is_enum, property_not_empty, property_is_boolean
 from .exceptions import UnpopulatedPropertyError
+from .property_decorators import property_not_empty, property_is_boolean
 
 
 class TableItem(object):
     def __init__(self, name, description=None):
         self._id = None
         self.description = description
         self.name = name
@@ -16,23 +13,31 @@
         self._contact_id = None
         self._certified = None
         self._certification_note = None
         self._permissions = None
         self._schema = None
 
         self._columns = None
+        self._data_quality_warnings = None
 
     @property
     def permissions(self):
         if self._permissions is None:
             error = "Project item must be populated with permissions first."
             raise UnpopulatedPropertyError(error)
         return self._permissions()
 
     @property
+    def dqws(self):
+        if self._data_quality_warnings is None:
+            error = "Project item must be populated with dqws first."
+            raise UnpopulatedPropertyError(error)
+        return self._data_quality_warnings()
+
+    @property
     def id(self):
         return self._id
 
     @property
     def name(self):
         return self._name
 
@@ -85,63 +90,66 @@
             raise UnpopulatedPropertyError(error)
         #  Each call to `.columns` should create a new pager, this just runs the callable
         return self._columns()
 
     def _set_columns(self, columns):
         self._columns = columns
 
+    def _set_data_quality_warnings(self, dqws):
+        self._data_quality_warnings = dqws
+
     def _set_values(self, table_values):
-        if 'id' in table_values:
-            self._id = table_values['id']
+        if "id" in table_values:
+            self._id = table_values["id"]
 
-        if 'name' in table_values:
-            self._name = table_values['name']
+        if "name" in table_values:
+            self._name = table_values["name"]
 
-        if 'description' in table_values:
-            self._description = table_values['description']
+        if "description" in table_values:
+            self._description = table_values["description"]
 
-        if 'isCertified' in table_values:
-            self._certified = string_to_bool(table_values['isCertified'])
+        if "isCertified" in table_values:
+            self._certified = string_to_bool(table_values["isCertified"])
 
-        if 'certificationNote' in table_values:
-            self._certification_note = table_values['certificationNote']
+        if "certificationNote" in table_values:
+            self._certification_note = table_values["certificationNote"]
 
-        if 'isEmbedded' in table_values:
-            self._embedded = string_to_bool(table_values['isEmbedded'])
+        if "isEmbedded" in table_values:
+            self._embedded = string_to_bool(table_values["isEmbedded"])
 
-        if 'schema' in table_values:
-            self._schema = table_values['schema']
+        if "schema" in table_values:
+            self._schema = table_values["schema"]
 
-        if 'contact' in table_values:
-            self._contact_id = table_values['contact']['id']
+        if "contact" in table_values:
+            self._contact_id = table_values["contact"]["id"]
 
     def _set_permissions(self, permissions):
         self._permissions = permissions
 
     @classmethod
     def from_response(cls, resp, ns):
         all_table_items = list()
-        parsed_response = ET.fromstring(resp)
-        all_table_xml = parsed_response.findall('.//t:table', namespaces=ns)
+        parsed_response = fromstring(resp)
+        all_table_xml = parsed_response.findall(".//t:table", namespaces=ns)
 
         for table_xml in all_table_xml:
             parsed_table = cls._parse_element(table_xml, ns)
             table_item = cls(parsed_table["name"])
             table_item._set_values(parsed_table)
             all_table_items.append(table_item)
         return all_table_items
 
     @staticmethod
     def _parse_element(table_xml, ns):
 
         table_values = table_xml.attrib.copy()
 
-        contact = table_xml.find('.//t:contact', namespaces=ns)
+        contact = table_xml.find(".//t:contact", namespaces=ns)
         if contact is not None:
-            table_values['contact'] = contact.attrib.copy()
+            table_values["contact"] = contact.attrib.copy()
 
         return table_values
 
 
 # Used to convert string represented boolean to a boolean type
 def string_to_bool(s):
-    return s.lower() == 'true'
+    return s.lower() == "true"
```

### Comparing `tableauserverclient-0.9/tableauserverclient/models/fileupload_item.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/fileupload_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import xml.etree.ElementTree as ET
+from defusedxml.ElementTree import fromstring
 
 
 class FileuploadItem(object):
     def __init__(self):
         self._file_size = None
         self._upload_session_id = None
 
@@ -12,13 +12,13 @@
 
     @property
     def file_size(self):
         return self._file_size
 
     @classmethod
     def from_response(cls, resp, ns):
-        parsed_response = ET.fromstring(resp)
-        fileupload_elem = parsed_response.find('.//t:fileUpload', namespaces=ns)
+        parsed_response = fromstring(resp)
+        fileupload_elem = parsed_response.find(".//t:fileUpload", namespaces=ns)
         fileupload_item = cls()
-        fileupload_item._upload_session_id = fileupload_elem.get('uploadSessionId', None)
-        fileupload_item._file_size = fileupload_elem.get('fileSize', None)
+        fileupload_item._upload_session_id = fileupload_elem.get("uploadSessionId", None)
+        fileupload_item._file_size = fileupload_elem.get("fileSize", None)
         return fileupload_item
```

### Comparing `tableauserverclient-0.9/tableauserverclient/models/group_item.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/group_item.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,110 @@
-import xml.etree.ElementTree as ET
+from typing import Callable, List, Optional, TYPE_CHECKING
+
+from defusedxml.ElementTree import fromstring
+
 from .exceptions import UnpopulatedPropertyError
-from .property_decorators import property_not_empty
+from .property_decorators import property_not_empty, property_is_enum
 from .reference_item import ResourceReference
+from .user_item import UserItem
+
+if TYPE_CHECKING:
+    from ..server import Pager
 
 
 class GroupItem(object):
 
-    tag_name = 'group'
+    tag_name: str = "group"
 
-    def __init__(self, name=None):
-        self._domain_name = None
-        self._id = None
-        self._users = None
-        self.name = name
+    class LicenseMode:
+        onLogin: str = "onLogin"
+        onSync: str = "onSync"
+
+    def __init__(self, name=None, domain_name=None) -> None:
+        self._id: Optional[str] = None
+        self._license_mode: Optional[str] = None
+        self._minimum_site_role: Optional[str] = None
+        self._users: Optional[Callable[..., "Pager"]] = None
+        self.name: Optional[str] = name
+        self.domain_name: Optional[str] = domain_name
 
     @property
-    def domain_name(self):
+    def domain_name(self) -> Optional[str]:
         return self._domain_name
 
+    @domain_name.setter
+    def domain_name(self, value: str) -> None:
+        self._domain_name = value
+
     @property
-    def id(self):
+    def id(self) -> Optional[str]:
         return self._id
 
     @property
-    def name(self):
+    def name(self) -> Optional[str]:
         return self._name
 
     @name.setter
     @property_not_empty
-    def name(self, value):
+    def name(self, value: str) -> None:
         self._name = value
 
     @property
-    def users(self):
+    def license_mode(self) -> Optional[str]:
+        return self._license_mode
+
+    @license_mode.setter
+    @property_is_enum(LicenseMode)
+    def license_mode(self, value: str) -> None:
+        self._license_mode = value
+
+    @property
+    def minimum_site_role(self) -> Optional[str]:
+        return self._minimum_site_role
+
+    @minimum_site_role.setter
+    @property_is_enum(UserItem.Roles)
+    def minimum_site_role(self, value: str) -> None:
+        self._minimum_site_role = value
+
+    @property
+    def users(self) -> "Pager":
         if self._users is None:
             error = "Group must be populated with users first."
             raise UnpopulatedPropertyError(error)
         #  Each call to `.users` should create a new pager, this just runs the callable
         return self._users()
 
-    def to_reference(self):
+    def to_reference(self) -> ResourceReference:
         return ResourceReference(id_=self.id, tag_name=self.tag_name)
 
-    def _set_users(self, users):
+    def _set_users(self, users: Callable[..., "Pager"]) -> None:
         self._users = users
 
     @classmethod
-    def from_response(cls, resp, ns):
+    def from_response(cls, resp, ns) -> List["GroupItem"]:
         all_group_items = list()
-        parsed_response = ET.fromstring(resp)
-        all_group_xml = parsed_response.findall('.//t:group', namespaces=ns)
+        parsed_response = fromstring(resp)
+        all_group_xml = parsed_response.findall(".//t:group", namespaces=ns)
         for group_xml in all_group_xml:
-            name = group_xml.get('name', None)
+            name = group_xml.get("name", None)
             group_item = cls(name)
-            group_item._id = group_xml.get('id', None)
+            group_item._id = group_xml.get("id", None)
 
-            domain_elem = group_xml.find('.//t:domain', namespaces=ns)
+            # Domain name is returned in a domain element for some calls
+            domain_elem = group_xml.find(".//t:domain", namespaces=ns)
             if domain_elem is not None:
-                group_item._domain_name = domain_elem.get('name', None)
+                group_item.domain_name = domain_elem.get("name", None)
+
+            # Import element is returned for both local and AD groups (2020.3+)
+            import_elem = group_xml.find(".//t:import", namespaces=ns)
+            if import_elem is not None:
+                group_item.domain_name = import_elem.get("domainName", None)
+                group_item.license_mode = import_elem.get("grantLicenseMode", None)
+                group_item.minimum_site_role = import_elem.get("siteRole", None)
+
             all_group_items.append(group_item)
         return all_group_items
 
     @staticmethod
-    def as_reference(id_):
+    def as_reference(id_: str) -> ResourceReference:
         return ResourceReference(id_, GroupItem.tag_name)
```

### Comparing `tableauserverclient-0.9/tableauserverclient/models/column_item.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/column_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import xml.etree.ElementTree as ET
+from defusedxml.ElementTree import fromstring
 
-from .property_decorators import property_is_enum, property_not_empty
-from .exceptions import UnpopulatedPropertyError
+from .property_decorators import property_not_empty
 
 
 class ColumnItem(object):
     def __init__(self, name, description=None):
         self._id = None
         self.description = description
         self.name = name
@@ -44,26 +43,26 @@
             self.description = description
         if remote_type:
             self._remote_type = remote_type
 
     @classmethod
     def from_response(cls, resp, ns):
         all_column_items = list()
-        parsed_response = ET.fromstring(resp)
-        all_column_xml = parsed_response.findall('.//t:column', namespaces=ns)
+        parsed_response = fromstring(resp)
+        all_column_xml = parsed_response.findall(".//t:column", namespaces=ns)
 
         for column_xml in all_column_xml:
             (id, name, description, remote_type) = cls._parse_element(column_xml, ns)
             column_item = cls(name)
             column_item._set_values(id, name, description, remote_type)
             all_column_items.append(column_item)
 
         return all_column_items
 
     @staticmethod
     def _parse_element(column_xml, ns):
-        id = column_xml.get('id', None)
-        name = column_xml.get('name', None)
-        description = column_xml.get('description', None)
-        remote_type = column_xml.get('remoteType', None)
+        id = column_xml.get("id", None)
+        name = column_xml.get("name", None)
+        description = column_xml.get("description", None)
+        remote_type = column_xml.get("remoteType", None)
 
         return id, name, description, remote_type
```

### Comparing `tableauserverclient-0.9/tableauserverclient/models/connection_item.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/models/connection_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import xml.etree.ElementTree as ET
+from defusedxml.ElementTree import fromstring
+
 from .connection_credentials import ConnectionCredentials
 
 
 class ConnectionItem(object):
     def __init__(self):
         self._datasource_id = None
         self._datasource_name = None
@@ -28,63 +29,64 @@
         return self._id
 
     @property
     def connection_type(self):
         return self._connection_type
 
     def __repr__(self):
-        return "<ConnectionItem#{_id} embed={embed_password} type={_connection_type} username={username}>"\
-            .format(**self.__dict__)
+        return "<ConnectionItem#{_id} embed={embed_password} " "type={_connection_type} username={username}>".format(
+            **self.__dict__
+        )
 
     @classmethod
     def from_response(cls, resp, ns):
         all_connection_items = list()
-        parsed_response = ET.fromstring(resp)
-        all_connection_xml = parsed_response.findall('.//t:connection', namespaces=ns)
+        parsed_response = fromstring(resp)
+        all_connection_xml = parsed_response.findall(".//t:connection", namespaces=ns)
         for connection_xml in all_connection_xml:
             connection_item = cls()
-            connection_item._id = connection_xml.get('id', None)
-            connection_item._connection_type = connection_xml.get('type', None)
-            connection_item.embed_password = string_to_bool(connection_xml.get('embedPassword', ''))
-            connection_item.server_address = connection_xml.get('serverAddress', None)
-            connection_item.server_port = connection_xml.get('serverPort', None)
-            connection_item.username = connection_xml.get('userName', None)
-            datasource_elem = connection_xml.find('.//t:datasource', namespaces=ns)
+            connection_item._id = connection_xml.get("id", None)
+            connection_item._connection_type = connection_xml.get("type", None)
+            connection_item.embed_password = string_to_bool(connection_xml.get("embedPassword", ""))
+            connection_item.server_address = connection_xml.get("serverAddress", None)
+            connection_item.server_port = connection_xml.get("serverPort", None)
+            connection_item.username = connection_xml.get("userName", None)
+            datasource_elem = connection_xml.find(".//t:datasource", namespaces=ns)
             if datasource_elem is not None:
-                connection_item._datasource_id = datasource_elem.get('id', None)
-                connection_item._datasource_name = datasource_elem.get('name', None)
+                connection_item._datasource_id = datasource_elem.get("id", None)
+                connection_item._datasource_name = datasource_elem.get("name", None)
             all_connection_items.append(connection_item)
         return all_connection_items
 
     @classmethod
     def from_xml_element(cls, parsed_response, ns):
-        '''
+        """
         <connections>
             <connection serverAddress="mysql.test.com">
                 <connectionCredentials embed="true" name="test" password="secret" />
             </connection>
             <connection serverAddress="pgsql.test.com">
                 <connectionCredentials embed="true" name="test" password="secret" />
                 </connection>
         </connections>
-        '''
+        """
         all_connection_items = list()
-        all_connection_xml = parsed_response.findall('.//t:connection', namespaces=ns)
+        all_connection_xml = parsed_response.findall(".//t:connection", namespaces=ns)
 
         for connection_xml in all_connection_xml:
             connection_item = cls()
 
-            connection_item.server_address = connection_xml.get('serverAddress', None)
-            connection_item.server_port = connection_xml.get('serverPort', None)
+            connection_item.server_address = connection_xml.get("serverAddress", None)
+            connection_item.server_port = connection_xml.get("serverPort", None)
 
-            connection_credentials = connection_xml.find('.//t:connectionCredentials', namespaces=ns)
+            connection_credentials = connection_xml.find(".//t:connectionCredentials", namespaces=ns)
 
             if connection_credentials is not None:
 
                 connection_item.connection_credentials = ConnectionCredentials.from_xml_element(connection_credentials)
 
         return all_connection_items
 
 
 # Used to convert string represented boolean to a boolean type
 def string_to_bool(s):
-    return s.lower() == 'true'
+    return s.lower() == "true"
```

### Comparing `tableauserverclient-0.9/tableauserverclient/namespace.py` & `tableauserverclient-0.9.31.post0.dev1/tableauserverclient/namespace.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from xml.etree import ElementTree as ET
 import re
 
-OLD_NAMESPACE = 'http://tableausoftware.com/api'
-NEW_NAMESPACE = 'http://tableau.com/api'
-NAMESPACE_RE = re.compile(r'\{(.*?)\}')
+from defusedxml.ElementTree import fromstring
+
+OLD_NAMESPACE = "http://tableausoftware.com/api"
+NEW_NAMESPACE = "http://tableau.com/api"
+NAMESPACE_RE = re.compile(r"\{(.*?)\}")
 
 
 class UnknownNamespaceError(Exception):
     pass
 
 
 class Namespace(object):
     def __init__(self):
-        self._namespace = {'t': NEW_NAMESPACE}
+        self._namespace = {"t": NEW_NAMESPACE}
         self._detected = False
 
     def __call__(self):
         return self._namespace
 
     def detect(self, xml):
         if self._detected:
             return
 
-        if not xml.startswith(b'<?xml'):
+        if not xml.startswith(b"<?xml"):
             return  # Not an xml file, don't detect anything
 
-        root = ET.fromstring(xml)
+        root = fromstring(xml)
         matches = NAMESPACE_RE.match(root.tag)
         if matches:
             detected_ns = matches.group(1)
             if detected_ns in (OLD_NAMESPACE, NEW_NAMESPACE):
-                self._namespace = {'t': detected_ns}
+                self._namespace = {"t": detected_ns}
                 self._detected = True
             else:
                 raise UnknownNamespaceError(detected_ns)
```

### Comparing `tableauserverclient-0.9/versioneer.py` & `tableauserverclient-0.9.31.post0.dev1/versioneer.py`

 * *Files identical despite different names*

