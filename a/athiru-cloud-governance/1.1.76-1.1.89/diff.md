# Comparing `tmp/athiru-cloud-governance-1.1.76.tar.gz` & `tmp/athiru-cloud-governance-1.1.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athiru-cloud-governance-1.1.76.tar", last modified: Sat Mar  4 04:59:11 2023, max compression
+gzip compressed data, was "athiru-cloud-governance-1.1.89.tar", last modified: Tue Apr 25 10:29:38 2023, max compression
```

## Comparing `athiru-cloud-governance-1.1.76.tar` & `athiru-cloud-governance-1.1.89.tar`

### file list

```diff
@@ -1,210 +1,216 @@
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.240935 athiru-cloud-governance-1.1.76/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11357 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/LICENSE
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      100 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/MANIFEST.in
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14830 2023-03-04 04:59:11.240935 athiru-cloud-governance-1.1.76/PKG-INFO
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14122 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/README.md
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.207934 athiru-cloud-governance-1.1.76/athiru_cloud_governance.egg-info/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14830 2023-03-04 04:59:11.000000 athiru-cloud-governance-1.1.76/athiru_cloud_governance.egg-info/PKG-INFO
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9082 2023-03-04 04:59:11.000000 athiru-cloud-governance-1.1.76/athiru_cloud_governance.egg-info/SOURCES.txt
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        1 2023-03-04 04:59:11.000000 athiru-cloud-governance-1.1.76/athiru_cloud_governance.egg-info/dependency_links.txt
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        1 2023-03-04 04:59:11.000000 athiru-cloud-governance-1.1.76/athiru_cloud_governance.egg-info/not-zip-safe
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      551 2023-03-04 04:59:11.000000 athiru-cloud-governance-1.1.76/athiru_cloud_governance.egg-info/requires.txt
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       17 2023-03-04 04:59:11.000000 athiru-cloud-governance-1.1.76/athiru_cloud_governance.egg-info/top_level.txt
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.207934 athiru-cloud-governance-1.1.76/cloud_governance/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.207934 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.208935 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/aws/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/aws/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.209935 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/aws/long_run/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/aws/long_run/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7715 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6068 2023-02-28 06:34:22.000000 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7207 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6380 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.209935 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/aws/short_run/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/aws/short_run/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       87 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/aws/short_run/ec2_short_run.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.210934 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/common/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/common/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11864 2023-02-28 06:34:22.000000 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.210934 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/monitor/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3787 2023-02-28 06:34:22.000000 athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.211935 athiru-cloud-governance-1.1.76/cloud_governance/common/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.211935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.211935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.211935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/cloudtrail/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    13290 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.212935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/cloudwatch/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2312 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.213935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/cost_explorer/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3754 2023-03-04 04:19:08.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.213935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/dynamodb/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/dynamodb/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4916 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.214935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/ec2/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/ec2/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    17861 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.214935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/iam/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/iam/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1471 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/iam/iam_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.215935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/price/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/price/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5501 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/price/price.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1599 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/price/resources_pricing.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.216935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/s3/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/s3/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11967 2023-02-14 05:18:50.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/s3/s3_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.216935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/sts/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/sts/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      376 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/sts/sts_oprations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.217935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/utils/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/utils/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1093 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/utils/utils.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.217935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/azure/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/azure/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.217935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/azure/cost_management/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/azure/cost_management/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3647 2023-02-28 06:34:22.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.218935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/azure/subscriptions/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/azure/subscriptions/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2143 2023-02-03 17:37:00.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.219935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/ibm/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/ibm/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.219935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/ibm/account/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/ibm/account/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8637 2023-01-24 06:14:19.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/ibm/account/ibm_account.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.220935 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/ibm/classic/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/ibm/classic/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3531 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/ibm/classic/classic_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.221935 athiru-cloud-governance-1.1.76/cloud_governance/common/elasticsearch/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/elasticsearch/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2523 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/elasticsearch/elastic_upload.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      484 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10430 2023-03-03 19:37:37.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/elasticsearch/elasticsearch_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.221935 athiru-cloud-governance-1.1.76/cloud_governance/common/google_drive/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/google_drive/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8244 2023-03-03 17:59:26.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/google_drive/google_drive_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9504 2023-03-03 19:40:17.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/google_drive/upload_to_gsheet.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.222935 athiru-cloud-governance-1.1.76/cloud_governance/common/jira/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/jira/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9020 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/jira/jira.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5638 2023-02-28 06:34:22.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/jira/jira_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.222935 athiru-cloud-governance-1.1.76/cloud_governance/common/ldap/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/ldap/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2400 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/ldap/ldap_search.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.223935 athiru-cloud-governance-1.1.76/cloud_governance/common/logger/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/logger/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      466 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/logger/init_logger.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1578 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/logger/logger_time_stamp.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.224935 athiru-cloud-governance-1.1.76/cloud_governance/common/mails/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/mails/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1858 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/mails/gmail.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    12254 2023-02-08 04:46:31.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/mails/mail_message.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5648 2023-02-27 16:58:51.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/mails/postfix.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.224935 athiru-cloud-governance-1.1.76/cloud_governance/common/tool/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/tool/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      248 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/common/tool/tool.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.225935 athiru-cloud-governance-1.1.76/cloud_governance/main/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/main/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    13645 2023-03-03 19:37:37.000000 athiru-cloud-governance-1.1.76/cloud_governance/main/environment_variables.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      437 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/main/environment_variables_exceptions.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10656 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/main/es_uploader.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    15327 2023-03-03 18:02:16.000000 athiru-cloud-governance-1.1.76/cloud_governance/main/main.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.225935 athiru-cloud-governance-1.1.76/cloud_governance/policy/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.229935 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7414 2023-01-24 06:14:19.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/cost_billing_reports.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6305 2023-03-03 18:02:29.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/cost_explorer.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10080 2023-03-04 04:46:53.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/cost_explorer_payer_billings.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5350 2023-03-03 18:04:44.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/cost_over_usage.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      616 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/ebs_in_use.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4452 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/ebs_unattached.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9741 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/ec2_idle.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1592 2023-02-02 07:19:23.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/ec2_run.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8141 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/ec2_stop.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2538 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/empty_roles.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3027 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/ip_unattached.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6776 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/monthly_report.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2906 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/nat_gateway_unused.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2839 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/s3_inactive.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5680 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/skipped_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    51423 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/zombie_cluster_resource.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3505 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/zombie_snapshots.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.229935 athiru-cloud-governance-1.1.76/cloud_governance/policy/azure/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/azure/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10216 2023-03-04 04:19:08.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/azure/cost_billing_reports.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.230935 athiru-cloud-governance-1.1.76/cloud_governance/policy/ibm/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/ibm/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4118 2023-03-04 04:45:54.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/ibm/cost_billing_reports.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3595 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/ibm/ibm_cost_over_usage.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5384 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/ibm/ibm_cost_report.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4997 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/ibm/tag_baremetal.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4583 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/ibm/tag_vm.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.231935 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.231935 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.231935 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/cost_expenditure/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1060 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.232935 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1900 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2534 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.233935 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_cluster/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    25600 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5115 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2627 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    41748 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.235935 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7267 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8362 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2613 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11455 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6139 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.236935 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_user/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3389 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1968 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2912 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10510 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.237935 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_cluster/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    26104 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3470 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1373 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9166 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1164 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14154 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.238935 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    16686 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1712 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.238935 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/azure/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/azure/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1129 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.239935 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/gitleaks/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/gitleaks/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3795 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.239935 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/ibm/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/ibm/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.239935 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/ibm/ibm_operations/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      625 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1123 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-03-04 04:59:11.240935 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/ibm/tagging/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2357 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       79 2023-03-04 04:59:11.240935 athiru-cloud-governance-1.1.76/setup.cfg
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2805 2023-03-04 04:57:39.000000 athiru-cloud-governance-1.1.76/setup.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.923040 athiru-cloud-governance-1.1.89/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11357 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/LICENSE
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      100 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/MANIFEST.in
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14830 2023-04-25 10:29:38.923040 athiru-cloud-governance-1.1.89/PKG-INFO
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14122 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/README.md
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.896040 athiru-cloud-governance-1.1.89/athiru_cloud_governance.egg-info/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14830 2023-04-25 10:29:38.000000 athiru-cloud-governance-1.1.89/athiru_cloud_governance.egg-info/PKG-INFO
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9283 2023-04-25 10:29:38.000000 athiru-cloud-governance-1.1.89/athiru_cloud_governance.egg-info/SOURCES.txt
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        1 2023-04-25 10:29:38.000000 athiru-cloud-governance-1.1.89/athiru_cloud_governance.egg-info/dependency_links.txt
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        1 2023-04-25 10:29:38.000000 athiru-cloud-governance-1.1.89/athiru_cloud_governance.egg-info/not-zip-safe
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      608 2023-04-25 10:29:38.000000 athiru-cloud-governance-1.1.89/athiru_cloud_governance.egg-info/requires.txt
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       17 2023-04-25 10:29:38.000000 athiru-cloud-governance-1.1.89/athiru_cloud_governance.egg-info/top_level.txt
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.896040 athiru-cloud-governance-1.1.89/cloud_governance/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.896040 athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.896040 athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.897040 athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9321 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/collect_cro_reports.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9238 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/cost_over_usage.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3473 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_cro_instances.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11021 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_tickets.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5259 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/run_cro.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6629 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/tag_cro_instances.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.897040 athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/monitor/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1439 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.897040 athiru-cloud-governance-1.1.89/cloud_governance/common/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.897040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.897040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.897040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cloudtrail/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    13290 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.897040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cloudwatch/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2312 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.898040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cost_explorer/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4589 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.898040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/dynamodb/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/dynamodb/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4916 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.898040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/ec2/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/ec2/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    19858 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.899040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/iam/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/iam/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1797 2023-04-19 05:12:45.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/iam/iam_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.899040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/price/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/price/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5501 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/price/price.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1599 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/price/resources_pricing.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.900040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/s3/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/s3/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11967 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/s3/s3_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.900040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/sts/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/sts/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      376 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/sts/sts_oprations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.901040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/utils/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/utils/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3210 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/utils/utils.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.901040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.901040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/cost_management/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/cost_management/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3647 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.902040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/subscriptions/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/subscriptions/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2143 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.902040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/gcp/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/gcp/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1746 2023-03-17 06:23:24.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/gcp/google_account.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.903040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.903040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/account/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/account/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8637 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/account/ibm_account.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.903040 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/classic/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/classic/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3531 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/classic/classic_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.904040 athiru-cloud-governance-1.1.89/cloud_governance/common/elasticsearch/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/elasticsearch/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2523 2023-04-18 07:27:25.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/elasticsearch/elastic_upload.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      484 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11528 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/elasticsearch/elasticsearch_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.905040 athiru-cloud-governance-1.1.89/cloud_governance/common/google_drive/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/google_drive/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8244 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/google_drive/google_drive_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10366 2023-03-17 06:23:24.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/google_drive/upload_to_gsheet.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.905040 athiru-cloud-governance-1.1.89/cloud_governance/common/jira/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/jira/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9020 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/jira/jira.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9134 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/jira/jira_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.906040 athiru-cloud-governance-1.1.89/cloud_governance/common/ldap/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/ldap/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2500 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/ldap/ldap_search.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.906040 athiru-cloud-governance-1.1.89/cloud_governance/common/logger/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/logger/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      466 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/logger/init_logger.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1578 2023-03-09 13:52:50.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/logger/logger_time_stamp.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.907040 athiru-cloud-governance-1.1.89/cloud_governance/common/mails/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/mails/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1858 2023-04-16 06:07:13.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/mails/gmail.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    15245 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/mails/mail_message.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6165 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/mails/postfix.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.907040 athiru-cloud-governance-1.1.89/cloud_governance/common/tool/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/tool/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      248 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/common/tool/tool.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.909040 athiru-cloud-governance-1.1.89/cloud_governance/main/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/main/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    18288 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/main/environment_variables.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      437 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/main/environment_variables_exceptions.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10656 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/main/es_uploader.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    16298 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/main/main.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      776 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/main/run_cloud_resource_orchestration.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.909040 athiru-cloud-governance-1.1.89/cloud_governance/policy/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.913040 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7428 2023-03-17 06:23:24.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/cost_billing_reports.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6305 2023-04-18 07:13:29.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/cost_explorer.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    15631 2023-03-17 06:23:24.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/cost_explorer_payer_billings.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5350 2023-03-03 18:04:44.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/cost_over_usage.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      616 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/ebs_in_use.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4452 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/ebs_unattached.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9741 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/ec2_idle.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1592 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/ec2_run.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8141 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/ec2_stop.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2538 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/empty_roles.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3027 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/ip_unattached.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6776 2023-04-18 07:27:25.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/monthly_report.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2906 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/nat_gateway_unused.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2839 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/s3_inactive.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5680 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/skipped_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    51727 2023-03-23 05:18:00.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/zombie_cluster_resource.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3505 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/zombie_snapshots.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.913040 athiru-cloud-governance-1.1.89/cloud_governance/policy/azure/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/azure/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10216 2023-03-17 06:23:24.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/azure/cost_billing_reports.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.914040 athiru-cloud-governance-1.1.89/cloud_governance/policy/gcp/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/gcp/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14218 2023-03-17 06:23:24.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/gcp/cost_billing_reports.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.915040 athiru-cloud-governance-1.1.89/cloud_governance/policy/ibm/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/ibm/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4118 2023-03-17 06:23:24.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/ibm/cost_billing_reports.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3595 2023-04-18 07:27:25.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/ibm/ibm_cost_over_usage.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5384 2023-01-13 08:45:30.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/ibm/ibm_cost_report.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4997 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/ibm/tag_baremetal.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4583 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/ibm/tag_vm.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.915040 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.916040 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.916040 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/cost_expenditure/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1060 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.916040 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1900 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2534 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.918040 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    25600 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5115 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3776 2023-04-19 05:44:11.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    41752 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.918040 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8869 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8362 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2613 2023-04-20 10:33:28.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11803 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6139 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.919040 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3389 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1968 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2912 2023-03-22 05:22:40.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10510 2023-04-18 07:27:25.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.921040 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    27642 2023-03-23 05:18:00.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3470 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1373 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9166 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1164 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14370 2023-04-18 07:27:25.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.922040 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    17153 2023-04-18 07:27:25.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1712 2023-04-25 10:01:46.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.922040 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/azure/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/azure/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1129 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.922040 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/gcp/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/gcp/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1116 2023-03-17 06:23:24.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.923040 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/gitleaks/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/gitleaks/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3795 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.923040 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.923040 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/ibm_operations/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      625 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1123 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 10:29:38.923040 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/tagging/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2357 2023-03-09 05:50:15.000000 athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       79 2023-04-25 10:29:38.924040 athiru-cloud-governance-1.1.89/setup.cfg
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2926 2023-04-25 10:29:33.000000 athiru-cloud-governance-1.1.89/setup.py
```

### Comparing `athiru-cloud-governance-1.1.76/LICENSE` & `athiru-cloud-governance-1.1.89/LICENSE`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/PKG-INFO` & `athiru-cloud-governance-1.1.89/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athiru-cloud-governance
-Version: 1.1.76
+Version: 1.1.89
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `athiru-cloud-governance-1.1.76/README.md` & `athiru-cloud-governance-1.1.89/README.md`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/athiru_cloud_governance.egg-info/PKG-INFO` & `athiru-cloud-governance-1.1.89/athiru_cloud_governance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athiru-cloud-governance
-Version: 1.1.76
+Version: 1.1.89
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `athiru-cloud-governance-1.1.76/athiru_cloud_governance.egg-info/SOURCES.txt` & `athiru-cloud-governance-1.1.89/athiru_cloud_governance.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 athiru_cloud_governance.egg-info/dependency_links.txt
 athiru_cloud_governance.egg-info/not-zip-safe
 athiru_cloud_governance.egg-info/requires.txt
 athiru_cloud_governance.egg-info/top_level.txt
 cloud_governance/__init__.py
 cloud_governance/cloud_resource_orchestration/__init__.py
 cloud_governance/cloud_resource_orchestration/aws/__init__.py
-cloud_governance/cloud_resource_orchestration/aws/long_run/__init__.py
-cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py
-cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py
-cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py
-cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py
-cloud_governance/cloud_resource_orchestration/aws/short_run/__init__.py
-cloud_governance/cloud_resource_orchestration/aws/short_run/ec2_short_run.py
-cloud_governance/cloud_resource_orchestration/common/__init__.py
-cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py
+cloud_governance/cloud_resource_orchestration/aws/ec2/__init__.py
+cloud_governance/cloud_resource_orchestration/aws/ec2/collect_cro_reports.py
+cloud_governance/cloud_resource_orchestration/aws/ec2/cost_over_usage.py
+cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_cro_instances.py
+cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_tickets.py
+cloud_governance/cloud_resource_orchestration/aws/ec2/run_cro.py
+cloud_governance/cloud_resource_orchestration/aws/ec2/tag_cro_instances.py
 cloud_governance/cloud_resource_orchestration/monitor/__init__.py
 cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
 cloud_governance/common/__init__.py
 cloud_governance/common/clouds/__init__.py
 cloud_governance/common/clouds/aws/__init__.py
 cloud_governance/common/clouds/aws/cloudtrail/__init__.py
 cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
@@ -48,14 +46,16 @@
 cloud_governance/common/clouds/aws/utils/__init__.py
 cloud_governance/common/clouds/aws/utils/utils.py
 cloud_governance/common/clouds/azure/__init__.py
 cloud_governance/common/clouds/azure/cost_management/__init__.py
 cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
 cloud_governance/common/clouds/azure/subscriptions/__init__.py
 cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
+cloud_governance/common/clouds/gcp/__init__.py
+cloud_governance/common/clouds/gcp/google_account.py
 cloud_governance/common/clouds/ibm/__init__.py
 cloud_governance/common/clouds/ibm/account/__init__.py
 cloud_governance/common/clouds/ibm/account/ibm_account.py
 cloud_governance/common/clouds/ibm/classic/__init__.py
 cloud_governance/common/clouds/ibm/classic/classic_operations.py
 cloud_governance/common/elasticsearch/__init__.py
 cloud_governance/common/elasticsearch/elastic_upload.py
@@ -79,14 +79,15 @@
 cloud_governance/common/tool/__init__.py
 cloud_governance/common/tool/tool.py
 cloud_governance/main/__init__.py
 cloud_governance/main/environment_variables.py
 cloud_governance/main/environment_variables_exceptions.py
 cloud_governance/main/es_uploader.py
 cloud_governance/main/main.py
+cloud_governance/main/run_cloud_resource_orchestration.py
 cloud_governance/policy/__init__.py
 cloud_governance/policy/aws/__init__.py
 cloud_governance/policy/aws/cost_billing_reports.py
 cloud_governance/policy/aws/cost_explorer.py
 cloud_governance/policy/aws/cost_explorer_payer_billings.py
 cloud_governance/policy/aws/cost_over_usage.py
 cloud_governance/policy/aws/ebs_in_use.py
@@ -100,14 +101,16 @@
 cloud_governance/policy/aws/nat_gateway_unused.py
 cloud_governance/policy/aws/s3_inactive.py
 cloud_governance/policy/aws/skipped_resources.py
 cloud_governance/policy/aws/zombie_cluster_resource.py
 cloud_governance/policy/aws/zombie_snapshots.py
 cloud_governance/policy/azure/__init__.py
 cloud_governance/policy/azure/cost_billing_reports.py
+cloud_governance/policy/gcp/__init__.py
+cloud_governance/policy/gcp/cost_billing_reports.py
 cloud_governance/policy/ibm/__init__.py
 cloud_governance/policy/ibm/cost_billing_reports.py
 cloud_governance/policy/ibm/ibm_cost_over_usage.py
 cloud_governance/policy/ibm/ibm_cost_report.py
 cloud_governance/policy/ibm/tag_baremetal.py
 cloud_governance/policy/ibm/tag_vm.py
 cloud_governance/policy/policy_operations/__init__.py
@@ -141,14 +144,16 @@
 cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
 cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
 cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
 cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
 cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
 cloud_governance/policy/policy_operations/azure/__init__.py
 cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
+cloud_governance/policy/policy_operations/gcp/__init__.py
+cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
 cloud_governance/policy/policy_operations/gitleaks/__init__.py
 cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
 cloud_governance/policy/policy_operations/ibm/__init__.py
 cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
 cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
 cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
 cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py` & `athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/collect_cro_reports.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,137 +1,164 @@
+from datetime import datetime, timedelta
 
-import datetime
+import typeguard
 
-
-from cloud_governance.cloud_resource_orchestration.aws.long_run.monitor_long_run import MonitorLongRun
-from cloud_governance.cloud_resource_orchestration.aws.long_run.tag_long_run import TagLongRun
-from cloud_governance.common.elasticsearch.elastic_upload import ElasticUpload
-from cloud_governance.common.logger.init_logger import logger
+from cloud_governance.cloud_resource_orchestration.aws.ec2.cost_over_usage import CostOverUsage
+from cloud_governance.cloud_resource_orchestration.aws.ec2.monitor_tickets import MonitorTickets
+from cloud_governance.common.jira.jira_operations import JiraOperations
 from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
-
-from cloud_governance.common.clouds.aws.ec2.ec2_operations import EC2Operations
 from cloud_governance.main.environment_variables import environment_variables
 
 
-class EC2LongRun:
+class CollectCROReports:
     """
-    This class tag & monitor the LongRun EC2 instances.
-    User Steps:
-    1. Create a Jira Issue in Clouds portal, store the JiraId
-    2. Create the EC2 instance, tag JiraId
-    CI Steps:
-    1. CI Look the instances which are tagged with JiraId
-    2. Checks the JiraId had manager approval in the data
-    3. If manger approval, append LongRun tags ( Project, LongRunDays, ApprovedManager )
+    This method collects the user/instance-id data from the cost-explorer
     """
 
-    def __init__(self, region_name: str = ''):
+    DEFAULT_ROUND_DIGITS = 3
+    ZERO = 0
+
+    def __init__(self):
         self.__environment_variables_dict = environment_variables.environment_variables_dict
-        self.__region_name = region_name if region_name else self.__environment_variables_dict.get('AWS_DEFAULT_REGION')
-        self.__tag_long_run = TagLongRun(region_name=region_name)
-        self.__monitor_long_run = MonitorLongRun(region_name=region_name)
-        self.__ec2_operations = EC2Operations()
-        self.__es_upload = ElasticUpload()
-        self.__es_index = self.__environment_variables_dict.get('es_index')
-        self.__account = self.__environment_variables_dict.get('account')
-        self.__jira_queue = self.__environment_variables_dict.get('JIRA_QUEUE')
-
-    def update_es_data(self, cost_estimation: float, instances: list, jira_id: str):
-        """This method update the es_data"""
-        es_data = self.__es_upload.elastic_search_operations.get_es_data_by_id(id=jira_id, index=self.__es_index)
-        source = es_data.get('_source')
-        instance_ids = source.get('instance_ids', [])
-        update_es_data = {'cost_estimation': cost_estimation,
-                          'long_run_days': int(instances[0].get('long_run_days')),
-                          'total_instances': len(instances)}
-        running_days = 0
-        total_price = 0
-        for instance in instances:
-            running_days = max(running_days, instance.get('instance_running_days'))
-            total_price += instance.get('total_run_price')
-            instance_id = instance.get('instance_id')
-            instance_ids.append(instance_id)
-            source_instance_id = source.get(instance_id)
-            update_es_data[instance_id] = \
-                {'total_run_price': round(source_instance_id.get('total_run_price') + instance.get('total_run_price'),
-                                         3)}
-            update_es_data[instance_id].update({'total_run_hours': round(
-                source_instance_id.get('total_run_hours') + instance.get('total_run_hours'), 3)})
-            update_es_data[instance_id].update({'last_saved_time': instance.get('last_saved_time')})
-            update_es_data[instance_id].update({'instance_state': instance.get('instance_state')})
-            update_es_data[instance_id].update({'instance_running_days': instance.get('instance_running_days')})
-            update_es_data[instance_id].update(
-                {'ebs_cost': round(float(instance.get('ebs_cost') + source_instance_id.get('ebs_cost')), 3)})
-        update_es_data['running_days'] = running_days
-        update_es_data['total_run_price'] = float(source.get('total_run_price')) + total_price
-        update_es_data['remaining_days'] = int(update_es_data.get('long_run_days')) - running_days
-        update_es_data['timestamp'] = datetime.datetime.utcnow()
-        update_es_data['instance_ids'] = list(set(instance_ids))
-        self.__es_upload.elastic_search_operations.update_elasticsearch_index(index=self.__es_index, id=jira_id,
-                                                                              metadata=update_es_data)
-        logger.info(f'Updated the jira-id: {jira_id} data : {update_es_data}')
-
-    def upload_new_es_data(self, jira_id: str, instances: list, cost_estimation: float):
-        """This method upload the new es_data"""
-        es_data = {'jira_id': jira_id, 'cloud_name': 'aws', 'account_name': self.__account,
-                   'user': instances[0].get('user'), 'long_run_days': instances[0].get('long_run_days'),
-                   'owner': instances[0].get('owner'), 'approved_manager': instances[0].get('approved_manager'),
-                   'user_manager': instances[0].get('manager'), 'region_name': self.__region_name,
-                   'project': instances[0].get('project'), 'cost_estimation': cost_estimation,
-                   'jira_id_state': 'in-progress',
-                   'total_instances': len(instances)}
-        running_days = 0
-        total_price = 0
-        for instance in instances:
-            running_days = max(running_days, instance.get('instance_running_days'))
-            total_price += instance.get('total_run_price')
-            es_data.setdefault('instance_ids', []).append(instance.get('instance_id'))
-            instance.pop('user')
-            instance.pop('long_run_days')
-            instance.pop('owner')
-            instance.pop('approved_manager')
-            instance.pop('project')
-            instance.pop('manager')
-            es_data[instance.get('instance_id')] = instance
-        es_data['running_days'] = running_days
-        es_data['remaining_days'] = int(es_data.get('long_run_days')) - running_days
-        es_data['total_run_price'] = round(total_price, 3)
-        es_data['timestamp'] = datetime.datetime.utcnow()
-        self.__es_upload.es_upload_data(items=[es_data], es_index=self.__es_index, set_index='jira_id')
-        logger.info(f'Uploaded data to the es index {self.__es_index}')
+        self.__account_name = self.__environment_variables_dict.get('account', '').replace('OPENSHIFT-', '').strip()
+        self.__cost_over_usage = CostOverUsage()
+        self.jira_operations = JiraOperations()
+        self.__public_cloud_name = self.__environment_variables_dict.get('PUBLIC_CLOUD_NAME', '')
+        self.__es_index_cro = self.__environment_variables_dict.get('CRO_ES_INDEX', '')
+        self.__monitor_ticket = MonitorTickets()
 
+    @typeguard.typechecked
     @logger_time_stamp
-    def prepare_to_upload_es(self, upload_data: dict):
+    def get_user_cost_data(self, user: str, requested_date: datetime, user_project: str = ''):
         """
-        This method beautify and upload data to ES
+        This method fetch data from the es_reports
+        :param user_project:
+        :param user:
+        :param requested_date:
+        :return:
+        """
+        jira_created_date = requested_date.replace(minute=self.ZERO, hour=self.ZERO, second=self.ZERO, microsecond=self.ZERO)
+        response = self.__cost_over_usage.get_monthly_user_es_cost_data(start_date=jira_created_date,
+                                                                        end_date=datetime.utcnow().replace(microsecond=self.ZERO) + timedelta(days=1),
+                                                                        extra_matches=[{'Tags': {'Key': 'User', 'Values': [user]}}, {'Tags': {'Key': 'Project', 'Values': [user_project]}}], extra_operation='And', tag_name='User')
+        if response:
+            return round(response[self.ZERO].get('Cost'), self.DEFAULT_ROUND_DIGITS)
+        return self.ZERO
+
+    @typeguard.typechecked
+    @logger_time_stamp
+    def prepare_instance_data(self, instance_data: list, user: str, ticket_id: str, user_cost: float,
+                              cost_estimation: float, ticket_opened_date: datetime):
         """
-        for jira_id, instances in upload_data.items():
-            issue_description = self.__tag_long_run.jira_operations.get_issue_description(jira_id=jira_id, state='any')
-            cost_estimation = float(issue_description.get('CostEstimation', 0))
-            cost_estimation += float(
-                self.__tag_long_run.jira_operations.get_issue_sub_tasks_cost_estimation(jira_id=jira_id))
-            if self.__jira_queue not in jira_id:
-                jira_id = f"{self.__jira_queue}-{jira_id}"
-            if self.__es_upload.elastic_search_operations.verify_elastic_index_doc_id(index=self.__es_index,
-                                                                                      doc_id=jira_id):
-                self.update_es_data(cost_estimation=cost_estimation, instances=instances, jira_id=jira_id)
-            else:
-                self.upload_new_es_data(cost_estimation=cost_estimation, instances=instances, jira_id=jira_id)
+        This method returns es data to upload
+        :param instance_data:
+        :param user:
+        :param ticket_id:
+        :param user_cost:
+        :param cost_estimation:
+        :param ticket_opened_date:
+        :return: dict data
+        """
+        return {
+            'cloud_name': self.__public_cloud_name.upper(),
+            'account_name': self.__account_name,
+            'region_name': instance_data[self.ZERO].get('region_name'),
+            'user': user,
+            'user_cro': instance_data[self.ZERO].get('user_cro'),
+            'actual_cost': user_cost,
+            'ticket_id': ticket_id,
+            'ticket_id_state': 'in-progress',
+            'estimated_cost': cost_estimation,
+            'total_instances': len(instance_data),
+            'monitored_days': (datetime.utcnow().date() - ticket_opened_date.date()).days,
+            'ticket_opened_date': ticket_opened_date.date(),
+            'duration': int(instance_data[self.ZERO].get('duration')),
+            'approved_manager': instance_data[self.ZERO].get('approved_manager'),
+            'user_manager': instance_data[self.ZERO].get('manager'),
+            'project': instance_data[self.ZERO].get('project'),
+            'owner': instance_data[self.ZERO].get('owner'),
+            'total_spots': len([instance for instance in instance_data if instance.get('instance_plan').lower() == 'spot']),
+            'total_ondemand': len([instance for instance in instance_data if instance.get('instance_plan').lower() == 'ondemand']),
+            'instances': [f"{instance.get('instance_name')}, {instance.get('instance_id')}, "
+                          f"{instance.get('instance_plan')}, "
+                          f"{instance.get('instance_type')}, "
+                          f"{instance.get('instance_state')}, {instance.get('instance_running_days')}" for instance in instance_data]
+        }
 
-    def __long_run(self):
+    @typeguard.typechecked
+    @logger_time_stamp
+    def __prepare_update_es_data(self, source: dict, instance_data: list, user_cost: float, cost_estimation: float):
         """
-        This method start the long run process
-        1. tag the instances which have tag JiraId
-        2. Monitor the long_run instances based on LongRunDays
+        This method update the values of jira id data
+        :param source:
+        :param instance_data:
+        :param user_cost:
+        :param cost_estimation:
+        :return: dict data
+        """
+        for instance in instance_data:
+            index = [idx for idx, es_instance in enumerate(source.get('instances')) if instance.get('instance_id') in es_instance]
+            running_days = instance.get('instance_running_days')
+            if index:
+                source['instances'][index[self.ZERO]] = f"{instance.get('instance_name')}, {instance.get('instance_id')}, " \
+                                                f"{instance.get('instance_plan')}, {instance.get('instance_type')}, " \
+                                                f"{instance.get('instance_state')}, {running_days}"
+            else:
+                source['instances'].append(f"{instance.get('instance_name')}, {instance.get('instance_id')}, "
+                                           f"{instance.get('instance_plan')}, {instance.get('instance_type')}, "
+                                           f"{instance.get('instance_state')}, {running_days}")
+                if instance.get('instance_plan').lower() == 'spot':
+                    source['total_spots'] = source.get('total_spots') + 1
+                else:
+                    if instance.get('instance_plan').lower() == 'ondemand':
+                        source['total_ondemand'] = source.get('total_ondemand') + 1
+        self.__monitor_ticket.verify_es_instances_state(es_data=source)
+        if datetime.strptime(source.get('timestamp'), "%Y-%m-%dT%H:%M:%S.%f").date() != datetime.now().date():
+            source['monitored_days'] = (datetime.utcnow().date() - source.get('ticket_opened_date')).days
+        source['total_instances'] = len(source.get('instances', self.ZERO))
+        source['duration'] = int(instance_data[self.ZERO].get('duration'))
+        source['estimated_cost'] = round(cost_estimation, self.DEFAULT_ROUND_DIGITS)
+        source['actual_cost'] = user_cost
+        if instance_data[self.ZERO].get('user_cro') and source.get('user_cro') != instance_data[self.ZERO].get('user_cro'):
+            source['user_cro'] = instance_data[self.ZERO].get('user_cro')
+        source['timestamp'] = datetime.utcnow()
+        return source
+
+    @typeguard.typechecked
+    @logger_time_stamp
+    def __upload_cro_report_to_es(self, monitor_data: dict):
         """
-        tag_response = self.__tag_long_run.run()
-        if tag_response:
-            logger.info(f'Tags are added to the JiraId tag instances: {tag_response}')
-        monitor_response = self.__monitor_long_run.run()
-        if monitor_response:
-            self.prepare_to_upload_es(monitor_response)
+        This method uploads the data to elastic search index and return the data
+        :param monitor_data:
+        :return:
+        """
+        upload_data = {}
+        for ticket_id, instance_data in monitor_data.items():
+            user = instance_data[self.ZERO].get('user')
+            user_project = instance_data[self.ZERO].get('project')
+            issue_description = self.jira_operations.get_issue_description(ticket_id=ticket_id, state='ANY')
+            ticket_opened_date = issue_description.get('TicketOpenedDate')
+            user_cost = self.get_user_cost_data(user, requested_date=ticket_opened_date, user_project=user_project)
+            cost_estimation = float(instance_data[self.ZERO].get('estimated_cost', self.ZERO))
+            if self.__cost_over_usage.es_operations.verify_elastic_index_doc_id(index=self.__cost_over_usage.es_index_cro, doc_id=ticket_id):
+                es_data = self.__cost_over_usage.es_operations.get_es_data_by_id(id=ticket_id, index=self.__cost_over_usage.es_index_cro)
+                es_data['_source']['ticket_opened_date'] = ticket_opened_date.date()
+                source = self.__prepare_update_es_data(source=es_data.get('_source'), instance_data=instance_data, cost_estimation=cost_estimation, user_cost=user_cost)
+                self.__cost_over_usage.es_operations.update_elasticsearch_index(index=self.__es_index_cro, id=ticket_id, metadata=source)
+                upload_data[ticket_id] = source
+            else:
+                if ticket_id not in upload_data:
+                    source = self.prepare_instance_data(instance_data=instance_data, ticket_id=ticket_id, cost_estimation=cost_estimation, user=user,  user_cost=user_cost, ticket_opened_date=ticket_opened_date)
+                    source['ticket_opened_date'] = ticket_opened_date.date()
+                    self.__cost_over_usage.es_operations.upload_to_elasticsearch(index=self.__es_index_cro, data=source, id=ticket_id)
+                    upload_data[ticket_id] = source
+        return upload_data
 
-    def run(self):
+    @typeguard.typechecked
+    @logger_time_stamp
+    def run(self, monitor_data: dict):
         """
-        This method run the long run methods
+        This method run data collection methods
+        :param monitor_data:
+        :return:
         """
-        self.__long_run()
+        return self.__upload_cro_report_to_es(monitor_data=monitor_data)
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py` & `athiru-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/tag_cro_instances.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,117 +1,130 @@
+import boto3
+import typeguard
 
-from cloud_governance.cloud_resource_orchestration.aws.long_run.monitor_in_progress_issues import MonitorInProgressIssues
-from cloud_governance.cloud_resource_orchestration.aws.long_run.tag_long_run import TagLongRun
-from cloud_governance.cloud_resource_orchestration.common.ec2_monitor_operations import EC2MonitorOperations
-from cloud_governance.common.elasticsearch.elastic_upload import ElasticUpload
-from cloud_governance.common.jira.jira import logger
+from cloud_governance.common.clouds.aws.ec2.ec2_operations import EC2Operations
 from cloud_governance.common.jira.jira_operations import JiraOperations
 from cloud_governance.common.ldap.ldap_search import LdapSearch
-from cloud_governance.common.mails.mail_message import MailMessage
-from cloud_governance.common.mails.postfix import Postfix
+from cloud_governance.common.logger.init_logger import logger
+from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
 from cloud_governance.main.environment_variables import environment_variables
 
-from cloud_governance.common.clouds.aws.ec2.ec2_operations import EC2Operations
-
 
-class MonitorLongRun:
-    """This class monitors the long run instances and returns the data"""
-
-    FIRST_ALERT: int = 5
-    SECOND_ALERT: int = 3
-    DEFAULT_ADMINS = ['athiruma@redhat.com', 'ebattat@redhat.com', 'natashba@redhat.com']
-    HOURS_IN_SECONDS = 3600
-    JIRA_ID = 'JiraId'
+class TagCROInstances:
+    """
+    This class manages the tagging instances which have the tag TicketId
+    """
+    KEY = 'Key'
+    VALUE = 'Value'
+    NA_USER = 'NA'
+    EMPTY_USER = ''
 
     def __init__(self, region_name: str = ''):
         self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.__region_name = region_name if region_name else self.__environment_variables_dict.get('AWS_DEFAULT_REGION')
+        self.__cro_resource_tag_name = self.__environment_variables_dict.get('CRO_RESOURCE_TAG_NAME')
+        self.__ec2_client = boto3.client('ec2', region_name=self.__region_name)
         self.__ec2_operations = EC2Operations(region=self.__region_name)
-        self.__ldap_search = LdapSearch(ldap_host_name=self.__environment_variables_dict.get('LDAP_HOST_NAME'))
-        self.__tag_long_run = TagLongRun(region_name=self.__region_name)
         self.jira_operations = JiraOperations()
-        self.__es_upload = ElasticUpload()
-        self.__es_index = self.__environment_variables_dict.get('es_index')
-        self.__mail_message = MailMessage()
-        self.__postfix = Postfix()
-        self.__ec2_monitor_operations = EC2MonitorOperations(region_name=self.__region_name)
-        self.monitor_in_progress = MonitorInProgressIssues(region_name=self.__region_name)
-        self.__jira_queue = self.__environment_variables_dict.get('JIRA_QUEUE')
-
-    def __alert_instance_user(self, issues_data: dict):
-        """
-        This method alert the instance user, if the LongRunDays are running out
-        """
-        for jira_id, instances in issues_data.items():
-            if self.__jira_queue not in jira_id:
-                jira_id = f'{self.__jira_queue}-{jira_id}'
-            long_run_days = int(instances[0].get('long_run_days'))
-            approved_manager = instances[0].get('approved_manager')
-            user = instances[0].get('user')
-            running_days = 0
-            for instance in instances:
-                running_days = max(running_days, instance.get('instance_running_days'))
-            cc = self.DEFAULT_ADMINS
-            if approved_manager:
-                cc.append(approved_manager)
-            user_details = self.__ldap_search.get_user_details(user_name=user)
-            if user_details:
-                cc.append(f'{user_details.get("managerId")}@redhat.com')
-            if running_days >= long_run_days - self.FIRST_ALERT:
-                sub_tasks = self.jira_operations.get_jira_id_sub_tasks(jira_id=jira_id)
-                if sub_tasks:
-                    self.__tag_long_run.tag_extend_instances(sub_tasks=sub_tasks, jira_id=jira_id)
-            subject, body = '', ''
-            if running_days == long_run_days - self.FIRST_ALERT:
-                subject, body = self.__mail_message.get_long_run_alert(user=user, days=self.FIRST_ALERT, jira_id=jira_id)
-            elif running_days == long_run_days - self.SECOND_ALERT:
-                subject, body = self.__mail_message.get_long_run_alert(user=user, days=self.FIRST_ALERT, jira_id=jira_id)
-            else:
-                if running_days >= long_run_days:
-                    subject, body = self.__mail_message.get_long_run_expire_alert(user=user, jira_id=jira_id)
-            if subject and body:
-                self.__postfix.send_email_postfix(subject=subject, to=user, cc=cc, content=body, mime_type='html')
-
-    def monitor_instances(self):
-        """
-        This method monitoring the LongRun instances which have tag LongRunDays
-        """
-        jira_id_alerts = {}
-        long_run_instances = self.__ec2_monitor_operations.get_instances_by_filtering(tag_key_name='LongRunDays')
-        for instance in long_run_instances:
-            for resource in instance['Instances']:
-                instance_id, instance_type, tags, launch_datetime, instance_state = resource.get('InstanceId'), resource.get('InstanceType'), resource.get('Tags'), resource.get('LaunchTime'), resource.get('State')['Name']
-                jira_id = self.__ec2_operations.get_tag_value_from_tags(tag_name=self.JIRA_ID, tags=tags)
-                run_hours, last_saved_time = self.__ec2_monitor_operations.get_instance_run_hours(instance=resource, jira_id=jira_id)
-                price = self.__ec2_monitor_operations.get_instance_hours_price(instance_type=instance_type, run_hours=run_hours)
-                create_time = self.__ec2_monitor_operations.get_attached_time(volume_list=resource.get('BlockDeviceMappings'))
-                ebs_cost = self.__ec2_monitor_operations.get_volumes_cost(resource.get('BlockDeviceMappings'))
-                running_days = self.__ec2_monitor_operations.calculate_days(launch_date=launch_datetime)
-                jira_id_alerts.setdefault(jira_id, []).append({
-                    'instance_id': instance_id,
-                    'total_run_hours': run_hours,
-                    'total_run_price': price,
-                    'instance_create_time': create_time,
-                    'instance_state': instance_state,
-                    'instance_type': instance_type,
-                    'last_saved_time': last_saved_time,
-                    'jira_id': jira_id,
-                    'user': self.__ec2_operations.get_tag_value_from_tags(tag_name='User', tags=tags),
-                    'manager': self.__ec2_operations.get_tag_value_from_tags(tag_name='Manager', tags=tags),
-                    'approved_manager': self.__ec2_operations.get_tag_value_from_tags(tag_name='ApprovedManager', tags=tags),
-                    'long_run_days': self.__ec2_operations.get_tag_value_from_tags(tag_name='LongRunDays', tags=tags),
-                    'instance_running_days': running_days,
-                    'owner': self.__ec2_operations.get_tag_value_from_tags(tag_name='Owner', tags=tags),
-                    'project': self.__ec2_operations.get_tag_value_from_tags(tag_name='Project', tags=tags),
-                    'instance_name': self.__ec2_operations.get_tag_value_from_tags(tag_name='Name', tags=tags),
-                    'ebs_cost': ebs_cost
-                })
-        self.__alert_instance_user(issues_data=jira_id_alerts)
-        return jira_id_alerts
+        self.__ldap_search = LdapSearch(ldap_host_name=self.__environment_variables_dict.get('LDAP_HOST_NAME', ''))
+        self.__replace_user_names = self.__environment_variables_dict.get('CRO_REPLACED_USERNAMES')
+
+    @typeguard.typechecked
+    @logger_time_stamp
+    def __get_instance_volumes(self, block_device_mappings: list):
+        """
+        This method returns the instance volumes
+        :param block_device_mappings:
+        :return:
+        """
+        volumes_list = []
+        for mapping in block_device_mappings:
+            if mapping.get('Ebs').get('VolumeId'):
+                volumes_list.append(mapping.get('Ebs').get('VolumeId'))
+        return volumes_list
+
+    @typeguard.typechecked
+    @logger_time_stamp
+    def __get_ldap_user_data(self, user: str, tag_name: str):
+        """
+        This method returns the ldap user tag_name
+        :param user:
+        :param tag_name:
+        :return:
+        """
+        user_details = self.__ldap_search.get_user_details(user)
+        if user_details:
+            return user_details.get(tag_name)
+        return self.NA_USER
+
+    @logger_time_stamp
+    def __tag_ticket_id_attach_instance(self, ticket_id: str, instance_id: str, volume_ids: list):
+        """
+        This method tag the instances which have the tag TicketId
+        :param ticket_id:
+        :param instance_id:
+        :param volume_ids:
+        :return:
+        """
+        ticket_description = self.jira_operations.get_issue_description(ticket_id=ticket_id, state='INPROGRESS')
+        if ticket_description:
+            duration = ticket_description.get('Days')
+            estimated_cost = ticket_description.get('CostEstimation')
+            manager_approved = ticket_description.get('ApprovedManager')
+            if not manager_approved:
+                manager_approved = ticket_description.get('ManagerApprovalAddress')
+            user_email = ticket_description.get('EmailAddress')
+            user = user_email.split('@')[0]
+            project = ticket_description.get('Project')
+            tags = [{self.KEY: 'Duration', self.VALUE: duration},
+                    {self.KEY: 'EstimatedCost', self.VALUE: estimated_cost},
+                    {self.KEY: 'ApprovedManager', self.VALUE: manager_approved},
+                    {self.KEY: 'Project', self.VALUE: project.upper()},
+                    {self.KEY: 'Email', self.VALUE: user_email},
+                    {self.KEY: self.__cro_resource_tag_name, self.VALUE: ticket_id},
+                    {self.KEY: 'UserCRO', self.VALUE: user},
+                    {self.KEY: 'Manager', self.VALUE: self.__get_ldap_user_data(user, "ManagerName").upper()},
+                    {self.KEY: 'Owner', self.VALUE: self.__get_ldap_user_data(user, "FullName").upper()}]
+            self.__ec2_operations.tag_ec2_resources(client_method=self.__ec2_client.create_tags, resource_ids=[instance_id], tags=tags)
+            self.jira_operations.move_issue_state(ticket_id=ticket_id, state='inprogress')
+            logger.info(f'Extra tags are added to the instances: {instance_id}, had an ticket_id: {ticket_id}')
+            if volume_ids:
+                self.__ec2_operations.tag_ec2_resources(client_method=self.__ec2_client.create_tags, resource_ids=volume_ids, tags=tags)
+                logger.info(f'Tagged the instance: {instance_id} attached volumes {volume_ids}')
+            return True
+        return False
+
+    @logger_time_stamp
+    def __tag_instances(self):
+        """
+        This method list the instances and tag the instances which have the tag TicketId
+        :return:
+        """
+        ticket_id_instances = {}
+        instances = self.__ec2_operations.get_ec2_instance_list()
+        for resource in instances:
+            instance_id = resource.get('InstanceId')
+            ticket_id = self.__ec2_operations.get_tag_value_from_tags(tags=resource.get('Tags'), tag_name=self.__cro_resource_tag_name) if resource.get('Tags') else None
+            if ticket_id:
+                duration = self.__ec2_operations.get_tag_value_from_tags(tags=resource.get('Tags'), tag_name='Duration')
+                if not duration:
+                    volume_ids = self.__get_instance_volumes(resource.get('BlockDeviceMappings'))
+                    if self.__tag_ticket_id_attach_instance(ticket_id=ticket_id, instance_id=instance_id, volume_ids=volume_ids):
+                        ticket_id_instances.setdefault(ticket_id, []).append(instance_id)
+                user = self.__ec2_operations.get_tag_value_from_tags(tags=resource.get('Tags'), tag_name='User')
+                tag_user = False
+                if user in [*self.__replace_user_names, self.NA_USER, self.EMPTY_USER]:
+                    tag_user = True
+                if tag_user:
+                    user_cro = self.__ec2_operations.get_tag_value_from_tags(tags=resource.get('Tags'), tag_name='UserCRO')
+                    if user_cro:
+                        volume_ids = self.__get_instance_volumes(resource.get('BlockDeviceMappings'))
+                        self.__ec2_operations.tag_ec2_resources(client_method=self.__ec2_client.create_tags, resource_ids=[instance_id, *volume_ids], tags=[{self.KEY: 'User', self.VALUE: user_cro}])
+        return ticket_id_instances
 
+    @logger_time_stamp
     def run(self):
         """
-        This method run the long run monitoring methods
+        This method run the tag instance methods
+        :return:
         """
-        response = self.monitor_in_progress.monitor_progress_issues()
-        logger.info(f"Closed JiraId's: {response}")
-        return self.monitor_instances()
+        return self.__tag_instances()
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,34 +11,53 @@
     START_DAY = 1
     END_DAY = 31
     PURCHASE_OPTIONS = ['On Demand Instances', 'Savings Plans', 'Spot Instances', 'Standard Reserved Instances']
 
     def __init__(self, ce_client=''):
         self.cost_explorer_client = boto3.client('ce') if not ce_client else ce_client
 
+    def get_filter_data(self, ce_data: list, tag_name: str = ''):
+        """
+        This method filter the cost_explorer_data
+        :param tag_name:
+        :param ce_data:
+        :return:
+        """
+        user_cost_response = {}
+        for data in ce_data:
+            for cost_group in data.get('Groups'):
+                user = cost_group.get('Keys')[0].split('$')[-1]
+                user = user if user else 'REFUND'
+                user_cost = float(cost_group.get('Metrics').get('UnblendedCost').get('Amount'))
+                if user in user_cost_response:
+                    user_cost_response[user]['Cost'] += user_cost
+                else:
+                    user_cost_response[user] = {tag_name: user, 'Cost': user_cost}
+        return list(user_cost_response.values())
+
     def get_cost_by_tags(self, tag: str, granularity: str = 'DAILY', cost_metric: str = 'UnblendedCost',
-                         start_date: str = '', end_date: str = ''):
+                         start_date: str = '', end_date: str = '', **kwargs):
         """
         This method extracts the price by Tag provided
         @return:
         """
         if not start_date and not end_date:
             end_date = datetime.now() + timedelta(self.START_DAY)
             start_date = end_date - timedelta(self.END_DAY)
             start_date = str(start_date.strftime('%Y-%m-%d'))
             end_date = str(end_date.strftime('%Y-%m-%d'))
         if tag.upper() == 'ChargeType'.upper():
             return self.get_cost_and_usage_from_aws(start_date=start_date, end_date=end_date, granularity=granularity,
-                                                    GroupBy=[{'Type': 'DIMENSION', 'Key': 'RECORD_TYPE'}])
+                                                    GroupBy=[{'Type': 'DIMENSION', 'Key': 'RECORD_TYPE'}], **kwargs)
         elif tag.upper() == 'PURCHASETYPE':
             return self.get_cost_and_usage_from_aws(start_date=start_date, end_date=end_date, granularity=granularity,
-                                                    GroupBy=[{'Type': 'DIMENSION', 'Key': 'PURCHASE_TYPE'}])
+                                                    GroupBy=[{'Type': 'DIMENSION', 'Key': 'PURCHASE_TYPE'}], **kwargs)
         else:
             return self.get_cost_and_usage_from_aws(start_date=start_date, end_date=end_date, granularity=granularity,
-                                                    cost_metric=cost_metric, GroupBy=[{'Type': 'TAG', 'Key': tag}])
+                                                    cost_metric=cost_metric, GroupBy=[{'Type': 'TAG', 'Key': tag}], **kwargs)
 
     def get_cost_and_usage_from_aws(self, start_date: str, end_date: str, granularity: str = 'DAILY',
                                     cost_metric: str = 'UnblendedCost', **kwargs):
         """
         This method returns the cost and usage reports
         @param start_date:
         @param end_date:
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/ec2/ec2_operations.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/ec2/ec2_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import os
 
 import boto3
 import typeguard
+from typing import Callable
 
 from cloud_governance.common.clouds.aws.utils.utils import Utils
 from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
 from cloud_governance.main.environment_variables import environment_variables
 
 
 class EC2Operations:
     """
     This class is useful for writing EC2 Operations
     """
 
+    TAG_BATCHES = 20
+
     def __init__(self, region: str = 'us-east-2'):
         """
         Initializing the AWS resources
         """
         self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.elb1_client = boto3.client('elb', region_name=region)
         self.elbv2_client = boto3.client('elbv2', region_name=region)
@@ -501,18 +504,73 @@
                 user = self.get_tag(name='User', tags=instance.get('Tags'))
                 if user in users_list:
                     users_list[user].append(user_data)
                 else:
                     users_list[user] = [user_data]
         return users_list
 
-    def get_tag_value_from_tags(self, tags: list, tag_name: str) -> str:
+    def get_tag_value_from_tags(self, tags: list, tag_name: str, cast_type: str = 'str') -> any:
         """
         This method return the tag value inputted by tag_name
         """
         if tags:
             for tag in tags:
-                key = tag.get('Key').lower().replace("_", '').replace("-", '')
+                key = tag.get('Key').lower().replace("_", '').replace("-", '').strip()
                 if key == tag_name.lower():
-                    return tag.get('Value')
+                    if cast_type:
+                        if cast_type == 'int':
+                            return int(tag.get('Value').strip())
+                        elif cast_type == 'float':
+                            return float(tag.get('Value').strip())
+                        return str(tag.get('Value').strip())
         return ''
 
+    def get_ec2_instance_list(self, **kwargs):
+        """
+        This method returns the list of instances
+        :param kwargs:
+        :return:
+        """
+        instances_list = []
+        instances = self.get_instances(**kwargs)
+        for instance in instances:
+            for resource in instance['Instances']:
+                instances_list.append(resource)
+        return instances_list
+
+    def get_ec2_instance_ids(self, **kwargs):
+        """
+        This method return the ec2 instance ids
+        :param kwargs:
+        :return:
+        """
+        instances = self.get_ec2_instance_list(**kwargs)
+        instance_ids = []
+        for instance in instances:
+            instance_ids.append(instance.get('InstanceId'))
+        return instance_ids
+
+    def tag_ec2_resources(self, client_method: Callable, tags: list, resource_ids: list):
+        """
+        This method tag the ec2 resources with batch wise of 10
+        :param client_method:
+        :param tags:
+        :param resource_ids:
+        :return:
+        """
+        co = 0
+        for start in range(0, len(resource_ids), self.TAG_BATCHES):
+            end = start + self.TAG_BATCHES
+            client_method(Resources=resource_ids[start:end], Tags=tags)
+            co += 1
+        return co
+
+    def get_attached_time(self, volume_list: list):
+        """
+        This method return the root volume attached time
+        :param volume_list:
+        :return:
+        """
+        for mapping in volume_list:
+            if mapping.get('Ebs').get('DeleteOnTermination'):
+                return mapping.get('Ebs').get('AttachTime')
+        return ''
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/iam/iam_operations.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/iam/iam_operations.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,11 +41,24 @@
         return self.utils.get_details_resource_list(self.iam_client.list_users, input_tag='Users', check_tag='Marker')
 
     def get_account_alias_cloud_name(self):
         """
         This method returns the aws account alias and cloud name
         @return:
         """
-        account_alias = self.iam_client.list_account_aliases()['AccountAliases']
-        if account_alias:
-            return account_alias[0].upper(), 'AwsCloud'.upper()
-        return os.environ.get('account', '').upper(), 'AwsCloud'.upper()
+        try:
+            account_alias = self.iam_client.list_account_aliases()['AccountAliases']
+            if account_alias:
+                return account_alias[0].upper(), 'AwsCloud'.upper()
+        except:
+            return os.environ.get('account', '').upper(), 'AwsCloud'.upper()
+
+    def get_iam_users_list(self):
+        """
+        This method return the IAM users list
+        :return:
+        """
+        iam_users = []
+        users = self.get_users()
+        for user in users:
+            iam_users.append(user.get('UserName'))
+        return iam_users
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/price/price.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/price/price.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/price/resources_pricing.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/price/resources_pricing.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/aws/s3/s3_operations.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/s3/s3_operations.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/ibm/account/ibm_account.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/account/ibm_account.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/clouds/ibm/classic/classic_operations.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/classic/classic_operations.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/elasticsearch/elastic_upload.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/elasticsearch/elastic_upload.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/elasticsearch/elasticsearch_operations.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/elasticsearch/elasticsearch_operations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from datetime import datetime, timedelta
 import time
 import pandas as pd
 from cloud_governance.main.environment_variables import environment_variables
 
 from elasticsearch_dsl import Search
 from elasticsearch import Elasticsearch
@@ -27,16 +26,19 @@
 
     def __init__(self, es_host: str, es_port: str, region: str = '', bucket: str = '', logs_bucket_key: str = '',
                  timeout: int = 2000):
         self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.__es_host = es_host
         self.__es_port = es_port
         self.__region = region
-        self.__timeout = int(self.__environment_variables_dict.get('ES_TIMEOUT')) if self.__environment_variables_dict.get('ES_TIMEOUT') else timeout
-        self.__es = Elasticsearch([{'host': self.__es_host, 'port': self.__es_port}], timeout=self.__timeout, max_retries=2)
+        self.__timeout = int(
+            self.__environment_variables_dict.get('ES_TIMEOUT')) if self.__environment_variables_dict.get(
+            'ES_TIMEOUT') else timeout
+        self.__es = Elasticsearch([{'host': self.__es_host, 'port': self.__es_port}], timeout=self.__timeout,
+                                  max_retries=2)
 
     def __elasticsearch_get_index_hits(self, index: str, uuid: str = '', workload: str = '', fast_check: bool = False,
                                        id: bool = False):
         """
         This method search for data per index in last 2 minutes and return the number of docs or zero
         :param index:
         :param workload: need only if there is different timestamp parameter in Elasticsearch
@@ -107,15 +109,16 @@
                                                            fast_check=fast_check)
             # sleep for x seconds
             time.sleep(self.SLEEP_TIME)
             current_wait_time += self.SLEEP_TIME
         raise ElasticSearchDataNotUploaded
 
     @typechecked()
-    def upload_to_elasticsearch(self, index: str, data: dict, doc_type: str = '_doc', es_add_items: dict = None, **kwargs):
+    def upload_to_elasticsearch(self, index: str, data: dict, doc_type: str = '_doc', es_add_items: dict = None,
+                                **kwargs):
         """
         This method is upload json data into elasticsearch
         :param index: index name to be stored in elasticsearch
         :param data: data must me in dictionary i.e. {'key': 'value'}
         :param doc_type:
         :param es_add_items:
         :return:
@@ -204,28 +207,46 @@
         }
         query['query']['bool']['filter']['range']['timestamp']['lte'] = str(end_datetime.replace(microsecond=0))
         query['query']['bool']['filter']['range']['timestamp']['gte'] = str(start_datetime.replace(microsecond=0))
         return query
 
     @typechecked()
     @logger_time_stamp
-    def fetch_data_between_range(self, es_index: str, start_datetime: datetime, end_datetime: datetime):
+    def fetch_data_by_es_query(self, es_index: str, query: dict = None, start_datetime: datetime = None,
+                               end_datetime: datetime = None, result_agg: bool = False, group_by: str = ''):
         """
-        This method fetches the data in between range
+        This method fetches the data in between range, if you need aggregation results pass you own query with aggegation
         @param es_index:
         @param start_datetime:
         @param end_datetime:
+        @param query:
+        @param result_agg:
+        @param group_by:
         @return:
         """
+        es_data = []
         if self.__es.indices.exists(index=es_index):
-            query_body = self.get_query_data_between_range(start_datetime=start_datetime, end_datetime=end_datetime)
-            data = self.__es.search(index=es_index, body=query_body, doc_type='_doc').get('hits')
-            if data:
-                return data['hits']
-        return []
+            if not query:
+                if start_datetime and end_datetime:
+                    query = self.get_query_data_between_range(start_datetime=start_datetime, end_datetime=end_datetime)
+            if query:
+                response = self.__es.search(index=es_index, body=query, doc_type='_doc', size=100, scroll='1h')
+                if result_agg:
+                    es_data.extend(response.get('aggregations').get(group_by).get('buckets'))
+                else:
+                    scroll_id = response.get('_scroll_id')
+                    if response.get('hits').get('hits'):
+                        es_data.extend(response.get('hits').get('hits'))
+                    while scroll_id:
+                        response = self.__es.scroll(scroll_id=scroll_id, scroll="1h")
+                        if len(response.get('hits').get('hits')) > 0:
+                            es_data.extend(response.get('hits').get('hits'))
+                        else:
+                            break
+        return es_data
 
     @typechecked()
     @logger_time_stamp
     def delete_data_in_between_in_es(self, es_index: str, start_datetime: datetime, end_datetime: datetime):
         """
         This method deletes the data in between two ranges
         @param es_index:
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/google_drive/google_drive_operations.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/google_drive/google_drive_operations.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/google_drive/upload_to_gsheet.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/google_drive/upload_to_gsheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,29 @@
                 accounts_df['AccountId'] == account_id].reset_index().to_dict(
                 orient='records')
             if account_row:
                 return account_row[0].get('CostCenter', 0), round(
                     float(account_row[0].get('Budget', '0').replace(',', '')), 0), str(account_row[0].get('Year')), account_row[0].get('Owner')
             return 0, 0, '', 'Others'
 
+    def get_monthly_spa(self, month_name: str, dir_path: str = ''):
+        """This method gets the monthly savings plan amortization"""
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            sheet_name = 'ASP'
+            dirtectory = dir_path if dir_path else tmp_dir
+            file_path = f'{tmp_dir}/{sheet_name}.csv' if not dir_path else f'{dir_path}/{sheet_name}.csv'
+            if not os.path.exists(file_path):
+                self.gsheet_operations.download_spreadsheet(spreadsheet_id=self.__gsheet_id, sheet_name=sheet_name, file_path=dirtectory)
+            accounts_df = pd.read_csv(file_path)
+            records = accounts_df.to_dict(orient='records')
+            for record in records:
+                if record.get('Month').lower() == month_name.lower():
+                    return float(record.get('Total'))
+            return 0
+
     def format_for_updating_the_cells(self, update_data: list, gsheet_data: pd, sheet_name: str, doc_id: str, doc_id2: str = ''):
         """
         This method format the data to be updated to GSheet and update in the GSheet
         @param doc_id2:
         @param update_data:
         @param gsheet_data:
         @param sheet_name:
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/jira/jira.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/jira/jira.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/ldap/ldap_search.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/ldap/ldap_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,16 @@
         @return:
         """
         try:
             user_data = {'displayName': str(data['displayName'][0], 'UTF-8'), 'FullName': str(data['cn'][0], 'UTF-8')}
             manager_name, manager_id = self.__get_manager_name(manager_data=str(data['manager'][0], 'UTF-8'))
             user_data['managerName'] = manager_name
             user_data['managerId'] = manager_id
+            user_data['ManagerName'] = manager_name
+            user_data['ManagerId'] = manager_id
             return user_data
         except Exception as err:
             return []
 
     def get_details(self, user_name: str):
         """
         This method get the user data from ldap
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/logger/logger_time_stamp.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/logger/logger_time_stamp.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/mails/gmail.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/mails/gmail.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/mails/mail_message.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/mails/mail_message.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,34 @@
-
+from cloud_governance.common.ldap.ldap_search import LdapSearch
 from cloud_governance.main.environment_variables import environment_variables
 
 
 class MailMessage:
+
     RESTRICTION = 'Do not reply this email. If you need more clarification, please reach out to us in the CoreOS slack channel - #perf-dept-public-clouds.'
+    FOOTER = '<div style="color:gray">---<br />Thanks, <br />Cloud GovernanceTeam</div>'
 
     def __init__(self):
         self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.account = self.__environment_variables_dict.get('account', '')
         self.policy = self.__environment_variables_dict.get('policy', '')
         self.region = self.__environment_variables_dict.get('AWS_DEFAULT_REGION', '')
+        self.__portal = self.__environment_variables_dict.get('CRO_PORTAL', '')
+        self.__cro_duration_days = self.__environment_variables_dict.get('CRO_DURATION_DAYS')
+        self.__LDAP_HOST_NAME = self.__environment_variables_dict.get('LDAP_HOST_NAME')
+        self.__ldap_search = LdapSearch(ldap_host_name=self.__LDAP_HOST_NAME)
+
+    def get_user_ldap_details(self, user_name: str):
+        """
+        This method return user details from ldap
+        :param user_name:
+        :return:
+        """
+        user_details = self.__ldap_search.get_user_details(user_name=user_name)
+        return user_details.get('displayName')
 
     def ec2_stop(self, name: str, days: int, image_id: str, delete_instance_days: int, instance_name: str,
                  resource_id: str, stopped_time: str, ec2_type: str, **kwargs):
         extra_purse = ''
         if kwargs.get("extra_purse"):
             extra_purse = f', Cost {round(kwargs.get("extra_purse"), 3)} $ '
         subject = f'cloud-governance alert: ec2-stop'
@@ -223,56 +238,117 @@
                 Best Regards,<br/>
                 Cloud-governance Team<br/>
             </address>
         </div>
         """.strip()
         return subject, body
 
-    def get_long_run_alert(self, days: int, user: str, jira_id: str):
-        """
-        This method return the LongRun, second Alert Message
+    def cro_monitor_alert_message(self, days: int, user: str, ticket_id: str):
         """
-        subject = f'Cloud LongRun Alert: Expiring in {days} days'
+        This method return the CRO Alert Message
+        :param days:
+        :param user:
+        :param ticket_id:
+        :return:
+        """
+        ticket_id = ticket_id.split('-')[-1]
+        subject = f'CRO Alert: Expiring in {days} days'
+        user_display_name = self.get_user_ldap_details(user_name=user)
         body = f"""
                 <div>
-                <p>Hi {user},</p>
+                <p>Hi {user_display_name},</p>
                 </div>
                 <div>
-                    <p>This is a message to alert you that in {days} days, the cloud request is expiring.</p>
-                    <p>Please take an action. If you are not using the instances Terminate the instances.</p>
-                    <p>Refer to the Jira issue: <a href="https://issues.redhat.com/browse/{jira_id}" target="_blank">{jira_id}</a></p>
-                    <p>Visit the <a href="https://clouds.perfdept.aws.rhperfscale.org:5000/wiki/clouds">wiki page</a> to get more information</p>
-                </div>
-                <div style="color:gray" class="footer">
-                    <address>
-                        --<br/>
-                        Best Regards,<br/>
-                        Cloud-governance Team<br/>
-                    </address>
+                    <p>You project budget request (TicketId: {ticket_id}) will be expired in {days} days</p>
+                    <p>You can extend the project duration in the following url {self.__portal} or terminate the instances</p>
+                    <p>Visit the <a href="{self.__portal}">wiki page</a> to get more information</p>
                 </div>
+                {self.FOOTER}
 """.strip()
         return subject, body
 
-    def get_long_run_expire_alert(self, user: str, jira_id: str):
+    def cro_cost_over_usage(self, **kwargs):
         """
-        This method return the LongRun, Expire Alert Message
+        This method returns the subject, body for cost over usage
+        :param kwargs:
+        :return:
+        """
+        cloud_name = kwargs.get('CloudName', 'NA').upper()
+        over_usage_cost = kwargs.get('OverUsageCost', 'NA')
+        full_name = kwargs.get('FullName', '')
+        if not full_name:
+            full_name = kwargs.get('to')
+        user_cost = round(kwargs.get('Cost', 0), 3)
+        subject = f'{cloud_name} Cost Over Usage alert: > {over_usage_cost} $'
+        body = f"""
+        <div>
+        Hi {full_name},
+        </div><br/>
+        <div>
+            Your {cloud_name} cost usage in the last {self.__cro_duration_days} days is {user_cost}$ and it's over {over_usage_cost} $.<br/>
+            You must open the project ticket in the following <a href="{self.__portal}">Link</a>.<br />
+            After submitting a ticket, you must add Tag (TicketID:#) to every active resource that is related to the project ticket.<br/>
+            
+            If you have any questions, please let us know in slack channel #perf-dept-public-clouds
+        <div><br/><br/>
+        {self.FOOTER}
+"""
+        return subject, body
+
+    def cro_request_for_manager_approval(self, manager: str, user: str, cloud_name: str):
         """
-        subject = f'LongRun Alert: Expired'
+        This method returns the message for manager, regarding user approval
+        :param manager:
+        :param user:
+        :param cloud_name:
+        :return:
+        """
+        subject = 'CRO Alert: Required budget approval'
+        manager_full_name = self.get_user_ldap_details(user_name=manager)
+        user_full_name = self.get_user_ldap_details(user_name=user)
         body = f"""
-                <div>
-                <p>Hi {user},</p>
-                </div>
-                <div>
-                    <p>This is a message to alert you that the cloud long run request is expired.</p>
-                    <p>Please take an action. If you are not using the instances Terminate the instances.</p>
-                    <p>Refer to the Jira issue: <a href="https://issues.redhat.com/browse/{jira_id}" target=="_blank">{jira_id}</a></p>
-                    <p>Visit the <a href="https://clouds.perfdept.aws.rhperfscale.org:5000/wiki/clouds">wiki page</a> to get more information</p>
-                </div>
-                <div style="color:gray" class="footer">
-                    <address>
-                        --<br/>
-                        Best Regards,<br/>
-                        Cloud-governance Team<br/>
-                    </address>
-                </div>
-        """.strip()
+            <div>Hi {manager_full_name},</div><br />
+            <div>{user_full_name} is waiting for your project budget approval<br />
+            Please verify and approve the request in the following url <a href="{self.__portal}">{self.__portal}</a></div><br />
+            {self.FOOTER}
+        """
+        return subject, body
+
+    def cro_send_user_alert_to_add_tags(self, user: str, ticket_id: str):
+        """
+        This method return the subject, body for adding tags
+        :param user:
+        :param ticket_id:
+        :return:
+        """
+        subject = 'CRO Alert: Required addition of TicketId tag'
+        ticket_id = ticket_id.split('-')[-1]
+        user_display_name = self.get_user_ldap_details(user_name=user)
+        body = f"""
+        <div>Hi {user_display_name},</div><br />
+        <p>Your project budget request ( TicketId: # ) was approved by your manager.</p><br />
+        <p>Please tag your instances with tag TicketId: {ticket_id}</p>
+        </div><br />
+        {self.FOOTER}
+        """
+        return subject, body
+
+    def cro_send_closed_alert(self, user: str, es_data: dict, ticket_id: str):
+        """
+        This method send cro ticket close alert
+        :param user:
+        :param es_data:
+        :param ticket_id:
+        :return:
+        """
+        subject = 'CRO Alert: Closing ticket'
+        ticket_id = ticket_id.split('-')[-1]
+        user_full_name = self.get_user_ldap_details(user_name=user)
+        body = f"""
+        <div>Hi {user_full_name},</div><br />
+            <div>
+            Your cloud project request ( TicketId:{ticket_id} ) duration expired and the ticket auto closed.<br />
+            You can find the summary in <a href="{self.__portal}/wikipage">Portal</a>.<br />
+            </div><br /><br/>
+        {self.FOOTER}
+        """
         return subject, body
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/common/mails/postfix.py` & `athiru-cloud-governance-1.1.89/cloud_governance/common/mails/postfix.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.reply_to = self.__environment_variables_dict.get('REPLY_TO', 'dev-null@redhat.com')
         self.__es_host = self.__environment_variables_dict.get('es_host', '')
         self.__policy = self.__environment_variables_dict.get('policy', '')
         self.__es_port = self.__environment_variables_dict.get('es_port', '')
         self.__account = self.__environment_variables_dict.get('account', '')
         self.__policy_output = self.__environment_variables_dict.get('policy_output', '')
+        self.__email_alert = self.__environment_variables_dict.get('EMAIL_ALERT')
         self.bucket_name, self.key = self.get_bucket_name()
         self.__es_index = 'cloud-governance-mail-messages'
         if self.__es_host:
             self.__es_operations = ElasticSearchOperations(es_host=self.__es_host, es_port=self.__es_port)
         if self.__policy_output:
             self.__s3_operations = S3Operations(region_name='us-east-1')
 
@@ -49,66 +50,69 @@
             key = targets[3]
         else:
             bucket_name = self.__policy_output
         return bucket_name, key
 
     @logger_time_stamp
     def send_email_postfix(self, subject: str, to: any, cc: list, content: str, **kwargs):
-        msg = MIMEMultipart('alternative')
-        msg["Subject"] = subject
-        msg["From"] = "%s <%s>" % (
-            'cloud-governance',
-            "@".join(["noreply-cloud-governance", 'redhat.com']),
-        )
-        if isinstance(to, str):
-            msg["To"] = "@".join([to, 'redhat.com'])
-        elif isinstance(to, list):
-            msg["To"] = ", ".join(to)
-        msg["Cc"] = ",".join(cc)
-        # msg.add_header("Reply-To", self.reply_to)
-        # msg.add_header("User-Agent", self.reply_to)
-        if kwargs.get('filename'):
-            attachment = MIMEText(open(kwargs['filename']).read())
-            attachment.add_header('Content-Disposition', 'attachment',
-                                  filename=kwargs['filename'].split('/')[-1])
-            msg.attach(attachment)
-        if kwargs.get('mime_type'):
-            msg.attach(MIMEText(content, kwargs.get('mime_type')))
-        else:
-            msg.attach(MIMEText(content))
-        email_string = msg.as_string()
-        email_host = 'localhost'
-        try:
-            with smtplib.SMTP(email_host) as s:
-                try:
-                    logger.debug(email_string)
-                    s.send_message(msg)
-                    if isinstance(to, str):
-                        logger.info(f'Mail sent successfully to {to}@redhat.com')
-                    elif isinstance(to, list):
-                        logger.info(f'Mail sent successfully to {", ".join(to)}@redhat.com')
-                    if kwargs.get('filename'):
-                        file_name = kwargs['filename'].split('/')[-1]
-                        date_key = datetime.datetime.now().strftime("%Y%m%d%H")
-                        if self.__policy_output:
-                            self.__s3_operations.upload_file(file_name_path=kwargs['filename'],
-                                                             bucket=self.bucket_name, key=f'{self.key}/{self.__policy}/{date_key}',
-                                                             upload_file=file_name)
-                            s3_path = f'{self.__policy_output}/logs/{self.__policy}/{date_key}/{file_name}'
-                            content += f'\n\nresource_file_path: s3://{s3_path}\n\n'
-                    data = {'Policy': self.__policy, 'To': to, 'Cc': cc, 'Message': content, 'Account': self.__account.upper(), 'MessageType': kwargs.get('message_type')}
-                    if kwargs.get('resource_id'):
-                        data['resource_id'] = kwargs['resource_id']
-                    if kwargs.get('extra_purse'):
-                        data['extra_purse'] = round(kwargs['extra_purse'], 3)
-                    if self.__es_host:
-                        self.__es_operations.upload_to_elasticsearch(data=data, index=self.__es_index)
-                        logger.info(f'Uploaded to es index: {self.__es_index}')
-                    else:
-                        logger.info('Error missing the es_host')
-                except smtplib.SMTPException as ex:
-                    logger.info(f'Error while sending mail, {ex}')
-                    return False
-            return True
-        except Exception as err:
-            logger.info(f'Some error occurred, {err}')
-            return False
+        if self.__email_alert:
+            cc = [cc_user for cc_user in cc if to not in cc_user]
+            cc = [cc_user if '@redhat.com' in cc_user else f'{cc_user}@redhat.com' for cc_user in cc]
+            msg = MIMEMultipart('alternative')
+            msg["Subject"] = subject
+            msg["From"] = "%s <%s>" % (
+                'cloud-governance',
+                "@".join(["noreply-cloud-governance", 'redhat.com']),
+            )
+            if isinstance(to, str):
+                msg["To"] = "@".join([to, 'redhat.com'])
+            elif isinstance(to, list):
+                msg["To"] = ", ".join(to)
+            msg["Cc"] = ",".join(cc)
+            # msg.add_header("Reply-To", self.reply_to)
+            # msg.add_header("User-Agent", self.reply_to)
+            if kwargs.get('filename'):
+                attachment = MIMEText(open(kwargs['filename']).read())
+                attachment.add_header('Content-Disposition', 'attachment',
+                                      filename=kwargs['filename'].split('/')[-1])
+                msg.attach(attachment)
+            if kwargs.get('mime_type'):
+                msg.attach(MIMEText(content, kwargs.get('mime_type')))
+            else:
+                msg.attach(MIMEText(content))
+            email_string = msg.as_string()
+            email_host = 'localhost'
+            try:
+                with smtplib.SMTP(email_host) as s:
+                    try:
+                        logger.debug(email_string)
+                        s.send_message(msg)
+                        if isinstance(to, str):
+                            logger.info(f'Mail sent successfully to {to}@redhat.com')
+                        elif isinstance(to, list):
+                            logger.info(f'Mail sent successfully to {", ".join(to)}@redhat.com')
+                        if kwargs.get('filename'):
+                            file_name = kwargs['filename'].split('/')[-1]
+                            date_key = datetime.datetime.now().strftime("%Y%m%d%H")
+                            if self.__policy_output:
+                                self.__s3_operations.upload_file(file_name_path=kwargs['filename'],
+                                                                 bucket=self.bucket_name, key=f'{self.key}/{self.__policy}/{date_key}',
+                                                                 upload_file=file_name)
+                                s3_path = f'{self.__policy_output}/logs/{self.__policy}/{date_key}/{file_name}'
+                                content += f'\n\nresource_file_path: s3://{s3_path}\n\n'
+                        data = {'Policy': self.__policy, 'To': to, 'Cc': cc, 'Message': content, 'Account': self.__account.upper(), 'MessageType': kwargs.get('message_type')}
+                        if kwargs.get('resource_id'):
+                            data['resource_id'] = kwargs['resource_id']
+                        if kwargs.get('extra_purse'):
+                            data['extra_purse'] = round(kwargs['extra_purse'], 3)
+                        if self.__es_host:
+                            self.__es_operations.upload_to_elasticsearch(data=data, index=self.__es_index)
+                            logger.info(f'Uploaded to es index: {self.__es_index}')
+                        else:
+                            logger.info('Error missing the es_host')
+                    except smtplib.SMTPException as ex:
+                        logger.info(f'Error while sending mail, {ex}')
+                        return False
+                return True
+            except Exception as err:
+                logger.info(f'Some error occurred, {err}')
+                return False
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/main/environment_variables.py` & `athiru-cloud-governance-1.1.89/cloud_governance/main/environment_variables.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+import argparse
 import os
+import tempfile
+from ast import literal_eval
 
-from cloud_governance.common.clouds.aws.iam.iam_operations import IAMOperations
+import boto3
+
+from cloud_governance.main.environment_variables_exceptions import ParseFailed
 
 
 class EnvironmentVariables:
     """
     This class manages the environment variable parameters
     """
 
@@ -27,21 +32,19 @@
 
             except FileNotFoundError:
                 pass  # ignore
 
         ##################################################################################################
         # dynamic parameters - configure for local run
         # parameters for running policies
-        self._environment_variables_dict['account'] = EnvironmentVariables.get_env('account', '').upper()
+        self._environment_variables_dict['account'] = EnvironmentVariables.get_env('account', '').upper().strip()
         self._environment_variables_dict['AWS_DEFAULT_REGION'] = EnvironmentVariables.get_env('AWS_DEFAULT_REGION', '')
-
+        self._environment_variables_dict['PUBLIC_CLOUD_NAME'] = EnvironmentVariables.get_env('PUBLIC_CLOUD_NAME', 'AWS')
         if EnvironmentVariables.get_env('AWS_ACCESS_KEY_ID', '') and EnvironmentVariables.get_env('AWS_SECRET_ACCESS_KEY', ''):
-            self.iam_operations = IAMOperations()
-            self._environment_variables_dict['account'] = self.iam_operations.get_account_alias_cloud_name()[0].upper()
-
+            self._environment_variables_dict['account'] = self.get_aws_account_alias_name().upper()
         self._environment_variables_dict['policy'] = EnvironmentVariables.get_env('policy', '')
 
         self._environment_variables_dict['aws_non_cluster_policies'] = ['ec2_idle', 'ec2_stop', 'ec2_run', 'ebs_in_use',
                                                                         'ebs_unattached', 's3_inactive',
                                                                         'empty_roles', 'ip_unattached',
                                                                         'nat_gateway_unused',
                                                                         'zombie_snapshots', 'skipped_resources',
@@ -67,24 +70,25 @@
 
         # AWS Cost Explorer tags
         self._environment_variables_dict['cost_metric'] = EnvironmentVariables.get_env('cost_metric', 'UnblendedCost')
         self._environment_variables_dict['start_date'] = EnvironmentVariables.get_env('start_date', '')
         self._environment_variables_dict['end_date'] = EnvironmentVariables.get_env('end_date', '')
         self._environment_variables_dict['granularity'] = EnvironmentVariables.get_env('granularity', 'DAILY')
         self._environment_variables_dict['cost_explorer_tags'] = EnvironmentVariables.get_env('cost_explorer_tags', '{}')
+        self._environment_variables_dict['PUBLIC_CLOUD_NAME'] = EnvironmentVariables.get_env('PUBLIC_CLOUD_NAME', 'AWS')
 
         # AZURE Credentials
         self._environment_variables_dict['AZURE_ACCOUNT_ID'] = EnvironmentVariables.get_env('AZURE_ACCOUNT_ID', '')
         self._environment_variables_dict['AZURE_CLIENT_ID'] = EnvironmentVariables.get_env('AZURE_CLIENT_ID', '')
         self._environment_variables_dict['AZURE_TENANT_ID'] = EnvironmentVariables.get_env('AZURE_TENANT_ID', '')
         self._environment_variables_dict['AZURE_CLIENT_SECRET'] = EnvironmentVariables.get_env('AZURE_CLIENT_SECRET', '')
         if self._environment_variables_dict['AZURE_CLIENT_ID'] and self._environment_variables_dict['AZURE_TENANT_ID']\
                 and self._environment_variables_dict['AZURE_CLIENT_SECRET']:
             self._environment_variables_dict['PUBLIC_CLOUD_NAME'] = 'AZURE'
-        self._environment_variables_dict['TOTAL_ACCOUNTS'] = bool(EnvironmentVariables.get_env('TOTAL_ACCOUNTS', ''))
+        self._environment_variables_dict['TOTAL_ACCOUNTS'] = EnvironmentVariables.get_boolean_from_environment('TOTAL_ACCOUNTS', False)
 
         # IBM env vars
         self._environment_variables_dict['IBM_ACCOUNT_ID'] = EnvironmentVariables.get_env('IBM_ACCOUNT_ID', '')
         self._environment_variables_dict['IBM_API_USERNAME'] = EnvironmentVariables.get_env('IBM_API_USERNAME', '')
         self._environment_variables_dict['IBM_API_KEY'] = EnvironmentVariables.get_env('IBM_API_KEY', '')
         self._environment_variables_dict['USAGE_REPORTS_APIKEY'] = EnvironmentVariables.get_env('USAGE_REPORTS_APIKEY', '')
         if self._environment_variables_dict['USAGE_REPORTS_APIKEY']:
@@ -94,15 +98,15 @@
         self._environment_variables_dict['COST_CENTER_OWNER'] = EnvironmentVariables.get_env('COST_CENTER_OWNER', '')
 
         self._environment_variables_dict['tag_remove_name'] = EnvironmentVariables.get_env('tag_remove_name', '')
         self._environment_variables_dict['tag_custom'] = EnvironmentVariables.get_env('tag_custom', '{}')
 
         # Common env vars
         self._environment_variables_dict['dry_run'] = EnvironmentVariables.get_env('dry_run', 'yes')
-        self._environment_variables_dict['FORCE_DELETE'] = EnvironmentVariables.get_env('FORCE_DELETE', False)
+        self._environment_variables_dict['FORCE_DELETE'] = EnvironmentVariables.get_boolean_from_environment('FORCE_DELETE', False)
         self._environment_variables_dict['policy_output'] = EnvironmentVariables.get_env('policy_output', '')
         self._environment_variables_dict['bucket'] = EnvironmentVariables.get_env('bucket', '')
         self._environment_variables_dict['file_path'] = EnvironmentVariables.get_env('file_path', '')
         self._environment_variables_dict['file_name'] = EnvironmentVariables.get_env('file_name', '')
 
         # common elastic search vars
         self._environment_variables_dict['upload_data_elk'] = EnvironmentVariables.get_env('upload_data_elk', '')
@@ -133,42 +137,117 @@
 
         # Google Drive env vars
         self._environment_variables_dict['GOOGLE_APPLICATION_CREDENTIALS'] = EnvironmentVariables.get_env('GOOGLE_APPLICATION_CREDENTIALS', '')
         self._environment_variables_dict['SPREADSHEET_ID'] = EnvironmentVariables.get_env('SPREADSHEET_ID', '')
 
         # AWS Top Acconut
         self._environment_variables_dict['AWS_ACCOUNT_ROLE'] = EnvironmentVariables.get_env('AWS_ACCOUNT_ROLE', '')
+        self._environment_variables_dict['PAYER_SUPPORT_FEE_CREDIT'] = EnvironmentVariables.get_env('PAYER_SUPPORT_FEE_CREDIT', 0)
+        self._environment_variables_dict['TEMPORARY_DIR'] = EnvironmentVariables.get_env('TEMPORARY_DIR', '/tmp')
         self._environment_variables_dict['COST_CENTER_OWNER'] = EnvironmentVariables.get_env('COST_CENTER_OWNER', '{}')
 
         # Jira env parameters
         self._environment_variables_dict['JIRA_URL'] = EnvironmentVariables.get_env('JIRA_URL', '')
         self._environment_variables_dict['JIRA_USERNAME'] = EnvironmentVariables.get_env('JIRA_USERNAME', '')
         self._environment_variables_dict['JIRA_TOKEN'] = EnvironmentVariables.get_env('JIRA_TOKEN', '')
         self._environment_variables_dict['JIRA_QUEUE'] = EnvironmentVariables.get_env('JIRA_QUEUE', '')
         self._environment_variables_dict['JIRA_PASSWORD'] = EnvironmentVariables.get_env('JIRA_PASSWORD', '')
 
         # Cloud Resource Orchestration
+        self._environment_variables_dict['CRO_PORTAL'] = EnvironmentVariables.get_env('CRO_PORTAL', '')
         self._environment_variables_dict['CLOUD_NAME'] = EnvironmentVariables.get_env('CLOUD_NAME', '')
         self._environment_variables_dict['MONITOR'] = EnvironmentVariables.get_env('MONITOR', '')
-        self._environment_variables_dict['MANAGEMENT'] = bool(EnvironmentVariables.get_env('MANAGEMENT', False))
+        self._environment_variables_dict['MANAGEMENT'] = EnvironmentVariables.get_boolean_from_environment('MANAGEMENT', False)
+
+        # GCP Account
+        self._environment_variables_dict['GCP_DATABASE_NAME'] = EnvironmentVariables.get_env('GCP_DATABASE_NAME')
+        self._environment_variables_dict['GCP_DATABASE_TABLE_NAME'] = EnvironmentVariables.get_env('GCP_DATABASE_TABLE_NAME')
+        if self._environment_variables_dict.get('GCP_DATABASE_TABLE_NAME'):
+            self._environment_variables_dict['PUBLIC_CLOUD_NAME'] = 'GCP'
+
+        self._environment_variables_dict['EMAIL_ALERT'] = EnvironmentVariables.get_boolean_from_environment('EMAIL_ALERT', True)
+        self._environment_variables_dict['MANAGER_EMAIL_ALERT'] = EnvironmentVariables.get_boolean_from_environment('MANAGER_EMAIL_ALERT', True)
+        self._environment_variables_dict['UPDATE_TAG_BULKS'] = int(EnvironmentVariables.get_env('UPDATE_TAG_BULKS', '20'))
+
+        # CRO -- Cloud Resource Orch
+        self._environment_variables_dict['CLOUD_RESOURCE_ORCHESTRATION'] = EnvironmentVariables.get_boolean_from_environment('CLOUD_RESOURCE_ORCHESTRATION', False)
+        self._environment_variables_dict['USER_COST_INDEX'] = EnvironmentVariables.get_env('USER_COST_INDEX', '')
+        self._environment_variables_dict['CRO_ES_INDEX'] = EnvironmentVariables.get_env('CRO_ES_INDEX', 'cloud-governance-resource-orchestration')
+        self._environment_variables_dict['CRO_COST_OVER_USAGE'] = int(EnvironmentVariables.get_env('CRO_COST_OVER_USAGE', '500'))
+        self._environment_variables_dict['CRO_DEFAULT_ADMINS'] = literal_eval(EnvironmentVariables.get_env('CRO_DEFAULT_ADMINS', "[]"))
+        self._environment_variables_dict['CRO_DURATION_DAYS'] = int(EnvironmentVariables.get_env('CRO_DURATION_DAYS', '30'))
+        self._environment_variables_dict['RUN_ACTIVE_REGIONS'] = EnvironmentVariables.get_boolean_from_environment('RUN_ACTIVE_REGIONS', False)
+        self._environment_variables_dict['CRO_RESOURCE_TAG_NAME'] = EnvironmentVariables.get_env('CRO_RESOURCE_TAG_NAME', 'TicketId')
+        self._environment_variables_dict['CRO_REPLACED_USERNAMES'] = literal_eval(EnvironmentVariables.get_env('CRO_REPLACED_USERNAMES', "['osdCcsAdmin']"))
+
 
     @staticmethod
-    def get_env(var: str, defval: any = ''):
-        return os.environ.get(var, defval)
+    def to_bool(arg, def_val: bool = None):
+        if isinstance(arg, bool):
+            return arg
+        if isinstance(arg, (int, float)):
+            return arg != 0
+        if isinstance(arg, str):
+            arg = arg.lower()
+            if arg == 'true' or arg == 'yes':
+                return True
+            elif arg == 'false' or arg == 'no':
+                return False
+            try:
+                arg1 = int(arg)
+                return arg1 != 0
+            except Exception:
+                pass
+        if def_val is not None:
+            return def_val
+        raise ParseFailed(f'Cannot parse {arg} as a boolean value')
+
+    def get_aws_account_alias_name(self):
+        """
+        This method return the aws account alias name
+        :return:
+        """
+        iam_client = boto3.client('iam')
+        try:
+            account_alias = iam_client.list_account_aliases()['AccountAliases']
+            if account_alias:
+                return account_alias[0].upper()
+        except:
+            return os.environ.get('account', '').upper()
+
+
+    @staticmethod
+    def get_env(var: str, defval=''):
+        lcvar = var.lower()
+        dashvar = lcvar.replace('_', '-')
+        parser = argparse.ArgumentParser(description='Run CloudGovernance', allow_abbrev=False)
+        if lcvar == dashvar:
+            parser.add_argument(f"--{lcvar}", default=os.environ.get(var, defval), type=str, metavar='String', help=var)
+        else:
+            parser.add_argument(f"--{lcvar}", f"--{dashvar}", default=os.environ.get(var, defval), type=str,
+                                metavar='String', help=var)
+        args, ignore = parser.parse_known_args()
+        if hasattr(args, lcvar):
+            return getattr(args, lcvar)
+        else:
+            return os.environ.get(var, defval)
+
+    @staticmethod
+    def get_boolean_from_environment(var: str, defval: bool):
+        return EnvironmentVariables.to_bool(EnvironmentVariables.get_env(var), defval)
 
     @property
     def environment_variables_dict(self):
         """
         This method is getter
         """
         return self._environment_variables_dict
 
 
 environment_variables = EnvironmentVariables()
-
 # env vars examples
 # os.environ['AWS_DEFAULT_REGION'] = 'us-east-2'
 # os.environ['AWS_DEFAULT_REGION'] = 'all'
 # os.environ['policy'] = 'zombie_cluster_resource'
 # os.environ['validate_type'] = 'tags'
 # os.environ['user_tags'] = "['Budget', 'User', 'Owner', 'Manager', 'Environment', 'Project']"
 # os.environ['cost_metric'] = ''
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/main/es_uploader.py` & `athiru-cloud-governance-1.1.89/cloud_governance/main/es_uploader.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/main/main.py` & `athiru-cloud-governance-1.1.89/cloud_governance/main/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 import typeguard
 from ast import literal_eval  # str to dict
 import boto3  # regions
 
 from cloud_governance.cloud_resource_orchestration.monitor.cloud_monitor import CloudMonitor
+from cloud_governance.main.run_cloud_resource_orchestration import run_cloud_resource_orchestration
 from cloud_governance.policy.policy_operations.aws.cost_expenditure.cost_report_policies import CostReportPolicies
 from cloud_governance.policy.policy_operations.azure.azure_policy_runner import AzurePolicyRunner
 from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp, logger
 from cloud_governance.policy.policy_operations.aws.tag_cluster.run_tag_cluster_resouces import tag_cluster_resource, \
     remove_cluster_resources_tags
 from cloud_governance.policy.policy_operations.aws.tag_non_cluster.run_tag_non_cluster_resources import tag_non_cluster_resource, \
     remove_tag_non_cluster_resource, tag_na_resources
 from cloud_governance.policy.policy_operations.aws.tag_user.run_tag_iam_user import tag_iam_user, run_validate_iam_user_tags
 from cloud_governance.policy.policy_operations.aws.zombie_cluster.run_zombie_cluster_resources import zombie_cluster_resource
+from cloud_governance.policy.policy_operations.gcp.gcp_policy_runner import GcpPolicyRunner
 from cloud_governance.policy.policy_operations.gitleaks.gitleaks import GitLeaks
 from cloud_governance.policy.policy_operations.ibm.ibm_operations.ibm_policy_runner import IBMPolicyRunner
 from cloud_governance.main.environment_variables import environment_variables
 from cloud_governance.main.es_uploader import ESUploader
 from cloud_governance.common.clouds.aws.s3.s3_operations import S3Operations
 from cloud_governance.policy.policy_operations.aws.zombie_cluster.validate_zombies import ValidateZombies
 from cloud_governance.policy.policy_operations.aws.zombie_non_cluster.zombie_non_cluster_polices import ZombieNonClusterPolicies
@@ -164,20 +166,14 @@
             logger.exception(f'BadCredentialsException : {err}')
     else:
         logger.exception(f'Missing Policy name: {policy}')
         raise Exception(f'Missing Policy name: {policy}')
 
 
 @logger_time_stamp
-def run_cloud_management():
-    """This method run the cloud management"""
-    return CloudMonitor().run()
-
-
-@logger_time_stamp
 def main():
     """
     This main run 2 processes:
     1. ES uploader
     2. Run policy
     :return: the action output
     """
@@ -190,114 +186,126 @@
     upload_data_es = environment_variables_dict.get('upload_data_es', '')
     es_host = environment_variables_dict.get('es_host', '')
     es_port = environment_variables_dict.get('es_port', '')
     es_index = environment_variables_dict.get('es_index', '')
     es_doc_type = environment_variables_dict.get('es_doc_type', '')
     bucket = environment_variables_dict.get('bucket', '')
 
-    non_cluster_polices_runner = None
-    is_non_cluster_polices_runner = policy in environment_variables_dict.get('aws_non_cluster_policies')
-    if is_non_cluster_polices_runner:
-        non_cluster_polices_runner = ZombieNonClusterPolicies()
-
-    ibm_classic_infrastructure_policy_runner = None
-    is_tag_ibm_classic_infrastructure_runner = policy in environment_variables_dict.get('ibm_policies')
-    if not is_tag_ibm_classic_infrastructure_runner:
-        if environment_variables_dict.get('PUBLIC_CLOUD_NAME') and environment_variables_dict.get('PUBLIC_CLOUD_NAME').upper() == 'IBM':
-            is_tag_ibm_classic_infrastructure_runner = policy in environment_variables_dict.get('cost_policies')
-    if is_tag_ibm_classic_infrastructure_runner:
-        ibm_classic_infrastructure_policy_runner = IBMPolicyRunner()
-
-    is_cost_explorer_policies_runner = ''
-    if not environment_variables_dict.get('PUBLIC_CLOUD_NAME'):
-        cost_explorer_policies_runner = None
-        is_cost_explorer_policies_runner = policy in environment_variables_dict.get('cost_policies')
-        if is_cost_explorer_policies_runner:
-            cost_explorer_policies_runner = CostReportPolicies()
-
-    is_azure_policy_runner = ''
-    if environment_variables_dict.get('PUBLIC_CLOUD_NAME') and environment_variables_dict.get('PUBLIC_CLOUD_NAME').upper() == 'AZURE':
-        azure_cost_policy_runner = None
-        is_azure_policy_runner = policy in environment_variables_dict.get('cost_policies')
-        if is_azure_policy_runner:
-            azure_cost_policy_runner = AzurePolicyRunner()
-
-    # cloud_resource_orchestration lon_run/short_run
-    is_cloud_management = False
-    if environment_variables_dict.get('MANAGEMENT'):
-        is_cloud_management = True
-
-    @logger_time_stamp
-    def run_non_cluster_polices_runner():
-        """
-        This method run the aws non-cluster policies
-        @return:
-        """
-        non_cluster_polices_runner.run()
-
-    def run_tag_ibm_classic_infrastructure_runner():
-        """
-        This method run the IBM policies
-        @return:
-        """
-        ibm_classic_infrastructure_policy_runner.run()
-
-    @logger_time_stamp
-    def run_cost_explorer_policies_runner():
-        """
-        This method run the aws cost_explorer policies
-        @return:
-        """
-        cost_explorer_policies_runner.run()
-
-    @logger_time_stamp
-    def run_azure_policy_runner():
-        """
-        This method run the azure policies
-        @return:
-        """
-        azure_cost_policy_runner.run()
-
-    # 1. ELK Uploader
-    if upload_data_es:
-        input_data = {'es_host': es_host,
-                      'es_port': int(es_port),
-                      'es_index': es_index,
-                      'es_doc_type': es_doc_type,
-                      'es_add_items': {'account': account},
-                      'bucket': bucket,
-                      'logs_bucket_key': 'logs',
-                      's3_file_name': 'resources.json',
-                      'region': region_env,
-                      'policy': policy,
-                      }
-        elk_uploader = ESUploader(**input_data)
-        elk_uploader.upload_to_es(account=account)
-    # 2. POLICY
-    elif is_non_cluster_polices_runner:
-        run_non_cluster_polices_runner()
-    elif is_tag_ibm_classic_infrastructure_runner:
-        run_tag_ibm_classic_infrastructure_runner()
-    elif is_cost_explorer_policies_runner:
-        run_cost_explorer_policies_runner()
-    elif is_azure_policy_runner:
-        run_azure_policy_runner()
-    elif is_cloud_management:
-        run_cloud_management()
+    if environment_variables_dict.get('CLOUD_RESOURCE_ORCHESTRATION'):
+        run_cloud_resource_orchestration()
     else:
-        if not policy:
-            logger.exception(f'Missing Policy name: "{policy}"')
-            raise Exception(f'Missing Policy name: "{policy}"')
-        if region_env == 'all':
-            # must be set for boto3 client default region
-            # environment_variables_dict['AWS_DEFAULT_REGION'] = 'us-east-2'
-            ec2 = boto3.client('ec2')
-            regions_data = ec2.describe_regions()
-            for region in regions_data['Regions']:
-                # logger.info(f"region: {region['RegionName']}")
-                environment_variables_dict['AWS_DEFAULT_REGION'] = region['RegionName']
-                run_policy(account=account, policy=policy, region=region['RegionName'], dry_run=dry_run)
+        non_cluster_polices_runner = None
+        is_non_cluster_polices_runner = policy in environment_variables_dict.get('aws_non_cluster_policies')
+        if is_non_cluster_polices_runner:
+            non_cluster_polices_runner = ZombieNonClusterPolicies()
+
+        ibm_classic_infrastructure_policy_runner = None
+        is_tag_ibm_classic_infrastructure_runner = policy in environment_variables_dict.get('ibm_policies')
+        if not is_tag_ibm_classic_infrastructure_runner:
+            if environment_variables_dict.get('PUBLIC_CLOUD_NAME') and environment_variables_dict.get('PUBLIC_CLOUD_NAME').upper() == 'IBM':
+                is_tag_ibm_classic_infrastructure_runner = policy in environment_variables_dict.get('cost_policies')
+        if is_tag_ibm_classic_infrastructure_runner:
+            ibm_classic_infrastructure_policy_runner = IBMPolicyRunner()
+
+        is_cost_explorer_policies_runner = ''
+        if environment_variables_dict.get('PUBLIC_CLOUD_NAME') == 'AWS':
+            cost_explorer_policies_runner = None
+            is_cost_explorer_policies_runner = policy in environment_variables_dict.get('cost_policies')
+            if is_cost_explorer_policies_runner:
+                cost_explorer_policies_runner = CostReportPolicies()
+
+        is_azure_policy_runner = ''
+        if environment_variables_dict.get('PUBLIC_CLOUD_NAME') and environment_variables_dict.get('PUBLIC_CLOUD_NAME').upper() == 'AZURE':
+            azure_cost_policy_runner = None
+            is_azure_policy_runner = policy in environment_variables_dict.get('cost_policies')
+            if is_azure_policy_runner:
+                azure_cost_policy_runner = AzurePolicyRunner()
+
+        is_gcp_policy_runner = ''
+        if environment_variables_dict.get('PUBLIC_CLOUD_NAME') and environment_variables_dict.get('PUBLIC_CLOUD_NAME').upper() == 'GCP':
+            gcp_cost_policy_runner = None
+            is_gcp_policy_runner = policy in environment_variables_dict.get('cost_policies')
+            if is_gcp_policy_runner:
+                gcp_cost_policy_runner = GcpPolicyRunner()
+
+        @logger_time_stamp
+        def run_non_cluster_polices_runner():
+            """
+            This method run the aws non-cluster policies
+            @return:
+            """
+            non_cluster_polices_runner.run()
+
+        def run_tag_ibm_classic_infrastructure_runner():
+            """
+            This method run the IBM policies
+            @return:
+            """
+            ibm_classic_infrastructure_policy_runner.run()
+
+        @logger_time_stamp
+        def run_cost_explorer_policies_runner():
+            """
+            This method run the aws cost_explorer policies
+            @return:
+            """
+            cost_explorer_policies_runner.run()
+
+        @logger_time_stamp
+        def run_azure_policy_runner():
+            """
+            This method run the azure policies
+            @return:
+            """
+            azure_cost_policy_runner.run()
+
+        @logger_time_stamp
+        def run_gcp_policy_runner():
+            """
+            This method run the gcp policies
+            """
+            gcp_cost_policy_runner.run()
+
+        # 1. ELK Uploader
+        if upload_data_es:
+            input_data = {'es_host': es_host,
+                          'es_port': int(es_port),
+                          'es_index': es_index,
+                          'es_doc_type': es_doc_type,
+                          'es_add_items': {'account': account},
+                          'bucket': bucket,
+                          'logs_bucket_key': 'logs',
+                          's3_file_name': 'resources.json',
+                          'region': region_env,
+                          'policy': policy,
+                          }
+            elk_uploader = ESUploader(**input_data)
+            elk_uploader.upload_to_es(account=account)
+        # 2. POLICY
+        elif is_non_cluster_polices_runner:
+            run_non_cluster_polices_runner()
+        elif is_tag_ibm_classic_infrastructure_runner:
+            run_tag_ibm_classic_infrastructure_runner()
+        elif is_cost_explorer_policies_runner:
+            run_cost_explorer_policies_runner()
+        elif is_azure_policy_runner:
+            run_azure_policy_runner()
+        elif is_gcp_policy_runner:
+            run_gcp_policy_runner()
         else:
-            run_policy(account=account, policy=policy, region=region_env, dry_run=dry_run)
+            if not policy:
+                logger.exception(f'Missing Policy name: "{policy}"')
+                raise Exception(f'Missing Policy name: "{policy}"')
+            if region_env == 'all':
+                # must be set for boto3 client default region
+                # environment_variables_dict['AWS_DEFAULT_REGION'] = 'us-east-2'
+                ec2 = boto3.client('ec2')
+                regions_data = ec2.describe_regions()
+                for region in regions_data['Regions']:
+                    # logger.info(f"region: {region['RegionName']}")
+                    environment_variables_dict['AWS_DEFAULT_REGION'] = region['RegionName']
+                    run_policy(account=account, policy=policy, region=region['RegionName'], dry_run=dry_run)
+            else:
+                run_policy(account=account, policy=policy, region=region_env, dry_run=dry_run)
 
 
 main()
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/cost_billing_reports.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/cost_billing_reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             self.__cost_explorer_operations = CostExplorerOperations()
             self.elastic_upload = ElasticUpload()
             self.account_name, self.__cloud_name = IAMOperations().get_account_alias_cloud_name()
             self.__account_id = STSOperations().get_account_id()
             self.__gsheet_id = self._environment_variables_dict.get('SPREADSHEET_ID', '')
             self.gdrive_operations = GoogleDriveOperations()
             self.update_to_gsheet = UploadToGsheet()
-            self.cost_center, self.__account_budget, self.__years = self.update_to_gsheet.get_cost_center_budget_details(account_id=self.__account_id)
+            self.cost_center, self.__account_budget, self.__years, self.__owner = self.update_to_gsheet.get_cost_center_budget_details(account_id=self.__account_id)
         except:
             pass
 
     def __get_start_date(self, end_date: datetime, days: int, operation: operator) -> datetime:
         """
         This method return start_date
         @param operation:
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/cost_explorer.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/cost_explorer.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/cost_over_usage.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/cost_over_usage.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/ebs_in_use.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/ebs_in_use.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/ebs_unattached.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/ebs_unattached.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/ec2_idle.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/ec2_idle.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/ec2_run.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/ec2_run.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/ec2_stop.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/ec2_stop.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/empty_roles.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/empty_roles.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/ip_unattached.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/ip_unattached.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/monthly_report.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/monthly_report.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/nat_gateway_unused.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/nat_gateway_unused.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/s3_inactive.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/s3_inactive.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/skipped_resources.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/skipped_resources.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/zombie_cluster_resource.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/zombie_cluster_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         cluster_left_out_days = {}
         if zombies:
             for zombie, cluster_tag in zombies.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_ec2_resource.delete_zombie_resource(resource_id=zombie, resource='ec2_volume')
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         self.delete_ec2_resource.delete_zombie_resource(resource_id=zombie, resource='ec2_volume')
 
         return zombies, cluster_left_out_days
 
     def zombie_cluster_ami(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of cluster's ami according to cluster tag name and cluster name data
@@ -221,15 +221,15 @@
                     resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie,
                     cluster_tag=cluster_tag)
                 try:
                     if delete_cluster_resource and self.delete:
                         self.ec2_client.deregister_image(ImageId=zombie)
                         logger.info(f'deregister_image: {zombie}')
                     else:
-                        if self._force_delete:
+                        if self._force_delete and self.delete:
                             self.ec2_client.deregister_image(ImageId=zombie)
                             logger.info(f'deregister_image: {zombie}')
                 except Exception as err:
                     logger.exception(f'Cannot deregister_image: {zombie}, {err}')
         return zombies, cluster_left_out_days
 
     def zombie_cluster_snapshot(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
@@ -243,15 +243,15 @@
         cluster_left_out_days = {}
         if zombies:
             for zombie, cluster_tag in zombies.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_ec2_resource.delete_zombie_resource(resource='ebs_snapshots', resource_id=zombie)
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         self.delete_ec2_resource.delete_zombie_resource(resource='ebs_snapshots', resource_id=zombie)
         return zombies, cluster_left_out_days
 
     def __get_tag_from_resource_tags(self, tags: list, cluster_tag: str):
         """
         This method retunrs the cluster tag
         @param tags:
@@ -334,15 +334,15 @@
                 vpc_id = self.__extract_vpc_id_from_resource_data(zombie_id=zombie, resource_data=security_groups, input_tag='GroupId')
                 zombie_ids = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=security_groups, output_tag='GroupId', cluster_tag=cluster_tag)
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     for zombie_id in zombie_ids:
                         self.delete_ec2_resource.delete_zombie_resource('security_group', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         for zombie_id in zombie_ids:
                             self.delete_ec2_resource.delete_zombie_resource('security_group', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
 
         return zombies, cluster_left_out_days
 
     def zombie_cluster_elastic_ip(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
@@ -373,15 +373,15 @@
                         self.delete_ec2_resource.delete_zombie_resource(resource='elastic_ip', resource_id=zombie, deletion_type='disassociate')
         if zombies_all:
             for zombie, cluster_tag in zombies_all.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources_all, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_ec2_resource.delete_zombie_resource(resource='elastic_ip', resource_id=zombie, cluster_tag=cluster_tag)
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         self.delete_ec2_resource.delete_zombie_resource(resource='elastic_ip', resource_id=zombie, cluster_tag=cluster_tag)
         zombies = {**zombies_all}
         return zombies, cluster_left_out_days
 
     def zombie_cluster_network_interface(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of zombie cluster's network interface according to existing instances and cluster name data
@@ -402,15 +402,15 @@
                 else:
                     zombie_ids = [zombie]
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days( resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     for zombie_id in zombie_ids:
                         self.delete_ec2_resource.delete_zombie_resource(resource='network_interface', resource_id=zombie_id, cluster_tag=cluster_tag)
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         for zombie_id in zombie_ids:
                             self.delete_ec2_resource.delete_zombie_resource(resource='network_interface', resource_id=zombie_id, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_load_balancer(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of cluster's load balancer according to cluster vpc and cluster name data
@@ -437,15 +437,15 @@
         cluster_left_out_days = {}
         if zombies:
             for zombie, cluster_tag in zombies.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_ec2_resource.delete_zombie_resource(resource='load_balancer', resource_id=zombie, cluster_tag=cluster_tag)
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         self.delete_ec2_resource.delete_zombie_resource(resource='load_balancer', resource_id=zombie, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_load_balancer_v2(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of cluster's load balancer according to cluster vpc and cluster name data
         """
@@ -470,15 +470,15 @@
         cluster_left_out_days = {}
         if zombies:
             for zombie, cluster_tag in zombies.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_ec2_resource.delete_zombie_resource(resource='load_balancer_v2', resource_id=zombie, cluster_tag=cluster_tag)
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         self.delete_ec2_resource.delete_zombie_resource(resource='load_balancer_v2', resource_id=zombie, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def __get_all_exist_vpcs(self):
         """
         This method return all exist vpc ids (for supporting Network ACL - missing OpenShift tags)
         :return:
@@ -506,15 +506,15 @@
         cluster_left_out_days = {}
         if zombies:
             for zombie, cluster_tag in zombies.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_ec2_resource.delete_zombie_resource(resource='vpc', resource_id=zombie, pending_resources=delete_dict, cluster_tag=cluster_tag)
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         self.delete_ec2_resource.delete_zombie_resource(resource='vpc', resource_id=zombie, pending_resources=delete_dict, cluster_tag=cluster_tag)
 
         return zombies, cluster_left_out_days
 
     def zombie_cluster_subnet(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of cluster's subnet according to cluster tag name and cluster name data
@@ -533,15 +533,15 @@
                 vpc_id = self.__extract_vpc_id_from_resource_data(zombie_id=zombie, resource_data=subnets_data, input_tag='SubnetId')
                 zombie_ids = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=subnets_data, output_tag='SubnetId', cluster_tag=cluster_tag)
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     for zombie_id in zombie_ids:
                         self.delete_ec2_resource.delete_zombie_resource(resource='subnet', resource_id=zombie_id, cluster_tag=cluster_tag)
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         for zombie_id in zombie_ids:
                             self.delete_ec2_resource.delete_zombie_resource(resource='subnet', resource_id=zombie_id,  cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_route_table(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of cluster's route table according to cluster tag name and cluster name data
@@ -560,15 +560,15 @@
                 zombie_ids = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=route_tables_data,
                                                           output_tag='RouteTableId', cluster_tag=cluster_tag)
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     for zombie_id in zombie_ids:
                         self.delete_ec2_resource.delete_zombie_resource(resource='route_table', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         for zombie_id in zombie_ids:
                             self.delete_ec2_resource.delete_zombie_resource(resource='route_table', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_internet_gateway(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of cluster's route table internet gateway according to cluster tag name and cluster name data
@@ -589,15 +589,15 @@
                 else:
                     zombie_ids = [zombie]
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     for zombie_id in zombie_ids:
                         self.delete_ec2_resource.delete_zombie_resource(resource='internet_gateway', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         for zombie_id in zombie_ids:
                             self.delete_ec2_resource.delete_zombie_resource(resource='internet_gateway', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
 
         return zombies, cluster_left_out_days
 
     def zombie_cluster_dhcp_option(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
@@ -615,15 +615,15 @@
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     if vpc_id:
                         self.delete_ec2_resource.delete_zombie_resource(resource='dhcp_options', resource_id=zombie, vpc_id=vpc_id)
                     else:
                         self.delete_ec2_resource.delete_zombie_resource(resource='dhcp_options', resource_id=zombie)
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         if vpc_id:
                             self.delete_ec2_resource.delete_zombie_resource(resource='dhcp_options', resource_id=zombie, vpc_id=vpc_id)
                         else:
                             self.delete_ec2_resource.delete_zombie_resource(resource='dhcp_options', resource_id=zombie)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_vpc_endpoint(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
@@ -646,15 +646,15 @@
                 else:
                     zombie_ids = [zombies]
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     for zombie_id in zombie_ids:
                         self.delete_ec2_resource.delete_zombie_resource(resource='vpc_endpoints', resource_id=zombie_id, cluster_tag=cluster_tag)
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         for zombie_id in zombie_ids:
                             self.delete_ec2_resource.delete_zombie_resource(resource='vpc_endpoints', resource_id=zombie_id, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_nat_gateway(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of zombie cluster's nat gateway according to cluster tag name and cluster name data
@@ -672,15 +672,15 @@
                 vpc_id = self.__extract_vpc_id_from_resource_data(zombie, nat_gateways_data, input_tag='NatGatewayId')
                 zombie_ids = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=nat_gateways_data, output_tag='NatGatewayId', cluster_tag=cluster_tag)
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     for zombie_id in zombie_ids:
                         self.delete_ec2_resource.delete_zombie_resource(resource='nat_gateways', resource_id=zombie_id, cluster_tag=cluster_tag)
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         for zombie_id in zombie_ids:
                             self.delete_ec2_resource.delete_zombie_resource(resource='nat_gateways', resource_id=zombie_id, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_network_acl(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
         This method return list of zombie cluster's network acl according to existing vpc id and cluster name data
@@ -709,15 +709,15 @@
                     vpc_id = self.__extract_vpc_id_from_resource_data(zombie_id=zombie, resource_data=network_acls_data, input_tag='NetworkAclId')
                 zombie_ids = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=network_acls_data, output_tag='NetworkAclId', cluster_tag=cluster_tag)
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     for zombie_id in zombie_ids:
                         self.delete_ec2_resource.delete_zombie_resource(resource='network_acl', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         for zombie_id in zombie_ids:
                             self.delete_ec2_resource.delete_zombie_resource(resource='network_acl', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_role(self):
         """
         This method return list of cluster's role in all regions according to cluster name and cluster name data
@@ -747,15 +747,15 @@
             resources = self._get_tags_of_zombie_resources(resources=roles_data, resource_id_name='RoleName', zombies=zombies, aws_service='role')
             if zombies:
                 for zombie, cluster_tag in zombies.items():
                     cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                     if delete_cluster_resource and self.delete:
                         self.delete_iam_resource.delete_iam_zombie_resource(resource_id=zombie, resource_type='iam_role')
                     else:
-                        if self._force_delete:
+                        if self._force_delete and self.delete:
                             self.delete_iam_resource.delete_iam_zombie_resource(resource_id=zombie, resource_type='iam_role')
         return zombies, cluster_left_out_days
 
     def zombie_cluster_user(self):
         """
         This method return list of cluster's user according to cluster name and cluster name data
         * User is a global resource, need to scan for live cluster in all regions
@@ -781,15 +781,15 @@
         cluster_left_out_days = {}
         if zombies:
             for zombie, cluster_tag in zombies.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_iam_resource.delete_iam_zombie_resource(resource_id=zombie, resource_type='iam_user')
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         self.delete_iam_resource.delete_iam_zombie_resource(resource_id=zombie, resource_type='iam_user')
 
         return zombies, cluster_left_out_days
 
     def zombie_cluster_s3_bucket(self, cluster_stamp: str = 'image-registry'):
         """
         This method return list of cluster's s3 bucket according to cluster name and cluster name data
@@ -820,14 +820,14 @@
         cluster_left_out_days = {}
         if zombies:
             for zombie, cluster_tag in zombies.items():
                 cluster_left_out_days, delete_cluster_resource = self._check_zombie_cluster_deleted_days(resources=resources, cluster_left_out_days=cluster_left_out_days, zombie=zombie, cluster_tag=cluster_tag)
                 if delete_cluster_resource and self.delete:
                     self.delete_s3_resource.delete_zombie_s3_resource(resource_type='s3_bucket', resource_id=zombie)
                 else:
-                    if self._force_delete:
+                    if self._force_delete and self.delete:
                         self.delete_s3_resource.delete_zombie_s3_resource(resource_type='s3_bucket', resource_id=zombie)
 
         return zombies, cluster_left_out_days
 
 # zombie_cluster_resources = ZombieClusterResources(cluster_prefix='kubernetes.io/cluster/', delete=False, region='us-east-2')
 # print(zombie_cluster_resources.zombie_cluster_subnet())
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/aws/zombie_snapshots.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/aws/zombie_snapshots.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/azure/cost_billing_reports.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/azure/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/ibm/cost_billing_reports.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/ibm/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/ibm/ibm_cost_over_usage.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/ibm/ibm_cost_over_usage.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/ibm/ibm_cost_report.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/ibm/ibm_cost_report.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/ibm/tag_baremetal.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/ibm/tag_baremetal.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/ibm/tag_vm.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/ibm/tag_vm.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 class TagClusterResources(TagClusterOperations):
     """
     This class filter cluster resources by cluster name, and update tags when passing input_tags
     """
 
     SHORT_ID = 5
+    NA_VALUE = 'NA'
 
     def __init__(self, cluster_name: str = None, cluster_prefix: str = None, input_tags: dict = None,
                  region: str = 'us-east-2', dry_run: str = 'yes', cluster_only: bool = False):
         super().__init__(cluster_name=cluster_name, cluster_prefix=cluster_prefix, input_tags=input_tags, region=region, dry_run=dry_run, cluster_only=cluster_only)
         self.cluster_key = self.__init_cluster_name()
         self.non_cluster_update = TagNonClusterResources(region=region, dry_run=dry_run, input_tags=input_tags)
 
@@ -137,18 +138,15 @@
                                     cluster_ids[tag.get('Key')].append(resource_id)
                             else:
                                 cluster_ids[tag.get('Key')].append(resource_id)
         result_resources_list = []
         for cluster_name, cluster_id in cluster_ids.items():
             if self.dry_run == 'no':
                 try:
-                    if self.cluster_name in cluster_name:
-                        self.ec2_client.create_tags(Resources=cluster_id, Tags=cluster_tags.get(cluster_name))
-                    else:
-                        self.ec2_client.create_tags(Resources=cluster_id, Tags=cluster_tags.get(cluster_name))
+                    self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=cluster_id, tags=cluster_tags.get(cluster_name))
                     logger.info(f'{input_resource_id}:: {cluster_name}, count: {len(cluster_id)}, {cluster_id},  {cluster_tags.get(cluster_name)}')
                 except Exception as err:
                     logger.info(err)
             result_resources_list.extend(cluster_id)
         return sorted(result_resources_list)
 
     def __generate_cluster_resources_list_by_vpc(self, resources_list: list, input_resource_id: str):
@@ -170,20 +168,20 @@
                         all_tags = self.__check_name_in_tags(tags=all_tags, resource_id=resource_id)
                         all_tags = self.__filter_resource_tags_by_add_tags(resource.get('Tags'), all_tags)
                         cluster_tag = [tag for tag in vpc_data.get(vpc_id) if self.cluster_prefix in tag.get('Key')]
                         if all_tags:
                             if self.cluster_name:
                                 if self.cluster_name in cluster_tag[0].get('Key'):
                                     if self.dry_run == 'no':
-                                        self.ec2_client.create_tags(Resources=[resource_id], Tags=all_tags)
+                                        self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[resource_id],  tags=all_tags)
                                         logger.info(all_tags)
                                     result_resources_list.append(resource_id)
                             else:
                                 if self.dry_run == 'no':
-                                    self.ec2_client.create_tags(Resources=[resource_id], Tags=all_tags)
+                                    self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[resource_id], tags=all_tags)
                                     logger.info(all_tags)
                                 result_resources_list.append(resource_id)
                         break
         return sorted(result_resources_list)
 
     def __scan_resource_for_cluster_fullname(self, resources_list: list, tags: str = 'Tags'):
         """
@@ -225,51 +223,51 @@
 
     def __validate_existing_tag(self, tags: list):
         """
         This method validates that permanent tag exists in tags list
         @param tags:
         @return:
         """
+        check_tags = ['User', 'Project', 'Manager', 'Owner', 'Email']
         for tag in tags:
-            for key, value in self.input_tags.items():
-                if tag.get('Key') == key:
-                    return True
-        return False
+            if tag.get('Key') in check_tags:
+                if tag.get('Value') == 'NA':
+                    return False
+            else:
+                return False
+        return True
 
     def update_cluster_tags(self, resources: list):
         """
         This method update the Cluster instance tags and returns the updated tags list ids.
         @param resources:
         @param queue:
         @return:
         """
         cluster_instances = {}
         result_instance_list = []
         cluster_tags = {}
         for instance in resources:
             for item in instance:
                 instance_id = item['InstanceId']
-                if item.get('Tags'):
+                tags = item.get('Tags')
+                if tags:
                     # search that not exist permanent tags in the resource
-                    if not self.__validate_existing_tag(item.get('Tags')):
-                        for tag in item['Tags']:
+                    if not self.__validate_existing_tag(tags):
+                        for tag in tags:
                             if self.cluster_prefix in tag.get('Key'):
                                 add_tags = self.__append_input_tags()
                                 cluster_name = tag.get('Key').split('/')[-1]
                                 if cluster_name in cluster_instances:
-                                    add_tags = self.__filter_resource_tags_by_add_tags(tags=item.get('Tags'),
-                                                                                       search_tags=cluster_tags[
-                                                                                           cluster_name])
+                                    add_tags = self.__filter_resource_tags_by_add_tags(tags=tags, search_tags=cluster_tags[cluster_name])
                                     if add_tags:
                                         cluster_instances[cluster_name].append(instance_id)
                                     break
                                 else:
-                                    username = self._get_username_from_instance_id_and_time(
-                                        start_time=item.get('LaunchTime'), resource_id=instance_id,
-                                        resource_type='AWS::EC2::Instance')
+                                    username = self.get_username(start_time=item.get('LaunchTime'), resource_id=instance_id, resource_type='AWS::EC2::Instance', tags=tags)
                                     if username:
                                         if username == 'AutoScaling':
                                             add_tags.extend(self._fill_na_tags(user=username))
                                             logger.info(f'Autoscaling instance :: {instance_id}')
                                         else:
                                             user_tags = self.iam_operations.get_user_tags(username=username)
                                             if not self.__check_user_in_username_tags(user_tags):
@@ -296,19 +294,15 @@
                                     if add_tags:
                                         cluster_instances[cluster_name] = [instance_id]
                                         cluster_tags[cluster_name] = add_tags
                                     break
         for cluster_instance_name, instance_ids in cluster_instances.items():
             if self.dry_run == 'no':
                 try:
-                    if self.cluster_name:
-                        if cluster_instance_name == self.cluster_name:
-                            self.ec2_client.create_tags(Resources=instance_ids, Tags=cluster_tags.get(cluster_instance_name))
-                    else:
-                        self.ec2_client.create_tags(Resources=instance_ids, Tags=cluster_tags.get(cluster_instance_name))
+                    self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=instance_ids, tags=cluster_tags.get(cluster_instance_name))
                     logger.info(f'Cluster :: {cluster_instance_name} count: {len(instance_ids)} :: InstanceId :: {instance_ids} :: {cluster_tags.get(cluster_instance_name)}')
                 except Exception as err:
                     logger.info(err)
             result_instance_list.extend(instance_ids)
         logger.info(f'cluster_instance :: {len(result_instance_list)} :: {result_instance_list}')
         if not self.cluster_key:
             self.cluster_role(list(cluster_instances.keys()))
@@ -726,21 +720,30 @@
         @return:
         """
         add_tags = []
         if tags:
             for search_tag in search_tags:
                 found = False
                 for tag in tags:
-                    if tag.get('Key') == search_tag.get('Key'):
+                    if tag.get('Key') == search_tag.get('Key') and tag.get('Value') != 'NA':
                         found = True
+                        break
                 if not found:
                     add_tags.append(search_tag)
         else:
             add_tags.extend(search_tags)
-        return add_tags
+        filter_tags = {}
+        for tag in add_tags:
+            key = tag.get('Key')
+            value = tag.get('Value')
+            if key in filter_tags and filter_tags[key].get('Value') == self.NA_VALUE:
+                filter_tags[key] = {'Key': key, 'Value': value}
+            else:
+                filter_tags[key] = {'Key': key, 'Value': value}
+        return list(filter_tags.values())
 
     def __remove_launchTime(self, tags: list):
         """
         This method removes the launch time form the instance tags
         @param tags:
         @return:
         """
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 from cloud_governance.common.clouds.aws.ec2.ec2_operations import EC2Operations
 from cloud_governance.common.clouds.aws.iam.iam_operations import IAMOperations
 from cloud_governance.common.clouds.aws.utils.utils import Utils
 
 
 class NonClusterOperations:
 
+    NA_VALUE = 'NA'
+
     def __init__(self, region: str = 'us-east-2', dry_run: str = 'yes', input_tags: dict = ''):
         self.region = region
         self.dry_run = dry_run
         self.input_tags = input_tags
         self.cloudtrail = boto3.client('cloudtrail', region_name=region)
         self.cluster_prefix = 'kubernetes.io/cluster/'
         self.ec2_client = boto3.client('ec2', region_name=region)
         self.cloudtrail = CloudTrailOperations(region_name=self.region)
         self.iam_client = IAMOperations()
         self.ec2_operations = EC2Operations(region=region)
         self.utils = Utils(region=region)
+        self.iam_users = self.iam_client.get_iam_users_list()
 
     def _get_instances_data(self, instance_id: str = ''):
         """
         This method go over all instances
         :return:
         """
         ec2s_data = self.ec2_operations.get_instances()
@@ -59,21 +62,29 @@
         @return:
         """
         add_tags = []
         if tags:
             for search_tag in search_tags:
                 found = False
                 for tag in tags:
-                    if tag.get('Key') == search_tag.get('Key'):
+                    if tag.get('Key') == search_tag.get('Key') and tag.get('Value') != 'NA':
                         found = True
                 if not found:
                     add_tags.append(search_tag)
         else:
             add_tags.extend(search_tags)
-        return add_tags
+        filter_tags = {}
+        for tag in add_tags:
+            key = tag.get('Key')
+            value = tag.get('Value')
+            if key in filter_tags and filter_tags[key].get('Value') == self.NA_VALUE:
+                filter_tags[key] = {'Key': key, 'Value': value}
+            else:
+                filter_tags[key] = {'Key': key, 'Value': value}
+        return list(filter_tags.values())
 
     def _fill_na_tags(self, user: str = None):
         """
         This method fill NA tags
         @param user:
         @return:
         """
@@ -179,8 +190,31 @@
                             [tag for tag in image.get('Tags') if not tag.get('Key') == "Name"])
                     else:
                         tags.extend(self._append_input_tags())
                     start_time = datetime.fromisoformat(image.get('CreationDate')[:-1] + '+00:00')
                     username = self._get_username_from_cloudtrail(start_time=start_time, resource_id=image_id, resource_type='AWS::EC2::Ami')
         return tags, username
 
+    def get_user_name_from_name_tag(self, tags: list = None, resource_name: str = None):
+        """
+        This method retuns the username from the name tag verified  with iam users
+        :param resource_name:
+        :param tags:
+        :return:
+        """
+        name_tag = self.ec2_operations.get_tag_value_from_tags(tags=tags, tag_name='Name') if tags else resource_name
+        for user in self.iam_users:
+            if user in name_tag:
+                return user
+        return None
 
+    def get_username(self, start_time: datetime, resource_id: str, resource_type: str, tags: list, resource_name: str = ''):
+        """
+        This method returns the username
+        :return:
+        """
+        iam_username = self.get_user_name_from_name_tag(tags=tags, resource_name=resource_name)
+        if not iam_username:
+            iam_username = self.get_user_name_from_name_tag(resource_name=resource_name)
+            if not iam_username:
+                return self._get_username_from_cloudtrail(start_time=start_time, resource_id=resource_id, resource_type=resource_type)
+        return iam_username
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         """
         This method returns the tags to update  the instance tags
         @param launch_time:
         @param instance_id:
         @param tags:
         @return:
         """
-        username = self._get_username_from_cloudtrail(start_time=launch_time, resource_id=instance_id, resource_type='AWS::EC2::Instance')
+        username = self.get_username(start_time=launch_time, resource_id=instance_id, resource_type='AWS::EC2::Instance', tags=tags)
         search_tags = []
         user_tags = []
         if not username:
             search_tags.extend(self._fill_na_tags())
         else:
             search_tags.append(self._build_tag(key='Email', value=f'{username}@redhat.com'))
             user_tags = self.iam_client.get_user_tags(username=username)
@@ -67,15 +67,15 @@
             for item in instance:
                 instance_id = item.get('InstanceId')
                 launch_time = item.get('LaunchTime')
                 add_tags = self.__get_instance_tags(launch_time=launch_time, instance_id=instance_id, tags=item.get('Tags'))
                 if add_tags:
                     if self.dry_run == 'no':
                         try:
-                            self.ec2_client.create_tags(Resources=[instance_id], Tags=add_tags)
+                            self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[instance_id], tags=add_tags)
                             logger.info(f'Added tags to instance: {instance_id} total: {len(add_tags)} tags: {add_tags}')
                         except Exception as err:
                             logger.info(err)
                     instances_ids.append(instance_id)
         logger.info(f'non_cluster_ec2 count: {len(sorted(instances_ids))} {sorted(instances_ids)}')
         return sorted(instances_ids)
 
@@ -86,15 +86,16 @@
         @return:
         """
         if not volumes_data:
             volumes_data = self._get_resource_data(resource_method=self.ec2_operations.get_volumes)
         volume_ids = []
         for volume in volumes_data:
             volume_id = volume.get('VolumeId')
-            username = self._get_username_from_cloudtrail(start_time=volume.get('CreateTime'), resource_id=volume_id, resource_type='AWS::EC2::Volume')
+            tags = volume.get('Tags')
+            username = self.get_username(start_time=volume.get('CreateTime'), resource_id=volume_id, resource_type='AWS::EC2::Volume', tags=tags)
             search_tags = []
             if not username:
                 get_tags, username = self._get_tags_fom_attachments(attachments=volume.get('Attachments'))
                 search_tags.extend(get_tags)
             else:
                 search_tags.extend(self._append_input_tags())
             if username:
@@ -112,15 +113,15 @@
             if not self.__check_name_in_tags(volume.get('Tags')):
                 tag_name = f'{username}-{volume_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{volume_id[:self.SHORT_RESOURCE_NAME]}-{self.region}-{volume_id[-self.SHORT_RESOURCE_ID:]}'
                 search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
             volume_tags = self._get_tags_of_resources(tags=volume.get('Tags'), search_tags=search_tags)
             if volume_tags:
                 if self.dry_run == 'no':
                     try:
-                        self.ec2_client.create_tags(Resources=[volume_id], Tags=volume_tags)
+                        self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[volume_id], tags=volume_tags)
                         logger.info(f'added tags to volume_id: {volume_id} total: {len(volume_tags)}  tags: {volume_tags}')
                     except Exception as err:
                         logger.info(err)
                 volume_ids.append(volume_id)
         logger.info(f'non_cluster_volumes count: {len(sorted(volume_ids))} {sorted(volume_ids)}')
         return sorted(volume_ids)
 
@@ -131,15 +132,16 @@
         @return:
         """
         if not snapshots:
             snapshots = self._get_resource_data(resource_method=self.ec2_operations.get_snapshots)
         snapshot_ids = []
         for snapshot in snapshots:
             snapshot_id = snapshot.get('SnapshotId')
-            username = self._get_username_from_cloudtrail(start_time=snapshot.get('StartTime'), resource_id=snapshot_id, resource_type='AWS::EC2::Snapshot')
+            tags = snapshot.get('Tags')
+            username = self.get_username(start_time=snapshot.get('StartTime'), resource_id=snapshot_id, resource_type='AWS::EC2::Snapshot', tags=tags)
             search_tags = []
             if not username:
                 if snapshot.get('Description') and 'Created' in snapshot.get('Description'):
                     image_tags, username = self._get_tags_from_snapshot_description_images(description=snapshot.get('Description'))
                     if not username:
                         instance_id = snapshot.get('Description').split(" ")[2].split("(")[1][:-1]
                         instances = self._get_instances_data(instance_id)
@@ -163,15 +165,15 @@
                 tag_name = f'{username}-{snapshot_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{snapshot_id[:self.SHOT_SNAPSHOT_ID]}-{self.region}-{snapshot_id[-self.SHORT_RESOURCE_ID:]}'
                 search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
             search_tags.append(self._build_tag(key='LaunchTime', value=snapshot.get('StartTime')))
             snapshot_tags = self._get_tags_of_resources(tags=snapshot.get('Tags'), search_tags=search_tags)
             if snapshot_tags:
                 if self.dry_run == 'no':
                     try:
-                        self.ec2_client.create_tags(Resources=[snapshot_id], Tags=snapshot_tags)
+                        self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[snapshot_id], tags=snapshot_tags)
                         logger.info(f'added tags to snapshots: {snapshot_id} total: {len(snapshot_tags)} tags: {snapshot_tags}')
                     except Exception as err:
                         logger.info(err)
                 snapshot_ids.append(snapshot_id)
         logger.info(f'non_cluster_snapshot count: {len(sorted(snapshot_ids))} {sorted(snapshot_ids)}')
         return sorted(snapshot_ids)
 
@@ -183,16 +185,18 @@
         """
         if not images:
             images = self.ec2_operations.get_images()
             _, images = self.ec2_operations.scan_cluster_non_cluster_resources(images)
         image_ids = []
         for image in images:
             image_id = image.get('ImageId')
+            tags = image.get('Tags')
+            image_name = image.get('Name')
             start_time = datetime.fromisoformat(image.get('CreationDate')[:-1] + '+00:00')
-            username = self._get_username_from_cloudtrail(start_time=start_time, resource_id=image_id, resource_type='AWS::EC2::Ami')
+            username = self.get_username(start_time=start_time, resource_id=image_id, resource_type='AWS::EC2::Ami', tags=tags, resource_name=image_name)
             search_tags = []
             search_tags.extend(self._append_input_tags())
             if username:
                 user_tags = self.iam_client.get_user_tags(username=username)
                 search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
                 if not user_tags:
                     search_tags.extend(self._fill_na_tags(user=username))
@@ -204,14 +208,14 @@
                 tag_name = f'{username}-{image_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{image_id[:self.SHORT_RESOURCE_NAME]}-{self.region}-{image_id[-self.SHORT_RESOURCE_ID:]}'
                 search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
             search_tags.append(self._build_tag(key='LaunchTime', value=start_time))
             image_tags = self._get_tags_of_resources(tags=image.get('Tags'), search_tags=search_tags)
             if image_tags:
                 if self.dry_run == 'no':
                     try:
-                        self.ec2_client.create_tags(Resources=[image_id], Tags=image_tags)
+                        self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[image_id], tags=image_tags)
                         logger.info(f'added tags to image: {image_id} total: {len(image_tags)} tags: {image_tags}')
                     except Exception as err:
                         logger.info(err)
                 image_ids.append(image_id)
         logger.info(f'non_cluster_amis count: {len(sorted(image_ids))} {sorted(image_ids)}')
         return sorted(image_ids)
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -161,16 +161,17 @@
                                     logger.info(f'delete_load_balancer: {resource_id}')
                                 except Exception as err:
                                     logger.exception(f'Cannot delete_load_balancer: {resource_id}, {err}')
 
     @typeguard.typechecked
     def __delete_volume(self, resource_id: str):
         try:
-            self.client.delete_volume(VolumeId=resource_id)
-            logger.info(f'delete_volume: {resource_id}')
+            logger.info(f'Cluster volumes are handled by ebs_unattached')
+            # self.client.delete_volume(VolumeId=resource_id)
+            # logger.info(f'delete_volume: {resource_id}')
         except Exception as err:
             logger.exception(f'Cannot delete_volume: {resource_id}, {err}')
 
     @typeguard.typechecked
     def __delete_snapshots(self, resource_id: str):
         try:
             self.client.delete_snapshot(SnapshotId=resource_id)
@@ -256,30 +257,39 @@
         :param resource_id:
         :return:
         """
         try:
             security_groups = self.ec2_operations.get_security_groups()
             vpc_security_groups = self.__get_cluster_references(resource_id=vpc_id, resource_list=security_groups, input_resource_id='VpcId', output_result='')
             for vpc_security_group in vpc_security_groups:
-                if vpc_security_group.get('GroupName') == 'default':
-                    if vpc_security_group.get('IpPermissions'):
-                        for ip_permission in vpc_security_group.get('IpPermissions'):
-                            self.client.revoke_security_group_ingress(GroupId=vpc_security_group.get('GroupId'), IpPermissions=[ip_permission])
-                            logger.info(f'Removed the Ingress rules of Security Group {resource_id} :: {ip_permission}')
-                else:
-                    if vpc_security_group.get('Tags'):
-                        if self.__is_cluster_resource(tags=vpc_security_group.get('Tags'), cluster_tag=self.cluster_tag):
-                            logger.info(vpc_security_group.get('GroupId'))
-                            if vpc_security_group.get('IpPermissions'):
-                                for ip_permission in vpc_security_group.get('IpPermissions'):
-                                    if ip_permission.get('UserIdGroupPairs'):
-                                        for user_id_group_pair in ip_permission.get('UserIdGroupPairs'):
-                                            if user_id_group_pair.get('GroupId') == resource_id:
-                                                self.client.revoke_security_group_ingress(GroupId=vpc_security_group.get('GroupId'), IpPermissions=[ip_permission])
-                                                logger.info(f'Removed the Ingress rules of Security Group {resource_id} from {vpc_security_group.get("GroupId")}')
+                if resource_id != vpc_security_group.get('GroupId'):
+                    if vpc_security_group.get('GroupName') == 'default':
+                        logger.info(f'Removing the {resource_id} ingress rule from Default Security Group: {vpc_security_group.get("GroupId")}')
+                        if vpc_security_group.get('IpPermissions'):
+                            for ip_permission in vpc_security_group.get('IpPermissions'):
+                                if ip_permission.get('UserIdGroupPairs'):
+                                    for user_id_group_pair in ip_permission.get('UserIdGroupPairs'):
+                                        if user_id_group_pair.get('GroupId') == resource_id:
+                                            ingress_rule = {'FromPort': ip_permission.get('FromPort'), 'IpProtocol': ip_permission.get('IpProtocol'), 'IpRanges': ip_permission.get('IpRanges'), 'Ipv6Ranges': ip_permission.get('Ipv6Ranges'), 'PrefixListIds': ip_permission.get('PrefixListIds'), 'ToPort': ip_permission.get('ToPort'), 'UserIdGroupPairs': [user_id_group_pair]}
+                                            self.client.revoke_security_group_ingress(GroupId=vpc_security_group.get('GroupId'), IpPermissions=[ingress_rule])
+                                            logger.info(f'Removed the Ingress rules of Security Group {vpc_security_group.get("GroupId")} :: {ingress_rule}')
+                    else:
+                        if vpc_security_group.get('Tags'):
+                            if self.__is_cluster_resource(tags=vpc_security_group.get('Tags'), cluster_tag=self.cluster_tag):
+                                logger.info(vpc_security_group.get('GroupId'))
+                                if vpc_security_group.get('IpPermissions'):
+                                    for ip_permission in vpc_security_group.get('IpPermissions'):
+                                        if ip_permission.get('UserIdGroupPairs'):
+                                            for user_id_group_pair in ip_permission.get('UserIdGroupPairs'):
+                                                if user_id_group_pair.get('GroupId') == resource_id:
+                                                    ingress_rule = {'FromPort': ip_permission.get('FromPort'), 'IpProtocol': ip_permission.get('IpProtocol'), 'IpRanges': ip_permission.get('IpRanges'),
+                                                                    'Ipv6Ranges': ip_permission.get('Ipv6Ranges'), 'PrefixListIds': ip_permission.get('PrefixListIds'),
+                                                                    'ToPort': ip_permission.get('ToPort'), 'UserIdGroupPairs': [user_id_group_pair]}
+                                                    self.client.revoke_security_group_ingress(GroupId=vpc_security_group.get('GroupId'), IpPermissions=[ingress_rule])
+                                                    logger.info(f'Removed the Ingress rules of Security Group {resource_id} from {ingress_rule}')
             network_interfaces = self.ec2_operations.get_network_interface()
             network_interface_ids = self.__get_cluster_references(resource_id=vpc_id, resource_list=network_interfaces,
                                                                   input_resource_id='VpcId',
                                                                   output_result='')
             default_security_group_id = [security_group.get('GroupId') for security_group in vpc_security_groups
                                          if security_group.get('GroupName') == 'default']
             if default_security_group_id:
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         self.elbv2_client = boto3.client('elbv2', region_name=region)
         self.iam_client = boto3.client('iam', region_name=region)
         self.s3_client = boto3.client('s3')
         self.s3_resource = boto3.resource('s3')
         self.__ldap_host_name = self.__environment_variables_dict.get('LDAP_HOST_NAME', '')
         self._special_user_mails = self.__environment_variables_dict.get('special_user_mails', '{}')
         self._account_admin = self.__environment_variables_dict.get('account_admin', '')
+        self.__email_alert = self.__environment_variables_dict.get('EMAIL_ALERT') if self.__environment_variables_dict.get('EMAIL_ALERT') else False
         self._ldap = LdapSearch(ldap_host_name=self.__ldap_host_name)
         self._mail = Postfix()
         self._mail_description = MailMessage()
         self._force_delete = self.__environment_variables_dict.get('FORCE_DELETE') if self.__environment_variables_dict.get('FORCE_DELETE') else force_delete
 
     def _literal_eval(self, data: any):
         tags = {}
@@ -259,23 +260,24 @@
         """
         This method send mail to the user to notify cluster status
         @param cluster_data:
         @param notify_data:
         @param delete_data:
         @return:
         """
-        for cluster_tag, resource_ids in notify_data.items():
-            self.update_resource_tags(tags=cluster_data[cluster_tag], tag_name='Name', tag_value=cluster_tag)
-            self.trigger_mail(tags=cluster_data[cluster_tag], resource_id=cluster_tag,
-                              days=self.DAYS_TO_TRIGGER_RESOURCE_MAIL,
-                              resources=resource_ids, message_type='notification')
-        for cluster_tag, resource_ids in delete_data.items():
-            self.update_resource_tags(tags=cluster_data[cluster_tag], tag_name='Name', tag_value=cluster_tag)
-            self.trigger_mail(tags=cluster_data[cluster_tag], resource_id=cluster_tag,
-                              days=self.DAYS_TO_DELETE_RESOURCE, resources=resource_ids, message_type='delete')
+        if self.__email_alert:
+            for cluster_tag, resource_ids in notify_data.items():
+                self.update_resource_tags(tags=cluster_data[cluster_tag], tag_name='Name', tag_value=cluster_tag)
+                self.trigger_mail(tags=cluster_data[cluster_tag], resource_id=cluster_tag,
+                                  days=self.DAYS_TO_TRIGGER_RESOURCE_MAIL,
+                                  resources=resource_ids, message_type='notification')
+            for cluster_tag, resource_ids in delete_data.items():
+                self.update_resource_tags(tags=cluster_data[cluster_tag], tag_name='Name', tag_value=cluster_tag)
+                self.trigger_mail(tags=cluster_data[cluster_tag], resource_id=cluster_tag,
+                                  days=self.DAYS_TO_DELETE_RESOURCE, resources=resource_ids, message_type='delete')
 
     @logger_time_stamp
     def _check_zombie_cluster_deleted_days(self, resources: dict, cluster_left_out_days: dict, zombie: str, cluster_tag: str):
         """
         This method check the cluster delete days and return the clusters
         @param resources:
         @param cluster_left_out_days:
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,16 @@
         self._cloudtrail = CloudTrailOperations(region_name=self._region)
         self._special_user_mails = self.__environment_variables_dict.get('special_user_mails', '{}')
         self._account_admin = self.__environment_variables_dict.get('account_admin', '')
         self._mail = Postfix()
         self._mail_description = MailMessage()
         self.__ldap_host_name = self.__environment_variables_dict.get('LDAP_HOST_NAME', '')
         self._ldap = LdapSearch(ldap_host_name=self.__ldap_host_name)
+        self.__email_alert = self.__environment_variables_dict.get('EMAIL_ALERT') if self.__environment_variables_dict.get('EMAIL_ALERT') else False
+        self.__manager_email_alert = self.__environment_variables_dict.get('MANAGER_EMAIL_ALERT')
         self._admins = ['athiruma@redhat.com', 'ebattat@redhat.com']
         self._es_upload = ElasticUpload()
         self.resource_pricing = ResourcesPricing()
 
     def set_dryrun(self, value: str):
         self._dry_run = value
 
@@ -160,38 +162,40 @@
     def _trigger_mail(self, tags: list, resource_id: str, days: int, resource_type: str, **kwargs):
         """
         This method send triggering mail
         @param tags:
         @param resource_id:
         @return:
         """
-        try:
-            special_user_mails = self._literal_eval(self._special_user_mails)
-            user, resource_name = self._get_tag_name_from_tags(tags=tags, tag_name='User'), self._get_tag_name_from_tags(
-                tags=tags, tag_name='Name')
-            if not resource_name:
-                resource_name = self._get_tag_name_from_tags(tags=tags, tag_name='cg-Name')
-            to = user if user not in special_user_mails else special_user_mails[user]
-            ldap_data = self._ldap.get_user_details(user_name=to)
-            cc = [self._account_admin, f'{ldap_data.get("managerId")}@redhat.com']
-            name = to
-            if ldap_data:
-                name = ldap_data.get('displayName')
-            subject, body = self._mail_description.resource_message(name=name, days=days,
-                                                                    notification_days=self.DAYS_TO_TRIGGER_RESOURCE_MAIL,
-                                                                    delete_days=self.DAYS_TO_DELETE_RESOURCE,
-                                                                    resource_name=resource_name, resource_id=resource_id,
-                                                                    resource_type=resource_type, msgadmins=self.DAYS_TO_NOTIFY_ADMINS, extra_purse=kwargs.get('extra_purse'))
-            if not kwargs.get('admins'):
-                self._mail.send_email_postfix(to=to, content=body, subject=subject, cc=cc, resource_id=resource_id, message_type=kwargs.get('message_type'), extra_purse=kwargs.get('delta_cost', 0))
-            else:
-                kwargs['admins'].append(f'{ldap_data.get("managerId")}@redhat.com')
-                self._mail.send_email_postfix(to=kwargs.get('admins'), content=body, subject=subject, cc=[], resource_id=resource_id, message_type=kwargs.get('message_type'), extra_purse=kwargs.get('delta_cost', 0))
-        except Exception as err:
-            logger.info(err)
+        if self.__email_alert:
+            try:
+                special_user_mails = self._literal_eval(self._special_user_mails)
+                user, resource_name = self._get_tag_name_from_tags(tags=tags, tag_name='User'), self._get_tag_name_from_tags(
+                    tags=tags, tag_name='Name')
+                if not resource_name:
+                    resource_name = self._get_tag_name_from_tags(tags=tags, tag_name='cg-Name')
+                to = user if user not in special_user_mails else special_user_mails[user]
+                ldap_data = self._ldap.get_user_details(user_name=to)
+                cc = [self._account_admin, f'{ldap_data.get("managerId")}@redhat.com'] if self.__manager_email_alert else []
+                name = to
+                if ldap_data:
+                    name = ldap_data.get('displayName')
+                subject, body = self._mail_description.resource_message(name=name, days=days,
+                                                                        notification_days=self.DAYS_TO_TRIGGER_RESOURCE_MAIL,
+                                                                        delete_days=self.DAYS_TO_DELETE_RESOURCE,
+                                                                        resource_name=resource_name, resource_id=resource_id,
+                                                                        resource_type=resource_type, msgadmins=self.DAYS_TO_NOTIFY_ADMINS, extra_purse=kwargs.get('extra_purse'))
+                if not kwargs.get('admins'):
+                    self._mail.send_email_postfix(to=to, content=body, subject=subject, cc=cc, resource_id=resource_id, message_type=kwargs.get('message_type'), extra_purse=kwargs.get('delta_cost', 0))
+                else:
+                    if self.__manager_email_alert:
+                        kwargs['admins'].append(f'{ldap_data.get("managerId")}@redhat.com')
+                    self._mail.send_email_postfix(to=kwargs.get('admins'), content=body, subject=subject, cc=[], resource_id=resource_id, message_type=kwargs.get('message_type'), extra_purse=kwargs.get('delta_cost', 0))
+            except Exception as err:
+                logger.info(err)
 
     def _update_tag_value(self, tags: list, tag_name: str, tag_value: str):
         """
         This method updates the tag value
         @param tags:
         @param tag_name:
         @param tag_value:
```

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py` & `athiru-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py`

 * *Files identical despite different names*

### Comparing `athiru-cloud-governance-1.1.76/setup.py` & `athiru-cloud-governance-1.1.89/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from codecs import open
 from os import path
 from setuptools import setup, find_packages
 
 
-__version__ = '1.1.76'
+__version__ = '1.1.89'
 
 
 here = path.abspath(path.dirname(__file__))
 
 
 if path.isfile(path.join(here, 'README.md')):
     with open(path.join(here, 'README.md'), encoding='utf-8') as f:
@@ -49,14 +49,16 @@
         'botocore==1.29.1',  # required by c7n 0.9.14
         'boto3==1.26.1',  # required by c7n 0.9.14
         'elasticsearch==7.11.0',  # depend on elasticsearch server
         'elasticsearch-dsl==7.4.0',
         'google-api-python-client==2.57.0',  # google drive
         'google-auth-httplib2==0.1.0',  # google drive
         'google-auth-oauthlib==0.5.2',  # google drive
+        'google-cloud-billing==1.9.1',  # google cloud cost
+        'google-cloud-bigquery==3.5.0',  # google cloud cost
         'ibm_platform_services==0.27.0',  # IBM Usage reports
         'myst-parser==0.17.0',  # readthedocs
         'pandas',  # latest: aggregate ec2/ebs cluster data
         'PyGitHub==1.55',  # gitleaks
         'python-ldap==3.4.2',  # prerequisite: sudo dnf install -y python39-devel openldap-devel gcc
         'requests==2.27.1',  # rest api & lambda
         'retry==0.9.2',
```

