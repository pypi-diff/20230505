# Comparing `tmp/mercoa-0.0.6.tar.gz` & `tmp/mercoa-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercoa-0.0.6.tar", max compression
+gzip compressed data, was "mercoa-0.0.7.tar", max compression
```

## Comparing `mercoa-0.0.6.tar` & `mercoa-0.0.7.tar`

### file list

```diff
@@ -1,126 +1,137 @@
--rw-r--r--   0        0        0      410 2023-04-20 17:45:56.381406 mercoa-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4363 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/__init__.py
--rw-r--r--   0        0        0     4216 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/client.py
--rw-r--r--   0        0        0      348 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/core/__init__.py
--rw-r--r--   0        0        0      326 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      157 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/environment.py
--rw-r--r--   0        0        0        0 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/py.typed
--rw-r--r--   0        0        0     4472 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/__init__.py
--rw-r--r--   0        0        0      165 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/bank_lookup/__init__.py
--rw-r--r--   0        0        0     2582 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/bank_lookup/client.py
--rw-r--r--   0        0        0      205 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/bank_lookup/types/__init__.py
--rw-r--r--   0        0        0      960 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/bank_lookup/types/bank_address.py
--rw-r--r--   0        0        0      946 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
--rw-r--r--   0        0        0      359 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/__init__.py
--rw-r--r--   0        0        0      148 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      216 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/errors/unauthorized_error.py
--rw-r--r--   0        0        0      407 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/types/__init__.py
--rw-r--r--   0        0        0     1093 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/types/address.py
--rw-r--r--   0        0        0      824 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/types/birth_date.py
--rw-r--r--   0        0        0      994 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/types/full_name.py
--rw-r--r--   0        0        0      850 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/types/individual_government_id.py
--rw-r--r--   0        0        0      857 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/types/itin.py
--rw-r--r--   0        0        0      855 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/types/phone_number.py
--rw-r--r--   0        0        0      856 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/types/ssn.py
--rw-r--r--   0        0        0      141 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/counterparty/__init__.py
--rw-r--r--   0        0        0     4542 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/counterparty/client.py
--rw-r--r--   0        0        0      157 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/counterparty/types/__init__.py
--rw-r--r--   0        0        0     1022 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/counterparty/types/counterparty_response.py
--rw-r--r--   0        0        0      753 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/__init__.py
--rw-r--r--   0        0        0    16466 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/client.py
--rw-r--r--   0        0        0     1104 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/__init__.py
--rw-r--r--   0        0        0      487 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/account_type.py
--rw-r--r--   0        0        0     1535 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/business_profile_request.py
--rw-r--r--   0        0        0     1492 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/business_profile_response.py
--rw-r--r--   0        0        0     1917 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/business_type.py
--rw-r--r--   0        0        0      741 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/ein.py
--rw-r--r--   0        0        0       80 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/entity_id.py
--rw-r--r--   0        0        0     1262 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/entity_request.py
--rw-r--r--   0        0        0     1497 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/entity_response.py
--rw-r--r--   0        0        0     1084 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/entity/types/entity_status.py
--rw-r--r--   0        0        0     1302 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/entity/types/entity_update_request.py
--rw-r--r--   0        0        0     1372 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/entity/types/individual_profile_request.py
--rw-r--r--   0        0        0     1206 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/entity/types/individual_profile_response.py
--rw-r--r--   0        0        0      974 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/entity/types/profile_request.py
--rw-r--r--   0        0        0      981 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/entity/types/profile_response.py
--rw-r--r--   0        0        0      761 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/entity/types/tax_id.py
--rw-r--r--   0        0        0      577 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/__init__.py
--rw-r--r--   0        0        0    12453 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/client.py
--rw-r--r--   0        0        0      826 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/__init__.py
--rw-r--r--   0        0        0     1048 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/create_vendor_request.py
--rw-r--r--   0        0        0      955 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/document_response.py
--rw-r--r--   0        0        0       81 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_id.py
--rw-r--r--   0        0        0     1255 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_line_item_request.py
--rw-r--r--   0        0        0     1182 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_line_item_response.py
--rw-r--r--   0        0        0     3076 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_request.py
--rw-r--r--   0        0        0     3075 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_response.py
--rw-r--r--   0        0        0     1332 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_status.py
--rw-r--r--   0        0        0     1060 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/transaction_response.py
--rw-r--r--   0        0        0     1261 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/transaction_status.py
--rw-r--r--   0        0        0      213 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/ocr/__init__.py
--rw-r--r--   0        0        0     4443 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/ocr/client.py
--rw-r--r--   0        0        0      298 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/ocr/types/__init__.py
--rw-r--r--   0        0        0     1068 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/ocr/types/attachments.py
--rw-r--r--   0        0        0     1969 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/ocr/types/email_ocr_request.py
--rw-r--r--   0        0        0      891 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/ocr/types/ocr_mailbox.py
--rw-r--r--   0        0        0     1234 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/ocr/types/ocr_response.py
--rw-r--r--   0        0        0      881 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/__init__.py
--rw-r--r--   0        0        0     7158 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/client.py
--rw-r--r--   0        0        0     1305 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/__init__.py
--rw-r--r--   0        0        0      981 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/email_log_response.py
--rw-r--r--   0        0        0      932 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/email_provider_request.py
--rw-r--r--   0        0        0      936 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/email_provider_response.py
--rw-r--r--   0        0        0      656 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/email_sender_provider.py
--rw-r--r--   0        0        0     1052 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/email_sender_request.py
--rw-r--r--   0        0        0     1044 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/email_sender_response.py
--rw-r--r--   0        0        0       86 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/organization_id.py
--rw-r--r--   0        0        0     1318 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/organization_request.py
--rw-r--r--   0        0        0     1431 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/organization_response.py
--rw-r--r--   0        0        0     1142 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/payment_methods_request.py
--rw-r--r--   0        0        0     1148 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/payment_methods_response.py
--rw-r--r--   0        0        0      849 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/payment_rail_markup.py
--rw-r--r--   0        0        0      482 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/payment_rail_markup_type.py
--rw-r--r--   0        0        0     1009 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/payment_rail_request.py
--rw-r--r--   0        0        0      797 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/payment_rail_response.py
--rw-r--r--   0        0        0      943 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/__init__.py
--rw-r--r--   0        0        0    12242 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/client.py
--rw-r--r--   0        0        0     1411 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/__init__.py
--rw-r--r--   0        0        0       85 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_account_id.py
--rw-r--r--   0        0        0     1147 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_account_request.py
--rw-r--r--   0        0        0     1318 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_account_response.py
--rw-r--r--   0        0        0      960 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_status.py
--rw-r--r--   0        0        0      632 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_type.py
--rw-r--r--   0        0        0      819 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_brand.py
--rw-r--r--   0        0        0       78 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_id.py
--rw-r--r--   0        0        0     1120 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_request.py
--rw-r--r--   0        0        0     1217 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_response.py
--rw-r--r--   0        0        0      750 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_type.py
--rw-r--r--   0        0        0       79 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/check_id.py
--rw-r--r--   0        0        0     1152 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/check_request.py
--rw-r--r--   0        0        0     1327 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/check_response.py
--rw-r--r--   0        0        0       80 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/custom_id.py
--rw-r--r--   0        0        0     1568 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/custom_payment_method_request.py
--rw-r--r--   0        0        0     1922 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/custom_payment_method_response.py
--rw-r--r--   0        0        0       87 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/payment_method_id.py
--rw-r--r--   0        0        0     1296 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/payment_method_request.py
--rw-r--r--   0        0        0     1508 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/payment_method_response.py
--rw-r--r--   0        0        0     1229 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/payment_method_type.py
--rw-r--r--   0        0        0      425 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method_schema/__init__.py
--rw-r--r--   0        0        0     6115 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method_schema/client.py
--rw-r--r--   0        0        0      589 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/__init__.py
--rw-r--r--   0        0        0     1160 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py
--rw-r--r--   0        0        0      682 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py
--rw-r--r--   0        0        0       93 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_id.py
--rw-r--r--   0        0        0     1249 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py
--rw-r--r--   0        0        0     1468 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py
--rw-r--r--   0        0        0      269 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/representative/__init__.py
--rw-r--r--   0        0        0     8182 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/representative/client.py
--rw-r--r--   0        0        0      381 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/representative/types/__init__.py
--rw-r--r--   0        0        0       88 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/representative/types/representative_id.py
--rw-r--r--   0        0        0     1370 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/representative/types/representative_request.py
--rw-r--r--   0        0        0     1539 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/representative/types/representative_response.py
--rw-r--r--   0        0        0     1100 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/representative/types/responsibilities.py
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 mercoa-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      410 2023-05-05 17:43:49.129647 mercoa-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4757 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/__init__.py
+-rw-r--r--   0        0        0     4619 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/client.py
+-rw-r--r--   0        0        0      348 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/core/__init__.py
+-rw-r--r--   0        0        0      326 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/core/datetime_utils.py
+-rw-r--r--   0        0        0     3507 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      157 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/environment.py
+-rw-r--r--   0        0        0        0 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/py.typed
+-rw-r--r--   0        0        0     4879 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/__init__.py
+-rw-r--r--   0        0        0      165 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/bank_lookup/__init__.py
+-rw-r--r--   0        0        0     2582 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/bank_lookup/client.py
+-rw-r--r--   0        0        0      205 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/bank_lookup/types/__init__.py
+-rw-r--r--   0        0        0      960 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/bank_lookup/types/bank_address.py
+-rw-r--r--   0        0        0      946 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
+-rw-r--r--   0        0        0      359 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/__init__.py
+-rw-r--r--   0        0        0      148 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      407 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0     1093 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/types/address.py
+-rw-r--r--   0        0        0      824 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/types/birth_date.py
+-rw-r--r--   0        0        0      994 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/types/full_name.py
+-rw-r--r--   0        0        0      850 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/types/individual_government_id.py
+-rw-r--r--   0        0        0      857 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/types/itin.py
+-rw-r--r--   0        0        0      855 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      856 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/types/ssn.py
+-rw-r--r--   0        0        0      141 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/counterparty/__init__.py
+-rw-r--r--   0        0        0     4542 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/counterparty/client.py
+-rw-r--r--   0        0        0      157 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/counterparty/types/__init__.py
+-rw-r--r--   0        0        0     1022 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/counterparty/types/counterparty_response.py
+-rw-r--r--   0        0        0      753 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/__init__.py
+-rw-r--r--   0        0        0    18085 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/client.py
+-rw-r--r--   0        0        0     1104 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/__init__.py
+-rw-r--r--   0        0        0      487 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/account_type.py
+-rw-r--r--   0        0        0     1535 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/business_profile_request.py
+-rw-r--r--   0        0        0     1492 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/business_profile_response.py
+-rw-r--r--   0        0        0     1917 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/business_type.py
+-rw-r--r--   0        0        0      741 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/ein.py
+-rw-r--r--   0        0        0       80 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/entity_id.py
+-rw-r--r--   0        0        0     1262 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/entity_request.py
+-rw-r--r--   0        0        0     1497 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/entity_response.py
+-rw-r--r--   0        0        0     1084 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/entity_status.py
+-rw-r--r--   0        0        0     1302 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/entity_update_request.py
+-rw-r--r--   0        0        0     1372 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/individual_profile_request.py
+-rw-r--r--   0        0        0     1206 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/individual_profile_response.py
+-rw-r--r--   0        0        0      974 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/profile_request.py
+-rw-r--r--   0        0        0      981 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/profile_response.py
+-rw-r--r--   0        0        0      761 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/tax_id.py
+-rw-r--r--   0        0        0      207 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity_users/__init__.py
+-rw-r--r--   0        0        0     9662 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity_users/client.py
+-rw-r--r--   0        0        0      281 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity_users/types/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity_users/types/entity_user_id.py
+-rw-r--r--   0        0        0     1100 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity_users/types/entity_user_request.py
+-rw-r--r--   0        0        0     1224 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity_users/types/entity_user_response.py
+-rw-r--r--   0        0        0      695 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    19563 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/client.py
+-rw-r--r--   0        0        0     1012 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/__init__.py
+-rw-r--r--   0        0        0       81 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/comment_id.py
+-rw-r--r--   0        0        0      750 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/comment_request.py
+-rw-r--r--   0        0        0      937 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/comment_response.py
+-rw-r--r--   0        0        0     1048 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/create_vendor_request.py
+-rw-r--r--   0        0        0      955 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/document_response.py
+-rw-r--r--   0        0        0       81 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_id.py
+-rw-r--r--   0        0        0     1253 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_line_item_request.py
+-rw-r--r--   0        0        0     1180 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_line_item_response.py
+-rw-r--r--   0        0        0     3388 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_request.py
+-rw-r--r--   0        0        0     3075 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_response.py
+-rw-r--r--   0        0        0     1332 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_status.py
+-rw-r--r--   0        0        0     1060 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/transaction_response.py
+-rw-r--r--   0        0        0     1261 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/transaction_status.py
+-rw-r--r--   0        0        0      213 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/ocr/__init__.py
+-rw-r--r--   0        0        0     4443 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/ocr/client.py
+-rw-r--r--   0        0        0      298 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/ocr/types/__init__.py
+-rw-r--r--   0        0        0     1068 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/ocr/types/attachments.py
+-rw-r--r--   0        0        0     1969 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/ocr/types/email_ocr_request.py
+-rw-r--r--   0        0        0      891 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/ocr/types/ocr_mailbox.py
+-rw-r--r--   0        0        0     1234 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/ocr/types/ocr_response.py
+-rw-r--r--   0        0        0      983 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/organization/__init__.py
+-rw-r--r--   0        0        0     7449 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/organization/client.py
+-rw-r--r--   0        0        0     1466 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/organization/types/__init__.py
+-rw-r--r--   0        0        0      948 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/organization/types/color_scheme_request.py
+-rw-r--r--   0        0        0      949 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/organization/types/color_scheme_response.py
+-rw-r--r--   0        0        0      981 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/organization/types/email_log_response.py
+-rw-r--r--   0        0        0      932 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/organization/types/email_provider_request.py
+-rw-r--r--   0        0        0      936 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/organization/types/email_provider_response.py
+-rw-r--r--   0        0        0      656 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/email_sender_provider.py
+-rw-r--r--   0        0        0     1052 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/email_sender_request.py
+-rw-r--r--   0        0        0     1044 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/email_sender_response.py
+-rw-r--r--   0        0        0       86 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/organization_id.py
+-rw-r--r--   0        0        0     1463 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/organization_request.py
+-rw-r--r--   0        0        0     1579 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/organization_response.py
+-rw-r--r--   0        0        0     1142 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/payment_methods_request.py
+-rw-r--r--   0        0        0     1148 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/payment_methods_response.py
+-rw-r--r--   0        0        0      849 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/payment_rail_markup.py
+-rw-r--r--   0        0        0      482 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/payment_rail_markup_type.py
+-rw-r--r--   0        0        0     1009 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/payment_rail_request.py
+-rw-r--r--   0        0        0      797 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/payment_rail_response.py
+-rw-r--r--   0        0        0      943 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/__init__.py
+-rw-r--r--   0        0        0    12242 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/client.py
+-rw-r--r--   0        0        0     1411 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_account_id.py
+-rw-r--r--   0        0        0     1297 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_account_request.py
+-rw-r--r--   0        0        0     1318 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_account_response.py
+-rw-r--r--   0        0        0      960 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_status.py
+-rw-r--r--   0        0        0      632 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_type.py
+-rw-r--r--   0        0        0      819 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_brand.py
+-rw-r--r--   0        0        0       78 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_id.py
+-rw-r--r--   0        0        0     1120 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_request.py
+-rw-r--r--   0        0        0     1217 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_response.py
+-rw-r--r--   0        0        0      750 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_type.py
+-rw-r--r--   0        0        0       79 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/check_id.py
+-rw-r--r--   0        0        0     1152 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/check_request.py
+-rw-r--r--   0        0        0     1327 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/check_response.py
+-rw-r--r--   0        0        0       80 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/custom_id.py
+-rw-r--r--   0        0        0     1568 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/custom_payment_method_request.py
+-rw-r--r--   0        0        0     1922 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/custom_payment_method_response.py
+-rw-r--r--   0        0        0       87 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/payment_method_id.py
+-rw-r--r--   0        0        0     1296 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/payment_method_request.py
+-rw-r--r--   0        0        0     1508 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/payment_method_response.py
+-rw-r--r--   0        0        0     1229 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/payment_method_type.py
+-rw-r--r--   0        0        0      425 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method_schema/__init__.py
+-rw-r--r--   0        0        0     6115 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method_schema/client.py
+-rw-r--r--   0        0        0      589 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/__init__.py
+-rw-r--r--   0        0        0     1160 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py
+-rw-r--r--   0        0        0      682 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py
+-rw-r--r--   0        0        0       93 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_id.py
+-rw-r--r--   0        0        0     1249 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py
+-rw-r--r--   0        0        0     1468 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py
+-rw-r--r--   0        0        0      269 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/representative/__init__.py
+-rw-r--r--   0        0        0     8182 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/representative/client.py
+-rw-r--r--   0        0        0      381 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/representative/types/__init__.py
+-rw-r--r--   0        0        0       88 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/representative/types/representative_id.py
+-rw-r--r--   0        0        0     1370 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/representative/types/representative_request.py
+-rw-r--r--   0        0        0     1539 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/representative/types/representative_response.py
+-rw-r--r--   0        0        0     1100 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/representative/types/responsibilities.py
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 mercoa-0.0.7/PKG-INFO
```

### Comparing `mercoa-0.0.6/src/mercoa/__init__.py` & `mercoa-0.0.7/src/mercoa/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,19 @@
     CardId,
     CardRequest,
     CardResponse,
     CardType,
     CheckId,
     CheckRequest,
     CheckResponse,
+    ColorSchemeRequest,
+    ColorSchemeResponse,
+    CommentId,
+    CommentRequest,
+    CommentResponse,
     CounterpartyResponse,
     CreateVendorRequest,
     CustomId,
     CustomPaymentMethodRequest,
     CustomPaymentMethodResponse,
     DocumentResponse,
     Ein,
@@ -41,14 +46,17 @@
     EmailSenderRequest,
     EmailSenderResponse,
     EntityId,
     EntityRequest,
     EntityResponse,
     EntityStatus,
     EntityUpdateRequest,
+    EntityUserId,
+    EntityUserRequest,
+    EntityUserResponse,
     FullName,
     IndividualGovernmentID,
     IndividualProfileRequest,
     IndividualProfileResponse,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
@@ -86,14 +94,15 @@
     TransactionResponse,
     TransactionStatus,
     UnauthorizedError,
     bank_lookup,
     commons,
     counterparty,
     entity,
+    entity_users,
     invoice,
     ocr,
     organization,
     payment_method,
     payment_method_schema,
     representative,
 )
@@ -117,14 +126,19 @@
     "CardId",
     "CardRequest",
     "CardResponse",
     "CardType",
     "CheckId",
     "CheckRequest",
     "CheckResponse",
+    "ColorSchemeRequest",
+    "ColorSchemeResponse",
+    "CommentId",
+    "CommentRequest",
+    "CommentResponse",
     "CounterpartyResponse",
     "CreateVendorRequest",
     "CustomId",
     "CustomPaymentMethodRequest",
     "CustomPaymentMethodResponse",
     "DocumentResponse",
     "Ein",
@@ -136,14 +150,17 @@
     "EmailSenderRequest",
     "EmailSenderResponse",
     "EntityId",
     "EntityRequest",
     "EntityResponse",
     "EntityStatus",
     "EntityUpdateRequest",
+    "EntityUserId",
+    "EntityUserRequest",
+    "EntityUserResponse",
     "FullName",
     "ITIN",
     "IndividualGovernmentID",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
@@ -184,14 +201,15 @@
     "TransactionResponse",
     "TransactionStatus",
     "UnauthorizedError",
     "bank_lookup",
     "commons",
     "counterparty",
     "entity",
+    "entity_users",
     "invoice",
     "ocr",
     "organization",
     "payment_method",
     "payment_method_schema",
     "representative",
 ]
```

### Comparing `mercoa-0.0.6/src/mercoa/client.py` & `mercoa-0.0.7/src/mercoa/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from backports.cached_property import cached_property
 
 from .environment import MercoaEnvironment
 from .resources.bank_lookup.client import AsyncBankLookupClient, BankLookupClient
 from .resources.counterparty.client import AsyncCounterpartyClient, CounterpartyClient
 from .resources.entity.client import AsyncEntityClient, EntityClient
+from .resources.entity_users.client import AsyncEntityUsersClient, EntityUsersClient
 from .resources.invoice.client import AsyncInvoiceClient, InvoiceClient
 from .resources.ocr.client import AsyncOcrClient, OcrClient
 from .resources.organization.client import AsyncOrganizationClient, OrganizationClient
 from .resources.payment_method.client import AsyncPaymentMethodClient, PaymentMethodClient
 from .resources.payment_method_schema.client import AsyncPaymentMethodSchemaClient, PaymentMethodSchemaClient
 from .resources.representative.client import AsyncRepresentativeClient, RepresentativeClient
 
@@ -28,14 +29,18 @@
         return BankLookupClient(environment=self._environment, token=self._token)
 
     @cached_property
     def counterparty(self) -> CounterpartyClient:
         return CounterpartyClient(environment=self._environment, token=self._token)
 
     @cached_property
+    def entity_users(self) -> EntityUsersClient:
+        return EntityUsersClient(environment=self._environment, token=self._token)
+
+    @cached_property
     def entity(self) -> EntityClient:
         return EntityClient(environment=self._environment, token=self._token)
 
     @cached_property
     def invoice(self) -> InvoiceClient:
         return InvoiceClient(environment=self._environment, token=self._token)
 
@@ -72,14 +77,18 @@
         return AsyncBankLookupClient(environment=self._environment, token=self._token)
 
     @cached_property
     def counterparty(self) -> AsyncCounterpartyClient:
         return AsyncCounterpartyClient(environment=self._environment, token=self._token)
 
     @cached_property
+    def entity_users(self) -> AsyncEntityUsersClient:
+        return AsyncEntityUsersClient(environment=self._environment, token=self._token)
+
+    @cached_property
     def entity(self) -> AsyncEntityClient:
         return AsyncEntityClient(environment=self._environment, token=self._token)
 
     @cached_property
     def invoice(self) -> AsyncInvoiceClient:
         return AsyncInvoiceClient(environment=self._environment, token=self._token)
```

### Comparing `mercoa-0.0.6/src/mercoa/core/datetime_utils.py` & `mercoa-0.0.7/src/mercoa/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/core/jsonable_encoder.py` & `mercoa-0.0.7/src/mercoa/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/__init__.py` & `mercoa-0.0.7/src/mercoa/resources/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from . import (
     bank_lookup,
     commons,
     counterparty,
     entity,
+    entity_users,
     invoice,
     ocr,
     organization,
     payment_method,
     payment_method_schema,
     representative,
 )
@@ -28,28 +29,34 @@
     EntityUpdateRequest,
     IndividualProfileRequest,
     IndividualProfileResponse,
     ProfileRequest,
     ProfileResponse,
     TaxID,
 )
+from .entity_users import EntityUserId, EntityUserRequest, EntityUserResponse
 from .invoice import (
+    CommentId,
+    CommentRequest,
+    CommentResponse,
     CreateVendorRequest,
     DocumentResponse,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
     TransactionResponse,
     TransactionStatus,
 )
 from .ocr import Attachments, EmailOcrRequest, OcrMailbox, OCRResponse
 from .organization import (
+    ColorSchemeRequest,
+    ColorSchemeResponse,
     EmailLogResponse,
     EmailProviderRequest,
     EmailProviderResponse,
     EmailSenderProvider,
     EmailSenderRequest,
     EmailSenderResponse,
     OrganizationId,
@@ -112,14 +119,19 @@
     "CardId",
     "CardRequest",
     "CardResponse",
     "CardType",
     "CheckId",
     "CheckRequest",
     "CheckResponse",
+    "ColorSchemeRequest",
+    "ColorSchemeResponse",
+    "CommentId",
+    "CommentRequest",
+    "CommentResponse",
     "CounterpartyResponse",
     "CreateVendorRequest",
     "CustomId",
     "CustomPaymentMethodRequest",
     "CustomPaymentMethodResponse",
     "DocumentResponse",
     "Ein",
@@ -131,14 +143,17 @@
     "EmailSenderRequest",
     "EmailSenderResponse",
     "EntityId",
     "EntityRequest",
     "EntityResponse",
     "EntityStatus",
     "EntityUpdateRequest",
+    "EntityUserId",
+    "EntityUserRequest",
+    "EntityUserResponse",
     "FullName",
     "ITIN",
     "IndividualGovernmentID",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
@@ -178,14 +193,15 @@
     "TransactionResponse",
     "TransactionStatus",
     "UnauthorizedError",
     "bank_lookup",
     "commons",
     "counterparty",
     "entity",
+    "entity_users",
     "invoice",
     "ocr",
     "organization",
     "payment_method",
     "payment_method_schema",
     "representative",
 ]
```

### Comparing `mercoa-0.0.6/src/mercoa/resources/bank_lookup/client.py` & `mercoa-0.0.7/src/mercoa/resources/bank_lookup/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/bank_lookup/types/bank_address.py` & `mercoa-0.0.7/src/mercoa/resources/bank_lookup/types/bank_address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py` & `mercoa-0.0.7/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/commons/types/address.py` & `mercoa-0.0.7/src/mercoa/resources/commons/types/address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/commons/types/birth_date.py` & `mercoa-0.0.7/src/mercoa/resources/commons/types/birth_date.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/commons/types/full_name.py` & `mercoa-0.0.7/src/mercoa/resources/commons/types/full_name.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/commons/types/individual_government_id.py` & `mercoa-0.0.7/src/mercoa/resources/commons/types/individual_government_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/commons/types/itin.py` & `mercoa-0.0.7/src/mercoa/resources/commons/types/itin.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/commons/types/phone_number.py` & `mercoa-0.0.7/src/mercoa/resources/commons/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/commons/types/ssn.py` & `mercoa-0.0.7/src/mercoa/resources/commons/types/ssn.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/counterparty/client.py` & `mercoa-0.0.7/src/mercoa/resources/counterparty/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/counterparty/types/counterparty_response.py` & `mercoa-0.0.7/src/mercoa/resources/counterparty/types/counterparty_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/entity/__init__.py` & `mercoa-0.0.7/src/mercoa/resources/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/entity/client.py` & `mercoa-0.0.7/src/mercoa/resources/entity/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,30 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def plaid_link_token(self, entity_id: EntityId) -> str:
+        _response = httpx.request(
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/plaidLinkToken"),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
+        )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
 
 class AsyncEntityClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
@@ -339,11 +355,28 @@
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def plaid_link_token(self, entity_id: EntityId) -> str:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "GET",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/plaidLinkToken"),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
+            )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mercoa-0.0.6/src/mercoa/resources/entity/types/__init__.py` & `mercoa-0.0.7/src/mercoa/resources/entity/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/entity/types/business_profile_request.py` & `mercoa-0.0.7/src/mercoa/resources/entity/types/business_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/entity/types/business_profile_response.py` & `mercoa-0.0.7/src/mercoa/resources/entity/types/business_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/entity/types/business_type.py` & `mercoa-0.0.7/src/mercoa/resources/entity/types/business_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/entity/types/ein.py` & `mercoa-0.0.7/src/mercoa/resources/entity/types/ein.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/entity/types/entity_request.py` & `mercoa-0.0.7/src/mercoa/resources/entity/types/entity_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/entity/types/entity_response.py` & `mercoa-0.0.7/src/mercoa/resources/entity/types/entity_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/entity/types/entity_status.py` & `mercoa-0.0.7/src/mercoa/resources/entity/types/entity_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/entity/types/entity_update_request.py` & `mercoa-0.0.7/src/mercoa/resources/entity/types/entity_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/entity/types/individual_profile_request.py` & `mercoa-0.0.7/src/mercoa/resources/entity/types/individual_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/entity/types/individual_profile_response.py` & `mercoa-0.0.7/src/mercoa/resources/entity/types/individual_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/entity/types/profile_request.py` & `mercoa-0.0.7/src/mercoa/resources/entity/types/profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/entity/types/profile_response.py` & `mercoa-0.0.7/src/mercoa/resources/entity/types/profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/entity/types/tax_id.py` & `mercoa-0.0.7/src/mercoa/resources/entity/types/tax_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/invoice/__init__.py` & `mercoa-0.0.7/src/mercoa/resources/invoice/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
+    CommentId,
+    CommentRequest,
+    CommentResponse,
     CreateVendorRequest,
     DocumentResponse,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
     TransactionResponse,
     TransactionStatus,
 )
 
 __all__ = [
+    "CommentId",
+    "CommentRequest",
+    "CommentResponse",
     "CreateVendorRequest",
     "DocumentResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceRequest",
     "InvoiceResponse",
```

### Comparing `mercoa-0.0.6/src/mercoa/resources/invoice/client.py` & `mercoa-0.0.7/src/mercoa/resources/entity_users/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,258 +7,194 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
-from .types.document_response import DocumentResponse
-from .types.invoice_id import InvoiceId
-from .types.invoice_request import InvoiceRequest
-from .types.invoice_response import InvoiceResponse
+from ..entity.types.entity_id import EntityId
+from .types.entity_user_id import EntityUserId
+from .types.entity_user_request import EntityUserRequest
+from .types.entity_user_response import EntityUserResponse
 
 
-class InvoiceClient:
+class EntityUsersClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    def create(self, *, request: InvoiceRequest) -> InvoiceResponse:
-        _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "invoice"),
-            json=jsonable_encoder(request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get(self, invoice_id: InvoiceId) -> InvoiceResponse:
+    def get_all(self, entity_id: EntityId) -> typing.List[EntityUserResponse]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/users"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[EntityUserResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(self, invoice_id: InvoiceId, *, request: InvoiceRequest) -> InvoiceResponse:
+    def create(self, entity_id: EntityId, *, request: EntityUserRequest) -> EntityUserResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def delete(self, invoice_id: InvoiceId) -> None:
-        _response = httpx.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
+            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_documents(self, invoice_id: InvoiceId) -> typing.List[DocumentResponse]:
+    def get(self, entity_id: EntityId, user_id: EntityUserId) -> EntityUserResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/documents"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[DocumentResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_vendor_link(self, invoice_id: InvoiceId) -> str:
+    def update(self, entity_id: EntityId, user_id: EntityUserId, *, request: EntityUserRequest) -> EntityUserResponse:
         _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/vendorlink"),
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
+            json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def send_vendor_email(self, invoice_id: InvoiceId) -> None:
+    def delete(self, entity_id: EntityId, user_id: EntityUserId) -> None:
         _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/sendVendorEmail"),
+            "DELETE",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncInvoiceClient:
+class AsyncEntityUsersClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    async def create(self, *, request: InvoiceRequest) -> InvoiceResponse:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "invoice"),
-                json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get(self, invoice_id: InvoiceId) -> InvoiceResponse:
+    async def get_all(self, entity_id: EntityId) -> typing.List[EntityUserResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/users"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[EntityUserResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(self, invoice_id: InvoiceId, *, request: InvoiceRequest) -> InvoiceResponse:
+    async def create(self, entity_id: EntityId, *, request: EntityUserRequest) -> EntityUserResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def delete(self, invoice_id: InvoiceId) -> None:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
+            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_documents(self, invoice_id: InvoiceId) -> typing.List[DocumentResponse]:
+    async def get(self, entity_id: EntityId, user_id: EntityUserId) -> EntityUserResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/documents"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[DocumentResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_vendor_link(self, invoice_id: InvoiceId) -> str:
+    async def update(
+        self, entity_id: EntityId, user_id: EntityUserId, *, request: EntityUserRequest
+    ) -> EntityUserResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/vendorlink"),
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
+                json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def send_vendor_email(self, invoice_id: InvoiceId) -> None:
+    async def delete(self, entity_id: EntityId, user_id: EntityUserId) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/sendVendorEmail"),
+                "DELETE",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         if 200 <= _response.status_code < 300:
             return
         try:
```

### Comparing `mercoa-0.0.6/src/mercoa/resources/invoice/types/__init__.py` & `mercoa-0.0.7/src/mercoa/resources/invoice/types/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from .comment_id import CommentId
+from .comment_request import CommentRequest
+from .comment_response import CommentResponse
 from .create_vendor_request import CreateVendorRequest
 from .document_response import DocumentResponse
 from .invoice_id import InvoiceId
 from .invoice_line_item_request import InvoiceLineItemRequest
 from .invoice_line_item_response import InvoiceLineItemResponse
 from .invoice_request import InvoiceRequest
 from .invoice_response import InvoiceResponse
 from .invoice_status import InvoiceStatus
 from .transaction_response import TransactionResponse
 from .transaction_status import TransactionStatus
 
 __all__ = [
+    "CommentId",
+    "CommentRequest",
+    "CommentResponse",
     "CreateVendorRequest",
     "DocumentResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceRequest",
     "InvoiceResponse",
```

### Comparing `mercoa-0.0.6/src/mercoa/resources/invoice/types/create_vendor_request.py` & `mercoa-0.0.7/src/mercoa/resources/invoice/types/create_vendor_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/invoice/types/document_response.py` & `mercoa-0.0.7/src/mercoa/resources/invoice/types/document_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_line_item_request.py` & `mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_line_item_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             "If provided, will overwrite line item on the invoice with this ID. If not provided, will create a new line item.\n"
         )
     )
     amount: typing.Optional[float]
     currency: typing.Optional[str]
     description: typing.Optional[str]
     name: typing.Optional[str]
-    quantity: typing.Optional[float]
+    quantity: typing.Optional[int]
     unit_price: typing.Optional[float] = pydantic.Field(alias="unitPrice")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_line_item_response.py` & `mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_line_item_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class InvoiceLineItemResponse(pydantic.BaseModel):
     id: str
     amount: typing.Optional[float]
     currency: typing.Optional[str]
     description: typing.Optional[str]
     name: typing.Optional[str]
-    quantity: typing.Optional[float]
+    quantity: typing.Optional[int]
     unit_price: typing.Optional[float] = pydantic.Field(alias="unitPrice")
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_request.py` & `mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,17 +13,21 @@
 from .invoice_status import InvoiceStatus
 
 
 class InvoiceRequest(pydantic.BaseModel):
     status: typing.Optional[InvoiceStatus]
     amount: typing.Optional[float]
     currency: typing.Optional[str]
-    deduction_date: typing.Optional[dt.datetime] = pydantic.Field(alias="deductionDate")
-    funded_date: typing.Optional[dt.datetime] = pydantic.Field(alias="fundedDate")
-    due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate")
+    deduction_date: typing.Optional[dt.datetime] = pydantic.Field(
+        alias="deductionDate", description=("Date when funds will be deducted from payer's account.\n")
+    )
+    funded_date: typing.Optional[dt.datetime] = pydantic.Field(
+        alias="fundedDate", description=("Date of funds settlement.\n")
+    )
+    due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate", description=("Due date of invoice.\n"))
     invoice_number: typing.Optional[str] = pydantic.Field(alias="invoiceNumber")
     note_to_self: typing.Optional[str] = pydantic.Field(alias="noteToSelf")
     service_start_date: typing.Optional[dt.datetime] = pydantic.Field(alias="serviceStartDate")
     service_end_date: typing.Optional[dt.datetime] = pydantic.Field(alias="serviceEndDate")
     payer_id: typing.Optional[EntityId] = pydantic.Field(alias="payerId")
     payment_source_id: typing.Optional[PaymentMethodId] = pydantic.Field(alias="paymentSourceId")
     vendor_id: typing.Optional[EntityId] = pydantic.Field(alias="vendorId")
@@ -37,15 +41,18 @@
     update_vendor: typing.Optional[CreateVendorRequest] = pydantic.Field(
         alias="updateVendor",
         description=(
             "When paying to an existing vendor with an incomplete profile, use the updateVendor object. Mercoa will update the vendor entity tied to this invoice. This object is ignored if the vendor already has already been created with complete information and when creating a new invoice.\n"
         ),
     )
     line_items: typing.Optional[typing.List[InvoiceLineItemRequest]] = pydantic.Field(alias="lineItems")
-    uploaded_image: typing.Optional[str] = pydantic.Field(alias="uploadedImage")
+    uploaded_image: typing.Optional[str] = pydantic.Field(
+        alias="uploadedImage",
+        description=("Base64 encoded image or PDF of invoice. PNG, JPG, and PDF are supported. 10MB max.\n"),
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_response.py` & `mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_status.py` & `mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/invoice/types/transaction_response.py` & `mercoa-0.0.7/src/mercoa/resources/invoice/types/transaction_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/invoice/types/transaction_status.py` & `mercoa-0.0.7/src/mercoa/resources/invoice/types/transaction_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/ocr/client.py` & `mercoa-0.0.7/src/mercoa/resources/ocr/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/ocr/types/attachments.py` & `mercoa-0.0.7/src/mercoa/resources/ocr/types/attachments.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/ocr/types/email_ocr_request.py` & `mercoa-0.0.7/src/mercoa/resources/ocr/types/email_ocr_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/ocr/types/ocr_mailbox.py` & `mercoa-0.0.7/src/mercoa/resources/ocr/types/ocr_mailbox.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/ocr/types/ocr_response.py` & `mercoa-0.0.7/src/mercoa/resources/ocr/types/ocr_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/organization/client.py` & `mercoa-0.0.7/src/mercoa/resources/organization/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,20 +22,24 @@
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
     def get(
-        self, *, payment_methods: typing.Optional[bool] = None, email_provider: typing.Optional[bool] = None
+        self,
+        *,
+        payment_methods: typing.Optional[bool] = None,
+        email_provider: typing.Optional[bool] = None,
+        color_scheme: typing.Optional[bool] = None,
     ) -> OrganizationResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "organization"),
-            params={"paymentMethods": payment_methods, "emailProvider": email_provider},
+            params={"paymentMethods": payment_methods, "emailProvider": email_provider, "colorScheme": color_scheme},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -88,21 +92,29 @@
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
     async def get(
-        self, *, payment_methods: typing.Optional[bool] = None, email_provider: typing.Optional[bool] = None
+        self,
+        *,
+        payment_methods: typing.Optional[bool] = None,
+        email_provider: typing.Optional[bool] = None,
+        color_scheme: typing.Optional[bool] = None,
     ) -> OrganizationResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "organization"),
-                params={"paymentMethods": payment_methods, "emailProvider": email_provider},
+                params={
+                    "paymentMethods": payment_methods,
+                    "emailProvider": email_provider,
+                    "colorScheme": color_scheme,
+                },
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
```

### Comparing `mercoa-0.0.6/src/mercoa/resources/organization/types/__init__.py` & `mercoa-0.0.7/src/mercoa/resources/organization/types/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from .color_scheme_request import ColorSchemeRequest
+from .color_scheme_response import ColorSchemeResponse
 from .email_log_response import EmailLogResponse
 from .email_provider_request import EmailProviderRequest
 from .email_provider_response import EmailProviderResponse
 from .email_sender_provider import EmailSenderProvider
 from .email_sender_request import EmailSenderRequest
 from .email_sender_response import EmailSenderResponse
 from .organization_id import OrganizationId
@@ -13,14 +15,16 @@
 from .payment_methods_response import PaymentMethodsResponse
 from .payment_rail_markup import PaymentRailMarkup
 from .payment_rail_markup_type import PaymentRailMarkupType
 from .payment_rail_request import PaymentRailRequest
 from .payment_rail_response import PaymentRailResponse
 
 __all__ = [
+    "ColorSchemeRequest",
+    "ColorSchemeResponse",
     "EmailLogResponse",
     "EmailProviderRequest",
     "EmailProviderResponse",
     "EmailSenderProvider",
     "EmailSenderRequest",
     "EmailSenderResponse",
     "OrganizationId",
```

### Comparing `mercoa-0.0.6/src/mercoa/resources/organization/types/email_log_response.py` & `mercoa-0.0.7/src/mercoa/resources/organization/types/email_log_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/organization/types/email_provider_request.py` & `mercoa-0.0.7/src/mercoa/resources/organization/types/email_provider_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/organization/types/email_provider_response.py` & `mercoa-0.0.7/src/mercoa/resources/organization/types/email_provider_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/organization/types/email_sender_provider.py` & `mercoa-0.0.7/src/mercoa/resources/organization/types/email_sender_provider.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/organization/types/email_sender_request.py` & `mercoa-0.0.7/src/mercoa/resources/organization/types/email_sender_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/organization/types/email_sender_response.py` & `mercoa-0.0.7/src/mercoa/resources/organization/types/email_sender_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/organization/types/organization_request.py` & `mercoa-0.0.7/src/mercoa/resources/organization/types/organization_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from .color_scheme_request import ColorSchemeRequest
 from .email_provider_request import EmailProviderRequest
 from .payment_methods_request import PaymentMethodsRequest
 
 
 class OrganizationRequest(pydantic.BaseModel):
     name: typing.Optional[str]
     logo: typing.Optional[str]
     website_url: typing.Optional[str] = pydantic.Field(alias="websiteUrl")
     support_email: typing.Optional[str] = pydantic.Field(alias="supportEmail")
     payment_methods: typing.Optional[PaymentMethodsRequest] = pydantic.Field(alias="paymentMethods")
     email_provider: typing.Optional[EmailProviderRequest] = pydantic.Field(alias="emailProvider")
+    color_scheme: typing.Optional[ColorSchemeRequest] = pydantic.Field(alias="colorScheme")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.6/src/mercoa/resources/organization/types/organization_response.py` & `mercoa-0.0.7/src/mercoa/resources/organization/types/organization_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from .color_scheme_response import ColorSchemeResponse
 from .email_provider_response import EmailProviderResponse
 from .organization_id import OrganizationId
 from .payment_methods_response import PaymentMethodsResponse
 
 
 class OrganizationResponse(pydantic.BaseModel):
     id: OrganizationId
     sandbox: bool
     name: str
     logo_url: typing.Optional[str] = pydantic.Field(alias="logoUrl")
     website_url: typing.Optional[str] = pydantic.Field(alias="websiteUrl")
     support_email: typing.Optional[str] = pydantic.Field(alias="supportEmail")
     payment_methods: typing.Optional[PaymentMethodsResponse] = pydantic.Field(alias="paymentMethods")
     email_provider: typing.Optional[EmailProviderResponse] = pydantic.Field(alias="emailProvider")
+    color_scheme: typing.Optional[ColorSchemeResponse] = pydantic.Field(alias="colorScheme")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.6/src/mercoa/resources/organization/types/payment_methods_request.py` & `mercoa-0.0.7/src/mercoa/resources/organization/types/payment_methods_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/organization/types/payment_methods_response.py` & `mercoa-0.0.7/src/mercoa/resources/organization/types/payment_methods_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/organization/types/payment_rail_markup.py` & `mercoa-0.0.7/src/mercoa/resources/organization/types/payment_rail_markup.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/organization/types/payment_rail_request.py` & `mercoa-0.0.7/src/mercoa/resources/organization/types/payment_rail_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/organization/types/payment_rail_response.py` & `mercoa-0.0.7/src/mercoa/resources/organization/types/payment_rail_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/__init__.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/client.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/types/__init__.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_account_request.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_account_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 
 class BankAccountRequest(pydantic.BaseModel):
     id: typing.Optional[BankAccountId]
     bank_name: str = pydantic.Field(alias="bankName")
     routing_number: str = pydantic.Field(alias="routingNumber")
     account_number: str = pydantic.Field(alias="accountNumber")
+    plaid_public_token: typing.Optional[str] = pydantic.Field(
+        alias="plaidPublicToken", description=("Public token from Plaid Link\n")
+    )
     account_type: BankType = pydantic.Field(alias="accountType")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_account_response.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_account_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_status.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_type.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_brand.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_brand.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_request.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_response.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_type.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/types/check_request.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/types/check_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/types/check_response.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/types/check_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/types/custom_payment_method_request.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/types/custom_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/types/custom_payment_method_response.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/types/custom_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/types/payment_method_request.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/types/payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/types/payment_method_response.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/types/payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method/types/payment_method_type.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method/types/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method_schema/client.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method_schema/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/__init__.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py` & `mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/representative/client.py` & `mercoa-0.0.7/src/mercoa/resources/representative/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/representative/types/representative_request.py` & `mercoa-0.0.7/src/mercoa/resources/representative/types/representative_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/representative/types/representative_response.py` & `mercoa-0.0.7/src/mercoa/resources/representative/types/representative_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/src/mercoa/resources/representative/types/responsibilities.py` & `mercoa-0.0.7/src/mercoa/resources/representative/types/responsibilities.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.6/PKG-INFO` & `mercoa-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercoa
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

