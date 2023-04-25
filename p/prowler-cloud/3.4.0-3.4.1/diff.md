# Comparing `tmp/prowler_cloud-3.4.0.tar.gz` & `tmp/prowler_cloud-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prowler_cloud-3.4.0.tar", max compression
+gzip compressed data, was "prowler_cloud-3.4.1.tar", max compression
```

## Comparing `prowler_cloud-3.4.0.tar` & `prowler_cloud-3.4.1.tar`

### file list

```diff
@@ -1,1295 +1,1295 @@
--rw-r--r--   0        0        0    11339 2023-04-19 12:29:23.881015 prowler_cloud-3.4.0/LICENSE
--rw-r--r--   0        0        0    13104 2023-04-19 12:29:23.881214 prowler_cloud-3.4.0/README.md
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.914816 prowler_cloud-3.4.0/prowler/__init__.py
--rw-r--r--   0        0        0     8364 2023-04-19 16:59:58.235656 prowler_cloud-3.4.0/prowler/__main__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.915066 prowler_cloud-3.4.0/prowler/compliance/aws/__init__.py
--rw-r--r--   0        0        0     6516 2023-04-19 12:29:23.915167 prowler_cloud-3.4.0/prowler/compliance/aws/aws_audit_manager_control_tower_guardrails_aws.json
--rw-r--r--   0        0        0    17475 2023-04-19 14:30:31.781622 prowler_cloud-3.4.0/prowler/compliance/aws/aws_foundational_security_best_practices_aws.json
--rw-r--r--   0        0        0   260398 2023-04-19 14:30:31.782770 prowler_cloud-3.4.0/prowler/compliance/aws/cis_1.4_aws.json
--rw-r--r--   0        0        0   287275 2023-04-19 14:30:31.783625 prowler_cloud-3.4.0/prowler/compliance/aws/cis_1.5_aws.json
--rw-r--r--   0        0        0    15458 2023-04-19 14:30:31.783934 prowler_cloud-3.4.0/prowler/compliance/aws/cisa_aws.json
--rw-r--r--   0        0        0   124269 2023-04-19 14:30:31.784533 prowler_cloud-3.4.0/prowler/compliance/aws/ens_rd2022_aws.json
--rw-r--r--   0        0        0    18551 2023-04-19 14:30:31.784938 prowler_cloud-3.4.0/prowler/compliance/aws/fedramp_low_revision_4_aws.json
--rw-r--r--   0        0        0    57257 2023-04-19 14:30:31.785245 prowler_cloud-3.4.0/prowler/compliance/aws/fedramp_moderate_revision_4_aws.json
--rw-r--r--   0        0        0    31059 2023-04-19 14:30:31.785581 prowler_cloud-3.4.0/prowler/compliance/aws/ffiec_aws.json
--rw-r--r--   0        0        0    10166 2023-04-19 14:30:31.785863 prowler_cloud-3.4.0/prowler/compliance/aws/gdpr_aws.json
--rw-r--r--   0        0        0    18763 2023-04-19 14:30:31.786156 prowler_cloud-3.4.0/prowler/compliance/aws/gxp_21_cfr_part_11_aws.json
--rw-r--r--   0        0        0    11774 2023-04-19 12:29:23.917593 prowler_cloud-3.4.0/prowler/compliance/aws/gxp_eu_annex_11_aws.json
--rw-r--r--   0        0        0    31000 2023-04-19 14:30:31.786493 prowler_cloud-3.4.0/prowler/compliance/aws/hipaa_aws.json
--rw-r--r--   0        0        0    86208 2023-04-19 14:30:31.787189 prowler_cloud-3.4.0/prowler/compliance/aws/nist_800_171_revision_2_aws.json
--rw-r--r--   0        0        0    50559 2023-04-19 14:30:31.787572 prowler_cloud-3.4.0/prowler/compliance/aws/nist_800_53_revision_4_aws.json
--rw-r--r--   0        0        0   243911 2023-04-19 14:30:31.788157 prowler_cloud-3.4.0/prowler/compliance/aws/nist_800_53_revision_5_aws.json
--rw-r--r--   0        0        0    40042 2023-04-19 14:30:31.788517 prowler_cloud-3.4.0/prowler/compliance/aws/nist_csf_1.1_aws.json
--rw-r--r--   0        0        0     8722 2023-04-19 14:30:31.788905 prowler_cloud-3.4.0/prowler/compliance/aws/pci_3.2.1_aws.json
--rw-r--r--   0        0        0     8563 2023-04-19 14:30:31.789072 prowler_cloud-3.4.0/prowler/compliance/aws/rbi_cyber_security_framework_aws.json
--rw-r--r--   0        0        0    93913 2023-04-19 14:30:31.789715 prowler_cloud-3.4.0/prowler/compliance/aws/soc2_aws.json
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.918830 prowler_cloud-3.4.0/prowler/compliance/azure/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.918896 prowler_cloud-3.4.0/prowler/compliance/gcp/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.919011 prowler_cloud-3.4.0/prowler/config/__init__.py
--rw-r--r--   0        0        0     2352 2023-04-19 12:29:23.919100 prowler_cloud-3.4.0/prowler/config/allowlist.yaml
--rw-r--r--   0        0        0      165 2023-04-19 12:29:23.919158 prowler_cloud-3.4.0/prowler/config/checklist_example.json
--rw-r--r--   0        0        0     2554 2023-04-20 13:32:41.057004 prowler_cloud-3.4.0/prowler/config/config.py
--rw-r--r--   0        0        0     1942 2023-04-19 12:29:23.919734 prowler_cloud-3.4.0/prowler/config/config.yaml
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.919791 prowler_cloud-3.4.0/prowler/lib/__init__.py
--rw-r--r--   0        0        0      854 2023-04-19 12:29:23.919861 prowler_cloud-3.4.0/prowler/lib/banner.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.919915 prowler_cloud-3.4.0/prowler/lib/check/__init__.py
--rw-r--r--   0        0        0    23001 2023-04-19 16:59:58.235931 prowler_cloud-3.4.0/prowler/lib/check/check.py
--rw-r--r--   0        0        0     2973 2023-04-19 12:29:23.920475 prowler_cloud-3.4.0/prowler/lib/check/checks_loader.py
--rw-r--r--   0        0        0     4413 2023-04-19 12:29:23.920553 prowler_cloud-3.4.0/prowler/lib/check/compliance.py
--rw-r--r--   0        0        0     3645 2023-04-19 12:29:23.920631 prowler_cloud-3.4.0/prowler/lib/check/compliance_models.py
--rw-r--r--   0        0        0     3835 2023-04-19 12:29:23.920708 prowler_cloud-3.4.0/prowler/lib/check/models.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.920774 prowler_cloud-3.4.0/prowler/lib/cli/__init__.py
--rw-r--r--   0        0        0    17266 2023-04-19 12:29:23.920928 prowler_cloud-3.4.0/prowler/lib/cli/parser.py
--rw-r--r--   0        0        0     1885 2023-04-19 12:29:23.921010 prowler_cloud-3.4.0/prowler/lib/logger.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.921073 prowler_cloud-3.4.0/prowler/lib/outputs/__init__.py
--rw-r--r--   0        0        0    19729 2023-04-19 12:29:23.921187 prowler_cloud-3.4.0/prowler/lib/outputs/compliance.py
--rw-r--r--   0        0        0     6687 2023-04-19 12:29:23.922980 prowler_cloud-3.4.0/prowler/lib/outputs/file_descriptors.py
--rw-r--r--   0        0        0    20055 2023-04-19 12:29:23.923272 prowler_cloud-3.4.0/prowler/lib/outputs/html.py
--rw-r--r--   0        0        0     3721 2023-04-19 12:29:23.923348 prowler_cloud-3.4.0/prowler/lib/outputs/json.py
--rw-r--r--   0        0        0    20235 2023-04-19 12:29:23.923478 prowler_cloud-3.4.0/prowler/lib/outputs/models.py
--rw-r--r--   0        0        0    10451 2023-04-19 12:29:23.923678 prowler_cloud-3.4.0/prowler/lib/outputs/outputs.py
--rw-r--r--   0        0        0     6058 2023-04-19 12:29:23.923779 prowler_cloud-3.4.0/prowler/lib/outputs/summary_table.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.923838 prowler_cloud-3.4.0/prowler/lib/scan_filters/__init__.py
--rw-r--r--   0        0        0      552 2023-04-19 12:29:23.923910 prowler_cloud-3.4.0/prowler/lib/scan_filters/scan_filters.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.923974 prowler_cloud-3.4.0/prowler/lib/utils/__init__.py
--rw-r--r--   0        0        0     2200 2023-04-19 12:29:23.924056 prowler_cloud-3.4.0/prowler/lib/utils/utils.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.924142 prowler_cloud-3.4.0/prowler/providers/aws/__init__.py
--rw-r--r--   0        0        0    10318 2023-04-19 12:29:23.924275 prowler_cloud-3.4.0/prowler/providers/aws/aws_provider.py
--rw-r--r--   0        0        0   211438 2023-04-20 11:36:04.257133 prowler_cloud-3.4.0/prowler/providers/aws/aws_regions_by_service.json
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.924651 prowler_cloud-3.4.0/prowler/providers/aws/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.924735 prowler_cloud-3.4.0/prowler/providers/aws/lib/allowlist/__init__.py
--rw-r--r--   0        0        0     7931 2023-04-19 12:29:23.924815 prowler_cloud-3.4.0/prowler/providers/aws/lib/allowlist/allowlist.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.924868 prowler_cloud-3.4.0/prowler/providers/aws/lib/arn/__init__.py
--rw-r--r--   0        0        0     1902 2023-04-19 12:29:23.924941 prowler_cloud-3.4.0/prowler/providers/aws/lib/arn/arn.py
--rw-r--r--   0        0        0     1932 2023-04-19 12:29:23.925001 prowler_cloud-3.4.0/prowler/providers/aws/lib/arn/error.py
--rw-r--r--   0        0        0      953 2023-04-19 12:29:23.925101 prowler_cloud-3.4.0/prowler/providers/aws/lib/audit_info/audit_info.py
--rw-r--r--   0        0        0     1178 2023-04-19 12:29:23.925172 prowler_cloud-3.4.0/prowler/providers/aws/lib/audit_info/models.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925231 prowler_cloud-3.4.0/prowler/providers/aws/lib/quick_inventory/__init__.py
--rw-r--r--   0        0        0    13659 2023-04-19 12:29:23.925364 prowler_cloud-3.4.0/prowler/providers/aws/lib/quick_inventory/quick_inventory.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925429 prowler_cloud-3.4.0/prowler/providers/aws/lib/resource_api_tagging/__init__.py
--rw-r--r--   0        0        0     1585 2023-04-19 12:29:23.925524 prowler_cloud-3.4.0/prowler/providers/aws/lib/resource_api_tagging/resource_api_tagging.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925602 prowler_cloud-3.4.0/prowler/providers/aws/lib/security_hub/__init__.py
--rw-r--r--   0        0        0     5867 2023-04-19 12:29:23.925704 prowler_cloud-3.4.0/prowler/providers/aws/lib/security_hub/security_hub.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925777 prowler_cloud-3.4.0/prowler/providers/aws/services/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925856 prowler_cloud-3.4.0/prowler/providers/aws/services/accessanalyzer/__init__.py
--rw-r--r--   0        0        0      244 2023-04-19 12:29:23.925925 prowler_cloud-3.4.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925983 prowler_cloud-3.4.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/__init__.py
--rw-r--r--   0        0        0     1584 2023-04-19 12:29:23.926072 prowler_cloud-3.4.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.metadata.json
--rw-r--r--   0        0        0     1478 2023-04-19 12:29:23.926147 prowler_cloud-3.4.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.926226 prowler_cloud-3.4.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/__init__.py
--rw-r--r--   0        0        0     1635 2023-04-19 12:29:23.926328 prowler_cloud-3.4.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.metadata.json
--rw-r--r--   0        0        0     2184 2023-04-19 12:29:23.926396 prowler_cloud-3.4.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.py
--rw-r--r--   0        0        0     4735 2023-04-19 12:29:23.926489 prowler_cloud-3.4.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.926555 prowler_cloud-3.4.0/prowler/providers/aws/services/account/__init__.py
--rw-r--r--   0        0        0      200 2023-04-19 12:29:23.926641 prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.926710 prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/__init__.py
--rw-r--r--   0        0        0     1753 2023-04-19 12:29:23.926813 prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.metadata.json
--rw-r--r--   0        0        0      652 2023-04-19 12:29:23.926914 prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.926987 prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/__init__.py
--rw-r--r--   0        0        0     1315 2023-04-19 12:29:23.927076 prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.metadata.json
--rw-r--r--   0        0        0      681 2023-04-19 12:29:23.927162 prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.927235 prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/__init__.py
--rw-r--r--   0        0        0     1674 2023-04-19 12:29:23.927318 prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.metadata.json
--rw-r--r--   0        0        0      699 2023-04-19 12:29:23.927389 prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.py
--rw-r--r--   0        0        0      769 2023-04-19 12:29:23.927493 prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.927558 prowler_cloud-3.4.0/prowler/providers/aws/services/acm/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.927642 prowler_cloud-3.4.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/__init__.py
--rw-r--r--   0        0        0     1368 2023-04-19 12:29:23.927732 prowler_cloud-3.4.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.metadata.json
--rw-r--r--   0        0        0     1233 2023-04-19 12:29:23.927811 prowler_cloud-3.4.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.927881 prowler_cloud-3.4.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/__init__.py
--rw-r--r--   0        0        0     1316 2023-04-19 12:29:23.927960 prowler_cloud-3.4.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.metadata.json
--rw-r--r--   0        0        0     1636 2023-04-19 12:29:23.928023 prowler_cloud-3.4.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.928090 prowler_cloud-3.4.0/prowler/providers/aws/services/acm/acm_client.py
--rw-r--r--   0        0        0     4752 2023-04-19 12:29:23.928187 prowler_cloud-3.4.0/prowler/providers/aws/services/acm/acm_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.928261 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.928350 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/__init__.py
--rw-r--r--   0        0        0     1133 2023-04-19 12:29:23.928450 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.metadata.json
--rw-r--r--   0        0        0      976 2023-04-19 12:29:23.928524 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.py
--rw-r--r--   0        0        0      215 2023-04-19 12:29:23.928590 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.928660 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/__init__.py
--rw-r--r--   0        0        0     1250 2023-04-19 12:29:23.928751 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.metadata.json
--rw-r--r--   0        0        0     1126 2023-04-19 12:29:23.928823 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.928899 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/__init__.py
--rw-r--r--   0        0        0     1087 2023-04-19 12:29:23.928989 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.metadata.json
--rw-r--r--   0        0        0      994 2023-04-19 12:29:23.929063 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.929128 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1676 2023-04-19 12:29:23.929219 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1079 2023-04-19 12:29:23.929284 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.py
--rw-r--r--   0        0        0     5312 2023-04-19 12:29:23.929343 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.929405 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/__init__.py
--rw-r--r--   0        0        0     1181 2023-04-19 12:29:23.929484 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.metadata.json
--rw-r--r--   0        0        0     1093 2023-04-19 12:29:23.929553 prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.929624 prowler_cloud-3.4.0/prowler/providers/aws/services/apigatewayv2/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.929711 prowler_cloud-3.4.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1095 2023-04-19 12:29:23.929800 prowler_cloud-3.4.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1123 2023-04-19 12:29:23.929864 prowler_cloud-3.4.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.929939 prowler_cloud-3.4.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/__init__.py
--rw-r--r--   0        0        0     1038 2023-04-19 12:29:23.930024 prowler_cloud-3.4.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.metadata.json
--rw-r--r--   0        0        0     1037 2023-04-19 12:29:23.930091 prowler_cloud-3.4.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.py
--rw-r--r--   0        0        0      234 2023-04-19 12:29:23.930163 prowler_cloud-3.4.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_client.py
--rw-r--r--   0        0        0     3806 2023-04-19 12:29:23.930279 prowler_cloud-3.4.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.930354 prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/__init__.py
--rw-r--r--   0        0        0      210 2023-04-19 12:29:23.930444 prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.930518 prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/__init__.py
--rw-r--r--   0        0        0     1346 2023-04-19 12:29:23.930597 prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.metadata.json
--rw-r--r--   0        0        0     1273 2023-04-19 12:29:23.930659 prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.930725 prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/__init__.py
--rw-r--r--   0        0        0     1257 2023-04-19 12:29:23.930807 prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.metadata.json
--rw-r--r--   0        0        0     1408 2023-04-19 12:29:23.930874 prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.930944 prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/__init__.py
--rw-r--r--   0        0        0     1269 2023-04-19 12:29:23.931029 prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.metadata.json
--rw-r--r--   0        0        0     1420 2023-04-19 12:29:23.931102 prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.931165 prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/__init__.py
--rw-r--r--   0        0        0     1363 2023-04-19 12:29:23.931240 prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.metadata.json
--rw-r--r--   0        0        0     1583 2023-04-19 12:29:23.931295 prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.py
--rw-r--r--   0        0        0     3619 2023-04-19 12:29:23.931383 prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.931448 prowler_cloud-3.4.0/prowler/providers/aws/services/autoscaling/__init__.py
--rw-r--r--   0        0        0      220 2023-04-19 12:29:23.931525 prowler_cloud-3.4.0/prowler/providers/aws/services/autoscaling/autoscaling_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.931592 prowler_cloud-3.4.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/__init__.py
--rw-r--r--   0        0        0     1172 2023-04-19 12:29:23.931671 prowler_cloud-3.4.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.metadata.json
--rw-r--r--   0        0        0     1902 2023-04-19 12:29:23.931745 prowler_cloud-3.4.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.py
--rw-r--r--   0        0        0       78 2023-04-19 12:29:23.931828 prowler_cloud-3.4.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/fixtures/fixture
--rw-r--r--   0        0        0     2626 2023-04-19 12:29:23.931901 prowler_cloud-3.4.0/prowler/providers/aws/services/autoscaling/autoscaling_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.931954 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/__init__.py
--rw-r--r--   0        0        0      204 2023-04-19 12:29:23.932016 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.932077 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1198 2023-04-19 12:29:23.932164 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.metadata.json
--rw-r--r--   0        0        0     2548 2023-04-19 12:29:23.932234 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.932304 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/__init__.py
--rw-r--r--   0        0        0     1341 2023-04-19 12:29:23.932378 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.metadata.json
--rw-r--r--   0        0        0     3352 2023-04-19 12:29:23.932441 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.932505 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/__init__.py
--rw-r--r--   0        0        0     1536 2023-04-19 12:29:23.932592 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.metadata.json
--rw-r--r--   0        0        0     2209 2023-04-19 12:29:23.932663 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.932740 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1399 2023-04-19 12:29:23.932821 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1823 2023-04-19 12:29:23.932902 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.932963 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/__init__.py
--rw-r--r--   0        0        0     1272 2023-04-19 12:29:23.933034 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.metadata.json
--rw-r--r--   0        0        0     1058 2023-04-19 12:29:23.933094 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.933149 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/__init__.py
--rw-r--r--   0        0        0     1120 2023-04-19 12:29:23.933215 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.metadata.json
--rw-r--r--   0        0        0     1144 2023-04-19 12:29:23.933278 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.933349 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/__init__.py
--rw-r--r--   0        0        0     1619 2023-04-19 12:29:23.933433 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.metadata.json
--rw-r--r--   0        0        0     1169 2023-04-19 12:29:23.933505 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.py
--rw-r--r--   0        0        0     7807 2023-04-19 12:29:23.933581 prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.933644 prowler_cloud-3.4.0/prowler/providers/aws/services/backup/__init__.py
--rw-r--r--   0        0        0      195 2023-04-19 12:29:23.933747 prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.933815 prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_plans_exist/__init__.py
--rw-r--r--   0        0        0     1197 2023-04-19 12:29:23.933931 prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.metadata.json
--rw-r--r--   0        0        0      920 2023-04-19 12:29:23.934028 prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.934091 prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_reportplans_exist/__init__.py
--rw-r--r--   0        0        0     1167 2023-04-19 12:29:23.934209 prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.metadata.json
--rw-r--r--   0        0        0      975 2023-04-19 12:29:23.934311 prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.py
--rw-r--r--   0        0        0     6992 2023-04-19 12:29:23.934426 prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.934489 prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/__init__.py
--rw-r--r--   0        0        0     1162 2023-04-19 12:29:23.934607 prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.metadata.json
--rw-r--r--   0        0        0     1096 2023-04-19 12:29:23.934711 prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.934779 prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_vaults_exist/__init__.py
--rw-r--r--   0        0        0     1134 2023-04-19 12:29:23.935070 prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.metadata.json
--rw-r--r--   0        0        0      928 2023-04-19 12:29:23.935188 prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.935269 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudformation/__init__.py
--rw-r--r--   0        0        0      244 2023-04-19 12:29:23.935355 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudformation/cloudformation_client.py
--rw-r--r--   0        0        0     4466 2023-04-19 12:29:23.935455 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudformation/cloudformation_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.935540 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/__init__.py
--rw-r--r--   0        0        0     1367 2023-04-19 12:29:23.935635 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.metadata.json
--rw-r--r--   0        0        0     1992 2023-04-19 12:29:23.935711 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.935787 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/__init__.py
--rw-r--r--   0        0        0     1286 2023-04-19 12:29:23.935877 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.metadata.json
--rw-r--r--   0        0        0     1249 2023-04-19 12:29:23.935948 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.936018 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/__init__.py
--rw-r--r--   0        0        0      215 2023-04-19 12:29:23.936101 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.936165 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1432 2023-04-19 12:29:23.936241 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1166 2023-04-19 12:29:23.936308 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.936374 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/__init__.py
--rw-r--r--   0        0        0     1321 2023-04-19 12:29:23.936463 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.metadata.json
--rw-r--r--   0        0        0     1164 2023-04-19 12:29:23.936530 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.936609 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/__init__.py
--rw-r--r--   0        0        0     1395 2023-04-19 12:29:23.936692 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.metadata.json
--rw-r--r--   0        0        0     1912 2023-04-19 12:29:23.936753 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.936817 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1501 2023-04-19 12:29:23.936890 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1230 2023-04-19 12:29:23.936947 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.937022 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/__init__.py
--rw-r--r--   0        0        0     1385 2023-04-19 12:29:23.937123 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.metadata.json
--rw-r--r--   0        0        0     1781 2023-04-19 12:29:23.937196 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.937272 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/__init__.py
--rw-r--r--   0        0        0     1479 2023-04-19 12:29:23.937369 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.metadata.json
--rw-r--r--   0        0        0     1031 2023-04-19 12:29:23.937430 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.py
--rw-r--r--   0        0        0     6244 2023-04-19 12:29:23.937508 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.937579 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.937669 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/__init__.py
--rw-r--r--   0        0        0     1268 2023-04-19 12:29:23.937759 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.metadata.json
--rw-r--r--   0        0        0     1707 2023-04-19 12:29:23.937826 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.py
--rw-r--r--   0        0        0      215 2023-04-19 12:29:23.937892 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.937965 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1575 2023-04-19 12:29:23.938067 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.metadata.json
--rw-r--r--   0        0        0     2245 2023-04-19 12:29:23.938153 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.938212 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/__init__.py
--rw-r--r--   0        0        0     1287 2023-04-19 12:29:23.938333 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.metadata.json
--rw-r--r--   0        0        0     1073 2023-04-19 12:29:23.938697 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.938764 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1951 2023-04-19 12:29:23.938841 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1524 2023-04-19 12:29:23.938890 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.938948 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/__init__.py
--rw-r--r--   0        0        0     1315 2023-04-19 12:29:23.939027 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.metadata.json
--rw-r--r--   0        0        0     1457 2023-04-19 12:29:23.939086 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.939144 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1380 2023-04-19 12:29:23.939214 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.metadata.json
--rw-r--r--   0        0        0     2232 2023-04-19 12:29:23.939277 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.939341 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1393 2023-04-19 12:29:23.939412 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     2755 2023-04-19 12:29:23.939471 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.939529 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/__init__.py
--rw-r--r--   0        0        0     1730 2023-04-19 12:29:23.939601 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.metadata.json
--rw-r--r--   0        0        0     1956 2023-04-19 12:29:23.939664 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.939720 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/__init__.py
--rw-r--r--   0        0        0     1537 2023-04-19 12:29:23.939796 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.metadata.json
--rw-r--r--   0        0        0     2892 2023-04-19 12:29:23.939867 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.939922 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/__init__.py
--rw-r--r--   0        0        0     1565 2023-04-19 12:29:23.939984 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.metadata.json
--rw-r--r--   0        0        0     2894 2023-04-19 12:29:23.940038 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.py
--rw-r--r--   0        0        0     9085 2023-04-19 12:29:23.940142 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.940199 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.940267 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/__init__.py
--rw-r--r--   0        0        0     1496 2023-04-19 12:29:23.940345 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.metadata.json
--rw-r--r--   0        0        0     2391 2023-04-19 12:29:23.940408 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.940466 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/__init__.py
--rw-r--r--   0        0        0     1462 2023-04-19 12:29:23.940535 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.metadata.json
--rw-r--r--   0        0        0     2397 2023-04-19 12:29:23.940589 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.940649 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/__init__.py
--rw-r--r--   0        0        0     1450 2023-04-19 12:29:23.940721 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.metadata.json
--rw-r--r--   0        0        0     2415 2023-04-19 12:29:23.940779 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.940837 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/__init__.py
--rw-r--r--   0        0        0     1418 2023-04-19 12:29:23.940906 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.metadata.json
--rw-r--r--   0        0        0     2600 2023-04-19 12:29:23.940955 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.py
--rw-r--r--   0        0        0      215 2023-04-19 12:29:23.941012 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.941070 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-19 12:29:23.941158 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.metadata.json
--rw-r--r--   0        0        0      841 2023-04-19 12:29:23.941216 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.941280 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1249 2023-04-19 12:29:23.941353 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1002 2023-04-19 12:29:23.941409 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.941464 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/__init__.py
--rw-r--r--   0        0        0     1345 2023-04-19 12:29:23.941540 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.metadata.json
--rw-r--r--   0        0        0     4856 2023-04-19 12:29:23.941604 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.941667 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/__init__.py
--rw-r--r--   0        0        0     1365 2023-04-19 12:29:23.941749 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.metadata.json
--rw-r--r--   0        0        0     1249 2023-04-19 12:29:23.941809 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.941872 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1498 2023-04-19 12:29:23.941939 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2391 2023-04-19 12:29:23.942001 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.942073 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1498 2023-04-19 12:29:23.942161 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2337 2023-04-19 12:29:23.942224 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.942293 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/__init__.py
--rw-r--r--   0        0        0     1495 2023-04-19 12:29:23.942381 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.metadata.json
--rw-r--r--   0        0        0     2208 2023-04-19 12:29:23.942459 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.942526 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/__init__.py
--rw-r--r--   0        0        0     1453 2023-04-19 12:29:23.942602 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.metadata.json
--rw-r--r--   0        0        0     3046 2023-04-19 12:29:23.942673 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.942746 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/__init__.py
--rw-r--r--   0        0        0     1560 2023-04-19 12:29:23.942838 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.metadata.json
--rw-r--r--   0        0        0     2261 2023-04-19 12:29:23.942907 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.942969 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/__init__.py
--rw-r--r--   0        0        0     1456 2023-04-19 12:29:23.943038 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.metadata.json
--rw-r--r--   0        0        0     2543 2023-04-19 12:29:23.943097 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.943156 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/__init__.py
--rw-r--r--   0        0        0     1430 2023-04-19 12:29:23.943233 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.metadata.json
--rw-r--r--   0        0        0     2748 2023-04-19 12:29:23.943292 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.943362 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/__init__.py
--rw-r--r--   0        0        0     1432 2023-04-19 12:29:23.943440 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.metadata.json
--rw-r--r--   0        0        0     2228 2023-04-19 12:29:23.943501 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.943561 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/__init__.py
--rw-r--r--   0        0        0     1448 2023-04-19 12:29:23.943632 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.metadata.json
--rw-r--r--   0        0        0     2413 2023-04-19 12:29:23.943687 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.943748 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/__init__.py
--rw-r--r--   0        0        0     1475 2023-04-19 12:29:23.943818 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.metadata.json
--rw-r--r--   0        0        0     2203 2023-04-19 12:29:23.943882 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.943942 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/__init__.py
--rw-r--r--   0        0        0     1446 2023-04-19 12:29:23.944012 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.metadata.json
--rw-r--r--   0        0        0     2208 2023-04-19 12:29:23.944079 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.py
--rw-r--r--   0        0        0    10747 2023-04-19 12:29:23.944157 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_service.py
--rw-r--r--   0        0        0      197 2023-04-19 12:29:23.944212 prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/logs_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.944273 prowler_cloud-3.4.0/prowler/providers/aws/services/codeartifact/__init__.py
--rw-r--r--   0        0        0      234 2023-04-19 12:29:23.944347 prowler_cloud-3.4.0/prowler/providers/aws/services/codeartifact/codeartifact_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.944416 prowler_cloud-3.4.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/__init__.py
--rw-r--r--   0        0        0     1540 2023-04-19 12:29:23.944500 prowler_cloud-3.4.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.metadata.json
--rw-r--r--   0        0        0     1665 2023-04-19 12:29:23.944568 prowler_cloud-3.4.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.py
--rw-r--r--   0        0        0    10499 2023-04-19 12:29:23.944707 prowler_cloud-3.4.0/prowler/providers/aws/services/codeartifact/codeartifact_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.944765 prowler_cloud-3.4.0/prowler/providers/aws/services/codebuild/__init__.py
--rw-r--r--   0        0        0      210 2023-04-19 12:29:23.944830 prowler_cloud-3.4.0/prowler/providers/aws/services/codebuild/codebuild_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.944884 prowler_cloud-3.4.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/__init__.py
--rw-r--r--   0        0        0     1053 2023-04-19 12:29:23.944969 prowler_cloud-3.4.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.metadata.json
--rw-r--r--   0        0        0     1241 2023-04-19 12:29:23.945033 prowler_cloud-3.4.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.945096 prowler_cloud-3.4.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/__init__.py
--rw-r--r--   0        0        0     1018 2023-04-19 12:29:23.945184 prowler_cloud-3.4.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.metadata.json
--rw-r--r--   0        0        0     1049 2023-04-19 12:29:23.945366 prowler_cloud-3.4.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.py
--rw-r--r--   0        0        0     3606 2023-04-19 12:29:23.945608 prowler_cloud-3.4.0/prowler/providers/aws/services/codebuild/codebuild_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.945694 prowler_cloud-3.4.0/prowler/providers/aws/services/config/__init__.py
--rw-r--r--   0        0        0      195 2023-04-19 12:29:23.945780 prowler_cloud-3.4.0/prowler/providers/aws/services/config/config_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.945850 prowler_cloud-3.4.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/__init__.py
--rw-r--r--   0        0        0     1326 2023-04-19 12:29:23.945945 prowler_cloud-3.4.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.metadata.json
--rw-r--r--   0        0        0     1486 2023-04-19 12:29:23.946036 prowler_cloud-3.4.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.py
--rw-r--r--   0        0        0     3167 2023-04-19 12:29:23.946102 prowler_cloud-3.4.0/prowler/providers/aws/services/config/config_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.946178 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/__init__.py
--rw-r--r--   0        0        0      254 2023-04-19 12:29:23.946265 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.946353 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/__init__.py
--rw-r--r--   0        0        0     1191 2023-04-19 12:29:23.946439 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.metadata.json
--rw-r--r--   0        0        0      997 2023-04-19 12:29:23.946510 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.946579 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/__init__.py
--rw-r--r--   0        0        0     1187 2023-04-19 12:29:23.946679 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.metadata.json
--rw-r--r--   0        0        0     1041 2023-04-19 12:29:23.946756 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.946833 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/__init__.py
--rw-r--r--   0        0        0     1042 2023-04-19 12:29:23.946921 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.metadata.json
--rw-r--r--   0        0        0     1872 2023-04-19 12:29:23.946998 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.947066 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/__init__.py
--rw-r--r--   0        0        0     1098 2023-04-19 12:29:23.947152 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.metadata.json
--rw-r--r--   0        0        0     1660 2023-04-19 12:29:23.947219 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.947291 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/__init__.py
--rw-r--r--   0        0        0     1533 2023-04-19 12:29:23.947380 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.metadata.json
--rw-r--r--   0        0        0     1373 2023-04-19 12:29:23.947451 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.py
--rw-r--r--   0        0        0    12175 2023-04-19 12:29:23.947512 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.947590 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/__init__.py
--rw-r--r--   0        0        0     1265 2023-04-19 12:29:23.947677 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.metadata.json
--rw-r--r--   0        0        0     1269 2023-04-19 12:29:23.947755 prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.947825 prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/__init__.py
--rw-r--r--   0        0        0      190 2023-04-19 12:29:23.947904 prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dax_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.947975 prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1594 2023-04-19 12:29:23.948080 prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      957 2023-04-19 12:29:23.948147 prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.py
--rw-r--r--   0        0        0      205 2023-04-19 12:29:23.948205 prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_client.py
--rw-r--r--   0        0        0     8153 2023-04-19 12:29:23.948289 prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.948358 prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1497 2023-04-19 12:29:23.948440 prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      988 2023-04-19 12:29:23.948503 prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.948563 prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/__init__.py
--rw-r--r--   0        0        0     1529 2023-04-19 12:29:23.948637 prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.metadata.json
--rw-r--r--   0        0        0      933 2023-04-19 12:29:23.948691 prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.948749 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.948833 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ami_public/__init__.py
--rw-r--r--   0        0        0     1299 2023-04-19 12:29:23.948914 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.metadata.json
--rw-r--r--   0        0        0      843 2023-04-19 12:29:23.948970 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.949029 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.949092 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/__init__.py
--rw-r--r--   0        0        0     1192 2023-04-19 12:29:23.949180 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.metadata.json
--rw-r--r--   0        0        0      783 2023-04-19 12:29:23.949243 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.949304 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/__init__.py
--rw-r--r--   0        0        0     1176 2023-04-19 12:29:23.949464 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.metadata.json
--rw-r--r--   0        0        0      965 2023-04-19 12:29:23.949557 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.949630 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/__init__.py
--rw-r--r--   0        0        0     1530 2023-04-19 12:29:23.949725 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.metadata.json
--rw-r--r--   0        0        0      922 2023-04-19 12:29:23.949801 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.949868 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/__init__.py
--rw-r--r--   0        0        0     1239 2023-04-19 12:29:23.949957 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.metadata.json
--rw-r--r--   0        0        0      849 2023-04-19 12:29:23.950030 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.950097 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/__init__.py
--rw-r--r--   0        0        0     1057 2023-04-19 12:29:23.950180 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.metadata.json
--rw-r--r--   0        0        0     2037 2023-04-19 12:29:23.950242 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.950302 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/__init__.py
--rw-r--r--   0        0        0     1107 2023-04-19 12:29:23.950384 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.metadata.json
--rw-r--r--   0        0        0      971 2023-04-19 12:29:23.950439 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.950496 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/__init__.py
--rw-r--r--   0        0        0     1461 2023-04-19 12:29:23.950579 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.metadata.json
--rw-r--r--   0        0        0     1179 2023-04-19 12:29:23.950656 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.950724 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/__init__.py
--rw-r--r--   0        0        0     1067 2023-04-19 12:29:23.950816 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.metadata.json
--rw-r--r--   0        0        0     1111 2023-04-19 12:29:23.950882 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.950943 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/__init__.py
--rw-r--r--   0        0        0     1174 2023-04-19 12:29:23.951025 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.metadata.json
--rw-r--r--   0        0        0     1253 2023-04-19 12:29:23.951080 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.951148 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/__init__.py
--rw-r--r--   0        0        0     1201 2023-04-19 12:29:23.951220 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.metadata.json
--rw-r--r--   0        0        0     1491 2023-04-19 12:29:23.951290 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.951360 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/__init__.py
--rw-r--r--   0        0        0     1543 2023-04-19 12:29:23.951437 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.metadata.json
--rw-r--r--   0        0        0     1034 2023-04-19 12:29:23.951499 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.951556 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/__init__.py
--rw-r--r--   0        0        0     1141 2023-04-19 12:29:23.951627 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.metadata.json
--rw-r--r--   0        0        0     1118 2023-04-19 12:29:23.951691 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.951757 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/__init__.py
--rw-r--r--   0        0        0     1292 2023-04-19 12:29:23.951839 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.metadata.json
--rw-r--r--   0        0        0     2348 2023-04-19 12:29:23.951906 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.py
--rw-r--r--   0        0        0       78 2023-04-19 12:29:23.951997 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/fixtures/fixture
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.952059 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/__init__.py
--rw-r--r--   0        0        0     1378 2023-04-19 12:29:23.952133 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.metadata.json
--rw-r--r--   0        0        0     1247 2023-04-19 12:29:23.952190 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.952247 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/__init__.py
--rw-r--r--   0        0        0     1483 2023-04-19 12:29:23.952329 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.metadata.json
--rw-r--r--   0        0        0     1268 2023-04-19 12:29:23.952407 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.952471 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/__init__.py
--rw-r--r--   0        0        0     1513 2023-04-19 12:29:23.952556 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.metadata.json
--rw-r--r--   0        0        0     1296 2023-04-19 12:29:23.952633 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.952700 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/__init__.py
--rw-r--r--   0        0        0     1139 2023-04-19 12:29:23.952777 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.metadata.json
--rw-r--r--   0        0        0     1323 2023-04-19 12:29:23.952846 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.952917 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/__init__.py
--rw-r--r--   0        0        0     1197 2023-04-19 12:29:23.953015 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.metadata.json
--rw-r--r--   0        0        0     1468 2023-04-19 12:29:23.953101 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.953177 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/__init__.py
--rw-r--r--   0        0        0     1169 2023-04-19 12:29:23.953258 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.metadata.json
--rw-r--r--   0        0        0     1436 2023-04-19 12:29:23.953328 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.953390 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/__init__.py
--rw-r--r--   0        0        0     1429 2023-04-19 12:29:23.953489 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.metadata.json
--rw-r--r--   0        0        0     1409 2023-04-19 12:29:23.953553 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.953618 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/__init__.py
--rw-r--r--   0        0        0     1371 2023-04-19 12:29:23.953692 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.metadata.json
--rw-r--r--   0        0        0     1437 2023-04-19 12:29:23.953786 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.953865 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/__init__.py
--rw-r--r--   0        0        0     1220 2023-04-19 12:29:23.953950 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.metadata.json
--rw-r--r--   0        0        0     1497 2023-04-19 12:29:23.954013 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.954078 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-19 12:29:23.954157 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.metadata.json
--rw-r--r--   0        0        0     1532 2023-04-19 12:29:23.954241 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.954310 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/__init__.py
--rw-r--r--   0        0        0     1164 2023-04-19 12:29:23.954387 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.metadata.json
--rw-r--r--   0        0        0     1427 2023-04-19 12:29:23.954452 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.954527 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-19 12:29:23.954613 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.metadata.json
--rw-r--r--   0        0        0     1443 2023-04-19 12:29:23.954685 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.954805 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/__init__.py
--rw-r--r--   0        0        0     1165 2023-04-19 12:29:23.954886 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.metadata.json
--rw-r--r--   0        0        0     1486 2023-04-19 12:29:23.954956 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.955027 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/__init__.py
--rw-r--r--   0        0        0     1190 2023-04-19 12:29:23.955101 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.metadata.json
--rw-r--r--   0        0        0     1461 2023-04-19 12:29:23.955156 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.955225 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/__init__.py
--rw-r--r--   0        0        0     1173 2023-04-19 12:29:23.955470 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.metadata.json
--rw-r--r--   0        0        0     1436 2023-04-19 12:29:23.955638 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.955701 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/__init__.py
--rw-r--r--   0        0        0     1164 2023-04-19 12:29:23.955778 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.metadata.json
--rw-r--r--   0        0        0     1427 2023-04-19 12:29:23.955843 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.955937 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/__init__.py
--rw-r--r--   0        0        0     1218 2023-04-19 12:29:23.956030 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.metadata.json
--rw-r--r--   0        0        0     1499 2023-04-19 12:29:23.956108 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.956187 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/__init__.py
--rw-r--r--   0        0        0     1161 2023-04-19 12:29:23.956261 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.metadata.json
--rw-r--r--   0        0        0     1422 2023-04-19 12:29:23.956316 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.956378 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/__init__.py
--rw-r--r--   0        0        0     1127 2023-04-19 12:29:23.956461 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.metadata.json
--rw-r--r--   0        0        0     2440 2023-04-19 12:29:23.956526 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.956612 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/__init__.py
--rw-r--r--   0        0        0     1374 2023-04-19 12:29:23.956694 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.metadata.json
--rw-r--r--   0        0        0     1305 2023-04-19 12:29:23.956775 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.956843 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/__init__.py
--rw-r--r--   0        0        0     1221 2023-04-19 12:29:23.956915 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.metadata.json
--rw-r--r--   0        0        0     1029 2023-04-19 12:29:23.956978 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.957038 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/__init__.py
--rw-r--r--   0        0        0     1043 2023-04-19 12:29:23.957111 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.metadata.json
--rw-r--r--   0        0        0     1144 2023-04-19 12:29:23.957178 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.957238 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/__init__.py
--rw-r--r--   0        0        0     1080 2023-04-19 12:29:23.957327 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.metadata.json
--rw-r--r--   0        0        0     1219 2023-04-19 12:29:23.957388 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.py
--rw-r--r--   0        0        0    18754 2023-04-19 12:29:23.957527 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.957595 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/lib/__init__.py
--rw-r--r--   0        0        0     2581 2023-04-19 12:29:23.957667 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/lib/network_acls.py
--rw-r--r--   0        0        0     3766 2023-04-19 12:29:23.957735 prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/lib/security_groups.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.957793 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.957867 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.957926 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/__init__.py
--rw-r--r--   0        0        0     1375 2023-04-19 12:29:23.958354 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.metadata.json
--rw-r--r--   0        0        0     1302 2023-04-19 12:29:23.958488 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.958564 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/__init__.py
--rw-r--r--   0        0        0     1123 2023-04-19 12:29:23.958647 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.metadata.json
--rw-r--r--   0        0        0      973 2023-04-19 12:29:23.958715 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.958786 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1213 2023-04-19 12:29:23.958874 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1322 2023-04-19 12:29:23.958949 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.959014 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/__init__.py
--rw-r--r--   0        0        0     1501 2023-04-19 12:29:23.959140 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.metadata.json
--rw-r--r--   0        0        0      990 2023-04-19 12:29:23.959214 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.959276 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/__init__.py
--rw-r--r--   0        0        0     1268 2023-04-19 12:29:23.959354 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.metadata.json
--rw-r--r--   0        0        0     2034 2023-04-19 12:29:23.959422 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.py
--rw-r--r--   0        0        0    10008 2023-04-19 12:29:23.959556 prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.959623 prowler_cloud-3.4.0/prowler/providers/aws/services/ecs/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.959708 prowler_cloud-3.4.0/prowler/providers/aws/services/ecs/ecs_client.py
--rw-r--r--   0        0        0     3857 2023-04-19 12:29:23.959800 prowler_cloud-3.4.0/prowler/providers/aws/services/ecs/ecs_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.959863 prowler_cloud-3.4.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/__init__.py
--rw-r--r--   0        0        0     1625 2023-04-19 12:29:23.959946 prowler_cloud-3.4.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.metadata.json
--rw-r--r--   0        0        0     2328 2023-04-19 12:29:23.960011 prowler_cloud-3.4.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.960125 prowler_cloud-3.4.0/prowler/providers/aws/services/efs/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.960222 prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.960305 prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/__init__.py
--rw-r--r--   0        0        0     1366 2023-04-19 12:29:23.960396 prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.metadata.json
--rw-r--r--   0        0        0      853 2023-04-19 12:29:23.960463 prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.960528 prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/__init__.py
--rw-r--r--   0        0        0     1099 2023-04-19 12:29:23.960600 prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.metadata.json
--rw-r--r--   0        0        0      843 2023-04-19 12:29:23.960658 prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.960737 prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0      981 2023-04-19 12:29:23.960839 prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1853 2023-04-19 12:29:23.960935 prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.py
--rw-r--r--   0        0        0     3889 2023-04-19 12:29:23.961042 prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.961116 prowler_cloud-3.4.0/prowler/providers/aws/services/eks/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.961185 prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.961253 prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/__init__.py
--rw-r--r--   0        0        0     1362 2023-04-19 12:29:23.961335 prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.metadata.json
--rw-r--r--   0        0        0      992 2023-04-19 12:29:23.961410 prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.961481 prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/__init__.py
--rw-r--r--   0        0        0     1559 2023-04-19 12:29:23.961578 prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.metadata.json
--rw-r--r--   0        0        0     1215 2023-04-19 12:29:23.961639 prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.961713 prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/__init__.py
--rw-r--r--   0        0        0     1374 2023-04-19 12:29:23.961815 prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.metadata.json
--rw-r--r--   0        0        0     1489 2023-04-19 12:29:23.961889 prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.961959 prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1533 2023-04-19 12:29:23.962044 prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1020 2023-04-19 12:29:23.962138 prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.py
--rw-r--r--   0        0        0     4579 2023-04-19 12:29:23.962243 prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.962323 prowler_cloud-3.4.0/prowler/providers/aws/services/elb/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.962401 prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.962478 prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/__init__.py
--rw-r--r--   0        0        0     1364 2023-04-19 12:29:23.962564 prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.metadata.json
--rw-r--r--   0        0        0     1115 2023-04-19 12:29:23.962633 prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.962724 prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_internet_facing/__init__.py
--rw-r--r--   0        0        0     1111 2023-04-19 12:29:23.962884 prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.metadata.json
--rw-r--r--   0        0        0      823 2023-04-19 12:29:23.963014 prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.963091 prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1392 2023-04-19 12:29:23.963168 prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.metadata.json
--rw-r--r--   0        0        0      817 2023-04-19 12:29:23.963238 prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.py
--rw-r--r--   0        0        0     4592 2023-04-19 12:29:23.963365 prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.963437 prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_ssl_listeners/__init__.py
--rw-r--r--   0        0        0     1360 2023-04-19 12:29:23.963512 prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.metadata.json
--rw-r--r--   0        0        0      937 2023-04-19 12:29:23.963596 prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.963667 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/__init__.py
--rw-r--r--   0        0        0      190 2023-04-19 12:29:23.963732 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.963789 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/__init__.py
--rw-r--r--   0        0        0     1347 2023-04-19 12:29:23.963879 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.metadata.json
--rw-r--r--   0        0        0      892 2023-04-19 12:29:23.963953 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.964013 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/__init__.py
--rw-r--r--   0        0        0     1718 2023-04-19 12:29:23.964087 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.metadata.json
--rw-r--r--   0        0        0     1367 2023-04-19 12:29:23.964151 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.964211 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/__init__.py
--rw-r--r--   0        0        0     1337 2023-04-19 12:29:23.964275 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.metadata.json
--rw-r--r--   0        0        0     1646 2023-04-19 12:29:23.964347 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.964420 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/__init__.py
--rw-r--r--   0        0        0     1162 2023-04-19 12:29:23.964495 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.metadata.json
--rw-r--r--   0        0        0      888 2023-04-19 12:29:23.964568 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.964639 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/__init__.py
--rw-r--r--   0        0        0      996 2023-04-19 12:29:23.964720 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.metadata.json
--rw-r--r--   0        0        0      836 2023-04-19 12:29:23.964781 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.964855 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1435 2023-04-19 12:29:23.964939 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.metadata.json
--rw-r--r--   0        0        0      924 2023-04-19 12:29:23.965007 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.py
--rw-r--r--   0        0        0     7882 2023-04-19 12:29:23.965093 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.965174 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/__init__.py
--rw-r--r--   0        0        0     1325 2023-04-19 12:29:23.965247 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.metadata.json
--rw-r--r--   0        0        0     1664 2023-04-19 12:29:23.965315 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.965389 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/__init__.py
--rw-r--r--   0        0        0     1004 2023-04-19 12:29:23.965478 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.metadata.json
--rw-r--r--   0        0        0     1439 2023-04-19 12:29:23.965558 prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.965631 prowler_cloud-3.4.0/prowler/providers/aws/services/emr/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.965708 prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.965783 prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/__init__.py
--rw-r--r--   0        0        0     1029 2023-04-19 12:29:23.965875 prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.metadata.json
--rw-r--r--   0        0        0      917 2023-04-19 12:29:23.965953 prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.966035 prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/__init__.py
--rw-r--r--   0        0        0      897 2023-04-19 12:29:23.966124 prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.metadata.json
--rw-r--r--   0        0        0     1200 2023-04-19 12:29:23.966202 prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.966274 prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/__init__.py
--rw-r--r--   0        0        0     1018 2023-04-19 12:29:23.966359 prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.metadata.json
--rw-r--r--   0        0        0     4444 2023-04-19 12:29:23.966445 prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.py
--rw-r--r--   0        0        0     7714 2023-04-19 12:29:23.966535 prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.966618 prowler_cloud-3.4.0/prowler/providers/aws/services/glacier/__init__.py
--rw-r--r--   0        0        0      200 2023-04-19 12:29:23.966702 prowler_cloud-3.4.0/prowler/providers/aws/services/glacier/glacier_client.py
--rw-r--r--   0        0        0     3995 2023-04-19 12:29:23.966792 prowler_cloud-3.4.0/prowler/providers/aws/services/glacier/glacier_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.966878 prowler_cloud-3.4.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/__init__.py
--rw-r--r--   0        0        0     1219 2023-04-19 12:29:23.966963 prowler_cloud-3.4.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.metadata.json
--rw-r--r--   0        0        0     1940 2023-04-19 12:29:23.967043 prowler_cloud-3.4.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.967105 prowler_cloud-3.4.0/prowler/providers/aws/services/globalaccelerator/__init__.py
--rw-r--r--   0        0        0      259 2023-04-19 12:29:23.967180 prowler_cloud-3.4.0/prowler/providers/aws/services/globalaccelerator/globalaccelerator_client.py
--rw-r--r--   0        0        0     2362 2023-04-19 12:29:23.967253 prowler_cloud-3.4.0/prowler/providers/aws/services/globalaccelerator/globalaccelerator_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.967325 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/__init__.py
--rw-r--r--   0        0        0      185 2023-04-19 12:29:23.967397 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.967474 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1464 2023-04-19 12:29:23.967574 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      928 2023-04-19 12:29:23.967664 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.967737 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1539 2023-04-19 12:29:23.967812 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      920 2023-04-19 12:29:23.967877 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.967951 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/__init__.py
--rw-r--r--   0        0        0     1222 2023-04-19 12:29:23.968034 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.metadata.json
--rw-r--r--   0        0        0      884 2023-04-19 12:29:23.968106 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.968182 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1632 2023-04-19 12:29:23.968257 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1361 2023-04-19 12:29:23.968320 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.968383 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1623 2023-04-19 12:29:23.968454 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1352 2023-04-19 12:29:23.968520 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.968592 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1644 2023-04-19 12:29:23.968667 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1322 2023-04-19 12:29:23.968732 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.968797 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1574 2023-04-19 12:29:23.968878 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1622 2023-04-19 12:29:23.968944 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.969022 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1600 2023-04-19 12:29:23.969110 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1293 2023-04-19 12:29:23.969174 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.969240 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1591 2023-04-19 12:29:23.969311 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1284 2023-04-19 12:29:23.969372 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.py
--rw-r--r--   0        0        0     9722 2023-04-19 12:29:23.969452 prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.969509 prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.969576 prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/__init__.py
--rw-r--r--   0        0        0      998 2023-04-19 12:29:23.969697 prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.metadata.json
--rw-r--r--   0        0        0     1221 2023-04-19 12:29:23.969805 prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.py
--rw-r--r--   0        0        0      210 2023-04-19 12:29:23.969867 prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.969929 prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/__init__.py
--rw-r--r--   0        0        0     1282 2023-04-19 12:29:23.970039 prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.metadata.json
--rw-r--r--   0        0        0     1130 2023-04-19 12:29:23.970105 prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.970169 prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-19 12:29:23.970275 prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.metadata.json
--rw-r--r--   0        0        0      961 2023-04-19 12:29:23.970332 prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.py
--rw-r--r--   0        0        0     7252 2023-04-19 12:29:23.970460 prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.970527 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.970612 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/__init__.py
--rw-r--r--   0        0        0     1010 2023-04-19 12:29:23.970708 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.metadata.json
--rw-r--r--   0        0        0     1933 2023-04-19 12:29:23.970784 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.970861 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/__init__.py
--rw-r--r--   0        0        0     1112 2023-04-19 12:29:23.970944 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.metadata.json
--rw-r--r--   0        0        0     2805 2023-04-19 12:29:23.971012 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.py
--rw-r--r--   0        0        0        0 2023-04-19 14:30:31.789842 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/__init__.py
--rw-r--r--   0        0        0     2073 2023-04-19 14:30:31.790116 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.metadata.json
--rw-r--r--   0        0        0     2227 2023-04-19 14:30:31.790324 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.971078 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/__init__.py
--rw-r--r--   0        0        0     1494 2023-04-19 12:29:23.971163 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.metadata.json
--rw-r--r--   0        0        0      802 2023-04-19 12:29:23.971231 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.971296 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_client.py
--rw-r--r--   0        0        0        0 2023-04-19 14:30:31.790386 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/__init__.py
--rw-r--r--   0        0        0     2088 2023-04-19 14:30:31.790500 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.metadata.json
--rw-r--r--   0        0        0     2238 2023-04-19 14:30:31.790593 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.py
--rw-r--r--   0        0        0        0 2023-04-19 14:30:31.790657 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/__init__.py
--rw-r--r--   0        0        0     2118 2023-04-19 14:30:31.790778 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.metadata.json
--rw-r--r--   0        0        0     2251 2023-04-19 14:30:31.790879 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.971377 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/__init__.py
--rw-r--r--   0        0        0     1413 2023-04-19 12:29:23.971535 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.metadata.json
--rw-r--r--   0        0        0     4192 2023-04-19 12:29:23.971628 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.971705 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/__init__.py
--rw-r--r--   0        0        0     1413 2023-04-19 12:29:23.971792 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.metadata.json
--rw-r--r--   0        0        0     4146 2023-04-19 12:29:23.971858 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.971926 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/__init__.py
--rw-r--r--   0        0        0     1417 2023-04-19 12:29:23.972003 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.metadata.json
--rw-r--r--   0        0        0     4192 2023-04-19 12:29:23.972081 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.972166 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/__init__.py
--rw-r--r--   0        0        0     1089 2023-04-19 12:29:23.972256 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.metadata.json
--rw-r--r--   0        0        0     2665 2023-04-19 14:30:31.791220 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.972389 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/__init__.py
--rw-r--r--   0        0        0     1707 2023-04-19 12:29:23.972482 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.metadata.json
--rw-r--r--   0        0        0     1090 2023-04-19 12:29:23.972558 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.972624 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_no_root_access_key/__init__.py
--rw-r--r--   0        0        0     1453 2023-04-19 12:29:23.972706 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.metadata.json
--rw-r--r--   0        0        0     1541 2023-04-19 12:29:23.972769 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.972838 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/__init__.py
--rw-r--r--   0        0        0     1314 2023-04-19 12:29:23.972940 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.metadata.json
--rw-r--r--   0        0        0     1360 2023-04-19 12:29:23.973008 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.973071 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/__init__.py
--rw-r--r--   0        0        0     1299 2023-04-19 12:29:23.973150 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.metadata.json
--rw-r--r--   0        0        0     1086 2023-04-19 12:29:23.973217 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.973285 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/__init__.py
--rw-r--r--   0        0        0     1299 2023-04-19 12:29:23.973378 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.metadata.json
--rw-r--r--   0        0        0     1185 2023-04-19 12:29:23.973440 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.973504 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_number/__init__.py
--rw-r--r--   0        0        0     1254 2023-04-19 12:29:23.973578 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.metadata.json
--rw-r--r--   0        0        0     1095 2023-04-19 12:29:23.973645 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.973709 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/__init__.py
--rw-r--r--   0        0        0     1280 2023-04-19 12:29:23.973792 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.metadata.json
--rw-r--r--   0        0        0     1231 2023-04-19 12:29:23.973863 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.973931 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/__init__.py
--rw-r--r--   0        0        0     1294 2023-04-19 12:29:23.974020 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.metadata.json
--rw-r--r--   0        0        0     1095 2023-04-19 12:29:23.974086 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.974151 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/__init__.py
--rw-r--r--   0        0        0     1300 2023-04-19 12:29:23.974224 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.metadata.json
--rw-r--r--   0        0        0     1083 2023-04-19 12:29:23.974290 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.974357 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/__init__.py
--rw-r--r--   0        0        0     1223 2023-04-19 12:29:23.974457 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.metadata.json
--rw-r--r--   0        0        0     6229 2023-04-19 14:30:31.791478 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.974606 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/__init__.py
--rw-r--r--   0        0        0     1533 2023-04-19 12:29:23.974689 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.metadata.json
--rw-r--r--   0        0        0     1925 2023-04-19 12:29:23.974757 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.975046 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/__init__.py
--rw-r--r--   0        0        0     1384 2023-04-19 12:29:23.975177 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.metadata.json
--rw-r--r--   0        0        0     2059 2023-04-19 14:30:31.791710 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.975347 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/__init__.py
--rw-r--r--   0        0        0     1356 2023-04-19 12:29:23.975454 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.metadata.json
--rw-r--r--   0        0        0     2045 2023-04-19 14:30:31.791846 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.975766 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/__init__.py
--rw-r--r--   0        0        0     1174 2023-04-19 12:29:23.975851 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.metadata.json
--rw-r--r--   0        0        0     3419 2023-04-19 12:29:23.975921 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.975982 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/__init__.py
--rw-r--r--   0        0        0     1424 2023-04-19 12:29:23.976060 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.metadata.json
--rw-r--r--   0        0        0     1595 2023-04-19 12:29:23.976119 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.976178 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/__init__.py
--rw-r--r--   0        0        0     1738 2023-04-19 12:29:23.976255 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.metadata.json
--rw-r--r--   0        0        0     1020 2023-04-19 12:29:23.976311 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.976377 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/__init__.py
--rw-r--r--   0        0        0     1424 2023-04-19 12:29:23.976446 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.metadata.json
--rw-r--r--   0        0        0     2832 2023-04-19 12:29:23.976523 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.976606 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/__init__.py
--rw-r--r--   0        0        0     1335 2023-04-19 12:29:23.976734 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.metadata.json
--rw-r--r--   0        0        0      901 2023-04-19 12:29:23.976840 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.py
--rw-r--r--   0        0        0    21365 2023-04-19 14:30:31.792148 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.977064 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_support_role_created/__init__.py
--rw-r--r--   0        0        0     1256 2023-04-19 12:29:23.977144 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.metadata.json
--rw-r--r--   0        0        0      940 2023-04-19 12:29:23.977241 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.977300 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/__init__.py
--rw-r--r--   0        0        0     1061 2023-04-19 12:29:23.977369 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.metadata.json
--rw-r--r--   0        0        0     1341 2023-04-19 12:29:23.977431 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.977490 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/__init__.py
--rw-r--r--   0        0        0     1309 2023-04-19 12:29:23.977576 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.metadata.json
--rw-r--r--   0        0        0     1698 2023-04-19 12:29:23.977650 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.977716 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/__init__.py
--rw-r--r--   0        0        0     1671 2023-04-19 12:29:23.977798 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.metadata.json
--rw-r--r--   0        0        0     2671 2023-04-19 12:29:23.977863 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.977919 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/__init__.py
--rw-r--r--   0        0        0      998 2023-04-19 12:29:23.977991 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.metadata.json
--rw-r--r--   0        0        0     1341 2023-04-19 12:29:23.978054 prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.978113 prowler_cloud-3.4.0/prowler/providers/aws/services/kms/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.978191 prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.978250 prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_cmk_are_used/__init__.py
--rw-r--r--   0        0        0     1053 2023-04-19 12:29:23.978323 prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.metadata.json
--rw-r--r--   0        0        0     1194 2023-04-19 12:29:23.978399 prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.978466 prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/__init__.py
--rw-r--r--   0        0        0     1309 2023-04-19 12:29:23.978546 prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.metadata.json
--rw-r--r--   0        0        0     1294 2023-04-19 12:29:23.978604 prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.978665 prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1354 2023-04-19 12:29:23.978738 prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     2525 2023-04-19 12:29:23.978835 prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py
--rw-r--r--   0        0        0     5255 2023-04-19 12:29:23.978919 prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.978985 prowler_cloud-3.4.0/prowler/providers/aws/services/macie/__init__.py
--rw-r--r--   0        0        0      190 2023-04-19 12:29:23.979068 prowler_cloud-3.4.0/prowler/providers/aws/services/macie/macie_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.979172 prowler_cloud-3.4.0/prowler/providers/aws/services/macie/macie_is_enabled/__init__.py
--rw-r--r--   0        0        0     1065 2023-04-19 12:29:23.979278 prowler_cloud-3.4.0/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.metadata.json
--rw-r--r--   0        0        0      894 2023-04-19 12:29:23.979368 prowler_cloud-3.4.0/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.py
--rw-r--r--   0        0        0     1785 2023-04-19 12:29:23.979447 prowler_cloud-3.4.0/prowler/providers/aws/services/macie/macie_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.979538 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/__init__.py
--rw-r--r--   0        0        0      238 2023-04-19 12:29:23.979628 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_client.py
--rw-r--r--   0        0        0     6959 2023-04-19 12:29:23.979719 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.979801 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1124 2023-04-19 12:29:23.979914 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1102 2023-04-19 12:29:23.979989 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.980060 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1478 2023-04-19 12:29:23.980138 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1871 2023-04-19 12:29:23.980196 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.980261 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/__init__.py
--rw-r--r--   0        0        0     1555 2023-04-19 12:29:23.980344 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.metadata.json
--rw-r--r--   0        0        0     1003 2023-04-19 12:29:23.980412 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.980494 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/__init__.py
--rw-r--r--   0        0        0     1281 2023-04-19 12:29:23.980571 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.metadata.json
--rw-r--r--   0        0        0      991 2023-04-19 12:29:23.980633 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.980699 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/__init__.py
--rw-r--r--   0        0        0     1128 2023-04-19 12:29:23.980766 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.metadata.json
--rw-r--r--   0        0        0      983 2023-04-19 12:29:23.980826 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.980887 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1766 2023-04-19 12:29:23.980964 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1023 2023-04-19 12:29:23.981024 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.981096 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1281 2023-04-19 12:29:23.981163 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     2655 2023-04-19 12:29:23.981223 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.981286 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/__init__.py
--rw-r--r--   0        0        0     1736 2023-04-19 12:29:23.981364 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.metadata.json
--rw-r--r--   0        0        0     1046 2023-04-19 12:29:23.981430 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.981492 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/__init__.py
--rw-r--r--   0        0        0     1242 2023-04-19 12:29:23.981574 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.metadata.json
--rw-r--r--   0        0        0     1023 2023-04-19 12:29:23.981643 prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.981710 prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.981781 prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/__init__.py
--rw-r--r--   0        0        0     1359 2023-04-19 12:29:23.981880 prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.metadata.json
--rw-r--r--   0        0        0      984 2023-04-19 12:29:23.981978 prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.py
--rw-r--r--   0        0        0      239 2023-04-19 12:29:23.982039 prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.982100 prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/__init__.py
--rw-r--r--   0        0        0     1579 2023-04-19 12:29:23.982181 prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.metadata.json
--rw-r--r--   0        0        0     1816 2023-04-19 12:29:23.982292 prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.982372 prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/__init__.py
--rw-r--r--   0        0        0     1548 2023-04-19 12:29:23.982458 prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.metadata.json
--rw-r--r--   0        0        0     5605 2023-04-19 12:29:23.982567 prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.py
--rw-r--r--   0        0        0     8903 2023-04-19 12:29:23.982687 prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.982747 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.982808 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.982868 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/__init__.py
--rw-r--r--   0        0        0     1473 2023-04-19 12:29:23.982939 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.metadata.json
--rw-r--r--   0        0        0      984 2023-04-19 12:29:23.983003 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.983065 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/__init__.py
--rw-r--r--   0        0        0     1367 2023-04-19 12:29:23.983129 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.metadata.json
--rw-r--r--   0        0        0      980 2023-04-19 12:29:23.983184 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.983243 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/__init__.py
--rw-r--r--   0        0        0     1309 2023-04-19 12:29:23.983318 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.metadata.json
--rw-r--r--   0        0        0      960 2023-04-19 12:29:23.983380 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.983450 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/__init__.py
--rw-r--r--   0        0        0     1488 2023-04-19 12:29:23.983528 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.metadata.json
--rw-r--r--   0        0        0      947 2023-04-19 12:29:23.983588 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.983654 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/__init__.py
--rw-r--r--   0        0        0     1732 2023-04-19 12:29:23.983734 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.metadata.json
--rw-r--r--   0        0        0      969 2023-04-19 12:29:23.983790 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.983846 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_multi_az/__init__.py
--rw-r--r--   0        0        0     1309 2023-04-19 12:29:23.983913 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.metadata.json
--rw-r--r--   0        0        0      944 2023-04-19 12:29:23.983967 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.984024 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/__init__.py
--rw-r--r--   0        0        0     1426 2023-04-19 12:29:23.984110 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.metadata.json
--rw-r--r--   0        0        0      959 2023-04-19 12:29:23.984175 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.984238 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/__init__.py
--rw-r--r--   0        0        0     1370 2023-04-19 12:29:23.984322 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.metadata.json
--rw-r--r--   0        0        0      892 2023-04-19 12:29:23.984376 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.984438 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/__init__.py
--rw-r--r--   0        0        0     1510 2023-04-19 12:29:23.984507 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.metadata.json
--rw-r--r--   0        0        0     1367 2023-04-20 13:29:08.794503 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.py
--rw-r--r--   0        0        0    10647 2023-04-19 12:29:23.984614 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.984675 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/__init__.py
--rw-r--r--   0        0        0     1552 2023-04-19 12:29:23.984750 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.metadata.json
--rw-r--r--   0        0        0     1543 2023-04-19 12:29:23.984811 prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.984870 prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/__init__.py
--rw-r--r--   0        0        0      205 2023-04-19 12:29:23.984935 prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.985000 prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/__init__.py
--rw-r--r--   0        0        0     1384 2023-04-19 12:29:23.985070 prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.metadata.json
--rw-r--r--   0        0        0      973 2023-04-19 12:29:23.985129 prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.985188 prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/__init__.py
--rw-r--r--   0        0        0     1204 2023-04-19 12:29:23.985268 prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.metadata.json
--rw-r--r--   0        0        0      984 2023-04-19 12:29:23.985335 prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.985415 prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/__init__.py
--rw-r--r--   0        0        0     1285 2023-04-20 13:29:08.795139 prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.metadata.json
--rw-r--r--   0        0        0      996 2023-04-19 12:29:23.985566 prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.985646 prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/__init__.py
--rw-r--r--   0        0        0     1297 2023-04-19 12:29:23.985733 prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.metadata.json
--rw-r--r--   0        0        0      992 2023-04-19 12:29:23.985798 prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.py
--rw-r--r--   0        0        0     4912 2023-04-19 12:29:23.985905 prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.985981 prowler_cloud-3.4.0/prowler/providers/aws/services/resourceexplorer2/__init__.py
--rw-r--r--   0        0        0      261 2023-04-19 12:29:23.986103 prowler_cloud-3.4.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.986181 prowler_cloud-3.4.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/__init__.py
--rw-r--r--   0        0        0      973 2023-04-19 12:29:23.986311 prowler_cloud-3.4.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.metadata.json
--rw-r--r--   0        0        0      940 2023-04-19 12:29:23.986424 prowler_cloud-3.4.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.py
--rw-r--r--   0        0        0     2344 2023-04-19 12:29:23.986545 prowler_cloud-3.4.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.986621 prowler_cloud-3.4.0/prowler/providers/aws/services/route53/__init__.py
--rw-r--r--   0        0        0      200 2023-04-19 12:29:23.986702 prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.986785 prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/__init__.py
--rw-r--r--   0        0        0     1188 2023-04-19 12:29:23.986873 prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.metadata.json
--rw-r--r--   0        0        0     1023 2023-04-19 12:29:23.986944 prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.987014 prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/__init__.py
--rw-r--r--   0        0        0      998 2023-04-19 12:29:23.987103 prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.metadata.json
--rw-r--r--   0        0        0     1058 2023-04-19 12:29:23.987177 prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.987269 prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1362 2023-04-19 12:29:23.987366 prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1249 2023-04-19 12:29:23.987444 prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.py
--rw-r--r--   0        0        0     6911 2023-04-19 12:29:23.987538 prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_service.py
--rw-r--r--   0        0        0      221 2023-04-19 12:29:23.987613 prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53domains_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.987693 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.987787 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/__init__.py
--rw-r--r--   0        0        0     1392 2023-04-19 12:29:23.987884 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.metadata.json
--rw-r--r--   0        0        0     1068 2023-04-19 12:29:23.987956 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.988015 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/__init__.py
--rw-r--r--   0        0        0     1266 2023-04-19 12:29:23.988088 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.metadata.json
--rw-r--r--   0        0        0      957 2023-04-19 12:29:23.988152 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.988226 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/__init__.py
--rw-r--r--   0        0        0     1459 2023-04-19 12:29:23.988319 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.metadata.json
--rw-r--r--   0        0        0      917 2023-04-19 12:29:23.988387 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.988462 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/__init__.py
--rw-r--r--   0        0        0     1496 2023-04-19 12:29:23.988553 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.metadata.json
--rw-r--r--   0        0        0     1123 2023-04-19 12:29:23.988658 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.988729 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/__init__.py
--rw-r--r--   0        0        0     1426 2023-04-19 12:29:23.988821 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.metadata.json
--rw-r--r--   0        0        0      943 2023-04-19 12:29:23.988889 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.988968 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-19 12:29:23.989059 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.metadata.json
--rw-r--r--   0        0        0      947 2023-04-19 12:29:23.989147 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.989246 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/__init__.py
--rw-r--r--   0        0        0     1080 2023-04-19 12:29:23.989355 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.metadata.json
--rw-r--r--   0        0        0     1716 2023-04-19 12:29:23.989421 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.989491 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_public_access/__init__.py
--rw-r--r--   0        0        0     1939 2023-04-19 12:29:23.989572 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.metadata.json
--rw-r--r--   0        0        0     4014 2023-04-19 12:29:23.989689 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.989751 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/__init__.py
--rw-r--r--   0        0        0     1190 2023-04-19 12:29:23.989835 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.metadata.json
--rw-r--r--   0        0        0     2099 2023-04-19 12:29:23.989900 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.989969 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1372 2023-04-19 12:29:23.990050 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.metadata.json
--rw-r--r--   0        0        0      978 2023-04-19 12:29:23.990109 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.py
--rw-r--r--   0        0        0      175 2023-04-19 12:29:23.990183 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_client.py
--rw-r--r--   0        0        0    14801 2023-04-19 12:29:23.990265 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_service.py
--rw-r--r--   0        0        0      196 2023-04-19 12:29:23.990316 prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3control_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.990374 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/__init__.py
--rw-r--r--   0        0        0      210 2023-04-19 12:29:23.990438 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.990496 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/__init__.py
--rw-r--r--   0        0        0     1100 2023-04-19 12:29:23.990579 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.metadata.json
--rw-r--r--   0        0        0      945 2023-04-19 12:29:23.990641 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.990707 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/__init__.py
--rw-r--r--   0        0        0     1094 2023-04-19 12:29:23.990791 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.metadata.json
--rw-r--r--   0        0        0      966 2023-04-19 12:29:23.990864 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.990928 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1412 2023-04-19 12:29:23.991009 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1046 2023-04-19 12:29:23.991068 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.991133 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/__init__.py
--rw-r--r--   0        0        0     1227 2023-04-19 12:29:23.991201 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.metadata.json
--rw-r--r--   0        0        0     1037 2023-04-19 12:29:23.991261 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.991361 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/__init__.py
--rw-r--r--   0        0        0     1361 2023-04-19 12:29:23.991468 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.metadata.json
--rw-r--r--   0        0        0     1063 2023-04-19 12:29:23.991540 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.991611 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/__init__.py
--rw-r--r--   0        0        0     1524 2023-04-19 12:29:23.991699 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.metadata.json
--rw-r--r--   0        0        0     1091 2023-04-19 12:29:23.991760 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.py
--rw-r--r--   0        0        0    11132 2023-04-19 12:29:23.991819 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.991885 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1119 2023-04-19 12:29:23.991978 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1040 2023-04-19 12:29:23.992040 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.992106 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/__init__.py
--rw-r--r--   0        0        0     1106 2023-04-19 12:29:23.992184 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.metadata.json
--rw-r--r--   0        0        0     1005 2023-04-19 12:29:23.992243 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.992305 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-19 12:29:23.992378 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1042 2023-04-19 12:29:23.992438 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.992502 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/__init__.py
--rw-r--r--   0        0        0     1100 2023-04-19 12:29:23.992573 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.metadata.json
--rw-r--r--   0        0        0     1072 2023-04-19 12:29:23.992638 prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.992702 prowler_cloud-3.4.0/prowler/providers/aws/services/secretsmanager/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.992781 prowler_cloud-3.4.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/__init__.py
--rw-r--r--   0        0        0     1341 2023-04-19 12:29:23.992866 prowler_cloud-3.4.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.metadata.json
--rw-r--r--   0        0        0     1054 2023-04-19 12:29:23.992929 prowler_cloud-3.4.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.py
--rw-r--r--   0        0        0      244 2023-04-19 12:29:23.992979 prowler_cloud-3.4.0/prowler/providers/aws/services/secretsmanager/secretsmanager_client.py
--rw-r--r--   0        0        0     2442 2023-04-19 12:29:23.993056 prowler_cloud-3.4.0/prowler/providers/aws/services/secretsmanager/secretsmanager_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.993113 prowler_cloud-3.4.0/prowler/providers/aws/services/securityhub/__init__.py
--rw-r--r--   0        0        0      220 2023-04-19 12:29:23.993184 prowler_cloud-3.4.0/prowler/providers/aws/services/securityhub/securityhub_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.993254 prowler_cloud-3.4.0/prowler/providers/aws/services/securityhub/securityhub_enabled/__init__.py
--rw-r--r--   0        0        0     1315 2023-04-19 12:29:23.993329 prowler_cloud-3.4.0/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.metadata.json
--rw-r--r--   0        0        0     1296 2023-04-19 12:29:23.993393 prowler_cloud-3.4.0/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.py
--rw-r--r--   0        0        0     4490 2023-04-19 12:29:23.993473 prowler_cloud-3.4.0/prowler/providers/aws/services/securityhub/securityhub_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.993540 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.993616 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/__init__.py
--rw-r--r--   0        0        0     1051 2023-04-19 12:29:23.993699 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.metadata.json
--rw-r--r--   0        0        0     1259 2023-04-19 12:29:23.993773 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.993837 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/__init__.py
--rw-r--r--   0        0        0     1045 2023-04-19 12:29:23.993917 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.metadata.json
--rw-r--r--   0        0        0     1267 2023-04-19 12:29:23.993973 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.994037 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/__init__.py
--rw-r--r--   0        0        0     1041 2023-04-19 12:29:23.994115 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.metadata.json
--rw-r--r--   0        0        0     1316 2023-04-19 12:29:23.994182 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.994249 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/__init__.py
--rw-r--r--   0        0        0     1021 2023-04-19 12:29:23.994335 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.metadata.json
--rw-r--r--   0        0        0     1271 2023-04-19 12:29:23.994405 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.994473 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/__init__.py
--rw-r--r--   0        0        0     1095 2023-04-19 12:29:23.994548 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.metadata.json
--rw-r--r--   0        0        0     1353 2023-04-19 12:29:23.994604 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.994667 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/__init__.py
--rw-r--r--   0        0        0     1020 2023-04-19 12:29:23.994734 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.metadata.json
--rw-r--r--   0        0        0     1275 2023-04-19 12:29:23.994798 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.py
--rw-r--r--   0        0        0      195 2023-04-19 12:29:23.994856 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_client.py
--rw-r--r--   0        0        0     2527 2023-04-19 12:29:23.994929 prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.994989 prowler_cloud-3.4.0/prowler/providers/aws/services/sns/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.995057 prowler_cloud-3.4.0/prowler/providers/aws/services/sns/sns_client.py
--rw-r--r--   0        0        0     3814 2023-04-19 12:29:23.995137 prowler_cloud-3.4.0/prowler/providers/aws/services/sns/sns_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.995195 prowler_cloud-3.4.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/__init__.py
--rw-r--r--   0        0        0     1283 2023-04-19 12:29:23.995275 prowler_cloud-3.4.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.metadata.json
--rw-r--r--   0        0        0      841 2023-04-19 12:29:23.995345 prowler_cloud-3.4.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.995410 prowler_cloud-3.4.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1340 2023-04-19 12:29:23.995514 prowler_cloud-3.4.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1921 2023-04-19 12:29:23.995571 prowler_cloud-3.4.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.995633 prowler_cloud-3.4.0/prowler/providers/aws/services/sqs/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.995710 prowler_cloud-3.4.0/prowler/providers/aws/services/sqs/sqs_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.995775 prowler_cloud-3.4.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1396 2023-04-19 12:29:23.995846 prowler_cloud-3.4.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1933 2023-04-19 12:29:23.995899 prowler_cloud-3.4.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.995957 prowler_cloud-3.4.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1479 2023-04-19 12:29:23.996042 prowler_cloud-3.4.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      939 2023-04-19 12:29:23.996103 prowler_cloud-3.4.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.py
--rw-r--r--   0        0        0     4137 2023-04-19 12:29:23.996159 prowler_cloud-3.4.0/prowler/providers/aws/services/sqs/sqs_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.996219 prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.996281 prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.996339 prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_document_secrets/__init__.py
--rw-r--r--   0        0        0     1225 2023-04-19 12:29:23.996410 prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.metadata.json
--rw-r--r--   0        0        0     1974 2023-04-19 12:29:23.996483 prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.996550 prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/__init__.py
--rw-r--r--   0        0        0     1142 2023-04-19 12:29:23.996637 prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.metadata.json
--rw-r--r--   0        0        0      884 2023-04-19 12:29:23.996701 prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.996767 prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/__init__.py
--rw-r--r--   0        0        0     1557 2023-04-19 12:29:23.996859 prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.metadata.json
--rw-r--r--   0        0        0      993 2023-04-19 12:29:23.996922 prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.py
--rw-r--r--   0        0        0     7622 2023-04-19 12:29:23.997006 prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.997076 prowler_cloud-3.4.0/prowler/providers/aws/services/ssmincidents/__init__.py
--rw-r--r--   0        0        0      234 2023-04-19 12:29:23.997207 prowler_cloud-3.4.0/prowler/providers/aws/services/ssmincidents/ssmincidents_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.997283 prowler_cloud-3.4.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/__init__.py
--rw-r--r--   0        0        0     1073 2023-04-19 12:29:23.997398 prowler_cloud-3.4.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.metadata.json
--rw-r--r--   0        0        0     1396 2023-04-19 12:29:23.997661 prowler_cloud-3.4.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.py
--rw-r--r--   0        0        0     6747 2023-04-19 12:29:23.997948 prowler_cloud-3.4.0/prowler/providers/aws/services/ssmincidents/ssmincidents_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.998014 prowler_cloud-3.4.0/prowler/providers/aws/services/trustedadvisor/__init__.py
--rw-r--r--   0        0        0      244 2023-04-19 12:29:23.998077 prowler_cloud-3.4.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.998144 prowler_cloud-3.4.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/__init__.py
--rw-r--r--   0        0        0     1132 2023-04-19 12:29:23.998228 prowler_cloud-3.4.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.metadata.json
--rw-r--r--   0        0        0     1272 2023-04-19 12:29:23.998296 prowler_cloud-3.4.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.py
--rw-r--r--   0        0        0     2972 2023-04-19 12:29:23.998367 prowler_cloud-3.4.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.998427 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.998500 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.998559 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_different_regions/__init__.py
--rw-r--r--   0        0        0      860 2023-04-19 12:29:23.998681 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.metadata.json
--rw-r--r--   0        0        0     1070 2023-04-19 12:29:23.998778 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.998838 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/__init__.py
--rw-r--r--   0        0        0     1094 2023-04-19 12:29:23.998922 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.metadata.json
--rw-r--r--   0        0        0     3142 2023-04-19 12:29:23.998993 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.999058 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/__init__.py
--rw-r--r--   0        0        0     1173 2023-04-19 12:29:23.999134 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.metadata.json
--rw-r--r--   0        0        0     2056 2023-04-19 12:29:23.999201 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.999264 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/__init__.py
--rw-r--r--   0        0        0     1214 2023-04-19 12:29:23.999341 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.metadata.json
--rw-r--r--   0        0        0      822 2023-04-19 12:29:23.999398 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.999459 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/__init__.py
--rw-r--r--   0        0        0     1294 2023-04-19 12:29:23.999536 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.metadata.json
--rw-r--r--   0        0        0     1496 2023-04-19 12:29:23.999598 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.py
--rw-r--r--   0        0        0    15315 2023-04-19 12:29:23.999724 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.999799 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/__init__.py
--rw-r--r--   0        0        0      913 2023-04-19 12:29:23.999916 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.metadata.json
--rw-r--r--   0        0        0     1276 2023-04-19 12:29:24.000149 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.000210 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/__init__.py
--rw-r--r--   0        0        0      900 2023-04-19 12:29:24.000322 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.metadata.json
--rw-r--r--   0        0        0     1432 2023-04-19 12:29:24.000414 prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.000473 prowler_cloud-3.4.0/prowler/providers/aws/services/waf/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:24.000539 prowler_cloud-3.4.0/prowler/providers/aws/services/waf/waf_client.py
--rw-r--r--   0        0        0     2645 2023-04-19 12:29:24.000622 prowler_cloud-3.4.0/prowler/providers/aws/services/waf/waf_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.000680 prowler_cloud-3.4.0/prowler/providers/aws/services/wafv2/__init__.py
--rw-r--r--   0        0        0      190 2023-04-19 12:29:24.000748 prowler_cloud-3.4.0/prowler/providers/aws/services/wafv2/wafv2_client.py
--rw-r--r--   0        0        0     2724 2023-04-19 12:29:24.000842 prowler_cloud-3.4.0/prowler/providers/aws/services/wafv2/wafv2_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.000903 prowler_cloud-3.4.0/prowler/providers/aws/services/workspaces/__init__.py
--rw-r--r--   0        0        0      215 2023-04-19 12:29:24.000979 prowler_cloud-3.4.0/prowler/providers/aws/services/workspaces/workspaces_client.py
--rw-r--r--   0        0        0     3457 2023-04-19 12:29:24.001045 prowler_cloud-3.4.0/prowler/providers/aws/services/workspaces/workspaces_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.001108 prowler_cloud-3.4.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     2073 2023-04-19 12:29:24.001196 prowler_cloud-3.4.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1586 2023-04-19 12:29:24.001258 prowler_cloud-3.4.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.001325 prowler_cloud-3.4.0/prowler/providers/azure/__init__.py
--rw-r--r--   0        0        0     8032 2023-04-19 12:29:24.001448 prowler_cloud-3.4.0/prowler/providers/azure/azure_provider.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.001546 prowler_cloud-3.4.0/prowler/providers/azure/lib/audit_info/__init__.py
--rw-r--r--   0        0        0      258 2023-04-19 12:29:24.001624 prowler_cloud-3.4.0/prowler/providers/azure/lib/audit_info/audit_info.py
--rw-r--r--   0        0        0      796 2023-04-19 12:29:24.001856 prowler_cloud-3.4.0/prowler/providers/azure/lib/audit_info/models.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.001965 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/__init__.py
--rw-r--r--   0        0        0      205 2023-04-19 12:29:24.002041 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.002107 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/__init__.py
--rw-r--r--   0        0        0     1496 2023-04-19 12:29:24.002201 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.metadata.json
--rw-r--r--   0        0        0     1182 2023-04-19 12:29:24.002300 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.002370 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/__init__.py
--rw-r--r--   0        0        0      926 2023-04-19 12:29:24.002447 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.metadata.json
--rw-r--r--   0        0        0     1121 2023-04-19 12:29:24.002545 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.002609 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/__init__.py
--rw-r--r--   0        0        0     1654 2023-04-19 12:29:24.002689 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.metadata.json
--rw-r--r--   0        0        0     1210 2023-04-19 12:29:24.002792 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.002856 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/__init__.py
--rw-r--r--   0        0        0     1561 2023-04-19 12:29:24.002928 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.metadata.json
--rw-r--r--   0        0        0     1181 2023-04-19 12:29:24.003026 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.003101 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/__init__.py
--rw-r--r--   0        0        0     1306 2023-04-19 12:29:24.003180 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.metadata.json
--rw-r--r--   0        0        0     1163 2023-04-19 12:29:24.003285 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.003354 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/__init__.py
--rw-r--r--   0        0        0      906 2023-04-19 12:29:24.003441 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.metadata.json
--rw-r--r--   0        0        0     1638 2023-04-19 12:29:24.003543 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.003612 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/__init__.py
--rw-r--r--   0        0        0     1254 2023-04-19 12:29:24.003699 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.metadata.json
--rw-r--r--   0        0        0     1122 2023-04-19 12:29:24.003798 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.003875 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/__init__.py
--rw-r--r--   0        0        0     1590 2023-04-19 12:29:24.003965 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.metadata.json
--rw-r--r--   0        0        0     1163 2023-04-19 12:29:24.004069 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.004143 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/__init__.py
--rw-r--r--   0        0        0     1187 2023-04-19 12:29:24.004227 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.metadata.json
--rw-r--r--   0        0        0     1346 2023-04-19 12:29:24.004336 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.004406 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/__init__.py
--rw-r--r--   0        0        0     1509 2023-04-19 12:29:24.004481 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.metadata.json
--rw-r--r--   0        0        0     1170 2023-04-19 12:29:24.004577 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.004642 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-19 12:29:24.004717 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.metadata.json
--rw-r--r--   0        0        0     1227 2023-04-19 12:29:24.004839 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.004910 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/__init__.py
--rw-r--r--   0        0        0     1693 2023-04-19 12:29:24.005006 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.metadata.json
--rw-r--r--   0        0        0     1202 2023-04-19 12:29:24.005103 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.py
--rw-r--r--   0        0        0     2326 2023-04-19 12:29:24.005198 prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.005261 prowler_cloud-3.4.0/prowler/providers/azure/services/iam/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:24.005325 prowler_cloud-3.4.0/prowler/providers/azure/services/iam/iam_client.py
--rw-r--r--   0        0        0     2696 2023-04-19 12:29:24.005421 prowler_cloud-3.4.0/prowler/providers/azure/services/iam/iam_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.005484 prowler_cloud-3.4.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/__init__.py
--rw-r--r--   0        0        0      996 2023-04-19 12:29:24.005565 prowler_cloud-3.4.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.metadata.json
--rw-r--r--   0        0        0     1330 2023-04-19 12:29:24.005639 prowler_cloud-3.4.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.005701 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.005772 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/__init__.py
--rw-r--r--   0        0        0     1470 2023-04-19 12:29:24.005850 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.metadata.json
--rw-r--r--   0        0        0     1166 2023-04-19 12:29:24.005926 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.py
--rw-r--r--   0        0        0      200 2023-04-19 12:29:24.005980 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.006041 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/__init__.py
--rw-r--r--   0        0        0     1354 2023-04-19 12:29:24.006117 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.metadata.json
--rw-r--r--   0        0        0     1179 2023-04-19 12:29:24.006185 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.006249 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/__init__.py
--rw-r--r--   0        0        0     1765 2023-04-19 12:29:24.006334 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.metadata.json
--rw-r--r--   0        0        0     1265 2023-04-19 12:29:24.006399 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.006465 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/__init__.py
--rw-r--r--   0        0        0     1399 2023-04-19 12:29:24.006543 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.metadata.json
--rw-r--r--   0        0        0     1156 2023-04-19 12:29:24.006608 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.006669 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/__init__.py
--rw-r--r--   0        0        0     1246 2023-04-19 12:29:24.006748 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.metadata.json
--rw-r--r--   0        0        0     1151 2023-04-19 12:29:24.006809 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.006877 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/__init__.py
--rw-r--r--   0        0        0     1093 2023-04-19 12:29:24.006957 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.metadata.json
--rw-r--r--   0        0        0     1169 2023-04-19 12:29:24.007018 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.007076 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/__init__.py
--rw-r--r--   0        0        0     1272 2023-04-19 12:29:24.007155 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.metadata.json
--rw-r--r--   0        0        0     1166 2023-04-19 12:29:24.007210 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.py
--rw-r--r--   0        0        0     3651 2023-04-19 12:29:24.007316 prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.007373 prowler_cloud-3.4.0/prowler/providers/common/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-19 12:29:24.007448 prowler_cloud-3.4.0/prowler/providers/common/allowlist.py
--rw-r--r--   0        0        0    17566 2023-04-19 12:29:24.007922 prowler_cloud-3.4.0/prowler/providers/common/audit_info.py
--rw-r--r--   0        0        0      251 2023-04-19 12:29:24.008002 prowler_cloud-3.4.0/prowler/providers/common/models.py
--rw-r--r--   0        0        0     4693 2023-04-19 12:29:24.008267 prowler_cloud-3.4.0/prowler/providers/common/outputs.py
--rw-r--r--   0        0        0      885 2023-04-19 12:29:24.008368 prowler_cloud-3.4.0/prowler/providers/common/quick_inventory.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.008430 prowler_cloud-3.4.0/prowler/providers/gcp/__init__.py
--rw-r--r--   0        0        0     1695 2023-04-19 12:29:24.008547 prowler_cloud-3.4.0/prowler/providers/gcp/gcp_provider.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.008639 prowler_cloud-3.4.0/prowler/providers/gcp/lib/audit_info/__init__.py
--rw-r--r--   0        0        0      201 2023-04-19 12:29:24.008706 prowler_cloud-3.4.0/prowler/providers/gcp/lib/audit_info/audit_info.py
--rw-r--r--   0        0        0      522 2023-04-19 12:29:24.008769 prowler_cloud-3.4.0/prowler/providers/gcp/lib/audit_info/models.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.008869 prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/__init__.py
--rw-r--r--   0        0        0      197 2023-04-19 12:29:24.008942 prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.009000 prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/__init__.py
--rw-r--r--   0        0        0     1445 2023-04-19 12:29:24.009076 prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.metadata.json
--rw-r--r--   0        0        0      996 2023-04-19 12:29:24.009145 prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.009202 prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/__init__.py
--rw-r--r--   0        0        0     1314 2023-04-19 12:29:24.009314 prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.metadata.json
--rw-r--r--   0        0        0      948 2023-04-19 12:29:24.009408 prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.py
--rw-r--r--   0        0        0     4116 2023-04-19 12:29:24.009507 prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.009566 prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/__init__.py
--rw-r--r--   0        0        0     1373 2023-04-19 12:29:24.009671 prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.metadata.json
--rw-r--r--   0        0        0      974 2023-04-19 12:29:24.009766 prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.009835 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudresourcemanager/__init__.py
--rw-r--r--   0        0        0      266 2023-04-19 12:29:24.009910 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_client.py
--rw-r--r--   0        0        0     1262 2023-04-19 12:29:24.009969 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.010050 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/__init__.py
--rw-r--r--   0        0        0      197 2023-04-19 12:29:24.010112 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.010172 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/__init__.py
--rw-r--r--   0        0        0     1408 2023-04-19 12:29:24.010282 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.metadata.json
--rw-r--r--   0        0        0     1011 2023-04-19 12:29:24.010380 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.010443 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/__init__.py
--rw-r--r--   0        0        0     1359 2023-04-19 12:29:24.010556 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.metadata.json
--rw-r--r--   0        0        0     1182 2023-04-19 12:29:24.010649 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.010712 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/__init__.py
--rw-r--r--   0        0        0     1216 2023-04-19 12:29:24.011215 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.metadata.json
--rw-r--r--   0        0        0     1203 2023-04-19 12:29:24.011559 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.011633 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/__init__.py
--rw-r--r--   0        0        0     2058 2023-04-19 12:29:24.011749 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.metadata.json
--rw-r--r--   0        0        0     1302 2023-04-19 12:29:24.011849 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.011912 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-19 12:29:24.012026 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.metadata.json
--rw-r--r--   0        0        0     1207 2023-04-19 12:29:24.012120 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.012183 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/__init__.py
--rw-r--r--   0        0        0     1447 2023-04-19 12:29:24.012289 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.metadata.json
--rw-r--r--   0        0        0     1219 2023-04-19 12:29:24.012566 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.012642 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/__init__.py
--rw-r--r--   0        0        0     1618 2023-04-19 12:29:24.012759 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.metadata.json
--rw-r--r--   0        0        0     1310 2023-04-19 12:29:24.012938 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.013002 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/__init__.py
--rw-r--r--   0        0        0     1442 2023-04-19 12:29:24.013111 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.metadata.json
--rw-r--r--   0        0        0     1323 2023-04-19 12:29:24.013203 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.013261 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/__init__.py
--rw-r--r--   0        0        0     1955 2023-04-19 12:29:24.013390 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.metadata.json
--rw-r--r--   0        0        0     1466 2023-04-19 12:29:24.013630 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.013695 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/__init__.py
--rw-r--r--   0        0        0     1745 2023-04-19 12:29:24.013803 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.metadata.json
--rw-r--r--   0        0        0     1410 2023-04-19 12:29:24.013897 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.013964 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/__init__.py
--rw-r--r--   0        0        0     1326 2023-04-19 12:29:24.014087 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.metadata.json
--rw-r--r--   0        0        0     1368 2023-04-19 12:29:24.014258 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.014331 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/__init__.py
--rw-r--r--   0        0        0     1151 2023-04-19 12:29:24.014469 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.metadata.json
--rw-r--r--   0        0        0     1104 2023-04-19 12:29:24.014571 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.014636 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/__init__.py
--rw-r--r--   0        0        0     1492 2023-04-19 12:29:24.014749 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.metadata.json
--rw-r--r--   0        0        0     1046 2023-04-19 12:29:24.014844 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.014903 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/__init__.py
--rw-r--r--   0        0        0     1319 2023-04-19 12:29:24.014985 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.metadata.json
--rw-r--r--   0        0        0      991 2023-04-19 12:29:24.015046 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.015134 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/__init__.py
--rw-r--r--   0        0        0     2153 2023-04-19 12:29:24.015262 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.metadata.json
--rw-r--r--   0        0        0     1350 2023-04-19 12:29:24.015367 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.015435 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/__init__.py
--rw-r--r--   0        0        0     1702 2023-04-19 12:29:24.015548 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.metadata.json
--rw-r--r--   0        0        0     1232 2023-04-19 12:29:24.015643 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.015707 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/__init__.py
--rw-r--r--   0        0        0     1583 2023-04-19 12:29:24.015828 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.metadata.json
--rw-r--r--   0        0        0     1319 2023-04-19 12:29:24.016131 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.016272 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/__init__.py
--rw-r--r--   0        0        0     1860 2023-04-19 12:29:24.016436 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.metadata.json
--rw-r--r--   0        0        0     1201 2023-04-19 12:29:24.016571 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.016651 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/__init__.py
--rw-r--r--   0        0        0     2002 2023-04-19 12:29:24.016785 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.metadata.json
--rw-r--r--   0        0        0     1190 2023-04-19 12:29:24.016898 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.016981 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/__init__.py
--rw-r--r--   0        0        0     2238 2023-04-19 12:29:24.017114 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.metadata.json
--rw-r--r--   0        0        0     1210 2023-04-19 12:29:24.017227 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.017311 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/__init__.py
--rw-r--r--   0        0        0     1583 2023-04-19 12:29:24.017749 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.metadata.json
--rw-r--r--   0        0        0     1179 2023-04-19 12:29:24.017983 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.018063 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/__init__.py
--rw-r--r--   0        0        0     1428 2023-04-19 12:29:24.018178 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.metadata.json
--rw-r--r--   0        0        0      977 2023-04-19 12:29:24.018274 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.py
--rw-r--r--   0        0        0     2467 2023-04-19 12:29:24.018383 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.018443 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudstorage/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.018527 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/__init__.py
--rw-r--r--   0        0        0     1351 2023-04-19 12:29:24.018636 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.metadata.json
--rw-r--r--   0        0        0      926 2023-04-19 12:29:24.018724 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.018787 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/__init__.py
--rw-r--r--   0        0        0     1270 2023-04-19 12:29:24.018893 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.metadata.json
--rw-r--r--   0        0        0     1067 2023-04-19 12:29:24.018961 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.py
--rw-r--r--   0        0        0      226 2023-04-19 12:29:24.019016 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_client.py
--rw-r--r--   0        0        0     2099 2023-04-19 12:29:24.019113 prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.019173 prowler_cloud-3.4.0/prowler/providers/gcp/services/compute/__init__.py
--rw-r--r--   0        0        0      192 2023-04-19 12:29:24.019237 prowler_cloud-3.4.0/prowler/providers/gcp/services/compute/compute_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.019294 prowler_cloud-3.4.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/__init__.py
--rw-r--r--   0        0        0     1327 2023-04-19 12:29:24.019382 prowler_cloud-3.4.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.metadata.json
--rw-r--r--   0        0        0      897 2023-04-19 12:29:24.019443 prowler_cloud-3.4.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.019505 prowler_cloud-3.4.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/__init__.py
--rw-r--r--   0        0        0     1132 2023-04-19 12:29:24.019597 prowler_cloud-3.4.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.metadata.json
--rw-r--r--   0        0        0      827 2023-04-19 12:29:24.019661 prowler_cloud-3.4.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.py
--rw-r--r--   0        0        0     3489 2023-04-19 12:29:24.019722 prowler_cloud-3.4.0/prowler/providers/gcp/services/compute/compute_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.019781 prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/__init__.py
--rw-r--r--   0        0        0      172 2023-04-19 12:29:24.019858 prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.019919 prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/__init__.py
--rw-r--r--   0        0        0     1459 2023-04-19 12:29:24.019998 prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.metadata.json
--rw-r--r--   0        0        0     1395 2023-04-19 12:29:24.020445 prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.020509 prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/__init__.py
--rw-r--r--   0        0        0     1363 2023-04-19 12:29:24.020619 prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.metadata.json
--rw-r--r--   0        0        0     1038 2023-04-19 12:29:24.020846 prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.020931 prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/__init__.py
--rw-r--r--   0        0        0     1133 2023-04-19 12:29:24.021052 prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.metadata.json
--rw-r--r--   0        0        0     1317 2023-04-19 12:29:24.021164 prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.py
--rw-r--r--   0        0        0     3292 2023-04-19 12:29:24.021266 prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.021333 prowler_cloud-3.4.0/prowler/providers/gcp/services/kms/__init__.py
--rw-r--r--   0        0        0      172 2023-04-19 12:29:24.021401 prowler_cloud-3.4.0/prowler/providers/gcp/services/kms/kms_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.021465 prowler_cloud-3.4.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1195 2023-04-19 12:29:24.021537 prowler_cloud-3.4.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1000 2023-04-19 12:29:24.021594 prowler_cloud-3.4.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.021662 prowler_cloud-3.4.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/__init__.py
--rw-r--r--   0        0        0     1233 2023-04-19 12:29:24.021737 prowler_cloud-3.4.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.metadata.json
--rw-r--r--   0        0        0     1135 2023-04-19 12:29:24.021794 prowler_cloud-3.4.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.py
--rw-r--r--   0        0        0     4837 2023-04-19 12:29:24.021859 prowler_cloud-3.4.0/prowler/providers/gcp/services/kms/kms_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.021915 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/__init__.py
--rw-r--r--   0        0        0      192 2023-04-19 12:29:24.021981 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.022046 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1438 2023-04-19 12:29:24.022174 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.metadata.json
--rw-r--r--   0        0        0     1996 2023-04-19 12:29:24.022441 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.022510 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1243 2023-04-19 12:29:24.022758 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.metadata.json
--rw-r--r--   0        0        0     1971 2023-04-19 12:29:24.022856 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.022918 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1239 2023-04-19 12:29:24.023029 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2090 2023-04-19 12:29:24.023132 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.023196 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1590 2023-04-19 12:29:24.023306 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2288 2023-04-19 12:29:24.023447 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.023535 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-19 12:29:24.023657 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.metadata.json
--rw-r--r--   0        0        0     1955 2023-04-19 12:29:24.023765 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.023843 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1233 2023-04-19 12:29:24.023959 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2086 2023-04-19 12:29:24.024065 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.024131 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1113 2023-04-19 12:29:24.024268 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2188 2023-04-19 12:29:24.024385 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.024464 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1157 2023-04-19 12:29:24.024600 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2019 2023-04-19 12:29:24.024712 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.py
--rw-r--r--   0        0        0     2577 2023-04-19 12:29:24.024824 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.024897 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_sink_created/__init__.py
--rw-r--r--   0        0        0     1235 2023-04-19 12:29:24.024987 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.metadata.json
--rw-r--r--   0        0        0     1473 2023-04-19 12:29:24.025096 prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.025173 prowler_cloud-3.4.0/prowler/providers/gcp/services/monitoring/__init__.py
--rw-r--r--   0        0        0      207 2023-04-19 12:29:24.025294 prowler_cloud-3.4.0/prowler/providers/gcp/services/monitoring/monitoring_client.py
--rw-r--r--   0        0        0     1893 2023-04-19 12:29:24.025405 prowler_cloud-3.4.0/prowler/providers/gcp/services/monitoring/monitoring_service.py
--rw-r--r--   0        0        0     2449 2023-04-20 13:34:48.467350 prowler_cloud-3.4.0/pyproject.toml
--rw-r--r--   0        0        0    47089 1970-01-01 00:00:00.000000 prowler_cloud-3.4.0/setup.py
--rw-r--r--   0        0        0    15171 1970-01-01 00:00:00.000000 prowler_cloud-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-19 12:29:23.881015 prowler_cloud-3.4.1/LICENSE
+-rw-r--r--   0        0        0    13104 2023-04-19 12:29:23.881214 prowler_cloud-3.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.914816 prowler_cloud-3.4.1/prowler/__init__.py
+-rw-r--r--   0        0        0     8364 2023-04-24 08:22:21.142090 prowler_cloud-3.4.1/prowler/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.915066 prowler_cloud-3.4.1/prowler/compliance/aws/__init__.py
+-rw-r--r--   0        0        0     6516 2023-04-19 12:29:23.915167 prowler_cloud-3.4.1/prowler/compliance/aws/aws_audit_manager_control_tower_guardrails_aws.json
+-rw-r--r--   0        0        0    17475 2023-04-19 14:30:31.781622 prowler_cloud-3.4.1/prowler/compliance/aws/aws_foundational_security_best_practices_aws.json
+-rw-r--r--   0        0        0   260398 2023-04-19 14:30:31.782770 prowler_cloud-3.4.1/prowler/compliance/aws/cis_1.4_aws.json
+-rw-r--r--   0        0        0   287275 2023-04-19 14:30:31.783625 prowler_cloud-3.4.1/prowler/compliance/aws/cis_1.5_aws.json
+-rw-r--r--   0        0        0    15458 2023-04-19 14:30:31.783934 prowler_cloud-3.4.1/prowler/compliance/aws/cisa_aws.json
+-rw-r--r--   0        0        0   124269 2023-04-19 14:30:31.784533 prowler_cloud-3.4.1/prowler/compliance/aws/ens_rd2022_aws.json
+-rw-r--r--   0        0        0    18551 2023-04-19 14:30:31.784938 prowler_cloud-3.4.1/prowler/compliance/aws/fedramp_low_revision_4_aws.json
+-rw-r--r--   0        0        0    57257 2023-04-19 14:30:31.785245 prowler_cloud-3.4.1/prowler/compliance/aws/fedramp_moderate_revision_4_aws.json
+-rw-r--r--   0        0        0    31059 2023-04-19 14:30:31.785581 prowler_cloud-3.4.1/prowler/compliance/aws/ffiec_aws.json
+-rw-r--r--   0        0        0    10166 2023-04-19 14:30:31.785863 prowler_cloud-3.4.1/prowler/compliance/aws/gdpr_aws.json
+-rw-r--r--   0        0        0    18763 2023-04-19 14:30:31.786156 prowler_cloud-3.4.1/prowler/compliance/aws/gxp_21_cfr_part_11_aws.json
+-rw-r--r--   0        0        0    11774 2023-04-19 12:29:23.917593 prowler_cloud-3.4.1/prowler/compliance/aws/gxp_eu_annex_11_aws.json
+-rw-r--r--   0        0        0    31000 2023-04-19 14:30:31.786493 prowler_cloud-3.4.1/prowler/compliance/aws/hipaa_aws.json
+-rw-r--r--   0        0        0    86208 2023-04-19 14:30:31.787189 prowler_cloud-3.4.1/prowler/compliance/aws/nist_800_171_revision_2_aws.json
+-rw-r--r--   0        0        0    50559 2023-04-19 14:30:31.787572 prowler_cloud-3.4.1/prowler/compliance/aws/nist_800_53_revision_4_aws.json
+-rw-r--r--   0        0        0   243911 2023-04-19 14:30:31.788157 prowler_cloud-3.4.1/prowler/compliance/aws/nist_800_53_revision_5_aws.json
+-rw-r--r--   0        0        0    40042 2023-04-19 14:30:31.788517 prowler_cloud-3.4.1/prowler/compliance/aws/nist_csf_1.1_aws.json
+-rw-r--r--   0        0        0     8722 2023-04-19 14:30:31.788905 prowler_cloud-3.4.1/prowler/compliance/aws/pci_3.2.1_aws.json
+-rw-r--r--   0        0        0     8563 2023-04-19 14:30:31.789072 prowler_cloud-3.4.1/prowler/compliance/aws/rbi_cyber_security_framework_aws.json
+-rw-r--r--   0        0        0    93913 2023-04-19 14:30:31.789715 prowler_cloud-3.4.1/prowler/compliance/aws/soc2_aws.json
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.918830 prowler_cloud-3.4.1/prowler/compliance/azure/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.918896 prowler_cloud-3.4.1/prowler/compliance/gcp/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.919011 prowler_cloud-3.4.1/prowler/config/__init__.py
+-rw-r--r--   0        0        0     2352 2023-04-19 12:29:23.919100 prowler_cloud-3.4.1/prowler/config/allowlist.yaml
+-rw-r--r--   0        0        0      165 2023-04-19 12:29:23.919158 prowler_cloud-3.4.1/prowler/config/checklist_example.json
+-rw-r--r--   0        0        0     2725 2023-04-25 11:50:25.453058 prowler_cloud-3.4.1/prowler/config/config.py
+-rw-r--r--   0        0        0     1942 2023-04-19 12:29:23.919734 prowler_cloud-3.4.1/prowler/config/config.yaml
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.919791 prowler_cloud-3.4.1/prowler/lib/__init__.py
+-rw-r--r--   0        0        0      854 2023-04-19 12:29:23.919861 prowler_cloud-3.4.1/prowler/lib/banner.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.919915 prowler_cloud-3.4.1/prowler/lib/check/__init__.py
+-rw-r--r--   0        0        0    23001 2023-04-19 16:59:58.235931 prowler_cloud-3.4.1/prowler/lib/check/check.py
+-rw-r--r--   0        0        0     2973 2023-04-19 12:29:23.920475 prowler_cloud-3.4.1/prowler/lib/check/checks_loader.py
+-rw-r--r--   0        0        0     4413 2023-04-19 12:29:23.920553 prowler_cloud-3.4.1/prowler/lib/check/compliance.py
+-rw-r--r--   0        0        0     3645 2023-04-19 12:29:23.920631 prowler_cloud-3.4.1/prowler/lib/check/compliance_models.py
+-rw-r--r--   0        0        0     3835 2023-04-19 12:29:23.920708 prowler_cloud-3.4.1/prowler/lib/check/models.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.920774 prowler_cloud-3.4.1/prowler/lib/cli/__init__.py
+-rw-r--r--   0        0        0    17295 2023-04-25 10:05:59.352943 prowler_cloud-3.4.1/prowler/lib/cli/parser.py
+-rw-r--r--   0        0        0     1885 2023-04-19 12:29:23.921010 prowler_cloud-3.4.1/prowler/lib/logger.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.921073 prowler_cloud-3.4.1/prowler/lib/outputs/__init__.py
+-rw-r--r--   0        0        0    19729 2023-04-19 12:29:23.921187 prowler_cloud-3.4.1/prowler/lib/outputs/compliance.py
+-rw-r--r--   0        0        0     6687 2023-04-19 12:29:23.922980 prowler_cloud-3.4.1/prowler/lib/outputs/file_descriptors.py
+-rw-r--r--   0        0        0    20055 2023-04-19 12:29:23.923272 prowler_cloud-3.4.1/prowler/lib/outputs/html.py
+-rw-r--r--   0        0        0     3721 2023-04-19 12:29:23.923348 prowler_cloud-3.4.1/prowler/lib/outputs/json.py
+-rw-r--r--   0        0        0    20235 2023-04-19 12:29:23.923478 prowler_cloud-3.4.1/prowler/lib/outputs/models.py
+-rw-r--r--   0        0        0    10451 2023-04-19 12:29:23.923678 prowler_cloud-3.4.1/prowler/lib/outputs/outputs.py
+-rw-r--r--   0        0        0     6058 2023-04-19 12:29:23.923779 prowler_cloud-3.4.1/prowler/lib/outputs/summary_table.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.923838 prowler_cloud-3.4.1/prowler/lib/scan_filters/__init__.py
+-rw-r--r--   0        0        0      552 2023-04-19 12:29:23.923910 prowler_cloud-3.4.1/prowler/lib/scan_filters/scan_filters.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.923974 prowler_cloud-3.4.1/prowler/lib/utils/__init__.py
+-rw-r--r--   0        0        0     2200 2023-04-19 12:29:23.924056 prowler_cloud-3.4.1/prowler/lib/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.924142 prowler_cloud-3.4.1/prowler/providers/aws/__init__.py
+-rw-r--r--   0        0        0    10318 2023-04-19 12:29:23.924275 prowler_cloud-3.4.1/prowler/providers/aws/aws_provider.py
+-rw-r--r--   0        0        0   211895 2023-04-24 11:04:11.502593 prowler_cloud-3.4.1/prowler/providers/aws/aws_regions_by_service.json
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.924651 prowler_cloud-3.4.1/prowler/providers/aws/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.924735 prowler_cloud-3.4.1/prowler/providers/aws/lib/allowlist/__init__.py
+-rw-r--r--   0        0        0     7931 2023-04-19 12:29:23.924815 prowler_cloud-3.4.1/prowler/providers/aws/lib/allowlist/allowlist.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.924868 prowler_cloud-3.4.1/prowler/providers/aws/lib/arn/__init__.py
+-rw-r--r--   0        0        0     1902 2023-04-19 12:29:23.924941 prowler_cloud-3.4.1/prowler/providers/aws/lib/arn/arn.py
+-rw-r--r--   0        0        0     1932 2023-04-19 12:29:23.925001 prowler_cloud-3.4.1/prowler/providers/aws/lib/arn/error.py
+-rw-r--r--   0        0        0      953 2023-04-19 12:29:23.925101 prowler_cloud-3.4.1/prowler/providers/aws/lib/audit_info/audit_info.py
+-rw-r--r--   0        0        0     1178 2023-04-19 12:29:23.925172 prowler_cloud-3.4.1/prowler/providers/aws/lib/audit_info/models.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925231 prowler_cloud-3.4.1/prowler/providers/aws/lib/quick_inventory/__init__.py
+-rw-r--r--   0        0        0    13659 2023-04-19 12:29:23.925364 prowler_cloud-3.4.1/prowler/providers/aws/lib/quick_inventory/quick_inventory.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925429 prowler_cloud-3.4.1/prowler/providers/aws/lib/resource_api_tagging/__init__.py
+-rw-r--r--   0        0        0     1585 2023-04-19 12:29:23.925524 prowler_cloud-3.4.1/prowler/providers/aws/lib/resource_api_tagging/resource_api_tagging.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925602 prowler_cloud-3.4.1/prowler/providers/aws/lib/security_hub/__init__.py
+-rw-r--r--   0        0        0     5867 2023-04-19 12:29:23.925704 prowler_cloud-3.4.1/prowler/providers/aws/lib/security_hub/security_hub.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925777 prowler_cloud-3.4.1/prowler/providers/aws/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925856 prowler_cloud-3.4.1/prowler/providers/aws/services/accessanalyzer/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-19 12:29:23.925925 prowler_cloud-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925983 prowler_cloud-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/__init__.py
+-rw-r--r--   0        0        0     1584 2023-04-19 12:29:23.926072 prowler_cloud-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.metadata.json
+-rw-r--r--   0        0        0     1478 2023-04-19 12:29:23.926147 prowler_cloud-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.926226 prowler_cloud-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/__init__.py
+-rw-r--r--   0        0        0     1635 2023-04-19 12:29:23.926328 prowler_cloud-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.metadata.json
+-rw-r--r--   0        0        0     2184 2023-04-19 12:29:23.926396 prowler_cloud-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.py
+-rw-r--r--   0        0        0     4735 2023-04-19 12:29:23.926489 prowler_cloud-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.926555 prowler_cloud-3.4.1/prowler/providers/aws/services/account/__init__.py
+-rw-r--r--   0        0        0      200 2023-04-19 12:29:23.926641 prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.926710 prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/__init__.py
+-rw-r--r--   0        0        0     1753 2023-04-19 12:29:23.926813 prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.metadata.json
+-rw-r--r--   0        0        0      652 2023-04-19 12:29:23.926914 prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.926987 prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/__init__.py
+-rw-r--r--   0        0        0     1315 2023-04-19 12:29:23.927076 prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.metadata.json
+-rw-r--r--   0        0        0      681 2023-04-19 12:29:23.927162 prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.927235 prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/__init__.py
+-rw-r--r--   0        0        0     1674 2023-04-19 12:29:23.927318 prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.metadata.json
+-rw-r--r--   0        0        0      699 2023-04-19 12:29:23.927389 prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.py
+-rw-r--r--   0        0        0      769 2023-04-19 12:29:23.927493 prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.927558 prowler_cloud-3.4.1/prowler/providers/aws/services/acm/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.927642 prowler_cloud-3.4.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/__init__.py
+-rw-r--r--   0        0        0     1368 2023-04-19 12:29:23.927732 prowler_cloud-3.4.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.metadata.json
+-rw-r--r--   0        0        0     1233 2023-04-19 12:29:23.927811 prowler_cloud-3.4.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.927881 prowler_cloud-3.4.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/__init__.py
+-rw-r--r--   0        0        0     1316 2023-04-19 12:29:23.927960 prowler_cloud-3.4.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.metadata.json
+-rw-r--r--   0        0        0     1636 2023-04-19 12:29:23.928023 prowler_cloud-3.4.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:23.928090 prowler_cloud-3.4.1/prowler/providers/aws/services/acm/acm_client.py
+-rw-r--r--   0        0        0     4752 2023-04-19 12:29:23.928187 prowler_cloud-3.4.1/prowler/providers/aws/services/acm/acm_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.928261 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.928350 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/__init__.py
+-rw-r--r--   0        0        0     1133 2023-04-19 12:29:23.928450 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.metadata.json
+-rw-r--r--   0        0        0      976 2023-04-19 12:29:23.928524 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.py
+-rw-r--r--   0        0        0      215 2023-04-19 12:29:23.928590 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.928660 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/__init__.py
+-rw-r--r--   0        0        0     1250 2023-04-19 12:29:23.928751 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.metadata.json
+-rw-r--r--   0        0        0     1126 2023-04-19 12:29:23.928823 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.928899 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/__init__.py
+-rw-r--r--   0        0        0     1087 2023-04-19 12:29:23.928989 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.metadata.json
+-rw-r--r--   0        0        0      994 2023-04-19 12:29:23.929063 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.929128 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1676 2023-04-19 12:29:23.929219 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1079 2023-04-19 12:29:23.929284 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.py
+-rw-r--r--   0        0        0     5312 2023-04-19 12:29:23.929343 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.929405 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/__init__.py
+-rw-r--r--   0        0        0     1181 2023-04-19 12:29:23.929484 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.metadata.json
+-rw-r--r--   0        0        0     1093 2023-04-19 12:29:23.929553 prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.929624 prowler_cloud-3.4.1/prowler/providers/aws/services/apigatewayv2/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.929711 prowler_cloud-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1095 2023-04-19 12:29:23.929800 prowler_cloud-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1123 2023-04-19 12:29:23.929864 prowler_cloud-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.929939 prowler_cloud-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/__init__.py
+-rw-r--r--   0        0        0     1038 2023-04-19 12:29:23.930024 prowler_cloud-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.metadata.json
+-rw-r--r--   0        0        0     1037 2023-04-19 12:29:23.930091 prowler_cloud-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.py
+-rw-r--r--   0        0        0      234 2023-04-19 12:29:23.930163 prowler_cloud-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_client.py
+-rw-r--r--   0        0        0     3806 2023-04-19 12:29:23.930279 prowler_cloud-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.930354 prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/__init__.py
+-rw-r--r--   0        0        0      210 2023-04-19 12:29:23.930444 prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.930518 prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/__init__.py
+-rw-r--r--   0        0        0     1346 2023-04-19 12:29:23.930597 prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.metadata.json
+-rw-r--r--   0        0        0     1273 2023-04-19 12:29:23.930659 prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.930725 prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/__init__.py
+-rw-r--r--   0        0        0     1257 2023-04-19 12:29:23.930807 prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.metadata.json
+-rw-r--r--   0        0        0     1408 2023-04-19 12:29:23.930874 prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.930944 prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/__init__.py
+-rw-r--r--   0        0        0     1269 2023-04-19 12:29:23.931029 prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.metadata.json
+-rw-r--r--   0        0        0     1420 2023-04-19 12:29:23.931102 prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.931165 prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/__init__.py
+-rw-r--r--   0        0        0     1363 2023-04-19 12:29:23.931240 prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.metadata.json
+-rw-r--r--   0        0        0     1583 2023-04-19 12:29:23.931295 prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.py
+-rw-r--r--   0        0        0     3619 2023-04-19 12:29:23.931383 prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.931448 prowler_cloud-3.4.1/prowler/providers/aws/services/autoscaling/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-19 12:29:23.931525 prowler_cloud-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.931592 prowler_cloud-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/__init__.py
+-rw-r--r--   0        0        0     1172 2023-04-19 12:29:23.931671 prowler_cloud-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.metadata.json
+-rw-r--r--   0        0        0     1902 2023-04-19 12:29:23.931745 prowler_cloud-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.py
+-rw-r--r--   0        0        0       78 2023-04-19 12:29:23.931828 prowler_cloud-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/fixtures/fixture
+-rw-r--r--   0        0        0     2626 2023-04-19 12:29:23.931901 prowler_cloud-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.931954 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/__init__.py
+-rw-r--r--   0        0        0      204 2023-04-19 12:29:23.932016 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.932077 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1198 2023-04-19 12:29:23.932164 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     2548 2023-04-19 12:29:23.932234 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.932304 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/__init__.py
+-rw-r--r--   0        0        0     1341 2023-04-19 12:29:23.932378 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.metadata.json
+-rw-r--r--   0        0        0     3352 2023-04-19 12:29:23.932441 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.932505 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/__init__.py
+-rw-r--r--   0        0        0     1536 2023-04-19 12:29:23.932592 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.metadata.json
+-rw-r--r--   0        0        0     2209 2023-04-19 12:29:23.932663 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.932740 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1399 2023-04-19 12:29:23.932821 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1823 2023-04-19 12:29:23.932902 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.932963 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/__init__.py
+-rw-r--r--   0        0        0     1272 2023-04-19 12:29:23.933034 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.metadata.json
+-rw-r--r--   0        0        0     1058 2023-04-19 12:29:23.933094 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.933149 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/__init__.py
+-rw-r--r--   0        0        0     1120 2023-04-19 12:29:23.933215 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.metadata.json
+-rw-r--r--   0        0        0     1144 2023-04-19 12:29:23.933278 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.933349 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/__init__.py
+-rw-r--r--   0        0        0     1619 2023-04-19 12:29:23.933433 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.metadata.json
+-rw-r--r--   0        0        0     1169 2023-04-19 12:29:23.933505 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.py
+-rw-r--r--   0        0        0     7807 2023-04-19 12:29:23.933581 prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.933644 prowler_cloud-3.4.1/prowler/providers/aws/services/backup/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-19 12:29:23.933747 prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.933815 prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_plans_exist/__init__.py
+-rw-r--r--   0        0        0     1197 2023-04-19 12:29:23.933931 prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.metadata.json
+-rw-r--r--   0        0        0      920 2023-04-19 12:29:23.934028 prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.934091 prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_reportplans_exist/__init__.py
+-rw-r--r--   0        0        0     1167 2023-04-19 12:29:23.934209 prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.metadata.json
+-rw-r--r--   0        0        0      975 2023-04-19 12:29:23.934311 prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.py
+-rw-r--r--   0        0        0     6992 2023-04-19 12:29:23.934426 prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.934489 prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/__init__.py
+-rw-r--r--   0        0        0     1162 2023-04-19 12:29:23.934607 prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.metadata.json
+-rw-r--r--   0        0        0     1096 2023-04-19 12:29:23.934711 prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.934779 prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_vaults_exist/__init__.py
+-rw-r--r--   0        0        0     1134 2023-04-19 12:29:23.935070 prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.metadata.json
+-rw-r--r--   0        0        0      928 2023-04-19 12:29:23.935188 prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.935269 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudformation/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-19 12:29:23.935355 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_client.py
+-rw-r--r--   0        0        0     4466 2023-04-19 12:29:23.935455 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.935540 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/__init__.py
+-rw-r--r--   0        0        0     1367 2023-04-19 12:29:23.935635 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.metadata.json
+-rw-r--r--   0        0        0     1992 2023-04-19 12:29:23.935711 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.935787 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/__init__.py
+-rw-r--r--   0        0        0     1286 2023-04-19 12:29:23.935877 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.metadata.json
+-rw-r--r--   0        0        0     1249 2023-04-19 12:29:23.935948 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.936018 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/__init__.py
+-rw-r--r--   0        0        0      215 2023-04-19 12:29:23.936101 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.936165 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1432 2023-04-19 12:29:23.936241 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1166 2023-04-19 12:29:23.936308 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.936374 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/__init__.py
+-rw-r--r--   0        0        0     1321 2023-04-19 12:29:23.936463 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.metadata.json
+-rw-r--r--   0        0        0     1164 2023-04-19 12:29:23.936530 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.936609 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/__init__.py
+-rw-r--r--   0        0        0     1395 2023-04-19 12:29:23.936692 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.metadata.json
+-rw-r--r--   0        0        0     1912 2023-04-19 12:29:23.936753 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.936817 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1501 2023-04-19 12:29:23.936890 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1230 2023-04-19 12:29:23.936947 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.937022 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/__init__.py
+-rw-r--r--   0        0        0     1385 2023-04-19 12:29:23.937123 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.metadata.json
+-rw-r--r--   0        0        0     1781 2023-04-19 12:29:23.937196 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.937272 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/__init__.py
+-rw-r--r--   0        0        0     1479 2023-04-19 12:29:23.937369 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.metadata.json
+-rw-r--r--   0        0        0     1031 2023-04-19 12:29:23.937430 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.py
+-rw-r--r--   0        0        0     6244 2023-04-19 12:29:23.937508 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.937579 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.937669 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/__init__.py
+-rw-r--r--   0        0        0     1268 2023-04-19 12:29:23.937759 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.metadata.json
+-rw-r--r--   0        0        0     1707 2023-04-19 12:29:23.937826 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.py
+-rw-r--r--   0        0        0      215 2023-04-19 12:29:23.937892 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.937965 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1575 2023-04-19 12:29:23.938067 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     2245 2023-04-19 12:29:23.938153 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.938212 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/__init__.py
+-rw-r--r--   0        0        0     1287 2023-04-19 12:29:23.938333 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.metadata.json
+-rw-r--r--   0        0        0     1073 2023-04-19 12:29:23.938697 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.938764 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1951 2023-04-19 12:29:23.938841 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1524 2023-04-19 12:29:23.938890 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.938948 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/__init__.py
+-rw-r--r--   0        0        0     1315 2023-04-19 12:29:23.939027 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.metadata.json
+-rw-r--r--   0        0        0     1457 2023-04-19 12:29:23.939086 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.939144 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1380 2023-04-19 12:29:23.939214 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     2232 2023-04-19 12:29:23.939277 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.939341 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1393 2023-04-19 12:29:23.939412 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     2755 2023-04-19 12:29:23.939471 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.939529 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/__init__.py
+-rw-r--r--   0        0        0     1730 2023-04-19 12:29:23.939601 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.metadata.json
+-rw-r--r--   0        0        0     1956 2023-04-19 12:29:23.939664 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.939720 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/__init__.py
+-rw-r--r--   0        0        0     1537 2023-04-19 12:29:23.939796 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.metadata.json
+-rw-r--r--   0        0        0     2892 2023-04-19 12:29:23.939867 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.939922 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/__init__.py
+-rw-r--r--   0        0        0     1565 2023-04-19 12:29:23.939984 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.metadata.json
+-rw-r--r--   0        0        0     2894 2023-04-19 12:29:23.940038 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.py
+-rw-r--r--   0        0        0     9085 2023-04-19 12:29:23.940142 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.940199 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.940267 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/__init__.py
+-rw-r--r--   0        0        0     1496 2023-04-19 12:29:23.940345 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.metadata.json
+-rw-r--r--   0        0        0     2391 2023-04-19 12:29:23.940408 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.940466 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/__init__.py
+-rw-r--r--   0        0        0     1462 2023-04-19 12:29:23.940535 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.metadata.json
+-rw-r--r--   0        0        0     2397 2023-04-19 12:29:23.940589 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.940649 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/__init__.py
+-rw-r--r--   0        0        0     1450 2023-04-19 12:29:23.940721 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.metadata.json
+-rw-r--r--   0        0        0     2415 2023-04-19 12:29:23.940779 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.940837 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/__init__.py
+-rw-r--r--   0        0        0     1418 2023-04-19 12:29:23.940906 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.metadata.json
+-rw-r--r--   0        0        0     2600 2023-04-19 12:29:23.940955 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.py
+-rw-r--r--   0        0        0      215 2023-04-19 12:29:23.941012 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.941070 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/__init__.py
+-rw-r--r--   0        0        0     1179 2023-04-19 12:29:23.941158 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.metadata.json
+-rw-r--r--   0        0        0      841 2023-04-19 12:29:23.941216 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.941280 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1249 2023-04-19 12:29:23.941353 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1002 2023-04-19 12:29:23.941409 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.941464 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/__init__.py
+-rw-r--r--   0        0        0     1345 2023-04-19 12:29:23.941540 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.metadata.json
+-rw-r--r--   0        0        0     4856 2023-04-19 12:29:23.941604 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.941667 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/__init__.py
+-rw-r--r--   0        0        0     1365 2023-04-19 12:29:23.941749 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.metadata.json
+-rw-r--r--   0        0        0     1569 2023-04-25 10:05:59.404720 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.941872 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1498 2023-04-19 12:29:23.941939 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2391 2023-04-19 12:29:23.942001 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.942073 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1498 2023-04-19 12:29:23.942161 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2337 2023-04-19 12:29:23.942224 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.942293 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/__init__.py
+-rw-r--r--   0        0        0     1495 2023-04-19 12:29:23.942381 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.metadata.json
+-rw-r--r--   0        0        0     2208 2023-04-19 12:29:23.942459 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.942526 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/__init__.py
+-rw-r--r--   0        0        0     1453 2023-04-19 12:29:23.942602 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.metadata.json
+-rw-r--r--   0        0        0     3046 2023-04-19 12:29:23.942673 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.942746 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/__init__.py
+-rw-r--r--   0        0        0     1560 2023-04-19 12:29:23.942838 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.metadata.json
+-rw-r--r--   0        0        0     2261 2023-04-19 12:29:23.942907 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.942969 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/__init__.py
+-rw-r--r--   0        0        0     1456 2023-04-19 12:29:23.943038 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.metadata.json
+-rw-r--r--   0        0        0     2543 2023-04-19 12:29:23.943097 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.943156 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/__init__.py
+-rw-r--r--   0        0        0     1430 2023-04-19 12:29:23.943233 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.metadata.json
+-rw-r--r--   0        0        0     2748 2023-04-19 12:29:23.943292 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.943362 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/__init__.py
+-rw-r--r--   0        0        0     1432 2023-04-19 12:29:23.943440 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.metadata.json
+-rw-r--r--   0        0        0     2228 2023-04-19 12:29:23.943501 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.943561 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/__init__.py
+-rw-r--r--   0        0        0     1448 2023-04-19 12:29:23.943632 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.metadata.json
+-rw-r--r--   0        0        0     2413 2023-04-19 12:29:23.943687 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.943748 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/__init__.py
+-rw-r--r--   0        0        0     1475 2023-04-19 12:29:23.943818 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.metadata.json
+-rw-r--r--   0        0        0     2203 2023-04-19 12:29:23.943882 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.943942 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/__init__.py
+-rw-r--r--   0        0        0     1446 2023-04-19 12:29:23.944012 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.metadata.json
+-rw-r--r--   0        0        0     2208 2023-04-19 12:29:23.944079 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.py
+-rw-r--r--   0        0        0    10786 2023-04-25 10:05:59.404878 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_service.py
+-rw-r--r--   0        0        0      197 2023-04-19 12:29:23.944212 prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/logs_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.944273 prowler_cloud-3.4.1/prowler/providers/aws/services/codeartifact/__init__.py
+-rw-r--r--   0        0        0      234 2023-04-19 12:29:23.944347 prowler_cloud-3.4.1/prowler/providers/aws/services/codeartifact/codeartifact_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.944416 prowler_cloud-3.4.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/__init__.py
+-rw-r--r--   0        0        0     1540 2023-04-19 12:29:23.944500 prowler_cloud-3.4.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.metadata.json
+-rw-r--r--   0        0        0     1665 2023-04-19 12:29:23.944568 prowler_cloud-3.4.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.py
+-rw-r--r--   0        0        0    10499 2023-04-19 12:29:23.944707 prowler_cloud-3.4.1/prowler/providers/aws/services/codeartifact/codeartifact_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.944765 prowler_cloud-3.4.1/prowler/providers/aws/services/codebuild/__init__.py
+-rw-r--r--   0        0        0      210 2023-04-19 12:29:23.944830 prowler_cloud-3.4.1/prowler/providers/aws/services/codebuild/codebuild_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.944884 prowler_cloud-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/__init__.py
+-rw-r--r--   0        0        0     1053 2023-04-19 12:29:23.944969 prowler_cloud-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.metadata.json
+-rw-r--r--   0        0        0     1241 2023-04-19 12:29:23.945033 prowler_cloud-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.945096 prowler_cloud-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/__init__.py
+-rw-r--r--   0        0        0     1018 2023-04-19 12:29:23.945184 prowler_cloud-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.metadata.json
+-rw-r--r--   0        0        0     1049 2023-04-19 12:29:23.945366 prowler_cloud-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.py
+-rw-r--r--   0        0        0     3606 2023-04-19 12:29:23.945608 prowler_cloud-3.4.1/prowler/providers/aws/services/codebuild/codebuild_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.945694 prowler_cloud-3.4.1/prowler/providers/aws/services/config/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-19 12:29:23.945780 prowler_cloud-3.4.1/prowler/providers/aws/services/config/config_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.945850 prowler_cloud-3.4.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/__init__.py
+-rw-r--r--   0        0        0     1326 2023-04-19 12:29:23.945945 prowler_cloud-3.4.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.metadata.json
+-rw-r--r--   0        0        0     1486 2023-04-19 12:29:23.946036 prowler_cloud-3.4.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.py
+-rw-r--r--   0        0        0     3167 2023-04-19 12:29:23.946102 prowler_cloud-3.4.1/prowler/providers/aws/services/config/config_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.946178 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/__init__.py
+-rw-r--r--   0        0        0      254 2023-04-19 12:29:23.946265 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.946353 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/__init__.py
+-rw-r--r--   0        0        0     1191 2023-04-19 12:29:23.946439 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.metadata.json
+-rw-r--r--   0        0        0      997 2023-04-19 12:29:23.946510 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.946579 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/__init__.py
+-rw-r--r--   0        0        0     1187 2023-04-19 12:29:23.946679 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.metadata.json
+-rw-r--r--   0        0        0     1041 2023-04-19 12:29:23.946756 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.946833 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/__init__.py
+-rw-r--r--   0        0        0     1042 2023-04-19 12:29:23.946921 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.metadata.json
+-rw-r--r--   0        0        0     1872 2023-04-19 12:29:23.946998 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.947066 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/__init__.py
+-rw-r--r--   0        0        0     1098 2023-04-19 12:29:23.947152 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.metadata.json
+-rw-r--r--   0        0        0     1660 2023-04-19 12:29:23.947219 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.947291 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/__init__.py
+-rw-r--r--   0        0        0     1533 2023-04-19 12:29:23.947380 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.metadata.json
+-rw-r--r--   0        0        0     1373 2023-04-19 12:29:23.947451 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.py
+-rw-r--r--   0        0        0    12175 2023-04-19 12:29:23.947512 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.947590 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/__init__.py
+-rw-r--r--   0        0        0     1265 2023-04-19 12:29:23.947677 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.metadata.json
+-rw-r--r--   0        0        0     1269 2023-04-19 12:29:23.947755 prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.947825 prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/__init__.py
+-rw-r--r--   0        0        0      190 2023-04-19 12:29:23.947904 prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dax_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.947975 prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1594 2023-04-19 12:29:23.948080 prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      957 2023-04-19 12:29:23.948147 prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.py
+-rw-r--r--   0        0        0      205 2023-04-19 12:29:23.948205 prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_client.py
+-rw-r--r--   0        0        0     8153 2023-04-19 12:29:23.948289 prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.948358 prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1497 2023-04-19 12:29:23.948440 prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      988 2023-04-19 12:29:23.948503 prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.948563 prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/__init__.py
+-rw-r--r--   0        0        0     1529 2023-04-19 12:29:23.948637 prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.metadata.json
+-rw-r--r--   0        0        0      933 2023-04-19 12:29:23.948691 prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.948749 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.948833 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ami_public/__init__.py
+-rw-r--r--   0        0        0     1299 2023-04-19 12:29:23.948914 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.metadata.json
+-rw-r--r--   0        0        0      843 2023-04-19 12:29:23.948970 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:23.949029 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.949092 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/__init__.py
+-rw-r--r--   0        0        0     1192 2023-04-19 12:29:23.949180 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.metadata.json
+-rw-r--r--   0        0        0      783 2023-04-19 12:29:23.949243 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.949304 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/__init__.py
+-rw-r--r--   0        0        0     1176 2023-04-19 12:29:23.949464 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.metadata.json
+-rw-r--r--   0        0        0      965 2023-04-19 12:29:23.949557 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.949630 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/__init__.py
+-rw-r--r--   0        0        0     1530 2023-04-19 12:29:23.949725 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.metadata.json
+-rw-r--r--   0        0        0      922 2023-04-19 12:29:23.949801 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.949868 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/__init__.py
+-rw-r--r--   0        0        0     1239 2023-04-19 12:29:23.949957 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.metadata.json
+-rw-r--r--   0        0        0      849 2023-04-19 12:29:23.950030 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.950097 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/__init__.py
+-rw-r--r--   0        0        0     1057 2023-04-19 12:29:23.950180 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.metadata.json
+-rw-r--r--   0        0        0     2037 2023-04-19 12:29:23.950242 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.950302 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/__init__.py
+-rw-r--r--   0        0        0     1107 2023-04-19 12:29:23.950384 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.metadata.json
+-rw-r--r--   0        0        0      971 2023-04-19 12:29:23.950439 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.950496 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/__init__.py
+-rw-r--r--   0        0        0     1461 2023-04-19 12:29:23.950579 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.metadata.json
+-rw-r--r--   0        0        0     1179 2023-04-19 12:29:23.950656 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.950724 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/__init__.py
+-rw-r--r--   0        0        0     1067 2023-04-19 12:29:23.950816 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.metadata.json
+-rw-r--r--   0        0        0     1111 2023-04-19 12:29:23.950882 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.950943 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/__init__.py
+-rw-r--r--   0        0        0     1174 2023-04-19 12:29:23.951025 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.metadata.json
+-rw-r--r--   0        0        0     1253 2023-04-19 12:29:23.951080 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.951148 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/__init__.py
+-rw-r--r--   0        0        0     1201 2023-04-19 12:29:23.951220 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.metadata.json
+-rw-r--r--   0        0        0     1491 2023-04-19 12:29:23.951290 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.951360 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/__init__.py
+-rw-r--r--   0        0        0     1543 2023-04-19 12:29:23.951437 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.metadata.json
+-rw-r--r--   0        0        0     1034 2023-04-19 12:29:23.951499 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.951556 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/__init__.py
+-rw-r--r--   0        0        0     1141 2023-04-19 12:29:23.951627 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.metadata.json
+-rw-r--r--   0        0        0     1118 2023-04-19 12:29:23.951691 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.951757 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/__init__.py
+-rw-r--r--   0        0        0     1292 2023-04-19 12:29:23.951839 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.metadata.json
+-rw-r--r--   0        0        0     2348 2023-04-19 12:29:23.951906 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.py
+-rw-r--r--   0        0        0       78 2023-04-19 12:29:23.951997 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/fixtures/fixture
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.952059 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/__init__.py
+-rw-r--r--   0        0        0     1378 2023-04-19 12:29:23.952133 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.metadata.json
+-rw-r--r--   0        0        0     1247 2023-04-19 12:29:23.952190 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.952247 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/__init__.py
+-rw-r--r--   0        0        0     1483 2023-04-19 12:29:23.952329 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.metadata.json
+-rw-r--r--   0        0        0     1268 2023-04-19 12:29:23.952407 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.952471 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/__init__.py
+-rw-r--r--   0        0        0     1513 2023-04-19 12:29:23.952556 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.metadata.json
+-rw-r--r--   0        0        0     1296 2023-04-19 12:29:23.952633 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.952700 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/__init__.py
+-rw-r--r--   0        0        0     1139 2023-04-19 12:29:23.952777 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.metadata.json
+-rw-r--r--   0        0        0     1323 2023-04-19 12:29:23.952846 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.952917 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/__init__.py
+-rw-r--r--   0        0        0     1197 2023-04-19 12:29:23.953015 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.metadata.json
+-rw-r--r--   0        0        0     1468 2023-04-19 12:29:23.953101 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.953177 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/__init__.py
+-rw-r--r--   0        0        0     1169 2023-04-19 12:29:23.953258 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.metadata.json
+-rw-r--r--   0        0        0     1436 2023-04-19 12:29:23.953328 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.953390 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/__init__.py
+-rw-r--r--   0        0        0     1429 2023-04-19 12:29:23.953489 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.metadata.json
+-rw-r--r--   0        0        0     1409 2023-04-19 12:29:23.953553 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.953618 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/__init__.py
+-rw-r--r--   0        0        0     1371 2023-04-19 12:29:23.953692 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.metadata.json
+-rw-r--r--   0        0        0     1437 2023-04-19 12:29:23.953786 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.953865 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/__init__.py
+-rw-r--r--   0        0        0     1220 2023-04-19 12:29:23.953950 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.metadata.json
+-rw-r--r--   0        0        0     1497 2023-04-19 12:29:23.954013 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.954078 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/__init__.py
+-rw-r--r--   0        0        0     1211 2023-04-19 12:29:23.954157 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.metadata.json
+-rw-r--r--   0        0        0     1532 2023-04-19 12:29:23.954241 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.954310 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/__init__.py
+-rw-r--r--   0        0        0     1164 2023-04-19 12:29:23.954387 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.metadata.json
+-rw-r--r--   0        0        0     1427 2023-04-19 12:29:23.954452 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.954527 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/__init__.py
+-rw-r--r--   0        0        0     1179 2023-04-19 12:29:23.954613 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.metadata.json
+-rw-r--r--   0        0        0     1443 2023-04-19 12:29:23.954685 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.954805 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/__init__.py
+-rw-r--r--   0        0        0     1165 2023-04-19 12:29:23.954886 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.metadata.json
+-rw-r--r--   0        0        0     1486 2023-04-19 12:29:23.954956 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.955027 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/__init__.py
+-rw-r--r--   0        0        0     1190 2023-04-19 12:29:23.955101 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.metadata.json
+-rw-r--r--   0        0        0     1461 2023-04-19 12:29:23.955156 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.955225 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/__init__.py
+-rw-r--r--   0        0        0     1173 2023-04-19 12:29:23.955470 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.metadata.json
+-rw-r--r--   0        0        0     1436 2023-04-19 12:29:23.955638 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.955701 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/__init__.py
+-rw-r--r--   0        0        0     1164 2023-04-19 12:29:23.955778 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.metadata.json
+-rw-r--r--   0        0        0     1427 2023-04-19 12:29:23.955843 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.955937 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/__init__.py
+-rw-r--r--   0        0        0     1218 2023-04-19 12:29:23.956030 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.metadata.json
+-rw-r--r--   0        0        0     1499 2023-04-19 12:29:23.956108 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.956187 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/__init__.py
+-rw-r--r--   0        0        0     1161 2023-04-19 12:29:23.956261 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.metadata.json
+-rw-r--r--   0        0        0     1422 2023-04-19 12:29:23.956316 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.956378 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/__init__.py
+-rw-r--r--   0        0        0     1127 2023-04-19 12:29:23.956461 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.metadata.json
+-rw-r--r--   0        0        0     2440 2023-04-19 12:29:23.956526 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.956612 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/__init__.py
+-rw-r--r--   0        0        0     1374 2023-04-19 12:29:23.956694 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.metadata.json
+-rw-r--r--   0        0        0     1305 2023-04-19 12:29:23.956775 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.956843 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/__init__.py
+-rw-r--r--   0        0        0     1221 2023-04-19 12:29:23.956915 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.metadata.json
+-rw-r--r--   0        0        0     1029 2023-04-19 12:29:23.956978 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.957038 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/__init__.py
+-rw-r--r--   0        0        0     1043 2023-04-19 12:29:23.957111 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.metadata.json
+-rw-r--r--   0        0        0     1144 2023-04-19 12:29:23.957178 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.957238 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/__init__.py
+-rw-r--r--   0        0        0     1080 2023-04-19 12:29:23.957327 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.metadata.json
+-rw-r--r--   0        0        0     1219 2023-04-19 12:29:23.957388 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.py
+-rw-r--r--   0        0        0    18754 2023-04-19 12:29:23.957527 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.957595 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/lib/__init__.py
+-rw-r--r--   0        0        0     2581 2023-04-19 12:29:23.957667 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/lib/network_acls.py
+-rw-r--r--   0        0        0     3766 2023-04-19 12:29:23.957735 prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/lib/security_groups.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.957793 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:23.957867 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.957926 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/__init__.py
+-rw-r--r--   0        0        0     1375 2023-04-19 12:29:23.958354 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.metadata.json
+-rw-r--r--   0        0        0     1302 2023-04-19 12:29:23.958488 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.958564 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/__init__.py
+-rw-r--r--   0        0        0     1123 2023-04-19 12:29:23.958647 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.metadata.json
+-rw-r--r--   0        0        0      973 2023-04-19 12:29:23.958715 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.958786 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1213 2023-04-19 12:29:23.958874 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1322 2023-04-19 12:29:23.958949 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.959014 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/__init__.py
+-rw-r--r--   0        0        0     1501 2023-04-19 12:29:23.959140 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.metadata.json
+-rw-r--r--   0        0        0      990 2023-04-19 12:29:23.959214 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.959276 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/__init__.py
+-rw-r--r--   0        0        0     1268 2023-04-19 12:29:23.959354 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.metadata.json
+-rw-r--r--   0        0        0     2034 2023-04-19 12:29:23.959422 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.py
+-rw-r--r--   0        0        0    10008 2023-04-19 12:29:23.959556 prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.959623 prowler_cloud-3.4.1/prowler/providers/aws/services/ecs/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:23.959708 prowler_cloud-3.4.1/prowler/providers/aws/services/ecs/ecs_client.py
+-rw-r--r--   0        0        0     3857 2023-04-19 12:29:23.959800 prowler_cloud-3.4.1/prowler/providers/aws/services/ecs/ecs_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.959863 prowler_cloud-3.4.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/__init__.py
+-rw-r--r--   0        0        0     1625 2023-04-19 12:29:23.959946 prowler_cloud-3.4.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.metadata.json
+-rw-r--r--   0        0        0     2328 2023-04-19 12:29:23.960011 prowler_cloud-3.4.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.960125 prowler_cloud-3.4.1/prowler/providers/aws/services/efs/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:23.960222 prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.960305 prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/__init__.py
+-rw-r--r--   0        0        0     1366 2023-04-19 12:29:23.960396 prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.metadata.json
+-rw-r--r--   0        0        0      853 2023-04-19 12:29:23.960463 prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.960528 prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/__init__.py
+-rw-r--r--   0        0        0     1099 2023-04-19 12:29:23.960600 prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.metadata.json
+-rw-r--r--   0        0        0      843 2023-04-19 12:29:23.960658 prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.960737 prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0      981 2023-04-19 12:29:23.960839 prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1853 2023-04-19 12:29:23.960935 prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.py
+-rw-r--r--   0        0        0     3889 2023-04-19 12:29:23.961042 prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.961116 prowler_cloud-3.4.1/prowler/providers/aws/services/eks/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:23.961185 prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.961253 prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/__init__.py
+-rw-r--r--   0        0        0     1362 2023-04-19 12:29:23.961335 prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.metadata.json
+-rw-r--r--   0        0        0      992 2023-04-19 12:29:23.961410 prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.961481 prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/__init__.py
+-rw-r--r--   0        0        0     1559 2023-04-19 12:29:23.961578 prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.metadata.json
+-rw-r--r--   0        0        0     1215 2023-04-19 12:29:23.961639 prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.961713 prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/__init__.py
+-rw-r--r--   0        0        0     1374 2023-04-19 12:29:23.961815 prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.metadata.json
+-rw-r--r--   0        0        0     1489 2023-04-19 12:29:23.961889 prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.961959 prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1533 2023-04-19 12:29:23.962044 prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1020 2023-04-19 12:29:23.962138 prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.py
+-rw-r--r--   0        0        0     4579 2023-04-19 12:29:23.962243 prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.962323 prowler_cloud-3.4.1/prowler/providers/aws/services/elb/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:23.962401 prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.962478 prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/__init__.py
+-rw-r--r--   0        0        0     1364 2023-04-19 12:29:23.962564 prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.metadata.json
+-rw-r--r--   0        0        0     1115 2023-04-19 12:29:23.962633 prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.962724 prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_internet_facing/__init__.py
+-rw-r--r--   0        0        0     1111 2023-04-19 12:29:23.962884 prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.metadata.json
+-rw-r--r--   0        0        0      823 2023-04-19 12:29:23.963014 prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.963091 prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1392 2023-04-19 12:29:23.963168 prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.metadata.json
+-rw-r--r--   0        0        0      817 2023-04-19 12:29:23.963238 prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.py
+-rw-r--r--   0        0        0     4592 2023-04-19 12:29:23.963365 prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.963437 prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_ssl_listeners/__init__.py
+-rw-r--r--   0        0        0     1360 2023-04-19 12:29:23.963512 prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.metadata.json
+-rw-r--r--   0        0        0      937 2023-04-19 12:29:23.963596 prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.963667 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/__init__.py
+-rw-r--r--   0        0        0      190 2023-04-19 12:29:23.963732 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.963789 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/__init__.py
+-rw-r--r--   0        0        0     1347 2023-04-19 12:29:23.963879 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.metadata.json
+-rw-r--r--   0        0        0      892 2023-04-19 12:29:23.963953 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.964013 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/__init__.py
+-rw-r--r--   0        0        0     1718 2023-04-19 12:29:23.964087 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.metadata.json
+-rw-r--r--   0        0        0     1367 2023-04-19 12:29:23.964151 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.964211 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/__init__.py
+-rw-r--r--   0        0        0     1337 2023-04-19 12:29:23.964275 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.metadata.json
+-rw-r--r--   0        0        0     1646 2023-04-19 12:29:23.964347 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.964420 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/__init__.py
+-rw-r--r--   0        0        0     1162 2023-04-19 12:29:23.964495 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.metadata.json
+-rw-r--r--   0        0        0      888 2023-04-19 12:29:23.964568 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.964639 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/__init__.py
+-rw-r--r--   0        0        0      996 2023-04-19 12:29:23.964720 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.metadata.json
+-rw-r--r--   0        0        0      836 2023-04-19 12:29:23.964781 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.964855 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1435 2023-04-19 12:29:23.964939 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.metadata.json
+-rw-r--r--   0        0        0      924 2023-04-19 12:29:23.965007 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.py
+-rw-r--r--   0        0        0     7882 2023-04-19 12:29:23.965093 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.965174 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/__init__.py
+-rw-r--r--   0        0        0     1325 2023-04-19 12:29:23.965247 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.metadata.json
+-rw-r--r--   0        0        0     1664 2023-04-19 12:29:23.965315 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.965389 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/__init__.py
+-rw-r--r--   0        0        0     1004 2023-04-19 12:29:23.965478 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.metadata.json
+-rw-r--r--   0        0        0     1439 2023-04-19 12:29:23.965558 prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.965631 prowler_cloud-3.4.1/prowler/providers/aws/services/emr/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:23.965708 prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.965783 prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/__init__.py
+-rw-r--r--   0        0        0     1029 2023-04-19 12:29:23.965875 prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.metadata.json
+-rw-r--r--   0        0        0      917 2023-04-19 12:29:23.965953 prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.966035 prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/__init__.py
+-rw-r--r--   0        0        0      897 2023-04-19 12:29:23.966124 prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.metadata.json
+-rw-r--r--   0        0        0     1200 2023-04-19 12:29:23.966202 prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.966274 prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/__init__.py
+-rw-r--r--   0        0        0     1018 2023-04-19 12:29:23.966359 prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.metadata.json
+-rw-r--r--   0        0        0     4444 2023-04-19 12:29:23.966445 prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.py
+-rw-r--r--   0        0        0     7714 2023-04-19 12:29:23.966535 prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.966618 prowler_cloud-3.4.1/prowler/providers/aws/services/glacier/__init__.py
+-rw-r--r--   0        0        0      200 2023-04-19 12:29:23.966702 prowler_cloud-3.4.1/prowler/providers/aws/services/glacier/glacier_client.py
+-rw-r--r--   0        0        0     3995 2023-04-19 12:29:23.966792 prowler_cloud-3.4.1/prowler/providers/aws/services/glacier/glacier_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.966878 prowler_cloud-3.4.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/__init__.py
+-rw-r--r--   0        0        0     1219 2023-04-19 12:29:23.966963 prowler_cloud-3.4.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.metadata.json
+-rw-r--r--   0        0        0     1940 2023-04-19 12:29:23.967043 prowler_cloud-3.4.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.967105 prowler_cloud-3.4.1/prowler/providers/aws/services/globalaccelerator/__init__.py
+-rw-r--r--   0        0        0      259 2023-04-19 12:29:23.967180 prowler_cloud-3.4.1/prowler/providers/aws/services/globalaccelerator/globalaccelerator_client.py
+-rw-r--r--   0        0        0     2362 2023-04-19 12:29:23.967253 prowler_cloud-3.4.1/prowler/providers/aws/services/globalaccelerator/globalaccelerator_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.967325 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/__init__.py
+-rw-r--r--   0        0        0      185 2023-04-19 12:29:23.967397 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.967474 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1464 2023-04-19 12:29:23.967574 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      928 2023-04-19 12:29:23.967664 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.967737 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1539 2023-04-19 12:29:23.967812 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      920 2023-04-19 12:29:23.967877 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.967951 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/__init__.py
+-rw-r--r--   0        0        0     1222 2023-04-19 12:29:23.968034 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.metadata.json
+-rw-r--r--   0        0        0      884 2023-04-19 12:29:23.968106 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.968182 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1632 2023-04-19 12:29:23.968257 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1361 2023-04-19 12:29:23.968320 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.968383 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1623 2023-04-19 12:29:23.968454 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1352 2023-04-19 12:29:23.968520 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.968592 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1644 2023-04-19 12:29:23.968667 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1322 2023-04-19 12:29:23.968732 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.968797 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1574 2023-04-19 12:29:23.968878 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1622 2023-04-19 12:29:23.968944 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.969022 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1600 2023-04-19 12:29:23.969110 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1293 2023-04-19 12:29:23.969174 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.969240 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1591 2023-04-19 12:29:23.969311 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1284 2023-04-19 12:29:23.969372 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.py
+-rw-r--r--   0        0        0     9722 2023-04-19 12:29:23.969452 prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.969509 prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.969576 prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/__init__.py
+-rw-r--r--   0        0        0      998 2023-04-19 12:29:23.969697 prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.metadata.json
+-rw-r--r--   0        0        0     1221 2023-04-19 12:29:23.969805 prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.py
+-rw-r--r--   0        0        0      210 2023-04-19 12:29:23.969867 prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.969929 prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1282 2023-04-19 12:29:23.970039 prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1130 2023-04-19 12:29:23.970105 prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.970169 prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/__init__.py
+-rw-r--r--   0        0        0     1179 2023-04-19 12:29:23.970275 prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.metadata.json
+-rw-r--r--   0        0        0      961 2023-04-19 12:29:23.970332 prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.py
+-rw-r--r--   0        0        0     7252 2023-04-19 12:29:23.970460 prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.970527 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.970612 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/__init__.py
+-rw-r--r--   0        0        0     1010 2023-04-19 12:29:23.970708 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.metadata.json
+-rw-r--r--   0        0        0     1933 2023-04-19 12:29:23.970784 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.970861 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/__init__.py
+-rw-r--r--   0        0        0     1112 2023-04-19 12:29:23.970944 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.metadata.json
+-rw-r--r--   0        0        0     2805 2023-04-19 12:29:23.971012 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:30:31.789842 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/__init__.py
+-rw-r--r--   0        0        0     2073 2023-04-19 14:30:31.790116 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.metadata.json
+-rw-r--r--   0        0        0     2227 2023-04-19 14:30:31.790324 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.971078 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/__init__.py
+-rw-r--r--   0        0        0     1494 2023-04-19 12:29:23.971163 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.metadata.json
+-rw-r--r--   0        0        0      802 2023-04-19 12:29:23.971231 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:23.971296 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:30:31.790386 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/__init__.py
+-rw-r--r--   0        0        0     2088 2023-04-19 14:30:31.790500 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.metadata.json
+-rw-r--r--   0        0        0     2238 2023-04-19 14:30:31.790593 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:30:31.790657 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/__init__.py
+-rw-r--r--   0        0        0     2118 2023-04-19 14:30:31.790778 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.metadata.json
+-rw-r--r--   0        0        0     2251 2023-04-19 14:30:31.790879 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.971377 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/__init__.py
+-rw-r--r--   0        0        0     1413 2023-04-19 12:29:23.971535 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.metadata.json
+-rw-r--r--   0        0        0     4192 2023-04-19 12:29:23.971628 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.971705 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/__init__.py
+-rw-r--r--   0        0        0     1413 2023-04-19 12:29:23.971792 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.metadata.json
+-rw-r--r--   0        0        0     4146 2023-04-19 12:29:23.971858 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.971926 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/__init__.py
+-rw-r--r--   0        0        0     1417 2023-04-19 12:29:23.972003 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.metadata.json
+-rw-r--r--   0        0        0     4192 2023-04-19 12:29:23.972081 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.972166 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/__init__.py
+-rw-r--r--   0        0        0     1089 2023-04-19 12:29:23.972256 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.metadata.json
+-rw-r--r--   0        0        0     2665 2023-04-19 14:30:31.791220 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.972389 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/__init__.py
+-rw-r--r--   0        0        0     1707 2023-04-19 12:29:23.972482 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.metadata.json
+-rw-r--r--   0        0        0     1090 2023-04-19 12:29:23.972558 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.972624 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_no_root_access_key/__init__.py
+-rw-r--r--   0        0        0     1453 2023-04-19 12:29:23.972706 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.metadata.json
+-rw-r--r--   0        0        0     1541 2023-04-19 12:29:23.972769 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.972838 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/__init__.py
+-rw-r--r--   0        0        0     1314 2023-04-19 12:29:23.972940 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.metadata.json
+-rw-r--r--   0        0        0     1360 2023-04-19 12:29:23.973008 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.973071 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/__init__.py
+-rw-r--r--   0        0        0     1299 2023-04-19 12:29:23.973150 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.metadata.json
+-rw-r--r--   0        0        0     1086 2023-04-19 12:29:23.973217 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.973285 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/__init__.py
+-rw-r--r--   0        0        0     1299 2023-04-19 12:29:23.973378 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.metadata.json
+-rw-r--r--   0        0        0     1185 2023-04-19 12:29:23.973440 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.973504 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_number/__init__.py
+-rw-r--r--   0        0        0     1254 2023-04-19 12:29:23.973578 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.metadata.json
+-rw-r--r--   0        0        0     1095 2023-04-19 12:29:23.973645 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.973709 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/__init__.py
+-rw-r--r--   0        0        0     1280 2023-04-19 12:29:23.973792 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.metadata.json
+-rw-r--r--   0        0        0     1231 2023-04-19 12:29:23.973863 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.973931 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/__init__.py
+-rw-r--r--   0        0        0     1294 2023-04-19 12:29:23.974020 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.metadata.json
+-rw-r--r--   0        0        0     1095 2023-04-19 12:29:23.974086 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.974151 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/__init__.py
+-rw-r--r--   0        0        0     1300 2023-04-19 12:29:23.974224 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.metadata.json
+-rw-r--r--   0        0        0     1083 2023-04-19 12:29:23.974290 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.974357 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/__init__.py
+-rw-r--r--   0        0        0     1223 2023-04-19 12:29:23.974457 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.metadata.json
+-rw-r--r--   0        0        0     6229 2023-04-20 14:41:59.231195 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.974606 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/__init__.py
+-rw-r--r--   0        0        0     1533 2023-04-19 12:29:23.974689 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.metadata.json
+-rw-r--r--   0        0        0     1925 2023-04-19 12:29:23.974757 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.975046 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/__init__.py
+-rw-r--r--   0        0        0     1384 2023-04-19 12:29:23.975177 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.metadata.json
+-rw-r--r--   0        0        0     2059 2023-04-19 14:30:31.791710 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.975347 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/__init__.py
+-rw-r--r--   0        0        0     1356 2023-04-19 12:29:23.975454 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.metadata.json
+-rw-r--r--   0        0        0     2045 2023-04-19 14:30:31.791846 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.975766 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/__init__.py
+-rw-r--r--   0        0        0     1174 2023-04-19 12:29:23.975851 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.metadata.json
+-rw-r--r--   0        0        0     3534 2023-04-21 08:58:58.224015 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.975982 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/__init__.py
+-rw-r--r--   0        0        0     1424 2023-04-19 12:29:23.976060 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.metadata.json
+-rw-r--r--   0        0        0     1595 2023-04-19 12:29:23.976119 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.976178 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/__init__.py
+-rw-r--r--   0        0        0     1738 2023-04-19 12:29:23.976255 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.metadata.json
+-rw-r--r--   0        0        0     1020 2023-04-19 12:29:23.976311 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.976377 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/__init__.py
+-rw-r--r--   0        0        0     1424 2023-04-19 12:29:23.976446 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.metadata.json
+-rw-r--r--   0        0        0     2832 2023-04-19 12:29:23.976523 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.976606 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/__init__.py
+-rw-r--r--   0        0        0     1335 2023-04-19 12:29:23.976734 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.metadata.json
+-rw-r--r--   0        0        0      901 2023-04-19 12:29:23.976840 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.py
+-rw-r--r--   0        0        0    21365 2023-04-20 16:55:17.936940 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.977064 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_support_role_created/__init__.py
+-rw-r--r--   0        0        0     1256 2023-04-19 12:29:23.977144 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.metadata.json
+-rw-r--r--   0        0        0      940 2023-04-19 12:29:23.977241 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.977300 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/__init__.py
+-rw-r--r--   0        0        0     1061 2023-04-19 12:29:23.977369 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.metadata.json
+-rw-r--r--   0        0        0     1341 2023-04-19 12:29:23.977431 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.977490 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/__init__.py
+-rw-r--r--   0        0        0     1309 2023-04-19 12:29:23.977576 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.metadata.json
+-rw-r--r--   0        0        0     1698 2023-04-19 12:29:23.977650 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.977716 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/__init__.py
+-rw-r--r--   0        0        0     1671 2023-04-19 12:29:23.977798 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.metadata.json
+-rw-r--r--   0        0        0     2671 2023-04-19 12:29:23.977863 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.977919 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/__init__.py
+-rw-r--r--   0        0        0      998 2023-04-19 12:29:23.977991 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.metadata.json
+-rw-r--r--   0        0        0     1341 2023-04-19 12:29:23.978054 prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.978113 prowler_cloud-3.4.1/prowler/providers/aws/services/kms/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:23.978191 prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.978250 prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_cmk_are_used/__init__.py
+-rw-r--r--   0        0        0     1053 2023-04-19 12:29:23.978323 prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.metadata.json
+-rw-r--r--   0        0        0     1194 2023-04-19 12:29:23.978399 prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.978466 prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/__init__.py
+-rw-r--r--   0        0        0     1309 2023-04-19 12:29:23.978546 prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.metadata.json
+-rw-r--r--   0        0        0     1294 2023-04-19 12:29:23.978604 prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.978665 prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1354 2023-04-19 12:29:23.978738 prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     2525 2023-04-19 12:29:23.978835 prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py
+-rw-r--r--   0        0        0     5255 2023-04-19 12:29:23.978919 prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.978985 prowler_cloud-3.4.1/prowler/providers/aws/services/macie/__init__.py
+-rw-r--r--   0        0        0      190 2023-04-19 12:29:23.979068 prowler_cloud-3.4.1/prowler/providers/aws/services/macie/macie_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.979172 prowler_cloud-3.4.1/prowler/providers/aws/services/macie/macie_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1065 2023-04-19 12:29:23.979278 prowler_cloud-3.4.1/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.metadata.json
+-rw-r--r--   0        0        0      894 2023-04-19 12:29:23.979368 prowler_cloud-3.4.1/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.py
+-rw-r--r--   0        0        0     1785 2023-04-19 12:29:23.979447 prowler_cloud-3.4.1/prowler/providers/aws/services/macie/macie_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.979538 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/__init__.py
+-rw-r--r--   0        0        0      238 2023-04-19 12:29:23.979628 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_client.py
+-rw-r--r--   0        0        0     6959 2023-04-19 12:29:23.979719 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.979801 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1124 2023-04-19 12:29:23.979914 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1102 2023-04-19 12:29:23.979989 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.980060 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1478 2023-04-19 12:29:23.980138 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1871 2023-04-19 12:29:23.980196 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.980261 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/__init__.py
+-rw-r--r--   0        0        0     1555 2023-04-19 12:29:23.980344 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.metadata.json
+-rw-r--r--   0        0        0     1003 2023-04-19 12:29:23.980412 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.980494 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/__init__.py
+-rw-r--r--   0        0        0     1281 2023-04-19 12:29:23.980571 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.metadata.json
+-rw-r--r--   0        0        0      991 2023-04-19 12:29:23.980633 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.980699 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/__init__.py
+-rw-r--r--   0        0        0     1128 2023-04-19 12:29:23.980766 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.metadata.json
+-rw-r--r--   0        0        0      983 2023-04-19 12:29:23.980826 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.980887 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1766 2023-04-19 12:29:23.980964 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1023 2023-04-19 12:29:23.981024 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.981096 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1281 2023-04-19 12:29:23.981163 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     2655 2023-04-19 12:29:23.981223 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.981286 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/__init__.py
+-rw-r--r--   0        0        0     1736 2023-04-19 12:29:23.981364 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.metadata.json
+-rw-r--r--   0        0        0     1046 2023-04-19 12:29:23.981430 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.981492 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/__init__.py
+-rw-r--r--   0        0        0     1242 2023-04-19 12:29:23.981574 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.metadata.json
+-rw-r--r--   0        0        0     1023 2023-04-19 12:29:23.981643 prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.981710 prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.981781 prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/__init__.py
+-rw-r--r--   0        0        0     1359 2023-04-19 12:29:23.981880 prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.metadata.json
+-rw-r--r--   0        0        0      984 2023-04-19 12:29:23.981978 prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.py
+-rw-r--r--   0        0        0      239 2023-04-19 12:29:23.982039 prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.982100 prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/__init__.py
+-rw-r--r--   0        0        0     1579 2023-04-19 12:29:23.982181 prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.metadata.json
+-rw-r--r--   0        0        0     1816 2023-04-19 12:29:23.982292 prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.982372 prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/__init__.py
+-rw-r--r--   0        0        0     1548 2023-04-19 12:29:23.982458 prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.metadata.json
+-rw-r--r--   0        0        0     5605 2023-04-19 12:29:23.982567 prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.py
+-rw-r--r--   0        0        0     8903 2023-04-19 12:29:23.982687 prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.982747 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:23.982808 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.982868 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/__init__.py
+-rw-r--r--   0        0        0     1473 2023-04-19 12:29:23.982939 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.metadata.json
+-rw-r--r--   0        0        0      984 2023-04-19 12:29:23.983003 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.983065 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/__init__.py
+-rw-r--r--   0        0        0     1367 2023-04-19 12:29:23.983129 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.metadata.json
+-rw-r--r--   0        0        0      980 2023-04-19 12:29:23.983184 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.983243 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/__init__.py
+-rw-r--r--   0        0        0     1309 2023-04-19 12:29:23.983318 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.metadata.json
+-rw-r--r--   0        0        0      960 2023-04-19 12:29:23.983380 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.983450 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/__init__.py
+-rw-r--r--   0        0        0     1488 2023-04-19 12:29:23.983528 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.metadata.json
+-rw-r--r--   0        0        0      947 2023-04-19 12:29:23.983588 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.983654 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/__init__.py
+-rw-r--r--   0        0        0     1732 2023-04-19 12:29:23.983734 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.metadata.json
+-rw-r--r--   0        0        0      969 2023-04-19 12:29:23.983790 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.983846 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_multi_az/__init__.py
+-rw-r--r--   0        0        0     1309 2023-04-19 12:29:23.983913 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.metadata.json
+-rw-r--r--   0        0        0      944 2023-04-19 12:29:23.983967 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.984024 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/__init__.py
+-rw-r--r--   0        0        0     1426 2023-04-19 12:29:23.984110 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.metadata.json
+-rw-r--r--   0        0        0      959 2023-04-19 12:29:23.984175 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.984238 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/__init__.py
+-rw-r--r--   0        0        0     1370 2023-04-19 12:29:23.984322 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.metadata.json
+-rw-r--r--   0        0        0      892 2023-04-19 12:29:23.984376 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.984438 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/__init__.py
+-rw-r--r--   0        0        0     1510 2023-04-19 12:29:23.984507 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.metadata.json
+-rw-r--r--   0        0        0     1367 2023-04-20 13:29:08.794503 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.py
+-rw-r--r--   0        0        0    10647 2023-04-19 12:29:23.984614 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.984675 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/__init__.py
+-rw-r--r--   0        0        0     1552 2023-04-19 12:29:23.984750 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.metadata.json
+-rw-r--r--   0        0        0     1543 2023-04-19 12:29:23.984811 prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.984870 prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/__init__.py
+-rw-r--r--   0        0        0      205 2023-04-19 12:29:23.984935 prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.985000 prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/__init__.py
+-rw-r--r--   0        0        0     1384 2023-04-19 12:29:23.985070 prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.metadata.json
+-rw-r--r--   0        0        0      973 2023-04-19 12:29:23.985129 prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.985188 prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/__init__.py
+-rw-r--r--   0        0        0     1204 2023-04-19 12:29:23.985268 prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.metadata.json
+-rw-r--r--   0        0        0      984 2023-04-19 12:29:23.985335 prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.985415 prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/__init__.py
+-rw-r--r--   0        0        0     1285 2023-04-20 13:29:08.795139 prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.metadata.json
+-rw-r--r--   0        0        0      996 2023-04-19 12:29:23.985566 prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.985646 prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/__init__.py
+-rw-r--r--   0        0        0     1297 2023-04-19 12:29:23.985733 prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.metadata.json
+-rw-r--r--   0        0        0      992 2023-04-19 12:29:23.985798 prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.py
+-rw-r--r--   0        0        0     4912 2023-04-19 12:29:23.985905 prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.985981 prowler_cloud-3.4.1/prowler/providers/aws/services/resourceexplorer2/__init__.py
+-rw-r--r--   0        0        0      261 2023-04-19 12:29:23.986103 prowler_cloud-3.4.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.986181 prowler_cloud-3.4.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/__init__.py
+-rw-r--r--   0        0        0      973 2023-04-19 12:29:23.986311 prowler_cloud-3.4.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.metadata.json
+-rw-r--r--   0        0        0      940 2023-04-19 12:29:23.986424 prowler_cloud-3.4.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.py
+-rw-r--r--   0        0        0     2344 2023-04-19 12:29:23.986545 prowler_cloud-3.4.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.986621 prowler_cloud-3.4.1/prowler/providers/aws/services/route53/__init__.py
+-rw-r--r--   0        0        0      200 2023-04-19 12:29:23.986702 prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.986785 prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/__init__.py
+-rw-r--r--   0        0        0     1188 2023-04-19 12:29:23.986873 prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.metadata.json
+-rw-r--r--   0        0        0     1023 2023-04-19 12:29:23.986944 prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.987014 prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/__init__.py
+-rw-r--r--   0        0        0      998 2023-04-19 12:29:23.987103 prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.metadata.json
+-rw-r--r--   0        0        0     1058 2023-04-19 12:29:23.987177 prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.987269 prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1362 2023-04-19 12:29:23.987366 prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1249 2023-04-19 12:29:23.987444 prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.py
+-rw-r--r--   0        0        0     6911 2023-04-19 12:29:23.987538 prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_service.py
+-rw-r--r--   0        0        0      221 2023-04-19 12:29:23.987613 prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53domains_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.987693 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.987787 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/__init__.py
+-rw-r--r--   0        0        0     1392 2023-04-19 12:29:23.987884 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.metadata.json
+-rw-r--r--   0        0        0     1068 2023-04-19 12:29:23.987956 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.988015 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/__init__.py
+-rw-r--r--   0        0        0     1266 2023-04-19 12:29:23.988088 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.metadata.json
+-rw-r--r--   0        0        0      957 2023-04-19 12:29:23.988152 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.988226 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/__init__.py
+-rw-r--r--   0        0        0     1459 2023-04-19 12:29:23.988319 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.metadata.json
+-rw-r--r--   0        0        0      917 2023-04-19 12:29:23.988387 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.988462 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/__init__.py
+-rw-r--r--   0        0        0     1496 2023-04-19 12:29:23.988553 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.metadata.json
+-rw-r--r--   0        0        0     1123 2023-04-19 12:29:23.988658 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.988729 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/__init__.py
+-rw-r--r--   0        0        0     1426 2023-04-19 12:29:23.988821 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.metadata.json
+-rw-r--r--   0        0        0      943 2023-04-19 12:29:23.988889 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.988968 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/__init__.py
+-rw-r--r--   0        0        0     1212 2023-04-19 12:29:23.989059 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.metadata.json
+-rw-r--r--   0        0        0      947 2023-04-19 12:29:23.989147 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.989246 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/__init__.py
+-rw-r--r--   0        0        0     1080 2023-04-19 12:29:23.989355 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.metadata.json
+-rw-r--r--   0        0        0     1716 2023-04-19 12:29:23.989421 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.989491 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_public_access/__init__.py
+-rw-r--r--   0        0        0     1939 2023-04-19 12:29:23.989572 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.metadata.json
+-rw-r--r--   0        0        0     4014 2023-04-19 12:29:23.989689 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.989751 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/__init__.py
+-rw-r--r--   0        0        0     1190 2023-04-19 12:29:23.989835 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.metadata.json
+-rw-r--r--   0        0        0     2099 2023-04-19 12:29:23.989900 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.989969 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1372 2023-04-19 12:29:23.990050 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.metadata.json
+-rw-r--r--   0        0        0      978 2023-04-19 12:29:23.990109 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.py
+-rw-r--r--   0        0        0      175 2023-04-19 12:29:23.990183 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_client.py
+-rw-r--r--   0        0        0    14801 2023-04-25 11:40:22.196393 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_service.py
+-rw-r--r--   0        0        0      196 2023-04-19 12:29:23.990316 prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3control_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.990374 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/__init__.py
+-rw-r--r--   0        0        0      210 2023-04-19 12:29:23.990438 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.990496 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/__init__.py
+-rw-r--r--   0        0        0     1100 2023-04-19 12:29:23.990579 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.metadata.json
+-rw-r--r--   0        0        0      945 2023-04-19 12:29:23.990641 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.990707 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/__init__.py
+-rw-r--r--   0        0        0     1094 2023-04-19 12:29:23.990791 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.metadata.json
+-rw-r--r--   0        0        0      966 2023-04-19 12:29:23.990864 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.990928 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1412 2023-04-19 12:29:23.991009 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1046 2023-04-19 12:29:23.991068 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.991133 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/__init__.py
+-rw-r--r--   0        0        0     1227 2023-04-19 12:29:23.991201 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.metadata.json
+-rw-r--r--   0        0        0     1037 2023-04-19 12:29:23.991261 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.991361 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/__init__.py
+-rw-r--r--   0        0        0     1361 2023-04-19 12:29:23.991468 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.metadata.json
+-rw-r--r--   0        0        0     1063 2023-04-19 12:29:23.991540 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.991611 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/__init__.py
+-rw-r--r--   0        0        0     1524 2023-04-19 12:29:23.991699 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.metadata.json
+-rw-r--r--   0        0        0     1091 2023-04-19 12:29:23.991760 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.py
+-rw-r--r--   0        0        0    11132 2023-04-19 12:29:23.991819 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.991885 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1119 2023-04-19 12:29:23.991978 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1040 2023-04-19 12:29:23.992040 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.992106 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/__init__.py
+-rw-r--r--   0        0        0     1106 2023-04-19 12:29:23.992184 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.metadata.json
+-rw-r--r--   0        0        0     1005 2023-04-19 12:29:23.992243 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.992305 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1179 2023-04-19 12:29:23.992378 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1042 2023-04-19 12:29:23.992438 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.992502 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/__init__.py
+-rw-r--r--   0        0        0     1100 2023-04-19 12:29:23.992573 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.metadata.json
+-rw-r--r--   0        0        0     1072 2023-04-19 12:29:23.992638 prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.992702 prowler_cloud-3.4.1/prowler/providers/aws/services/secretsmanager/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.992781 prowler_cloud-3.4.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/__init__.py
+-rw-r--r--   0        0        0     1341 2023-04-19 12:29:23.992866 prowler_cloud-3.4.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.metadata.json
+-rw-r--r--   0        0        0     1054 2023-04-19 12:29:23.992929 prowler_cloud-3.4.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.py
+-rw-r--r--   0        0        0      244 2023-04-19 12:29:23.992979 prowler_cloud-3.4.1/prowler/providers/aws/services/secretsmanager/secretsmanager_client.py
+-rw-r--r--   0        0        0     2442 2023-04-19 12:29:23.993056 prowler_cloud-3.4.1/prowler/providers/aws/services/secretsmanager/secretsmanager_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.993113 prowler_cloud-3.4.1/prowler/providers/aws/services/securityhub/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-19 12:29:23.993184 prowler_cloud-3.4.1/prowler/providers/aws/services/securityhub/securityhub_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.993254 prowler_cloud-3.4.1/prowler/providers/aws/services/securityhub/securityhub_enabled/__init__.py
+-rw-r--r--   0        0        0     1315 2023-04-19 12:29:23.993329 prowler_cloud-3.4.1/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.metadata.json
+-rw-r--r--   0        0        0     1296 2023-04-19 12:29:23.993393 prowler_cloud-3.4.1/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.py
+-rw-r--r--   0        0        0     4490 2023-04-19 12:29:23.993473 prowler_cloud-3.4.1/prowler/providers/aws/services/securityhub/securityhub_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.993540 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.993616 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/__init__.py
+-rw-r--r--   0        0        0     1051 2023-04-19 12:29:23.993699 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.metadata.json
+-rw-r--r--   0        0        0     1259 2023-04-19 12:29:23.993773 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.993837 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/__init__.py
+-rw-r--r--   0        0        0     1045 2023-04-19 12:29:23.993917 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.metadata.json
+-rw-r--r--   0        0        0     1267 2023-04-19 12:29:23.993973 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.994037 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/__init__.py
+-rw-r--r--   0        0        0     1041 2023-04-19 12:29:23.994115 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.metadata.json
+-rw-r--r--   0        0        0     1316 2023-04-19 12:29:23.994182 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.994249 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/__init__.py
+-rw-r--r--   0        0        0     1021 2023-04-19 12:29:23.994335 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.metadata.json
+-rw-r--r--   0        0        0     1271 2023-04-19 12:29:23.994405 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.994473 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/__init__.py
+-rw-r--r--   0        0        0     1095 2023-04-19 12:29:23.994548 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.metadata.json
+-rw-r--r--   0        0        0     1353 2023-04-19 12:29:23.994604 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.994667 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/__init__.py
+-rw-r--r--   0        0        0     1020 2023-04-19 12:29:23.994734 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.metadata.json
+-rw-r--r--   0        0        0     1275 2023-04-19 12:29:23.994798 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.py
+-rw-r--r--   0        0        0      195 2023-04-19 12:29:23.994856 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_client.py
+-rw-r--r--   0        0        0     2527 2023-04-19 12:29:23.994929 prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.994989 prowler_cloud-3.4.1/prowler/providers/aws/services/sns/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:23.995057 prowler_cloud-3.4.1/prowler/providers/aws/services/sns/sns_client.py
+-rw-r--r--   0        0        0     3814 2023-04-19 12:29:23.995137 prowler_cloud-3.4.1/prowler/providers/aws/services/sns/sns_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.995195 prowler_cloud-3.4.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/__init__.py
+-rw-r--r--   0        0        0     1283 2023-04-19 12:29:23.995275 prowler_cloud-3.4.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.metadata.json
+-rw-r--r--   0        0        0      841 2023-04-19 12:29:23.995345 prowler_cloud-3.4.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.995410 prowler_cloud-3.4.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1340 2023-04-19 12:29:23.995514 prowler_cloud-3.4.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1921 2023-04-19 12:29:23.995571 prowler_cloud-3.4.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.995633 prowler_cloud-3.4.1/prowler/providers/aws/services/sqs/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:23.995710 prowler_cloud-3.4.1/prowler/providers/aws/services/sqs/sqs_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.995775 prowler_cloud-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1396 2023-04-19 12:29:23.995846 prowler_cloud-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1933 2023-04-19 12:29:23.995899 prowler_cloud-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.995957 prowler_cloud-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1479 2023-04-19 12:29:23.996042 prowler_cloud-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      939 2023-04-19 12:29:23.996103 prowler_cloud-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.py
+-rw-r--r--   0        0        0     4137 2023-04-19 12:29:23.996159 prowler_cloud-3.4.1/prowler/providers/aws/services/sqs/sqs_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.996219 prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:23.996281 prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.996339 prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_document_secrets/__init__.py
+-rw-r--r--   0        0        0     1225 2023-04-19 12:29:23.996410 prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.metadata.json
+-rw-r--r--   0        0        0     1974 2023-04-19 12:29:23.996483 prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.996550 prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/__init__.py
+-rw-r--r--   0        0        0     1142 2023-04-19 12:29:23.996637 prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.metadata.json
+-rw-r--r--   0        0        0      884 2023-04-19 12:29:23.996701 prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.996767 prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/__init__.py
+-rw-r--r--   0        0        0     1557 2023-04-19 12:29:23.996859 prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.metadata.json
+-rw-r--r--   0        0        0      993 2023-04-19 12:29:23.996922 prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.py
+-rw-r--r--   0        0        0     7622 2023-04-19 12:29:23.997006 prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.997076 prowler_cloud-3.4.1/prowler/providers/aws/services/ssmincidents/__init__.py
+-rw-r--r--   0        0        0      234 2023-04-19 12:29:23.997207 prowler_cloud-3.4.1/prowler/providers/aws/services/ssmincidents/ssmincidents_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.997283 prowler_cloud-3.4.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/__init__.py
+-rw-r--r--   0        0        0     1073 2023-04-19 12:29:23.997398 prowler_cloud-3.4.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.metadata.json
+-rw-r--r--   0        0        0     1396 2023-04-19 12:29:23.997661 prowler_cloud-3.4.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.py
+-rw-r--r--   0        0        0     6747 2023-04-19 12:29:23.997948 prowler_cloud-3.4.1/prowler/providers/aws/services/ssmincidents/ssmincidents_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.998014 prowler_cloud-3.4.1/prowler/providers/aws/services/trustedadvisor/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-19 12:29:23.998077 prowler_cloud-3.4.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.998144 prowler_cloud-3.4.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/__init__.py
+-rw-r--r--   0        0        0     1132 2023-04-19 12:29:23.998228 prowler_cloud-3.4.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.metadata.json
+-rw-r--r--   0        0        0     1272 2023-04-19 12:29:23.998296 prowler_cloud-3.4.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.py
+-rw-r--r--   0        0        0     2972 2023-04-19 12:29:23.998367 prowler_cloud-3.4.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.998427 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:23.998500 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.998559 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_different_regions/__init__.py
+-rw-r--r--   0        0        0      860 2023-04-19 12:29:23.998681 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.metadata.json
+-rw-r--r--   0        0        0     1070 2023-04-19 12:29:23.998778 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.998838 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/__init__.py
+-rw-r--r--   0        0        0     1094 2023-04-19 12:29:23.998922 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.metadata.json
+-rw-r--r--   0        0        0     3142 2023-04-19 12:29:23.998993 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.999058 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/__init__.py
+-rw-r--r--   0        0        0     1173 2023-04-19 12:29:23.999134 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.metadata.json
+-rw-r--r--   0        0        0     2056 2023-04-19 12:29:23.999201 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.999264 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/__init__.py
+-rw-r--r--   0        0        0     1214 2023-04-19 12:29:23.999341 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.metadata.json
+-rw-r--r--   0        0        0      822 2023-04-19 12:29:23.999398 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.999459 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/__init__.py
+-rw-r--r--   0        0        0     1294 2023-04-19 12:29:23.999536 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.metadata.json
+-rw-r--r--   0        0        0     1496 2023-04-19 12:29:23.999598 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.py
+-rw-r--r--   0        0        0    15315 2023-04-19 12:29:23.999724 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:23.999799 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/__init__.py
+-rw-r--r--   0        0        0      913 2023-04-19 12:29:23.999916 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.metadata.json
+-rw-r--r--   0        0        0     1276 2023-04-19 12:29:24.000149 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.000210 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/__init__.py
+-rw-r--r--   0        0        0      900 2023-04-19 12:29:24.000322 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.metadata.json
+-rw-r--r--   0        0        0     1432 2023-04-19 12:29:24.000414 prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.000473 prowler_cloud-3.4.1/prowler/providers/aws/services/waf/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:24.000539 prowler_cloud-3.4.1/prowler/providers/aws/services/waf/waf_client.py
+-rw-r--r--   0        0        0     2645 2023-04-19 12:29:24.000622 prowler_cloud-3.4.1/prowler/providers/aws/services/waf/waf_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.000680 prowler_cloud-3.4.1/prowler/providers/aws/services/wafv2/__init__.py
+-rw-r--r--   0        0        0      190 2023-04-19 12:29:24.000748 prowler_cloud-3.4.1/prowler/providers/aws/services/wafv2/wafv2_client.py
+-rw-r--r--   0        0        0     2724 2023-04-19 12:29:24.000842 prowler_cloud-3.4.1/prowler/providers/aws/services/wafv2/wafv2_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.000903 prowler_cloud-3.4.1/prowler/providers/aws/services/workspaces/__init__.py
+-rw-r--r--   0        0        0      215 2023-04-19 12:29:24.000979 prowler_cloud-3.4.1/prowler/providers/aws/services/workspaces/workspaces_client.py
+-rw-r--r--   0        0        0     3457 2023-04-19 12:29:24.001045 prowler_cloud-3.4.1/prowler/providers/aws/services/workspaces/workspaces_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.001108 prowler_cloud-3.4.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     2073 2023-04-19 12:29:24.001196 prowler_cloud-3.4.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1586 2023-04-19 12:29:24.001258 prowler_cloud-3.4.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.001325 prowler_cloud-3.4.1/prowler/providers/azure/__init__.py
+-rw-r--r--   0        0        0     8032 2023-04-19 12:29:24.001448 prowler_cloud-3.4.1/prowler/providers/azure/azure_provider.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.001546 prowler_cloud-3.4.1/prowler/providers/azure/lib/audit_info/__init__.py
+-rw-r--r--   0        0        0      258 2023-04-19 12:29:24.001624 prowler_cloud-3.4.1/prowler/providers/azure/lib/audit_info/audit_info.py
+-rw-r--r--   0        0        0      796 2023-04-19 12:29:24.001856 prowler_cloud-3.4.1/prowler/providers/azure/lib/audit_info/models.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.001965 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/__init__.py
+-rw-r--r--   0        0        0      205 2023-04-19 12:29:24.002041 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.002107 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/__init__.py
+-rw-r--r--   0        0        0     1496 2023-04-19 12:29:24.002201 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.metadata.json
+-rw-r--r--   0        0        0     1182 2023-04-19 12:29:24.002300 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.002370 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/__init__.py
+-rw-r--r--   0        0        0      926 2023-04-19 12:29:24.002447 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.metadata.json
+-rw-r--r--   0        0        0     1121 2023-04-19 12:29:24.002545 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.002609 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/__init__.py
+-rw-r--r--   0        0        0     1654 2023-04-19 12:29:24.002689 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.metadata.json
+-rw-r--r--   0        0        0     1210 2023-04-19 12:29:24.002792 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.002856 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/__init__.py
+-rw-r--r--   0        0        0     1561 2023-04-19 12:29:24.002928 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.metadata.json
+-rw-r--r--   0        0        0     1181 2023-04-19 12:29:24.003026 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.003101 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/__init__.py
+-rw-r--r--   0        0        0     1306 2023-04-19 12:29:24.003180 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.metadata.json
+-rw-r--r--   0        0        0     1163 2023-04-19 12:29:24.003285 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.003354 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/__init__.py
+-rw-r--r--   0        0        0      906 2023-04-19 12:29:24.003441 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.metadata.json
+-rw-r--r--   0        0        0     1638 2023-04-19 12:29:24.003543 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.003612 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/__init__.py
+-rw-r--r--   0        0        0     1254 2023-04-19 12:29:24.003699 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.metadata.json
+-rw-r--r--   0        0        0     1122 2023-04-19 12:29:24.003798 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.003875 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/__init__.py
+-rw-r--r--   0        0        0     1590 2023-04-19 12:29:24.003965 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.metadata.json
+-rw-r--r--   0        0        0     1163 2023-04-19 12:29:24.004069 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.004143 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/__init__.py
+-rw-r--r--   0        0        0     1187 2023-04-19 12:29:24.004227 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.metadata.json
+-rw-r--r--   0        0        0     1346 2023-04-19 12:29:24.004336 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.004406 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/__init__.py
+-rw-r--r--   0        0        0     1509 2023-04-19 12:29:24.004481 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.metadata.json
+-rw-r--r--   0        0        0     1170 2023-04-19 12:29:24.004577 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.004642 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/__init__.py
+-rw-r--r--   0        0        0     1751 2023-04-19 12:29:24.004717 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.metadata.json
+-rw-r--r--   0        0        0     1227 2023-04-19 12:29:24.004839 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.004910 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/__init__.py
+-rw-r--r--   0        0        0     1693 2023-04-19 12:29:24.005006 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.metadata.json
+-rw-r--r--   0        0        0     1202 2023-04-19 12:29:24.005103 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.py
+-rw-r--r--   0        0        0     2326 2023-04-19 12:29:24.005198 prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.005261 prowler_cloud-3.4.1/prowler/providers/azure/services/iam/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-19 12:29:24.005325 prowler_cloud-3.4.1/prowler/providers/azure/services/iam/iam_client.py
+-rw-r--r--   0        0        0     2696 2023-04-19 12:29:24.005421 prowler_cloud-3.4.1/prowler/providers/azure/services/iam/iam_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.005484 prowler_cloud-3.4.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/__init__.py
+-rw-r--r--   0        0        0      996 2023-04-19 12:29:24.005565 prowler_cloud-3.4.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.metadata.json
+-rw-r--r--   0        0        0     1330 2023-04-19 12:29:24.005639 prowler_cloud-3.4.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.005701 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.005772 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/__init__.py
+-rw-r--r--   0        0        0     1470 2023-04-19 12:29:24.005850 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.metadata.json
+-rw-r--r--   0        0        0     1166 2023-04-19 12:29:24.005926 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.py
+-rw-r--r--   0        0        0      200 2023-04-19 12:29:24.005980 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.006041 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/__init__.py
+-rw-r--r--   0        0        0     1354 2023-04-19 12:29:24.006117 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.metadata.json
+-rw-r--r--   0        0        0     1179 2023-04-19 12:29:24.006185 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.006249 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1765 2023-04-19 12:29:24.006334 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1265 2023-04-19 12:29:24.006399 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.006465 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/__init__.py
+-rw-r--r--   0        0        0     1399 2023-04-19 12:29:24.006543 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.metadata.json
+-rw-r--r--   0        0        0     1156 2023-04-19 12:29:24.006608 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.006669 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/__init__.py
+-rw-r--r--   0        0        0     1246 2023-04-19 12:29:24.006748 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.metadata.json
+-rw-r--r--   0        0        0     1151 2023-04-19 12:29:24.006809 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.006877 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1093 2023-04-19 12:29:24.006957 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1169 2023-04-19 12:29:24.007018 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.007076 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1272 2023-04-19 12:29:24.007155 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1166 2023-04-19 12:29:24.007210 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.py
+-rw-r--r--   0        0        0     3651 2023-04-19 12:29:24.007316 prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.007373 prowler_cloud-3.4.1/prowler/providers/common/__init__.py
+-rw-r--r--   0        0        0     1212 2023-04-19 12:29:24.007448 prowler_cloud-3.4.1/prowler/providers/common/allowlist.py
+-rw-r--r--   0        0        0    17566 2023-04-19 12:29:24.007922 prowler_cloud-3.4.1/prowler/providers/common/audit_info.py
+-rw-r--r--   0        0        0      251 2023-04-19 12:29:24.008002 prowler_cloud-3.4.1/prowler/providers/common/models.py
+-rw-r--r--   0        0        0     4693 2023-04-19 12:29:24.008267 prowler_cloud-3.4.1/prowler/providers/common/outputs.py
+-rw-r--r--   0        0        0      885 2023-04-19 12:29:24.008368 prowler_cloud-3.4.1/prowler/providers/common/quick_inventory.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.008430 prowler_cloud-3.4.1/prowler/providers/gcp/__init__.py
+-rw-r--r--   0        0        0     1695 2023-04-19 12:29:24.008547 prowler_cloud-3.4.1/prowler/providers/gcp/gcp_provider.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.008639 prowler_cloud-3.4.1/prowler/providers/gcp/lib/audit_info/__init__.py
+-rw-r--r--   0        0        0      201 2023-04-19 12:29:24.008706 prowler_cloud-3.4.1/prowler/providers/gcp/lib/audit_info/audit_info.py
+-rw-r--r--   0        0        0      522 2023-04-19 12:29:24.008769 prowler_cloud-3.4.1/prowler/providers/gcp/lib/audit_info/models.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.008869 prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/__init__.py
+-rw-r--r--   0        0        0      197 2023-04-19 12:29:24.008942 prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.009000 prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/__init__.py
+-rw-r--r--   0        0        0     1445 2023-04-19 12:29:24.009076 prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.metadata.json
+-rw-r--r--   0        0        0      996 2023-04-19 12:29:24.009145 prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.009202 prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/__init__.py
+-rw-r--r--   0        0        0     1314 2023-04-19 12:29:24.009314 prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.metadata.json
+-rw-r--r--   0        0        0      948 2023-04-19 12:29:24.009408 prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.py
+-rw-r--r--   0        0        0     4116 2023-04-19 12:29:24.009507 prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.009566 prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/__init__.py
+-rw-r--r--   0        0        0     1373 2023-04-19 12:29:24.009671 prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.metadata.json
+-rw-r--r--   0        0        0      974 2023-04-19 12:29:24.009766 prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.009835 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudresourcemanager/__init__.py
+-rw-r--r--   0        0        0      266 2023-04-19 12:29:24.009910 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_client.py
+-rw-r--r--   0        0        0     1262 2023-04-19 12:29:24.009969 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.010050 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/__init__.py
+-rw-r--r--   0        0        0      197 2023-04-19 12:29:24.010112 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.010172 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/__init__.py
+-rw-r--r--   0        0        0     1408 2023-04-19 12:29:24.010282 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.metadata.json
+-rw-r--r--   0        0        0     1011 2023-04-19 12:29:24.010380 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.010443 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/__init__.py
+-rw-r--r--   0        0        0     1359 2023-04-19 12:29:24.010556 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.metadata.json
+-rw-r--r--   0        0        0     1182 2023-04-19 12:29:24.010649 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.010712 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/__init__.py
+-rw-r--r--   0        0        0     1216 2023-04-19 12:29:24.011215 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.metadata.json
+-rw-r--r--   0        0        0     1203 2023-04-19 12:29:24.011559 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.011633 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/__init__.py
+-rw-r--r--   0        0        0     2058 2023-04-19 12:29:24.011749 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.metadata.json
+-rw-r--r--   0        0        0     1302 2023-04-19 12:29:24.011849 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.011912 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/__init__.py
+-rw-r--r--   0        0        0     1587 2023-04-19 12:29:24.012026 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.metadata.json
+-rw-r--r--   0        0        0     1207 2023-04-19 12:29:24.012120 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.012183 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/__init__.py
+-rw-r--r--   0        0        0     1447 2023-04-19 12:29:24.012289 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.metadata.json
+-rw-r--r--   0        0        0     1219 2023-04-19 12:29:24.012566 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.012642 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/__init__.py
+-rw-r--r--   0        0        0     1618 2023-04-19 12:29:24.012759 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.metadata.json
+-rw-r--r--   0        0        0     1310 2023-04-19 12:29:24.012938 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.013002 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/__init__.py
+-rw-r--r--   0        0        0     1442 2023-04-19 12:29:24.013111 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.metadata.json
+-rw-r--r--   0        0        0     1323 2023-04-19 12:29:24.013203 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.013261 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/__init__.py
+-rw-r--r--   0        0        0     1955 2023-04-19 12:29:24.013390 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.metadata.json
+-rw-r--r--   0        0        0     1466 2023-04-19 12:29:24.013630 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.013695 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/__init__.py
+-rw-r--r--   0        0        0     1745 2023-04-19 12:29:24.013803 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.metadata.json
+-rw-r--r--   0        0        0     1410 2023-04-19 12:29:24.013897 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.013964 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/__init__.py
+-rw-r--r--   0        0        0     1326 2023-04-19 12:29:24.014087 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.metadata.json
+-rw-r--r--   0        0        0     1368 2023-04-19 12:29:24.014258 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.014331 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/__init__.py
+-rw-r--r--   0        0        0     1151 2023-04-19 12:29:24.014469 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.metadata.json
+-rw-r--r--   0        0        0     1104 2023-04-19 12:29:24.014571 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.014636 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/__init__.py
+-rw-r--r--   0        0        0     1492 2023-04-19 12:29:24.014749 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.metadata.json
+-rw-r--r--   0        0        0     1046 2023-04-19 12:29:24.014844 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.014903 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/__init__.py
+-rw-r--r--   0        0        0     1319 2023-04-19 12:29:24.014985 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.metadata.json
+-rw-r--r--   0        0        0      991 2023-04-19 12:29:24.015046 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.015134 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/__init__.py
+-rw-r--r--   0        0        0     2153 2023-04-19 12:29:24.015262 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.metadata.json
+-rw-r--r--   0        0        0     1350 2023-04-19 12:29:24.015367 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.015435 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/__init__.py
+-rw-r--r--   0        0        0     1702 2023-04-19 12:29:24.015548 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.metadata.json
+-rw-r--r--   0        0        0     1232 2023-04-19 12:29:24.015643 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.015707 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/__init__.py
+-rw-r--r--   0        0        0     1583 2023-04-19 12:29:24.015828 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.metadata.json
+-rw-r--r--   0        0        0     1319 2023-04-19 12:29:24.016131 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.016272 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/__init__.py
+-rw-r--r--   0        0        0     1860 2023-04-19 12:29:24.016436 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.metadata.json
+-rw-r--r--   0        0        0     1201 2023-04-19 12:29:24.016571 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.016651 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/__init__.py
+-rw-r--r--   0        0        0     2002 2023-04-19 12:29:24.016785 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.metadata.json
+-rw-r--r--   0        0        0     1190 2023-04-19 12:29:24.016898 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.016981 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/__init__.py
+-rw-r--r--   0        0        0     2238 2023-04-19 12:29:24.017114 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.metadata.json
+-rw-r--r--   0        0        0     1210 2023-04-19 12:29:24.017227 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.017311 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/__init__.py
+-rw-r--r--   0        0        0     1583 2023-04-19 12:29:24.017749 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.metadata.json
+-rw-r--r--   0        0        0     1179 2023-04-19 12:29:24.017983 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.018063 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/__init__.py
+-rw-r--r--   0        0        0     1428 2023-04-19 12:29:24.018178 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.metadata.json
+-rw-r--r--   0        0        0      977 2023-04-19 12:29:24.018274 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.py
+-rw-r--r--   0        0        0     2467 2023-04-19 12:29:24.018383 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.018443 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudstorage/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.018527 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/__init__.py
+-rw-r--r--   0        0        0     1351 2023-04-19 12:29:24.018636 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.metadata.json
+-rw-r--r--   0        0        0      926 2023-04-19 12:29:24.018724 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.018787 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/__init__.py
+-rw-r--r--   0        0        0     1270 2023-04-19 12:29:24.018893 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.metadata.json
+-rw-r--r--   0        0        0     1067 2023-04-19 12:29:24.018961 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.py
+-rw-r--r--   0        0        0      226 2023-04-19 12:29:24.019016 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_client.py
+-rw-r--r--   0        0        0     2099 2023-04-19 12:29:24.019113 prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.019173 prowler_cloud-3.4.1/prowler/providers/gcp/services/compute/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-19 12:29:24.019237 prowler_cloud-3.4.1/prowler/providers/gcp/services/compute/compute_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.019294 prowler_cloud-3.4.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/__init__.py
+-rw-r--r--   0        0        0     1327 2023-04-19 12:29:24.019382 prowler_cloud-3.4.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.metadata.json
+-rw-r--r--   0        0        0      897 2023-04-19 12:29:24.019443 prowler_cloud-3.4.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.019505 prowler_cloud-3.4.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/__init__.py
+-rw-r--r--   0        0        0     1132 2023-04-19 12:29:24.019597 prowler_cloud-3.4.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.metadata.json
+-rw-r--r--   0        0        0      827 2023-04-19 12:29:24.019661 prowler_cloud-3.4.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.py
+-rw-r--r--   0        0        0     3489 2023-04-19 12:29:24.019722 prowler_cloud-3.4.1/prowler/providers/gcp/services/compute/compute_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.019781 prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-19 12:29:24.019858 prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.019919 prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/__init__.py
+-rw-r--r--   0        0        0     1459 2023-04-19 12:29:24.019998 prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.metadata.json
+-rw-r--r--   0        0        0     1395 2023-04-19 12:29:24.020445 prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.020509 prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/__init__.py
+-rw-r--r--   0        0        0     1363 2023-04-19 12:29:24.020619 prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.metadata.json
+-rw-r--r--   0        0        0     1038 2023-04-19 12:29:24.020846 prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.020931 prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/__init__.py
+-rw-r--r--   0        0        0     1133 2023-04-19 12:29:24.021052 prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.metadata.json
+-rw-r--r--   0        0        0     1317 2023-04-19 12:29:24.021164 prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.py
+-rw-r--r--   0        0        0     3292 2023-04-19 12:29:24.021266 prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.021333 prowler_cloud-3.4.1/prowler/providers/gcp/services/kms/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-19 12:29:24.021401 prowler_cloud-3.4.1/prowler/providers/gcp/services/kms/kms_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.021465 prowler_cloud-3.4.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1195 2023-04-19 12:29:24.021537 prowler_cloud-3.4.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1000 2023-04-19 12:29:24.021594 prowler_cloud-3.4.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.021662 prowler_cloud-3.4.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/__init__.py
+-rw-r--r--   0        0        0     1233 2023-04-19 12:29:24.021737 prowler_cloud-3.4.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.metadata.json
+-rw-r--r--   0        0        0     1135 2023-04-19 12:29:24.021794 prowler_cloud-3.4.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.py
+-rw-r--r--   0        0        0     4837 2023-04-19 12:29:24.021859 prowler_cloud-3.4.1/prowler/providers/gcp/services/kms/kms_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.021915 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-19 12:29:24.021981 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.022046 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1438 2023-04-19 12:29:24.022174 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     1996 2023-04-19 12:29:24.022441 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.022510 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1243 2023-04-19 12:29:24.022758 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     1971 2023-04-19 12:29:24.022856 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.022918 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1239 2023-04-19 12:29:24.023029 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2090 2023-04-19 12:29:24.023132 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.023196 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1590 2023-04-19 12:29:24.023306 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2288 2023-04-19 12:29:24.023447 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.023535 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1212 2023-04-19 12:29:24.023657 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     1955 2023-04-19 12:29:24.023765 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.023843 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1233 2023-04-19 12:29:24.023959 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2086 2023-04-19 12:29:24.024065 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.024131 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1113 2023-04-19 12:29:24.024268 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2188 2023-04-19 12:29:24.024385 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.024464 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1157 2023-04-19 12:29:24.024600 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2019 2023-04-19 12:29:24.024712 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.py
+-rw-r--r--   0        0        0     2577 2023-04-19 12:29:24.024824 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_service.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.024897 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_sink_created/__init__.py
+-rw-r--r--   0        0        0     1235 2023-04-19 12:29:24.024987 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.metadata.json
+-rw-r--r--   0        0        0     1473 2023-04-19 12:29:24.025096 prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:29:24.025173 prowler_cloud-3.4.1/prowler/providers/gcp/services/monitoring/__init__.py
+-rw-r--r--   0        0        0      207 2023-04-19 12:29:24.025294 prowler_cloud-3.4.1/prowler/providers/gcp/services/monitoring/monitoring_client.py
+-rw-r--r--   0        0        0     1893 2023-04-19 12:29:24.025405 prowler_cloud-3.4.1/prowler/providers/gcp/services/monitoring/monitoring_service.py
+-rw-r--r--   0        0        0     2449 2023-04-25 11:50:32.191557 prowler_cloud-3.4.1/pyproject.toml
+-rw-r--r--   0        0        0    47089 1970-01-01 00:00:00.000000 prowler_cloud-3.4.1/setup.py
+-rw-r--r--   0        0        0    15171 1970-01-01 00:00:00.000000 prowler_cloud-3.4.1/PKG-INFO
```

### Comparing `prowler_cloud-3.4.0/LICENSE` & `prowler_cloud-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/README.md` & `prowler_cloud-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/__main__.py` & `prowler_cloud-3.4.1/prowler/__main__.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/aws_audit_manager_control_tower_guardrails_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/aws_audit_manager_control_tower_guardrails_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/aws_foundational_security_best_practices_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/aws_foundational_security_best_practices_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/cis_1.4_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/cis_1.4_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/cis_1.5_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/cis_1.5_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/cisa_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/cisa_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/ens_rd2022_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/ens_rd2022_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/fedramp_low_revision_4_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/fedramp_low_revision_4_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/fedramp_moderate_revision_4_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/fedramp_moderate_revision_4_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/ffiec_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/ffiec_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/gdpr_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/gdpr_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/gxp_21_cfr_part_11_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/gxp_21_cfr_part_11_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/gxp_eu_annex_11_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/gxp_eu_annex_11_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/hipaa_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/hipaa_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/nist_800_171_revision_2_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/nist_800_171_revision_2_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/nist_800_53_revision_4_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/nist_800_53_revision_4_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/nist_800_53_revision_5_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/nist_800_53_revision_5_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/nist_csf_1.1_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/nist_csf_1.1_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/pci_3.2.1_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/pci_3.2.1_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/rbi_cyber_security_framework_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/rbi_cyber_security_framework_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/compliance/aws/soc2_aws.json` & `prowler_cloud-3.4.1/prowler/compliance/aws/soc2_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/config/allowlist.yaml` & `prowler_cloud-3.4.1/prowler/config/allowlist.yaml`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/config/config.py` & `prowler_cloud-3.4.1/prowler/config/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import requests
 import yaml
 
 from prowler.lib.logger import logger
 
 timestamp = datetime.today()
 timestamp_utc = datetime.now(timezone.utc).replace(tzinfo=timezone.utc)
-prowler_version = "3.4.0"
+prowler_version = "3.4.1"
 html_logo_url = "https://github.com/prowler-cloud/prowler/"
 html_logo_img = "https://user-images.githubusercontent.com/3985464/113734260-7ba06900-96fb-11eb-82bc-d4f68a1e2710.png"
 
 orange_color = "\033[38;5;208m"
 banner_color = "\033[1;92m"
 
 # Compliance
@@ -42,27 +42,28 @@
 csv_file_suffix = ".csv"
 json_file_suffix = ".json"
 json_asff_file_suffix = ".asff.json"
 html_file_suffix = ".html"
 config_yaml = f"{pathlib.Path(os.path.dirname(os.path.realpath(__file__)))}/config.yaml"
 
 
-def check_current_version(prowler_version):
+def check_current_version():
     try:
+        prowler_version_string = f"Prowler {prowler_version}"
         release_response = requests.get(
             "https://api.github.com/repos/prowler-cloud/prowler/tags"
         )
         latest_version = release_response.json()[0]["name"]
         if latest_version != prowler_version:
-            return f"(latest is {latest_version}, upgrade for the latest features)"
+            return f"{prowler_version_string} (latest is {latest_version}, upgrade for the latest features)"
         else:
-            return "(it is the latest version, yay!)"
-    except Exception as e:
-        print(e)
-        return ""
+            return f"{prowler_version_string} (it is the latest version, yay!)"
+    except Exception as error:
+        logger.error(f"{error.__class__.__name__}: {error}")
+        return f"{prowler_version_string}"
 
 
 def change_config_var(variable, value):
     try:
         with open(config_yaml) as f:
             doc = yaml.safe_load(f)
```

### Comparing `prowler_cloud-3.4.0/prowler/config/config.yaml` & `prowler_cloud-3.4.1/prowler/config/config.yaml`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/lib/banner.py` & `prowler_cloud-3.4.1/prowler/lib/banner.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/lib/check/check.py` & `prowler_cloud-3.4.1/prowler/lib/check/check.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/lib/check/checks_loader.py` & `prowler_cloud-3.4.1/prowler/lib/check/checks_loader.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/lib/check/compliance.py` & `prowler_cloud-3.4.1/prowler/lib/check/compliance.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/lib/check/compliance_models.py` & `prowler_cloud-3.4.1/prowler/lib/check/compliance_models.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/lib/check/models.py` & `prowler_cloud-3.4.1/prowler/lib/check/models.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/lib/cli/parser.py` & `prowler_cloud-3.4.1/prowler/lib/cli/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import sys
 from argparse import RawTextHelpFormatter
 
 from prowler.config.config import (
     available_compliance_frameworks,
     check_current_version,
     default_output_directory,
-    prowler_version,
 )
 from prowler.providers.aws.aws_provider import get_aws_available_regions
 from prowler.providers.aws.lib.arn.arn import is_valid_arn
 
 
 def arn_type(arn: str) -> bool:
     """arn_type returns a string ARN if it is valid and raises an argparse.ArgumentError if not."""
@@ -32,16 +31,15 @@
 Detailed documentation at https://docs.prowler.cloud
 """,
         )
         # Default
         self.parser.add_argument(
             "-v",
             "--version",
-            action="version",
-            version=f"Prowler {prowler_version} {check_current_version(prowler_version)}",
+            action="store_true",
             help="show Prowler version",
         )
         # Common arguments parser
         self.common_providers_parser = argparse.ArgumentParser(add_help=False)
 
         # Providers Parser
         self.subparsers = self.parser.add_subparsers(
@@ -64,14 +62,18 @@
         """
         parse is a wrapper to call parse_args() and do some validation
         """
         # We can override sys.argv
         if args:
             sys.argv = args
 
+        if len(sys.argv) == 2 and sys.argv[1] in ("-v", "--version"):
+            print(check_current_version())
+            sys.exit(0)
+
         # Set AWS as the default provider if no provider is supplied
         if len(sys.argv) == 1:
             sys.argv = self.__set_default_provider__(sys.argv)
 
         # Help and Version flags cannot set a default provider
         if (
             len(sys.argv) >= 2
```

### Comparing `prowler_cloud-3.4.0/prowler/lib/logger.py` & `prowler_cloud-3.4.1/prowler/lib/logger.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/lib/outputs/compliance.py` & `prowler_cloud-3.4.1/prowler/lib/outputs/compliance.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/lib/outputs/file_descriptors.py` & `prowler_cloud-3.4.1/prowler/lib/outputs/file_descriptors.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/lib/outputs/html.py` & `prowler_cloud-3.4.1/prowler/lib/outputs/html.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/lib/outputs/json.py` & `prowler_cloud-3.4.1/prowler/lib/outputs/json.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/lib/outputs/models.py` & `prowler_cloud-3.4.1/prowler/lib/outputs/models.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/lib/outputs/outputs.py` & `prowler_cloud-3.4.1/prowler/lib/outputs/outputs.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/lib/outputs/summary_table.py` & `prowler_cloud-3.4.1/prowler/lib/outputs/summary_table.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/lib/scan_filters/scan_filters.py` & `prowler_cloud-3.4.1/prowler/lib/scan_filters/scan_filters.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/lib/utils/utils.py` & `prowler_cloud-3.4.1/prowler/lib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/aws_provider.py` & `prowler_cloud-3.4.1/prowler/providers/aws/aws_provider.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/aws_regions_by_service.json` & `prowler_cloud-3.4.1/prowler/providers/aws/aws_regions_by_service.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999467428598927%*

 * *Differences: {"'services'": "{'backup': {'regions': {'aws': {insert: [(10, 'ap-southeast-4')]}}}, "*

 * *               "'controltower': {'regions': {'aws': {insert: [(0, 'af-south-1'), (1, 'ap-east-1'), "*

 * *               "(4, 'ap-northeast-3'), (8, 'ap-southeast-3'), (12, 'eu-south-1'), (16, "*

 * *               "'me-south-1'), (20, 'us-west-1')]}}}, 'iotdevicedefender': {'regions': {'aws': "*

 * *               "{insert: [(12, 'me-central-1')]}}}, 'iotsecuretunneling': {'regions': {'aws': "*

 * *               "{insert: [(12, 'me-central […]*

```diff
@@ -989,14 +989,15 @@
                     "ap-northeast-2",
                     "ap-northeast-3",
                     "ap-south-1",
                     "ap-south-2",
                     "ap-southeast-1",
                     "ap-southeast-2",
                     "ap-southeast-3",
+                    "ap-southeast-4",
                     "ca-central-1",
                     "eu-central-1",
                     "eu-central-2",
                     "eu-north-1",
                     "eu-south-1",
                     "eu-south-2",
                     "eu-west-1",
@@ -2286,28 +2287,35 @@
                     "us-gov-west-1"
                 ]
             }
         },
         "controltower": {
             "regions": {
                 "aws": [
+                    "af-south-1",
+                    "ap-east-1",
                     "ap-northeast-1",
                     "ap-northeast-2",
+                    "ap-northeast-3",
                     "ap-south-1",
                     "ap-southeast-1",
                     "ap-southeast-2",
+                    "ap-southeast-3",
                     "ca-central-1",
                     "eu-central-1",
                     "eu-north-1",
+                    "eu-south-1",
                     "eu-west-1",
                     "eu-west-2",
                     "eu-west-3",
+                    "me-south-1",
                     "sa-east-1",
                     "us-east-1",
                     "us-east-2",
+                    "us-west-1",
                     "us-west-2"
                 ],
                 "aws-cn": [],
                 "aws-us-gov": [
                     "us-gov-east-1",
                     "us-gov-west-1"
                 ]
@@ -4682,14 +4690,15 @@
                     "ap-southeast-2",
                     "ca-central-1",
                     "eu-central-1",
                     "eu-north-1",
                     "eu-west-1",
                     "eu-west-2",
                     "eu-west-3",
+                    "me-central-1",
                     "me-south-1",
                     "us-east-1",
                     "us-east-2",
                     "us-west-1",
                     "us-west-2"
                 ],
                 "aws-cn": [
@@ -4825,14 +4834,15 @@
                     "ap-southeast-2",
                     "ca-central-1",
                     "eu-central-1",
                     "eu-north-1",
                     "eu-west-1",
                     "eu-west-2",
                     "eu-west-3",
+                    "me-central-1",
                     "me-south-1",
                     "sa-east-1",
                     "us-east-1",
                     "us-east-2",
                     "us-west-1",
                     "us-west-2"
                 ],
@@ -6101,22 +6111,29 @@
                 "aws-us-gov": []
             }
         },
         "migration-hub-refactor-spaces": {
             "regions": {
                 "aws": [
                     "ap-northeast-1",
+                    "ap-northeast-2",
+                    "ap-northeast-3",
+                    "ap-south-1",
                     "ap-southeast-1",
                     "ap-southeast-2",
+                    "ca-central-1",
                     "eu-central-1",
                     "eu-north-1",
                     "eu-west-1",
                     "eu-west-2",
+                    "eu-west-3",
+                    "sa-east-1",
                     "us-east-1",
                     "us-east-2",
+                    "us-west-1",
                     "us-west-2"
                 ],
                 "aws-cn": [],
                 "aws-us-gov": []
             }
         },
         "migrationhuborchestrator": {
@@ -7784,14 +7801,15 @@
                     "ap-northeast-1",
                     "ap-northeast-2",
                     "ap-northeast-3",
                     "ap-south-1",
                     "ap-southeast-1",
                     "ap-southeast-2",
                     "ap-southeast-3",
+                    "ap-southeast-4",
                     "ca-central-1",
                     "eu-central-1",
                     "eu-central-2",
                     "eu-north-1",
                     "eu-south-1",
                     "eu-south-2",
                     "eu-west-1",
```

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/lib/allowlist/allowlist.py` & `prowler_cloud-3.4.1/prowler/providers/aws/lib/allowlist/allowlist.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/lib/arn/arn.py` & `prowler_cloud-3.4.1/prowler/providers/aws/lib/arn/arn.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/lib/arn/error.py` & `prowler_cloud-3.4.1/prowler/providers/aws/lib/arn/error.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/lib/audit_info/audit_info.py` & `prowler_cloud-3.4.1/prowler/providers/aws/lib/audit_info/audit_info.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/lib/audit_info/models.py` & `prowler_cloud-3.4.1/prowler/providers/aws/lib/audit_info/models.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/lib/quick_inventory/quick_inventory.py` & `prowler_cloud-3.4.1/prowler/providers/aws/lib/quick_inventory/quick_inventory.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/lib/resource_api_tagging/resource_api_tagging.py` & `prowler_cloud-3.4.1/prowler/providers/aws/lib/resource_api_tagging/resource_api_tagging.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/lib/security_hub/security_hub.py` & `prowler_cloud-3.4.1/prowler/providers/aws/lib/security_hub/security_hub.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/account/account_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/account/account_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/acm/acm_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/acm/acm_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/appstream/appstream_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/appstream/appstream_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/autoscaling/autoscaling_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/awslambda/awslambda_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/awslambda/awslambda_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudformation/cloudformation_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudfront/cloudfront_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudtrail/cloudtrail_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,15 +9,21 @@
         specific_retention_days = get_config_var("log_group_retention_days")
         for log_group in logs_client.log_groups:
             report = Check_Report_AWS(self.metadata())
             report.region = log_group.region
             report.resource_id = log_group.name
             report.resource_arn = log_group.arn
             report.resource_tags = log_group.tags
-            if log_group.retention_days < specific_retention_days:
+            if (
+                log_group.never_expire is False
+                and log_group.retention_days < specific_retention_days
+            ):
                 report.status = "FAIL"
                 report.status_extended = f"Log Group {log_group.name} has less than {specific_retention_days} days retention period ({log_group.retention_days} days)."
             else:
                 report.status = "PASS"
-                report.status_extended = f"Log Group {log_group.name} comply with {specific_retention_days} days retention period since it has {log_group.retention_days} days."
+                if log_group.never_expire is True:
+                    report.status_extended = f"Log Group {log_group.name} comply with {specific_retention_days} days retention period since it never expires."
+                else:
+                    report.status_extended = f"Log Group {log_group.name} comply with {specific_retention_days} days retention period since it has {log_group.retention_days} days."
             findings.append(report)
         return findings
```

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/cloudwatch/cloudwatch_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,25 +148,26 @@
                 "describe_log_groups"
             )
             for page in describe_log_groups_paginator.paginate():
                 for log_group in page["logGroups"]:
                     if not self.audit_resources or (
                         is_resource_filtered(log_group["arn"], self.audit_resources)
                     ):
-                        kms = None
-                        retention_days = 0
-                        if "kmsKeyId" in log_group:
-                            kms = log_group["kmsKeyId"]
-                        if "retentionInDays" in log_group:
-                            retention_days = log_group["retentionInDays"]
+                        never_expire = False
+                        kms = log_group.get("kmsKeyId")
+                        retention_days = log_group.get("retentionInDays")
+                        if not retention_days:
+                            never_expire = True
+                            retention_days = 9999
                         self.log_groups.append(
                             LogGroup(
                                 arn=log_group["arn"],
                                 name=log_group["logGroupName"],
                                 retention_days=retention_days,
+                                never_expire=never_expire,
                                 kms_id=kms,
                                 region=regional_client.region,
                             )
                         )
         except Exception as error:
             logger.error(
                 f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
@@ -205,16 +206,16 @@
         )
 
     def __list_tags_for_resource__(self):
         logger.info("CloudWatch Logs - List Tags...")
         try:
             for log_group in self.log_groups:
                 regional_client = self.regional_clients[log_group.region]
-                response = regional_client.list_tags_for_resource(
-                    resourceArn=log_group.arn.replace(":*", "")  # Remove the tailing :*
+                response = regional_client.list_tags_log_group(
+                    logGroupName=log_group.name
                 )["tags"]
                 log_group.tags = [response]
         except Exception as error:
             logger.error(
                 f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
 
@@ -236,14 +237,15 @@
     region: str
 
 
 class LogGroup(BaseModel):
     arn: str
     name: str
     retention_days: int
+    never_expire: bool
     kms_id: Optional[str]
     region: str
     log_streams: dict[
         str, list[str]
     ] = {}  # Log stream name as the key, array of events as the value
     tags: Optional[list] = []
```

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/codeartifact/codeartifact_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/codeartifact/codeartifact_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/codebuild/codebuild_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/codebuild/codebuild_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/config/config_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/config/config_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/ec2_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/ec2_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/lib/network_acls.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/lib/network_acls.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ec2/lib/security_groups.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ec2/lib/security_groups.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ecr/ecr_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ecr/ecr_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ecs/ecs_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ecs/ecs_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/efs/efs_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/efs/efs_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/eks/eks_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/eks/eks_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/emr/emr_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/emr/emr_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glacier/glacier_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glacier/glacier_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/globalaccelerator/globalaccelerator_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/globalaccelerator/globalaccelerator_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/glue/glue_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/glue/glue_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/guardduty/guardduty_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/guardduty/guardduty_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from prowler.providers.aws.services.iam.iam_client import iam_client
 
 
 class iam_role_cross_service_confused_deputy_prevention(Check):
     def execute(self) -> Check_Report_AWS:
         findings = []
         for role in iam_client.roles:
-            # This check should only be performed against service roles
-            if role.is_service_role:
+            # This check should only be performed against service roles (avoid Service Linked Roles since the trust relationship cannot be changed)
+            if role.is_service_role and "aws-service-role" not in role.arn:
                 report = Check_Report_AWS(self.metadata())
                 report.region = iam_client.region
                 report.resource_arn = role.arn
                 report.resource_id = role.name
                 report.resource_tags = role.tags
                 report.status = "FAIL"
-                report.status_extended = f"IAM Service Role {role.name} prevents against a cross-service confused deputy attack"
+                report.status_extended = f"IAM Service Role {role.name} does not prevent against a cross-service confused deputy attack"
                 for statement in role.assume_role_policy["Statement"]:
                     if (
                         statement["Effect"] == "Allow"
                         and (
                             "sts:AssumeRole" in statement["Action"]
                             or "sts:*" in statement["Action"]
                             or "*" in statement["Action"]
@@ -55,13 +55,13 @@
                                 in str(
                                     statement["Condition"]["ArnLike"]["aws:SourceArn"]
                                 )
                             )
                         )
                     ):
                         report.status = "PASS"
-                        report.status_extended = f"IAM Service Role {role.name} does not prevent against a cross-service confused deputy attack"
+                        report.status_extended = f"IAM Service Role {role.name} prevents against a cross-service confused deputy attack"
                         break
 
                 findings.append(report)
 
         return findings
```

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/kms/kms_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/kms/kms_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/macie/macie_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/macie/macie_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/organizations/organizations_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/organizations/organizations_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/redshift/redshift_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/redshift/redshift_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/route53/route53_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/route53/route53_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/s3/s3_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/s3/s3_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/secretsmanager/secretsmanager_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/secretsmanager/secretsmanager_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/securityhub/securityhub_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/securityhub/securityhub_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/shield/shield_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/shield/shield_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sns/sns_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sns/sns_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/sqs/sqs_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/sqs/sqs_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ssm/ssm_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ssm/ssm_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/ssmincidents/ssmincidents_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/ssmincidents/ssmincidents_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/waf/waf_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/waf/waf_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/wafv2/wafv2_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/wafv2/wafv2_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/workspaces/workspaces_service.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/workspaces/workspaces_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/azure_provider.py` & `prowler_cloud-3.4.1/prowler/providers/azure/azure_provider.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/lib/audit_info/models.py` & `prowler_cloud-3.4.1/prowler/providers/azure/lib/audit_info/models.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/defender/defender_service.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/defender/defender_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/iam/iam_service.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/iam/iam_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/azure/services/storage/storage_service.py` & `prowler_cloud-3.4.1/prowler/providers/azure/services/storage/storage_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/common/allowlist.py` & `prowler_cloud-3.4.1/prowler/providers/common/allowlist.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/common/audit_info.py` & `prowler_cloud-3.4.1/prowler/providers/common/audit_info.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/common/outputs.py` & `prowler_cloud-3.4.1/prowler/providers/common/outputs.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/common/quick_inventory.py` & `prowler_cloud-3.4.1/prowler/providers/common/quick_inventory.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/gcp_provider.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/gcp_provider.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/lib/audit_info/models.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/lib/audit_info/models.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_service.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_service.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudsql/cloudsql_service.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_service.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/compute/compute_service.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/compute/compute_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/iam/iam_service.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/iam/iam_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/kms/kms_service.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/kms/kms_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_service.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.metadata.json` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/prowler/providers/gcp/services/monitoring/monitoring_service.py` & `prowler_cloud-3.4.1/prowler/providers/gcp/services/monitoring/monitoring_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.4.0/pyproject.toml` & `prowler_cloud-3.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 authors = [ "Toni de la Fuente <toni@blyx.com>",]
 classifiers = [ "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.9", "License :: OSI Approved :: Apache Software License",]
 description = "Prowler is an Open Source security tool to perform Cloud Security best practices assessments, audits, incident response, continuous monitoring, hardening and forensics readiness. It contains more than 240 controls covering CIS, PCI-DSS, ISO27001, GDPR, HIPAA, FFIEC, SOC2, AWS FTR, ENS and custom security frameworks."
 license = "Apache-2.0"
 maintainers = [ "Sergio Garcia <sergio@verica.io>", "Nacho Rivera <nacho@verica.io>", "Pepe Fagoaga <pepe@verica.io>",]
 name = "prowler-cloud"
 readme = "README.md"
-version = "3.4.0"
+version = "3.4.1"
 [[tool.poetry.packages]]
 include = "prowler"
 
 [tool.poetry-version-plugin]
 source = "init"
 
 [tool.poetry.dependencies]
 alive-progress = "3.1.1"
 arnparse = "0.0.2"
 azure-identity = "1.12.0"
 azure-mgmt-authorization = "3.0.0"
-azure-mgmt-security = "4.0.0"
+azure-mgmt-security = "5.0.0"
 azure-mgmt-storage = "21.0.0"
 azure-mgmt-subscription = "3.1.1"
 azure-storage-blob = "12.16.0"
-boto3 = "1.26.105"
+boto3 = "1.26.115"
 botocore = "1.29.115"
 colorama = "0.4.6"
 detect-secrets = "1.4.0"
 google-api-python-client = "2.84.0"
 msgraph-core = "0.2.2"
 pydantic = "1.10.7"
 python = "^3.9"
@@ -68,15 +68,15 @@
 [tool.poetry.group.dev.dependencies]
 bandit = "1.7.5"
 black = "22.12.0"
 coverage = "7.2.3"
 docker = "6.0.1"
 flake8 = "6.0.0"
 freezegun = "1.2.2"
-moto = "4.1.7"
+moto = "4.1.8"
 openapi-spec-validator = "0.5.6"
-pylint = "2.17.2"
-pytest = "7.3.0"
+pylint = "2.17.3"
+pytest = "7.3.1"
 pytest-xdist = "3.2.1"
 safety = "2.3.5"
 sure = "2.0.1"
 vulture = "2.7"
```

### Comparing `prowler_cloud-3.4.0/setup.py` & `prowler_cloud-3.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,19 +433,19 @@
  'prowler.providers.aws.services.ec2.ec2_instance_secrets_user_data': ['fixtures/*']}
 
 install_requires = \
 ['alive-progress==3.1.1',
  'arnparse==0.0.2',
  'azure-identity==1.12.0',
  'azure-mgmt-authorization==3.0.0',
- 'azure-mgmt-security==4.0.0',
+ 'azure-mgmt-security==5.0.0',
  'azure-mgmt-storage==21.0.0',
  'azure-mgmt-subscription==3.1.1',
  'azure-storage-blob==12.16.0',
- 'boto3==1.26.105',
+ 'boto3==1.26.115',
  'botocore==1.29.115',
  'colorama==0.4.6',
  'detect-secrets==1.4.0',
  'google-api-python-client==2.84.0',
  'msgraph-core==0.2.2',
  'pydantic==1.10.7',
  'schema==0.7.5',
@@ -456,15 +456,15 @@
 {'docs': ['mkdocs==1.4.2', 'mkdocs-material==9.1.6']}
 
 entry_points = \
 {'console_scripts': ['prowler = prowler.__main__:prowler']}
 
 setup_kwargs = {
     'name': 'prowler-cloud',
-    'version': '3.4.0',
+    'version': '3.4.1',
     'description': 'Prowler is an Open Source security tool to perform Cloud Security best practices assessments, audits, incident response, continuous monitoring, hardening and forensics readiness. It contains more than 240 controls covering CIS, PCI-DSS, ISO27001, GDPR, HIPAA, FFIEC, SOC2, AWS FTR, ENS and custom security frameworks.',
     'long_description': '<p align="center">\n  <img align="center" src="https://github.com/prowler-cloud/prowler/blob/62c1ce73bbcdd6b9e5ba03dfcae26dfd165defd9/docs/img/prowler-pro-dark.png?raw=True#gh-dark-mode-only" width="150" height="36">\n  <img align="center" src="https://github.com/prowler-cloud/prowler/blob/62c1ce73bbcdd6b9e5ba03dfcae26dfd165defd9/docs/img/prowler-pro-light.png?raw=True#gh-light-mode-only" width="15%" height="15%">\n</p>\n<p align="center">\n  <b><i>See all the things you and your team can do with ProwlerPro at <a href="https://prowler.pro">prowler.pro</a></i></b>\n</p>\n<hr>\n<p align="center">\n  <img src="https://user-images.githubusercontent.com/3985464/113734260-7ba06900-96fb-11eb-82bc-d4f68a1e2710.png" />\n</p>\n<p align="center">\n  <a href="https://join.slack.com/t/prowler-workspace/shared_invite/zt-1hix76xsl-2uq222JIXrC7Q8It~9ZNog"><img alt="Slack Shield" src="https://img.shields.io/badge/slack-prowler-brightgreen.svg?logo=slack"></a>\n  <a href="https://pypi.org/project/prowler-cloud/"><img alt="Python Version" src="https://img.shields.io/pypi/v/prowler.svg"></a>\n  <a href="https://pypi.python.org/pypi/prowler-cloud/"><img alt="Python Version" src="https://img.shields.io/pypi/pyversions/prowler.svg"></a>\n  <a href="https://pypistats.org/packages/prowler"><img alt="PyPI Prowler Downloads" src="https://img.shields.io/pypi/dw/prowler.svg?label=prowler%20downloads"></a>\n  <a href="https://pypistats.org/packages/prowler-cloud"><img alt="PyPI Prowler-Cloud Downloads" src="https://img.shields.io/pypi/dw/prowler-cloud.svg?label=prowler-cloud%20downloads"></a>\n  <a href="https://formulae.brew.sh/formula/prowler#default"><img alt="Brew Prowler Downloads" src="https://img.shields.io/homebrew/installs/dm/prowler?label=brew%20downloads"></a>\n  <a href="https://hub.docker.com/r/toniblyx/prowler"><img alt="Docker Pulls" src="https://img.shields.io/docker/pulls/toniblyx/prowler"></a>\n  <a href="https://hub.docker.com/r/toniblyx/prowler"><img alt="Docker" src="https://img.shields.io/docker/cloud/build/toniblyx/prowler"></a>\n  <a href="https://hub.docker.com/r/toniblyx/prowler"><img alt="Docker" src="https://img.shields.io/docker/image-size/toniblyx/prowler"></a>\n  <a href="https://gallery.ecr.aws/prowler-cloud/prowler"><img width="120" height=19" alt="AWS ECR Gallery" src="https://user-images.githubusercontent.com/3985464/151531396-b6535a68-c907-44eb-95a1-a09508178616.png"></a>\n</p>\n<p align="center">\n  <a href="https://github.com/prowler-cloud/prowler"><img alt="Repo size" src="https://img.shields.io/github/repo-size/prowler-cloud/prowler"></a>\n  <a href="https://github.com/prowler-cloud/prowler/issues"><img alt="Issues" src="https://img.shields.io/github/issues/prowler-cloud/prowler"></a>\n  <a href="https://github.com/prowler-cloud/prowler/releases"><img alt="Version" src="https://img.shields.io/github/v/release/prowler-cloud/prowler?include_prereleases"></a>\n  <a href="https://github.com/prowler-cloud/prowler/releases"><img alt="Version" src="https://img.shields.io/github/release-date/prowler-cloud/prowler"></a>\n  <a href="https://github.com/prowler-cloud/prowler"><img alt="Contributors" src="https://img.shields.io/github/contributors-anon/prowler-cloud/prowler"></a>\n  <a href="https://github.com/prowler-cloud/prowler"><img alt="License" src="https://img.shields.io/github/license/prowler-cloud/prowler"></a>\n  <a href="https://twitter.com/ToniBlyx"><img alt="Twitter" src="https://img.shields.io/twitter/follow/toniblyx?style=social"></a>\n  <a href="https://twitter.com/prowlercloud"><img alt="Twitter" src="https://img.shields.io/twitter/follow/prowlercloud?style=social"></a>\n</p>\n\n# Description\n\n`Prowler` is an Open Source security tool to perform AWS, GCP and Azure security best practices assessments, audits, incident response, continuous monitoring, hardening and forensics readiness.\n\nIt contains hundreds of controls covering CIS, PCI-DSS, ISO27001, GDPR, HIPAA, FFIEC, SOC2, AWS FTR, ENS and custom security frameworks.\n\n# 📖 Documentation\n\nThe full documentation can now be found at [https://docs.prowler.cloud](https://docs.prowler.cloud)\n\n## Looking for Prowler v2 documentation?\nFor Prowler v2 Documentation, please go to https://github.com/prowler-cloud/prowler/tree/2.12.1.\n\n# ⚙️ Install\n\n## Pip package\nProwler is available as a project in [PyPI](https://pypi.org/project/prowler-cloud/), thus can be installed using pip with Python >= 3.9:\n\n```console\npip install prowler\nprowler -v\n```\nMore details at https://docs.prowler.cloud\n\n## Containers\n\nThe available versions of Prowler are the following:\n\n- `latest`: in sync with master branch (bear in mind that it is not a stable version)\n- `<x.y.z>` (release): you can find the releases [here](https://github.com/prowler-cloud/prowler/releases), those are stable releases.\n- `stable`: this tag always point to the latest release.\n\nThe container images are available here:\n\n- [DockerHub](https://hub.docker.com/r/toniblyx/prowler/tags)\n- [AWS Public ECR](https://gallery.ecr.aws/prowler-cloud/prowler)\n\n## From Github\n\nPython >= 3.9 is required with pip and poetry:\n\n```\ngit clone https://github.com/prowler-cloud/prowler\ncd prowler\npoetry shell\npoetry install\npython prowler.py -v\n```\n\n# 📐✏️ High level architecture\n\nYou can run Prowler from your workstation, an EC2 instance, Fargate or any other container, Codebuild, CloudShell and Cloud9.\n\n![Architecture](https://github.com/prowler-cloud/prowler/blob/62c1ce73bbcdd6b9e5ba03dfcae26dfd165defd9/docs/img/architecture.png?raw=True)\n\n# 📝 Requirements\n\nProwler has been written in Python using the [AWS SDK (Boto3)](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html#) and [Azure SDK](https://azure.github.io/azure-sdk-for-python/).\n## AWS\n\nSince Prowler uses AWS Credentials under the hood, you can follow any authentication method as described [here](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html#cli-configure-quickstart-precedence).\nMake sure you have properly configured your AWS-CLI with a valid Access Key and Region or declare AWS variables properly (or instance profile/role):\n\n  ```console\n  aws configure\n  ```\n\n  or\n\n  ```console\n  export AWS_ACCESS_KEY_ID="ASXXXXXXX"\n  export AWS_SECRET_ACCESS_KEY="XXXXXXXXX"\n  export AWS_SESSION_TOKEN="XXXXXXXXX"\n  ```\n\nThose credentials must be associated to a user or role with proper permissions to do all checks. To make sure, add the following AWS managed policies to the user or role being used:\n\n  - arn:aws:iam::aws:policy/SecurityAudit\n  - arn:aws:iam::aws:policy/job-function/ViewOnlyAccess\n\n  > Moreover, some read-only additional permissions are needed for several checks, make sure you attach also the custom policy [prowler-additions-policy.json](https://github.com/prowler-cloud/prowler/blob/master/permissions/prowler-additions-policy.json) to the role you are using.\n\n  > If you want Prowler to send findings to [AWS Security Hub](https://aws.amazon.com/security-hub), make sure you also attach the custom policy [prowler-security-hub.json](https://github.com/prowler-cloud/prowler/blob/master/permissions/prowler-security-hub.json).\n\n## Google Cloud Platform\n\nProwler will follow the same credentials search as [Google authentication libraries](https://cloud.google.com/docs/authentication/application-default-credentials#search_order):\n\n1. [GOOGLE_APPLICATION_CREDENTIALS environment variable](https://cloud.google.com/docs/authentication/application-default-credentials#GAC)\n2. [User credentials set up by using the Google Cloud CLI](https://cloud.google.com/docs/authentication/application-default-credentials#personal)\n3. [The attached service account, returned by the metadata server](https://cloud.google.com/docs/authentication/application-default-credentials#attached-sa)\n\nThose credentials must be associated to a user or service account with proper permissions to do all checks. To make sure, add the following roles to the member associated with the credentials:\n\n  - Viewer\n  - Security Reviewer\n  - Stackdriver Account Viewer\n\n> `prowler` will scan the project associated with the credentials.\n\n  ## Azure\n\n  Prowler for Azure supports the following authentication types:\n\n- Service principal authentication by environment variables (Enterprise Application)\n- Current az cli credentials stored\n- Interactive browser authentication\n- Managed identity authentication\n\n### Service Principal authentication\n\nTo allow Prowler assume the service principal identity to start the scan, it is needed to configure the following environment variables:\n\n```console\nexport AZURE_CLIENT_ID="XXXXXXXXX"\nexport AZURE_TENANT_ID="XXXXXXXXX"\nexport AZURE_CLIENT_SECRET="XXXXXXX"\n```\n\nIf you try to execute Prowler with the `--sp-env-auth` flag and those variables are empty or not exported, the execution is going to fail.\n### AZ CLI / Browser / Managed Identity authentication\n\nThe other three cases do not need additional configuration, `--az-cli-auth` and `--managed-identity-auth` are automated options, `--browser-auth` needs the user to authenticate using the default browser to start the scan.\n\n### Permissions\n\nTo use each one, you need to pass the proper flag to the execution. Prowler for Azure handles two types of permission scopes, which are:\n\n- **Azure Active Directory permissions**: Used to retrieve metadata from the identity assumed by Prowler and future AAD checks (not mandatory to have access to execute the tool)\n- **Subscription scope permissions**: Required to launch the checks against your resources, mandatory to launch the tool.\n\n\n#### Azure Active Directory scope\n\nAzure Active Directory (AAD) permissions required by the tool are the following:\n\n- `Directory.Read.All`\n- `Policy.Read.All`\n\n\n#### Subscriptions scope\n\nRegarding the subscription scope, Prowler by default scans all the subscriptions that is able to list, so it is required to add the following RBAC builtin roles per subscription  to the entity that is going to be assumed by the tool:\n\n- `Security Reader`\n- `Reader`\n\n\n# 💻 Basic Usage\n\nTo run prowler, you will need to specify the provider (e.g aws or azure):\n\n```console\nprowler <provider>\n```\n\n![Prowler Execution](https://github.com/prowler-cloud/prowler/blob/b91b0103ff38e66a915c8a0ed84905a07e4aae1d/docs/img/short-display.png?raw=True)\n\n> Running the `prowler` command without options will use your environment variable credentials.\n\nBy default, prowler will generate a CSV, a JSON and a HTML report, however you can generate JSON-ASFF (only for AWS Security Hub) report with `-M` or `--output-modes`:\n\n```console\nprowler <provider> -M csv json json-asff html\n```\n\nThe html report will be located in the `output` directory as the other files and it will look like:\n\n![Prowler Execution](https://github.com/prowler-cloud/prowler/blob/62c1ce73bbcdd6b9e5ba03dfcae26dfd165defd9/docs/img/html-output.png?raw=True)\n\nYou can use `-l`/`--list-checks` or `--list-services` to list all available checks or services within the provider.\n\n```console\nprowler <provider> --list-checks\nprowler <provider> --list-services\n```\n\nFor executing specific checks or services you can use options `-c`/`--checks` or `-s`/`--services`:\n\n```console\nprowler aws --checks s3_bucket_public_access\nprowler aws --services s3 ec2\n```\n\nAlso, checks and services can be excluded with options `-e`/`--excluded-checks` or `--excluded-services`:\n\n```console\nprowler aws --excluded-checks s3_bucket_public_access\nprowler aws --excluded-services s3 ec2\n```\n\nYou can always use `-h`/`--help` to access to the usage information and all the possible options:\n\n```console\nprowler -h\n```\n\n## Checks Configurations\nSeveral Prowler\'s checks have user configurable variables that can be modified in a common **configuration file**.\nThis file can be found in the following path:\n```\nprowler/config/config.yaml\n```\n\n## AWS\n\nUse a custom AWS profile with `-p`/`--profile` and/or AWS regions which you want to audit with `-f`/`--filter-region`:\n\n```console\nprowler aws --profile custom-profile -f us-east-1 eu-south-2\n```\n> By default, `prowler` will scan all AWS regions.\n\n## Google Cloud Platform\n\nOptionally, you can provide the location of an application credential JSON file with the following argument:\n\n```console\nprowler gcp --credentials-file path\n```\n\n## Azure\n\nWith Azure you need to specify which auth method is going to be used:\n\n```console\nprowler azure [--sp-env-auth, --az-cli-auth, --browser-auth, --managed-identity-auth]\n```\n> By default, `prowler` will scan all Azure subscriptions.\n\n# 🎉 New Features\n\n- Python: we got rid of all bash and it is now all in Python.\n- Faster: huge performance improvements (same account from 2.5 hours to 4 minutes).\n- Developers and community: we have made it easier to contribute with new checks and new compliance frameworks. We also included unit tests.\n- Multi-cloud: in addition to AWS, we have added Azure, we plan to include GCP and OCI soon, let us know if you want to contribute!\n\n# 📃 License\n\nProwler is licensed as Apache License 2.0 as specified in each file. You may obtain a copy of the License at\n<http://www.apache.org/licenses/LICENSE-2.0>\n',
     'author': 'Toni de la Fuente',
     'author_email': 'toni@blyx.com',
     'maintainer': 'Sergio Garcia',
     'maintainer_email': 'sergio@verica.io',
     'url': 'None',
```

### Comparing `prowler_cloud-3.4.0/PKG-INFO` & `prowler_cloud-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prowler-cloud
-Version: 3.4.0
+Version: 3.4.1
 Summary: Prowler is an Open Source security tool to perform Cloud Security best practices assessments, audits, incident response, continuous monitoring, hardening and forensics readiness. It contains more than 240 controls covering CIS, PCI-DSS, ISO27001, GDPR, HIPAA, FFIEC, SOC2, AWS FTR, ENS and custom security frameworks.
 License: Apache-2.0
 Author: Toni de la Fuente
 Author-email: toni@blyx.com
 Maintainer: Sergio Garcia
 Maintainer-email: sergio@verica.io
 Requires-Python: >=3.9,<4.0
@@ -16,19 +16,19 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: docs
 Requires-Dist: alive-progress (==3.1.1)
 Requires-Dist: arnparse (==0.0.2)
 Requires-Dist: azure-identity (==1.12.0)
 Requires-Dist: azure-mgmt-authorization (==3.0.0)
-Requires-Dist: azure-mgmt-security (==4.0.0)
+Requires-Dist: azure-mgmt-security (==5.0.0)
 Requires-Dist: azure-mgmt-storage (==21.0.0)
 Requires-Dist: azure-mgmt-subscription (==3.1.1)
 Requires-Dist: azure-storage-blob (==12.16.0)
-Requires-Dist: boto3 (==1.26.105)
+Requires-Dist: boto3 (==1.26.115)
 Requires-Dist: botocore (==1.29.115)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: detect-secrets (==1.4.0)
 Requires-Dist: google-api-python-client (==2.84.0)
 Requires-Dist: mkdocs (==1.4.2) ; extra == "docs"
 Requires-Dist: mkdocs-material (==9.1.6) ; extra == "docs"
 Requires-Dist: msgraph-core (==0.2.2)
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: prowler-cloud Version: 3.4.0 Summary: Prowler is an
+Metadata-Version: 2.1 Name: prowler-cloud Version: 3.4.1 Summary: Prowler is an
 Open Source security tool to perform Cloud Security best practices assessments,
 audits, incident response, continuous monitoring, hardening and forensics
 readiness. It contains more than 240 controls covering CIS, PCI-DSS, ISO27001,
 GDPR, HIPAA, FFIEC, SOC2, AWS FTR, ENS and custom security frameworks. License:
 Apache-2.0 Author: Toni de la Fuente Author-email: toni@blyx.com Maintainer:
 Sergio Garcia Maintainer-email: sergio@verica.io Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Provides-Extra:
 docs Requires-Dist: alive-progress (==3.1.1) Requires-Dist: arnparse (==0.0.2)
 Requires-Dist: azure-identity (==1.12.0) Requires-Dist: azure-mgmt-
-authorization (==3.0.0) Requires-Dist: azure-mgmt-security (==4.0.0) Requires-
+authorization (==3.0.0) Requires-Dist: azure-mgmt-security (==5.0.0) Requires-
 Dist: azure-mgmt-storage (==21.0.0) Requires-Dist: azure-mgmt-subscription
 (==3.1.1) Requires-Dist: azure-storage-blob (==12.16.0) Requires-Dist: boto3
-(==1.26.105) Requires-Dist: botocore (==1.29.115) Requires-Dist: colorama
+(==1.26.115) Requires-Dist: botocore (==1.29.115) Requires-Dist: colorama
 (==0.4.6) Requires-Dist: detect-secrets (==1.4.0) Requires-Dist: google-api-
 python-client (==2.84.0) Requires-Dist: mkdocs (==1.4.2) ; extra == "docs"
 Requires-Dist: mkdocs-material (==9.1.6) ; extra == "docs" Requires-Dist:
 msgraph-core (==0.2.2) Requires-Dist: pydantic (==1.10.7) Requires-Dist: schema
 (==0.7.5) Requires-Dist: shodan (==1.28.0) Requires-Dist: tabulate (==0.9.0)
 Project-URL: Changelog, https://github.com/prowler-cloud/prowler/releases
 Project-URL: Documentation, https://docs.prowler.cloud Project-URL: Homepage,
```

