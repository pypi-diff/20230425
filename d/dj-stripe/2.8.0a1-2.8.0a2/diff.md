# Comparing `tmp/dj_stripe-2.8.0a1.tar.gz` & `tmp/dj_stripe-2.8.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_stripe-2.8.0a1.tar", max compression
+gzip compressed data, was "dj_stripe-2.8.0a2.tar", max compression
```

## Comparing `dj_stripe-2.8.0a1.tar` & `dj_stripe-2.8.0a2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1084 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a1/LICENSE
--rw-r--r--   0        0        0        0 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a1/djstripe/__init__.py
--rw-r--r--   0        0        0      130 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a1/djstripe/admin/__init__.py
--rw-r--r--   0        0        0     4219 2023-04-18 16:12:01.671673 dj_stripe-2.8.0a1/djstripe/admin/actions.py
--rw-r--r--   0        0        0    26470 2023-04-22 14:17:48.303372 dj_stripe-2.8.0a1/djstripe/admin/admin.py
--rw-r--r--   0        0        0     2390 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a1/djstripe/admin/admin_inline.py
--rw-r--r--   0        0        0     2861 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a1/djstripe/admin/filters.py
--rw-r--r--   0        0        0     9552 2023-04-22 14:18:37.516991 dj_stripe-2.8.0a1/djstripe/admin/forms.py
--rw-r--r--   0        0        0      880 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a1/djstripe/admin/utils.py
--rw-r--r--   0        0        0     4645 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a1/djstripe/admin/views.py
--rw-r--r--   0        0        0      766 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a1/djstripe/apps.py
--rw-r--r--   0        0        0    14315 2023-04-22 14:18:37.516991 dj_stripe-2.8.0a1/djstripe/checks.py
--rw-r--r--   0        0        0    27096 2023-04-22 14:18:37.516991 dj_stripe-2.8.0a1/djstripe/enums.py
--rw-r--r--   0        0        0    16030 2023-04-22 14:18:37.496991 dj_stripe-2.8.0a1/djstripe/event_handlers.py
--rw-r--r--   0        0        0      633 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a1/djstripe/exceptions.py
--rw-r--r--   0        0        0     6138 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a1/djstripe/fields.py
--rw-r--r--   0        0        0    17624 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a1/djstripe/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19987 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a1/djstripe/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a1/djstripe/management/__init__.py
--rw-r--r--   0        0        0        0 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a1/djstripe/management/commands/__init__.py
--rw-r--r--   0        0        0      271 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a1/djstripe/management/commands/djstripe_clear_expired_idempotency_keys.py
--rw-r--r--   0        0        0     1016 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a1/djstripe/management/commands/djstripe_init_customers.py
--rw-r--r--   0        0        0     4089 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a1/djstripe/management/commands/djstripe_process_events.py
--rw-r--r--   0        0        0      861 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a1/djstripe/management/commands/djstripe_sync_customers.py
--rw-r--r--   0        0        0    22901 2023-04-22 14:18:37.516991 dj_stripe-2.8.0a1/djstripe/management/commands/djstripe_sync_models.py
--rw-r--r--   0        0        0     2898 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a1/djstripe/management/commands/djstripe_update_invoiceitem_ids.py
--rw-r--r--   0        0        0     3267 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a1/djstripe/managers.py
--rw-r--r--   0        0        0   229743 2023-04-22 14:18:37.516991 dj_stripe-2.8.0a1/djstripe/migrations/0001_initial.py
--rw-r--r--   0        0        0    12750 2023-04-22 14:18:37.516991 dj_stripe-2.8.0a1/djstripe/migrations/0008_2_5.py
--rw-r--r--   0        0        0    14990 2023-04-22 14:18:37.516991 dj_stripe-2.8.0a1/djstripe/migrations/0009_2_6.py
--rw-r--r--   0        0        0      471 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a1/djstripe/migrations/0010_alter_customer_balance.py
--rw-r--r--   0        0        0    20038 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a1/djstripe/migrations/0011_2_7.py
--rw-r--r--   0        0        0    30983 2023-04-25 00:50:38.384803 dj_stripe-2.8.0a1/djstripe/migrations/0012_2_8.py
--rw-r--r--   0        0        0        0 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a1/djstripe/migrations/__init__.py
--rw-r--r--   0        0        0     1059 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a1/djstripe/migrations/sql/migrate_mysql_backward.sql
--rw-r--r--   0        0        0     1085 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a1/djstripe/migrations/sql/migrate_mysql_forward.sql
--rw-r--r--   0        0        0     1446 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a1/djstripe/migrations/sql/migrate_postgresql_backward.sql
--rw-r--r--   0        0        0     1216 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a1/djstripe/migrations/sql/migrate_postgresql_forward.sql
--rw-r--r--   0        0        0     5867 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a1/djstripe/migrations/sql/migrate_sqlite_backward.sql
--rw-r--r--   0        0        0     3269 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a1/djstripe/migrations/sql/migrate_sqlite_forward.sql
--rw-r--r--   0        0        0     1971 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a1/djstripe/mixins.py
--rw-r--r--   0        0        0     2153 2023-04-22 14:18:37.493658 dj_stripe-2.8.0a1/djstripe/models/__init__.py
--rw-r--r--   0        0        0    10318 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a1/djstripe/models/account.py
--rw-r--r--   0        0        0     4290 2023-04-20 18:31:54.175370 dj_stripe-2.8.0a1/djstripe/models/api.py
--rw-r--r--   0        0        0    40571 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a1/djstripe/models/base.py
--rw-r--r--   0        0        0   103701 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a1/djstripe/models/billing.py
--rw-r--r--   0        0        0     7709 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a1/djstripe/models/checkout.py
--rw-r--r--   0        0        0    13440 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a1/djstripe/models/connect.py
--rw-r--r--   0        0        0    87807 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a1/djstripe/models/core.py
--rw-r--r--   0        0        0        0 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a1/djstripe/models/fraud.py
--rw-r--r--   0        0        0     1340 2023-04-22 14:18:37.493658 dj_stripe-2.8.0a1/djstripe/models/identity.py
--rw-r--r--   0        0        0     8809 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a1/djstripe/models/orders.py
--rw-r--r--   0        0        0    42070 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a1/djstripe/models/payment_methods.py
--rw-r--r--   0        0        0     1558 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a1/djstripe/models/sigma.py
--rw-r--r--   0        0        0    11902 2023-04-22 15:33:15.352960 dj_stripe-2.8.0a1/djstripe/models/webhooks.py
--rw-r--r--   0        0        0     8205 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a1/djstripe/settings.py
--rw-r--r--   0        0        0     8324 2023-04-22 14:18:37.503658 dj_stripe-2.8.0a1/djstripe/signals.py
--rw-r--r--   0        0        0      579 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a1/djstripe/sync.py
--rw-r--r--   0        0        0      251 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a1/djstripe/templates/djstripe/admin/add_form.html
--rw-r--r--   0        0        0      984 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a1/djstripe/templates/djstripe/admin/change_form.html
--rw-r--r--   0        0        0     2790 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a1/djstripe/templates/djstripe/admin/confirm_action.html
--rw-r--r--   0        0        0      250 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a1/djstripe/templates/djstripe/admin/webhook_endpoint/add_form.html
--rw-r--r--   0        0        0      227 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a1/djstripe/templates/djstripe/admin/webhook_endpoint/change_form.html
--rw-r--r--   0        0        0     1251 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a1/djstripe/templates/djstripe/admin/webhook_endpoint/delete_confirmation.html
--rw-r--r--   0        0        0      679 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a1/djstripe/urls.py
--rw-r--r--   0        0        0     3362 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a1/djstripe/utils.py
--rw-r--r--   0        0        0     2158 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a1/djstripe/views.py
--rw-r--r--   0        0        0     3045 2022-10-18 02:15:05.683778 dj_stripe-2.8.0a1/djstripe/webhooks.py
--rw-r--r--   0        0        0     3634 2023-04-22 14:16:57.269741 dj_stripe-2.8.0a1/docs/README.md
--rw-r--r--   0        0        0     4696 2023-04-25 00:51:23.791737 dj_stripe-2.8.0a1/pyproject.toml
--rw-r--r--   0        0        0     5077 1970-01-01 00:00:00.000000 dj_stripe-2.8.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a2/LICENSE
+-rw-r--r--   0        0        0        0 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a2/djstripe/__init__.py
+-rw-r--r--   0        0        0      130 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a2/djstripe/admin/__init__.py
+-rw-r--r--   0        0        0     4219 2023-04-18 16:12:01.671673 dj_stripe-2.8.0a2/djstripe/admin/actions.py
+-rw-r--r--   0        0        0    26470 2023-04-22 14:17:48.303372 dj_stripe-2.8.0a2/djstripe/admin/admin.py
+-rw-r--r--   0        0        0     2390 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a2/djstripe/admin/admin_inline.py
+-rw-r--r--   0        0        0     2861 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a2/djstripe/admin/filters.py
+-rw-r--r--   0        0        0     9552 2023-04-22 14:18:37.516991 dj_stripe-2.8.0a2/djstripe/admin/forms.py
+-rw-r--r--   0        0        0      880 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a2/djstripe/admin/utils.py
+-rw-r--r--   0        0        0     4645 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a2/djstripe/admin/views.py
+-rw-r--r--   0        0        0      766 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a2/djstripe/apps.py
+-rw-r--r--   0        0        0    14315 2023-04-22 14:18:37.516991 dj_stripe-2.8.0a2/djstripe/checks.py
+-rw-r--r--   0        0        0    27096 2023-04-22 14:18:37.516991 dj_stripe-2.8.0a2/djstripe/enums.py
+-rw-r--r--   0        0        0    16030 2023-04-22 14:18:37.496991 dj_stripe-2.8.0a2/djstripe/event_handlers.py
+-rw-r--r--   0        0        0      633 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a2/djstripe/exceptions.py
+-rw-r--r--   0        0        0     6138 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a2/djstripe/fields.py
+-rw-r--r--   0        0        0    17624 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a2/djstripe/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19987 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a2/djstripe/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a2/djstripe/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a2/djstripe/management/commands/__init__.py
+-rw-r--r--   0        0        0      271 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a2/djstripe/management/commands/djstripe_clear_expired_idempotency_keys.py
+-rw-r--r--   0        0        0     1016 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a2/djstripe/management/commands/djstripe_init_customers.py
+-rw-r--r--   0        0        0     4089 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a2/djstripe/management/commands/djstripe_process_events.py
+-rw-r--r--   0        0        0      861 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a2/djstripe/management/commands/djstripe_sync_customers.py
+-rw-r--r--   0        0        0    22901 2023-04-22 14:18:37.516991 dj_stripe-2.8.0a2/djstripe/management/commands/djstripe_sync_models.py
+-rw-r--r--   0        0        0     2898 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a2/djstripe/management/commands/djstripe_update_invoiceitem_ids.py
+-rw-r--r--   0        0        0     3267 2022-10-18 02:15:05.677111 dj_stripe-2.8.0a2/djstripe/managers.py
+-rw-r--r--   0        0        0   229743 2023-04-22 14:18:37.516991 dj_stripe-2.8.0a2/djstripe/migrations/0001_initial.py
+-rw-r--r--   0        0        0    12750 2023-04-22 14:18:37.516991 dj_stripe-2.8.0a2/djstripe/migrations/0008_2_5.py
+-rw-r--r--   0        0        0    14990 2023-04-22 14:18:37.516991 dj_stripe-2.8.0a2/djstripe/migrations/0009_2_6.py
+-rw-r--r--   0        0        0      471 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a2/djstripe/migrations/0010_alter_customer_balance.py
+-rw-r--r--   0        0        0    20038 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a2/djstripe/migrations/0011_2_7.py
+-rw-r--r--   0        0        0    30983 2023-04-25 00:53:03.378988 dj_stripe-2.8.0a2/djstripe/migrations/0012_2_8.py
+-rw-r--r--   0        0        0        0 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a2/djstripe/migrations/__init__.py
+-rw-r--r--   0        0        0     1059 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a2/djstripe/migrations/sql/migrate_mysql_backward.sql
+-rw-r--r--   0        0        0     1085 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a2/djstripe/migrations/sql/migrate_mysql_forward.sql
+-rw-r--r--   0        0        0     1446 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a2/djstripe/migrations/sql/migrate_postgresql_backward.sql
+-rw-r--r--   0        0        0     1216 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a2/djstripe/migrations/sql/migrate_postgresql_forward.sql
+-rw-r--r--   0        0        0     5867 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a2/djstripe/migrations/sql/migrate_sqlite_backward.sql
+-rw-r--r--   0        0        0     3269 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a2/djstripe/migrations/sql/migrate_sqlite_forward.sql
+-rw-r--r--   0        0        0     1971 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a2/djstripe/mixins.py
+-rw-r--r--   0        0        0     2153 2023-04-22 14:18:37.493658 dj_stripe-2.8.0a2/djstripe/models/__init__.py
+-rw-r--r--   0        0        0    10318 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a2/djstripe/models/account.py
+-rw-r--r--   0        0        0     4290 2023-04-20 18:31:54.175370 dj_stripe-2.8.0a2/djstripe/models/api.py
+-rw-r--r--   0        0        0    40571 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a2/djstripe/models/base.py
+-rw-r--r--   0        0        0   103701 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a2/djstripe/models/billing.py
+-rw-r--r--   0        0        0     7709 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a2/djstripe/models/checkout.py
+-rw-r--r--   0        0        0    13440 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a2/djstripe/models/connect.py
+-rw-r--r--   0        0        0    87807 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a2/djstripe/models/core.py
+-rw-r--r--   0        0        0        0 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a2/djstripe/models/fraud.py
+-rw-r--r--   0        0        0     1340 2023-04-22 14:18:37.493658 dj_stripe-2.8.0a2/djstripe/models/identity.py
+-rw-r--r--   0        0        0     8809 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a2/djstripe/models/orders.py
+-rw-r--r--   0        0        0    42070 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a2/djstripe/models/payment_methods.py
+-rw-r--r--   0        0        0     1558 2023-04-22 14:18:37.520325 dj_stripe-2.8.0a2/djstripe/models/sigma.py
+-rw-r--r--   0        0        0    11902 2023-04-22 15:33:15.352960 dj_stripe-2.8.0a2/djstripe/models/webhooks.py
+-rw-r--r--   0        0        0     8205 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a2/djstripe/settings.py
+-rw-r--r--   0        0        0     8324 2023-04-22 14:18:37.503658 dj_stripe-2.8.0a2/djstripe/signals.py
+-rw-r--r--   0        0        0      579 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a2/djstripe/sync.py
+-rw-r--r--   0        0        0      251 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a2/djstripe/templates/djstripe/admin/add_form.html
+-rw-r--r--   0        0        0      984 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a2/djstripe/templates/djstripe/admin/change_form.html
+-rw-r--r--   0        0        0     2790 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a2/djstripe/templates/djstripe/admin/confirm_action.html
+-rw-r--r--   0        0        0      250 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a2/djstripe/templates/djstripe/admin/webhook_endpoint/add_form.html
+-rw-r--r--   0        0        0      227 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a2/djstripe/templates/djstripe/admin/webhook_endpoint/change_form.html
+-rw-r--r--   0        0        0     1251 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a2/djstripe/templates/djstripe/admin/webhook_endpoint/delete_confirmation.html
+-rw-r--r--   0        0        0      679 2022-10-18 02:15:05.680445 dj_stripe-2.8.0a2/djstripe/urls.py
+-rw-r--r--   0        0        0     3362 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a2/djstripe/utils.py
+-rw-r--r--   0        0        0     2158 2023-04-18 16:12:01.675006 dj_stripe-2.8.0a2/djstripe/views.py
+-rw-r--r--   0        0        0     3045 2022-10-18 02:15:05.683778 dj_stripe-2.8.0a2/djstripe/webhooks.py
+-rw-r--r--   0        0        0     3634 2023-04-22 14:16:57.269741 dj_stripe-2.8.0a2/docs/README.md
+-rw-r--r--   0        0        0     4696 2023-04-25 00:53:15.419058 dj_stripe-2.8.0a2/pyproject.toml
+-rw-r--r--   0        0        0     5077 1970-01-01 00:00:00.000000 dj_stripe-2.8.0a2/PKG-INFO
```

### Comparing `dj_stripe-2.8.0a1/LICENSE` & `dj_stripe-2.8.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/admin/actions.py` & `dj_stripe-2.8.0a2/djstripe/admin/actions.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/admin/admin.py` & `dj_stripe-2.8.0a2/djstripe/admin/admin.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/admin/admin_inline.py` & `dj_stripe-2.8.0a2/djstripe/admin/admin_inline.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/admin/filters.py` & `dj_stripe-2.8.0a2/djstripe/admin/filters.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/admin/forms.py` & `dj_stripe-2.8.0a2/djstripe/admin/forms.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/admin/utils.py` & `dj_stripe-2.8.0a2/djstripe/admin/utils.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/admin/views.py` & `dj_stripe-2.8.0a2/djstripe/admin/views.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/apps.py` & `dj_stripe-2.8.0a2/djstripe/apps.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/checks.py` & `dj_stripe-2.8.0a2/djstripe/checks.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/enums.py` & `dj_stripe-2.8.0a2/djstripe/enums.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/event_handlers.py` & `dj_stripe-2.8.0a2/djstripe/event_handlers.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/exceptions.py` & `dj_stripe-2.8.0a2/djstripe/exceptions.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/fields.py` & `dj_stripe-2.8.0a2/djstripe/fields.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/locale/fr/LC_MESSAGES/django.po` & `dj_stripe-2.8.0a2/djstripe/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/locale/ru/LC_MESSAGES/django.po` & `dj_stripe-2.8.0a2/djstripe/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/management/commands/djstripe_init_customers.py` & `dj_stripe-2.8.0a2/djstripe/management/commands/djstripe_init_customers.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/management/commands/djstripe_process_events.py` & `dj_stripe-2.8.0a2/djstripe/management/commands/djstripe_process_events.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/management/commands/djstripe_sync_customers.py` & `dj_stripe-2.8.0a2/djstripe/management/commands/djstripe_sync_customers.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/management/commands/djstripe_sync_models.py` & `dj_stripe-2.8.0a2/djstripe/management/commands/djstripe_sync_models.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/management/commands/djstripe_update_invoiceitem_ids.py` & `dj_stripe-2.8.0a2/djstripe/management/commands/djstripe_update_invoiceitem_ids.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/managers.py` & `dj_stripe-2.8.0a2/djstripe/managers.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/migrations/0001_initial.py` & `dj_stripe-2.8.0a2/djstripe/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/migrations/0008_2_5.py` & `dj_stripe-2.8.0a2/djstripe/migrations/0008_2_5.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/migrations/0009_2_6.py` & `dj_stripe-2.8.0a2/djstripe/migrations/0009_2_6.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/migrations/0011_2_7.py` & `dj_stripe-2.8.0a2/djstripe/migrations/0011_2_7.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/migrations/0012_2_8.py` & `dj_stripe-2.8.0a2/djstripe/migrations/0012_2_8.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import djstripe.enums
 import djstripe.fields
 
 
 class Migration(migrations.Migration):
     dependencies = [
-        ("djstripe", "0012_2_8"),
+        ("djstripe", "0011_2_7"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="InvoiceOrLineItem",
             fields=[
                 (
```

### Comparing `dj_stripe-2.8.0a1/djstripe/migrations/sql/migrate_mysql_backward.sql` & `dj_stripe-2.8.0a2/djstripe/migrations/sql/migrate_mysql_backward.sql`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/migrations/sql/migrate_mysql_forward.sql` & `dj_stripe-2.8.0a2/djstripe/migrations/sql/migrate_mysql_forward.sql`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/migrations/sql/migrate_postgresql_backward.sql` & `dj_stripe-2.8.0a2/djstripe/migrations/sql/migrate_postgresql_backward.sql`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/migrations/sql/migrate_postgresql_forward.sql` & `dj_stripe-2.8.0a2/djstripe/migrations/sql/migrate_postgresql_forward.sql`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/migrations/sql/migrate_sqlite_backward.sql` & `dj_stripe-2.8.0a2/djstripe/migrations/sql/migrate_sqlite_backward.sql`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/migrations/sql/migrate_sqlite_forward.sql` & `dj_stripe-2.8.0a2/djstripe/migrations/sql/migrate_sqlite_forward.sql`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/mixins.py` & `dj_stripe-2.8.0a2/djstripe/mixins.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/models/__init__.py` & `dj_stripe-2.8.0a2/djstripe/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/models/account.py` & `dj_stripe-2.8.0a2/djstripe/models/account.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/models/api.py` & `dj_stripe-2.8.0a2/djstripe/models/api.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/models/base.py` & `dj_stripe-2.8.0a2/djstripe/models/base.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/models/billing.py` & `dj_stripe-2.8.0a2/djstripe/models/billing.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/models/checkout.py` & `dj_stripe-2.8.0a2/djstripe/models/checkout.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/models/connect.py` & `dj_stripe-2.8.0a2/djstripe/models/connect.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/models/core.py` & `dj_stripe-2.8.0a2/djstripe/models/core.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/models/identity.py` & `dj_stripe-2.8.0a2/djstripe/models/identity.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/models/orders.py` & `dj_stripe-2.8.0a2/djstripe/models/orders.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/models/payment_methods.py` & `dj_stripe-2.8.0a2/djstripe/models/payment_methods.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/models/sigma.py` & `dj_stripe-2.8.0a2/djstripe/models/sigma.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/models/webhooks.py` & `dj_stripe-2.8.0a2/djstripe/models/webhooks.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/settings.py` & `dj_stripe-2.8.0a2/djstripe/settings.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/signals.py` & `dj_stripe-2.8.0a2/djstripe/signals.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/sync.py` & `dj_stripe-2.8.0a2/djstripe/sync.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/templates/djstripe/admin/change_form.html` & `dj_stripe-2.8.0a2/djstripe/templates/djstripe/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/templates/djstripe/admin/confirm_action.html` & `dj_stripe-2.8.0a2/djstripe/templates/djstripe/admin/confirm_action.html`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/templates/djstripe/admin/webhook_endpoint/delete_confirmation.html` & `dj_stripe-2.8.0a2/djstripe/templates/djstripe/admin/webhook_endpoint/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/urls.py` & `dj_stripe-2.8.0a2/djstripe/urls.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/utils.py` & `dj_stripe-2.8.0a2/djstripe/utils.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/views.py` & `dj_stripe-2.8.0a2/djstripe/views.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/djstripe/webhooks.py` & `dj_stripe-2.8.0a2/djstripe/webhooks.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/docs/README.md` & `dj_stripe-2.8.0a2/docs/README.md`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.0a1/pyproject.toml` & `dj_stripe-2.8.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dj-stripe"
-version = "2.8.0-alpha.1"
+version = "2.8.0-alpha.2"
 description = "Django + Stripe made easy"
 license = "MIT"
 authors = [
     "Alexander Kavanaugh <alex@kavdev.io>",
     "Jerome Leclanche <jerome@leclan.ch>",
 ]
 readme = "docs/README.md"
```

### Comparing `dj_stripe-2.8.0a1/PKG-INFO` & `dj_stripe-2.8.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-stripe
-Version: 2.8.0a1
+Version: 2.8.0a2
 Summary: Django + Stripe made easy
 Home-page: https://dj-stripe.dev
 License: MIT
 Author: Alexander Kavanaugh
 Author-email: alex@kavdev.io
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dj-stripe Version: 2.8.0a1 Summary: Django + Stripe
+Metadata-Version: 2.1 Name: dj-stripe Version: 2.8.0a2 Summary: Django + Stripe
 made easy Home-page: https://dj-stripe.dev License: MIT Author: Alexander
 Kavanaugh Author-email: alex@kavdev.io Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Framework :: Django Classifier: Framework ::
 Django :: 3.2 Classifier: Framework :: Django :: 4.0 Classifier: Framework ::
 Django :: 4.1 Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

