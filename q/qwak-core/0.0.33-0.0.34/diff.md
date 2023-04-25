# Comparing `tmp/qwak_core-0.0.33.tar.gz` & `tmp/qwak_core-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.33.tar", max compression
+gzip compressed data, was "qwak_core-0.0.34.tar", max compression
```

## Comparing `qwak_core-0.0.33.tar` & `qwak_core-0.0.34.tar`

### file list

```diff
@@ -1,535 +1,535 @@
--rw-r--r--   0        0        0      264 2023-04-25 06:05:59.163818 qwak_core-0.0.33/README.md
--rw-r--r--   0        0        0        0 2023-04-25 06:07:00.392258 qwak_core-0.0.33/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-04-25 06:07:00.416258 qwak_core-0.0.33/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-04-25 06:06:40.936117 qwak_core-0.0.33/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.416258 qwak_core-0.0.33/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-04-25 06:07:00.412258 qwak_core-0.0.33/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-04-25 06:06:40.584114 qwak_core-0.0.33/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.412258 qwak_core-0.0.33/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-04-25 06:07:00.412258 qwak_core-0.0.33/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-04-25 06:06:40.760116 qwak_core-0.0.33/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.416258 qwak_core-0.0.33/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-04-25 06:07:00.404258 qwak_core-0.0.33/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-04-25 06:06:40.056111 qwak_core-0.0.33/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-04-25 06:07:00.408258 qwak_core-0.0.33/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-04-25 06:07:00.408258 qwak_core-0.0.33/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-04-25 06:06:40.228112 qwak_core-0.0.33/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.408258 qwak_core-0.0.33/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-04-25 06:07:00.408258 qwak_core-0.0.33/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-04-25 06:06:40.404113 qwak_core-0.0.33/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.412258 qwak_core-0.0.33/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-04-25 06:07:00.392258 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-04-25 06:06:39.856109 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-04-25 06:07:00.392258 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-04-25 06:07:00.396258 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-04-25 06:06:41.116118 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.396258 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-04-25 06:07:00.400258 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-04-25 06:06:41.472121 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.400258 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-04-25 06:07:00.400258 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-04-25 06:06:41.652122 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-04-25 06:07:00.400258 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-04-25 06:07:00.396258 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-04-25 06:06:41.292119 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.396258 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-04-25 06:07:00.404258 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-04-25 06:06:41.832123 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.404258 qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-04-25 06:07:00.448258 qwak_core-0.0.33/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-04-25 06:06:44.332141 qwak_core-0.0.33/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.448258 qwak_core-0.0.33/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-04-25 06:07:00.448258 qwak_core-0.0.33/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-04-25 06:06:44.512142 qwak_core-0.0.33/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-04-25 06:07:00.452258 qwak_core-0.0.33/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-04-25 06:07:00.516259 qwak_core-0.0.33/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-04-25 06:06:49.380180 qwak_core-0.0.33/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.516259 qwak_core-0.0.33/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-04-25 06:07:00.516259 qwak_core-0.0.33/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-04-25 06:06:49.560181 qwak_core-0.0.33/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-04-25 06:07:00.520259 qwak_core-0.0.33/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-04-25 06:07:00.520259 qwak_core-0.0.33/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-04-25 06:06:50.464188 qwak_core-0.0.33/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-04-25 06:07:00.524259 qwak_core-0.0.33/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-04-25 06:07:00.520259 qwak_core-0.0.33/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-04-25 06:06:50.284187 qwak_core-0.0.33/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.520259 qwak_core-0.0.33/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-04-25 06:07:00.524259 qwak_core-0.0.33/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-04-25 06:06:50.652190 qwak_core-0.0.33/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.524259 qwak_core-0.0.33/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-04-25 06:07:00.524259 qwak_core-0.0.33/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-04-25 06:06:50.836191 qwak_core-0.0.33/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-04-25 06:07:00.528259 qwak_core-0.0.33/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    11441 2023-04-25 06:07:00.588260 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    17892 2023-04-25 06:06:55.964227 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.588260 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-04-25 06:07:00.584259 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-04-25 06:06:55.612225 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.584259 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-04-25 06:07:00.584259 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-04-25 06:06:55.788226 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.588260 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-04-25 06:07:00.580259 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-04-25 06:06:55.248222 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-04-25 06:07:00.580259 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-04-25 06:07:00.580259 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-04-25 06:06:55.432223 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.584259 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-04-25 06:07:00.592260 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-04-25 06:06:56.492231 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.596259 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-04-25 06:07:00.592260 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-04-25 06:06:56.316230 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.592260 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     3604 2023-04-25 06:07:00.588260 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4212 2023-04-25 06:06:56.140228 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.592260 qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-04-25 06:07:00.632260 qwak_core-0.0.33/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-04-25 06:06:59.752254 qwak_core-0.0.33/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.636260 qwak_core-0.0.33/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-04-25 06:07:00.628260 qwak_core-0.0.33/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-04-25 06:06:59.376251 qwak_core-0.0.33/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.628260 qwak_core-0.0.33/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    37419 2023-04-25 06:07:00.632260 qwak_core-0.0.33/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    48027 2023-04-25 06:06:59.568252 qwak_core-0.0.33/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-04-25 06:07:00.632260 qwak_core-0.0.33/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-04-25 06:07:00.552259 qwak_core-0.0.33/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-04-25 06:06:52.660204 qwak_core-0.0.33/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-04-25 06:07:00.552259 qwak_core-0.0.33/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-04-25 06:07:00.552259 qwak_core-0.0.33/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-04-25 06:06:52.476203 qwak_core-0.0.33/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.552259 qwak_core-0.0.33/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-04-25 06:07:00.540259 qwak_core-0.0.33/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-04-25 06:06:52.120200 qwak_core-0.0.33/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.544259 qwak_core-0.0.33/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-04-25 06:07:00.544259 qwak_core-0.0.33/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-04-25 06:06:52.296202 qwak_core-0.0.33/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.544259 qwak_core-0.0.33/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-04-25 06:07:00.544259 qwak_core-0.0.33/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-04-25 06:06:52.840205 qwak_core-0.0.33/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-04-25 06:07:00.548259 qwak_core-0.0.33/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-04-25 06:07:00.548259 qwak_core-0.0.33/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-04-25 06:06:53.224208 qwak_core-0.0.33/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-04-25 06:07:00.548259 qwak_core-0.0.33/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-04-25 06:07:00.560259 qwak_core-0.0.33/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-04-25 06:06:53.604211 qwak_core-0.0.33/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.560259 qwak_core-0.0.33/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-04-25 06:07:00.560259 qwak_core-0.0.33/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-04-25 06:06:53.780212 qwak_core-0.0.33/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-04-25 06:07:00.564259 qwak_core-0.0.33/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-04-25 06:07:00.536259 qwak_core-0.0.33/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-04-25 06:06:51.584197 qwak_core-0.0.33/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.536259 qwak_core-0.0.33/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-04-25 06:07:00.536259 qwak_core-0.0.33/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-04-25 06:06:51.760198 qwak_core-0.0.33/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-04-25 06:07:00.540259 qwak_core-0.0.33/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-04-25 06:07:00.532259 qwak_core-0.0.33/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-04-25 06:06:51.216194 qwak_core-0.0.33/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.532259 qwak_core-0.0.33/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    42956 2023-04-25 06:07:00.528259 qwak_core-0.0.33/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    62847 2023-04-25 06:06:51.032193 qwak_core-0.0.33/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.528259 qwak_core-0.0.33/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-04-25 06:07:00.532259 qwak_core-0.0.33/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-04-25 06:06:51.404195 qwak_core-0.0.33/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-04-25 06:07:00.532259 qwak_core-0.0.33/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-04-25 06:07:00.436258 qwak_core-0.0.33/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-04-25 06:06:43.436134 qwak_core-0.0.33/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.436258 qwak_core-0.0.33/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-04-25 06:07:00.440258 qwak_core-0.0.33/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-04-25 06:06:43.616136 qwak_core-0.0.33/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.440258 qwak_core-0.0.33/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-04-25 06:07:00.440258 qwak_core-0.0.33/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-04-25 06:06:43.800137 qwak_core-0.0.33/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-04-25 06:07:00.440258 qwak_core-0.0.33/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-04-25 06:07:00.496259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-04-25 06:06:48.312172 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.496259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-04-25 06:07:00.492259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-04-25 06:06:48.136170 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-04-25 06:07:00.496259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-04-25 06:07:00.476259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-04-25 06:06:46.692159 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.476259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-04-25 06:07:00.472259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-04-25 06:06:46.512158 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.476259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-04-25 06:07:00.468259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-04-25 06:06:45.960153 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.468259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    27847 2023-04-25 06:07:00.472259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20073 2023-04-25 06:06:46.332156 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    33080 2023-04-25 06:07:00.472259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-04-25 06:07:00.476259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-04-25 06:06:46.876160 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.480259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-04-25 06:07:00.480259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-04-25 06:06:47.056162 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-04-25 06:07:00.480259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    24876 2023-04-25 06:07:00.468259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    36861 2023-04-25 06:06:46.144155 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.468259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-04-25 06:07:00.484259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-04-25 06:06:47.232163 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.484259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-04-25 06:07:00.496259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-04-25 06:06:59.932255 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.500259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-04-25 06:07:00.500259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-04-25 06:07:00.120256 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-04-25 06:07:00.500259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-04-25 06:07:00.500259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-04-25 06:06:48.844176 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.504259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-04-25 06:07:00.504259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-04-25 06:06:49.024177 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-04-25 06:07:00.504259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-04-25 06:07:00.508259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-04-25 06:06:49.200178 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.508259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-04-25 06:07:00.512259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-04-25 06:06:49.924184 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.512259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-04-25 06:07:00.508259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-04-25 06:06:49.740182 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-04-25 06:07:00.508259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-04-25 06:07:00.512259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-04-25 06:06:50.104185 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.516259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    13329 2023-04-25 06:07:00.484259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23039 2023-04-25 06:06:47.416164 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.484259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-04-25 06:07:00.488259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-04-25 06:06:47.596166 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.488259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-04-25 06:07:00.488259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-04-25 06:06:47.776167 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-04-25 06:07:00.488259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-04-25 06:07:00.492259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-04-25 06:06:47.956169 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.492259 qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-04-25 06:07:00.596259 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-04-25 06:06:56.668232 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.596259 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-04-25 06:07:00.600260 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-04-25 06:06:56.844233 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-04-25 06:07:00.600260 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-04-25 06:07:00.600260 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-04-25 06:06:57.020234 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.600260 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-04-25 06:07:00.604260 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-04-25 06:06:57.200236 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-04-25 06:07:00.604260 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-04-25 06:07:00.604260 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-04-25 06:06:57.384237 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-04-25 06:07:00.604260 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-04-25 06:07:00.608260 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-04-25 06:06:57.560238 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.608260 qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-04-25 06:07:00.564259 qwak_core-0.0.33/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-04-25 06:06:53.960213 qwak_core-0.0.33/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.564259 qwak_core-0.0.33/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-04-25 06:07:00.564259 qwak_core-0.0.33/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-04-25 06:06:54.136214 qwak_core-0.0.33/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-04-25 06:07:00.568259 qwak_core-0.0.33/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-04-25 06:07:00.452258 qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-04-25 06:06:45.240148 qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.456259 qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-04-25 06:07:00.456259 qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-04-25 06:06:45.416149 qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.456259 qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-04-25 06:07:00.460259 qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-04-25 06:06:45.596150 qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-04-25 06:07:00.460259 qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-04-25 06:07:00.464259 qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-04-25 06:06:45.772152 qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.464259 qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-04-25 06:07:00.540259 qwak_core-0.0.33/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-04-25 06:06:51.940199 qwak_core-0.0.33/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-04-25 06:07:00.540259 qwak_core-0.0.33/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-04-25 06:07:00.608260 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-04-25 06:06:57.740239 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.612260 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-04-25 06:07:00.612260 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-04-25 06:06:57.916241 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.612260 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-04-25 06:07:00.612260 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-04-25 06:06:58.096242 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.616260 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-04-25 06:07:00.616260 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-04-25 06:06:58.280243 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.616260 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-04-25 06:07:00.616260 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-04-25 06:06:58.464245 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.620260 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-04-25 06:07:00.620260 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-04-25 06:06:58.660246 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-04-25 06:07:00.620260 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-04-25 06:07:00.624260 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-04-25 06:06:58.840247 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.624260 qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-04-25 06:07:00.572259 qwak_core-0.0.33/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-04-25 06:06:54.500217 qwak_core-0.0.33/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.572259 qwak_core-0.0.33/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-04-25 06:07:00.576259 qwak_core-0.0.33/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-04-25 06:06:55.064221 qwak_core-0.0.33/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.576259 qwak_core-0.0.33/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-04-25 06:07:00.572259 qwak_core-0.0.33/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-04-25 06:06:54.700218 qwak_core-0.0.33/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-04-25 06:07:00.572259 qwak_core-0.0.33/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-04-25 06:07:00.576259 qwak_core-0.0.33/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-04-25 06:06:54.888220 qwak_core-0.0.33/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.576259 qwak_core-0.0.33/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-04-25 06:07:00.556259 qwak_core-0.0.33/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-04-25 06:06:53.424209 qwak_core-0.0.33/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-04-25 06:07:00.560259 qwak_core-0.0.33/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-04-25 06:07:00.432258 qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-04-25 06:06:44.876145 qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-04-25 06:07:00.432258 qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-04-25 06:07:00.428258 qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-04-25 06:06:44.692144 qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.432258 qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-04-25 06:07:00.432258 qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-04-25 06:06:45.056146 qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-04-25 06:07:00.436258 qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-04-25 06:07:00.556259 qwak_core-0.0.33/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-04-25 06:06:53.028207 qwak_core-0.0.33/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-04-25 06:07:00.556259 qwak_core-0.0.33/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-04-25 06:07:00.568259 qwak_core-0.0.33/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-04-25 06:06:54.320216 qwak_core-0.0.33/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-04-25 06:07:00.568259 qwak_core-0.0.33/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-04-25 06:07:00.428258 qwak_core-0.0.33/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-04-25 06:06:42.720129 qwak_core-0.0.33/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.428258 qwak_core-0.0.33/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-04-25 06:07:00.424258 qwak_core-0.0.33/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-04-25 06:06:42.540128 qwak_core-0.0.33/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-04-25 06:07:00.428258 qwak_core-0.0.33/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-04-25 06:07:00.420258 qwak_core-0.0.33/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-04-25 06:06:42.008124 qwak_core-0.0.33/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.420258 qwak_core-0.0.33/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-04-25 06:07:00.420258 qwak_core-0.0.33/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-04-25 06:06:42.184126 qwak_core-0.0.33/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.420258 qwak_core-0.0.33/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-04-25 06:07:00.424258 qwak_core-0.0.33/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-04-25 06:06:42.360127 qwak_core-0.0.33/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-04-25 06:07:00.424258 qwak_core-0.0.33/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-04-25 06:07:00.628260 qwak_core-0.0.33/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-04-25 06:06:59.200250 qwak_core-0.0.33/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-04-25 06:07:00.628260 qwak_core-0.0.33/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-04-25 06:07:00.624260 qwak_core-0.0.33/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-04-25 06:06:59.020249 qwak_core-0.0.33/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.624260 qwak_core-0.0.33/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0     4083 2023-04-25 06:07:00.444259 qwak_core-0.0.33/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0     4036 2023-04-25 06:06:43.976138 qwak_core-0.0.33/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.444259 qwak_core-0.0.33/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3001 2023-04-25 06:07:00.444259 qwak_core-0.0.33/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2574 2023-04-25 06:06:44.152140 qwak_core-0.0.33/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 06:07:00.444259 qwak_core-0.0.33/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     1906 2023-04-25 06:07:01.764268 qwak_core-0.0.33/pyproject.toml
--rw-r--r--   0        0        0      447 2023-04-25 06:07:01.764268 qwak_core-0.0.33/qwak/__init__.py
--rw-r--r--   0        0        0     1204 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    32139 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/automations/automations.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5478 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0       77 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14950 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4255 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     2585 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-04-25 06:05:59.167818 qwak_core-0.0.33/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0     1201 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     2006 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2961 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1730 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     8808 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/const.py
--rw-r--r--   0        0        0     1377 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     5933 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6071 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      829 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/schema.py
--rw-r--r--   0        0        0     2964 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/schema_entities.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak/testing/fixtures.py
--rw-r--r--   0        0        0       46 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5776 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-04-25 06:05:59.171818 qwak_core-0.0.33/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-04-25 06:05:59.175818 qwak_core-0.0.33/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-04-25 06:05:59.175818 qwak_core-0.0.33/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-04-25 06:05:59.175818 qwak_core-0.0.33/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-04-25 06:05:59.175818 qwak_core-0.0.33/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     3995 2023-04-25 06:05:59.175818 qwak_core-0.0.33/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-04-25 06:05:59.175818 qwak_core-0.0.33/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-04-25 06:05:59.175818 qwak_core-0.0.33/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-04-25 06:05:59.175818 qwak_core-0.0.33/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.175818 qwak_core-0.0.33/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-04-25 06:05:59.175818 qwak_core-0.0.33/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13054 2023-04-25 06:05:59.175818 qwak_core-0.0.33/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-04-25 06:05:59.175818 qwak_core-0.0.33/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-04-25 06:05:59.175818 qwak_core-0.0.33/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4507 1970-01-01 00:00:00.000000 qwak_core-0.0.33/setup.py
--rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 qwak_core-0.0.33/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-04-25 07:42:36.574164 qwak_core-0.0.34/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 07:43:45.334675 qwak_core-0.0.34/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-04-25 07:43:45.358675 qwak_core-0.0.34/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-04-25 07:43:25.470527 qwak_core-0.0.34/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.358675 qwak_core-0.0.34/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-04-25 07:43:45.354675 qwak_core-0.0.34/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-04-25 07:43:25.110525 qwak_core-0.0.34/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.354675 qwak_core-0.0.34/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-04-25 07:43:45.358675 qwak_core-0.0.34/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-04-25 07:43:25.290526 qwak_core-0.0.34/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.358675 qwak_core-0.0.34/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-04-25 07:43:45.346675 qwak_core-0.0.34/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-04-25 07:43:24.574520 qwak_core-0.0.34/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-04-25 07:43:45.350675 qwak_core-0.0.34/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-04-25 07:43:45.350675 qwak_core-0.0.34/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-04-25 07:43:24.754522 qwak_core-0.0.34/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.350675 qwak_core-0.0.34/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-04-25 07:43:45.350675 qwak_core-0.0.34/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-04-25 07:43:24.934523 qwak_core-0.0.34/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.354675 qwak_core-0.0.34/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-04-25 07:43:45.334675 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-04-25 07:43:24.394519 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-04-25 07:43:45.334675 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-04-25 07:43:45.338675 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-04-25 07:43:25.650529 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.338675 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-04-25 07:43:45.342675 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-04-25 07:43:26.010531 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.342675 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-04-25 07:43:45.342675 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-04-25 07:43:26.190533 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-04-25 07:43:45.346675 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-04-25 07:43:45.338675 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-04-25 07:43:25.830530 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.338675 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-04-25 07:43:45.346675 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-04-25 07:43:26.370534 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.346675 qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-04-25 07:43:45.390675 qwak_core-0.0.34/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-04-25 07:43:28.902553 qwak_core-0.0.34/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.390675 qwak_core-0.0.34/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-04-25 07:43:45.390675 qwak_core-0.0.34/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-04-25 07:43:29.086554 qwak_core-0.0.34/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-04-25 07:43:45.390675 qwak_core-0.0.34/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-04-25 07:43:45.458676 qwak_core-0.0.34/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-04-25 07:43:34.054591 qwak_core-0.0.34/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.458676 qwak_core-0.0.34/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-04-25 07:43:45.458676 qwak_core-0.0.34/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-04-25 07:43:34.234592 qwak_core-0.0.34/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-04-25 07:43:45.458676 qwak_core-0.0.34/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-04-25 07:43:45.462676 qwak_core-0.0.34/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-04-25 07:43:35.158599 qwak_core-0.0.34/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-04-25 07:43:45.466676 qwak_core-0.0.34/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-04-25 07:43:45.462676 qwak_core-0.0.34/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-04-25 07:43:34.978598 qwak_core-0.0.34/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.462676 qwak_core-0.0.34/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-04-25 07:43:45.466676 qwak_core-0.0.34/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-04-25 07:43:35.342600 qwak_core-0.0.34/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.466676 qwak_core-0.0.34/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-04-25 07:43:45.466676 qwak_core-0.0.34/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-04-25 07:43:35.530602 qwak_core-0.0.34/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-04-25 07:43:45.470676 qwak_core-0.0.34/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11441 2023-04-25 07:43:45.530676 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    17892 2023-04-25 07:43:40.654640 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.530676 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-04-25 07:43:45.526676 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-04-25 07:43:40.294637 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.526676 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-04-25 07:43:45.526676 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-04-25 07:43:40.474639 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.526676 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-04-25 07:43:45.518676 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-04-25 07:43:39.938635 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-04-25 07:43:45.522676 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-04-25 07:43:45.522676 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-04-25 07:43:40.118636 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.522676 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-04-25 07:43:45.534676 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-04-25 07:43:41.202644 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.534676 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-04-25 07:43:45.534676 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-04-25 07:43:41.006643 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.534676 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-04-25 07:43:45.530676 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-04-25 07:43:40.830641 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.530676 qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-04-25 07:43:45.574677 qwak_core-0.0.34/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-04-25 07:43:44.698670 qwak_core-0.0.34/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.574677 qwak_core-0.0.34/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-04-25 07:43:45.570677 qwak_core-0.0.34/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-04-25 07:43:44.326667 qwak_core-0.0.34/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.570677 qwak_core-0.0.34/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    37419 2023-04-25 07:43:45.574677 qwak_core-0.0.34/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    48027 2023-04-25 07:43:44.518669 qwak_core-0.0.34/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-04-25 07:43:45.574677 qwak_core-0.0.34/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-04-25 07:43:45.494676 qwak_core-0.0.34/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-04-25 07:43:37.382616 qwak_core-0.0.34/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-04-25 07:43:45.494676 qwak_core-0.0.34/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-04-25 07:43:45.490676 qwak_core-0.0.34/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-04-25 07:43:37.198614 qwak_core-0.0.34/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.494676 qwak_core-0.0.34/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-04-25 07:43:45.482676 qwak_core-0.0.34/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-04-25 07:43:36.834612 qwak_core-0.0.34/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.482676 qwak_core-0.0.34/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-04-25 07:43:45.486676 qwak_core-0.0.34/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-04-25 07:43:37.014613 qwak_core-0.0.34/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.486676 qwak_core-0.0.34/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-04-25 07:43:45.486676 qwak_core-0.0.34/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-04-25 07:43:37.562617 qwak_core-0.0.34/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-04-25 07:43:45.490676 qwak_core-0.0.34/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-04-25 07:43:45.490676 qwak_core-0.0.34/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-04-25 07:43:37.958620 qwak_core-0.0.34/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-04-25 07:43:45.490676 qwak_core-0.0.34/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-04-25 07:43:45.502676 qwak_core-0.0.34/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-04-25 07:43:38.338623 qwak_core-0.0.34/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.502676 qwak_core-0.0.34/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-04-25 07:43:45.502676 qwak_core-0.0.34/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-04-25 07:43:38.514624 qwak_core-0.0.34/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-04-25 07:43:45.502676 qwak_core-0.0.34/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-04-25 07:43:45.478676 qwak_core-0.0.34/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-04-25 07:43:36.286608 qwak_core-0.0.34/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.478676 qwak_core-0.0.34/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-04-25 07:43:45.478676 qwak_core-0.0.34/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-04-25 07:43:36.470609 qwak_core-0.0.34/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-04-25 07:43:45.478676 qwak_core-0.0.34/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-04-25 07:43:45.470676 qwak_core-0.0.34/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-04-25 07:43:35.910605 qwak_core-0.0.34/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.474676 qwak_core-0.0.34/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    42956 2023-04-25 07:43:45.470676 qwak_core-0.0.34/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    62847 2023-04-25 07:43:35.726603 qwak_core-0.0.34/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.470676 qwak_core-0.0.34/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-04-25 07:43:45.474676 qwak_core-0.0.34/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-04-25 07:43:36.106606 qwak_core-0.0.34/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-04-25 07:43:45.474676 qwak_core-0.0.34/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-04-25 07:43:45.378675 qwak_core-0.0.34/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-04-25 07:43:27.994546 qwak_core-0.0.34/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.378675 qwak_core-0.0.34/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-04-25 07:43:45.378675 qwak_core-0.0.34/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-04-25 07:43:28.174547 qwak_core-0.0.34/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.382675 qwak_core-0.0.34/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-04-25 07:43:45.382675 qwak_core-0.0.34/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-04-25 07:43:28.358548 qwak_core-0.0.34/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-04-25 07:43:45.382675 qwak_core-0.0.34/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-04-25 07:43:45.438675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-04-25 07:43:32.986583 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.438675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-04-25 07:43:45.434676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-04-25 07:43:32.806582 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-04-25 07:43:45.438675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-04-25 07:43:45.418676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-04-25 07:43:31.306570 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.418676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-04-25 07:43:45.414675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-04-25 07:43:31.122569 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.418676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-04-25 07:43:45.410675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-04-25 07:43:30.562565 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.410675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    27847 2023-04-25 07:43:45.414675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20073 2023-04-25 07:43:30.938568 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    33080 2023-04-25 07:43:45.414675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-04-25 07:43:45.418676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-04-25 07:43:31.486572 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.422675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-04-25 07:43:45.422675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-04-25 07:43:31.666573 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-04-25 07:43:45.422675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    24876 2023-04-25 07:43:45.410675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    36861 2023-04-25 07:43:30.750566 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.410675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-04-25 07:43:45.426675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-04-25 07:43:31.842574 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.426675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-04-25 07:43:45.438675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-04-25 07:43:44.878672 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.442676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-04-25 07:43:45.442676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-04-25 07:43:45.058673 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-04-25 07:43:45.442676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-04-25 07:43:45.442676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-04-25 07:43:33.518587 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.446676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-04-25 07:43:45.446676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-04-25 07:43:33.698588 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-04-25 07:43:45.446676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-04-25 07:43:45.450676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-04-25 07:43:33.874590 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.450676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-04-25 07:43:45.454676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-04-25 07:43:34.602595 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.454676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-04-25 07:43:45.450676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-04-25 07:43:34.418594 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-04-25 07:43:45.450676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-04-25 07:43:45.454676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-04-25 07:43:34.794597 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.454676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    13329 2023-04-25 07:43:45.426675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23039 2023-04-25 07:43:32.030576 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.426675 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-04-25 07:43:45.430676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-04-25 07:43:32.262578 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.430676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-04-25 07:43:45.430676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-04-25 07:43:32.446579 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-04-25 07:43:45.430676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-04-25 07:43:45.434676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-04-25 07:43:32.630580 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.434676 qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-04-25 07:43:45.538676 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-04-25 07:43:41.382645 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.538676 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-04-25 07:43:45.538676 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-04-25 07:43:41.566647 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-04-25 07:43:45.542676 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-04-25 07:43:45.542676 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-04-25 07:43:41.762648 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.542676 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-04-25 07:43:45.542676 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-04-25 07:43:41.950650 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-04-25 07:43:45.546676 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-04-25 07:43:45.546676 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-04-25 07:43:42.158651 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-04-25 07:43:45.546676 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-04-25 07:43:45.546676 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-04-25 07:43:42.338652 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.550676 qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-04-25 07:43:45.506676 qwak_core-0.0.34/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-04-25 07:43:38.690625 qwak_core-0.0.34/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.506676 qwak_core-0.0.34/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-04-25 07:43:45.506676 qwak_core-0.0.34/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-04-25 07:43:38.866627 qwak_core-0.0.34/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-04-25 07:43:45.510676 qwak_core-0.0.34/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-04-25 07:43:45.394675 qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-04-25 07:43:29.830560 qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.398675 qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-04-25 07:43:45.398675 qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-04-25 07:43:30.010561 qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.398675 qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-04-25 07:43:45.402675 qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-04-25 07:43:30.190562 qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-04-25 07:43:45.406675 qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-04-25 07:43:45.406675 qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-04-25 07:43:30.374564 qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.406675 qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-04-25 07:43:45.482676 qwak_core-0.0.34/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-04-25 07:43:36.650610 qwak_core-0.0.34/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-04-25 07:43:45.482676 qwak_core-0.0.34/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-04-25 07:43:45.550676 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-04-25 07:43:42.526654 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.550676 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-04-25 07:43:45.554676 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-04-25 07:43:42.706655 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.554676 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-04-25 07:43:45.554676 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-04-25 07:43:42.890657 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.554676 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-04-25 07:43:45.558677 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-04-25 07:43:43.238659 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.558677 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-04-25 07:43:45.558677 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-04-25 07:43:43.426661 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.558677 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-04-25 07:43:45.562677 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-04-25 07:43:43.622662 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-04-25 07:43:45.562677 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-04-25 07:43:45.562677 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-04-25 07:43:43.802663 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.566676 qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-04-25 07:43:45.510676 qwak_core-0.0.34/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-04-25 07:43:39.222629 qwak_core-0.0.34/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.514676 qwak_core-0.0.34/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-04-25 07:43:45.518676 qwak_core-0.0.34/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-04-25 07:43:39.758633 qwak_core-0.0.34/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.518676 qwak_core-0.0.34/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-04-25 07:43:45.514676 qwak_core-0.0.34/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-04-25 07:43:39.398631 qwak_core-0.0.34/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-04-25 07:43:45.514676 qwak_core-0.0.34/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-04-25 07:43:45.514676 qwak_core-0.0.34/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-04-25 07:43:39.578632 qwak_core-0.0.34/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.518676 qwak_core-0.0.34/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-04-25 07:43:45.498676 qwak_core-0.0.34/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-04-25 07:43:38.158621 qwak_core-0.0.34/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-04-25 07:43:45.498676 qwak_core-0.0.34/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-04-25 07:43:45.374675 qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-04-25 07:43:29.458557 qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-04-25 07:43:45.374675 qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-04-25 07:43:45.370675 qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-04-25 07:43:29.274555 qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.374675 qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-04-25 07:43:45.374675 qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-04-25 07:43:29.646558 qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-04-25 07:43:45.378675 qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-04-25 07:43:45.498676 qwak_core-0.0.34/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-04-25 07:43:37.754619 qwak_core-0.0.34/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-04-25 07:43:45.498676 qwak_core-0.0.34/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-04-25 07:43:45.510676 qwak_core-0.0.34/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-04-25 07:43:39.042628 qwak_core-0.0.34/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-04-25 07:43:45.510676 qwak_core-0.0.34/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-04-25 07:43:45.370675 qwak_core-0.0.34/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-04-25 07:43:27.278540 qwak_core-0.0.34/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.370675 qwak_core-0.0.34/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-04-25 07:43:45.366675 qwak_core-0.0.34/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-04-25 07:43:27.086539 qwak_core-0.0.34/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-04-25 07:43:45.370675 qwak_core-0.0.34/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-04-25 07:43:45.362675 qwak_core-0.0.34/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-04-25 07:43:26.546535 qwak_core-0.0.34/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.362675 qwak_core-0.0.34/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-04-25 07:43:45.362675 qwak_core-0.0.34/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-04-25 07:43:26.726536 qwak_core-0.0.34/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.362675 qwak_core-0.0.34/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-04-25 07:43:45.366675 qwak_core-0.0.34/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-04-25 07:43:26.906538 qwak_core-0.0.34/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-04-25 07:43:45.366675 qwak_core-0.0.34/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-04-25 07:43:45.566676 qwak_core-0.0.34/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-04-25 07:43:44.150666 qwak_core-0.0.34/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-04-25 07:43:45.570677 qwak_core-0.0.34/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-04-25 07:43:45.566676 qwak_core-0.0.34/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-04-25 07:43:43.978665 qwak_core-0.0.34/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.566676 qwak_core-0.0.34/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0     4083 2023-04-25 07:43:45.386675 qwak_core-0.0.34/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0     4036 2023-04-25 07:43:28.542550 qwak_core-0.0.34/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.386675 qwak_core-0.0.34/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3001 2023-04-25 07:43:45.386675 qwak_core-0.0.34/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2574 2023-04-25 07:43:28.718551 qwak_core-0.0.34/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-25 07:43:45.386675 qwak_core-0.0.34/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     1906 2023-04-25 07:43:47.074688 qwak_core-0.0.34/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-04-25 07:43:47.074688 qwak_core-0.0.34/qwak/__init__.py
+-rw-r--r--   0        0        0     1204 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    32139 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/automations/automations.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5478 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-04-25 07:42:36.574164 qwak_core-0.0.34/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0       77 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14950 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4255 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     2585 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0     1201 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     2006 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2961 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1730 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     8808 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/const.py
+-rw-r--r--   0        0        0     1377 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     5933 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6071 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      829 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/schema.py
+-rw-r--r--   0        0        0     2964 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-04-25 07:42:36.578164 qwak_core-0.0.34/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0       46 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5776 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     3995 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13054 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-04-25 07:42:36.582164 qwak_core-0.0.34/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4507 1970-01-01 00:00:00.000000 qwak_core-0.0.34/setup.py
+-rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 qwak_core-0.0.34/PKG-INFO
```

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from _qwak_proto.qwak.automation.v1 import common_pb2 as qwak_dot_automation_dot_v1_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n qwak/automation/v1/trigger.proto\x12\x12qwak.automation.v1\x1a\x1fqwak/automation/v1/common.proto\"\xd8\x01\n\x07Trigger\x12\x41\n\x11scheduled_trigger\x18\x01 \x01(\x0b\x32$.qwak.automation.v1.ScheduledTriggerH\x00\x12\x46\n\x14metric_based_trigger\x18\x02 \x01(\x0b\x32&.qwak.automation.v1.MetricBasedTriggerH\x00\x12\x37\n\x0cnone_trigger\x18\x03 \x01(\x0b\x32\x1f.qwak.automation.v1.NoneTriggerH\x00\x42\t\n\x07trigger\"B\n\x10ScheduledTrigger\x12\x0e\n\x04\x63ron\x18\x01 \x01(\tH\x00\x12\x12\n\x08interval\x18\x02 \x01(\tH\x00\x42\n\n\x08schedule\"\xc3\x01\n\x12MetricBasedTrigger\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x06metric\x18\x02 \x01(\x0b\x32\x1a.qwak.automation.v1.Metric\x12I\n\x13threshold_direction\x18\x03 \x01(\x0e\x32,.qwak.automation.v1.MetricThresholdDirection\x12\x11\n\tthreshold\x18\x04 \x01(\t\x12\x15\n\roverride_cron\x18\x05 \x01(\t\"\r\n\x0bNoneTriggerB!\n\x1d\x63om.qwak.ai.automation.api.v1P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n qwak/automation/v1/trigger.proto\x12\x12qwak.automation.v1\x1a\x1fqwak/automation/v1/common.proto\"\x9e\x02\n\x07Trigger\x12\x41\n\x11scheduled_trigger\x18\x01 \x01(\x0b\x32$.qwak.automation.v1.ScheduledTriggerH\x00\x12\x46\n\x14metric_based_trigger\x18\x02 \x01(\x0b\x32&.qwak.automation.v1.MetricBasedTriggerH\x00\x12\x37\n\x0cnone_trigger\x18\x03 \x01(\x0b\x32\x1f.qwak.automation.v1.NoneTriggerH\x00\x12\x44\n\x13on_boarding_trigger\x18\x04 \x01(\x0b\x32%.qwak.automation.v1.OnBoardingTriggerH\x00\x42\t\n\x07trigger\"B\n\x10ScheduledTrigger\x12\x0e\n\x04\x63ron\x18\x01 \x01(\tH\x00\x12\x12\n\x08interval\x18\x02 \x01(\tH\x00\x42\n\n\x08schedule\"\xc3\x01\n\x12MetricBasedTrigger\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x06metric\x18\x02 \x01(\x0b\x32\x1a.qwak.automation.v1.Metric\x12I\n\x13threshold_direction\x18\x03 \x01(\x0e\x32,.qwak.automation.v1.MetricThresholdDirection\x12\x11\n\tthreshold\x18\x04 \x01(\t\x12\x15\n\roverride_cron\x18\x05 \x01(\t\"\r\n\x0bNoneTrigger\"\x13\n\x11OnBoardingTriggerB!\n\x1d\x63om.qwak.ai.automation.api.v1P\x01\x62\x06proto3')
 
 
 
 _TRIGGER = DESCRIPTOR.message_types_by_name['Trigger']
 _SCHEDULEDTRIGGER = DESCRIPTOR.message_types_by_name['ScheduledTrigger']
 _METRICBASEDTRIGGER = DESCRIPTOR.message_types_by_name['MetricBasedTrigger']
 _NONETRIGGER = DESCRIPTOR.message_types_by_name['NoneTrigger']
+_ONBOARDINGTRIGGER = DESCRIPTOR.message_types_by_name['OnBoardingTrigger']
 Trigger = _reflection.GeneratedProtocolMessageType('Trigger', (_message.Message,), {
   'DESCRIPTOR' : _TRIGGER,
   '__module__' : 'qwak.automation.v1.trigger_pb2'
   # @@protoc_insertion_point(class_scope:qwak.automation.v1.Trigger)
   })
 _sym_db.RegisterMessage(Trigger)
 
@@ -47,20 +48,29 @@
 NoneTrigger = _reflection.GeneratedProtocolMessageType('NoneTrigger', (_message.Message,), {
   'DESCRIPTOR' : _NONETRIGGER,
   '__module__' : 'qwak.automation.v1.trigger_pb2'
   # @@protoc_insertion_point(class_scope:qwak.automation.v1.NoneTrigger)
   })
 _sym_db.RegisterMessage(NoneTrigger)
 
+OnBoardingTrigger = _reflection.GeneratedProtocolMessageType('OnBoardingTrigger', (_message.Message,), {
+  'DESCRIPTOR' : _ONBOARDINGTRIGGER,
+  '__module__' : 'qwak.automation.v1.trigger_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.automation.v1.OnBoardingTrigger)
+  })
+_sym_db.RegisterMessage(OnBoardingTrigger)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\035com.qwak.ai.automation.api.v1P\001'
   _TRIGGER._serialized_start=90
-  _TRIGGER._serialized_end=306
-  _SCHEDULEDTRIGGER._serialized_start=308
-  _SCHEDULEDTRIGGER._serialized_end=374
-  _METRICBASEDTRIGGER._serialized_start=377
-  _METRICBASEDTRIGGER._serialized_end=572
-  _NONETRIGGER._serialized_start=574
-  _NONETRIGGER._serialized_end=587
+  _TRIGGER._serialized_end=376
+  _SCHEDULEDTRIGGER._serialized_start=378
+  _SCHEDULEDTRIGGER._serialized_end=444
+  _METRICBASEDTRIGGER._serialized_start=447
+  _METRICBASEDTRIGGER._serialized_end=642
+  _NONETRIGGER._serialized_start=644
+  _NONETRIGGER._serialized_end=657
+  _ONBOARDINGTRIGGER._serialized_start=659
+  _ONBOARDINGTRIGGER._serialized_end=678
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -17,30 +17,34 @@
 
 class Trigger(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SCHEDULED_TRIGGER_FIELD_NUMBER: builtins.int
     METRIC_BASED_TRIGGER_FIELD_NUMBER: builtins.int
     NONE_TRIGGER_FIELD_NUMBER: builtins.int
+    ON_BOARDING_TRIGGER_FIELD_NUMBER: builtins.int
     @property
     def scheduled_trigger(self) -> global___ScheduledTrigger: ...
     @property
     def metric_based_trigger(self) -> global___MetricBasedTrigger: ...
     @property
     def none_trigger(self) -> global___NoneTrigger: ...
+    @property
+    def on_boarding_trigger(self) -> global___OnBoardingTrigger: ...
     def __init__(
         self,
         *,
         scheduled_trigger: global___ScheduledTrigger | None = ...,
         metric_based_trigger: global___MetricBasedTrigger | None = ...,
         none_trigger: global___NoneTrigger | None = ...,
+        on_boarding_trigger: global___OnBoardingTrigger | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["metric_based_trigger", b"metric_based_trigger", "none_trigger", b"none_trigger", "scheduled_trigger", b"scheduled_trigger", "trigger", b"trigger"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["metric_based_trigger", b"metric_based_trigger", "none_trigger", b"none_trigger", "scheduled_trigger", b"scheduled_trigger", "trigger", b"trigger"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["trigger", b"trigger"]) -> typing_extensions.Literal["scheduled_trigger", "metric_based_trigger", "none_trigger"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["metric_based_trigger", b"metric_based_trigger", "none_trigger", b"none_trigger", "on_boarding_trigger", b"on_boarding_trigger", "scheduled_trigger", b"scheduled_trigger", "trigger", b"trigger"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["metric_based_trigger", b"metric_based_trigger", "none_trigger", b"none_trigger", "on_boarding_trigger", b"on_boarding_trigger", "scheduled_trigger", b"scheduled_trigger", "trigger", b"trigger"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["trigger", b"trigger"]) -> typing_extensions.Literal["scheduled_trigger", "metric_based_trigger", "none_trigger", "on_boarding_trigger"] | None: ...
 
 global___Trigger = Trigger
 
 class ScheduledTrigger(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CRON_FIELD_NUMBER: builtins.int
@@ -93,7 +97,16 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___NoneTrigger = NoneTrigger
+
+class OnBoardingTrigger(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
+
+global___OnBoardingTrigger = OnBoardingTrigger
```

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.34/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.34/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.34/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/pyproject.toml` & `qwak_core-0.0.34/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.33"
+version = "0.0.34"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     {include = "qwak"},
     {include = "_qwak_proto"},
```

### Comparing `qwak_core-0.0.33/qwak/automations/__init__.py` & `qwak_core-0.0.34/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/automations/automation_executions.py` & `qwak_core-0.0.34/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/automations/automations.py` & `qwak_core-0.0.34/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.34/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.34/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.34/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.34/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.34/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/alert_management/client.py` & `qwak_core-0.0.34/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/analytics/client.py` & `qwak_core-0.0.34/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/audience/client.py` & `qwak_core-0.0.34/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/automation_management/client.py` & `qwak_core-0.0.34/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.34/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.34/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.34/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.34/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/build_management/client.py` & `qwak_core-0.0.34/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.34/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.34/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/deployment/client.py` & `qwak_core-0.0.34/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.34/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.34/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.34/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.34/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.34/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/logging_client/client.py` & `qwak_core-0.0.34/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/model_management/client.py` & `qwak_core-0.0.34/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/project/client.py` & `qwak_core-0.0.34/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/secret_service/client.py` & `qwak_core-0.0.34/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.34/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.34/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.34/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.34/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.34/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.34/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.34/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.34/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.34/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.34/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.34/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.34/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/feature_store/online/client.py` & `qwak_core-0.0.34/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/inner/const.py` & `qwak_core-0.0.34/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.34/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.34/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.34/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.34/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/inner/singleton_meta.py` & `qwak_core-0.0.34/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/inner/tool/auth.py` & `qwak_core-0.0.34/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.34/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.34/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.34/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.34/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/model/adapters/__init__.py` & `qwak_core-0.0.34/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.34/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.34/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.34/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.34/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.34/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/model/base.py` & `qwak_core-0.0.34/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/model/decorators/api.py` & `qwak_core-0.0.34/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.34/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/model/experiment_tracking.py` & `qwak_core-0.0.34/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/model/schema.py` & `qwak_core-0.0.34/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/model/schema_entities.py` & `qwak_core-0.0.34/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.34/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.34/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.34/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.34/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.34/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.34/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/qwak_client/client.py` & `qwak_core-0.0.34/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.34/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/qwak_client/models/model.py` & `qwak_core-0.0.34/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.34/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.34/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.34/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/qwak_services_mock/services_mock.py` & `qwak_core-0.0.34/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.33/setup.py` & `qwak_core-0.0.34/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
  'protobuf>=3.10,<4',
  'python-jose',
  'requests',
  'typeguard>=2,<3']
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.33',
+    'version': '0.0.34',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.33/PKG-INFO` & `qwak_core-0.0.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.33
+Version: 0.0.34
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

