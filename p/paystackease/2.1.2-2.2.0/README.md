# Comparing `tmp/paystackease-2.1.2.tar.gz` & `tmp/paystackease-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paystackease-2.1.2.tar", max compression
+gzip compressed data, was "paystackease-2.2.0.tar", max compression
```

## Comparing `paystackease-2.1.2.tar` & `paystackease-2.2.0.tar`

### file list

```diff
@@ -1,70 +1,72 @@
--rw-r--r--   0        0        0     1069 2024-05-23 09:38:38.117702 paystackease-2.1.2/LICENSE
--rw-r--r--   0        0        0     4802 2024-05-23 09:38:38.117702 paystackease-2.1.2/README.md
--rw-r--r--   0        0        0     1767 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/__init__.py
--rw-r--r--   0        0        0     5713 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apaystack.py
--rw-r--r--   0        0        0      988 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/__init__.py
--rw-r--r--   0        0        0     2137 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/aapple_pay.py
--rw-r--r--   0        0        0     4355 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/abulk_charges.py
--rw-r--r--   0        0        0     5820 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/acharges.py
--rw-r--r--   0        0        0     6762 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/acustomers.py
--rw-r--r--   0        0        0     9269 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/adedicated_virtual_accounts.py
--rw-r--r--   0        0        0     7980 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/adisputes.py
--rw-r--r--   0        0        0     1146 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/aintegration.py
--rw-r--r--   0        0        0     4327 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/amiscellaneous.py
--rw-r--r--   0        0        0     5644 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/apayment_pages.py
--rw-r--r--   0        0        0     9834 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/apayment_requests.py
--rw-r--r--   0        0        0     4547 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/aplans.py
--rw-r--r--   0        0        0     4253 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/aproducts.py
--rw-r--r--   0        0        0     3233 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/arefund.py
--rw-r--r--   0        0        0     3250 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/asettlements.py
--rw-r--r--   0        0        0     6232 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/asubaccounts.py
--rw-r--r--   0        0        0     4396 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/asubscriptions.py
--rw-r--r--   0        0        0     5399 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/aterminal.py
--rw-r--r--   0        0        0     5844 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/atransaction_splits.py
--rw-r--r--   0        0        0    12559 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/atransactions.py
--rw-r--r--   0        0        0     5281 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/atransfer_recipients.py
--rw-r--r--   0        0        0     4822 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/atransfers.py
--rw-r--r--   0        0        0     2717 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/atransfers_control.py
--rw-r--r--   0        0        0     2802 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/async_apis/averification.py
--rw-r--r--   0        0        0        0 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/__init__.py
--rw-r--r--   0        0        0     2084 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/apple_pay.py
--rw-r--r--   0        0        0     4263 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/bulk_charges.py
--rw-r--r--   0        0        0     5724 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/charges.py
--rw-r--r--   0        0        0     6663 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/customers.py
--rw-r--r--   0        0        0     9141 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/dedicated_virtual_accounts.py
--rw-r--r--   0        0        0     7864 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/disputes.py
--rw-r--r--   0        0        0     1110 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/integration.py
--rw-r--r--   0        0        0     4283 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/miscellaneous.py
--rw-r--r--   0        0        0     5560 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/payment_pages.py
--rw-r--r--   0        0        0     9706 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/payment_requests.py
--rw-r--r--   0        0        0     4479 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/plans.py
--rw-r--r--   0        0        0     4185 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/products.py
--rw-r--r--   0        0        0     3177 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/refund.py
--rw-r--r--   0        0        0     3214 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/settlements.py
--rw-r--r--   0        0        0     6158 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/subaccounts.py
--rw-r--r--   0        0        0     4305 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/subscriptions.py
--rw-r--r--   0        0        0     5285 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/terminal.py
--rw-r--r--   0        0        0     5747 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/transaction_splits.py
--rw-r--r--   0        0        0    12421 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/transactions.py
--rw-r--r--   0        0        0     5189 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/transfer_recipients.py
--rw-r--r--   0        0        0     4730 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/transfers.py
--rw-r--r--   0        0        0     2625 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/transfers_control.py
--rw-r--r--   0        0        0     2746 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/apis/sync_apis/verification.py
--rw-r--r--   0        0        0      618 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/core/__init__.py
--rw-r--r--   0        0        0     3805 2024-05-23 09:38:38.121702 paystackease-2.1.2/paystackease/core/_api_base.py
--rw-r--r--   0        0        0     6727 2024-05-23 09:38:38.125702 paystackease-2.1.2/paystackease/core/_api_base_client.py
--rw-r--r--   0        0        0     4680 2024-05-23 09:38:38.125702 paystackease-2.1.2/paystackease/core/_api_client_requests.py
--rw-r--r--   0        0        0      660 2024-05-23 09:38:38.125702 paystackease-2.1.2/paystackease/core/_api_client_response.py
--rw-r--r--   0        0        0     5007 2024-05-23 09:38:38.125702 paystackease-2.1.2/paystackease/core/_api_errors.py
--rw-r--r--   0        0        0     1463 2024-05-23 09:38:38.125702 paystackease-2.1.2/paystackease/core/_webhook.py
--rw-r--r--   0        0        0      552 2024-05-23 09:38:38.125702 paystackease-2.1.2/paystackease/helpers/__init__.py
--rw-r--r--   0        0        0      742 2024-05-23 09:38:38.125702 paystackease-2.1.2/paystackease/helpers/convert.py
--rw-r--r--   0        0        0     3566 2024-05-23 09:38:38.125702 paystackease-2.1.2/paystackease/helpers/tool_kit.py
--rw-r--r--   0        0        0        0 2024-05-23 09:38:38.125702 paystackease-2.1.2/paystackease/metadata/__init__.py
--rw-r--r--   0        0        0       98 2024-05-23 09:38:38.125702 paystackease-2.1.2/paystackease/metadata/__version__.py
--rw-r--r--   0        0        0     3074 2024-05-23 09:38:38.125702 paystackease-2.1.2/paystackease/paystack.py
--rw-r--r--   0        0        0        0 2024-05-23 09:38:38.125702 paystackease-2.1.2/paystackease/utils/__init__.py
--rw-r--r--   0        0        0      193 2024-05-23 09:38:38.125702 paystackease-2.1.2/paystackease/utils/_compact.py
--rw-r--r--   0        0        0     2259 2024-05-23 09:38:39.673714 paystackease-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 paystackease-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-28 02:58:06.877679 paystackease-2.2.0/LICENSE
+-rw-r--r--   0        0        0     4802 2024-05-28 02:58:06.877679 paystackease-2.2.0/README.md
+-rw-r--r--   0        0        0     1767 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/__init__.py
+-rw-r--r--   0        0        0     4841 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apaystack.py
+-rw-r--r--   0        0        0      988 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/__init__.py
+-rw-r--r--   0        0        0     2137 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/aapple_pay.py
+-rw-r--r--   0        0        0     4355 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/abulk_charges.py
+-rw-r--r--   0        0        0     5820 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/acharges.py
+-rw-r--r--   0        0        0     6762 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/acustomers.py
+-rw-r--r--   0        0        0     9269 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/adedicated_virtual_accounts.py
+-rw-r--r--   0        0        0     7980 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/adisputes.py
+-rw-r--r--   0        0        0     1146 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/aintegration.py
+-rw-r--r--   0        0        0     4327 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/amiscellaneous.py
+-rw-r--r--   0        0        0     5644 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/apayment_pages.py
+-rw-r--r--   0        0        0     9834 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/apayment_requests.py
+-rw-r--r--   0        0        0     4547 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/aplans.py
+-rw-r--r--   0        0        0     4253 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/aproducts.py
+-rw-r--r--   0        0        0     3233 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/arefund.py
+-rw-r--r--   0        0        0     3250 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/asettlements.py
+-rw-r--r--   0        0        0     6232 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/asubaccounts.py
+-rw-r--r--   0        0        0     4396 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/asubscriptions.py
+-rw-r--r--   0        0        0     5399 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/aterminal.py
+-rw-r--r--   0        0        0     5844 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/atransaction_splits.py
+-rw-r--r--   0        0        0    12559 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/atransactions.py
+-rw-r--r--   0        0        0     5281 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/atransfer_recipients.py
+-rw-r--r--   0        0        0     4822 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/atransfers.py
+-rw-r--r--   0        0        0     2717 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/atransfers_control.py
+-rw-r--r--   0        0        0     2802 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/averification.py
+-rw-r--r--   0        0        0        0 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/__init__.py
+-rw-r--r--   0        0        0     2084 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/apple_pay.py
+-rw-r--r--   0        0        0     4263 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/bulk_charges.py
+-rw-r--r--   0        0        0     5724 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/charges.py
+-rw-r--r--   0        0        0     6663 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/customers.py
+-rw-r--r--   0        0        0     9141 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/dedicated_virtual_accounts.py
+-rw-r--r--   0        0        0     7864 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/disputes.py
+-rw-r--r--   0        0        0     1110 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/integration.py
+-rw-r--r--   0        0        0     4283 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/miscellaneous.py
+-rw-r--r--   0        0        0     5560 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/payment_pages.py
+-rw-r--r--   0        0        0     9706 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/payment_requests.py
+-rw-r--r--   0        0        0     4479 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/plans.py
+-rw-r--r--   0        0        0     4185 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/products.py
+-rw-r--r--   0        0        0     3177 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/refund.py
+-rw-r--r--   0        0        0     3214 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/settlements.py
+-rw-r--r--   0        0        0     6158 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/subaccounts.py
+-rw-r--r--   0        0        0     4305 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/subscriptions.py
+-rw-r--r--   0        0        0     5285 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/terminal.py
+-rw-r--r--   0        0        0     5747 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/transaction_splits.py
+-rw-r--r--   0        0        0    12421 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/transactions.py
+-rw-r--r--   0        0        0     5189 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/transfer_recipients.py
+-rw-r--r--   0        0        0     4730 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/transfers.py
+-rw-r--r--   0        0        0     2625 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/transfers_control.py
+-rw-r--r--   0        0        0     2746 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/verification.py
+-rw-r--r--   0        0        0      730 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/__init__.py
+-rw-r--r--   0        0        0     3101 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/_api_base.py
+-rw-r--r--   0        0        0     6808 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/_api_base_client.py
+-rw-r--r--   0        0        0     4680 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/_api_client_requests.py
+-rw-r--r--   0        0        0      660 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/_api_client_response.py
+-rw-r--r--   0        0        0      873 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/_api_env.py
+-rw-r--r--   0        0        0     5007 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/_api_errors.py
+-rw-r--r--   0        0        0     1968 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/_events.py
+-rw-r--r--   0        0        0     1547 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/_webhook.py
+-rw-r--r--   0        0        0      552 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/helpers/__init__.py
+-rw-r--r--   0        0        0      742 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/helpers/convert.py
+-rw-r--r--   0        0        0     3566 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/helpers/tool_kit.py
+-rw-r--r--   0        0        0        0 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/metadata/__init__.py
+-rw-r--r--   0        0        0       98 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/metadata/__version__.py
+-rw-r--r--   0        0        0     2334 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/paystack.py
+-rw-r--r--   0        0        0        0 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/utils/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/utils/_compact.py
+-rw-r--r--   0        0        0     2259 2024-05-28 02:58:08.457671 paystackease-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 paystackease-2.2.0/PKG-INFO
```

### Comparing `paystackease-2.1.2/LICENSE` & `paystackease-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/README.md` & `paystackease-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/__init__.py` & `paystackease-2.2.0/paystackease/__init__.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apaystack.py` & `paystackease-2.2.0/paystackease/apaystack.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,78 +23,52 @@
     atransaction_splits,
     atransactions,
     atransfer_recipients,
     atransfers,
     atransfers_control,
     averification,
 )
-from paystackease.core import AsyncRequestAPI
 from paystackease.metadata.__version__ import __version__
 
 
-class AsyncPayStackBase(AsyncRequestAPI):
+class AsyncPayStackBase:
     """AsyncPayStackBase acts as a wrapper around various client APIs to
     interact with the PayStack API
     """
 
     VERSION = __version__
 
     # pylint: disable=too-many-instance-attributes
-    def __init__(self, secret_key=None):
-        super().__init__(secret_key)
-        self.apple_pay = aapple_pay.AsyncApplePayClientAPI(secret_key=secret_key)
-        self.bulk_charges = abulk_charges.AsyncBulkChargesClientAPI(
-            secret_key=secret_key
-        )
-        self.charges = acharges.AsyncChargesClientAPI(secret_key=secret_key)
-        self.customers = acustomers.AsyncCustomerClientAPI(secret_key=secret_key)
-        self.dedicated_virtual_accounts = (
-            adedicated_virtual_accounts.AsyncDedicatedVirtualAccountClientAPI(
-                secret_key=secret_key
-            )
-        )
-        self.disputes = adisputes.AsyncDisputesClientAPI(secret_key=secret_key)
-        self.integration = aintegration.AsyncIntegrationClientAPI(secret_key=secret_key)
-        self.miscellaneous = amiscellaneous.AsyncMiscellaneousClientAPI(
-            secret_key=secret_key
-        )
-        self.payment_pages = apayment_pages.AsyncPaymentPagesClientAPI(
-            secret_key=secret_key
-        )
-        self.payment_requests = apayment_requests.AsyncPaymentRequestClientAPI(
-            secret_key=secret_key
-        )
-        self.plans = aplans.AsyncPlanClientAPI(secret_key=secret_key)
-        self.products = aproducts.AsyncProductClientAPI(secret_key=secret_key)
-        self.refund = arefund.AsyncRefundClientAPI(secret_key=secret_key)
-        self.settlements = asettlements.AsyncSettlementClientAPI(secret_key=secret_key)
-        self.subaccounts = asubaccounts.AsyncSubAccountClientAPI(secret_key=secret_key)
-        self.subscriptions = asubscriptions.AsyncSubscriptionClientAPI(
-            secret_key=secret_key
-        )
-        self.terminal = aterminal.AsyncTerminalClientAPI(secret_key=secret_key)
-        self.transaction_splits = atransaction_splits.AsyncTransactionSplitClientAPI(
-            secret_key=secret_key
-        )
-        self.transactions = atransactions.AsyncTransactionClientAPI(
-            secret_key=secret_key
-        )
-        self.transfer_recipients = (
-            atransfer_recipients.AsyncTransferRecipientsClientAPI(secret_key=secret_key)
-        )
-        self.transfers = atransfers.AsyncTransfersClientAPI(secret_key=secret_key)
-        self.transfer_control = atransfers_control.AsyncTransferControlClientAPI(
-            secret_key=secret_key
-        )
-        self.verification = averification.AsyncVerificationClientAPI(
-            secret_key=secret_key
-        )
+    def __init__(self):
+        self.apple_pay = aapple_pay.AsyncApplePayClientAPI()
+        self.bulk_charges = abulk_charges.AsyncBulkChargesClientAPI()
+        self.charges = acharges.AsyncChargesClientAPI()
+        self.customers = acustomers.AsyncCustomerClientAPI()
+        self.dedicated_virtual_accounts = adedicated_virtual_accounts.AsyncDedicatedVirtualAccountClientAPI()
+        self.disputes = adisputes.AsyncDisputesClientAPI()
+        self.integration = aintegration.AsyncIntegrationClientAPI()
+        self.miscellaneous = amiscellaneous.AsyncMiscellaneousClientAPI()
+        self.payment_pages = apayment_pages.AsyncPaymentPagesClientAPI()
+        self.payment_requests = apayment_requests.AsyncPaymentRequestClientAPI()
+        self.plans = aplans.AsyncPlanClientAPI()
+        self.products = aproducts.AsyncProductClientAPI()
+        self.refund = arefund.AsyncRefundClientAPI()
+        self.settlements = asettlements.AsyncSettlementClientAPI()
+        self.subaccounts = asubaccounts.AsyncSubAccountClientAPI()
+        self.subscriptions = asubscriptions.AsyncSubscriptionClientAPI()
+        self.terminal = aterminal.AsyncTerminalClientAPI()
+        self.transaction_splits = atransaction_splits.AsyncTransactionSplitClientAPI()
+        self.transactions = atransactions.AsyncTransactionClientAPI()
+        self.transfer_recipients = atransfer_recipients.AsyncTransferRecipientsClientAPI()
+        self.transfers = atransfers.AsyncTransfersClientAPI()
+        self.transfer_control = atransfers_control.AsyncTransferControlClientAPI()
+        self.verification = averification.AsyncVerificationClientAPI()
 
     async def __aenter__(self):
-        await super().__aenter__()
+        # await super().__aenter__()
         await self.apple_pay.__aenter__()
         await self.bulk_charges.__aenter__()
         await self.charges.__aenter__()
         await self.customers.__aenter__()
         await self.dedicated_virtual_accounts.__aenter__()
         await self.disputes.__aenter__()
         await self.integration.__aenter__()
@@ -136,8 +110,8 @@
         await self.terminal.__aexit__(*args)
         await self.transaction_splits.__aexit__(*args)
         await self.transactions.__aexit__(*args)
         await self.transfer_recipients.__aexit__(*args)
         await self.transfers.__aexit__(*args)
         await self.transfer_control.__aexit__(*args)
         await self.verification.__aexit__(*args)
-        await super().__aexit__(*args)
+        # await super().__aexit__(*args)
```

### Comparing `paystackease-2.1.2/paystackease/apis/__init__.py` & `paystackease-2.2.0/paystackease/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/aapple_pay.py` & `paystackease-2.2.0/paystackease/apis/async_apis/aapple_pay.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/abulk_charges.py` & `paystackease-2.2.0/paystackease/apis/async_apis/abulk_charges.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/acharges.py` & `paystackease-2.2.0/paystackease/apis/async_apis/acharges.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/acustomers.py` & `paystackease-2.2.0/paystackease/apis/async_apis/acustomers.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/adedicated_virtual_accounts.py` & `paystackease-2.2.0/paystackease/apis/async_apis/adedicated_virtual_accounts.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/adisputes.py` & `paystackease-2.2.0/paystackease/apis/async_apis/adisputes.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/aintegration.py` & `paystackease-2.2.0/paystackease/apis/async_apis/aintegration.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/amiscellaneous.py` & `paystackease-2.2.0/paystackease/apis/async_apis/amiscellaneous.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/apayment_pages.py` & `paystackease-2.2.0/paystackease/apis/async_apis/apayment_pages.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/apayment_requests.py` & `paystackease-2.2.0/paystackease/apis/async_apis/apayment_requests.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/aplans.py` & `paystackease-2.2.0/paystackease/apis/async_apis/aplans.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/aproducts.py` & `paystackease-2.2.0/paystackease/apis/async_apis/aproducts.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/arefund.py` & `paystackease-2.2.0/paystackease/apis/async_apis/arefund.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/asettlements.py` & `paystackease-2.2.0/paystackease/apis/async_apis/asettlements.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/asubaccounts.py` & `paystackease-2.2.0/paystackease/apis/async_apis/asubaccounts.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/asubscriptions.py` & `paystackease-2.2.0/paystackease/apis/async_apis/asubscriptions.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/aterminal.py` & `paystackease-2.2.0/paystackease/apis/async_apis/aterminal.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/atransaction_splits.py` & `paystackease-2.2.0/paystackease/apis/async_apis/atransaction_splits.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/atransactions.py` & `paystackease-2.2.0/paystackease/apis/async_apis/atransactions.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/atransfer_recipients.py` & `paystackease-2.2.0/paystackease/apis/async_apis/atransfer_recipients.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/atransfers.py` & `paystackease-2.2.0/paystackease/apis/async_apis/atransfers.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/atransfers_control.py` & `paystackease-2.2.0/paystackease/apis/async_apis/atransfers_control.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/async_apis/averification.py` & `paystackease-2.2.0/paystackease/apis/async_apis/averification.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/apple_pay.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/apple_pay.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/bulk_charges.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/bulk_charges.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/charges.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/charges.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/customers.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/customers.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/dedicated_virtual_accounts.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/dedicated_virtual_accounts.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/disputes.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/disputes.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/integration.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/integration.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/miscellaneous.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/payment_pages.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/payment_pages.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/payment_requests.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/payment_requests.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/plans.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/plans.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/products.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/products.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/refund.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/refund.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/settlements.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/settlements.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/subaccounts.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/subaccounts.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/subscriptions.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/subscriptions.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/terminal.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/terminal.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/transaction_splits.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/transaction_splits.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/transactions.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/transactions.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/transfer_recipients.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/transfer_recipients.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/transfers.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/transfers.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/transfers_control.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/transfers_control.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/apis/sync_apis/verification.py` & `paystackease-2.2.0/paystackease/apis/sync_apis/verification.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/core/__init__.py` & `paystackease-2.2.0/paystackease/core/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,10 @@
     InvalidRequestMethodError,
     PayStackError,
     PayStackServerError,
     PayStackSignatureVerifyError,
     SecretKeyError,
     TypeValueError,
 )
-from paystackease.core._webhook import PayStackWebhook
+from paystackease.core._webhook import PayStackWebhook, PayStackSignature
+from paystackease.core._events import Event
+from paystackease.core._api_env import EnvConfig
```

### Comparing `paystackease-2.1.2/paystackease/core/_api_base.py` & `paystackease-2.2.0/paystackease/core/_api_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,55 +2,38 @@
 BaseAPI serves as the base for creating client APIs to interact with the Paystack API
 with methods for handling HTTP requests, authentication using a secret key,
 constructing HTTP headers, joining URLs with the API base URL, and logging response information.
 """
 
 import logging
 from abc import ABC, abstractmethod
-
 from datetime import datetime, date
-from typing import Union, Dict, List, Any, Optional
+from typing import Union, Optional, Dict, List, Any
 from urllib.parse import urljoin
-from decouple import config
 
 from paystackease.core._api_client_response import PayStackResponse
-from paystackease.core._api_errors import SecretKeyError, TypeValueError
 
-logger = logging.getLogger(__name__)
+from paystackease.core._api_errors import TypeValueError
+from paystackease.core._api_env import EnvConfig, EnvBase
 
-PAYSTACK_SECRET_KEY = config("PAYSTACK_SECRET_KEY")
+
+logger = logging.getLogger(__name__)
 
 
 class BaseAPI(ABC):
     """Base Client API for Paystack API"""
 
     _PAYSTACK_API_URL: str = "https://api.paystack.co/"
     _VALID_HTTP_METHODS: set[str] = {"GET", "POST", "PUT", "DELETE"}
 
     # pylint: disable=too-few-public-methods
-    def __init__(self, secret_key: str = None) -> None:
+    def __init__(self, secret_key: EnvBase = EnvConfig()) -> None:
         self._secret_key = secret_key
-
-        # Default to PAYSTACK_SECRET_KEY if not provided in the instance
-        if not self._secret_key:
-            self._secret_key = PAYSTACK_SECRET_KEY  # or environment variables
-
-        # Raise an error if PAYSTACK_SECRET_KEY is not set in the instance or environment variables
-        if not self._secret_key:
-            error_message = "Please provide a secret key or set the environment variable PAYSTACK_SECRET_KEY"
-            logger.error(error_message)
-            raise SecretKeyError(error_message)
-
         self._headers = self._make_paystack_http_headers()
 
-    @classmethod
-    def _set_secret_key(cls, secret_key: str) -> None:
-        """Set the secret key for all instances of this class"""
-        cls._secret_key = secret_key
-
     def _join_url(self, path: str) -> str:
         """
         Join URL with Paystack API URL
         :param path:
         :return:
         """
         if path.startswith("/"):
@@ -59,21 +42,21 @@
 
     def _make_paystack_http_headers(self) -> dict:
         """
         Make Paystack HTTP Headers
         :return:
         """
         return {
-            "Authorization": f"Bearer {self._secret_key}",
+            "Authorization": f"Bearer {self._secret_key.secret_key()}",
             "content-type": "application/json",
         }
 
     @staticmethod
     def _convert_to_string(
-        value: Union[bool, date, datetime, None]
+            value: Union[bool, date, datetime, None]
     ) -> Union[str, int, None]:
         """
         Convert the type of value to a string
         :param value: The value to be converted
 
         :raise TypeError: if the value is not a supported type
```

### Comparing `paystackease-2.1.2/paystackease/core/_api_base_client.py` & `paystackease-2.2.0/paystackease/core/_api_base_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,18 +23,17 @@
 
 logger = logging.getLogger(__name__)
 
 
 class SyncBaseClientAPI(BaseAPI):
 
     # pylint: disable=too-few-public-methods
-    def __init__(self, secret_key: str = None) -> None:
-        super().__init__(secret_key)
-
-        self._session = Session()
+    def __init__(self, session: Optional[Session] = None) -> None:
+        super().__init__()
+        self._session = session or Session()
 
     def _request_url(
         self,
         method: str,
         url: str,
         data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
         params: Optional[Union[Dict[str, Any], None]] = None,
@@ -100,19 +99,19 @@
             raise PayStackError(message=error_message, status_code=status_code) from error
 
 
 class AsyncBaseClientAPI(BaseAPI):
     """Base Client API for Paystack API"""
 
     # pylint: disable=too-few-public-methods
-    def __init__(self, secret_key: str = None) -> None:
-        super().__init__(secret_key)
+    def __init__(self, session: Optional[ClientSession] = None, timeout: Optional[ClientTimeout] = None) -> None:
+        super().__init__()
 
-        self.timeout = ClientTimeout(total=30)
-        self._session = ClientSession(
+        self.timeout = timeout or ClientTimeout(total=30)
+        self._session = session or ClientSession(
             headers=self._make_paystack_http_headers(), timeout=self.timeout
         )
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
```

### Comparing `paystackease-2.1.2/paystackease/core/_api_client_requests.py` & `paystackease-2.2.0/paystackease/core/_api_client_requests.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/core/_api_client_response.py` & `paystackease-2.2.0/paystackease/core/_api_client_response.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/core/_api_errors.py` & `paystackease-2.2.0/paystackease/core/_api_errors.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/core/_webhook.py` & `paystackease-2.2.0/paystackease/core/_webhook.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import hmac
 from collections import OrderedDict
 from hashlib import sha512
 from paystackease.core._api_errors import PayStackSignatureVerifyError
+from paystackease.core._events import Event
 
 
 class PayStackWebhook(object):
 
     @staticmethod
     def get_event_data(
             secret_key,
@@ -15,15 +16,16 @@
     ):
         if hasattr(payload_type, 'decode'):
             payload_type = payload_type.decode("utf-8")
 
         PayStackSignature.verify_headers(payload_type, secret_key, signature_header)
 
         data = json.loads(payload_type, object_pairs_hook=lambda pairs: OrderedDict(pairs))
-        return data
+        event = Event._get_event(data)
+        return event
 
 
 class PayStackSignature(object):
     @staticmethod
     def _make_signature(payload, secret_key):
         hash_hex = hmac.new(
             secret_key.encode('utf-8'),
```

### Comparing `paystackease-2.1.2/paystackease/helpers/__init__.py` & `paystackease-2.2.0/paystackease/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/helpers/convert.py` & `paystackease-2.2.0/paystackease/helpers/convert.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/paystackease/helpers/tool_kit.py` & `paystackease-2.2.0/paystackease/helpers/tool_kit.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.2/pyproject.toml` & `paystackease-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paystackease"
-version = "2.1.2"
+version = "2.2.0"
 description = "This is a simple api wrapper that implements both asynchronous and synchronous http requests to interact with Paystack APIs."
 authors = ["Peter Mbachu <doublep098@gmail.com>"]
 maintainers = []
 license = "MIT"
 readme = "README.md"
 keywords = ["paystack", "paystackease", "python", "api", "payment integration"]
 classifiers = [
```

### Comparing `paystackease-2.1.2/PKG-INFO` & `paystackease-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paystackease
-Version: 2.1.2
+Version: 2.2.0
 Summary: This is a simple api wrapper that implements both asynchronous and synchronous http requests to interact with Paystack APIs.
 License: MIT
 Keywords: paystack,paystackease,python,api,payment integration
 Author: Peter Mbachu
 Author-email: doublep098@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

