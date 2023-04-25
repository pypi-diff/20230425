# Comparing `tmp/splitit-web-python-sdk-2.0.0.tar.gz` & `tmp/splitit-web-python-sdk-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/dylanhuang/Git/konfig-monorepo/customers/splitit/splitit-web-sdks/python/dist/.tmp-17sa4j5m/splitit-web-python-sdk-2.0.0", last modified: Fri Mar 24 08:16:21 2023, max compression
+gzip compressed data, was "/Users/dylanhuang/Git/konfig-monorepo/customers/splitit/splitit-web-sdks/python/dist/.tmp-vb1jd08t/splitit-web-python-sdk-2.1.0", last modified: Tue Apr 25 03:35:48 2023, max compression
```

## Comparing `splitit-web-python-sdk-2.0.0.tar` & `splitit-web-python-sdk-2.1.0.tar`

### file list

```diff
@@ -1,218 +1,220 @@
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1081 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/LICENSE
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7015 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/PKG-INFO
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6660 2023-03-24 08:15:47.000000 splitit-web-python-sdk-2.0.0/README.md
--rw-r--r--   0 dylanhuang   (501) staff       (20)       69 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/setup.cfg
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1311 2023-03-24 08:15:47.000000 splitit-web-python-sdk-2.0.0/setup.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      725 2023-03-24 08:15:47.000000 splitit-web-python-sdk-2.0.0/splitit_client/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    64528 2023-03-24 08:15:47.000000 splitit-web-python-sdk-2.0.0/splitit_client/api_client.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      266 2023-03-24 08:15:47.000000 splitit-web-python-sdk-2.0.0/splitit_client/api_response.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      214 2023-03-24 08:15:47.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3411 2023-03-24 08:15:47.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/path_to_api.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/paths/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      241 2023-03-24 08:15:47.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/paths/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      127 2023-03-24 08:15:47.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/paths/api_installmentplans.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      161 2023-03-24 08:15:47.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/paths/api_installmentplans_check_eligibility.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      144 2023-03-24 08:15:47.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/paths/api_installmentplans_initiate.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      169 2023-03-24 08:15:47.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      185 2023-03-24 08:15:47.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_cancel.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      185 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_refund.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      192 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_updateorder.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      208 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_verifyauthorization.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      137 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/paths/api_installmentplans_search.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      147 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/paths/api_installmentplans_updateorder.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      371 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/tag_to_api.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/tags/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      328 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/tags/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1373 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/apis/tags/installment_plan_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      713 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/client.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    18416 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/configuration.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5627 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/exceptions.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2274 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/exceptions_base.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      348 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4917 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/address_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4940 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/address_data_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7464 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/authorization_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1798 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/card_brand.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5920 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/card_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1617 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/card_type.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3784 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/check_installments_eligibility_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3403 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/error.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5510 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/error_extended.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2944 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/failed_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1234 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/gw_authorization_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4902 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/identifier_contract.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     9157 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/initiate_plan_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3407 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/initiate_redirection_endpoints_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4349 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/installment.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2545 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_cancel_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7394 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_create_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    13396 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_create_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    14840 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_get_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5929 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_initiate_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3122 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_refund_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5653 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_refund_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3467 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_search_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4296 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_update_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4431 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_update_request_by_identifier.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4463 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_update_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1128 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/installment_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3533 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/installments_eligibility_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4098 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/links_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3725 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/links_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3030 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/payment_method_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      868 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/payment_method_type.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5485 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/payment_plan_option_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7973 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/plan_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     8078 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/plan_data_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4322 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/plan_error_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1391 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/plan_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1137 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/purchase_method.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4169 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/redirection_endpoints_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5669 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/refund_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1115 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/refund_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1531 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/refund_strategy.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4292 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/refund_summary.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    14854 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/search_installment_plan_response_item.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1121 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/shipping_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1004 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/shipping_status2.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3920 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/shopper_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1214 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/test_modes.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4432 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/three_ds_redirect_data_v3.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4269 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/update_order_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3910 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/model/verify_authorization_response.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/models/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4222 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/models/__init__.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1223 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/__init__.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      327 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    26605 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_check_eligibility/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      362 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_check_eligibility/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    25085 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_check_eligibility/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_initiate/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      345 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_initiate/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    26556 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_initiate/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      375 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    15681 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      389 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    15735 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      389 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    27691 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      399 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    27711 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      415 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    15871 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_search/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      341 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_search/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    17471 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_search/get.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_updateorder/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      351 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_updateorder/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    25036 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_updateorder/put.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      639 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/request_after_hook.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      640 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/request_before_hook.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    10671 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/rest.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    94410 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/schemas.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3170 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/splitit_client/validation_metadata.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_web_python_sdk.egg-info/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7015 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_web_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dylanhuang   (501) staff       (20)     9476 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_web_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)        1 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_web_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)      139 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_web_python_sdk.egg-info/requires.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)       20 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/splitit_web_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/test/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1693 2023-03-24 08:14:08.000000 splitit-web-python-sdk-2.0.0/test/test_installment_plan_api_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/test/test_models/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      439 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_address_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      460 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_address_data_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      467 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_authorization_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      431 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_card_brand.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      427 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_card_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      427 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_card_type.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      537 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_check_installments_eligibility_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      414 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_error.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      447 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_error_extended.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      451 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_failed_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      480 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_gw_authorization_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      467 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_identifier_contract.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      476 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_initiate_plan_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      529 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_initiate_redirection_endpoints_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      438 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_installment.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      513 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_cancel_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      509 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_create_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      513 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_create_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      501 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_get_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      517 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_initiate_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      509 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_refund_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      513 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_refund_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      513 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_search_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      509 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_update_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      559 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_update_request_by_identifier.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      513 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_update_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      463 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_installment_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      520 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_installments_eligibility_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      431 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_links_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      435 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_links_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      468 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_payment_method_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      464 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_payment_method_type.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      485 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_payment_plan_option_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      427 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_plan_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      448 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_plan_data_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      464 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_plan_error_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      435 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_plan_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      451 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_purchase_method.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      496 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_redirection_endpoints_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      439 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_refund_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      443 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_refund_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      451 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_refund_strategy.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      447 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_refund_summary.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      530 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_search_installment_plan_response_item.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      451 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_shipping_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      455 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_shipping_status2.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      439 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_shopper_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      431 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_test_modes.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      482 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_three_ds_redirect_data_v3.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      468 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_update_order_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      504 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_models/test_verify_authorization_response.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/test/test_paths/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1984 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/__init__.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      591 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_check_eligibility/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_check_eligibility/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      641 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_check_eligibility/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_initiate/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_initiate/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      616 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_initiate/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      648 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number/test_get.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number_cancel/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number_cancel/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      668 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number_cancel/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number_refund/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number_refund/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      676 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number_refund/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number_updateorder/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number_updateorder/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      690 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number_updateorder/test_put.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number_verifyauthorization/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number_verifyauthorization/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      706 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number_verifyauthorization/test_get.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_search/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_search/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      601 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_search/test_get.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:16:21.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_updateorder/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_updateorder/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      624 2023-03-24 08:15:48.000000 splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_updateorder/test_put.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1081 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/LICENSE
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     7565 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/PKG-INFO
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     7205 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/README.md
+-rw-r--r--   0 dylanhuang   (501) staff       (20)       69 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/setup.cfg
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1319 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/setup.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      725 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    64438 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/api_client.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      266 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/api_response.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      214 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3411 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/path_to_api.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      241 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      127 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      161 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_check_eligibility.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      144 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_initiate.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      169 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      185 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_cancel.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      185 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_refund.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      192 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_updateorder.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      208 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_verifyauthorization.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      137 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_search.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      147 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_updateorder.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      371 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/tag_to_api.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/tags/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      328 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/tags/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1333 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/tags/installment_plan_api.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      713 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/client.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    18376 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/configuration.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     5627 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/exceptions.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     2274 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/exceptions_base.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      348 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     4871 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/address_data.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     4894 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/address_data_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     7418 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/authorization_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1752 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/card_brand.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     5874 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/card_data.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1571 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/card_type.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3738 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/check_installments_eligibility_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3357 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/error.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     5464 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/error_extended.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     2898 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/failed_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1188 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/gw_authorization_status.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     4856 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/identifier_contract.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     9111 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/initiate_plan_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3361 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/initiate_redirection_endpoints_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     4303 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     2499 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_cancel_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     7348 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_create_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    13350 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_create_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    14794 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_get_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     6528 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_initiate_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3076 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_refund_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     5607 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_refund_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3421 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_search_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     4250 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_update_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     4385 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_update_request_by_identifier.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     4417 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_update_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1082 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_status.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3487 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installments_eligibility_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     4052 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/links_data.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3679 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/links_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3476 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/payment_method_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      962 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/payment_method_type.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     5439 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/payment_plan_option_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    10239 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/plan_data.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     8734 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/plan_data_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     4276 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/plan_error_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1345 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/plan_status.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1091 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/purchase_method.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     4123 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/redirection_endpoints_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     5623 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/refund_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1069 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/refund_status.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1485 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/refund_strategy.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     4246 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/refund_summary.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    14808 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/search_installment_plan_response_item.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1075 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/shipping_status.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      958 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/shipping_status2.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3874 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/shopper_data.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1168 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/test_modes.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     4386 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/three_ds_redirect_data_v3.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     4223 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/update_order_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3409 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/ux_settings_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3864 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/verify_authorization_response.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/models/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     4289 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/models/__init__.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1223 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/__init__.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      327 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    27024 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans/post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_check_eligibility/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      362 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_check_eligibility/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    25504 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_check_eligibility/post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_initiate/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      345 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_initiate/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    26975 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_initiate/post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      375 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    16100 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      389 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    16154 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      389 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    28110 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      399 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    28130 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      415 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    16290 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_search/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      341 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_search/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    17890 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_search/get.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_updateorder/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      351 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_updateorder/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    25455 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_updateorder/put.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      639 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/request_after_hook.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      640 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/request_before_hook.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    10671 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/rest.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    95047 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/schemas.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3170 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/validation_metadata.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_web_python_sdk.egg-info/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     7565 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_web_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     9561 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_web_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        1 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_web_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      139 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_web_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 dylanhuang   (501) staff       (20)       20 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_web_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     2878 2023-04-25 03:29:08.000000 splitit-web-python-sdk-2.1.0/test/test_installment_plan_api_post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_models/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      439 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_address_data.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      460 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_address_data_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      467 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_authorization_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      431 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_card_brand.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      427 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_card_data.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      427 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_card_type.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      537 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_check_installments_eligibility_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      414 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_error.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      447 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_error_extended.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      451 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_failed_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      480 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_gw_authorization_status.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      467 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_identifier_contract.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      476 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_initiate_plan_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      529 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_initiate_redirection_endpoints_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      438 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      513 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_cancel_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      509 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_create_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      513 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_create_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      501 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_get_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      517 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_initiate_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      509 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_refund_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      513 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_refund_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      513 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_search_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      509 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_update_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      559 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_update_request_by_identifier.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      513 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_update_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      463 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_status.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      520 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installments_eligibility_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      431 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_links_data.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      435 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_links_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      468 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_payment_method_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      464 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_payment_method_type.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      485 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_payment_plan_option_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      427 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_plan_data.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      448 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_plan_data_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      464 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_plan_error_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      435 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_plan_status.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      451 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_purchase_method.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      496 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_redirection_endpoints_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      439 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_refund_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      443 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_refund_status.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      451 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_refund_strategy.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      447 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_refund_summary.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      530 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_search_installment_plan_response_item.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      451 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_shipping_status.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      455 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_shipping_status2.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      439 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_shopper_data.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      431 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_test_modes.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      482 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_three_ds_redirect_data_v3.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      468 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_update_order_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      456 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_ux_settings_model.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      504 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_verify_authorization_response.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1984 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/__init__.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      683 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans/test_post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_check_eligibility/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_check_eligibility/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      733 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_check_eligibility/test_post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_initiate/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_initiate/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      708 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_initiate/test_post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      740 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number/test_get.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_cancel/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_cancel/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      760 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_cancel/test_post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_refund/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_refund/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      768 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_refund/test_post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_updateorder/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_updateorder/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      782 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_updateorder/test_put.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_verifyauthorization/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_verifyauthorization/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      798 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_verifyauthorization/test_get.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_search/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_search/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      693 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_search/test_get.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_updateorder/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_updateorder/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      716 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_updateorder/test_put.py
```

### Comparing `splitit-web-python-sdk-2.0.0/LICENSE` & `splitit-web-python-sdk-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/PKG-INFO` & `splitit-web-python-sdk-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: splitit-web-python-sdk
-Version: 2.0.0
+Version: 2.1.0
 Summary: splitit-web-api-v3
 Home-page: https://github.com/konfig-dev/splitit-web-sdks/tree/main/python
 Author: Konfig
 Author-email: engineering@konfigthis.com
-Keywords: OpenAPI,Konfig,splitit-web-api-v3
+License: MIT
+Keywords: Konfig,splitit-web-api-v3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # splitit-web-python-sdk
 Splitit's Web API
 
 - API version: 1.0.0
-- Package version: 2.0.0
+- Package version: 2.1.0
 
 ## Requirements.
 
 Python >=3.7
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install splitit-web-python-sdk==2.0.0
+pip install splitit-web-python-sdk==2.1.0
 ```
-(you may need to run `pip` with root permission: `sudo pip install splitit-web-python-sdk==2.0.0`)
+(you may need to run `pip` with root permission: `sudo pip install splitit-web-python-sdk==2.1.0`)
 
 Then import the package:
 ```python
 import splitit_client
 ```
 ## Getting Started
 
@@ -47,32 +48,47 @@
     # See configuration.py for a list of all supported configuration parameters.
     host = "https://web-api-v3.sandbox.splitit.com",
 
     # Configure OAuth2 access token for authorization: oauth
     access_token = 'YOUR_ACCESS_TOKEN'
 )
 
-cancel_response = splitit.installment_plan.cancel(
-    path_params = {
-        'installmentPlanNumber': "installmentPlanNumber_example",
-    },
-    header_params = {
-        'X-Splitit-IdempotencyKey': "X-Splitit-IdempotencyKey_example",
-    },
-)
 try:
+    cancel_response = splitit.installment_plan.cancel(
+        path_params = {
+            'installmentPlanNumber': "installmentPlanNumber_example",
+        },
+        header_params = {
+            'X-Splitit-IdempotencyKey': "X-Splitit-IdempotencyKey_example",
+        },
+    )
+    pprint(cancel_response.body)
     pprint(cancel_response.body["installment_plan_number"])
     pprint(cancel_response.headers)
     pprint(cancel_response.status)
+    pprint(cancel_response.round_trip_time)
 except ApiException as e:
-    print("Exception when calling InstallmentPlanCancelResponse.cancel: %s\n" % e)
+    print("Exception when calling InstallmentPlanApi.cancel: %s\n" % e)
     pprint(e.body)
+    if e.status == 401:
+        pprint(e.body["trace_id"])
+        pprint(e.body["error"])
+    if e.status == 500:
+        pprint(e.body["trace_id"])
+        pprint(e.body["error"])
+    if e.status == 403:
+        pprint(e.body["trace_id"])
+        pprint(e.body["error"])
+    if e.status == 404:
+        pprint(e.body["trace_id"])
+        pprint(e.body["error"])
     pprint(e.headers)
     pprint(e.status)
     pprint(e.reason)
+    pprint(e.round_trip_time)
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://web-api-v3.sandbox.splitit.com*
 
 Class | Method | HTTP request | Description
@@ -136,14 +152,15 @@
  - [SearchInstallmentPlanResponseItem](docs/models/SearchInstallmentPlanResponseItem.md)
  - [ShippingStatus](docs/models/ShippingStatus.md)
  - [ShippingStatus2](docs/models/ShippingStatus2.md)
  - [ShopperData](docs/models/ShopperData.md)
  - [TestModes](docs/models/TestModes.md)
  - [ThreeDsRedirectDataV3](docs/models/ThreeDsRedirectDataV3.md)
  - [UpdateOrderRequest](docs/models/UpdateOrderRequest.md)
+ - [UxSettingsModel](docs/models/UxSettingsModel.md)
  - [VerifyAuthorizationResponse](docs/models/VerifyAuthorizationResponse.md)
 
 ## Documentation For Authorization
 
  Authentication schemes defined for the API:
 ## oauth
```

### Comparing `splitit-web-python-sdk-2.0.0/README.md` & `splitit-web-python-sdk-2.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # splitit-web-python-sdk
 Splitit's Web API
 
 - API version: 1.0.0
-- Package version: 2.0.0
+- Package version: 2.1.0
 
 ## Requirements.
 
 Python >=3.7
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install splitit-web-python-sdk==2.0.0
+pip install splitit-web-python-sdk==2.1.0
 ```
-(you may need to run `pip` with root permission: `sudo pip install splitit-web-python-sdk==2.0.0`)
+(you may need to run `pip` with root permission: `sudo pip install splitit-web-python-sdk==2.1.0`)
 
 Then import the package:
 ```python
 import splitit_client
 ```
 ## Getting Started
 
@@ -35,32 +35,47 @@
     # See configuration.py for a list of all supported configuration parameters.
     host = "https://web-api-v3.sandbox.splitit.com",
 
     # Configure OAuth2 access token for authorization: oauth
     access_token = 'YOUR_ACCESS_TOKEN'
 )
 
-cancel_response = splitit.installment_plan.cancel(
-    path_params = {
-        'installmentPlanNumber': "installmentPlanNumber_example",
-    },
-    header_params = {
-        'X-Splitit-IdempotencyKey': "X-Splitit-IdempotencyKey_example",
-    },
-)
 try:
+    cancel_response = splitit.installment_plan.cancel(
+        path_params = {
+            'installmentPlanNumber': "installmentPlanNumber_example",
+        },
+        header_params = {
+            'X-Splitit-IdempotencyKey': "X-Splitit-IdempotencyKey_example",
+        },
+    )
+    pprint(cancel_response.body)
     pprint(cancel_response.body["installment_plan_number"])
     pprint(cancel_response.headers)
     pprint(cancel_response.status)
+    pprint(cancel_response.round_trip_time)
 except ApiException as e:
-    print("Exception when calling InstallmentPlanCancelResponse.cancel: %s\n" % e)
+    print("Exception when calling InstallmentPlanApi.cancel: %s\n" % e)
     pprint(e.body)
+    if e.status == 401:
+        pprint(e.body["trace_id"])
+        pprint(e.body["error"])
+    if e.status == 500:
+        pprint(e.body["trace_id"])
+        pprint(e.body["error"])
+    if e.status == 403:
+        pprint(e.body["trace_id"])
+        pprint(e.body["error"])
+    if e.status == 404:
+        pprint(e.body["trace_id"])
+        pprint(e.body["error"])
     pprint(e.headers)
     pprint(e.status)
     pprint(e.reason)
+    pprint(e.round_trip_time)
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://web-api-v3.sandbox.splitit.com*
 
 Class | Method | HTTP request | Description
@@ -124,14 +139,15 @@
  - [SearchInstallmentPlanResponseItem](docs/models/SearchInstallmentPlanResponseItem.md)
  - [ShippingStatus](docs/models/ShippingStatus.md)
  - [ShippingStatus2](docs/models/ShippingStatus2.md)
  - [ShopperData](docs/models/ShopperData.md)
  - [TestModes](docs/models/TestModes.md)
  - [ThreeDsRedirectDataV3](docs/models/ThreeDsRedirectDataV3.md)
  - [UpdateOrderRequest](docs/models/UpdateOrderRequest.md)
+ - [UxSettingsModel](docs/models/UxSettingsModel.md)
  - [VerifyAuthorizationResponse](docs/models/VerifyAuthorizationResponse.md)
 
 ## Documentation For Authorization
 
  Authentication schemes defined for the API:
 ## oauth
```

### Comparing `splitit-web-python-sdk-2.0.0/setup.py` & `splitit-web-python-sdk-2.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "splitit-web-python-sdk"
-VERSION = "2.0.0"
+VERSION = "2.1.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -37,15 +37,16 @@
 setup(
     name=NAME,
     version=VERSION,
     description="splitit-web-api-v3",
     author="Konfig",
     author_email="engineering@konfigthis.com",
     url="https://github.com/konfig-dev/splitit-web-sdks/tree/main/python",
-    keywords=["OpenAPI", "Konfig", "splitit-web-api-v3"],
+    keywords=["Konfig", "splitit-web-api-v3"],
+    license="MIT",
     python_requires=">=3.7",
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/__init__.py` & `splitit-web-python-sdk-2.1.0/splitit_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Splitit's Web API
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
-__version__ = "2.0.0"
+__version__ = "2.1.0"
 
 # import ApiClient
 from splitit_client.api_client import ApiClient
 
 # import Configuration
 from splitit_client.configuration import Configuration
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/api_client.py` & `splitit-web-python-sdk-2.1.0/splitit_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1032,17 +1032,15 @@
     """Generic API client for OpenAPI client library builds.
 
     OpenAPI generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
     the methods and models for each application are generated from the OpenAPI
     templates.
 
-    NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-    Do not edit the class manually.
+    This class is auto generated by Konfig (https://konfigthis.com)
 
     :param configuration: .Configuration object for this client
     :param header_name: a header to pass when making calls to the API.
     :param header_value: a header value to pass when making calls to
         the API.
     :param cookie: a cookie to include in the header when making calls
         to the API
@@ -1067,15 +1065,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Konfig/2.0.0/python'
+        self.user_agent = 'Konfig/2.1.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
@@ -1394,18 +1392,16 @@
                 raise ApiValueError(
                     'Authentication token must be in `query` or `header`'
                 )
         return resource_path
 
 
 class Api:
-    """NOTE: This class is auto generated by Konfig
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """NOTE:
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
     def __init__(self, api_client: typing.Optional[ApiClient] = None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/apis/path_to_api.py` & `splitit-web-python-sdk-2.1.0/splitit_client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/apis/tags/installment_plan_api.py` & `splitit-web-python-sdk-2.1.0/splitit_client/apis/tags/installment_plan_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,13 +29,11 @@
     Post2,
     Refund,
     Search,
     UpdateOrder,
     UpdateOrder2,
     VerifyAuthorization,
 ):
-    """NOTE: This class is auto generated by Konfig
-    Ref: https://konfgithis.com
-
-    Do not edit the class manually.
+    """NOTE:
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
     pass
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/client.py` & `splitit-web-python-sdk-2.1.0/splitit_client/client.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/configuration.py` & `splitit-web-python-sdk-2.1.0/splitit_client/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,16 @@
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems',
     'uniqueItems', 'maxProperties', 'minProperties',
 }
 
 class Configuration(object):
-    """NOTE: This class is auto generated by Konfig
-
-    Ref: https://konfigthis.com
-    Do not edit the class manually.
+    """NOTE:
+    This class is auto generated by Konfig (https://konfigthis.com)
 
     :param host: Base url
     :param api_key: Dict to store API key(s).
       Each entry in the dict specifies an API key.
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is the API key secret.
     :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
@@ -398,15 +396,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 2.0.0".\
+               "SDK Package Version: 2.1.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/exceptions.py` & `splitit-web-python-sdk-2.1.0/splitit_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/exceptions_base.py` & `splitit-web-python-sdk-2.1.0/splitit_client/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/address_data.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/address_data_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,44 +19,42 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class AddressData(
+class AddressDataModel(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
-            AddressLine = schemas.StrSchema
+            AddressLine1 = schemas.StrSchema
             AddressLine2 = schemas.StrSchema
             City = schemas.StrSchema
             Country = schemas.StrSchema
             State = schemas.StrSchema
             Zip = schemas.StrSchema
             __annotations__ = {
-                "AddressLine": AddressLine,
+                "AddressLine1": AddressLine1,
                 "AddressLine2": AddressLine2,
                 "City": City,
                 "Country": Country,
                 "State": State,
                 "Zip": Zip,
             }
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["AddressLine"]) -> MetaOapg.properties.AddressLine: ...
+    def __getitem__(self, name: typing_extensions.Literal["AddressLine1"]) -> MetaOapg.properties.AddressLine1: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["AddressLine2"]) -> MetaOapg.properties.AddressLine2: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["City"]) -> MetaOapg.properties.City: ...
     
@@ -68,21 +66,21 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Zip"]) -> MetaOapg.properties.Zip: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AddressLine", "AddressLine2", "City", "Country", "State", "Zip", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AddressLine1", "AddressLine2", "City", "Country", "State", "Zip", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["AddressLine"]) -> typing.Union[MetaOapg.properties.AddressLine, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["AddressLine1"]) -> typing.Union[MetaOapg.properties.AddressLine1, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["AddressLine2"]) -> typing.Union[MetaOapg.properties.AddressLine2, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["City"]) -> typing.Union[MetaOapg.properties.City, schemas.Unset]: ...
     
@@ -94,34 +92,34 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Zip"]) -> typing.Union[MetaOapg.properties.Zip, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AddressLine", "AddressLine2", "City", "Country", "State", "Zip", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AddressLine1", "AddressLine2", "City", "Country", "State", "Zip", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        AddressLine: typing.Union[MetaOapg.properties.AddressLine, str, schemas.Unset] = schemas.unset,
+        AddressLine1: typing.Union[MetaOapg.properties.AddressLine1, str, schemas.Unset] = schemas.unset,
         AddressLine2: typing.Union[MetaOapg.properties.AddressLine2, str, schemas.Unset] = schemas.unset,
         City: typing.Union[MetaOapg.properties.City, str, schemas.Unset] = schemas.unset,
         Country: typing.Union[MetaOapg.properties.Country, str, schemas.Unset] = schemas.unset,
         State: typing.Union[MetaOapg.properties.State, str, schemas.Unset] = schemas.unset,
         Zip: typing.Union[MetaOapg.properties.Zip, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'AddressData':
+    ) -> 'AddressDataModel':
         return super().__new__(
             cls,
             *args,
-            AddressLine=AddressLine,
+            AddressLine1=AddressLine1,
             AddressLine2=AddressLine2,
             City=City,
             Country=Country,
             State=State,
             Zip=Zip,
             _configuration=_configuration,
             **kwargs,
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/address_data_model.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/address_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,44 +19,42 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class AddressDataModel(
+class AddressData(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
-            AddressLine1 = schemas.StrSchema
+            AddressLine = schemas.StrSchema
             AddressLine2 = schemas.StrSchema
             City = schemas.StrSchema
             Country = schemas.StrSchema
             State = schemas.StrSchema
             Zip = schemas.StrSchema
             __annotations__ = {
-                "AddressLine1": AddressLine1,
+                "AddressLine": AddressLine,
                 "AddressLine2": AddressLine2,
                 "City": City,
                 "Country": Country,
                 "State": State,
                 "Zip": Zip,
             }
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["AddressLine1"]) -> MetaOapg.properties.AddressLine1: ...
+    def __getitem__(self, name: typing_extensions.Literal["AddressLine"]) -> MetaOapg.properties.AddressLine: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["AddressLine2"]) -> MetaOapg.properties.AddressLine2: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["City"]) -> MetaOapg.properties.City: ...
     
@@ -68,21 +66,21 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Zip"]) -> MetaOapg.properties.Zip: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AddressLine1", "AddressLine2", "City", "Country", "State", "Zip", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AddressLine", "AddressLine2", "City", "Country", "State", "Zip", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["AddressLine1"]) -> typing.Union[MetaOapg.properties.AddressLine1, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["AddressLine"]) -> typing.Union[MetaOapg.properties.AddressLine, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["AddressLine2"]) -> typing.Union[MetaOapg.properties.AddressLine2, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["City"]) -> typing.Union[MetaOapg.properties.City, schemas.Unset]: ...
     
@@ -94,34 +92,34 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Zip"]) -> typing.Union[MetaOapg.properties.Zip, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AddressLine1", "AddressLine2", "City", "Country", "State", "Zip", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AddressLine", "AddressLine2", "City", "Country", "State", "Zip", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        AddressLine1: typing.Union[MetaOapg.properties.AddressLine1, str, schemas.Unset] = schemas.unset,
+        AddressLine: typing.Union[MetaOapg.properties.AddressLine, str, schemas.Unset] = schemas.unset,
         AddressLine2: typing.Union[MetaOapg.properties.AddressLine2, str, schemas.Unset] = schemas.unset,
         City: typing.Union[MetaOapg.properties.City, str, schemas.Unset] = schemas.unset,
         Country: typing.Union[MetaOapg.properties.Country, str, schemas.Unset] = schemas.unset,
         State: typing.Union[MetaOapg.properties.State, str, schemas.Unset] = schemas.unset,
         Zip: typing.Union[MetaOapg.properties.Zip, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'AddressDataModel':
+    ) -> 'AddressData':
         return super().__new__(
             cls,
             *args,
-            AddressLine1=AddressLine1,
+            AddressLine=AddressLine,
             AddressLine2=AddressLine2,
             City=City,
             Country=Country,
             State=State,
             Zip=Zip,
             _configuration=_configuration,
             **kwargs,
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/authorization_model.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/authorization_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class AuthorizationModel(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "Status",
         }
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/card_brand.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/card_brand.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,16 @@
 from splitit_client import schemas  # noqa: F401
 
 
 class CardBrand(
     schemas.EnumBase,
     schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
             "Mastercard": "MASTERCARD",
             "Visa": "VISA",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/card_data.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/card_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class CardData(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
             CardHolderFullName = schemas.StrSchema
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/card_type.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/card_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,18 +23,16 @@
 from splitit_client import schemas  # noqa: F401
 
 
 class CardType(
     schemas.EnumBase,
     schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
             "Credit": "CREDIT",
             "Debit": "DEBIT",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/check_installments_eligibility_request.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/check_installments_eligibility_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class CheckInstallmentsEligibilityRequest(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/error.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/error.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class Error(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
             Code = schemas.StrSchema
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/error_extended.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/error_extended.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class ErrorExtended(
     schemas.ComposedSchema,
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         
         class all_of_1(
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/failed_response.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/failed_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class FailedResponse(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
             TraceId = schemas.StrSchema
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/gw_authorization_status.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/gw_authorization_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,18 +23,16 @@
 from splitit_client import schemas  # noqa: F401
 
 
 class GwAuthorizationStatus(
     schemas.EnumBase,
     schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
             "NA": "NA",
             "Succeeded": "SUCCEEDED",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/identifier_contract.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/identifier_contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class IdentifierContract(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
             RefOrderNumber = schemas.StrSchema
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/initiate_plan_response.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/initiate_plan_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class InitiatePlanResponse(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "Status",
         }
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/initiate_redirection_endpoints_model.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/initiate_redirection_endpoints_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class InitiateRedirectionEndpointsModel(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
             Succeeded = schemas.StrSchema
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/installment.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/installment.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class Installment(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "Status",
             "InstallmentNumber",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_cancel_response.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_cancel_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class InstallmentPlanCancelResponse(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
             InstallmentPlanNumber = schemas.StrSchema
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_create_request.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class InstallmentPlanCreateRequest(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "TermsAndConditionsAccepted",
             "AutoCapture",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_create_response.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_create_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class InstallmentPlanCreateResponse(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "Status",
             "DateCreated",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_get_response.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_get_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class InstallmentPlanGetResponse(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "Status",
             "DateCreated",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_initiate_request.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_initiate_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,25 +22,22 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class InstallmentPlanInitiateRequest(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "AutoCapture",
-            "Attempt3dSecure",
         }
         
         class properties:
             AutoCapture = schemas.BoolSchema
             Attempt3dSecure = schemas.BoolSchema
         
             @staticmethod
@@ -54,25 +51,29 @@
             @staticmethod
             def BillingAddress() -> typing.Type['AddressDataModel']:
                 return AddressDataModel
         
             @staticmethod
             def RedirectUrls() -> typing.Type['InitiateRedirectionEndpointsModel']:
                 return InitiateRedirectionEndpointsModel
+        
+            @staticmethod
+            def UxSettings() -> typing.Type['UxSettingsModel']:
+                return UxSettingsModel
             __annotations__ = {
                 "AutoCapture": AutoCapture,
                 "Attempt3dSecure": Attempt3dSecure,
                 "Shopper": Shopper,
                 "PlanData": PlanData,
                 "BillingAddress": BillingAddress,
                 "RedirectUrls": RedirectUrls,
+                "UxSettings": UxSettings,
             }
     
     AutoCapture: MetaOapg.properties.AutoCapture
-    Attempt3dSecure: MetaOapg.properties.Attempt3dSecure
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["AutoCapture"]) -> MetaOapg.properties.AutoCapture: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Attempt3dSecure"]) -> MetaOapg.properties.Attempt3dSecure: ...
     
@@ -85,68 +86,77 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["BillingAddress"]) -> 'AddressDataModel': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["RedirectUrls"]) -> 'InitiateRedirectionEndpointsModel': ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["UxSettings"]) -> 'UxSettingsModel': ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "RedirectUrls", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "RedirectUrls", "UxSettings", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["AutoCapture"]) -> MetaOapg.properties.AutoCapture: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Attempt3dSecure"]) -> MetaOapg.properties.Attempt3dSecure: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Attempt3dSecure"]) -> typing.Union[MetaOapg.properties.Attempt3dSecure, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Shopper"]) -> typing.Union['ShopperData', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["PlanData"]) -> typing.Union['PlanDataModel', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["BillingAddress"]) -> typing.Union['AddressDataModel', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["RedirectUrls"]) -> typing.Union['InitiateRedirectionEndpointsModel', schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["UxSettings"]) -> typing.Union['UxSettingsModel', schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "RedirectUrls", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "RedirectUrls", "UxSettings", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         AutoCapture: typing.Union[MetaOapg.properties.AutoCapture, bool, ],
-        Attempt3dSecure: typing.Union[MetaOapg.properties.Attempt3dSecure, bool, ],
+        Attempt3dSecure: typing.Union[MetaOapg.properties.Attempt3dSecure, bool, schemas.Unset] = schemas.unset,
         Shopper: typing.Union['ShopperData', schemas.Unset] = schemas.unset,
         PlanData: typing.Union['PlanDataModel', schemas.Unset] = schemas.unset,
         BillingAddress: typing.Union['AddressDataModel', schemas.Unset] = schemas.unset,
         RedirectUrls: typing.Union['InitiateRedirectionEndpointsModel', schemas.Unset] = schemas.unset,
+        UxSettings: typing.Union['UxSettingsModel', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'InstallmentPlanInitiateRequest':
         return super().__new__(
             cls,
             *args,
             AutoCapture=AutoCapture,
             Attempt3dSecure=Attempt3dSecure,
             Shopper=Shopper,
             PlanData=PlanData,
             BillingAddress=BillingAddress,
             RedirectUrls=RedirectUrls,
+            UxSettings=UxSettings,
             _configuration=_configuration,
             **kwargs,
         )
 
 from splitit_client.model.address_data_model import AddressDataModel
 from splitit_client.model.initiate_redirection_endpoints_model import InitiateRedirectionEndpointsModel
 from splitit_client.model.plan_data_model import PlanDataModel
 from splitit_client.model.shopper_data import ShopperData
+from splitit_client.model.ux_settings_model import UxSettingsModel
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_refund_request.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_refund_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class InstallmentPlanRefundRequest(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "Amount",
         }
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_refund_response.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_refund_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class InstallmentPlanRefundResponse(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
             RefundId = schemas.StrSchema
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_search_response.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_search_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class InstallmentPlanSearchResponse(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_update_request.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_update_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class InstallmentPlanUpdateRequest(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
             RefOrderNumber = schemas.StrSchema
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_update_request_by_identifier.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_update_request_by_identifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class InstallmentPlanUpdateRequestByIdentifier(
     schemas.ComposedSchema,
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         
         class all_of_1(
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/installment_plan_update_response.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_update_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class InstallmentPlanUpdateResponse(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "Status",
             "ShippingStatus",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/installment_status.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,16 @@
 from splitit_client import schemas  # noqa: F401
 
 
 class InstallmentStatus(
     schemas.EnumBase,
     schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
             "Pending": "PENDING",
             "Processed": "PROCESSED",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/installments_eligibility_response.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/installments_eligibility_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class InstallmentsEligibilityResponse(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/links_data.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/links_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class LinksData(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
             Checkout = schemas.StrSchema
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/links_model.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/links_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class LinksModel(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
             PrivacyPolicyUrl = schemas.StrSchema
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/payment_method_model.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/payment_method_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class PaymentMethodModel(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "Type",
         }
@@ -43,60 +41,70 @@
             @staticmethod
             def Type() -> typing.Type['PaymentMethodType']:
                 return PaymentMethodType
         
             @staticmethod
             def Card() -> typing.Type['CardData']:
                 return CardData
+            Token = schemas.StrSchema
             __annotations__ = {
                 "Type": Type,
                 "Card": Card,
+                "Token": Token,
             }
     
     Type: 'PaymentMethodType'
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Type"]) -> 'PaymentMethodType': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Card"]) -> 'CardData': ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["Token"]) -> MetaOapg.properties.Token: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["Type", "Card", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["Type", "Card", "Token", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Type"]) -> 'PaymentMethodType': ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Card"]) -> typing.Union['CardData', schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["Token"]) -> typing.Union[MetaOapg.properties.Token, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["Type", "Card", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["Type", "Card", "Token", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         Type: 'PaymentMethodType',
         Card: typing.Union['CardData', schemas.Unset] = schemas.unset,
+        Token: typing.Union[MetaOapg.properties.Token, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'PaymentMethodModel':
         return super().__new__(
             cls,
             *args,
             Type=Type,
             Card=Card,
+            Token=Token,
             _configuration=_configuration,
             **kwargs,
         )
 
 from splitit_client.model.card_data import CardData
 from splitit_client.model.payment_method_type import PaymentMethodType
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/payment_method_type.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/payment_method_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,22 +23,25 @@
 from splitit_client import schemas  # noqa: F401
 
 
 class PaymentMethodType(
     schemas.EnumBase,
     schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
             "Card": "CARD",
+            "SplititToken": "SPLITIT_TOKEN",
         }
     
     @schemas.classproperty
     def CARD(cls):
         return cls("Card")
+    
+    @schemas.classproperty
+    def SPLITIT_TOKEN(cls):
+        return cls("SplititToken")
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/payment_plan_option_model.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/payment_plan_option_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class PaymentPlanOptionModel(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "LastInstallmentAmount",
             "InstallmentAmount",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/plan_data.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/plan_data_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,45 +19,41 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class PlanData(
+class PlanDataModel(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "PurchaseMethod",
             "TotalAmount",
-            "NumberOfInstallments",
         }
         
         class properties:
             TotalAmount = schemas.NumberSchema
-            NumberOfInstallments = schemas.Int32Schema
         
             @staticmethod
             def PurchaseMethod() -> typing.Type['PurchaseMethod']:
                 return PurchaseMethod
-            TerminalId = schemas.StrSchema
-            FirstInstallmentAmount = schemas.NumberSchema
             Currency = schemas.StrSchema
+            NumberOfInstallments = schemas.Int32Schema
+            TerminalId = schemas.StrSchema
             RefOrderNumber = schemas.StrSchema
             
             
-            class Tags(
+            class ExtendedParams(
                 schemas.DictSchema
             ):
             
             
                 class MetaOapg:
                     additional_properties = schemas.StrSchema
                 
@@ -69,122 +65,132 @@
                     return super().get_item_oapg(name)
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[MetaOapg.additional_properties, str, ],
-                ) -> 'Tags':
+                ) -> 'ExtendedParams':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
+            FirstInstallmentAmount = schemas.NumberSchema
+            FirstInstallmentDate = schemas.DateTimeSchema
             __annotations__ = {
                 "TotalAmount": TotalAmount,
-                "NumberOfInstallments": NumberOfInstallments,
                 "PurchaseMethod": PurchaseMethod,
-                "TerminalId": TerminalId,
-                "FirstInstallmentAmount": FirstInstallmentAmount,
                 "Currency": Currency,
+                "NumberOfInstallments": NumberOfInstallments,
+                "TerminalId": TerminalId,
                 "RefOrderNumber": RefOrderNumber,
-                "Tags": Tags,
+                "ExtendedParams": ExtendedParams,
+                "FirstInstallmentAmount": FirstInstallmentAmount,
+                "FirstInstallmentDate": FirstInstallmentDate,
             }
     
     PurchaseMethod: 'PurchaseMethod'
     TotalAmount: MetaOapg.properties.TotalAmount
-    NumberOfInstallments: MetaOapg.properties.NumberOfInstallments
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["TotalAmount"]) -> MetaOapg.properties.TotalAmount: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["NumberOfInstallments"]) -> MetaOapg.properties.NumberOfInstallments: ...
+    def __getitem__(self, name: typing_extensions.Literal["PurchaseMethod"]) -> 'PurchaseMethod': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["PurchaseMethod"]) -> 'PurchaseMethod': ...
+    def __getitem__(self, name: typing_extensions.Literal["Currency"]) -> MetaOapg.properties.Currency: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["NumberOfInstallments"]) -> MetaOapg.properties.NumberOfInstallments: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["TerminalId"]) -> MetaOapg.properties.TerminalId: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["FirstInstallmentAmount"]) -> MetaOapg.properties.FirstInstallmentAmount: ...
+    def __getitem__(self, name: typing_extensions.Literal["RefOrderNumber"]) -> MetaOapg.properties.RefOrderNumber: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Currency"]) -> MetaOapg.properties.Currency: ...
+    def __getitem__(self, name: typing_extensions.Literal["ExtendedParams"]) -> MetaOapg.properties.ExtendedParams: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["RefOrderNumber"]) -> MetaOapg.properties.RefOrderNumber: ...
+    def __getitem__(self, name: typing_extensions.Literal["FirstInstallmentAmount"]) -> MetaOapg.properties.FirstInstallmentAmount: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Tags"]) -> MetaOapg.properties.Tags: ...
+    def __getitem__(self, name: typing_extensions.Literal["FirstInstallmentDate"]) -> MetaOapg.properties.FirstInstallmentDate: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["TotalAmount", "NumberOfInstallments", "PurchaseMethod", "TerminalId", "FirstInstallmentAmount", "Currency", "RefOrderNumber", "Tags", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["TotalAmount", "PurchaseMethod", "Currency", "NumberOfInstallments", "TerminalId", "RefOrderNumber", "ExtendedParams", "FirstInstallmentAmount", "FirstInstallmentDate", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["TotalAmount"]) -> MetaOapg.properties.TotalAmount: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["NumberOfInstallments"]) -> MetaOapg.properties.NumberOfInstallments: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["PurchaseMethod"]) -> 'PurchaseMethod': ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["PurchaseMethod"]) -> 'PurchaseMethod': ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Currency"]) -> typing.Union[MetaOapg.properties.Currency, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["NumberOfInstallments"]) -> typing.Union[MetaOapg.properties.NumberOfInstallments, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["TerminalId"]) -> typing.Union[MetaOapg.properties.TerminalId, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["FirstInstallmentAmount"]) -> typing.Union[MetaOapg.properties.FirstInstallmentAmount, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["RefOrderNumber"]) -> typing.Union[MetaOapg.properties.RefOrderNumber, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Currency"]) -> typing.Union[MetaOapg.properties.Currency, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["ExtendedParams"]) -> typing.Union[MetaOapg.properties.ExtendedParams, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["RefOrderNumber"]) -> typing.Union[MetaOapg.properties.RefOrderNumber, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["FirstInstallmentAmount"]) -> typing.Union[MetaOapg.properties.FirstInstallmentAmount, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Tags"]) -> typing.Union[MetaOapg.properties.Tags, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["FirstInstallmentDate"]) -> typing.Union[MetaOapg.properties.FirstInstallmentDate, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["TotalAmount", "NumberOfInstallments", "PurchaseMethod", "TerminalId", "FirstInstallmentAmount", "Currency", "RefOrderNumber", "Tags", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["TotalAmount", "PurchaseMethod", "Currency", "NumberOfInstallments", "TerminalId", "RefOrderNumber", "ExtendedParams", "FirstInstallmentAmount", "FirstInstallmentDate", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         PurchaseMethod: 'PurchaseMethod',
         TotalAmount: typing.Union[MetaOapg.properties.TotalAmount, decimal.Decimal, int, float, ],
-        NumberOfInstallments: typing.Union[MetaOapg.properties.NumberOfInstallments, decimal.Decimal, int, ],
-        TerminalId: typing.Union[MetaOapg.properties.TerminalId, str, schemas.Unset] = schemas.unset,
-        FirstInstallmentAmount: typing.Union[MetaOapg.properties.FirstInstallmentAmount, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         Currency: typing.Union[MetaOapg.properties.Currency, str, schemas.Unset] = schemas.unset,
+        NumberOfInstallments: typing.Union[MetaOapg.properties.NumberOfInstallments, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        TerminalId: typing.Union[MetaOapg.properties.TerminalId, str, schemas.Unset] = schemas.unset,
         RefOrderNumber: typing.Union[MetaOapg.properties.RefOrderNumber, str, schemas.Unset] = schemas.unset,
-        Tags: typing.Union[MetaOapg.properties.Tags, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        ExtendedParams: typing.Union[MetaOapg.properties.ExtendedParams, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        FirstInstallmentAmount: typing.Union[MetaOapg.properties.FirstInstallmentAmount, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        FirstInstallmentDate: typing.Union[MetaOapg.properties.FirstInstallmentDate, str, datetime, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'PlanData':
+    ) -> 'PlanDataModel':
         return super().__new__(
             cls,
             *args,
             PurchaseMethod=PurchaseMethod,
             TotalAmount=TotalAmount,
+            Currency=Currency,
             NumberOfInstallments=NumberOfInstallments,
             TerminalId=TerminalId,
-            FirstInstallmentAmount=FirstInstallmentAmount,
-            Currency=Currency,
             RefOrderNumber=RefOrderNumber,
-            Tags=Tags,
+            ExtendedParams=ExtendedParams,
+            FirstInstallmentAmount=FirstInstallmentAmount,
+            FirstInstallmentDate=FirstInstallmentDate,
             _configuration=_configuration,
             **kwargs,
         )
 
 from splitit_client.model.purchase_method import PurchaseMethod
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/plan_data_model.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/plan_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,43 +19,66 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class PlanDataModel(
+class PlanData(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "PurchaseMethod",
             "TotalAmount",
+            "NumberOfInstallments",
         }
         
         class properties:
             TotalAmount = schemas.NumberSchema
+            NumberOfInstallments = schemas.Int32Schema
         
             @staticmethod
             def PurchaseMethod() -> typing.Type['PurchaseMethod']:
                 return PurchaseMethod
-            Currency = schemas.StrSchema
-            NumberOfInstallments = schemas.Int32Schema
             TerminalId = schemas.StrSchema
+            FirstInstallmentAmount = schemas.NumberSchema
+            Currency = schemas.StrSchema
             RefOrderNumber = schemas.StrSchema
             
             
-            class ExtendedParams(
+            class AllowedInstallmentOptions(
+                schemas.ListSchema
+            ):
+            
+            
+                class MetaOapg:
+                    items = schemas.Int32Schema
+            
+                def __new__(
+                    cls,
+                    arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, decimal.Decimal, int, ]], typing.List[typing.Union[MetaOapg.items, decimal.Decimal, int, ]]],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'AllowedInstallmentOptions':
+                    return super().__new__(
+                        cls,
+                        arg,
+                        _configuration=_configuration,
+                    )
+            
+                def __getitem__(self, i: int) -> MetaOapg.items:
+                    return super().__getitem__(i)
+            
+            
+            class Tags(
                 schemas.DictSchema
             ):
             
             
                 class MetaOapg:
                     additional_properties = schemas.StrSchema
                 
@@ -67,122 +90,141 @@
                     return super().get_item_oapg(name)
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[MetaOapg.additional_properties, str, ],
-                ) -> 'ExtendedParams':
+                ) -> 'Tags':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            FirstInstallmentAmount = schemas.NumberSchema
+            FirstInstallmentDate = schemas.DateTimeSchema
             __annotations__ = {
                 "TotalAmount": TotalAmount,
-                "PurchaseMethod": PurchaseMethod,
-                "Currency": Currency,
                 "NumberOfInstallments": NumberOfInstallments,
+                "PurchaseMethod": PurchaseMethod,
                 "TerminalId": TerminalId,
-                "RefOrderNumber": RefOrderNumber,
-                "ExtendedParams": ExtendedParams,
                 "FirstInstallmentAmount": FirstInstallmentAmount,
+                "Currency": Currency,
+                "RefOrderNumber": RefOrderNumber,
+                "AllowedInstallmentOptions": AllowedInstallmentOptions,
+                "Tags": Tags,
+                "FirstInstallmentDate": FirstInstallmentDate,
             }
     
     PurchaseMethod: 'PurchaseMethod'
     TotalAmount: MetaOapg.properties.TotalAmount
+    NumberOfInstallments: MetaOapg.properties.NumberOfInstallments
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["TotalAmount"]) -> MetaOapg.properties.TotalAmount: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["NumberOfInstallments"]) -> MetaOapg.properties.NumberOfInstallments: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["PurchaseMethod"]) -> 'PurchaseMethod': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Currency"]) -> MetaOapg.properties.Currency: ...
+    def __getitem__(self, name: typing_extensions.Literal["TerminalId"]) -> MetaOapg.properties.TerminalId: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["NumberOfInstallments"]) -> MetaOapg.properties.NumberOfInstallments: ...
+    def __getitem__(self, name: typing_extensions.Literal["FirstInstallmentAmount"]) -> MetaOapg.properties.FirstInstallmentAmount: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["TerminalId"]) -> MetaOapg.properties.TerminalId: ...
+    def __getitem__(self, name: typing_extensions.Literal["Currency"]) -> MetaOapg.properties.Currency: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["RefOrderNumber"]) -> MetaOapg.properties.RefOrderNumber: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["ExtendedParams"]) -> MetaOapg.properties.ExtendedParams: ...
+    def __getitem__(self, name: typing_extensions.Literal["AllowedInstallmentOptions"]) -> MetaOapg.properties.AllowedInstallmentOptions: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["FirstInstallmentAmount"]) -> MetaOapg.properties.FirstInstallmentAmount: ...
+    def __getitem__(self, name: typing_extensions.Literal["Tags"]) -> MetaOapg.properties.Tags: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["FirstInstallmentDate"]) -> MetaOapg.properties.FirstInstallmentDate: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["TotalAmount", "PurchaseMethod", "Currency", "NumberOfInstallments", "TerminalId", "RefOrderNumber", "ExtendedParams", "FirstInstallmentAmount", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["TotalAmount", "NumberOfInstallments", "PurchaseMethod", "TerminalId", "FirstInstallmentAmount", "Currency", "RefOrderNumber", "AllowedInstallmentOptions", "Tags", "FirstInstallmentDate", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["TotalAmount"]) -> MetaOapg.properties.TotalAmount: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["NumberOfInstallments"]) -> MetaOapg.properties.NumberOfInstallments: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["PurchaseMethod"]) -> 'PurchaseMethod': ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Currency"]) -> typing.Union[MetaOapg.properties.Currency, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["TerminalId"]) -> typing.Union[MetaOapg.properties.TerminalId, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["NumberOfInstallments"]) -> typing.Union[MetaOapg.properties.NumberOfInstallments, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["FirstInstallmentAmount"]) -> typing.Union[MetaOapg.properties.FirstInstallmentAmount, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["TerminalId"]) -> typing.Union[MetaOapg.properties.TerminalId, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Currency"]) -> typing.Union[MetaOapg.properties.Currency, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["RefOrderNumber"]) -> typing.Union[MetaOapg.properties.RefOrderNumber, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["ExtendedParams"]) -> typing.Union[MetaOapg.properties.ExtendedParams, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["AllowedInstallmentOptions"]) -> typing.Union[MetaOapg.properties.AllowedInstallmentOptions, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["FirstInstallmentAmount"]) -> typing.Union[MetaOapg.properties.FirstInstallmentAmount, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Tags"]) -> typing.Union[MetaOapg.properties.Tags, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["FirstInstallmentDate"]) -> typing.Union[MetaOapg.properties.FirstInstallmentDate, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["TotalAmount", "PurchaseMethod", "Currency", "NumberOfInstallments", "TerminalId", "RefOrderNumber", "ExtendedParams", "FirstInstallmentAmount", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["TotalAmount", "NumberOfInstallments", "PurchaseMethod", "TerminalId", "FirstInstallmentAmount", "Currency", "RefOrderNumber", "AllowedInstallmentOptions", "Tags", "FirstInstallmentDate", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         PurchaseMethod: 'PurchaseMethod',
         TotalAmount: typing.Union[MetaOapg.properties.TotalAmount, decimal.Decimal, int, float, ],
-        Currency: typing.Union[MetaOapg.properties.Currency, str, schemas.Unset] = schemas.unset,
-        NumberOfInstallments: typing.Union[MetaOapg.properties.NumberOfInstallments, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        NumberOfInstallments: typing.Union[MetaOapg.properties.NumberOfInstallments, decimal.Decimal, int, ],
         TerminalId: typing.Union[MetaOapg.properties.TerminalId, str, schemas.Unset] = schemas.unset,
-        RefOrderNumber: typing.Union[MetaOapg.properties.RefOrderNumber, str, schemas.Unset] = schemas.unset,
-        ExtendedParams: typing.Union[MetaOapg.properties.ExtendedParams, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         FirstInstallmentAmount: typing.Union[MetaOapg.properties.FirstInstallmentAmount, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        Currency: typing.Union[MetaOapg.properties.Currency, str, schemas.Unset] = schemas.unset,
+        RefOrderNumber: typing.Union[MetaOapg.properties.RefOrderNumber, str, schemas.Unset] = schemas.unset,
+        AllowedInstallmentOptions: typing.Union[MetaOapg.properties.AllowedInstallmentOptions, list, tuple, schemas.Unset] = schemas.unset,
+        Tags: typing.Union[MetaOapg.properties.Tags, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        FirstInstallmentDate: typing.Union[MetaOapg.properties.FirstInstallmentDate, str, datetime, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'PlanDataModel':
+    ) -> 'PlanData':
         return super().__new__(
             cls,
             *args,
             PurchaseMethod=PurchaseMethod,
             TotalAmount=TotalAmount,
-            Currency=Currency,
             NumberOfInstallments=NumberOfInstallments,
             TerminalId=TerminalId,
-            RefOrderNumber=RefOrderNumber,
-            ExtendedParams=ExtendedParams,
             FirstInstallmentAmount=FirstInstallmentAmount,
+            Currency=Currency,
+            RefOrderNumber=RefOrderNumber,
+            AllowedInstallmentOptions=AllowedInstallmentOptions,
+            Tags=Tags,
+            FirstInstallmentDate=FirstInstallmentDate,
             _configuration=_configuration,
             **kwargs,
         )
 
 from splitit_client.model.purchase_method import PurchaseMethod
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/plan_error_response.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/plan_error_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class PlanErrorResponse(
     schemas.ComposedSchema,
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         
         class all_of_1(
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/plan_status.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/refund_status.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,46 +19,34 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class PlanStatus(
+class RefundStatus(
     schemas.EnumBase,
     schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
-            "Initialized": "INITIALIZED",
-            "PendingCapture": "PENDING_CAPTURE",
-            "Active": "ACTIVE",
-            "Cleared": "CLEARED",
-            "Canceled": "CANCELED",
+            "Pending": "PENDING",
+            "Succeeded": "SUCCEEDED",
+            "Failed": "FAILED",
         }
     
     @schemas.classproperty
-    def INITIALIZED(cls):
-        return cls("Initialized")
-    
-    @schemas.classproperty
-    def PENDING_CAPTURE(cls):
-        return cls("PendingCapture")
-    
-    @schemas.classproperty
-    def ACTIVE(cls):
-        return cls("Active")
+    def PENDING(cls):
+        return cls("Pending")
     
     @schemas.classproperty
-    def CLEARED(cls):
-        return cls("Cleared")
+    def SUCCEEDED(cls):
+        return cls("Succeeded")
     
     @schemas.classproperty
-    def CANCELED(cls):
-        return cls("Canceled")
+    def FAILED(cls):
+        return cls("Failed")
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/purchase_method.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/purchase_method.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,18 +23,16 @@
 from splitit_client import schemas  # noqa: F401
 
 
 class PurchaseMethod(
     schemas.EnumBase,
     schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
             "InStore": "IN_STORE",
             "PhoneOrder": "PHONE_ORDER",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/redirection_endpoints_model.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/redirection_endpoints_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class RedirectionEndpointsModel(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
             AuthorizeSucceeded = schemas.StrSchema
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/refund_model.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/refund_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class RefundModel(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "Status",
             "NonCreditRefundAmount",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/refund_status.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/plan_status.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,36 +19,44 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class RefundStatus(
+class PlanStatus(
     schemas.EnumBase,
     schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
-            "Pending": "PENDING",
-            "Succeeded": "SUCCEEDED",
-            "Failed": "FAILED",
+            "Initialized": "INITIALIZED",
+            "PendingCapture": "PENDING_CAPTURE",
+            "Active": "ACTIVE",
+            "Cleared": "CLEARED",
+            "Canceled": "CANCELED",
         }
     
     @schemas.classproperty
-    def PENDING(cls):
-        return cls("Pending")
+    def INITIALIZED(cls):
+        return cls("Initialized")
+    
+    @schemas.classproperty
+    def PENDING_CAPTURE(cls):
+        return cls("PendingCapture")
+    
+    @schemas.classproperty
+    def ACTIVE(cls):
+        return cls("Active")
     
     @schemas.classproperty
-    def SUCCEEDED(cls):
-        return cls("Succeeded")
+    def CLEARED(cls):
+        return cls("Cleared")
     
     @schemas.classproperty
-    def FAILED(cls):
-        return cls("Failed")
+    def CANCELED(cls):
+        return cls("Canceled")
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/refund_strategy.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/refund_strategy.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,18 +23,16 @@
 from splitit_client import schemas  # noqa: F401
 
 
 class RefundStrategy(
     schemas.EnumBase,
     schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
             "FutureInstallmentsFirst": "FUTURE_INSTALLMENTS_FIRST",
             "FutureInstallmentsLast": "FUTURE_INSTALLMENTS_LAST",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/refund_summary.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/refund_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class RefundSummary(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
             TotalAmount = schemas.NumberSchema
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/search_installment_plan_response_item.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/search_installment_plan_response_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class SearchInstallmentPlanResponseItem(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "Status",
             "DateCreated",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/shipping_status.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/shipping_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,18 +23,16 @@
 from splitit_client import schemas  # noqa: F401
 
 
 class ShippingStatus(
     schemas.EnumBase,
     schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
             "Pending": "PENDING",
             "Shipped": "SHIPPED",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/shipping_status2.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/shipping_status2.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,18 +23,16 @@
 from splitit_client import schemas  # noqa: F401
 
 
 class ShippingStatus2(
     schemas.EnumBase,
     schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
             "Shipped": "SHIPPED",
             "Delivered": "DELIVERED",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/shopper_data.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/shopper_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class ShopperData(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
             FullName = schemas.StrSchema
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/test_modes.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/test_modes.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,18 +23,16 @@
 from splitit_client import schemas  # noqa: F401
 
 
 class TestModes(
     schemas.EnumBase,
     schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
             "None": "NONE",
             "Regular": "REGULAR",
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/three_ds_redirect_data_v3.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/three_ds_redirect_data_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class ThreeDsRedirectDataV3(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
             Url = schemas.StrSchema
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/update_order_request.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/update_order_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class UpdateOrderRequest(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
             TrackingNumber = schemas.StrSchema
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/model/verify_authorization_response.py` & `splitit-web-python-sdk-2.1.0/splitit_client/model/verify_authorization_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,16 @@
 
 from splitit_client import schemas  # noqa: F401
 
 
 class VerifyAuthorizationResponse(
     schemas.DictSchema
 ):
-    """NOTE: This class is auto generated by Konfig.
-    Ref: https://konfigthis.com
-
-    Do not edit the class manually.
+    """
+    This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "IsAuthorized",
         }
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/models/__init__.py` & `splitit-web-python-sdk-2.1.0/splitit_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,8 +57,9 @@
 from splitit_client.model.search_installment_plan_response_item import SearchInstallmentPlanResponseItem
 from splitit_client.model.shipping_status import ShippingStatus
 from splitit_client.model.shipping_status2 import ShippingStatus2
 from splitit_client.model.shopper_data import ShopperData
 from splitit_client.model.test_modes import TestModes
 from splitit_client.model.three_ds_redirect_data_v3 import ThreeDsRedirectDataV3
 from splitit_client.model.update_order_request import UpdateOrderRequest
+from splitit_client.model.ux_settings_model import UxSettingsModel
 from splitit_client.model.verify_authorization_response import VerifyAuthorizationResponse
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/paths/__init__.py` & `splitit-web-python-sdk-2.1.0/splitit_client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans/post.py` & `splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from splitit_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -442,15 +446,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_check_eligibility/post.py` & `splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_check_eligibility/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from splitit_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -377,15 +381,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_initiate/post.py` & `splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_initiate/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from splitit_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -442,15 +446,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.py` & `splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from splitit_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -321,15 +325,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.py` & `splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from splitit_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -321,15 +325,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.py` & `splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from splitit_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -425,15 +429,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.py` & `splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from splitit_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -425,15 +429,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.py` & `splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from splitit_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -321,15 +325,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_search/get.py` & `splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_search/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from splitit_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -368,15 +372,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/paths/api_installmentplans_updateorder/put.py` & `splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_updateorder/put.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from splitit_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -377,15 +381,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/request_after_hook.py` & `splitit-web-python-sdk-2.1.0/splitit_client/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/request_before_hook.py` & `splitit-web-python-sdk-2.1.0/splitit_client/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/rest.py` & `splitit-web-python-sdk-2.1.0/splitit_client/rest.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/schemas.py` & `splitit-web-python-sdk-2.1.0/splitit_client/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,19 +224,19 @@
                              True if it is a key in a dict
                              False if our item is an item in a tuple
         """
         key_or_value = "value"
         if key_type:
             key_or_value = "key"
         valid_classes_phrase = cls.__get_valid_classes_phrase(valid_classes)
-        msg = "Invalid type. Required {1} type {2} and " "passed type was {3}".format(
-            var_name,
+        msg = "Invalid type. Required {0} type {1} and " "passed type was {2} for \"{3}\"".format(
             key_or_value,
             valid_classes_phrase,
             type(var_value).__name__,
+            var_name,
         )
         return msg
 
     @classmethod
     def __get_type_error(cls, var_value, path_to_item, valid_classes, key_type=False):
         error_msg = cls.__type_error_message(
             var_name=path_to_item[-1],
@@ -458,15 +458,15 @@
         if not __kwargs and args and not isinstance(args[0], dict):
             __arg = args[0]
         else:
             __arg = cls.__get_input_dict(*args, **__kwargs)
         __from_server = False
         __validated_path_to_schemas = {}
         __arg = cast_to_allowed_types(
-            __arg, __from_server, __validated_path_to_schemas)
+            __arg, __from_server, __validated_path_to_schemas, schema=cls)
         __validation_metadata = ValidationMetadata(
             configuration=_configuration, from_server=__from_server, validated_path_to_schemas=__validated_path_to_schemas)
         __path_to_schemas = cls.__get_new_cls(__arg, __validation_metadata)
         __new_cls = __path_to_schemas[__validation_metadata.path_to_item]
         return __new_cls._get_new_instance_without_conversion_oapg(
             __arg,
             __validation_metadata.path_to_item,
@@ -509,21 +509,24 @@
 for cls in object_classes:
     print(cls)
 """
 if typing.TYPE_CHECKING:
     # qty 1
     NoneMixin = NoneClass
     FrozenDictMixin = frozendict.frozendict
+    IntMixin = int
     TupleMixin = tuple
     StrMixin = str
     DecimalMixin = decimal.Decimal
     BoolMixin = BoolClass
     BytesMixin = bytes
     FileMixin = FileIO
     # qty 2
+    class NumberMixin(decimal.Decimal, int):
+        pass
     class BinaryMixin(bytes, FileIO):
         pass
     class NoneFrozenDictMixin(NoneClass, frozendict.frozendict):
         pass
     class NoneTupleMixin(NoneClass, tuple):
         pass
     class NoneStrMixin(NoneClass, str):
@@ -636,36 +639,40 @@
     class NoneTupleStrDecimalBoolMixin(NoneClass, tuple, str, decimal.Decimal, BoolClass):
         pass
     class FrozenDictTupleStrDecimalBoolMixin(frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass):
         pass
     # qty 6
     class NoneFrozenDictTupleStrDecimalBoolMixin(NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass):
         pass
-    # qty 8
-    class NoneFrozenDictTupleStrDecimalBoolFileBytesMixin(NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass, FileIO, bytes):
+    # qty 9
+    class NoneFrozenDictTupleStrIntDecimalBoolFileBytesMixin(NoneClass, frozendict.frozendict, tuple, str, int, decimal.Decimal, BoolClass, FileIO, bytes):
         pass
 else:
     # qty 1
     class NoneMixin:
         _types = {NoneClass}
     class FrozenDictMixin:
         _types = {frozendict.frozendict}
     class TupleMixin:
         _types = {tuple}
     class StrMixin:
         _types = {str}
     class DecimalMixin:
         _types = {decimal.Decimal}
+    class IntMixin:
+        _types = {int}
     class BoolMixin:
         _types = {BoolClass}
     class BytesMixin:
         _types = {bytes}
     class FileMixin:
         _types = {FileIO}
     # qty 2
+    class NumberMixin:
+        _types = {decimal.Decimal, int}
     class BinaryMixin:
         _types = {bytes, FileIO}
     class NoneFrozenDictMixin:
         _types = {NoneClass, frozendict.frozendict}
     class NoneTupleMixin:
         _types = {NoneClass, tuple}
     class NoneStrMixin:
@@ -778,17 +785,17 @@
     class NoneTupleStrDecimalBoolMixin:
         _types = {NoneClass, tuple, str, decimal.Decimal, BoolClass}
     class FrozenDictTupleStrDecimalBoolMixin:
         _types = {frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass}
     # qty 6
     class NoneFrozenDictTupleStrDecimalBoolMixin:
         _types = {NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass}
-    # qty 8
-    class NoneFrozenDictTupleStrDecimalBoolFileBytesMixin:
-        _types = {NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass, FileIO, bytes}
+    # qty 9
+    class NoneFrozenDictTupleStrIntDecimalBoolFileBytesMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, str, int, decimal.Decimal, BoolClass, FileIO, bytes}
 
 
 class ValidatorBase:
     @staticmethod
     def _is_json_validation_enabled_oapg(schema_keyword, configuration=None):
         """Returns true if JSON schema validation is enabled for the specified
         validation keyword. This can be used to skip JSON schema structural validation
@@ -1535,17 +1542,17 @@
                 path_to_item=path_to_item,
                 validated_path_to_schemas=validation_metadata.validated_path_to_schemas
             )
             if arg_validation_metadata.validation_ran_earlier(schema):
                 continue
             try:
                 other_path_to_schemas = schema._validate_oapg(value, validation_metadata=arg_validation_metadata)
+                update(path_to_schemas, other_path_to_schemas)
             except (ApiTypeError, ApiValueError) as e:
                 validation_errors.append(e)
-            update(path_to_schemas, other_path_to_schemas)
         if len(validation_errors) > 0:
             raise SchemaValidationError(validation_errors)
         return path_to_schemas
 
     @classmethod
     def __check_dict_validations(
         cls,
@@ -1699,14 +1706,15 @@
 
 
 def cast_to_allowed_types(
     arg: typing.Union[str, date, datetime, uuid.UUID, decimal.Decimal, int, float, None, dict, frozendict.frozendict, list, tuple, bytes, Schema, io.FileIO, io.BufferedReader],
     from_server: bool,
     validated_path_to_schemas: typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]],
     path_to_item: typing.Tuple[typing.Union[str, int], ...] = tuple(['args[0]']),
+    schema: Schema = None,
 ) -> typing.Union[frozendict.frozendict, tuple, decimal.Decimal, str, bytes, BoolClass, NoneClass, FileIO]:
     """
     Casts the input payload arg into the allowed types
     The input validated_path_to_schemas is mutated by running this function
 
     When from_server is False then
     - date/datetime is cast to str
@@ -1751,29 +1759,36 @@
         this check must come before isinstance(arg, (int, float))
         because isinstance(True, int) is True
         """
         if arg:
             return BoolClass.TRUE
         return BoolClass.FALSE
     elif isinstance(arg, int):
-        return decimal.Decimal(arg)
+        return arg
     elif isinstance(arg, float):
         decimal_from_float = decimal.Decimal(arg)
         if decimal_from_float.as_integer_ratio()[1] == 1:
             # 9.0 -> Decimal('9.0')
             # 3.4028234663852886e+38 -> Decimal('340282346638528859811704183484516925440.0')
             return decimal.Decimal(str(decimal_from_float)+'.0')
         return decimal_from_float
     elif isinstance(arg, (tuple, list)):
         return tuple([cast_to_allowed_types(item, from_server, validated_path_to_schemas, path_to_item + (i,)) for i, item in enumerate(arg)])
     elif isinstance(arg, (none_type, NoneClass)):
         return NoneClass.NONE
     elif isinstance(arg, (date, datetime)):
         if not from_server:
-            return arg.isoformat()
+            # if schema itself is the DateTimeSchema class then convert to isoformat
+            # if schema itself is the DateSchema class then convert to yyyy-mm-dd using strftime
+            if schema is None:
+                return arg.isoformat()
+            if schema is DateTimeSchema:
+                return arg.isoformat()
+            if schema is DateSchema:
+                return arg.strftime('%Y-%m-%d')
         raise type_error
     elif isinstance(arg, uuid.UUID):
         if not from_server:
             return str(arg)
         raise type_error
     elif isinstance(arg, decimal.Decimal):
         return decimal.Decimal(arg)
@@ -2009,15 +2024,15 @@
     def __new__(cls, arg: None, **kwargs: Configuration):
         return super().__new__(cls, arg, **kwargs)
 
 
 class NumberSchema(
     NumberBase,
     Schema,
-    DecimalMixin
+    NumberMixin
 ):
     """
     This is used for type: number with no format
     Both integers AND floats are accepted
     """
 
     @classmethod
@@ -2057,15 +2072,15 @@
         IntBase _validate_oapg
         TODO what about types = (int, number) -> IntBase, NumberBase? We could drop int and keep number only
         """
         cls.__validate_format(arg, validation_metadata=validation_metadata)
         return super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
 
-class IntSchema(IntBase, NumberSchema):
+class IntSchema(IntBase, NumberBase, Schema, IntMixin):
 
     @classmethod
     def from_openapi_data_oapg(cls, arg: int, _configuration: typing.Optional[Configuration] = None):
         return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
     def __new__(cls, arg: typing.Union[decimal.Decimal, int], **kwargs: Configuration):
         return super().__new__(cls, arg, **kwargs)
@@ -2333,15 +2348,15 @@
     DictBase,
     ListBase,
     NumberBase,
     StrBase,
     BoolBase,
     NoneBase,
     Schema,
-    NoneFrozenDictTupleStrDecimalBoolFileBytesMixin
+    NoneFrozenDictTupleStrIntDecimalBoolFileBytesMixin
 ):
     # Python representation of a schema defined as true or {}
     pass
 
 
 class UnsetAnyTypeSchema(AnyTypeSchema):
     # Used when additionalProperties/items was not explicitly defined and a defining schema is needed
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_client/validation_metadata.py` & `splitit-web-python-sdk-2.1.0/splitit_client/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/splitit_web_python_sdk.egg-info/PKG-INFO` & `splitit-web-python-sdk-2.1.0/splitit_web_python_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: splitit-web-python-sdk
-Version: 2.0.0
+Version: 2.1.0
 Summary: splitit-web-api-v3
 Home-page: https://github.com/konfig-dev/splitit-web-sdks/tree/main/python
 Author: Konfig
 Author-email: engineering@konfigthis.com
-Keywords: OpenAPI,Konfig,splitit-web-api-v3
+License: MIT
+Keywords: Konfig,splitit-web-api-v3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # splitit-web-python-sdk
 Splitit's Web API
 
 - API version: 1.0.0
-- Package version: 2.0.0
+- Package version: 2.1.0
 
 ## Requirements.
 
 Python >=3.7
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install splitit-web-python-sdk==2.0.0
+pip install splitit-web-python-sdk==2.1.0
 ```
-(you may need to run `pip` with root permission: `sudo pip install splitit-web-python-sdk==2.0.0`)
+(you may need to run `pip` with root permission: `sudo pip install splitit-web-python-sdk==2.1.0`)
 
 Then import the package:
 ```python
 import splitit_client
 ```
 ## Getting Started
 
@@ -47,32 +48,47 @@
     # See configuration.py for a list of all supported configuration parameters.
     host = "https://web-api-v3.sandbox.splitit.com",
 
     # Configure OAuth2 access token for authorization: oauth
     access_token = 'YOUR_ACCESS_TOKEN'
 )
 
-cancel_response = splitit.installment_plan.cancel(
-    path_params = {
-        'installmentPlanNumber': "installmentPlanNumber_example",
-    },
-    header_params = {
-        'X-Splitit-IdempotencyKey': "X-Splitit-IdempotencyKey_example",
-    },
-)
 try:
+    cancel_response = splitit.installment_plan.cancel(
+        path_params = {
+            'installmentPlanNumber': "installmentPlanNumber_example",
+        },
+        header_params = {
+            'X-Splitit-IdempotencyKey': "X-Splitit-IdempotencyKey_example",
+        },
+    )
+    pprint(cancel_response.body)
     pprint(cancel_response.body["installment_plan_number"])
     pprint(cancel_response.headers)
     pprint(cancel_response.status)
+    pprint(cancel_response.round_trip_time)
 except ApiException as e:
-    print("Exception when calling InstallmentPlanCancelResponse.cancel: %s\n" % e)
+    print("Exception when calling InstallmentPlanApi.cancel: %s\n" % e)
     pprint(e.body)
+    if e.status == 401:
+        pprint(e.body["trace_id"])
+        pprint(e.body["error"])
+    if e.status == 500:
+        pprint(e.body["trace_id"])
+        pprint(e.body["error"])
+    if e.status == 403:
+        pprint(e.body["trace_id"])
+        pprint(e.body["error"])
+    if e.status == 404:
+        pprint(e.body["trace_id"])
+        pprint(e.body["error"])
     pprint(e.headers)
     pprint(e.status)
     pprint(e.reason)
+    pprint(e.round_trip_time)
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://web-api-v3.sandbox.splitit.com*
 
 Class | Method | HTTP request | Description
@@ -136,14 +152,15 @@
  - [SearchInstallmentPlanResponseItem](docs/models/SearchInstallmentPlanResponseItem.md)
  - [ShippingStatus](docs/models/ShippingStatus.md)
  - [ShippingStatus2](docs/models/ShippingStatus2.md)
  - [ShopperData](docs/models/ShopperData.md)
  - [TestModes](docs/models/TestModes.md)
  - [ThreeDsRedirectDataV3](docs/models/ThreeDsRedirectDataV3.md)
  - [UpdateOrderRequest](docs/models/UpdateOrderRequest.md)
+ - [UxSettingsModel](docs/models/UxSettingsModel.md)
  - [VerifyAuthorizationResponse](docs/models/VerifyAuthorizationResponse.md)
 
 ## Documentation For Authorization
 
  Authentication schemes defined for the API:
 ## oauth
```

### Comparing `splitit-web-python-sdk-2.0.0/splitit_web_python_sdk.egg-info/SOURCES.txt` & `splitit-web-python-sdk-2.1.0/splitit_web_python_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 splitit_client/model/search_installment_plan_response_item.py
 splitit_client/model/shipping_status.py
 splitit_client/model/shipping_status2.py
 splitit_client/model/shopper_data.py
 splitit_client/model/test_modes.py
 splitit_client/model/three_ds_redirect_data_v3.py
 splitit_client/model/update_order_request.py
+splitit_client/model/ux_settings_model.py
 splitit_client/model/verify_authorization_response.py
 splitit_client/models/__init__.py
 splitit_client/paths/__init__.py
 splitit_client/paths/api_installmentplans/__init__.py
 splitit_client/paths/api_installmentplans/post.py
 splitit_client/paths/api_installmentplans_check_eligibility/__init__.py
 splitit_client/paths/api_installmentplans_check_eligibility/post.py
@@ -157,14 +158,15 @@
 test/test_models/test_search_installment_plan_response_item.py
 test/test_models/test_shipping_status.py
 test/test_models/test_shipping_status2.py
 test/test_models/test_shopper_data.py
 test/test_models/test_test_modes.py
 test/test_models/test_three_ds_redirect_data_v3.py
 test/test_models/test_update_order_request.py
+test/test_models/test_ux_settings_model.py
 test/test_models/test_verify_authorization_response.py
 test/test_paths/__init__.py
 test/test_paths/test_api_installmentplans/__init__.py
 test/test_paths/test_api_installmentplans/test_post.py
 test/test_paths/test_api_installmentplans_check_eligibility/__init__.py
 test/test_paths/test_api_installmentplans_check_eligibility/test_post.py
 test/test_paths/test_api_installmentplans_initiate/__init__.py
```

### Comparing `splitit-web-python-sdk-2.0.0/test/test_installment_plan_api_post.py` & `splitit-web-python-sdk-2.1.0/test/test_installment_plan_api_post.py`

 * *Files 18% similar despite different names*

```diff
@@ -54,10 +54,43 @@
                 },
                 "RedirectUrls": {}
             }
         )
         print(response)
         assert response is not None, "Received null response"
 
+    def test_post_with_int_total_amount(self):
+        """Test case for post but with the PlanData.TotalAmount as an int to
+        ensure NumberSchema can handle both float/int
+        """
+        response = self.api.installment_plan.post(
+            header_params={
+                'X-Splitit-IdempotencyKey': str(uuid.uuid4()),
+            },
+            body={
+                "AutoCapture": True,
+                "Attempt3dSecure": True,
+                "Shopper": {
+                    "Email": "fake@email.com"
+                },
+                "BillingAddress": {
+                    "AddressLine1": "144 Union St",
+                    "City": "Brooklyn",
+                    "State": "North Dakota",
+                    "Zip": "11231",
+                    "Country": "United States",
+                },
+                "PlanData": {
+                    "TotalAmount": 10,
+                    "NumberOfInstallements": 10,
+                    "Currency": "USD",
+                    "PurchaseMethod": "InStore",
+                },
+                "RedirectUrls": {}
+            }
+        )
+        print(response)
+        assert response is not None, "Received null response"
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `splitit-web-python-sdk-2.0.0/test/test_models/test_check_installments_eligibility_request.py` & `splitit-web-python-sdk-2.1.0/test/test_models/test_check_installments_eligibility_request.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/test/test_models/test_initiate_redirection_endpoints_model.py` & `splitit-web-python-sdk-2.1.0/test/test_models/test_initiate_redirection_endpoints_model.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_cancel_response.py` & `splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_cancel_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_create_response.py` & `splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_create_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_initiate_request.py` & `splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_initiate_request.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_refund_response.py` & `splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_refund_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_search_response.py` & `splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_search_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_update_request_by_identifier.py` & `splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_update_request_by_identifier.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/test/test_models/test_installment_plan_update_response.py` & `splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_update_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/test/test_models/test_installments_eligibility_response.py` & `splitit-web-python-sdk-2.1.0/test/test_models/test_installments_eligibility_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/test/test_models/test_search_installment_plan_response_item.py` & `splitit-web-python-sdk-2.1.0/test/test_models/test_search_installment_plan_response_item.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/test/test_paths/__init__.py` & `splitit-web-python-sdk-2.1.0/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans/test_post.py` & `splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_initiate/test_post.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import splitit_client
-from splitit_client.paths.api_installmentplans import post
+from splitit_client.paths.api_installmentplans_initiate import post
 from splitit_client import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiInstallmentplans(ApiTestMixin, unittest.TestCase):
+class TestApiInstallmentplansInitiate(ApiTestMixin, unittest.TestCase):
     """
-    ApiInstallmentplans unit test stubs
+    ApiInstallmentplansInitiate unit test stubs
     """
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
```

### Comparing `splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_check_eligibility/test_post.py` & `splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_check_eligibility/test_post.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
```

### Comparing `splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_initiate/test_post.py` & `splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans/test_post.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import splitit_client
-from splitit_client.paths.api_installmentplans_initiate import post
+from splitit_client.paths.api_installmentplans import post
 from splitit_client import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiInstallmentplansInitiate(ApiTestMixin, unittest.TestCase):
+class TestApiInstallmentplans(ApiTestMixin, unittest.TestCase):
     """
-    ApiInstallmentplansInitiate unit test stubs
+    ApiInstallmentplans unit test stubs
     """
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
```

### Comparing `splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number/test_get.py` & `splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_search/test_get.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import splitit_client
-from splitit_client.paths.api_installmentplans_installment_plan_number import get
+from splitit_client.paths.api_installmentplans_search import get
 from splitit_client import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiInstallmentplansInstallmentPlanNumber(ApiTestMixin, unittest.TestCase):
+class TestApiInstallmentplansSearch(ApiTestMixin, unittest.TestCase):
     """
-    ApiInstallmentplansInstallmentPlanNumber unit test stubs
+    ApiInstallmentplansSearch unit test stubs
     """
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
```

### Comparing `splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number_cancel/test_post.py` & `splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_cancel/test_post.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
```

### Comparing `splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number_refund/test_post.py` & `splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_refund/test_post.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
```

### Comparing `splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number_updateorder/test_put.py` & `splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number/test_get.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import splitit_client
-from splitit_client.paths.api_installmentplans_installment_plan_number_updateorder import put
+from splitit_client.paths.api_installmentplans_installment_plan_number import get
 from splitit_client import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiInstallmentplansInstallmentPlanNumberUpdateorder(ApiTestMixin, unittest.TestCase):
+class TestApiInstallmentplansInstallmentPlanNumber(ApiTestMixin, unittest.TestCase):
     """
-    ApiInstallmentplansInstallmentPlanNumberUpdateorder unit test stubs
+    ApiInstallmentplansInstallmentPlanNumber unit test stubs
     """
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
@@ -33,18 +36,10 @@
 
 
 
 
 
 
 
-
-
-
-
-
-
-
-
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_installment_plan_number_verifyauthorization/test_get.py` & `splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_verifyauthorization/test_get.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
```

### Comparing `splitit-web-python-sdk-2.0.0/test/test_paths/test_api_installmentplans_search/test_get.py` & `splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_updateorder/test_put.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # coding: utf-8
 
 """
+    splitit-web-api-v3
 
+    Splitit's Web API
 
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import splitit_client
-from splitit_client.paths.api_installmentplans_search import get
+from splitit_client.paths.api_installmentplans_updateorder import put
 from splitit_client import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiInstallmentplansSearch(ApiTestMixin, unittest.TestCase):
+class TestApiInstallmentplansUpdateorder(ApiTestMixin, unittest.TestCase):
     """
-    ApiInstallmentplansSearch unit test stubs
+    ApiInstallmentplansUpdateorder unit test stubs
     """
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
@@ -33,10 +36,18 @@
 
 
 
 
 
 
 
+
+
+
+
+
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

